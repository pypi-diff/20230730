# Comparing `tmp/sqlx-exec-1.3.0.tar.gz` & `tmp/sqlx-exec-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.3.0.tar", last modified: Sat Jul 29 08:44:50 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.3.1.tar", last modified: Sun Jul 30 01:50:29 2023, max compression
```

## Comparing `sqlx-exec-1.3.0.tar` & `sqlx-exec-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     2759 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2226 2023-07-29 03:34:20.000000 sqlx-exec-1.3.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-29 08:44:45.000000 sqlx-exec-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlexec/
--rw-rw-rw-   0        0        0      489 2023-07-29 03:31:34.000000 sqlx-exec-1.3.0/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2551 2023-07-29 07:25:18.000000 sqlx-exec-1.3.0/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11488 2023-07-29 07:44:50.000000 sqlx-exec-1.3.0/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.0/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.0/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.0/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.0/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.0/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.0/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2759 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2976 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2441 2023-07-30 01:47:55.000000 sqlx-exec-1.3.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-30 01:47:56.000000 sqlx-exec-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/sqlexec/
+-rw-rw-rw-   0        0        0      774 2023-07-29 16:19:11.000000 sqlx-exec-1.3.1/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.1/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11642 2023-07-29 16:19:11.000000 sqlx-exec-1.3.1/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.1/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.1/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.1/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.1/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.1/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.1/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.1/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2976 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 01:50:29.000000 sqlx-exec-1.3.1/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.3.0/LICENSE` & `sqlx-exec-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.0/PKG-INFO` & `sqlx-exec-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.0
+Version: 1.3.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
@@ -16,14 +16,16 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
+       # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
        sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.3.0/README.rst` & `sqlx-exec-1.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
+       # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
        sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.3.0/setup.py` & `sqlx-exec-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.0',
+    version='1.3.1',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.3.0/sqlexec/exec.py` & `sqlx-exec-1.3.1/sqlexec/exec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 from . import sql_support
 from .engine import Engine
 from .init_import import import_driver
-from .constant import MYSQL_CONNECTOR, SQLITE
 from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
+from .constant import MYSQL_CONNECTOR, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
 
 _DB_CTX = None
 
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
@@ -21,52 +21,52 @@
     sqlexec.init_db(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql', pool_size=5, show_sql=True, debug=True)
 
     Addition parameters:
     :param driver=None: str, import driver, 'import pymysql'
     :param pool_size=0: int, default 0, size of connection pool
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
-    :param transform_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
+    :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
     global _DB_CTX
-    driver = kwargs.pop('driver') if 'driver' in kwargs else None
-    pool_size = kwargs.pop('pool_size') if 'pool_size' in kwargs else 0
-    show_sql = kwargs.pop('show_sql') if 'show_sql' in kwargs else False
-    transform_placeholder = kwargs.pop('transform_placeholder') if 'transform_placeholder' in kwargs else True
-
-    if 'debug' in kwargs and kwargs.pop('debug'):
+    pool_size = 0
+    driver = kwargs.pop(PARAM_DRIVER) if 'PARAM_DRIVER' in kwargs else None
+    show_sql = kwargs.pop(PARAM_SHOW_SQL) if PARAM_SHOW_SQL in kwargs else False
+    trans_placeholder = kwargs.pop(PARAM_TRANS_PLACEHOLDER) if PARAM_TRANS_PLACEHOLDER in kwargs else True
+    engine, driver, creator = import_driver(driver)
+    prepared = MYSQL_CONNECTOR == driver
+    if PARAM_DEBUG in kwargs and kwargs.pop(PARAM_DEBUG):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
-    engine, driver, creator = import_driver(driver)
-    prepared = MYSQL_CONNECTOR == driver
+    if PARAM_POOL_SIZE in kwargs:
+        if prepared:
+            # mysql.connector 用自带连接池
+            pool_size = kwargs[PARAM_POOL_SIZE]
+        else:
+            pool_size = kwargs.pop(PARAM_POOL_SIZE)
 
     pool_args = ['mincached', 'maxcached', 'maxshared', 'maxconnections', 'blocking', 'maxusage', 'setsession', 'reset', 'failures', 'ping']
     pool_kwargs = {key: kwargs.pop(key) for key in pool_args if key in kwargs}
-
-    if prepared:
-        # mysql.connector 用自带连接池
-        kwargs['pool_size'] = pool_size
     connect = lambda: creator.connect(*args, **kwargs)
-
     if pool_size >= 1 and not prepared:
         from .pooling import pooled_connect
         connect = pooled_connect(connect, pool_size, **pool_kwargs)
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
     if SQLITE == engine:
-        transform_placeholder = False
-    Engine.init0(engine, transform_placeholder, show_sql)
+        trans_placeholder = False
+    Engine.init0(engine, trans_placeholder, show_sql)
     if pool_size > 0:
         logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine, driver, pool_size))
     else:
         logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine, driver))
 
 
 def connection():
```

### Comparing `sqlx-exec-1.3.0/sqlexec/init_import.py` & `sqlx-exec-1.3.1/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.0/sqlexec/log_support.py` & `sqlx-exec-1.3.1/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.0/sqlexec/pooling.py` & `sqlx-exec-1.3.1/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.0/sqlexec/sql_support.py` & `sqlx-exec-1.3.1/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.0/sqlexec/support.py` & `sqlx-exec-1.3.1/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.0/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.3.1/sqlx_exec.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.0
+Version: 1.3.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
@@ -16,14 +16,16 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
+       # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
        sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

