# Comparing `tmp/gs_sql-0.0.2.tar.gz` & `tmp/gs_sql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_sql-0.0.2.tar", last modified: Sat Jul 29 18:20:58 2023, max compression
+gzip compressed data, was "gs_sql-0.0.3.tar", last modified: Sun Jul 30 18:34:11 2023, max compression
```

## Comparing `gs_sql-0.0.2.tar` & `gs_sql-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 18:20:58.957828 gs_sql-0.0.2/
--rw-rw-rw-   0        0        0     1041 2023-07-29 18:20:58.958670 gs_sql-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 18:20:58.785719 gs_sql-0.0.2/gs_sql/
--rw-rw-rw-   0        0        0     1830 2023-07-04 18:01:38.000000 gs_sql-0.0.2/gs_sql/BaseData.py
--rw-rw-rw-   0        0        0     1361 2023-07-03 13:07:41.000000 gs_sql-0.0.2/gs_sql/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-29 18:20:58.878788 gs_sql-0.0.2/gs_sql/Tests/
--rw-rw-rw-   0        0        0        0 2023-07-03 17:18:10.000000 gs_sql-0.0.2/gs_sql/Tests/__init__.py
--rw-rw-rw-   0        0        0     1180 2023-07-08 19:26:49.000000 gs_sql-0.0.2/gs_sql/Tests/unit_tests.py
--rw-rw-rw-   0        0        0       30 2023-07-22 19:34:22.000000 gs_sql-0.0.2/gs_sql/__init__.py
--rw-rw-rw-   0        0        0     1110 2023-07-03 13:48:24.000000 gs_sql-0.0.2/gs_sql/authorization.py
--rw-rw-rw-   0        0        0      115 2023-07-22 18:33:44.000000 gs_sql-0.0.2/gs_sql/configuration.py
--rw-rw-rw-   0        0        0     8370 2023-07-07 20:07:54.000000 gs_sql-0.0.2/gs_sql/data_difinition.py
--rw-rw-rw-   0        0        0     8274 2023-07-22 18:32:10.000000 gs_sql-0.0.2/gs_sql/data_manipulation.py
--rw-rw-rw-   0        0        0      554 2023-07-08 11:58:11.000000 gs_sql-0.0.2/gs_sql/dataclasses.py
-drwxrwxrwx   0        0        0        0 2023-07-29 18:20:58.901158 gs_sql-0.0.2/gs_sql/pandasql/
--rw-rw-rw-   0        0        0      417 2023-06-26 12:20:53.000000 gs_sql-0.0.2/gs_sql/pandasql/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-06-26 12:20:53.000000 gs_sql-0.0.2/gs_sql/pandasql/sqldf.py
-drwxrwxrwx   0        0        0        0 2023-07-29 18:20:58.956617 gs_sql-0.0.2/gs_sql/pandasql/tests/
--rw-rw-rw-   0        0        0        0 2023-06-26 12:20:53.000000 gs_sql-0.0.2/gs_sql/pandasql/tests/__init__.py
--rw-rw-rw-   0        0        0     7352 2023-06-26 12:20:53.000000 gs_sql-0.0.2/gs_sql/pandasql/tests/test_pandasql.py
--rw-rw-rw-   0        0        0     1180 2023-06-26 12:20:53.000000 gs_sql-0.0.2/gs_sql/pandasql/tests/test_utils.py
--rw-rw-rw-   0        0        0     1243 2023-07-08 19:45:30.000000 gs_sql-0.0.2/gs_sql/sheetsql.py
--rw-rw-rw-   0        0        0     8404 2023-07-22 18:32:58.000000 gs_sql-0.0.2/gs_sql/sql_parser.py
-drwxrwxrwx   0        0        0        0 2023-07-29 18:20:58.860964 gs_sql-0.0.2/gs_sql.egg-info/
--rw-rw-rw-   0        0        0     1041 2023-07-29 18:20:58.000000 gs_sql-0.0.2/gs_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      604 2023-07-29 18:20:58.000000 gs_sql-0.0.2/gs_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 18:20:58.000000 gs_sql-0.0.2/gs_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 18:20:58.000000 gs_sql-0.0.2/gs_sql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-29 18:20:58.000000 gs_sql-0.0.2/gs_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 18:20:58.960659 gs_sql-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1263 2023-07-29 18:20:51.000000 gs_sql-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.176723 gs_sql-0.0.3/
+-rw-rw-rw-   0        0        0     7152 2023-07-30 18:34:11.176723 gs_sql-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6121 2023-07-30 13:16:07.000000 gs_sql-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.000702 gs_sql-0.0.3/gs_sql/
+-rw-rw-rw-   0        0        0     1830 2023-07-04 18:01:38.000000 gs_sql-0.0.3/gs_sql/BaseData.py
+-rw-rw-rw-   0        0        0     1361 2023-07-03 13:07:41.000000 gs_sql-0.0.3/gs_sql/Exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.154785 gs_sql-0.0.3/gs_sql/Tests/
+-rw-rw-rw-   0        0        0        0 2023-07-03 17:18:10.000000 gs_sql-0.0.3/gs_sql/Tests/__init__.py
+-rw-rw-rw-   0        0        0     1180 2023-07-08 19:26:49.000000 gs_sql-0.0.3/gs_sql/Tests/unit_tests.py
+-rw-rw-rw-   0        0        0       30 2023-07-22 19:34:22.000000 gs_sql-0.0.3/gs_sql/__init__.py
+-rw-rw-rw-   0        0        0     1110 2023-07-03 13:48:24.000000 gs_sql-0.0.3/gs_sql/authorization.py
+-rw-rw-rw-   0        0        0      115 2023-07-22 18:33:44.000000 gs_sql-0.0.3/gs_sql/configuration.py
+-rw-rw-rw-   0        0        0     8370 2023-07-07 20:07:54.000000 gs_sql-0.0.3/gs_sql/data_difinition.py
+-rw-rw-rw-   0        0        0     8274 2023-07-22 18:32:10.000000 gs_sql-0.0.3/gs_sql/data_manipulation.py
+-rw-rw-rw-   0        0        0      554 2023-07-08 11:58:11.000000 gs_sql-0.0.3/gs_sql/dataclasses.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.170420 gs_sql-0.0.3/gs_sql/pandasql/
+-rw-rw-rw-   0        0        0      417 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/__init__.py
+-rw-rw-rw-   0        0        0     5563 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/sqldf.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.176226 gs_sql-0.0.3/gs_sql/pandasql/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/tests/__init__.py
+-rw-rw-rw-   0        0        0     7352 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/tests/test_pandasql.py
+-rw-rw-rw-   0        0        0     1180 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/tests/test_utils.py
+-rw-rw-rw-   0        0        0     1243 2023-07-08 19:45:30.000000 gs_sql-0.0.3/gs_sql/sheetsql.py
+-rw-rw-rw-   0        0        0     8404 2023-07-22 18:32:58.000000 gs_sql-0.0.3/gs_sql/sql_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.119843 gs_sql-0.0.3/gs_sql.egg-info/
+-rw-rw-rw-   0        0        0     7152 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 18:30:11.000000 gs_sql-0.0.3/gs_sql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 18:34:11.196792 gs_sql-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-30 18:34:04.000000 gs_sql-0.0.3/setup.py
```

### Comparing `gs_sql-0.0.2/gs_sql/BaseData.py` & `gs_sql-0.0.3/gs_sql/BaseData.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/Exceptions.py` & `gs_sql-0.0.3/gs_sql/Exceptions.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/Tests/unit_tests.py` & `gs_sql-0.0.3/gs_sql/Tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/authorization.py` & `gs_sql-0.0.3/gs_sql/authorization.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/data_difinition.py` & `gs_sql-0.0.3/gs_sql/data_difinition.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/data_manipulation.py` & `gs_sql-0.0.3/gs_sql/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/dataclasses.py` & `gs_sql-0.0.3/gs_sql/dataclasses.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/pandasql/sqldf.py` & `gs_sql-0.0.3/gs_sql/pandasql/sqldf.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/pandasql/tests/test_pandasql.py` & `gs_sql-0.0.3/gs_sql/pandasql/tests/test_pandasql.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/pandasql/tests/test_utils.py` & `gs_sql-0.0.3/gs_sql/pandasql/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/sheetsql.py` & `gs_sql-0.0.3/gs_sql/sheetsql.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql/sql_parser.py` & `gs_sql-0.0.3/gs_sql/sql_parser.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.2/gs_sql.egg-info/SOURCES.txt` & `gs_sql-0.0.3/gs_sql.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.cfg
 setup.py
 gs_sql/BaseData.py
 gs_sql/Exceptions.py
 gs_sql/__init__.py
 gs_sql/authorization.py
 gs_sql/configuration.py
```

