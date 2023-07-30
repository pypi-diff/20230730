# Comparing `tmp/webagt-0.1.1.tar.gz` & `tmp/webagt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webagt-0.1.1.tar", max compression
+gzip compressed data, was "webagt-0.1.2.tar", max compression
```

## Comparing `webagt-0.1.1.tar` & `webagt-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1107 2023-01-27 05:32:12.718398 webagt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    21064 2023-01-27 00:43:56.548287 webagt-0.1.1/webagt.py
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 webagt-0.1.1/setup.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 webagt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-07-30 01:55:59.317545 webagt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    21514 2023-07-30 01:54:37.660259 webagt-0.1.2/webagt.py
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 webagt-0.1.2/setup.py
+-rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 webagt-0.1.2/PKG-INFO
```

### Comparing `webagt-0.1.1/pyproject.toml` & `webagt-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webagt"
-version = "0.1.1"
+version = "0.1.2"
 description = "a web agent"
 homepage = "https://ragt.ag/code/webagt"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
 
 [tool.poetry.scripts]
 webagt = "web.__main__:main"
```

### Comparing `webagt-0.1.1/webagt.py` & `webagt-0.1.2/webagt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""A web client."""
+"""A web agent."""
 
 import json
 import pathlib
 import re
 import time
+from pprint import pprint
 
 import lxml.etree
 import lxml.html
 
 try:
     import pyscreenshot
 except ImportError:  # legacy OSX 10.x
     pass
 import mf
 import pyvirtualdisplay
 import requests
 import selenium
 import sqlyte
+import txt
 from easyuri import URI
 from easyuri import parse as uri
 from requests.exceptions import ConnectionError, SSLError
 from selenium import webdriver
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.firefox.service import Service as FirefoxService
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.ui import WebDriverWait
 from webdriver_manager.firefox import GeckoDriverManager
 
-# from .util import dump
-
 __all__ = [
     "post",
     "get",
     "put",
     "delete",
     "parse",
     "agent",
@@ -43,14 +43,15 @@
     "download",
     "ConnectionError",
     "SSLError",
     "uri",
     "URI",
 ]
 
+main = txt.application("webagt", __doc__)
 displays = []
 browsers = []
 
 tor_proxies = {"http": "socks5h://localhost:9150", "https": "socks5h://localhost:9150"}
 
 
 def post(url, **kwargs):
@@ -72,18 +73,19 @@
     """Delete from the web."""
     return Transaction(url, "delete", **kwargs)
 
 
 def download(url, filepath, chunk_size=1024):
     """Download url to filepath."""
     transaction = get(url, stream=True)
-    with pathlib.Path(filepath).open("wb") as fp:
-        for chunk in transaction.response.iter_content(chunk_size=chunk_size):
-            if chunk:
-                fp.write(chunk)
+    if transaction.ok:
+        with pathlib.Path(filepath).open("wb") as fp:
+            for chunk in transaction.response.iter_content(chunk_size=chunk_size):
+                if chunk:
+                    fp.write(chunk)
     return transaction
 
 
 def request(method, url, session=None, **kwargs):
     """
     Return the response to dereferencing given `url` using given `method`.
 
@@ -152,14 +154,15 @@
             _headers["accept"] = accept_header
             if headers:
                 _headers.update(headers)
             self.url, self.response = request(
                 method, self.url, session=session, headers=_headers, **kwargs
             )
             self.status = self.response.status_code
+            self.ok = self.response.ok
             self.text = self.response.text
             self.headers = self.response.headers
         # self.url = str(self.url)
 
     def __repr__(self):
         return f"<web.agent.Transaction object for {self.url}>"
 
@@ -215,45 +218,45 @@
 
     @property
     def mf2json(self):
         return Semantics(mf.parse(Document(self.text, self.url).html, self.url))
 
     @property
     def card(self):
-        return Semantics(mf.representative_card(self.mf2json.data, str(self.url)))
+        return Semantics(mf.util.representative_card(self.mf2json.data, str(self.url)))
 
     @property
     def feed(self):
-        # feed = mf.interpret_feed(self.mf2json.data, source_url=str(self.url))
+        # feed = mf.util.interpret_feed(self.mf2json.data, source_url=str(self.url))
         # for entry in feed["entries"]:
-        #     entry["post-type"] = mf.discover_post_type(entry)
+        #     entry["post-type"] = mf.util.discover_post_type(entry)
         # return Semantics(feed)
         return Semantics(
-            mf.representative_feed(self.mf2json.data, str(self.url), self.dom)
+            mf.util.representative_feed(self.mf2json.data, str(self.url), self.dom)
         )
 
     @property
     def entry(self):
-        return Semantics(mf.interpret_entry(self.mf2json.data, str(self.url)))
+        return Semantics(mf.util.interpret_entry(self.mf2json.data, str(self.url)))
 
     @property
     def event(self):
         return Semantics(
-            mf.interpret_event(self.mf2json.data, source_url=str(self.url))
+            mf.util.interpret_event(self.mf2json.data, source_url=str(self.url))
         )
 
     def mention(self, *target_urls):
         return Semantics(
-            mf.interpret_comment(self.mf2json.data, str(self.url), target_urls)
+            mf.util.interpret_comment(self.mf2json.data, str(self.url), target_urls)
         )
 
     # @property
     # def jf2(self):
-    #     return Semantics(mf.interpret_feed(self.mf2json.data,
-    #                                        source_url=self.url))
+    #     return Semantics(mf.util.interpret_feed(self.mf2json.data,
+    #                                             source_url=self.url))
 
 
 class Semantics:
     def __init__(self, data):
         self.data = data
 
     def __getitem__(self, item):
@@ -609,18 +612,18 @@
             wait.until(condition)
 
     def wait_until_url_contains(self, url):
         # XXX self.wait(self.EC.url_contains(apply_dns(url)))
         self.wait(self.EC.url_contains(url))
 
     def select(self, selector):
-        return self.browser.find_elements_by_css_selector(selector)
+        return self.browser.find_element(By.CSS_SELECTOR, selector)
 
     def select_first(self, selector):
-        return self.browser.find_element_by_css_selector(selector)
+        return self.browser.find_elements(By.CSS_SELECTOR, selector)
 
     def action(self):
         return ActionChains(self.browser)
 
     def shot(self, path):
         # TODO take in pieces & stitch together -- using way too much memory
         # self._height = self.browser.execute_script("return document.body."
@@ -689,7 +692,19 @@
 #         height = browser.execute_script("return document.body.scrollHeight;")
 #         browser.set_window_size(browser_width, height + 100)
 #         browser.get_screenshot_as_file(str(build_dir / "features" /
 #                                            shot_filename))
 #     features.append((test_case, shot_id, dashed_name, name, description))
 #     # XXX , shot_filename, [user for u in browsers.keys()]))
 #     shot_counter += 1
+
+
+@main.register()
+class Parse:
+    """Get a resource and parse it for Microformats."""
+
+    def setup(self, add_arg):
+        add_arg("uri", help="address of the resource")
+
+    def run(self, stdin, log):
+        pprint(webagt.get(self.uri).mf2json.data)
+        return 0
```

### Comparing `webagt-0.1.1/setup.py` & `webagt-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'webdriver-manager>=3.8.5,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['webagt = web.__main__:main']}
 
 setup_kwargs = {
     'name': 'webagt',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'a web agent',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/webagt',
```

### Comparing `webagt-0.1.1/PKG-INFO` & `webagt-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webagt
-Version: 0.1.1
+Version: 0.1.2
 Summary: a web agent
 Home-page: https://ragt.ag/code/webagt
 License: BSD-2-Clause
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: BSD License
```

