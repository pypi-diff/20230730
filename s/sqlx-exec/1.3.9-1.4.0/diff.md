# Comparing `tmp/sqlx-exec-1.3.9.tar.gz` & `tmp/sqlx-exec-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.3.9.tar", last modified: Sun Jul 30 08:37:21 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.4.0.tar", last modified: Sun Jul 30 15:51:27 2023, max compression
```

## Comparing `sqlx-exec-1.3.9.tar` & `sqlx-exec-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.9/LICENSE
--rw-rw-rw-   0        0        0     3728 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.3.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-07-30 08:37:11.000000 sqlx-exec-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlexec/
--rw-rw-rw-   0        0        0      898 2023-07-30 03:48:03.000000 sqlx-exec-1.3.9/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.3.9/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11676 2023-07-30 08:23:35.000000 sqlx-exec-1.3.9/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.9/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.9/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.9/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.9/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.9/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.9/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3728 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 08:37:21.000000 sqlx-exec-1.3.9/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     3728 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.4.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-07-30 15:51:19.000000 sqlx-exec-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlexec/
+-rw-rw-rw-   0        0        0      898 2023-07-30 03:48:03.000000 sqlx-exec-1.4.0/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.0/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    14143 2023-07-30 15:17:37.000000 sqlx-exec-1.4.0/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.4.0/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.0/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.0/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.0/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.0/sqlexec/support.py
+-rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.0/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3728 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 15:51:27.000000 sqlx-exec-1.4.0/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.3.9/LICENSE` & `sqlx-exec-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/PKG-INFO` & `sqlx-exec-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.9
+Version: 1.4.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.3.9/README.rst` & `sqlx-exec-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/setup.py` & `sqlx-exec-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.9',
+    version='1.4.0',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.3.9/sqlexec/constant.py` & `sqlx-exec-1.4.0/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/sqlexec/engine.py` & `sqlx-exec-1.4.0/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/sqlexec/exec.py` & `sqlx-exec-1.4.0/sqlexec/exec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 from . import sql_support
 from .engine import Engine
 from .init_import import import_driver
-from .log_support import logger, insert_log, save_log, get_log
+from .log_support import logger, insert_log, save_log, get_log, sql_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
 
 _DB_CTX = None
 
 
 def init_db(*args, **kwargs):
