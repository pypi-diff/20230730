# Comparing `tmp/sqlx-exec-1.3.3.tar.gz` & `tmp/sqlx-exec-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.3.3.tar", last modified: Sun Jul 30 02:01:17 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.3.5.tar", last modified: Sun Jul 30 02:03:51 2023, max compression
```

## Comparing `sqlx-exec-1.3.3.tar` & `sqlx-exec-1.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     3466 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2023-07-30 02:01:09.000000 sqlx-exec-1.3.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-30 02:01:15.000000 sqlx-exec-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/sqlexec/
--rw-rw-rw-   0        0        0      774 2023-07-29 16:19:11.000000 sqlx-exec-1.3.3/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.3/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11642 2023-07-29 16:19:11.000000 sqlx-exec-1.3.3/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.3/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.3/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.3/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.3/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.3/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.3/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.3/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3466 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 02:01:17.000000 sqlx-exec-1.3.3/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0     3469 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2922 2023-07-30 02:03:45.000000 sqlx-exec-1.3.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-30 02:03:45.000000 sqlx-exec-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/sqlexec/
+-rw-rw-rw-   0        0        0      774 2023-07-29 16:19:11.000000 sqlx-exec-1.3.5/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.5/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11642 2023-07-29 16:19:11.000000 sqlx-exec-1.3.5/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.5/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.5/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.5/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.5/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.5/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.5/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.5/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3469 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 02:03:51.000000 sqlx-exec-1.3.5/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.3.3/LICENSE` & `sqlx-exec-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/PKG-INFO` & `sqlx-exec-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.3
+Version: 1.3.5
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
        # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
        # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
-       sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
+       sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.3.3/README.rst` & `sqlx-exec-1.3.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
        # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
        # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
-       sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
+       sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.3.3/setup.py` & `sqlx-exec-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.3',
+    version='1.3.5',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.3.3/sqlexec/constant.py` & `sqlx-exec-1.3.5/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/engine.py` & `sqlx-exec-1.3.5/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/exec.py` & `sqlx-exec-1.3.5/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/init_import.py` & `sqlx-exec-1.3.5/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/log_support.py` & `sqlx-exec-1.3.5/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/pooling.py` & `sqlx-exec-1.3.5/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/sql_support.py` & `sqlx-exec-1.3.5/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlexec/support.py` & `sqlx-exec-1.3.5/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.3/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.3.5/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.3
+Version: 1.3.5
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
        # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
        # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
-       sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
+       sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

