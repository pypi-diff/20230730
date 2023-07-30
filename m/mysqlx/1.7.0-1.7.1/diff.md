# Comparing `tmp/mysqlx-1.7.0.tar.gz` & `tmp/mysqlx-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.7.0.tar", last modified: Sun Jul 30 06:45:13 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.7.1.tar", last modified: Sun Jul 30 16:19:43 2023, max compression
```

## Comparing `mysqlx-1.7.0.tar` & `mysqlx-1.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 06:45:13.000000 mysqlx-1.7.0/
-drwxrwxrwx   0        0        0        0 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx/
--rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.7.0/mysqlx/db.py
--rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.7.0/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.7.0/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.7.0/mysqlx/orm.py
--rw-rw-rw-   0        0        0     1483 2023-07-29 10:35:00.000000 mysqlx-1.7.0/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4972 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      279 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4972 2023-07-30 06:45:13.000000 mysqlx-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4453 2023-07-30 06:25:59.000000 mysqlx-1.7.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 06:45:13.000000 mysqlx-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-30 06:45:05.000000 mysqlx-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:19:43.000000 mysqlx-1.7.1/
+drwxrwxrwx   0        0        0        0 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx/
+-rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.7.1/mysqlx/db.py
+-rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.7.1/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.7.1/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.7.1/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     1430 2023-07-30 16:14:15.000000 mysqlx-1.7.1/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5290 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      279 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 16:19:43.000000 mysqlx-1.7.1/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5290 2023-07-30 16:19:43.000000 mysqlx-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4633 2023-07-30 08:45:57.000000 mysqlx-1.7.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:19:43.000000 mysqlx-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-07-30 16:19:36.000000 mysqlx-1.7.1/setup.py
```

### Comparing `mysqlx-1.7.0/mysqlx/db.py` & `mysqlx-1.7.1/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.0/mysqlx/dbx.py` & `mysqlx-1.7.1/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.0/mysqlx/log_support.py` & `mysqlx-1.7.1/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.0/mysqlx/orm.py` & `mysqlx-1.7.1/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.0/mysqlx/__init__.py` & `mysqlx-1.7.1/mysqlx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,13 +31,11 @@
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
     :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
-    from sqlbatis.constant import MYSQL
     from sqlbatis import init_db as supper_init_db
 
-    MySqlEngine.init(name=MYSQL)
+    MySqlEngine.init()
     supper_init_db(*args, **kwargs)
-
```

### Comparing `mysqlx-1.7.0/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.7.1/mysqlx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.7.0
-Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
+Version: 1.7.1
+Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -105,15 +105,17 @@
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         users = dbx.select('user.select_by_name', name='zhangsan')
         # result:
         # (3, 'zhangsan', 15)
 
-        # you can direct execte sql with db
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='user', name='zhaoliu', age=66)
+
         users = db.select('select id, name, age from user')
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         users = db.select('select id, name, age from user where name=?', 'zhangsan')
@@ -126,23 +128,26 @@
             __table__ = 'user'
 
             def __init__(self, id: int = None, name: str = None, age: int = None):
                 self.id = id
                 self.name = name
                 self.age = age
 
-        users = User.query()
+
+        effected_rowcount = User.insert(name='tianqi', age=77)
+
+        users = User.query(name='tianqi')
+        # select id, name, age from user where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
-        # {'id': 4, 'name': 'lisi', 'age': 26}
-        # {'id': 5, 'name': 'wangwu', 'age': 38}
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
 
         users = User.query(name__eq='zhangsan')
+        # select id, name, age from user where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from mysqlx import with_transaction, transaction
```

### Comparing `mysqlx-1.7.0/PKG-INFO` & `mysqlx-1.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.7.0
-Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
+Version: 1.7.1
+Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -105,15 +105,17 @@
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         users = dbx.select('user.select_by_name', name='zhangsan')
         # result:
         # (3, 'zhangsan', 15)
 
-        # you can direct execte sql with db
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='user', name='zhaoliu', age=66)
+
         users = db.select('select id, name, age from user')
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         users = db.select('select id, name, age from user where name=?', 'zhangsan')
@@ -126,23 +128,26 @@
             __table__ = 'user'
 
             def __init__(self, id: int = None, name: str = None, age: int = None):
                 self.id = id
                 self.name = name
                 self.age = age
 
-        users = User.query()
+
+        effected_rowcount = User.insert(name='tianqi', age=77)
+
+        users = User.query(name='tianqi')
+        # select id, name, age from user where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
-        # {'id': 4, 'name': 'lisi', 'age': 26}
-        # {'id': 5, 'name': 'wangwu', 'age': 38}
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
 
         users = User.query(name__eq='zhangsan')
+        # select id, name, age from user where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from mysqlx import with_transaction, transaction
```

### Comparing `mysqlx-1.7.0/README.rst` & `mysqlx-1.7.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -92,15 +92,17 @@
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         users = dbx.select('user.select_by_name', name='zhangsan')
         # result:
         # (3, 'zhangsan', 15)
 
-        # you can direct execte sql with db
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='user', name='zhaoliu', age=66)
+
         users = db.select('select id, name, age from user')
         # result:
         # (3, 'zhangsan', 15)
         # (4, 'lisi', 26)
         # (5, 'wangwu', 38)
 
         users = db.select('select id, name, age from user where name=?', 'zhangsan')
@@ -113,23 +115,26 @@
             __table__ = 'user'
 
             def __init__(self, id: int = None, name: str = None, age: int = None):
                 self.id = id
                 self.name = name
                 self.age = age
 
-        users = User.query()
+
+        effected_rowcount = User.insert(name='tianqi', age=77)
+
+        users = User.query(name='tianqi')
+        # select id, name, age from user where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
-        # {'id': 4, 'name': 'lisi', 'age': 26}
-        # {'id': 5, 'name': 'wangwu', 'age': 38}
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
 
         users = User.query(name__eq='zhangsan')
+        # select id, name, age from user where name = :name
         # result:
-        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from mysqlx import with_transaction, transaction
```

