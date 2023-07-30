# Comparing `tmp/examon_core-1.1.0.tar.gz` & `tmp/examon_core-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.1.0.tar", max compression
+gzip compressed data, was "examon_core-1.1.1.tar", max compression
```

## Comparing `examon_core-1.1.0.tar` & `examon_core-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      225 2023-07-28 15:55:25.250080 examon_core-1.1.0/examon_core/__init__.py
--rwxr-xr-x   0        0        0     1908 2023-07-30 15:28:57.756531 examon_core-1.1.0/examon_core/code_as_string_factory.py
--rw-r--r--   0        0        0     1301 2023-07-30 18:35:51.460062 examon_core-1.1.0/examon_core/code_execution_sandbox.py
--rw-r--r--   0        0        0     1671 2023-07-30 08:22:25.918054 examon_core-1.1.0/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.1.0/examon_core/examon_item.py
--rwxr-xr-x   0        0        0     2085 2023-07-30 15:20:51.926942 examon_core-1.1.0/examon_core/examon_item_registry.py
--rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.1.0/examon_core/multi_choice_factory.py
--rwxr-xr-x   0        0        0      617 2023-07-30 15:10:40.198476 examon_core-1.1.0/examon_core/question.py
--rw-r--r--   0        0        0     3000 2023-07-30 18:20:40.962231 examon_core-1.1.0/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.1.0/examon_core/question_response.py
--rw-r--r--   0        0        0      550 2023-07-30 18:39:40.266777 examon_core-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      225 2023-07-28 15:55:25.250080 examon_core-1.1.1/examon_core/__init__.py
+-rwxr-xr-x   0        0        0     1908 2023-07-30 15:28:57.756531 examon_core-1.1.1/examon_core/code_as_string_factory.py
+-rw-r--r--   0        0        0     1301 2023-07-30 18:35:51.460062 examon_core-1.1.1/examon_core/code_execution_sandbox.py
+-rw-r--r--   0        0        0     1671 2023-07-30 08:22:25.918054 examon_core-1.1.1/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.1.1/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0     2085 2023-07-30 15:20:51.926942 examon_core-1.1.1/examon_core/examon_item_registry.py
+-rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.1.1/examon_core/multi_choice_factory.py
+-rwxr-xr-x   0        0        0      617 2023-07-30 15:10:40.198476 examon_core-1.1.1/examon_core/question.py
+-rw-r--r--   0        0        0     3000 2023-07-30 18:20:40.962231 examon_core-1.1.1/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.1.1/examon_core/question_response.py
+-rw-r--r--   0        0        0      544 2023-07-30 18:48:54.898149 examon_core-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 examon_core-1.1.1/PKG-INFO
```

### Comparing `examon_core-1.1.0/examon_core/code_as_string_factory.py` & `examon_core-1.1.1/examon_core/code_as_string_factory.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/examon_core/code_execution_sandbox.py` & `examon_core-1.1.1/examon_core/code_execution_sandbox.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/examon_core/code_metrics.py` & `examon_core-1.1.1/examon_core/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/examon_core/examon_item.py` & `examon_core-1.1.1/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/examon_core/examon_item_registry.py` & `examon_core-1.1.1/examon_core/examon_item_registry.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/examon_core/question.py` & `examon_core-1.1.1/examon_core/question.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/examon_core/question_factory.py` & `examon_core-1.1.1/examon_core/question_factory.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.0/pyproject.toml` & `examon_core-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "examon_core"
-version = "1.1.0"
+version = "1.1.1"
 description = "Examon Core Libs"
 authors = ["Jarrod Folino <jdfolino@icloud.com>"]
 packages = [{include = "examon_core"}]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9"
 radon = "^6.0.1"
 dataclasses-serialization = "^1.3.1"
 restrictedpython = "^6.1"
 
 [[tool.poetry.source]]
 name = "test"
 url = "https://test.pypi.org/simple/"
```

