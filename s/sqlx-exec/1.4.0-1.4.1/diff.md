# Comparing `tmp/sqlx-exec-1.4.0.tar.gz` & `tmp/sqlx-exec-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.4.0.tar", last modified: Sun Jul 30 15:51:27 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.4.1.tar", last modified: Sun Jul 30 16:52:12 2023, max compression
```

## Comparing `sqlx-exec-1.4.0.tar` & `sqlx-exec-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     3728 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.4.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-07-30 15:51:19.000000 sqlx-exec-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlexec/
--rw-rw-rw-   0        0        0      898 2023-07-30 03:48:03.000000 sqlx-exec-1.4.0/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.0/sqlexec/engine.py
--rw-rw-rw-   0        0        0    14143 2023-07-30 15:17:37.000000 sqlx-exec-1.4.0/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.4.0/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.0/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.0/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.0/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.0/sqlexec/support.py
--rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.0/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3728 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3728 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.4.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-07-30 16:51:57.000000 sqlx-exec-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlexec/
+-rw-rw-rw-   0        0        0      962 2023-07-30 16:50:50.000000 sqlx-exec-1.4.1/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.1/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    14554 2023-07-30 16:50:50.000000 sqlx-exec-1.4.1/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1250 2023-07-30 16:40:52.000000 sqlx-exec-1.4.1/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.1/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.1/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.1/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.1/sqlexec/support.py
+-rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.1/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3728 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.4.0/LICENSE` & `sqlx-exec-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/PKG-INFO` & `sqlx-exec-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.0
+Version: 1.4.1
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.4.0/README.rst` & `sqlx-exec-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/setup.py` & `sqlx-exec-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.4.0',
+    version='1.4.1',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.4.0/sqlexec/constant.py` & `sqlx-exec-1.4.1/sqlexec/constant.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 CACHE_SIZE = 256
 
 NAMED_REGEX = r':[\w|\d]*'
 
+MYSQL_PORT, POSTGRESQL_PORT = 3306, 5432
+
 MYSQL, POSTGRESQL, ORACLE, SQL_SERVER, SQLITE, UNKNOW = 'MySQL', 'PostgreSQL', 'Oracle', 'SQL Server', 'SQLite', 'Unknow'
 
 MYSQLCLIENT_DRIVER, PYMYSQL_DRIVER, MYSQL_CONNECTOR_DRIVER, PSYCOPG2_DRIVER, PG8000_DRIVER, PY_POSTGRESQL_DRIVER, PYGRESQL_DRIVER, ORACLEDB_DRIVER,\
     SQLITE3_DRIVER = 'MySQLdb', 'pymysql', 'mysql.connector', 'psycopg2', 'pg8000', 'postgresql.driver.dbapi20', 'pgdb', 'oracledb', 'sqlite3'
 
 DRIVERS = {MYSQLCLIENT_DRIVER: MYSQL, PYMYSQL_DRIVER: MYSQL, MYSQL_CONNECTOR_DRIVER: MYSQL, PSYCOPG2_DRIVER: POSTGRESQL, PG8000_DRIVER: POSTGRESQL,\
            PY_POSTGRESQL_DRIVER: POSTGRESQL, PYGRESQL_DRIVER: POSTGRESQL, ORACLEDB_DRIVER: ORACLE, SQLITE3_DRIVER: SQLITE}
 
-PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE = 'driver', 'show_sql', 'trans_placeholder', 'debug', 'pool_size'
+PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE, PARAM_PORT = 'driver', 'show_sql', 'trans_placeholder', 'debug', 'pool_size', 'port'
```

### Comparing `sqlx-exec-1.4.0/sqlexec/engine.py` & `sqlx-exec-1.4.1/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/sqlexec/exec.py` & `sqlx-exec-1.4.1/sqlexec/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 from . import sql_support
 from .engine import Engine
 from .init_import import import_driver
 from .log_support import logger, insert_log, save_log, get_log, sql_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
-from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
+from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE, PARAM_PORT,\
+    MYSQL, POSTGRESQL, UNKNOW, MYSQL_PORT, POSTGRESQL_PORT
 
 _DB_CTX = None
 
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
@@ -31,15 +32,24 @@
     """
 
     global _DB_CTX
     pool_size = 0
     driver = kwargs.pop(PARAM_DRIVER) if PARAM_DRIVER in kwargs else None
     show_sql = kwargs.pop(PARAM_SHOW_SQL) if PARAM_SHOW_SQL in kwargs else False
     trans_placeholder = kwargs.pop(PARAM_TRANS_PLACEHOLDER) if PARAM_TRANS_PLACEHOLDER in kwargs else True
-    engine, driver, creator = import_driver(driver)
+
+    curr_engine = Engine.current_engine()
+    if driver is None and (curr_engine is None or curr_engine == UNKNOW) and PARAM_PORT in kwargs:
+        port = kwargs[PARAM_PORT]
+        if port == MYSQL_PORT:
+            curr_engine = MYSQL
+        elif port == POSTGRESQL_PORT:
+            curr_engine = POSTGRESQL
+
+    engine, driver, creator = import_driver(driver, curr_engine)
     prepared = MYSQL_CONNECTOR_DRIVER == driver
     if PARAM_DEBUG in kwargs and kwargs.pop(PARAM_DEBUG):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     if PARAM_POOL_SIZE in kwargs:
         if prepared:
```

### Comparing `sqlx-exec-1.4.0/sqlexec/init_import.py` & `sqlx-exec-1.4.1/sqlexec/init_import.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import importlib
-from .engine import Engine
 from .support import DBError
 from .log_support import logger
 from .constant import DRIVERS, UNKNOW
 
 
-def import_driver(driver):
+def import_driver(driver, curr_engine):
     creator = None
-    curr_engine = Engine.current_engine()
     if driver:
         if driver not in DRIVERS:
             logger.warning(f"Driver '{driver}' not support now, may be you should adapte it youself.")
         engine = DRIVERS.get(driver)
         creator = do_import(driver, engine)
         engine = engine if engine else curr_engine
     else:
```

### Comparing `sqlx-exec-1.4.0/sqlexec/log_support.py` & `sqlx-exec-1.4.1/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/sqlexec/pooling.py` & `sqlx-exec-1.4.1/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/sqlexec/sql_support.py` & `sqlx-exec-1.4.1/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/sqlexec/support.py` & `sqlx-exec-1.4.1/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.0/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.4.1/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.0
+Version: 1.4.1
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

