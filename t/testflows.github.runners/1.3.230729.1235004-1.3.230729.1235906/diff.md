# Comparing `tmp/testflows.github.runners-1.3.230729.1235004.tar.gz` & `tmp/testflows.github.runners-1.3.230729.1235906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230729.1235004.tar", last modified: Sat Jul 29 23:50:04 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230729.1235906.tar", last modified: Sat Jul 29 23:59:06 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230729.1235004.tar` & `testflows.github.runners-1.3.230729.1235906.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    47821 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    47229 2023-07-29 23:49:58.000000 testflows.github.runners-1.3.230729.1235004/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2491 2023-07-29 22:10:17.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    23217 2023-07-29 23:28:28.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     3995 2023-07-29 22:12:50.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    16705 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    47821 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1105 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    47821 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    47229 2023-07-29 23:49:58.000000 testflows.github.runners-1.3.230729.1235906/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.910268 testflows.github.runners-1.3.230729.1235906/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.910268 testflows.github.runners-1.3.230729.1235906/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2491 2023-07-29 22:10:17.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    23217 2023-07-29 23:28:28.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4008 2023-07-29 23:57:15.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16705 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235906/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:59:06.914268 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    47821 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1105 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-29 23:59:06.000000 testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230729.1235004/LICENSE` & `testflows.github.runners-1.3.230729.1235906/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/PKG-INFO` & `testflows.github.runners-1.3.230729.1235906/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230729.1235004
+Version: 1.3.230729.1235906
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230729.1235004/README.rst` & `testflows.github.runners-1.3.230729.1235906/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/setup.py` & `testflows.github.runners-1.3.230729.1235906/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230729.1235004",
+    version="1.3.230729.1235906",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230729.1235004"
+__version__ = "1.3.230729.1235906"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     labels: list[str]
     count: count = 1
     replenish_immediately: bool = True
 
 
 @dataclass
 class deploy:
-    server_type: server_type = "cpx11"
+    server_type: server_type = server_type("cpx11")
     image: image = image("system:ubuntu-22.04")
     location: location = None
     setup_script: path = None
 
 
 @dataclass
 class cloud:
```

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230729.1235906/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230729.1235004
+Version: 1.3.230729.1235906
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230729.1235906/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

