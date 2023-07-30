# Comparing `tmp/awyes-10.1.5.tar.gz` & `tmp/awyes-10.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.1.5.tar", last modified: Sat Jul 29 22:29:50 2023, max compression
+gzip compressed data, was "awyes-10.1.6.tar", last modified: Sun Jul 30 06:15:10 2023, max compression
```

## Comparing `awyes-10.1.5.tar` & `awyes-10.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:29:50.653030 awyes-10.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:29:50.653030 awyes-10.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-29 22:29:30.000000 awyes-10.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:29:50.649030 awyes-10.1.5/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 22:29:49.000000 awyes-10.1.5/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-29 22:29:30.000000 awyes-10.1.5/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-29 22:29:30.000000 awyes-10.1.5/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 22:29:30.000000 awyes-10.1.5/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:29:50.649030 awyes-10.1.5/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:29:50.000000 awyes-10.1.5/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:29:50.653030 awyes-10.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 22:29:30.000000 awyes-10.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:10.523998 awyes-10.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 06:15:10.523998 awyes-10.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-30 06:14:49.000000 awyes-10.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:10.523998 awyes-10.1.6/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 06:15:08.000000 awyes-10.1.6/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-30 06:14:49.000000 awyes-10.1.6/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-30 06:14:49.000000 awyes-10.1.6/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-30 06:14:49.000000 awyes-10.1.6/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:10.523998 awyes-10.1.6/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 06:15:10.000000 awyes-10.1.6/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 06:15:10.000000 awyes-10.1.6/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:15:10.000000 awyes-10.1.6/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 06:15:10.000000 awyes-10.1.6/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 06:15:10.000000 awyes-10.1.6/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 06:15:10.000000 awyes-10.1.6/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:15:10.523998 awyes-10.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-30 06:14:49.000000 awyes-10.1.6/setup.py
```

### Comparing `awyes-10.1.5/PKG-INFO` & `awyes-10.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.5
+Version: 10.1.6
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.5/README.md` & `awyes-10.1.6/README.md`

 * *Files identical despite different names*

### Comparing `awyes-10.1.5/awyes/awyes.py` & `awyes-10.1.6/awyes/awyes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import re
 import boto3
 import docker
 import yaml
+import json
 
 from sys import argv
 from pprint import pprint
 from textwrap import indent
 from os.path import normpath
 
 from .utils import rgetattr, rsetattr
 
 
 class Deployment:
     def __init__(self, path=""):
-        # Initialize paths and log settings
+        # Initialize paths
         self.path = path
 
         # Load the clients and config
         with open(normpath(path)) as config:
             self.config = yaml.safe_load(config)
             self.clients = {
                 "os": os,
@@ -89,31 +90,31 @@
         for node in self.get_topologically_sorted_nodes():
             node_name = rgetattr(node, "name")
             node_args = rgetattr(node, "args")
             node_client = rgetattr(self.clients, rgetattr(node, "client"))
 
             resource_name, action_name = node_name.split(".")
 
-            print(node_name)
+            print(f"\033[36m{node_name}\033[0m")
 
             try:
                 action = rgetattr(node_client, action_name)
                 value = action(**self.shared_lookup(node_args))
 
-                pprint(
-                    indent(f"setting value {value}", '\t+ ', lambda _: True))
+                print(indent(json.dumps(value, indent=2,
+                      default=str), '+ ', lambda _: True))
 
                 rsetattr(
                     context=self.config,
                     accessor=f"{resource_name}.{action_name}",
                     value=value,
                 )
             except Exception as e:
-                pprint(
-                    indent(f"err: {e}", '\t- ', lambda _: True))
+                print(indent(json.dumps(e, indent=2, default=str),
+                      '- ', lambda _: True))
 
 
 def main():
     _, *path = argv
     path = path[0] if path else "./awyes.yml"
 
     Deployment(path=path).deploy()
```

### Comparing `awyes-10.1.5/awyes/awyes_test.py` & `awyes-10.1.6/awyes/awyes_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,10 +13,13 @@
         self.assertEqual([rgetattr(node, 'name') for node in sorted_nodes], [
             'pastewin_role.create_role',
             'pastewin_role.get_role',
             'pastewin_role_attach_cloud.attach_role_policy',
             'pastewin_role_attach_s3.attach_role_policy'
         ])
 
+    def test_deploy(self):
+        self.d.deploy()
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `awyes-10.1.5/awyes/utils.py` & `awyes-10.1.6/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.5/awyes.egg-info/PKG-INFO` & `awyes-10.1.6/awyes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.5
+Version: 10.1.6
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.5/setup.py` & `awyes-10.1.6/setup.py`

 * *Files identical despite different names*

