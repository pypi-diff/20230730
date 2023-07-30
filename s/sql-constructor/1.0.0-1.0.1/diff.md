# Comparing `tmp/sql_constructor-1.0.0.tar.gz` & `tmp/sql_constructor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_constructor-1.0.0.tar", last modified: Sun Jul 30 07:16:45 2023, max compression
+gzip compressed data, was "sql_constructor-1.0.1.tar", last modified: Sun Jul 30 08:11:31 2023, max compression
```

## Comparing `sql_constructor-1.0.0.tar` & `sql_constructor-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 07:16:45.743848 sql_constructor-1.0.0/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-18 03:54:55.000000 sql_constructor-1.0.0/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1084 2023-07-30 07:16:45.743848 sql_constructor-1.0.0/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      348 2023-07-18 03:54:55.000000 sql_constructor-1.0.0/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      810 2023-07-30 07:15:22.000000 sql_constructor-1.0.0/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 07:16:45.743848 sql_constructor-1.0.0/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 07:16:45.741848 sql_constructor-1.0.0/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 07:16:45.743848 sql_constructor-1.0.0/src/sql_constructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:10:48.000000 sql_constructor-1.0.0/src/sql_constructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.0/src/sql_constructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.0/src/sql_constructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5120 2023-07-30 06:25:04.000000 sql_constructor-1.0.0/src/sql_constructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.0/src/sql_constructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.0/src/sql_constructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.0/src/sql_constructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 07:16:45.743848 sql_constructor-1.0.0/src/sql_constructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1084 2023-07-30 07:16:45.000000 sql_constructor-1.0.0/src/sql_constructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 07:16:45.000000 sql_constructor-1.0.0/src/sql_constructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 07:16:45.000000 sql_constructor-1.0.0/src/sql_constructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 07:16:45.000000 sql_constructor-1.0.0/src/sql_constructor.egg-info/top_level.txt
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.979083 sql_constructor-1.0.1/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.1/LICENSE
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1088 2023-07-30 08:11:31.979083 sql_constructor-1.0.1/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      348 2023-07-18 03:54:55.000000 sql_constructor-1.0.1/README.md
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      814 2023-07-30 08:11:06.000000 sql_constructor-1.0.1/pyproject.toml
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 08:11:31.979083 sql_constructor-1.0.1/setup.cfg
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.977083 sql_constructor-1.0.1/src/
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.978083 sql_constructor-1.0.1/src/sql_constructor/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.1/src/sql_constructor/__init__.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.1/src/sql_constructor/constants.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.1/src/sql_constructor/helpers.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5120 2023-07-30 06:25:04.000000 sql_constructor-1.0.1/src/sql_constructor/sql_container.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.1/src/sql_constructor/sql_cte.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.1/src/sql_constructor/sql_query.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.1/src/sql_constructor/sql_section.py
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.978083 sql_constructor-1.0.1/src/sql_constructor.egg-info/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1088 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/SOURCES.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/dependency_links.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/top_level.txt
```

### Comparing `sql_constructor-1.0.0/LICENSE` & `sql_constructor-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/PKG-INFO` & `sql_constructor-1.0.1/src/sql_constructor.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: sql_constructor
-Version: 1.0.0
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to and be constracted dynamicly. You could also build request once and cache it (and sql_constractor let you change passed parameters in cached SQL request).
+Name: sql-constructor
+Version: 1.0.1
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty. You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sql_constractor
 Project-URL: Bug Tracker, https://github.com/akvilary/sql_constractor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sql_constructor-1.0.0/src/sql_constructor/constants.py` & `sql_constructor-1.0.1/src/sql_constructor/constants.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/src/sql_constructor/helpers.py` & `sql_constructor-1.0.1/src/sql_constructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/src/sql_constructor/sql_container.py` & `sql_constructor-1.0.1/src/sql_constructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/src/sql_constructor/sql_cte.py` & `sql_constructor-1.0.1/src/sql_constructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/src/sql_constructor/sql_query.py` & `sql_constructor-1.0.1/src/sql_constructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/src/sql_constructor/sql_section.py` & `sql_constructor-1.0.1/src/sql_constructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.0/src/sql_constructor.egg-info/PKG-INFO` & `sql_constructor-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: sql-constructor
-Version: 1.0.0
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to and be constracted dynamicly. You could also build request once and cache it (and sql_constractor let you change passed parameters in cached SQL request).
+Name: sql_constructor
+Version: 1.0.1
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty. You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sql_constractor
 Project-URL: Bug Tracker, https://github.com/akvilary/sql_constractor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

