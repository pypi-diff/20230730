# Comparing `tmp/testflows.github.runners-1.3.230729.1231711.tar.gz` & `tmp/testflows.github.runners-1.3.230729.1235004.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230729.1231711.tar", last modified: Sat Jul 29 23:17:11 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230729.1235004.tar", last modified: Sat Jul 29 23:50:04 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230729.1231711.tar` & `testflows.github.runners-1.3.230729.1235004.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    46741 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    46149 2023-07-29 22:19:05.000000 testflows.github.runners-1.3.230729.1231711/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2491 2023-07-29 22:10:17.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22712 2023-07-29 21:42:45.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     3995 2023-07-29 22:12:50.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    16705 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1231711/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:17:11.804535 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    46741 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-29 23:17:11.000000 testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    47821 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    47229 2023-07-29 23:49:58.000000 testflows.github.runners-1.3.230729.1235004/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2491 2023-07-29 22:10:17.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    23217 2023-07-29 23:28:28.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3995 2023-07-29 22:12:50.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16705 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230729.1235004/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-29 23:50:04.743454 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    47821 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1105 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-29 23:50:04.000000 testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230729.1231711/LICENSE` & `testflows.github.runners-1.3.230729.1235004/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/PKG-INFO` & `testflows.github.runners-1.3.230729.1235004/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230729.1231711
+Version: 1.3.230729.1235004
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -409,14 +409,40 @@
              },
              "loggers": {
                  "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
              },
          }
      )
 
+----
+
+--------------------------------------
+Deleting All Runners And Their Servers
+--------------------------------------
+
+You can delete all runners, including standby runners, and their servers using the **delete** command.
+
+:✋ Note:
+   The **delete** command will not delete cloud service server. If you also want to delete it,
+   you also need to execute **cloud delete** command. For more information, see `Deleting Cloud Service`_ section.
+
+.. code-block:: bash
+
+   github-runners delete
+
+::
+
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to Hetzner Cloud
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to GitHub
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Getting repository testflows/testflows-github-runners
+   07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of self-hosted runners
+   07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of servers
+
+----
+
 ------------------------
 Using Configuration File
 ------------------------
 
 Instead of passing configuration options using command line arguments, you can use
 configuration file. The configuration file is Python file that must define the **config**
 object of the `Config class`_.
@@ -1322,14 +1348,17 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
+    * **delete**
+      delete all servers
+
     * **cloud**
       cloud service commands
 
       * **-n server, --name server**
         deployment server name, default: *github-runners*
 
       * **deploy**
```

### Comparing `testflows.github.runners-1.3.230729.1231711/README.rst` & `testflows.github.runners-1.3.230729.1235004/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,40 @@
              },
              "loggers": {
                  "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
              },
          }
      )
 
+----
+
+--------------------------------------
+Deleting All Runners And Their Servers
+--------------------------------------
+
+You can delete all runners, including standby runners, and their servers using the **delete** command.
+
+:✋ Note:
+   The **delete** command will not delete cloud service server. If you also want to delete it,
+   you also need to execute **cloud delete** command. For more information, see `Deleting Cloud Service`_ section.
+
+.. code-block:: bash
+
+   github-runners delete
+
+::
+
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to Hetzner Cloud
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to GitHub
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Getting repository testflows/testflows-github-runners
+   07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of self-hosted runners
+   07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of servers
+
+----
+
 ------------------------
 Using Configuration File
 ------------------------
 
 Instead of passing configuration options using command line arguments, you can use
 configuration file. The configuration file is Python file that must define the **config**
 object of the `Config class`_.
@@ -1305,14 +1331,17 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
+    * **delete**
+      delete all servers
+
     * **cloud**
       cloud service commands
 
       * **-n server, --name server**
         deployment server name, default: *github-runners*
 
       * **deploy**
