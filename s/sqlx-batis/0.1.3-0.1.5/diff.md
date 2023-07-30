# Comparing `tmp/sqlx-batis-0.1.3.tar.gz` & `tmp/sqlx-batis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.3.tar", last modified: Sat Jul 29 08:45:27 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.5.tar", last modified: Sun Jul 30 01:51:05 2023, max compression
```

## Comparing `sqlx-batis-0.1.3.tar` & `sqlx-batis-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/
--rw-rw-rw-   0        0        0     3373 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-29 08:45:23.000000 sqlx-batis-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlbatis/
--rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.3/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.3/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.3/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     5051 2023-07-29 07:30:33.000000 sqlx-batis-0.1.3/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.3/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.3/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.3/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.3/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.3/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.3/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.3/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1631 2023-07-29 06:24:56.000000 sqlx-batis-0.1.3/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3373 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/
+-rw-rw-rw-   0        0        0     3595 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3112 2023-07-30 01:49:27.000000 sqlx-batis-0.1.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-30 01:50:59.000000 sqlx-batis-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlbatis/
+-rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.5/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.5/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.5/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.5/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.5/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.5/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.5/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.5/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.5/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.5/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.5/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.5/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3595 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.3/PKG-INFO` & `sqlx-batis-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.3
+Version: 0.1.5
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -56,14 +56,16 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
+       # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
+       # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
        init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `sqlx-batis-0.1.3/README.rst` & `sqlx-batis-0.1.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
+       # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
+       # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
        init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `sqlx-batis-0.1.3/setup.py` & `sqlx-batis-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.3.0',
+        'sqlx-exec>=1.3.1',
     ],
-    version='0.1.3',
+    version='0.1.5',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.3/sqlbatis/constant.py` & `sqlx-batis-0.1.5/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/db.py` & `sqlx-batis-0.1.5/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/dbx.py` & `sqlx-batis-0.1.5/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/engine.py` & `sqlx-batis-0.1.5/sqlbatis/engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import re
 from typing import Sequence
 from .support import DBError
-from sqlexec import get, query
 from functools import lru_cache
 from .log_support import logger
-from sqlexec.engine import Engine as BaseEngine
+from sqlexec import get, query, select
+from sqlexec.engine import Engine as SupperEngine
 from .sql_support import require_limit, get_page_start
 from .constant import MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL, MYSQL_SELECT_KEY, LIMIT_1, MYSQL, POSTGRESQL, DEFAULT_KEY_FIELD, CACHE_SIZE, SQLITE, \
     SQLITE_SELECT_KEY
 
 
 # Engin = Enum('Engin', ['MYSQL', 'POSTGRESQL', 'OTHER'])
 # class Engin(Enum):
 #     MYSQL = 'MySQL'
 #     POSTGRESQL = 'PostgreSQL'
 #     OTHER = 'Other'
 
 
-class Engine(BaseEngine):
+class Engine(SupperEngine):
 
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
         if Engine.current_engine() == MYSQL:
             return MySqlEngine.get_page_sql_args(sql, page_num, page_size, *args)
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_page_sql_args(sql, page_num, page_size, *args)
@@ -33,28 +33,45 @@
     def get_select_key(*args, **kwargs):
         if Engine.current_engine() == MYSQL:
             return MySqlEngine.get_select_key()
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_select_key(*args, **kwargs)
         elif Engine.current_engine() == SQLITE:
             return SQLiteEngine.get_select_key()
-        raise NotImplementedError(f"Not implement method 'get_select_key' for {Engine.current_engine()}.")
+        raise NotImplementedError(f"Not implement method 'get_select_key' for {Engine.current_engine()}, you can use orm snowflake for primary key.")
 
     @staticmethod
     def get_table_columns(table: str):
         if Engine.current_engine() == MYSQL:
             return MySqlEngine.get_table_columns(table)
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_table_columns(table)
         elif Engine.current_engine() == SQLITE:
             return SQLiteEngine.get_table_columns(table)
         raise "*"
 
 
