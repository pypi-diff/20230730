# Comparing `tmp/ctdd-0.0.6.tar.gz` & `tmp/ctdd-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdd-0.0.6.tar", max compression
+gzip compressed data, was "ctdd-0.0.7.tar", max compression
```

## Comparing `ctdd-0.0.6.tar` & `ctdd-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.6/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.6/README.md
--rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.6/ctdd/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.6/ctdd/__main__.py
--rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.6/ctdd/ffi_factory.py
--rw-r--r--   0        0        0     1663 2023-07-13 11:47:07.434036 ctdd-0.0.6/ctdd/mocker.py
--rw-r--r--   0        0        0     2764 2023-07-17 12:11:04.503502 ctdd-0.0.6/ctdd/tester.py
--rw-r--r--   0        0        0     3088 2023-07-17 12:11:57.942213 ctdd-0.0.6/ctdd/tester_state.py
--rw-r--r--   0        0        0      736 2023-07-17 13:15:03.287677 ctdd-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.7/README.md
+-rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.7/ctdd/__init__.py
+-rw-r--r--   0        0        0     6426 2023-07-30 16:24:00.491814 ctdd-0.0.7/ctdd/__main__.py
+-rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.7/ctdd/ffi_factory.py
+-rw-r--r--   0        0        0     1663 2023-07-13 11:47:07.434036 ctdd-0.0.7/ctdd/mocker.py
+-rw-r--r--   0        0        0     2764 2023-07-29 12:08:37.412653 ctdd-0.0.7/ctdd/tester.py
+-rw-r--r--   0        0        0     3088 2023-07-17 12:11:57.942213 ctdd-0.0.7/ctdd/tester_state.py
+-rw-r--r--   0        0        0      736 2023-07-30 16:25:01.584272 ctdd-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.7/PKG-INFO
```

### Comparing `ctdd-0.0.6/LICENSE` & `ctdd-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.6/README.md` & `ctdd-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.6/ctdd/ffi_factory.py` & `ctdd-0.0.7/ctdd/ffi_factory.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.6/ctdd/mocker.py` & `ctdd-0.0.7/ctdd/mocker.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.6/ctdd/tester.py` & `ctdd-0.0.7/ctdd/tester.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.6/ctdd/tester_state.py` & `ctdd-0.0.7/ctdd/tester_state.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.6/pyproject.toml` & `ctdd-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctdd"
-version = "0.0.6"
+version = "0.0.7"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ctdd-0.0.6/PKG-INFO` & `ctdd-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctdd
-Version: 0.0.6
+Version: 0.0.7
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/ctdd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

