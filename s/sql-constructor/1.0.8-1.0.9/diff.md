# Comparing `tmp/sql_constructor-1.0.8.tar.gz` & `tmp/sql_constructor-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_constructor-1.0.8.tar", last modified: Sun Jul 30 16:47:51 2023, max compression
+gzip compressed data, was "sql_constructor-1.0.9.tar", last modified: Sun Jul 30 16:49:41 2023, max compression
```

## Comparing `sql_constructor-1.0.8.tar` & `sql_constructor-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:47:51.283821 sql_constructor-1.0.8/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.8/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8577 2023-07-30 16:47:51.283821 sql_constructor-1.0.8/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     7824 2023-07-30 16:47:29.000000 sql_constructor-1.0.8/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      827 2023-07-30 16:47:06.000000 sql_constructor-1.0.8/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 16:47:51.283821 sql_constructor-1.0.8/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:47:51.281821 sql_constructor-1.0.8/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:47:51.282821 sql_constructor-1.0.8/src/sql_constructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.8/src/sql_constructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.8/src/sql_constructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.8/src/sql_constructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.8/src/sql_constructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.8/src/sql_constructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.8/src/sql_constructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.8/src/sql_constructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:47:51.283821 sql_constructor-1.0.8/src/sql_constructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8577 2023-07-30 16:47:51.000000 sql_constructor-1.0.8/src/sql_constructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 16:47:51.000000 sql_constructor-1.0.8/src/sql_constructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 16:47:51.000000 sql_constructor-1.0.8/src/sql_constructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 16:47:51.000000 sql_constructor-1.0.8/src/sql_constructor.egg-info/top_level.txt
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:49:41.196119 sql_constructor-1.0.9/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.9/LICENSE
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8577 2023-07-30 16:49:41.195119 sql_constructor-1.0.9/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     7824 2023-07-30 16:47:29.000000 sql_constructor-1.0.9/README.md
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      827 2023-07-30 16:49:20.000000 sql_constructor-1.0.9/pyproject.toml
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 16:49:41.196119 sql_constructor-1.0.9/setup.cfg
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:49:41.194119 sql_constructor-1.0.9/src/
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:49:41.195119 sql_constructor-1.0.9/src/sql_constructor/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.9/src/sql_constructor/__init__.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.9/src/sql_constructor/constants.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.9/src/sql_constructor/helpers.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.9/src/sql_constructor/sql_container.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.9/src/sql_constructor/sql_cte.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.9/src/sql_constructor/sql_query.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.9/src/sql_constructor/sql_section.py
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:49:41.195119 sql_constructor-1.0.9/src/sql_constructor.egg-info/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8577 2023-07-30 16:49:41.000000 sql_constructor-1.0.9/src/sql_constructor.egg-info/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 16:49:41.000000 sql_constructor-1.0.9/src/sql_constructor.egg-info/SOURCES.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 16:49:41.000000 sql_constructor-1.0.9/src/sql_constructor.egg-info/dependency_links.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 16:49:41.000000 sql_constructor-1.0.9/src/sql_constructor.egg-info/top_level.txt
```

### Comparing `sql_constructor-1.0.8/LICENSE` & `sql_constructor-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/PKG-INFO` & `sql_constructor-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sql_constructor
-Version: 1.0.8
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
+Version: 1.0.9
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sql_constructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sql_constructor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sql_constructor-1.0.8/README.md` & `sql_constructor-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/pyproject.toml` & `sql_constructor-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sql_constructor"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
-description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!"
+description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sql_constructor-1.0.8/src/sql_constructor/constants.py` & `sql_constructor-1.0.9/src/sql_constructor/constants.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/src/sql_constructor/helpers.py` & `sql_constructor-1.0.9/src/sql_constructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/src/sql_constructor/sql_container.py` & `sql_constructor-1.0.9/src/sql_constructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/src/sql_constructor/sql_cte.py` & `sql_constructor-1.0.9/src/sql_constructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/src/sql_constructor/sql_query.py` & `sql_constructor-1.0.9/src/sql_constructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/src/sql_constructor/sql_section.py` & `sql_constructor-1.0.9/src/sql_constructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.8/src/sql_constructor.egg-info/PKG-INFO` & `sql_constructor-1.0.9/src/sql_constructor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sql-constructor
-Version: 1.0.8
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
+Version: 1.0.9
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sql_constructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sql_constructor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

