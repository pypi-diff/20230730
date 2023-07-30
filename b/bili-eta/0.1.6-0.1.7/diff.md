# Comparing `tmp/bili_eta-0.1.6.tar.gz` & `tmp/bili_eta-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.1.6.tar", max compression
+gzip compressed data, was "bili_eta-0.1.7.tar", max compression
```

## Comparing `bili_eta-0.1.6.tar` & `bili_eta-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.6/bili_eta/__init__.py
--rw-r--r--   0        0        0      946 2023-07-30 12:28:03.489510 bili_eta-0.1.6/bili_eta/__main__.py
--rw-r--r--   0        0        0      421 2023-07-30 12:15:27.190137 bili_eta-0.1.6/bili_eta/bot.py
--rw-r--r--   0        0        0      561 2023-07-30 12:30:05.805601 bili_eta-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.7/bili_eta/__init__.py
+-rw-r--r--   0        0        0      946 2023-07-30 12:28:03.489510 bili_eta-0.1.7/bili_eta/__main__.py
+-rw-r--r--   0        0        0      541 2023-07-30 12:39:21.039119 bili_eta-0.1.7/bili_eta/bot.py
+-rw-r--r--   0        0        0      561 2023-07-30 12:39:45.621749 bili_eta-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.7/PKG-INFO
```

### Comparing `bili_eta-0.1.6/bili_eta/__main__.py` & `bili_eta-0.1.7/bili_eta/__main__.py`

 * *Files identical despite different names*

### Comparing `bili_eta-0.1.6/pyproject.toml` & `bili_eta-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bili_eta-0.1.6/PKG-INFO` & `bili_eta-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-eta
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