@@ -167,37 +167,25 @@
     :return: Primary key
     """
     save_log('save', select_key, table, **kwargs)
     sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
     return save_sql(select_key, sql, *args)
 
 
-@with_connection
-def save_sql(select_key: str, sql: str, *args):
+def save_sql(select_key: str, sql: str, *args, **kwargs):
     """
     Insert data into table, return primary key.
     :param select_key: sql for select primary key
     :param sql: table
     :param args:
     :return: Primary key
     """
-    global _DB_CTX
-    cursor = None
-    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s" % ('save_sql', select_key, sql, args))
-    sql = Engine.before_execute_intf('save_sql', sql, *args)
-    try:
-        cursor = _DB_CTX.connection.cursor()
-        cursor.execute(sql, args)
-        cursor.execute(select_key)
-        result = cursor.fetchone()
-        try_commit(_DB_CTX)
-        return result[0]
-    finally:
-        if cursor:
-            cursor.close()
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s \n\t kwargs: %s" % ('save_sql', select_key, sql, args, kwargs))
+    sql, args = sql_support.get_mapping_sql_args(sql, *args, **kwargs)
+    return do_save_sql(select_key, sql, *args)
 
 
 def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
@@ -230,82 +218,167 @@
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
         if cursor:
             cursor.close()
 
 
-def get(sql: str, *args):
+def get(sql: str, *args, **kwargs):
+    """
+    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+    MultiColumnsError: Expect only one column.
+    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    sql, args = _try_mapping('sqlexec.get', sql, *args, **kwargs)
+    return do_get(sql, *args)
+
+
+def select(sql: str, *args, **kwargs):
+    """
+    execute select SQL and return unique result or list results(tuple).
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    sql, args = _try_mapping('sqlexec.select', sql, *args, **kwargs)
+    return do_select(sql, *args)
+
+
+def select_one(sql: str, *args, **kwargs):
+    """
+    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    sql, args = _try_mapping('sqlexec.select_one', sql, *args, **kwargs)
+    return do_select_one(sql, *args)
+
+
+def query(sql: str, *args, **kwargs):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    sql, args = _try_mapping('sqlexec.query', sql, *args, **kwargs)
+    return do_query(sql, *args)
+
+
+def query_one(sql: str, *args, **kwargs):
+    """
+    execute select SQL and return unique result(dict), SQL contain 'limit'.
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    sql, args = _try_mapping('sqlexec.query_one', sql, *args, **kwargs)
+    return do_query_one(sql, *args)
+
+
+@with_connection
+def do_execute(sql: str, *args):
+    """
+    Execute sql return effect rowcount
+    sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
+    """
+    global _DB_CTX
+    cursor = None
+    sql = Engine.before_execute_intf('do_execute', sql.strip(), *args)
+    try:
+        cursor = _DB_CTX.connection.cursor()
+        cursor.execute(sql, args)
+        effect_rowcount = cursor.rowcount
+        try_commit(_DB_CTX)
+        return effect_rowcount
+    finally:
+        if cursor:
+            cursor.close()
+
+
+@with_connection
+def do_save_sql(select_key: str, sql: str, *args):
+    """
+    Insert data into table, return primary key.
+    :param select_key: sql for select primary key
+    :param sql: table
+    :param args:
+    :return: Primary key
+    """
+    global _DB_CTX
+    cursor = None
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s" % ('do_save_sql', select_key))
+    sql = Engine.before_execute_intf('save_sql', sql, *args)
+    try:
+        cursor = _DB_CTX.connection.cursor()
+        cursor.execute(sql, args)
+        cursor.execute(select_key)
+        result = cursor.fetchone()
+        try_commit(_DB_CTX)
+        return result[0]
+    finally:
+        if cursor:
+            cursor.close()
+
+
+def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     get_log('get', sql, *args)
     result = select_one(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
-        msg = "Exec func 'sqlexec.%s' expect only one column but %d." % ('get', len(result))
+        msg = "Exec func 'sqlexec.%s' expect only one column but %d." % ('do_get', len(result))
         logger.error('%s  \n\t sql: %s \n\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
 
 
 @with_connection
-def select(sql: str, *args):
+def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = Engine.before_execute_intf('select', sql.strip(), *args)
+    sql = Engine.before_execute_intf('do_select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def select_one(sql: str, *args):
+def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = Engine.before_execute_intf('select_one', sql.strip(), *args)
+    sql = Engine.before_execute_intf('do_select_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
 
 
-# def select_page(sql: str, page_num, page_size, *args):
-#     page_log('select_page', sql.strip(), page_num, page_size, args)
-#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
-#     return select(sql, *args)
-
-
 @with_connection
-def query(sql: str, *args):
+def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = Engine.before_execute_intf('query', sql.strip(), *args)
+    sql = Engine.before_execute_intf('do_query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
             names = list(map(lambda x: x[0], cursor.description))
             return list(map(lambda x: Dict(names, x), results))
@@ -313,38 +386,37 @@
             return results
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def query_one(sql: str, *args):
+def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = Engine.before_execute_intf('query_one', sql.strip(), *args)
+    sql = Engine.before_execute_intf('do_query_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         result = cursor.fetchone()
         if result and cursor.description:
             names = [x[0] for x in cursor.description]
             return Dict(names, result)
         return result
     finally:
         if cursor:
             cursor.close()
 
 
-# def query_page(sql: str, page_num, page_size, *args):
-#     page_log('query_page', sql.strip(), page_num, page_size, args)
-#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
-#     return query(sql, *args)
-
-
 def get_connection():
     global _DB_CTX
     _DB_CTX.try_init()
     return _DB_CTX.connection
+
+
+def _try_mapping(function, sql, *args, **kwargs):
+    sql_log(function, sql, *args, **kwargs)
+    return sql_support.get_mapping_sql_args(sql, *args, **kwargs)
```

### Comparing `sqlx-exec-1.3.9/sqlexec/init_import.py` & `sqlx-exec-1.4.0/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/sqlexec/log_support.py` & `sqlx-exec-1.4.0/sqlexec/log_support.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', kwargs: %s" % (function, table, kwargs))
 
 
 def save_log(function: str, select_key: str, table: str, **kwargs):
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t Table: '%s', kwargs: %s" % (function, select_key, table, kwargs))
 
 
+def sql_log(function: str, sql: str, *args, **kwargs):
+    logger.debug("Exec func '%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+
+
 def get_log(function: str, sql: str, *args):
     logger.debug("Exec func 'sqlexec.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
 def db_ctx_log(action, connection):
     logger.debug('%s connection <%s>...' % (action, hex(id(connection))))
```

### Comparing `sqlx-exec-1.3.9/sqlexec/pooling.py` & `sqlx-exec-1.4.0/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/sqlexec/sql_support.py` & `sqlx-exec-1.4.0/sqlexec/sql_support.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 from .engine import Engine
 from typing import Sequence
+from .support import DBError
 from functools import lru_cache
 from .constant import CACHE_SIZE, NAMED_REGEX
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
     sql = Engine.create_insert_sql_intf(table, cols)
     return sql, args
 
 
+
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
 def batch_insert_sql_args(table: str, *args):
     args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
@@ -32,7 +34,31 @@
 @lru_cache(maxsize=CACHE_SIZE)
 def get_named_sql(sql: str):
     return re.sub(NAMED_REGEX, '?', sql)
 
 
 def get_named_args(sql: str, **kwargs):
     return [kwargs[r[1:]] for r in re.findall(NAMED_REGEX, sql)]
+
+
+def get_named_sql_args(sql: str, **kwargs):
+    args = get_named_args(sql, **kwargs)
+    return get_named_sql(sql), args
+
+
+def is_mapping(sql: str):
+    return ':' in sql
+
+
+def is_placeholder(sql: str):
+    return '?' in sql
+
+
+def get_mapping_sql_args(sql: str, *args, **kwargs):
+    if is_mapping(sql):
+        assert kwargs, "Named mapping SQL expect '**kwargs' should not be empty."
+        return get_named_sql_args(sql, **kwargs)
+
+    if is_placeholder(sql) and not args:
+        raise DBError("Placeholder sql expect '*args' should not be empty.")
+
+    return sql, args
```

### Comparing `sqlx-exec-1.3.9/sqlexec/support.py` & `sqlx-exec-1.4.0/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.3.9/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.4.0/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.3.9
+Version: 1.4.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

