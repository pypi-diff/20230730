# Comparing `tmp/TranslatorX-1.1.tar.gz` & `tmp/TranslatorX-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TranslatorX-1.1.tar", last modified: Sun Jul 30 15:39:37 2023, max compression
+gzip compressed data, was "TranslatorX-1.2.tar", last modified: Sun Jul 30 15:40:46 2023, max compression
```

## Comparing `TranslatorX-1.1.tar` & `TranslatorX-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 15:39:37.924024 TranslatorX-1.1/
--rw-rw-rw-   0        0        0     1487 2023-07-30 15:39:37.924024 TranslatorX-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-07-30 15:35:02.000000 TranslatorX-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 15:39:37.904083 TranslatorX-1.1/TranslatorX/
--rw-rw-rw-   0        0        0     2518 2023-07-30 15:39:31.000000 TranslatorX-1.1/TranslatorX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:39:37.924024 TranslatorX-1.1/TranslatorX.egg-info/
--rw-rw-rw-   0        0        0     1487 2023-07-30 15:39:37.000000 TranslatorX-1.1/TranslatorX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-30 15:39:37.000000 TranslatorX-1.1/TranslatorX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 15:39:37.000000 TranslatorX-1.1/TranslatorX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-30 15:39:37.000000 TranslatorX-1.1/TranslatorX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 15:39:37.000000 TranslatorX-1.1/TranslatorX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 15:39:37.924024 TranslatorX-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1166 2023-07-30 15:39:19.000000 TranslatorX-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:40:46.054376 TranslatorX-1.2/
+-rw-rw-rw-   0        0        0     1492 2023-07-30 15:40:46.054376 TranslatorX-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-07-30 15:35:02.000000 TranslatorX-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 15:40:46.036067 TranslatorX-1.2/TranslatorX/
+-rw-rw-rw-   0        0        0     2518 2023-07-30 15:40:40.000000 TranslatorX-1.2/TranslatorX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:40:46.054376 TranslatorX-1.2/TranslatorX.egg-info/
+-rw-rw-rw-   0        0        0     1492 2023-07-30 15:40:45.000000 TranslatorX-1.2/TranslatorX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-30 15:40:45.000000 TranslatorX-1.2/TranslatorX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:40:45.000000 TranslatorX-1.2/TranslatorX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-30 15:40:45.000000 TranslatorX-1.2/TranslatorX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 15:40:45.000000 TranslatorX-1.2/TranslatorX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 15:40:46.054376 TranslatorX-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1171 2023-07-30 15:40:33.000000 TranslatorX-1.2/setup.py
```

### Comparing `TranslatorX-1.1/PKG-INFO` & `TranslatorX-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: TranslatorX
-Version: 1.1
+Version: 1.2
 Summary: A Python package for translation that uses Google translator and also supports asynchronous programming!
-Home-page: https://github.com/shayanheidari01/rubika
+Home-page: https://github.com/shayanheidari01/TranslatorX
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: translator,translate,google,asyncio,googletrans
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `TranslatorX-1.1/README.md` & `TranslatorX-1.2/README.md`

 * *Files identical despite different names*

### Comparing `TranslatorX-1.1/TranslatorX/__init__.py` & `TranslatorX-1.2/TranslatorX/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from user_agent import generate_user_agent
 import urllib.parse
 import httpx
 import html
 import re
 
 
-__version__ = '1.1'
+__version__ = '1.2'
 __author__ = 'Shayan Heidari'
 
 
 class AsyncTranslator:
     def __init__(self, base_url: str = None) -> None:
         self.base_url = base_url or 'https://translate.google.com'
         self.__client = httpx.AsyncClient(base_url=self.base_url)
```

### Comparing `TranslatorX-1.1/TranslatorX.egg-info/PKG-INFO` & `TranslatorX-1.2/TranslatorX.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: TranslatorX
-Version: 1.1
+Version: 1.2
 Summary: A Python package for translation that uses Google translator and also supports asynchronous programming!
-Home-page: https://github.com/shayanheidari01/rubika
+Home-page: https://github.com/shayanheidari01/TranslatorX
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: translator,translate,google,asyncio,googletrans
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `TranslatorX-1.1/setup.py` & `TranslatorX-1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 requirements = ['httpx', 'user_agent']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'TranslatorX',
-    version = '1.1',
+    version = '1.2',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'A Python package for translation that uses Google translator and also supports asynchronous programming!',
     keywords = ['translator', 'translate', 'google', 'asyncio', 'googletrans'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
-    url = 'https://github.com/shayanheidari01/rubika',
+    url = 'https://github.com/shayanheidari01/TranslatorX',
     packages = find_packages(),
     install_requires = requirements,
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

