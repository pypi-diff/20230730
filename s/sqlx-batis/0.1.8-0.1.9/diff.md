# Comparing `tmp/sqlx-batis-0.1.8.tar.gz` & `tmp/sqlx-batis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.8.tar", last modified: Sun Jul 30 08:46:15 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.9.tar", last modified: Sun Jul 30 15:52:06 2023, max compression
```

## Comparing `sqlx-batis-0.1.8.tar` & `sqlx-batis-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/
--rw-rw-rw-   0        0        0     5701 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.1.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-07-30 08:39:58.000000 sqlx-batis-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlbatis/
--rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.8/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.8/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.8/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.8/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.8/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.8/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.8/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.8/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.8/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.8/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.8/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.8/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5701 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/
+-rw-rw-rw-   0        0        0     5701 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.1.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-07-30 15:51:52.000000 sqlx-batis-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlbatis/
+-rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.9/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8739 2023-07-30 15:39:23.000000 sqlx-batis-0.1.9/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-0.1.9/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.9/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     3892 2023-07-30 15:46:56.000000 sqlx-batis-0.1.9/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.9/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.9/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.9/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-0.1.9/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1757 2023-07-30 15:25:21.000000 sqlx-batis-0.1.9/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.9/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.9/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.8/PKG-INFO` & `sqlx-batis-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.8
+Version: 0.1.9
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.1.8/README.rst` & `sqlx-batis-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/setup.py` & `sqlx-batis-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.3.9',
+        'sqlx-exec>=1.4.0',
     ],
-    version='0.1.8',
+    version='0.1.9',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.8/sqlbatis/constant.py` & `sqlx-batis-0.1.9/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/sqlbatis/db.py` & `sqlx-batis-0.1.9/sqlbatis/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import sql_support, Engine, DBError
 from .log_support import sql_log, do_sql_log, save_log, do_page_log, page_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import insert, save as save_select_key, save_sql, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one,\
