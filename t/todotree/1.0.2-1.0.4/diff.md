# Comparing `tmp/todotree-1.0.2.tar.gz` & `tmp/todotree-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todotree-1.0.2.tar", max compression
+gzip compressed data, was "todotree-1.0.4.tar", max compression
```

## Comparing `todotree-1.0.2.tar` & `todotree-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1211 2023-07-30 08:50:14.009923 todotree-1.0.2/LICENSE
--rw-r--r--   0        0        0     1855 2023-07-30 08:50:14.009923 todotree-1.0.2/README.md
--rw-r--r--   0        0        0     2169 2023-07-30 08:50:34.122963 todotree-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      196 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Errors/ProjectFolderError.py
--rw-r--r--   0        0        0      180 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Errors/TaskParseError.py
--rw-r--r--   0        0        0      198 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Errors/WishListFolderError.py
--rw-r--r--   0        0        0        0 2023-07-30 08:50:14.044904 todotree-1.0.2/todotree/Errors/__init__.py
--rw-r--r--   0        0        0    12425 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Task.py
--rw-r--r--   0        0        0    11122 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Taskmanager.py
--rw-r--r--   0        0        0     4493 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Tree.py
--rw-r--r--   0        0        0        0 2023-07-30 08:50:14.044904 todotree-1.0.2/todotree/__init__.py
--rw-r--r--   0        0        0     5960 2023-07-30 08:50:14.015920 todotree-1.0.2/todotree/config.py
--rwxr-xr-x   0        0        0    10611 2023-07-30 08:50:14.015920 todotree-1.0.2/todotree/main.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 todotree-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-30 09:39:41.168573 todotree-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1855 2023-07-30 09:39:41.168573 todotree-1.0.4/README.md
+-rw-r--r--   0        0        0     2169 2023-07-30 09:40:02.068727 todotree-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Errors/ProjectFolderError.py
+-rw-r--r--   0        0        0      180 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Errors/TaskParseError.py
+-rw-r--r--   0        0        0      198 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Errors/WishListFolderError.py
+-rw-r--r--   0        0        0        0 2023-07-30 09:39:41.204573 todotree-1.0.4/todotree/Errors/__init__.py
+-rw-r--r--   0        0        0    12425 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Task.py
+-rw-r--r--   0        0        0    11122 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Taskmanager.py
+-rw-r--r--   0        0        0     4493 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Tree.py
+-rw-r--r--   0        0        0        0 2023-07-30 09:39:41.204573 todotree-1.0.4/todotree/__init__.py
+-rw-r--r--   0        0        0     5960 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/config.py
+-rwxr-xr-x   0        0        0    10611 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/main.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 todotree-1.0.4/PKG-INFO
```

### Comparing `todotree-1.0.2/LICENSE` & `todotree-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/README.md` & `todotree-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/pyproject.toml` & `todotree-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todotree"
-version = "1.0.2"
+version = "1.0.4"
 description = "todo.txt manager which adds tree printing"
 authors = ["chim1aap <fkjansen@protonmail.com>"]
 repository = "https://gitlab.com/chim1aap/todotree"
 documentation = "https://chim1aap.gitlab.io/todotree/"
 readme = "README.md"
 packages = [
   {include = "todotree"}
```

### Comparing `todotree-1.0.2/todotree/Task.py` & `todotree-1.0.4/todotree/Task.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/todotree/Taskmanager.py` & `todotree-1.0.4/todotree/Taskmanager.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/todotree/Tree.py` & `todotree-1.0.4/todotree/Tree.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/todotree/config.py` & `todotree-1.0.4/todotree/config.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/todotree/main.py` & `todotree-1.0.4/todotree/main.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.2/PKG-INFO` & `todotree-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todotree
-Version: 1.0.2
+Version: 1.0.4
 Summary: todo.txt manager which adds tree printing
 Home-page: https://gitlab.com/chim1aap/todotree
 Author: chim1aap
 Author-email: fkjansen@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

