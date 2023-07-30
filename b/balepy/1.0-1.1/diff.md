# Comparing `tmp/balepy-1.0.tar.gz` & `tmp/balepy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-1.0.tar", last modified: Sun Jul 30 11:39:28 2023, max compression
+gzip compressed data, was "balepy-1.1.tar", last modified: Sun Jul 30 13:59:24 2023, max compression
```

## Comparing `balepy-1.0.tar` & `balepy-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:39:28.520944 balepy-1.0/
--rw-r--r--   0 mamad     (1000) mamad     (1000)     1073 2023-07-29 20:43:35.000000 balepy-1.0/LICENSE
--rw-r--r--   0 mamad     (1000) mamad     (1000)     1289 2023-07-30 11:39:28.520944 balepy-1.0/PKG-INFO
--rw-r--r--   0 mamad     (1000) mamad     (1000)      535 2023-07-29 20:43:13.000000 balepy-1.0/README.md
-drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:39:28.520944 balepy-1.0/balepy/
--rw-r--r--   0 mamad     (1000) mamad     (1000)     5755 2023-07-30 11:26:13.000000 balepy-1.0/balepy/__init__.py
-drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:39:28.520944 balepy-1.0/balepy.egg-info/
--rw-r--r--   0 mamad     (1000) mamad     (1000)     1289 2023-07-30 11:39:28.000000 balepy-1.0/balepy.egg-info/PKG-INFO
--rw-r--r--   0 mamad     (1000) mamad     (1000)      165 2023-07-30 11:39:28.000000 balepy-1.0/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 mamad     (1000) mamad     (1000)        1 2023-07-30 11:39:28.000000 balepy-1.0/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 mamad     (1000) mamad     (1000)        7 2023-07-30 11:39:28.000000 balepy-1.0/balepy.egg-info/top_level.txt
--rw-r--r--   0 mamad     (1000) mamad     (1000)       38 2023-07-30 11:39:28.520944 balepy-1.0/setup.cfg
--rw-r--r--   0 mamad     (1000) mamad     (1000)      988 2023-07-30 11:39:09.000000 balepy-1.0/setup.py
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 13:59:24.638311 balepy-1.1/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1073 2023-07-29 20:43:35.000000 balepy-1.1/LICENSE
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1289 2023-07-30 13:59:24.638311 balepy-1.1/PKG-INFO
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      535 2023-07-29 20:43:13.000000 balepy-1.1/README.md
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 13:59:24.638311 balepy-1.1/balepy/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     5728 2023-07-30 13:55:17.000000 balepy-1.1/balepy/__init__.py
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 13:59:24.638311 balepy-1.1/balepy.egg-info/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1289 2023-07-30 13:59:24.000000 balepy-1.1/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      165 2023-07-30 13:59:24.000000 balepy-1.1/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)        1 2023-07-30 13:59:24.000000 balepy-1.1/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)        7 2023-07-30 13:59:24.000000 balepy-1.1/balepy.egg-info/top_level.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)       38 2023-07-30 13:59:24.638311 balepy-1.1/setup.cfg
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      988 2023-07-30 13:58:51.000000 balepy-1.1/setup.py
```

### Comparing `balepy-1.0/LICENSE` & `balepy-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balepy-1.0/PKG-INFO` & `balepy-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 1.0
+Version: 1.1
 Summary: balepy a Library Python for create bots API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: balepy Version: 1.0 Summary: balepy a Library
+Metadata-Version: 2.1 Name: balepy Version: 1.1 Summary: balepy a Library
 Python for create bots API in bale application Home-page: https://github.com/
 OnlyRad/bale Author: Mohammad and Erfan Author-email:
 mohammadmehrabi175@gmail.com Keywords: bot,Bot,bale,robot Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `balepy-1.0/README.md` & `balepy-1.1/README.md`

 * *Files identical despite different names*

### Comparing `balepy-1.0/balepy/__init__.py` & `balepy-1.1/balepy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from client import Client
 from requests import get , post
 
 print(f"""Wellcome to balepy library v1.0
 Mohammad Mehrabi Rad and Erfan Bafandeh <github.com/OnlyRad/balepy>\n\n""")
 
 
 class Client:
```

### Comparing `balepy-1.0/balepy.egg-info/PKG-INFO` & `balepy-1.1/balepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 1.0
+Version: 1.1
 Summary: balepy a Library Python for create bots API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: balepy Version: 1.0 Summary: balepy a Library
+Metadata-Version: 2.1 Name: balepy Version: 1.1 Summary: balepy a Library
 Python for create bots API in bale application Home-page: https://github.com/
 OnlyRad/bale Author: Mohammad and Erfan Author-email:
 mohammadmehrabi175@gmail.com Keywords: bot,Bot,bale,robot Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `balepy-1.0/setup.py` & `balepy-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '1.0',
+    version = '1.1',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bots API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