-    query as supper_query, select as supper_select, select_one as supper_select_one
+from sqlexec import insert, save as save_select_key, save_sql, do_save_sql, batch_insert, batch_execute, do_execute as sqlexec_execute, \
+    do_get as sqlexec_get, do_query_one as sqlexec_query_one,do_query as sqlexec_query, do_select as sqlexec_select, do_select_one as sqlexec_select_one
 
 
 def save(table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
@@ -23,135 +23,125 @@
 
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    sql_log('execute', sql, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql_args('sqlbatis.db.execute', sql, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_log('get', sql, *args, **kwargs)
-    global _DB_CTX
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql_args('sqlbatis.db.get', sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_log('query', sql, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql_args('sqlbatis.db.query', sql, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_log('query_one', sql, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql_args('sqlbatis.db.query_one', sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_log('select', sql, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql_args('sqlbatis.db.select', sql, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_log('select_one', sql, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql_args('sqlbatis.db.select_one', sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 # ----------------------------------------------------------Do function------------------------------------------------------------------
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into user(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
-    return supper_execute(sql, *args)
+    return sqlexec_execute(sql, *args)
 
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    do_sql_log('do_get', sql, *args)
-    sql, args = sql_support.limit_one_sql_args(sql, *args)
-    return supper_get(sql, *args)
+    sql, args = _do_limit_sql_args('do_get', sql, *args)
+    return sqlexec_get(sql, *args)
 
 
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return supper_query(sql, *args)
+    return sqlexec_query(sql, *args)
 
 
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return supper_select(sql, *args)
+    return sqlexec_select(sql, *args)
 
 
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    do_sql_log('do_query_one', sql, *args)
-    sql, args = sql_support.limit_one_sql_args(sql, *args)
-    return supper_query_one(sql, *args)
+    sql, args = _do_limit_sql_args('do_query_one', sql, *args)
+    return sqlexec_query_one(sql, *args)
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    do_sql_log('do_select_one', sql, *args)
-    sql, args = sql_support.limit_one_sql_args(sql, *args)
-    return supper_select_one(sql, *args)
+    sql, args = _do_limit_sql_args('do_select_one', sql, *args)
+    return sqlexec_select_one(sql, *args)
 
 
 # ----------------------------------------------------------Page function------------------------------------------------------------------
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
@@ -176,18 +166,28 @@
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('select_page', sql.strip(), page_num, page_size, args)
     sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
-    return supper_query(sql, *args)
+    return sqlexec_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
     sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
-    return supper_select(sql, *args)
+    return sqlexec_select(sql, *args)
+
+
+def _try_dynamic_sql_args(function, sql, *args, **kwargs):
+    sql_log(function, sql, *args, **kwargs)
+    return sql_support.dynamic_sql(sql, *args, **kwargs)
+
+
+def _do_limit_sql_args(function, sql, *args):
+    do_sql_log(function, sql, *args)
+    return sql_support.limit_one_sql_args(sql, *args)
```

### Comparing `sqlx-batis-0.1.8/sqlbatis/dbx.py` & `sqlx-batis-0.1.9/sqlbatis/dbx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .sql_support import get_batch_args
 from . import Engine, DBError, sql_holder as holder
 from .log_support import logger, sql_id_log, page_sql_id_log, sql_id_select_key_log
 
 # Don't remove. Import for not repetitive implementation
-from .db import(do_execute, insert, save_sql, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_select, \
+from .db import(do_execute, insert, do_save_sql, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_select, \
                 do_select_one, do_select_page, do_query_page)
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
@@ -17,110 +17,104 @@
     select_key = sql_model.select_key
     sql, args = holder.do_get_sql(sql_model, False, None, *args, **kwargs)
     if not select_key:
         try:
             select_key = Engine.get_select_key_intf(sql=sql)
         except NotImplementedError:
             raise DBError(f"Expect 'select_key' but not. you can set it in mapper file with 'selectKey'.")
-    return save_sql(select_key, sql, *args)
+    return do_save_sql(select_key, sql, *args)
 
 
 def save_select_key(select_key, sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
     sql_id_select_key_log('save_select_key', select_key, sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return save_sql(select_key, sql, *args)
+    return do_save_sql(select_key, sql, *args)
 
 
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    sql_id_log('dbx.execute', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    sql, args = _get_sql_args_from_id('sqlbatis.dbx.execute', sql_id, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 def batch_execute(sql_id: str, *args):
     """
     Batch execute
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    logger.debug("Exec func 'mysqlx.dbx.%s' \n\t sql_id: '%s' \n\t args: %s" % ('batch_execute', sql_id, args))
+    logger.debug("Exec func 'sqlbatis.dbx.%s' \n\t sql_id: '%s' \n\t args: %s" % ('batch_execute', sql_id, args))
     assert len(args) > 0, 'args must not be empty.'
     args = get_batch_args(*args)
     sql, _ = holder.do_get_sql(holder.get_sql_model(sql_id), True, None, *args)
     return db_batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_id_log('get', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    sql, args = _get_sql_args_from_id('sqlbatis.dbx.get', sql_id, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_id_log('query', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    sql, args = _get_sql_args_from_id('sqlbatis.dbx.query', sql_id, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_id_log('query_one', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    sql, args = _get_sql_args_from_id('sqlbatis.dbx.query_one', sql_id, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_id_log('select', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    sql, args = _get_sql_args_from_id('sqlbatis.dbx.select', sql_id, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql_id_log('select_one', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    sql, args = _get_sql_args_from_id('sqlbatis.dbx.select_one', sql_id, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
@@ -137,7 +131,11 @@
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
+
+def _get_sql_args_from_id(function, sql_id: str, *args, **kwargs):
+    sql_id_log(function, sql_id, *args, **kwargs)
+    return holder.get_sql(sql_id, *args, **kwargs)
```

### Comparing `sqlx-batis-0.1.8/sqlbatis/engine.py` & `sqlx-batis-0.1.9/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/sqlbatis/log_support.py` & `sqlx-batis-0.1.9/sqlbatis/log_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from sqlexec.log_support import logger
+from sqlexec.log_support import logger, sql_log
 
 
 def save_log(table, **kwargs):
     logger.debug("Exec func 'pgsqlx.db.save' \n\t Table: '%s', kwargs: %s" % (table, kwargs))
 
 
-def sql_log(function: str, sql: str, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.db.%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
-
-
 def do_sql_log(function: str, sql: str, *args):
     logger.debug("Exec func 'sqlbatis.db.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
 def do_page_log(function: str, sql: str, page_num, page_size, *args):
     logger.debug(
         "Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql.strip(), args))
@@ -24,15 +20,15 @@
 
 
 def page_sql_id_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
     logger.debug("Exec func 'sqlbatis.dbx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (function, page_num, page_size, sql_id, args, kwargs))
 
 
 def sql_id_log(function: str, sql_id: str, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.dbx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
+    logger.debug("Exec func '%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
 
 
 def sql_id_select_key_log(function: str, select_key: str, sql_id: str, *args, **kwargs):
     logger.debug("Exec func 'sqlbatis.dbx.%s', select_key: %s, sql_id: %s, args: %s, kwargs: %s" % (function, select_key, sql_id.strip(), args, kwargs))
 
 
 def orm_insert_log(function, class_name, **kwargs):
```

### Comparing `sqlx-batis-0.1.8/sqlbatis/orm.py` & `sqlx-batis-0.1.9/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/sqlbatis/snowflake.py` & `sqlx-batis-0.1.9/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.9/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.9/sqlbatis/sql_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                     use_select_key = sql_model.select_key
                     if use_select_key is None:
                         try:
                             use_select_key = Engine.get_select_key_intf(sql=use_sql)
                         except NotImplementedError:
                             return DBError(
                                 f"Expect 'select_key' but not. you can set it in mapper file with 'selectKey', or @mapper with 'select_key'")
-                return sqlexec.save_sql(use_select_key, use_sql, *args)
+                return sqlexec.do_save_sql(use_select_key, use_sql, *args)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             else:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
@@ -61,19 +61,19 @@
                         try:
                             use_select_key = Engine.get_select_key_intf(sql=use_sql)
                         except NotImplementedError:
                             return DBError(f"Expect 'select_key' but not in func '{func.__name__}' at file: '{func.__code__.co_filename}', line {func.__code__.co_firstlineno}. you can set it @sql with 'select_key'")
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                    return sqlexec.save_sql(use_select_key, use_sql, *args)
+                    return sqlexec.do_save_sql(use_select_key, use_sql, *args)
 
                 if kwargs:
                     use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                return sqlexec.execute(use_sql, *args)
+                return sqlexec.do_execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
                 select_func = get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
                 return select_func(use_sql, *args)
             else:
                 return ValueError("Invalid sql: {}.".format(sql))
 
@@ -84,32 +84,32 @@
 
 def get_exec_func(func, action, batch):
     if action == SqlAction.SELECT.value:
         return get_select_func(func)
     elif batch:
         return sqlexec.batch_execute
     else:
-        return sqlexec.execute
+        return sqlexec.do_execute
 
 
 def get_select_func(func):
     names = func.__code__.co_names
     is_list = 'list' in names or 'List' in names
     if 'Mapping' in names and is_list:
-        return sqlexec.query
+        return sqlexec.do_query
     elif 'Mapping' in names:
-        return sqlexec.query_one
+        return sqlexec.do_query_one
     elif len(names) == 1 and names[0] in ('int', 'float', 'Decimal', 'str', 'AnyStr', 'date', 'time', 'datetime'):
-        return sqlexec.get
+        return sqlexec.do_get
     elif len(names) == 1 and names[0] in ('tuple', 'Tuple'):
-        return sqlexec.select_one
+        return sqlexec.do_select_one
     elif is_list:
-        return sqlexec.select
+        return sqlexec.do_select
     else:
-        return sqlexec.query
+        return sqlexec.do_query
 
 
 def before(func, namespace, _id, *args, **kwargs):
     file_name = os.path.basename(func.__code__.co_filename)[:-3]
     _namespace = namespace if namespace else file_name
     _id = _id if _id else func.__name__
     sql_id = build_sql_id(_namespace, _id)
```

### Comparing `sqlx-batis-0.1.8/sqlbatis/sql_support.py` & `sqlx-batis-0.1.9/sqlbatis/sql_support.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from jinja2 import Template
 from functools import lru_cache
 from .support import MapperError
 from .constant import LIMIT_1, DYNAMIC_REGEX, CACHE_SIZE
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args
+from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args, get_named_sql_args, is_mapping
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
 def dynamic_sql(sql: str, *args, **kwargs):
@@ -34,19 +34,14 @@
     return sql, args
 
 
 def is_dynamic_sql(sql: str):
     return re.search(DYNAMIC_REGEX, sql)
 
 
-def get_named_sql_args(sql: str, **kwargs):
-    args = get_named_args(sql, **kwargs)
-    return get_named_sql(sql), args
-
-
 def require_limit(sql: str):
     lower_sql = sql.lower()
     if 'limit' not in lower_sql:
         return True
     idx = lower_sql.rindex('limit')
     if idx > 0 and ')' in lower_sql[idx:]:
         return True
@@ -56,11 +51,11 @@
 @lru_cache(maxsize=2*CACHE_SIZE)
 def _get_sql_type(sql: str):
     """
     :return: 0: placeholder, 1: dynamic, 2: named mapping
     """
     if is_dynamic_sql(sql):
         return 1
-    if ':' in sql:
+    if is_mapping(sql):
         return 2
     return 0
```

### Comparing `sqlx-batis-0.1.8/sqlbatis/__init__.py` & `sqlx-batis-0.1.9/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.8/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.9/sqlx_batis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.8
+Version: 0.1.9
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

