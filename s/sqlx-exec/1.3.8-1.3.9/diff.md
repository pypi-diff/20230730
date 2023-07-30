# Comparing `tmp/sqlx-exec-1.3.8.tar.gz` & `tmp/sqlx-exec-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.3.8.tar", last modified: Sun Jul 30 08:34:42 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.3.9.tar", last modified: Sun Jul 30 08:37:21 2023, max compression
```

## Comparing `sqlx-exec-1.3.8.tar` & `sqlx-exec-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     3779 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.3.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1283 2023-07-30 08:33:52.000000 sqlx-exec-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlexec/
--rw-rw-rw-   0        0        0      898 2023-07-30 03:48:03.000000 sqlx-exec-1.3.8/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.8/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11676 2023-07-30 08:23:35.000000 sqlx-exec-1.3.8/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.8/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.8/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.8/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.8/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.8/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.8/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3779 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     3728 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.3.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-07-30 08:37:11.000000 sqlx-exec-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlexec/
+-rw-rw-rw-   0        0        0      898 2023-07-30 03:48:03.000000 sqlx-exec-1.3.9/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.9/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11676 2023-07-30 08:23:35.000000 sqlx-exec-1.3.9/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.9/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.9/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.9/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.9/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.9/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.9/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3728 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.3.8/LICENSE` & `sqlx-exec-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/PKG-INFO` & `sqlx-exec-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.8
-Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
+Version: 1.3.9
+Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `sqlx-exec-1.3.8/README.rst` & `sqlx-exec-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/setup.py` & `sqlx-exec-1.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
-    description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
+    description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.8',
+    version='1.3.9',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.3.8/sqlexec/constant.py` & `sqlx-exec-1.3.9/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/engine.py` & `sqlx-exec-1.3.9/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/exec.py` & `sqlx-exec-1.3.9/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/init_import.py` & `sqlx-exec-1.3.9/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/log_support.py` & `sqlx-exec-1.3.9/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/pooling.py` & `sqlx-exec-1.3.9/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/sql_support.py` & `sqlx-exec-1.3.9/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlexec/support.py` & `sqlx-exec-1.3.9/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.8/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.3.9/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.8
-Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
+Version: 1.3.9
+Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

