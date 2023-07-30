# Comparing `tmp/seagoat-0.8.0.tar.gz` & `tmp/seagoat-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.8.0.tar", max compression
+gzip compressed data, was "seagoat-0.8.8.tar", max compression
```

## Comparing `seagoat-0.8.0.tar` & `seagoat-0.8.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-30 17:23:50.180361 seagoat-0.8.0/LICENSE
--rw-r--r--   0        0        0     1847 2023-07-30 17:23:50.184361 seagoat-0.8.0/README.md
--rw-r--r--   0        0        0     3085 2023-07-30 17:23:50.980374 seagoat-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-30 17:23:50.980374 seagoat-0.8.0/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/cache.py
--rw-r--r--   0        0        0     2901 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/common.py
--rw-r--r--   0        0        0     4424 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/server.py
--rw-r--r--   0        0        0     1692 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1105 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 20:20:21.979702 seagoat-0.8.8/LICENSE
+-rw-r--r--   0        0        0     1847 2023-07-30 20:20:21.979702 seagoat-0.8.8/README.md
+-rw-r--r--   0        0        0     3085 2023-07-30 20:20:22.743705 seagoat-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-30 20:20:22.743705 seagoat-0.8.8/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-30 20:20:21.983702 seagoat-0.8.8/seagoat/cache.py
+-rw-r--r--   0        0        0     2901 2023-07-30 20:20:21.983702 seagoat-0.8.8/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-30 20:20:21.983702 seagoat-0.8.8/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-07-30 20:20:21.983702 seagoat-0.8.8/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-30 20:20:21.983702 seagoat-0.8.8/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-30 20:20:21.983702 seagoat-0.8.8/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-30 20:20:21.987702 seagoat-0.8.8/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-07-30 20:20:21.987702 seagoat-0.8.8/seagoat/server.py
+-rw-r--r--   0        0        0     1692 2023-07-30 20:20:21.987702 seagoat-0.8.8/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-07-30 20:20:21.987702 seagoat-0.8.8/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.8.8/PKG-INFO
```

### Comparing `seagoat-0.8.0/LICENSE` & `seagoat-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/README.md` & `seagoat-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/pyproject.toml` & `seagoat-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.8.0"
+version = "0.8.8"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
```

### Comparing `seagoat-0.8.0/seagoat/cache.py` & `seagoat-0.8.8/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/cli.py` & `seagoat-0.8.8/seagoat/cli.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/engine.py` & `seagoat-0.8.8/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/file.py` & `seagoat-0.8.8/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/repository.py` & `seagoat-0.8.8/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/result.py` & `seagoat-0.8.8/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/server.py` & `seagoat-0.8.8/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/sources/chroma.py` & `seagoat-0.8.8/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/seagoat/sources/ripgrep.py` & `seagoat-0.8.8/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.0/PKG-INFO` & `seagoat-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.8.0
+Version: 0.8.8
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

