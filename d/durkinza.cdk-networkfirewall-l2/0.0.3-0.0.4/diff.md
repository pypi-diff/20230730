# Comparing `tmp/durkinza.cdk-networkfirewall-l2-0.0.3.tar.gz` & `tmp/durkinza.cdk-networkfirewall-l2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durkinza.cdk-networkfirewall-l2-0.0.3.tar", last modified: Sun Jul 30 18:32:30 2023, max compression
+gzip compressed data, was "durkinza.cdk-networkfirewall-l2-0.0.4.tar", last modified: Sun Jul 30 18:41:55 2023, max compression
```

## Comparing `durkinza.cdk-networkfirewall-l2-0.0.3.tar` & `durkinza.cdk-networkfirewall-l2-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.787728 durkinza.cdk-networkfirewall-l2-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.787728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/
--rw-r--r--   0 runner    (1001) docker     (123)   217751 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102135 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:32:17.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:32:30.791728 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:32:30.000000 durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/
+-rw-r--r--   0 runner    (1001) docker     (123)   217751 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102134 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/LICENSE` & `durkinza.cdk-networkfirewall-l2-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/PKG-INFO` & `durkinza.cdk-networkfirewall-l2-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkinza.cdk-networkfirewall-l2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Experimental L2 constructs for the aws-networkfirewall
 Home-page: https://github.com/durkinza/cdk-networkfirewall-l2#readme
 Author: durkinza<8985088+durkinza@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/durkinza/cdk-networkfirewall-l2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/README.md` & `durkinza.cdk-networkfirewall-l2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/setup.py` & `durkinza.cdk-networkfirewall-l2-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "durkinza.cdk-networkfirewall-l2",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "Experimental L2 constructs for the aws-networkfirewall",
     "license": "Apache-2.0",
     "url": "https://github.com/durkinza/cdk-networkfirewall-l2#readme",
     "long_description_content_type": "text/markdown",
     "author": "durkinza<8985088+durkinza@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "durkinza.cdk_networkfirewall_l2",
         "durkinza.cdk_networkfirewall_l2._jsii"
     ],
     "package_data": {
         "durkinza.cdk_networkfirewall_l2._jsii": [
-            "cdk-networkfirewall-l2@0.0.3.jsii.tgz"
+            "cdk-networkfirewall-l2@0.0.4.jsii.tgz"
         ],
         "durkinza.cdk_networkfirewall_l2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza/cdk_networkfirewall_l2/__init__.py` & `durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/__init__.py`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO` & `durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkinza.cdk-networkfirewall-l2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Experimental L2 constructs for the aws-networkfirewall
 Home-page: https://github.com/durkinza/cdk-networkfirewall-l2#readme
 Author: durkinza<8985088+durkinza@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/durkinza/cdk-networkfirewall-l2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.3/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt` & `durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
 src/durkinza/cdk_networkfirewall_l2/__init__.py
 src/durkinza/cdk_networkfirewall_l2/py.typed
 src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
-src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.3.jsii.tgz
+src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.4.jsii.tgz
```

