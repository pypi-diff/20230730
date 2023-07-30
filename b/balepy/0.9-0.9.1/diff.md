# Comparing `tmp/balepy-0.9.tar.gz` & `tmp/balepy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-0.9.tar", last modified: Sun Jul 30 11:02:15 2023, max compression
+gzip compressed data, was "balepy-0.9.1.tar", last modified: Sun Jul 30 11:26:49 2023, max compression
```

## Comparing `balepy-0.9.tar` & `balepy-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:02:15.602303 balepy-0.9/
--rw-r--r--   0 mamad     (1000) mamad     (1000)     1073 2023-07-29 20:43:35.000000 balepy-0.9/LICENSE
--rw-r--r--   0 mamad     (1000) mamad     (1000)     1288 2023-07-30 11:02:15.602303 balepy-0.9/PKG-INFO
--rw-r--r--   0 mamad     (1000) mamad     (1000)      535 2023-07-29 20:43:13.000000 balepy-0.9/README.md
-drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:02:15.602303 balepy-0.9/balepy/
--rw-r--r--   0 mamad     (1000) mamad     (1000)      156 2023-07-29 21:42:23.000000 balepy-0.9/balepy/__init__.py
--rw-r--r--   0 mamad     (1000) mamad     (1000)     5604 2023-07-29 21:42:03.000000 balepy-0.9/balepy/client.py
-drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:02:15.602303 balepy-0.9/balepy.egg-info/
--rw-r--r--   0 mamad     (1000) mamad     (1000)     1288 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/PKG-INFO
--rw-r--r--   0 mamad     (1000) mamad     (1000)      182 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 mamad     (1000) mamad     (1000)        1 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 mamad     (1000) mamad     (1000)        7 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/top_level.txt
--rw-r--r--   0 mamad     (1000) mamad     (1000)       38 2023-07-30 11:02:15.602303 balepy-0.9/setup.cfg
--rw-r--r--   0 mamad     (1000) mamad     (1000)      986 2023-07-29 21:43:06.000000 balepy-0.9/setup.py
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:26:49.942765 balepy-0.9.1/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1073 2023-07-29 20:43:35.000000 balepy-0.9.1/LICENSE
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1290 2023-07-30 11:26:49.942765 balepy-0.9.1/PKG-INFO
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      535 2023-07-29 20:43:13.000000 balepy-0.9.1/README.md
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:26:49.942765 balepy-0.9.1/balepy/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     5755 2023-07-30 11:26:13.000000 balepy-0.9.1/balepy/__init__.py
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:26:49.942765 balepy-0.9.1/balepy.egg-info/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1290 2023-07-30 11:26:49.000000 balepy-0.9.1/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      165 2023-07-30 11:26:49.000000 balepy-0.9.1/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)        1 2023-07-30 11:26:49.000000 balepy-0.9.1/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)        7 2023-07-30 11:26:49.000000 balepy-0.9.1/balepy.egg-info/top_level.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)       38 2023-07-30 11:26:49.942765 balepy-0.9.1/setup.cfg
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      989 2023-07-30 11:25:47.000000 balepy-0.9.1/setup.py
```

### Comparing `balepy-0.9/LICENSE` & `balepy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balepy-0.9/PKG-INFO` & `balepy-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.9
+Version: 0.9.1
 Summary: balepy a Library Python for create bot API in bale application
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
-Metadata-Version: 2.1 Name: balepy Version: 0.9 Summary: balepy a Library
+Metadata-Version: 2.1 Name: balepy Version: 0.9.1 Summary: balepy a Library
 Python for create bot API in bale application Home-page: https://github.com/
 OnlyRad/bale Author: Mohammad and Erfan Author-email:
 mohammadmehrabi175@gmail.com Keywords: bot,Bot,bale,robot Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `balepy-0.9/README.md` & `balepy-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `balepy-0.9/balepy/client.py` & `balepy-0.9.1/balepy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from client import Client
 from requests import get , post
 
+print(f"""Wellcome to balepy library v1.0
+Mohammad Mehrabi Rad and Erfan Bafandeh <github.com/OnlyRad/balepy>\n\n""")
+
 
 class Client:
 
     def __init__(self, token):
         self.token = token
         self.connection = None
 
@@ -108,8 +112,8 @@
     def get_chat_member(self, chat_id, user_id):
         json = {"chat_id": chat_id, "user_id": user_id}
         return post(f"https://tapi.bale.ai/bot{self.token}/getChatMember" , json=json)
 
     # payments
     def send_invoice(self, chat_id, title, description, provider_token, prices):
         json = {"chat_id": chat_id, "title": title, "description": description, "provider_token": provider_token, "prices": prices}
-        return post(f"https://tapi.bale.ai/bot{self.token}/sendInvoice" , json=json)
+        return post(f"https://tapi.bale.ai/bot{self.token}/sendInvoice" , json=json)
```

### Comparing `balepy-0.9/balepy.egg-info/PKG-INFO` & `balepy-0.9.1/balepy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.9
+Version: 0.9.1
 Summary: balepy a Library Python for create bot API in bale application
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
-Metadata-Version: 2.1 Name: balepy Version: 0.9 Summary: balepy a Library
+Metadata-Version: 2.1 Name: balepy Version: 0.9.1 Summary: balepy a Library
 Python for create bot API in bale application Home-page: https://github.com/
 OnlyRad/bale Author: Mohammad and Erfan Author-email:
 mohammadmehrabi175@gmail.com Keywords: bot,Bot,bale,robot Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `balepy-0.9/setup.py` & `balepy-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '0.9',
+    version = '0.9.1',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bot API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
@@ -19,8 +19,8 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ]
-)
+)
```

