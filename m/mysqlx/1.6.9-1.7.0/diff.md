# Comparing `tmp/mysqlx-1.6.9.tar.gz` & `tmp/mysqlx-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.6.9.tar", last modified: Sat Jul 29 08:48:36 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.7.0.tar", last modified: Sun Jul 30 06:45:13 2023, max compression
```

## Comparing `mysqlx-1.6.9.tar` & `mysqlx-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:48:36.000000 mysqlx-1.6.9/
-drwxrwxrwx   0        0        0        0 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx/
--rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.6.9/mysqlx/db.py
--rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.6.9/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.6.9/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.6.9/mysqlx/orm.py
--rw-rw-rw-   0        0        0     1487 2023-07-29 08:47:09.000000 mysqlx-1.6.9/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:48:36.000000 mysqlx-1.6.9/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4511 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      279 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4511 2023-07-29 08:48:36.000000 mysqlx-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 08:48:36.000000 mysqlx-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-29 08:47:34.000000 mysqlx-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:45:13.000000 mysqlx-1.7.0/
+drwxrwxrwx   0        0        0        0 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx/
+-rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.7.0/mysqlx/db.py
+-rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.7.0/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.7.0/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.7.0/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     1483 2023-07-29 10:35:00.000000 mysqlx-1.7.0/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4972 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      279 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 06:45:13.000000 mysqlx-1.7.0/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4972 2023-07-30 06:45:13.000000 mysqlx-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4453 2023-07-30 06:25:59.000000 mysqlx-1.7.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 06:45:13.000000 mysqlx-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-30 06:45:05.000000 mysqlx-1.7.0/setup.py
```

### Comparing `mysqlx-1.6.9/mysqlx/db.py` & `mysqlx-1.7.0/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.9/mysqlx/dbx.py` & `mysqlx-1.7.0/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.9/mysqlx/log_support.py` & `mysqlx-1.7.0/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.9/mysqlx/orm.py` & `mysqlx-1.7.0/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.9/mysqlx/__init__.py` & `mysqlx-1.7.0/mysqlx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
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
 
     from sqlbatis.constant import MYSQL
     from sqlbatis import init_db as supper_init_db
```

### Comparing `mysqlx-1.6.9/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.7.0/mysqlx.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.9
+Version: 1.7.0
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -19,115 +19,130 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/mysqlx/blob/master/dtd/mapper.dtd">
    <mapper namespace="user">
        <select id="select_all">
