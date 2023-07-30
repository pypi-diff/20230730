# Comparing `tmp/md_translate-3.0.2.tar.gz` & `tmp/md_translate-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_translate-3.0.2.tar", max compression
+gzip compressed data, was "md_translate-3.0.3.tar", max compression
```

## Comparing `md_translate-3.0.2.tar` & `md_translate-3.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-06 15:27:15.366243 md_translate-3.0.2/LICENSE
--rw-r--r--   0        0        0     5353 2023-06-06 15:27:15.366243 md_translate-3.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/__init__.py
--rw-r--r--   0        0        0     4457 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/application.py
--rw-r--r--   0        0        0      230 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/blocks.py
--rw-r--r--   0        0        0     5960 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/document.py
--rw-r--r--   0        0        0     3654 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/parser.py
--rw-r--r--   0        0        0      905 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/exceptions.py
--rw-r--r--   0        0        0      737 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/main.py
--rw-r--r--   0        0        0      157 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/settings/__init__.py
--rw-r--r--   0        0        0     5931 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/settings/_base_settings.py
--rw-r--r--   0        0        0     2687 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/settings/_settings_to_cli.py
--rw-r--r--   0        0        0      439 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/__init__.py
--rw-r--r--   0        0        0      687 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/_base_translator.py
--rw-r--r--   0        0        0     4960 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/_selenium_base.py
--rw-r--r--   0        0        0     1517 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/bing.py
--rw-r--r--   0        0        0     2059 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/deepl.py
--rw-r--r--   0        0        0     1839 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/google.py
--rw-r--r--   0        0        0        0 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/randomizer/__init__.py
--rw-r--r--   0        0        0     6618 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/randomizer/const.py
--rw-r--r--   0        0        0     1107 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/randomizer/randomizer.py
--rw-r--r--   0        0        0     1675 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/yandex.py
--rw-r--r--   0        0        0     2214 2023-06-06 15:27:15.366243 md_translate-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 md_translate-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-30 14:17:36.288505 md_translate-3.0.3/LICENSE
+-rw-r--r--   0        0        0     5353 2023-07-30 14:17:36.288505 md_translate-3.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/__init__.py
+-rw-r--r--   0        0        0     4457 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/application.py
+-rw-r--r--   0        0        0      230 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/document/__init__.py
+-rw-r--r--   0        0        0     6485 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/document/blocks.py
+-rw-r--r--   0        0        0     5960 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/document/document.py
+-rw-r--r--   0        0        0     3654 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/document/parser.py
+-rw-r--r--   0        0        0      905 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/exceptions.py
+-rw-r--r--   0        0        0      737 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/main.py
+-rw-r--r--   0        0        0      157 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/settings/__init__.py
+-rw-r--r--   0        0        0     5931 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/settings/_base_settings.py
+-rw-r--r--   0        0        0     2687 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/settings/_settings_to_cli.py
+-rw-r--r--   0        0        0      439 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/__init__.py
+-rw-r--r--   0        0        0      687 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/_base_translator.py
+-rw-r--r--   0        0        0     4999 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/_selenium_base.py
+-rw-r--r--   0        0        0     1517 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/bing.py
+-rw-r--r--   0        0        0     2059 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/deepl.py
+-rw-r--r--   0        0        0     1839 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/google.py
+-rw-r--r--   0        0        0        0 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/randomizer/__init__.py
+-rw-r--r--   0        0        0     6618 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/randomizer/const.py
+-rw-r--r--   0        0        0     1107 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/randomizer/randomizer.py
+-rw-r--r--   0        0        0     1675 2023-07-30 14:17:36.288505 md_translate-3.0.3/md_translate/translators/yandex.py
+-rw-r--r--   0        0        0     2214 2023-07-30 14:17:36.288505 md_translate-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 md_translate-3.0.3/PKG-INFO
```

### Comparing `md_translate-3.0.2/LICENSE` & `md_translate-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/README.md` & `md_translate-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/application.py` & `md_translate-3.0.3/md_translate/application.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/document/blocks.py` & `md_translate-3.0.3/md_translate/document/blocks.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/document/document.py` & `md_translate-3.0.3/md_translate/document/document.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/document/parser.py` & `md_translate-3.0.3/md_translate/document/parser.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/exceptions.py` & `md_translate-3.0.3/md_translate/exceptions.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/main.py` & `md_translate-3.0.3/md_translate/main.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/settings/_base_settings.py` & `md_translate-3.0.3/md_translate/settings/_base_settings.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/settings/_settings_to_cli.py` & `md_translate-3.0.3/md_translate/settings/_settings_to_cli.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/_base_translator.py` & `md_translate-3.0.3/md_translate/translators/_base_translator.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/_selenium_base.py` & `md_translate-3.0.3/md_translate/translators/_selenium_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import urllib.parse
 from typing import TYPE_CHECKING, Any, Optional
 
 import requests
 from selenium import webdriver
 from selenium.common.exceptions import NoSuchElementException
-from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.wait import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 
 from md_translate.translators._base_translator import BaseTranslator
 from md_translate.translators.randomizer.randomizer import Randomizer
@@ -48,15 +48,15 @@
         self.from_language = settings.from_lang
         self.to_language = settings.to_lang
         self.randomizer = Randomizer()
 
     def __enter__(self) -> 'BaseTranslator':
         options = self.randomizer.make_options()
         self._driver = webdriver.Chrome(  # type: ignore
-            service=Service(ChromeDriverManager().install()), options=options
+            service=ChromeService(ChromeDriverManager(version='latest').install()), options=options
         )
         return self
 
     def __exit__(self, *args: Any, **kwargs: Any) -> None:
         self._driver.quit()
 
     def translate(self, *, text: str) -> str:
```

### Comparing `md_translate-3.0.2/md_translate/translators/bing.py` & `md_translate-3.0.3/md_translate/translators/bing.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/deepl.py` & `md_translate-3.0.3/md_translate/translators/deepl.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/google.py` & `md_translate-3.0.3/md_translate/translators/google.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/randomizer/const.py` & `md_translate-3.0.3/md_translate/translators/randomizer/const.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/randomizer/randomizer.py` & `md_translate-3.0.3/md_translate/translators/randomizer/randomizer.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/md_translate/translators/yandex.py` & `md_translate-3.0.3/md_translate/translators/yandex.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.2/pyproject.toml` & `md_translate-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md_translate"
-version = "3.0.2"
+version = "3.0.3"
 description = "CLI tool to translate markdown files"
 authors = ["Ilya Chichak <ilyachch@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/ilyachch/md_docs-trans-app"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `md_translate-3.0.2/PKG-INFO` & `md_translate-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-translate
-Version: 3.0.2
+Version: 3.0.3
 Summary: CLI tool to translate markdown files
 Home-page: https://github.com/ilyachch/md_docs-trans-app
 License: MIT
 Author: Ilya Chichak
 Author-email: ilyachch@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