-class MySqlEngine(Engine):
+class BaseEngine(Engine):
+    @staticmethod
+    def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
+        start = get_page_start(page_num, page_size)
+        if require_limit(sql):
+            sql = '{} LIMIT ? OFFSET ?'.format(sql)
+        args = [*args, page_size, start]
+        return sql, args
+
+    def before_execute(self, function: str, sql: str, *args):
+        if self.show_sql:
+            logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+        if '%' in sql and 'like' in sql.lower():
+            sql = sql.replace('%', '%%').replace('%%%%', '%%')
+        return sql.replace('?', '%s')
+
+
+class MySqlEngine(BaseEngine):
     @staticmethod
     def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
         return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
 
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
@@ -68,23 +85,16 @@
     def get_table_columns(table: str):
         return get(MYSQL_COLUMN_SQL, table, LIMIT_1)
 
     @staticmethod
     def get_select_key():
         return MYSQL_SELECT_KEY
 
-class PostgresEngine(Engine):
-    @staticmethod
-    def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
-        start = get_page_start(page_num, page_size)
-        if require_limit(sql):
-            sql = '{} LIMIT ? OFFSET ?'.format(sql)
-        args = [*args, page_size, start]
-        return sql, args
 
+class PostgresEngine(BaseEngine):
     @staticmethod
     def get_table_columns(table: str):
         return get(POSTGRES_COLUMN_SQL, table, LIMIT_1)
 
     @staticmethod
     def get_select_key(key_seq: str = None, table: str = None, key: str =None, sql: str = None):
         if not key_seq:
@@ -108,15 +118,35 @@
     def _get_key_seq_from_sql(sql: str):
         table = re.search('(?<=into )\w+', sql, re.I)
         key_seq = PostgresEngine.build_key_seq(table.group())
         logger.warning("'key_seq' is None, will use default '{}' from sql.".format(key_seq))
         return key_seq
 
 
-class SQLiteEngine(PostgresEngine):
+class OracleEngine(BaseEngine):
+    @staticmethod
+    def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
+        start = get_page_start(page_num, page_size)
+        end = start + page_size
+        sql = 'SELECT * FROM (SELECT tmp.*, rownum row_num FROM ({}) tmp WHERE rownum <= >) WHERE row_num > :startRow '.format(sql)
+        args = [*args, end, start]
+        return sql, args
+
+    @staticmethod
+    def get_table_columns(table: str):
+        results = select('SELECT column_name FROM user_tab_columns WHERE table_name = ?')
+        return ','.join([result[0] for result in results])
+
+    @staticmethod
+    def get_select_key(key_seq: str):
+        # return get(f"SELECT {key_seq}.nextval FROM dual")
+        raise NotImplementedError(f"Not implement method 'get_select_key' for {Engine.current_engine()}, you can use orm snowflake for primary key.")
+
+
+class SQLiteEngine(BaseEngine):
     @staticmethod
     def get_table_columns(table: str):
         results = query(f'PRAGMA table_info({table})')
         return ','.join([result['name'] for result in results])
 
     @staticmethod
     def get_select_key():
```

### Comparing `sqlx-batis-0.1.3/sqlbatis/log_support.py` & `sqlx-batis-0.1.5/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/orm.py` & `sqlx-batis-0.1.5/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/snowflake.py` & `sqlx-batis-0.1.5/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.5/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.5/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/sql_support.py` & `sqlx-batis-0.1.5/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.3/sqlbatis/__init__.py` & `sqlx-batis-0.1.5/sqlbatis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     Addition parameters:
     :param mapper_path: str, path of mapper files
     :param driver=None: str, import driver, 'import pymysql'
     :param pool_size=0: int, default 0, size of connection pool
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
-    :param transform_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
+    :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
     from .sql_holder import load_mapper
     from sqlexec import init_db as supper_init_db
```

### Comparing `sqlx-batis-0.1.3/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.5/sqlx_batis.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.3
+Version: 0.1.5
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -56,14 +56,16 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
+       # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
+       # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
        init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

