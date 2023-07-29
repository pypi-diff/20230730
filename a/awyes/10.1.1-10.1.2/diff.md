# Comparing `tmp/awyes-10.1.1.tar.gz` & `tmp/awyes-10.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.1.1.tar", last modified: Sat Jul 29 21:54:09 2023, max compression
+gzip compressed data, was "awyes-10.1.2.tar", last modified: Sat Jul 29 22:01:02 2023, max compression
```

## Comparing `awyes-10.1.1.tar` & `awyes-10.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:54:09.720784 awyes-10.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:54:09.720784 awyes-10.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-29 21:53:48.000000 awyes-10.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:54:09.716783 awyes-10.1.1/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 21:54:08.000000 awyes-10.1.1/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-29 21:53:48.000000 awyes-10.1.1/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 21:53:48.000000 awyes-10.1.1/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 21:53:48.000000 awyes-10.1.1/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:54:09.716783 awyes-10.1.1/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:54:09.720784 awyes-10.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 21:53:48.000000 awyes-10.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:01:02.257196 awyes-10.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:01:02.257196 awyes-10.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-29 22:00:39.000000 awyes-10.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:01:02.257196 awyes-10.1.2/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 22:01:00.000000 awyes-10.1.2/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-29 22:00:39.000000 awyes-10.1.2/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 22:00:39.000000 awyes-10.1.2/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 22:00:39.000000 awyes-10.1.2/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:01:02.257196 awyes-10.1.2/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:01:02.000000 awyes-10.1.2/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 22:01:02.000000 awyes-10.1.2/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:01:02.000000 awyes-10.1.2/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 22:01:02.000000 awyes-10.1.2/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 22:01:02.000000 awyes-10.1.2/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:01:02.000000 awyes-10.1.2/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:01:02.257196 awyes-10.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 22:00:39.000000 awyes-10.1.2/setup.py
```

### Comparing `awyes-10.1.1/PKG-INFO` & `awyes-10.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.1
+Version: 10.1.2
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.1/README.md` & `awyes-10.1.2/README.md`

 * *Files identical despite different names*

### Comparing `awyes-10.1.1/awyes/awyes.py` & `awyes-10.1.2/awyes/awyes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 import boto3
 import docker
 import yaml
 
 from sys import argv
+from textwrap import indent
 from os.path import normpath
 
 from .utils import rgetattr, rsetattr
 
 
 class Deployment:
     def __init__(self, path=""):
@@ -85,28 +86,31 @@
         for node in self.get_topologically_sorted_nodes():
             node_name = rgetattr(node, "name")
             node_args = rgetattr(node, "args")
             node_client = rgetattr(self.clients, rgetattr(node, "client"))
 
             resource_name, action_name = node_name.split(".")
 
+            print(node_name)
+
             try:
                 action = rgetattr(node_client, action_name)
                 value = action(**self.shared_lookup(node_args))
 
-                print(f"executing: {node_name}")
-                print(f"setting value {value}")
+                print(
+                    indent(f"setting value {value}", '\t+ ', lambda: True))
 
                 rsetattr(
                     context=self.config,
                     accessor=f"{resource_name}.{action_name}",
                     value=value,
                 )
             except Exception as e:
-                print("err: ", e)
+                print(
+                    indent(f"err: {e}", '\t- ', lambda: True))
 
 
 def main():
     _, *path = argv
     path = path[0] if path else "./awyes.yml"
 
     Deployment(path=path).deploy()
```

### Comparing `awyes-10.1.1/awyes/awyes_test.py` & `awyes-10.1.2/awyes/awyes_test.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.1/awyes/utils.py` & `awyes-10.1.2/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.1/awyes.egg-info/PKG-INFO` & `awyes-10.1.2/awyes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.1
+Version: 10.1.2
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.1/setup.py` & `awyes-10.1.2/setup.py`

 * *Files identical despite different names*

