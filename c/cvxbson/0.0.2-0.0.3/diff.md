# Comparing `tmp/cvxbson-0.0.2.tar.gz` & `tmp/cvxbson-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxbson-0.0.2.tar", max compression
+gzip compressed data, was "cvxbson-0.0.3.tar", max compression
```

## Comparing `cvxbson-0.0.2.tar` & `cvxbson-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10790 2023-07-28 00:17:43.443217 cvxbson-0.0.2/LICENSE
--rw-r--r--   0        0        0     2588 2023-07-28 00:17:43.443217 cvxbson-0.0.2/README.md
--rw-r--r--   0        0        0       40 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/bson/__init__.py
--rw-r--r--   0        0        0     1951 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/bson/file.py
--rw-r--r--   0        0        0       40 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/json/__init__.py
--rw-r--r--   0        0        0     1009 2023-07-28 00:17:43.443217 cvxbson-0.0.2/cvx/json/file.py
--rw-r--r--   0        0        0     1066 2023-07-28 00:18:18.889892 cvxbson-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 cvxbson-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-07-30 19:25:02.552496 cvxbson-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2588 2023-07-30 19:25:02.552496 cvxbson-0.0.3/README.md
+-rw-r--r--   0        0        0       40 2023-07-30 19:25:02.556496 cvxbson-0.0.3/cvx/bson/__init__.py
+-rw-r--r--   0        0        0     1951 2023-07-30 19:25:02.556496 cvxbson-0.0.3/cvx/bson/file.py
+-rw-r--r--   0        0        0       40 2023-07-30 19:25:02.556496 cvxbson-0.0.3/cvx/json/__init__.py
+-rw-r--r--   0        0        0     1009 2023-07-30 19:25:02.556496 cvxbson-0.0.3/cvx/json/file.py
+-rw-r--r--   0        0        0     1066 2023-07-30 19:25:41.018683 cvxbson-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3233 1970-01-01 00:00:00.000000 cvxbson-0.0.3/PKG-INFO
```

### Comparing `cvxbson-0.0.2/LICENSE` & `cvxbson-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxbson-0.0.2/README.md` & `cvxbson-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cvxbson-0.0.2/cvx/bson/file.py` & `cvxbson-0.0.3/cvx/bson/file.py`

 * *Files identical despite different names*

### Comparing `cvxbson-0.0.2/cvx/json/file.py` & `cvxbson-0.0.3/cvx/json/file.py`

 * *Files identical despite different names*

### Comparing `cvxbson-0.0.2/pyproject.toml` & `cvxbson-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "cvxbson"
-version = "v0.0.2"
+version = "v0.0.3"
 description = "Dealing with json and bson files"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxbson"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 numpy = "*"
-requests = "*"
 numpyencoder = "*"
 pyarrow = "*"
 bson = "0.5.10"
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.2.0"
 pytest-cov = "4.0.0"
@@ -30,14 +29,15 @@
 pre-commit = "*"
 black = "23.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 loguru = "*"
 fire = "*"
+requests = "*"
 
 
 [tool.poetry.group.stubs.dependencies]
 mypy = "*"
 
 [tool.poetry.scripts]
 weather-fire = "cli.weather_fire:main"
```

### Comparing `cvxbson-0.0.2/PKG-INFO` & `cvxbson-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cvxbson
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dealing with json and bson files
 Home-page: https://github.com/cvxgrp/cvxbson
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bson (==0.5.10)
 Requires-Dist: numpy
 Requires-Dist: numpyencoder
 Requires-Dist: pyarrow
-Requires-Dist: requests
 Project-URL: Repository, https://github.com/cvxgrp/cvxbson
 Description-Content-Type: text/markdown
 
 # [cvxbson](https://www.cvxgrp.org/cvxbson/)
 
 [![PyPI version](https://badge.fury.io/py/cvxbson.svg)](https://badge.fury.io/py/cvxbson)
 [![Apache 2.0
```