```

### Comparing `testflows.github.runners-1.3.230729.1231711/setup.py` & `testflows.github.runners-1.3.230729.1235004/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230729.1231711",
+    version="1.3.230729.1235004",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/__init__.py`

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
-__version__ = "1.3.230729.1231711"
+__version__ = "1.3.230729.1235004"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from testflows.github.runners.scripts import Scripts, scripts
 from testflows.github.runners.logger import logger
 from testflows.github.runners.config import Config, check_image
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
+import testflows.github.runners.delete as delete
 
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
@@ -221,14 +222,27 @@
         help="enable debugging mode, default: False",
     )
 
     commands = parser.add_subparsers(
         title="commands", metavar="command", description=None, help=None
     )
 
+    delete_parser = commands.add_parser(
+        "delete",
+        help="delete all servers",
+        description=(
+            f"Delete all servers that provide runners and including any standby runners.\n\n"
+            "Note that cloud service server is not delete. If you have one use\n"
+            "'cloud delete' command to delete it."
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    delete_parser.set_defaults(func=delete.all)
+
     cloud_parser = commands.add_parser(
         "cloud",
         help="cloud service commands",
         description="Deploying and running application as a service on a cloud instance.",
         formatter_class=RawTextHelpFormatter,
     )
```

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     url,
     headers=None,
     data=None,
     format=None,
     encoding="utf-8",
     timeout=60,
     process_error=True,
+    method=None,
 ):
     """Perform URL request."""
     if headers is None:
         headers = {}
 
-    r = Request(url, headers=headers, data=data)
+    r = Request(url, headers=headers, data=data, method=method)
 
     try:
         with urlopen(r, timeout=timeout) as response:
             response: HTTPResponse = response
 
             data = response.read()
             if encoding:
```

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230729.1235004/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230729.1231711
+Version: 1.3.230729.1235004
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -409,14 +409,40 @@
              },
              "loggers": {
                  "testflows.github.runners": {"level": "INFO", "handlers": ["default"]},
              },
          }
      )
 
+----
+
+--------------------------------------
+Deleting All Runners And Their Servers
+--------------------------------------
+
+You can delete all runners, including standby runners, and their servers using the **delete** command.
+
+:✋ Note:
+   The **delete** command will not delete cloud service server. If you also want to delete it,
+   you also need to execute **cloud delete** command. For more information, see `Deleting Cloud Service`_ section.
+
+.. code-block:: bash
+
+   github-runners delete
+
+::
+
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to Hetzner Cloud
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Logging in to GitHub
+   07/29/2023 07:43:16 PM     INFO       MainThread             all 🍀 Getting repository testflows/testflows-github-runners
+   07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of self-hosted runners
+   07/29/2023 07:43:17 PM     INFO       MainThread             all 🍀 Getting list of servers
+
+----
+
 ------------------------
 Using Configuration File
 ------------------------
 
 Instead of passing configuration options using command line arguments, you can use
 configuration file. The configuration file is Python file that must define the **config**
 object of the `Config class`_.
@@ -1322,14 +1348,17 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
+    * **delete**
+      delete all servers
+
     * **cloud**
       cloud service commands
 
       * **-n server, --name server**
         deployment server name, default: *github-runners*
 
       * **deploy**
```

### Comparing `testflows.github.runners-1.3.230729.1231711/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230729.1235004/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 testflows.github.runners.egg-info/requires.txt
 testflows.github.runners.egg-info/top_level.txt
 testflows/github/runners/__init__.py
 testflows/github/runners/actions.py
 testflows/github/runners/args.py
 testflows/github/runners/cloud.py
 testflows/github/runners/config.py
+testflows/github/runners/delete.py
 testflows/github/runners/logger.py
 testflows/github/runners/request.py
 testflows/github/runners/scale_down.py
 testflows/github/runners/scale_up.py
 testflows/github/runners/server.py
 testflows/github/runners/service.py
 testflows/github/runners/shell.py
```

