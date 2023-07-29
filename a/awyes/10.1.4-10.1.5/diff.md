# Comparing `tmp/awyes-10.1.4.tar.gz` & `tmp/awyes-10.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.1.4.tar", last modified: Sat Jul 29 22:25:55 2023, max compression
+gzip compressed data, was "awyes-10.1.5.tar", last modified: Sat Jul 29 22:29:50 2023, max compression
```

## Comparing `awyes-10.1.4.tar` & `awyes-10.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:25:55.844055 awyes-10.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:25:55.844055 awyes-10.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-29 22:25:33.000000 awyes-10.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:25:55.844055 awyes-10.1.4/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 22:25:54.000000 awyes-10.1.4/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-29 22:25:33.000000 awyes-10.1.4/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-29 22:25:33.000000 awyes-10.1.4/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 22:25:33.000000 awyes-10.1.4/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:25:55.844055 awyes-10.1.4/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:25:55.844055 awyes-10.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 22:25:33.000000 awyes-10.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:29:50.653030 awyes-10.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:29:50.653030 awyes-10.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-29 22:29:30.000000 awyes-10.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:29:50.649030 awyes-10.1.5/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 22:29:49.000000 awyes-10.1.5/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-29 22:29:30.000000 awyes-10.1.5/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-29 22:29:30.000000 awyes-10.1.5/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 22:29:30.000000 awyes-10.1.5/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:29:50.649030 awyes-10.1.5/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:29:50.653030 awyes-10.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 22:29:30.000000 awyes-10.1.5/setup.py
```

### Comparing `awyes-10.1.4/PKG-INFO` & `awyes-10.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.4
+Version: 10.1.5
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.4/README.md` & `awyes-10.1.5/README.md`

 * *Files identical despite different names*

### Comparing `awyes-10.1.4/awyes/awyes.py` & `awyes-10.1.5/awyes/awyes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 import boto3
 import docker
 import yaml
 
 from sys import argv
+from pprint import pprint
 from textwrap import indent
 from os.path import normpath
 
 from .utils import rgetattr, rsetattr
 
 
 class Deployment:
@@ -94,24 +95,24 @@
 
             print(node_name)
 
             try:
                 action = rgetattr(node_client, action_name)
                 value = action(**self.shared_lookup(node_args))
 
-                print(
+                pprint(
                     indent(f"setting value {value}", '\t+ ', lambda _: True))
 
                 rsetattr(
                     context=self.config,
                     accessor=f"{resource_name}.{action_name}",
                     value=value,
                 )
             except Exception as e:
-                print(
+                pprint(
                     indent(f"err: {e}", '\t- ', lambda _: True))
 
 
 def main():
     _, *path = argv
     path = path[0] if path else "./awyes.yml"
```

### Comparing `awyes-10.1.4/awyes/awyes_test.py` & `awyes-10.1.5/awyes/awyes_test.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.4/awyes/utils.py` & `awyes-10.1.5/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.4/awyes.egg-info/PKG-INFO` & `awyes-10.1.5/awyes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.4
+Version: 10.1.5
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.4/setup.py` & `awyes-10.1.5/setup.py`

 * *Files identical despite different names*