-       <![CDATA[
-            select id, name, age from user
-       ]]>
-       </select>
-       
-       <select id="select_by_name" include="select_all">
-       <![CDATA[
-            {{select_all}}
-            {% if name -%}
-             where name=:name
-            {%- endif -%}
-       ]]>
-       </select>
+           select id, name, age from user
+        </select>
+
+        <select id="select_by_name">
+           select id, name, age from user where name = ?
+        </select>
+
+        <select id="select_by_name2">
+           select id, name, age from user where name = :name
+        </select>
+
+        <select id="select_include" include="select_all">
+           {{ select_all }}
+             {% if name -%}
+              where name = :name
+             {%- endif -%}
+        </select>
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx.orm import Model
-   from typing import List, Tuple, Mapping
-   from mysqlx import mapper, sql, db, dbx, init_db
-
-   @mapper(namespace='user')
-   def select_all(): List
-
-   @mapper(namespace='user')
-   def select_by_name(name: str): List
-
-   @sql('select id, name, age from user')
-   def query_all(): List(Mapping)
-
-   @sql('select id, name, age from user where name=?')
-   def query_by_name(name: str): List(Mapping)
-
-
-   if __name__ == '__main__':
-       init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
-       
-       users = select_all()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = select_by_name(name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       users = query_all()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       users = query_by_name('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       
-       # you can use dbx execte mapper sql with full sql id: namespace join sql id
-       users = dbx.select('user.select_all')  # 'user' is namespace, 'select_all' is sql id
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = dbx.select('user.select_by_name', name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can direct execte sql with db
-       users = db.select('select id, name, age from user')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = db.select('select id, name, age from user where name=?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can use orm to operate a single table
-       class User(Model):
-           __key__ = 'id'
-           __table__ = 'user'
-
-           def __init__(self, id: int = None, name: str = None, age: int = None):
-               self.id = id
-               self.name = name
-               self.age = age
-                     
-       users = User.query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       users = User.query(name__eq='zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+    from mysqlx.orm import Model
+    from typing import List, Tuple, Mapping
+    from mysqlx import mapper, sql, db, dbx, init_db
+
+    @mapper(namespace='user')
+    def select_all(): List
+
+    @mapper(namespace='user')
+    def select_by_name(name: str): List
+
+    @mapper(namespace='user')
+    def select_by_name2(name: str): List
+
+    @mapper(namespace='user')
+    def select_include(name: str): List
+
+    @sql('select id, name, age from user where name = ?')
+    def query_by_name(name: str): List(Mapping)
+
+    @sql('select id, name, age from user where name = :name')
+    def query_by_name2(name: str): List(Mapping)
+
+    if __name__ == '__main__':
+        init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+
+        users = select_all()
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = select_by_name('zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = select_by_name2(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = select_include(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = query_by_name('zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        users = query_by_name2(name='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+       
+        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        users = dbx.select('user.select_all')  # 'user' is namespace, 'select_all' is sql id
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = dbx.select('user.select_by_name', name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can direct execte sql with db
+        users = db.select('select id, name, age from user')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = db.select('select id, name, age from user where name=?', 'zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can use orm to operate a single table
+        class User(Model):
+            __key__ = 'id'
+            __table__ = 'user'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+        users = User.query()
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # {'id': 4, 'name': 'lisi', 'age': 26}
+        # {'id': 5, 'name': 'wangwu', 'age': 38}
+
+        users = User.query(name__eq='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from mysqlx import with_transaction, transaction
```

### Comparing `mysqlx-1.6.9/PKG-INFO` & `mysqlx-1.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.9
+Version: 1.7.0
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -19,115 +19,130 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/mysqlx/blob/master/dtd/mapper.dtd">
    <mapper namespace="user">
        <select id="select_all">
-       <![CDATA[
-            select id, name, age from user
-       ]]>
-       </select>
-       
-       <select id="select_by_name" include="select_all">
-       <![CDATA[
-            {{select_all}}
-            {% if name -%}
-             where name=:name
-            {%- endif -%}
-       ]]>
-       </select>
+           select id, name, age from user
+        </select>
+
+        <select id="select_by_name">
+           select id, name, age from user where name = ?
+        </select>
+
+        <select id="select_by_name2">
+           select id, name, age from user where name = :name
+        </select>
+
+        <select id="select_include" include="select_all">
+           {{ select_all }}
+             {% if name -%}
+              where name = :name
+             {%- endif -%}
+        </select>
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx.orm import Model
-   from typing import List, Tuple, Mapping
-   from mysqlx import mapper, sql, db, dbx, init_db
-
-   @mapper(namespace='user')
-   def select_all(): List
-
-   @mapper(namespace='user')
-   def select_by_name(name: str): List
-
-   @sql('select id, name, age from user')
-   def query_all(): List(Mapping)
-
-   @sql('select id, name, age from user where name=?')
-   def query_by_name(name: str): List(Mapping)
-
-
-   if __name__ == '__main__':
-       init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
-       
-       users = select_all()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = select_by_name(name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       users = query_all()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       users = query_by_name('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       
-       # you can use dbx execte mapper sql with full sql id: namespace join sql id
-       users = dbx.select('user.select_all')  # 'user' is namespace, 'select_all' is sql id
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = dbx.select('user.select_by_name', name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can direct execte sql with db
-       users = db.select('select id, name, age from user')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = db.select('select id, name, age from user where name=?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can use orm to operate a single table
-       class User(Model):
-           __key__ = 'id'
-           __table__ = 'user'
-
-           def __init__(self, id: int = None, name: str = None, age: int = None):
-               self.id = id
-               self.name = name
-               self.age = age
-                     
-       users = User.query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       users = User.query(name__eq='zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+    from mysqlx.orm import Model
+    from typing import List, Tuple, Mapping
+    from mysqlx import mapper, sql, db, dbx, init_db
+
+    @mapper(namespace='user')
+    def select_all(): List
+
+    @mapper(namespace='user')
+    def select_by_name(name: str): List
+
+    @mapper(namespace='user')
+    def select_by_name2(name: str): List
+
+    @mapper(namespace='user')
+    def select_include(name: str): List
+
+    @sql('select id, name, age from user where name = ?')
+    def query_by_name(name: str): List(Mapping)
+
+    @sql('select id, name, age from user where name = :name')
+    def query_by_name2(name: str): List(Mapping)
+
+    if __name__ == '__main__':
+        init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+
+        users = select_all()
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = select_by_name('zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = select_by_name2(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = select_include(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = query_by_name('zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        users = query_by_name2(name='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+       
+        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        users = dbx.select('user.select_all')  # 'user' is namespace, 'select_all' is sql id
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = dbx.select('user.select_by_name', name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can direct execte sql with db
+        users = db.select('select id, name, age from user')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = db.select('select id, name, age from user where name=?', 'zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can use orm to operate a single table
+        class User(Model):
+            __key__ = 'id'
+            __table__ = 'user'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+        users = User.query()
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # {'id': 4, 'name': 'lisi', 'age': 26}
+        # {'id': 5, 'name': 'wangwu', 'age': 38}
+
+        users = User.query(name__eq='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from mysqlx import with_transaction, transaction
```

### Comparing `mysqlx-1.6.9/README.rst` & `mysqlx-1.7.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -6,115 +6,130 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/mysqlx/blob/master/dtd/mapper.dtd">
    <mapper namespace="user">
        <select id="select_all">
-       <![CDATA[
-            select id, name, age from user
-       ]]>
-       </select>
-       
-       <select id="select_by_name" include="select_all">
-       <![CDATA[
-            {{select_all}}
-            {% if name -%}
-             where name=:name
-            {%- endif -%}
-       ]]>
-       </select>
+           select id, name, age from user
+        </select>
+
+        <select id="select_by_name">
+           select id, name, age from user where name = ?
+        </select>
+
+        <select id="select_by_name2">
+           select id, name, age from user where name = :name
+        </select>
+
+        <select id="select_include" include="select_all">
+           {{ select_all }}
+             {% if name -%}
+              where name = :name
+             {%- endif -%}
+        </select>
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx.orm import Model
-   from typing import List, Tuple, Mapping
-   from mysqlx import mapper, sql, db, dbx, init_db
-
-   @mapper(namespace='user')
-   def select_all(): List
-
-   @mapper(namespace='user')
-   def select_by_name(name: str): List
-
-   @sql('select id, name, age from user')
-   def query_all(): List(Mapping)
-
-   @sql('select id, name, age from user where name=?')
-   def query_by_name(name: str): List(Mapping)
-
-
-   if __name__ == '__main__':
-       init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
-       
-       users = select_all()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = select_by_name(name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       users = query_all()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       users = query_by_name('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       
-       # you can use dbx execte mapper sql with full sql id: namespace join sql id
-       users = dbx.select('user.select_all')  # 'user' is namespace, 'select_all' is sql id
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = dbx.select('user.select_by_name', name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can direct execte sql with db
-       users = db.select('select id, name, age from user')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       users = db.select('select id, name, age from user where name=?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can use orm to operate a single table
-       class User(Model):
-           __key__ = 'id'
-           __table__ = 'user'
-
-           def __init__(self, id: int = None, name: str = None, age: int = None):
-               self.id = id
-               self.name = name
-               self.age = age
-                     
-       users = User.query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       users = User.query(name__eq='zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+    from mysqlx.orm import Model
+    from typing import List, Tuple, Mapping
+    from mysqlx import mapper, sql, db, dbx, init_db
+
+    @mapper(namespace='user')
+    def select_all(): List
+
+    @mapper(namespace='user')
+    def select_by_name(name: str): List
+
+    @mapper(namespace='user')
+    def select_by_name2(name: str): List
+
+    @mapper(namespace='user')
+    def select_include(name: str): List
+
+    @sql('select id, name, age from user where name = ?')
+    def query_by_name(name: str): List(Mapping)
+
+    @sql('select id, name, age from user where name = :name')
+    def query_by_name2(name: str): List(Mapping)
+
+    if __name__ == '__main__':
+        init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+
+        users = select_all()
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = select_by_name('zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = select_by_name2(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = select_include(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        users = query_by_name('zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        users = query_by_name2(name='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+       
+        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        users = dbx.select('user.select_all')  # 'user' is namespace, 'select_all' is sql id
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = dbx.select('user.select_by_name', name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can direct execte sql with db
+        users = db.select('select id, name, age from user')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        users = db.select('select id, name, age from user where name=?', 'zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can use orm to operate a single table
+        class User(Model):
+            __key__ = 'id'
+            __table__ = 'user'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+        users = User.query()
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # {'id': 4, 'name': 'lisi', 'age': 26}
+        # {'id': 5, 'name': 'wangwu', 'age': 38}
+
+        users = User.query(name__eq='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from mysqlx import with_transaction, transaction
```

### Comparing `mysqlx-1.6.9/setup.py` & `mysqlx-1.7.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
-        'sqlx-batis>=0.1.3',
+        'sqlx-batis>=0.1.5',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.6.9',
+    version='1.7.0',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

