# Comparing `tmp/sql_constructor-1.0.4.tar.gz` & `tmp/sql_constructor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_constructor-1.0.4.tar", last modified: Sun Jul 30 10:17:55 2023, max compression
+gzip compressed data, was "sql_constructor-1.0.5.tar", last modified: Sun Jul 30 10:19:30 2023, max compression
```

## Comparing `sql_constructor-1.0.4.tar` & `sql_constructor-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:17:55.651271 sql_constructor-1.0.4/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.4/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4740 2023-07-30 10:17:55.651271 sql_constructor-1.0.4/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4000 2023-07-30 10:17:04.000000 sql_constructor-1.0.4/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      814 2023-07-30 10:17:11.000000 sql_constructor-1.0.4/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 10:17:55.651271 sql_constructor-1.0.4/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:17:55.649271 sql_constructor-1.0.4/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:17:55.650271 sql_constructor-1.0.4/src/sql_constructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.4/src/sql_constructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.4/src/sql_constructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.4/src/sql_constructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.4/src/sql_constructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.4/src/sql_constructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.4/src/sql_constructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.4/src/sql_constructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:17:55.651271 sql_constructor-1.0.4/src/sql_constructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4740 2023-07-30 10:17:55.000000 sql_constructor-1.0.4/src/sql_constructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 10:17:55.000000 sql_constructor-1.0.4/src/sql_constructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 10:17:55.000000 sql_constructor-1.0.4/src/sql_constructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 10:17:55.000000 sql_constructor-1.0.4/src/sql_constructor.egg-info/top_level.txt
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:19:30.188274 sql_constructor-1.0.5/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.5/LICENSE
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4740 2023-07-30 10:19:30.188274 sql_constructor-1.0.5/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4000 2023-07-30 10:17:04.000000 sql_constructor-1.0.5/README.md
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      814 2023-07-30 10:19:02.000000 sql_constructor-1.0.5/pyproject.toml
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 10:19:30.188274 sql_constructor-1.0.5/setup.cfg
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:19:30.187274 sql_constructor-1.0.5/src/
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:19:30.188274 sql_constructor-1.0.5/src/sql_constructor/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.5/src/sql_constructor/__init__.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.5/src/sql_constructor/constants.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.5/src/sql_constructor/helpers.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.5/src/sql_constructor/sql_container.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.5/src/sql_constructor/sql_cte.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.5/src/sql_constructor/sql_query.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.5/src/sql_constructor/sql_section.py
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:19:30.188274 sql_constructor-1.0.5/src/sql_constructor.egg-info/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4740 2023-07-30 10:19:30.000000 sql_constructor-1.0.5/src/sql_constructor.egg-info/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 10:19:30.000000 sql_constructor-1.0.5/src/sql_constructor.egg-info/SOURCES.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 10:19:30.000000 sql_constructor-1.0.5/src/sql_constructor.egg-info/dependency_links.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 10:19:30.000000 sql_constructor-1.0.5/src/sql_constructor.egg-info/top_level.txt
```

### Comparing `sql_constructor-1.0.4/LICENSE` & `sql_constructor-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/PKG-INFO` & `sql_constructor-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sql_constructor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
-Project-URL: Homepage, https://github.com/akvilary/sql_constractor
-Project-URL: Bug Tracker, https://github.com/akvilary/sql_constractor/issues
+Project-URL: Homepage, https://github.com/akvilary/sql_constructor
+Project-URL: Bug Tracker, https://github.com/akvilary/sql_constructor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sql_constructor-1.0.4/README.md` & `sql_constructor-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/pyproject.toml` & `sql_constructor-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sql_constructor"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/akvilary/sql_constractor"
-"Bug Tracker" = "https://github.com/akvilary/sql_constractor/issues"
+"Homepage" = "https://github.com/akvilary/sql_constructor"
+"Bug Tracker" = "https://github.com/akvilary/sql_constructor/issues"
```

### Comparing `sql_constructor-1.0.4/src/sql_constructor/constants.py` & `sql_constructor-1.0.5/src/sql_constructor/constants.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/src/sql_constructor/helpers.py` & `sql_constructor-1.0.5/src/sql_constructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/src/sql_constructor/sql_container.py` & `sql_constructor-1.0.5/src/sql_constructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/src/sql_constructor/sql_cte.py` & `sql_constructor-1.0.5/src/sql_constructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/src/sql_constructor/sql_query.py` & `sql_constructor-1.0.5/src/sql_constructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/src/sql_constructor/sql_section.py` & `sql_constructor-1.0.5/src/sql_constructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.4/src/sql_constructor.egg-info/PKG-INFO` & `sql_constructor-1.0.5/src/sql_constructor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sql-constructor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
-Project-URL: Homepage, https://github.com/akvilary/sql_constractor
-Project-URL: Bug Tracker, https://github.com/akvilary/sql_constractor/issues
+Project-URL: Homepage, https://github.com/akvilary/sql_constructor
+Project-URL: Bug Tracker, https://github.com/akvilary/sql_constructor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

