# Comparing `tmp/parsagon-0.8.1.tar.gz` & `tmp/parsagon-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.8.1.tar", last modified: Tue Jul 25 06:04:52 2023, max compression
+gzip compressed data, was "parsagon-0.9.0.tar", last modified: Sun Jul 30 03:09:47 2023, max compression
```

## Comparing `parsagon-0.8.1.tar` & `parsagon-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.838197 parsagon-0.8.1/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 06:04:52.837869 parsagon-0.8.1/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.8.1/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-25 06:04:15.000000 parsagon-0.8.1/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-25 06:04:52.838300 parsagon-0.8.1/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.823145 parsagon-0.8.1/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.1/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.830641 parsagon-0.8.1/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     4677 2023-07-25 05:41:45.000000 parsagon-0.8.1/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.8.1/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    11483 2023-07-25 05:49:16.000000 parsagon-0.8.1/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-25 03:32:53.000000 parsagon-0.8.1/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.8.1/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.837192 parsagon-0.8.1/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.1/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.833742 parsagon-0.8.1/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      646 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.528297 parsagon-0.9.0/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-30 03:09:47.527944 parsagon-0.9.0/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.0/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-30 03:09:01.000000 parsagon-0.9.0/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-30 03:09:47.528396 parsagon-0.9.0/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.515199 parsagon-0.9.0/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.0/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.519436 parsagon-0.9.0/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     4660 2023-07-30 02:20:05.000000 parsagon-0.9.0/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.0/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    12172 2023-07-30 02:56:40.000000 parsagon-0.9.0/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-25 03:32:53.000000 parsagon-0.9.0/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.0/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.527061 parsagon-0.9.0/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.0/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.0/src/parsagon/tests/test_executor.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.522699 parsagon-0.9.0/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      682 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.8.1/PKG-INFO` & `parsagon-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.8.1
+Version: 0.9.0
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.8.1/README.md` & `parsagon-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/pyproject.toml` & `parsagon-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.8.1"
+version = "0.9.0"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.8.1/src/parsagon/api.py` & `parsagon-0.9.0/src/parsagon/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,23 +76,23 @@
         httpx.post,
         "/transformers/get-nav-elem/",
         json={"html": marked_html, "elem_type": elem_type, "description": description},
     )["id"]
     return result
 
 
-def scrape_page(url, html, schema):
+def scrape_page(html, schema):
     """
     Scrapes data from the provided page HTML - data will be returned in the schema provided.
     :param url: url of the page to scrape.
     :param html: HTML of the page to scrape.
     :param schema: Schema of the data to scrape
     :return: Scraped data, with lists truncated.
     """
-    return _api_call(httpx.post, "/transformers/get-custom-data/", json={"url": url, "html": html, "schema": schema})
+    return _api_call(httpx.post, "/transformers/get-custom-data/", json={"html": html, "schema": schema})
 
 
 def create_pipeline(name, description, program_sketch):
     return _api_call(
         httpx.post, "/pipelines/", json={"name": name, "description": description, "program_sketch": program_sketch}
     )
```

### Comparing `parsagon-0.8.1/src/parsagon/custom_function.py` & `parsagon-0.9.0/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon/exceptions.py` & `parsagon-0.9.0/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon/executor.py` & `parsagon-0.9.0/src/parsagon/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import time
+from urllib.parse import urljoin
 
 import lxml.html
 from pyvirtualdisplay import Display
 from selenium import webdriver
 import seleniumwire.undetected_chromedriver as uc
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
@@ -70,19 +71,30 @@
             "let elemIdx = 0; for (const node of document.all) { node.setAttribute('data-psgn-id', elemIdx); elemIdx++; } return elemIdx;"
         )
         self.driver.execute_script(
             "for (const image of document.images) { image.setAttribute('data-psgn-width', image.width ?? -1); image.setAttribute('data-psgn-height', image.height ?? -1); }"
         )
 
     def _get_cleaned_lxml_root(self):
-        driver = self.driver
-        html = driver.page_source
-
         parser = lxml.html.HTMLParser(remove_comments=True, remove_pis=True)
-        root = lxml.html.fromstring(html, parser=parser)
+        root = lxml.html.fromstring(self.driver.page_source.replace('&nbsp;', ' '), parser=parser)
+
+        # make links absolute
+        root.make_links_absolute(self.driver.current_url)
+        for elem in root.xpath('//img[@srcset]'):
+            srcset_list = []
+            for s in elem.get('srcset').split(','):
+                parts = s.strip().split()
+                if not parts:
+                    continue
+                parts[0] = urljoin(self.driver.current_url, parts[0])
+                srcset_list.append(' '.join(parts))
+            elem.set('srcset', ', '.join(srcset_list))
+
+        # remove unnecessary and bulky elements
         for elem in root.iterfind(".//script"):
             elem.text = ""
         for elem in root.iterfind(".//noscript"):
             elem.text = ""
         for elem in root.iterfind(".//style"):
             elem.text = ""
         return root
@@ -184,14 +196,15 @@
         self.mark_html()
         custom_function = CustomFunction(
             "click_elem",
             arguments={},
             examples=[
                 {
                     "html": html,
+                    "url": self.driver.current_url,
                     "elem_id": elem_id,
                 }
             ],
         )
         self.add_custom_function(call_id, custom_function)
         return True
 
@@ -218,14 +231,15 @@
             "select_option",
             arguments={
                 "option": option,
             },
             examples=[
                 {
                     "html": html,
+                    "url": self.driver.current_url,
                     "elem_id": elem_id,
                 }
             ],
         )
         self.add_custom_function(call_id, custom_function)
         return True
 
@@ -256,14 +270,15 @@
             arguments={
                 "text": text,
                 "enter": enter,
             },
             examples=[
                 {
                     "html": html,
+                    "url": self.driver.current_url,
                     "elem_id": elem_id,
                 }
             ],
         )
         self.add_custom_function(call_id, custom_function)
         return True
 
@@ -283,15 +298,15 @@
     def scrape_data(self, schema, window_id, call_id):
         """
         Scrapes data from the current page.
         """
         self.driver.switch_to.window(window_id)
         logger.info("Scraping data...")
         html = self.get_scrape_html()
-        result = scrape_page(self.driver.current_url, html, schema)
+        result = scrape_page(html, schema)
         scraped_data = result["data"]
         nodes = result["nodes"]
         if not scraped_data and not nodes:
             raise ParsagonException(
                 f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt."
             )
         elif not nodes:
```

### Comparing `parsagon-0.8.1/src/parsagon/main.py` & `parsagon-0.9.0/src/parsagon/main.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon/settings.py` & `parsagon-0.9.0/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon/tests/api_mocks.py` & `parsagon-0.9.0/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.9.0/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.9.0/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.1/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.9.0/src/parsagon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.8.1
+Version: 0.9.0
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.8.1/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.9.0/src/parsagon.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 src/parsagon.egg-info/entry_points.txt
 src/parsagon.egg-info/requires.txt
 src/parsagon.egg-info/top_level.txt
 src/parsagon/tests/__init__.py
 src/parsagon/tests/api_mocks.py
 src/parsagon/tests/cli_mocks.py
 src/parsagon/tests/conftest.py
+src/parsagon/tests/test_executor.py
 src/parsagon/tests/test_invalid_args.py
 src/parsagon/tests/test_pipeline_operations.py
```

