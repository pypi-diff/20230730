# Comparing `tmp/python_test_helper-0.0.1.tar.gz` & `tmp/python_test_helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_test_helper-0.0.1.tar", last modified: Sun Jul 30 16:03:05 2023, max compression
+gzip compressed data, was "python_test_helper-0.0.2.tar", last modified: Sun Jul 30 21:02:15 2023, max compression
```

## Comparing `python_test_helper-0.0.1.tar` & `python_test_helper-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:03:05.540870 python_test_helper-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-30 16:03:05.540870 python_test_helper-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:03:05.536870 python_test_helper-0.0.1/helper_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/helper_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:03:05.540870 python_test_helper-0.0.1/helper_methods/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/helper_methods/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/helper_methods/helper/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/helper_methods/helper/jwt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/helper_methods/helper/request_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:03:05.540870 python_test_helper-0.0.1/python_test_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-30 16:03:05.000000 python_test_helper-0.0.1/python_test_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-30 16:03:05.000000 python_test_helper-0.0.1/python_test_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:03:05.000000 python_test_helper-0.0.1/python_test_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 16:03:05.000000 python_test_helper-0.0.1/python_test_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 16:03:05.000000 python_test_helper-0.0.1/python_test_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:03:05.540870 python_test_helper-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:03:05.540870 python_test_helper-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-30 16:02:48.000000 python_test_helper-0.0.1/tests/test_request_helper_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/helper_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/helper_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/helper_methods/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/helper_methods/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/helper_methods/helper/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/helper_methods/helper/jwt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/helper_methods/helper/request_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/python_test_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-30 21:02:15.000000 python_test_helper-0.0.2/python_test_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-30 21:02:15.000000 python_test_helper-0.0.2/python_test_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:02:15.000000 python_test_helper-0.0.2/python_test_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 21:02:15.000000 python_test_helper-0.0.2/python_test_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 21:02:15.000000 python_test_helper-0.0.2/python_test_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:02:15.219650 python_test_helper-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/tests/test_request_helper_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-30 21:01:54.000000 python_test_helper-0.0.2/tests/test_request_helper_multi_parts.py
```

### Comparing `python_test_helper-0.0.1/PKG-INFO` & `python_test_helper-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_test_helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Methods to help you in your tests
 Home-page: https://github.com/delrey1/python-test-helper
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -18,16 +18,22 @@
 
 # Python Test Helper
 
 ## Contents
 
 ### jwt_helper
 
-`sleep_until_access_token_ready`
+#### sleep_until_access_token_ready
 
-* Use this if your computer clock is behind the token server
+Use this if your computer clock is behind the token server
+
+```
+from helper_methods.helper import jwt_helper
+
+jwt_helper.sleep_until_access_token_ready(access_token)
+```
 
 ### request_helper
 
 `RequestHelper`
 
 * Extends the requests `Session` to allow a `base_url` to be provided
```

### Comparing `python_test_helper-0.0.1/python_test_helper.egg-info/PKG-INFO` & `python_test_helper-0.0.2/python_test_helper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-test-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Methods to help you in your tests
 Home-page: https://github.com/delrey1/python-test-helper
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -18,16 +18,22 @@
 
 # Python Test Helper
 
 ## Contents
 
 ### jwt_helper
 
-`sleep_until_access_token_ready`
+#### sleep_until_access_token_ready
 
-* Use this if your computer clock is behind the token server
+Use this if your computer clock is behind the token server
+
+```
+from helper_methods.helper import jwt_helper
+
+jwt_helper.sleep_until_access_token_ready(access_token)
+```
 
 ### request_helper
 
 `RequestHelper`
 
 * Extends the requests `Session` to allow a `base_url` to be provided
```

### Comparing `python_test_helper-0.0.1/setup.py` & `python_test_helper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 readme = open('README.md').read()
 
 NAME = "python_test_helper"
 
 setup(
     name=NAME,
-    version='0.0.1',
+    version='0.0.2',
     description="Simple Methods to help you in your tests",
     keywords=["python"],
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
     packages=find_packages(exclude=('tests*',)),
     test_suite='tests',
```

### Comparing `python_test_helper-0.0.1/tests/test_request_helper_basic.py` & `python_test_helper-0.0.2/tests/test_request_helper_basic.py`

 * *Files identical despite different names*

