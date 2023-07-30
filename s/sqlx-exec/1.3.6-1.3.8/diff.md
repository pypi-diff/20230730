# Comparing `tmp/sqlx-exec-1.3.6.tar.gz` & `tmp/sqlx-exec-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.3.6.tar", last modified: Sun Jul 30 03:11:08 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.3.8.tar", last modified: Sun Jul 30 08:34:42 2023, max compression
```

## Comparing `sqlx-exec-1.3.6.tar` & `sqlx-exec-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.6/LICENSE
--rw-rw-rw-   0        0        0     3667 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     3116 2023-07-30 02:15:16.000000 sqlx-exec-1.3.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-30 03:10:58.000000 sqlx-exec-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/sqlexec/
--rw-rw-rw-   0        0        0      774 2023-07-29 16:19:11.000000 sqlx-exec-1.3.6/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.6/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11642 2023-07-29 16:19:11.000000 sqlx-exec-1.3.6/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.6/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.6/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.6/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.6/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.6/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.6/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.6/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3667 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 03:11:08.000000 sqlx-exec-1.3.6/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0     3779 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.3.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1283 2023-07-30 08:33:52.000000 sqlx-exec-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlexec/
+-rw-rw-rw-   0        0        0      898 2023-07-30 03:48:03.000000 sqlx-exec-1.3.8/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.8/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11676 2023-07-30 08:23:35.000000 sqlx-exec-1.3.8/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.8/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.8/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.8/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.8/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.8/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.8/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3779 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 08:34:42.000000 sqlx-exec-1.3.8/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.3.6/LICENSE` & `sqlx-exec-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/PKG-INFO` & `sqlx-exec-1.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.6
-Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
+Version: 1.3.8
+Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
@@ -20,15 +20,15 @@
    import sqlexec
 
    if __name__ == '__main__':
        # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
        # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
        sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
-       rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
+       effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
 
@@ -61,19 +61,19 @@
        # result:
        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
        persons = sqlexec.query('select id, name, age from person where name = :name', name='zhangsan')
        # result:
        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       rowcount = sqlexec.execute('delete from person where id = ?', 5)
+       effected_rowcount = sqlexec.execute('delete from person where id = ?', 5)
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
-       rowcount = sqlexec.execute('delete from person where id = :id', 4)
+       effected_rowcount = sqlexec.execute('delete from person where id = :id', 4)
        count = sqlexec.get('select count(1) from person')
        # result: 2
 
 Transaction
 '''''''''''
 
 .. code:: python
```

### Comparing `sqlx-exec-1.3.6/README.rst` & `sqlx-exec-1.3.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    import sqlexec
 
    if __name__ == '__main__':
        # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
        # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
        sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
-       rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
+       effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
 
@@ -47,19 +47,19 @@
        # result:
        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
        persons = sqlexec.query('select id, name, age from person where name = :name', name='zhangsan')
        # result:
        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       rowcount = sqlexec.execute('delete from person where id = ?', 5)
+       effected_rowcount = sqlexec.execute('delete from person where id = ?', 5)
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
-       rowcount = sqlexec.execute('delete from person where id = :id', 4)
+       effected_rowcount = sqlexec.execute('delete from person where id = :id', 4)
        count = sqlexec.get('select count(1) from person')
        # result: 2
 
 Transaction
 '''''''''''
 
 .. code:: python
```

### Comparing `sqlx-exec-1.3.6/setup.py` & `sqlx-exec-1.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
-    description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
+    description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.6',
+    version='1.3.8',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
-    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Python'],
+    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
     python_requires='>=3.5',
     zip_safe=False
```

### Comparing `sqlx-exec-1.3.6/sqlexec/engine.py` & `sqlx-exec-1.3.8/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/sqlexec/exec.py` & `sqlx-exec-1.3.8/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 from . import sql_support
 from .engine import Engine
 from .init_import import import_driver
 from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
-from .constant import MYSQL_CONNECTOR, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
+from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
 
 _DB_CTX = None
 
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
@@ -28,19 +28,19 @@
     :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
     global _DB_CTX
     pool_size = 0
-    driver = kwargs.pop(PARAM_DRIVER) if 'PARAM_DRIVER' in kwargs else None
+    driver = kwargs.pop(PARAM_DRIVER) if PARAM_DRIVER in kwargs else None
     show_sql = kwargs.pop(PARAM_SHOW_SQL) if PARAM_SHOW_SQL in kwargs else False
     trans_placeholder = kwargs.pop(PARAM_TRANS_PLACEHOLDER) if PARAM_TRANS_PLACEHOLDER in kwargs else True
     engine, driver, creator = import_driver(driver)
-    prepared = MYSQL_CONNECTOR == driver
+    prepared = MYSQL_CONNECTOR_DRIVER == driver
     if PARAM_DEBUG in kwargs and kwargs.pop(PARAM_DEBUG):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     if PARAM_POOL_SIZE in kwargs:
         if prepared:
             # mysql.connector 用自带连接池
@@ -303,16 +303,16 @@
     cursor = None
     sql = Engine.before_execute_intf('query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
-            names = [x[0] for x in cursor.description]
-            return [Dict(names, x) for x in results]
+            names = list(map(lambda x: x[0], cursor.description))
+            return list(map(lambda x: Dict(names, x), results))
         else:
             return results
     finally:
         if cursor:
             cursor.close()
```

### Comparing `sqlx-exec-1.3.6/sqlexec/init_import.py` & `sqlx-exec-1.3.8/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/sqlexec/log_support.py` & `sqlx-exec-1.3.8/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/sqlexec/pooling.py` & `sqlx-exec-1.3.8/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/sqlexec/sql_support.py` & `sqlx-exec-1.3.8/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/sqlexec/support.py` & `sqlx-exec-1.3.8/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.6/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.3.8/sqlx_exec.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.6
-Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
+Version: 1.3.8
+Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
@@ -20,15 +20,15 @@
    import sqlexec
 
    if __name__ == '__main__':
        # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
        # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
        sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
-       rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
+       effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
 
@@ -61,19 +61,19 @@
        # result:
        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
        persons = sqlexec.query('select id, name, age from person where name = :name', name='zhangsan')
        # result:
        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       rowcount = sqlexec.execute('delete from person where id = ?', 5)
+       effected_rowcount = sqlexec.execute('delete from person where id = ?', 5)
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
-       rowcount = sqlexec.execute('delete from person where id = :id', 4)
+       effected_rowcount = sqlexec.execute('delete from person where id = :id', 4)
        count = sqlexec.get('select count(1) from person')
        # result: 2
 
 Transaction
 '''''''''''
 
 .. code:: python
```

