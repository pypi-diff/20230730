# Comparing `tmp/jobbergate_core-3.5.0a7.tar.gz` & `tmp/jobbergate_core-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_core-3.5.0a7.tar", max compression
+gzip compressed data, was "jobbergate_core-3.6.0.tar", max compression
```

## Comparing `jobbergate_core-3.5.0a7.tar` & `jobbergate_core-3.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/LICENSE
--rw-r--r--   0        0        0      420 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/README.rst
--rw-r--r--   0        0        0      329 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/jobbergate_core/__init__.py
--rw-r--r--   0        0        0      366 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/jobbergate_core/auth/__init__.py
--rw-r--r--   0        0        0      279 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/jobbergate_core/auth/exceptions.py
--rw-r--r--   0        0        0    11813 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/jobbergate_core/auth/handler.py
--rw-r--r--   0        0        0     5534 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/jobbergate_core/auth/token.py
--rw-r--r--   0        0        0      133 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/jobbergate_core/version.py
--rw-r--r--   0        0        0     1763 2023-06-28 19:08:36.535131 jobbergate_core-3.5.0a7/pyproject.toml
--rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 jobbergate_core-3.5.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/LICENSE
+-rw-r--r--   0        0        0      420 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/README.rst
+-rw-r--r--   0        0        0      329 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/jobbergate_core/__init__.py
+-rw-r--r--   0        0        0      366 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/jobbergate_core/auth/__init__.py
+-rw-r--r--   0        0        0      279 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/jobbergate_core/auth/exceptions.py
+-rw-r--r--   0        0        0    11813 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/jobbergate_core/auth/handler.py
+-rw-r--r--   0        0        0     5534 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/jobbergate_core/auth/token.py
+-rw-r--r--   0        0        0      133 2023-07-30 04:37:46.579528 jobbergate_core-3.6.0/jobbergate_core/version.py
+-rw-r--r--   0        0        0     1761 2023-07-30 04:37:46.583529 jobbergate_core-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 jobbergate_core-3.6.0/PKG-INFO
```

### Comparing `jobbergate_core-3.5.0a7/LICENSE` & `jobbergate_core-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_core-3.5.0a7/jobbergate_core/auth/handler.py` & `jobbergate_core-3.6.0/jobbergate_core/auth/handler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-3.5.0a7/jobbergate_core/auth/token.py` & `jobbergate_core-3.6.0/jobbergate_core/auth/token.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-3.5.0a7/pyproject.toml` & `jobbergate_core-3.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-core"
-version = "3.5.0a7"
+version = "3.6.0"
 description = "Jobbergate Core"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_core-3.5.0a7/PKG-INFO` & `jobbergate_core-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-core
-Version: 3.5.0a7
+Version: 3.6.0
 Summary: Jobbergate Core
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

