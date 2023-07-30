# Comparing `tmp/pgsqlx-1.7.1.tar.gz` & `tmp/pgsqlx-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.7.1.tar", last modified: Sun Jul 30 06:50:43 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.7.2.tar", last modified: Sun Jul 30 16:19:16 2023, max compression
```

## Comparing `pgsqlx-1.7.1.tar` & `pgsqlx-1.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/
-drwxrwxrwx   0        0        0        0 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx/
--rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.1/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.1/pgsqlx/db.py
--rw-rw-rw-   0        0        0     1250 2023-07-28 02:45:27.000000 pgsqlx-1.7.1/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.1/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.7.1/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.1/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     1501 2023-07-29 10:35:25.000000 pgsqlx-1.7.1/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5079 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5079 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     4548 2023-07-30 06:50:05.000000 pgsqlx-1.7.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-07-30 06:50:36.000000 pgsqlx-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/
+drwxrwxrwx   0        0        0        0 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx/
+-rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.2/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.2/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1259 2023-07-30 16:17:23.000000 pgsqlx-1.7.2/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.2/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.7.2/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.2/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     1446 2023-07-30 16:16:26.000000 pgsqlx-1.7.2/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5406 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      319 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5406 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2023-07-30 08:43:39.000000 pgsqlx-1.7.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:19:16.000000 pgsqlx-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-07-30 16:18:52.000000 pgsqlx-1.7.2/setup.py
```

### Comparing `pgsqlx-1.7.1/pgsqlx/db.py` & `pgsqlx-1.7.2/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.1/pgsqlx/dbx.py` & `pgsqlx-1.7.2/pgsqlx/dbx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from . import PostgresEngine
 from sqlbatis import sql_holder as holder
 from .log_support import sql_id_log, sql_id_key_seq_log
-from sqlbatis.dbx import insert, save_sql, save_select_key, batch_insert, batch_execute, execute, get, query, query_one, select, select_one, query_page, select_page
+from sqlbatis.dbx import insert, do_save_sql, save_select_key, batch_insert, batch_execute, execute, get, query, query_one, select, select_one, query_page, select_page
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
     sql_id_log('save', sql_id, *args, **kwargs)
     sql_model = holder.get_sql_model(sql_id)
     sql, args = holder.do_get_sql(sql_model, False, None, *args, **kwargs)
     select_key = PostgresEngine.get_select_key(key_seq=sql_model.key_seq, sql=sql)
-    return save_sql(select_key, sql, *args)
+    return do_save_sql(select_key, sql, *args)
 
 
 def save_key_seq(key_seq, sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
     sql_id_key_seq_log('save_key_seq', key_seq, sql_id, *args, **kwargs)
     sql_model = holder.get_sql_model(sql_id)
     sql, args = holder.get_sql(sql_model, False, None, *args, **kwargs)
     key_seq = key_seq if key_seq else sql_model.key_seq
     select_key = PostgresEngine.get_select_key(key_seq=key_seq, sql=sql)
-    return save_sql(select_key, sql, *args)
+    return do_save_sql(select_key, sql, *args)
```

### Comparing `pgsqlx-1.7.1/pgsqlx/log_support.py` & `pgsqlx-1.7.2/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.1/pgsqlx/orm.py` & `pgsqlx-1.7.2/pgsqlx/orm.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.1/pgsqlx/sql_mapper.py` & `pgsqlx-1.7.2/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.1/pgsqlx/__init__.py` & `pgsqlx-1.7.2/pgsqlx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,13 +28,11 @@
     :param pool_size=0: int, default 0, size of connection pool
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
     :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
-    from .constant import POSTGRESQL
     from sqlbatis import init_db as supper_init_db
 
-    PostgresEngine.init(name=POSTGRESQL)
+    PostgresEngine.init()
     supper_init_db(*args, **kwargs)
-
```

### Comparing `pgsqlx-1.7.1/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.7.2/pgsqlx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.7.1
-Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
+Version: 1.7.2
+Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -94,26 +94,28 @@
         # result:
         # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
         persons = query_by_name2(name='zhangsan')
         # result:
         # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        # you can use dbx execute mapper sql with full sql id: namespace join sql id
         persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         persons = dbx.select('person.select_by_name', name='zhangsan')
         # result:
         # (3, 'zhangsan', 15)
 
-        # you can direct execte sql with db
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='person', name='zhaoliu', age=66)
+
         persons = db.select('select id, name, age from person')
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         persons = db.select('select id, name, age from person where name=?', 'zhangsan')
@@ -127,23 +129,26 @@
             __pk_seq__ = 'person_id_seq'
 
             def __init__(self, id: int = None, name: str = None, age: int = None):
                 self.id = id
                 self.name = name
                 self.age = age
 
-        persons = person.query()
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
-        # {'id': 4, 'name': 'lisi', 'age': 26}
-        # {'id': 5, 'name': 'wangwu', 'age': 38}
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
 
-        persons = person.query(name__eq='zhangsan')
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from pgsqlx import with_transaction, transaction
```

### Comparing `pgsqlx-1.7.1/PKG-INFO` & `pgsqlx-1.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.7.1
-Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
+Version: 1.7.2
+Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -94,26 +94,28 @@
         # result:
         # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
         persons = query_by_name2(name='zhangsan')
         # result:
         # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        # you can use dbx execute mapper sql with full sql id: namespace join sql id
         persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         persons = dbx.select('person.select_by_name', name='zhangsan')
         # result:
         # (3, 'zhangsan', 15)
 
-        # you can direct execte sql with db
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='person', name='zhaoliu', age=66)
+
         persons = db.select('select id, name, age from person')
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         persons = db.select('select id, name, age from person where name=?', 'zhangsan')
@@ -127,23 +129,26 @@
             __pk_seq__ = 'person_id_seq'
 
             def __init__(self, id: int = None, name: str = None, age: int = None):
                 self.id = id
                 self.name = name
                 self.age = age
 
-        persons = person.query()
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
-        # {'id': 4, 'name': 'lisi', 'age': 26}
-        # {'id': 5, 'name': 'wangwu', 'age': 38}
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
 
-        persons = person.query(name__eq='zhangsan')
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from pgsqlx import with_transaction, transaction
```

### Comparing `pgsqlx-1.7.1/README.rst` & `pgsqlx-1.7.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -81,26 +81,28 @@
         # result:
         # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
         persons = query_by_name2(name='zhangsan')
         # result:
         # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        # you can use dbx execute mapper sql with full sql id: namespace join sql id
         persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         persons = dbx.select('person.select_by_name', name='zhangsan')
         # result:
         # (3, 'zhangsan', 15)
 
-        # you can direct execte sql with db
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='person', name='zhaoliu', age=66)
+
         persons = db.select('select id, name, age from person')
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         persons = db.select('select id, name, age from person where name=?', 'zhangsan')
@@ -114,23 +116,26 @@
             __pk_seq__ = 'person_id_seq'
 
             def __init__(self, id: int = None, name: str = None, age: int = None):
                 self.id = id
                 self.name = name
                 self.age = age
 
-        persons = person.query()
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
-        # {'id': 4, 'name': 'lisi', 'age': 26}
-        # {'id': 5, 'name': 'wangwu', 'age': 38}
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
 
-        persons = person.query(name__eq='zhangsan')
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from pgsqlx import with_transaction, transaction
```

