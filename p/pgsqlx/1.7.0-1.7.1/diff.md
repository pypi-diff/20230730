# Comparing `tmp/pgsqlx-1.7.0.tar.gz` & `tmp/pgsqlx-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.7.0.tar", last modified: Sat Jul 29 08:49:17 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.7.1.tar", last modified: Sun Jul 30 06:50:43 2023, max compression
```

## Comparing `pgsqlx-1.7.0.tar` & `pgsqlx-1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/
-drwxrwxrwx   0        0        0        0 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx/
--rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.0/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.0/pgsqlx/db.py
--rw-rw-rw-   0        0        0     1250 2023-07-28 02:45:27.000000 pgsqlx-1.7.0/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.0/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.7.0/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.0/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     1505 2023-07-29 08:25:34.000000 pgsqlx-1.7.0/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4612 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4612 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.7.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-07-29 08:48:18.000000 pgsqlx-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/
+drwxrwxrwx   0        0        0        0 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx/
+-rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.1/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.1/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1250 2023-07-28 02:45:27.000000 pgsqlx-1.7.1/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.1/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.7.1/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.1/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     1501 2023-07-29 10:35:25.000000 pgsqlx-1.7.1/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5079 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      319 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5079 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4548 2023-07-30 06:50:05.000000 pgsqlx-1.7.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 06:50:43.000000 pgsqlx-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-30 06:50:36.000000 pgsqlx-1.7.1/setup.py
```

### Comparing `pgsqlx-1.7.0/pgsqlx/db.py` & `pgsqlx-1.7.1/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.0/pgsqlx/dbx.py` & `pgsqlx-1.7.1/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.0/pgsqlx/log_support.py` & `pgsqlx-1.7.1/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.0/pgsqlx/orm.py` & `pgsqlx-1.7.1/pgsqlx/orm.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.0/pgsqlx/sql_mapper.py` & `pgsqlx-1.7.1/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.0/pgsqlx/__init__.py` & `pgsqlx-1.7.1/pgsqlx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
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
     from .constant import POSTGRESQL
     from sqlbatis import init_db as supper_init_db
 
     PostgresEngine.init(name=POSTGRESQL)
```

### Comparing `pgsqlx-1.7.0/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.7.1/pgsqlx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.7.0
+Version: 1.7.1
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -19,116 +19,131 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/pgsqlx/blob/master/dtd/mapper.dtd">
    <mapper namespace="person">
        <select id="select_all">
-       <![CDATA[
-            select id, name, age from person
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
+           select id, name, age from person
+        </select>
+
+        <select id="select_by_name">
+           select id, name, age from person where name = ?
+        </select>
+
+        <select id="select_by_name2">
+           select id, name, age from person where name = :name
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
 
-   from pgsqlx.orm import Model
-   from typing import List, Tuple, Mapping
-   from pgsqlx import mapper, sql, db, dbx, init_db
-
-   @mapper(namespace='person')
-   def select_all(): List
-
-   @mapper(namespace='person')
-   def select_by_name(name: str): List
-
-   @sql('select id, name, age from person')
-   def query_all(): List(Mapping)
-
-   @sql('select id, name, age from person where name=?')
-   def query_by_name(name: str): List(Mapping)
-
-
-   if __name__ == '__main__':
-       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
-       
-       persons = select_all()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = select_by_name(name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       persons = query_all()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       persons = query_by_name('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       
-       # you can use dbx execte mapper sql with full sql id: namespace join sql id
-       persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = dbx.select('person.select_by_name', name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can direct execte sql with db
-       persons = db.select('select id, name, age from person')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = db.select('select id, name, age from person where name=?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can use orm to operate a single table
-       class person(Model):
-           __pk__ = 'id'
-           __table__ = 'person'
-           __pk_seq__ = 'person_id_seq'
-
-           def __init__(self, id: int = None, name: str = None, age: int = None):
-               self.id = id
-               self.name = name
-               self.age = age
-                     
-       persons = person.query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       persons = person.query(name__eq='zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+    from pgsqlx.orm import Model
+    from typing import List, Tuple, Mapping
+    from pgsqlx import mapper, sql, db, dbx, init_db
+
+    @mapper(namespace='person')
+    def select_all(): List
+
+    @mapper(namespace='person')
+    def select_by_name(name: str): List
+
+    @mapper(namespace='person')
+    def select_by_name2(name: str): List
+
+    @mapper(namespace='person')
+    def select_include(name: str): List
+
+    @sql('select id, name, age from person where name = ?')
+    def query_by_name(name: str): List(Mapping)
+
+    @sql('select id, name, age from person where name = :name')
+    def query_by_name2(name: str): List(Mapping)
+
+    if __name__ == '__main__':
+        init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+
+        persons = select_all()
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = select_by_name('zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = select_by_name2(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = select_include(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = query_by_name('zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        persons = query_by_name2(name='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = dbx.select('person.select_by_name', name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can direct execte sql with db
+        persons = db.select('select id, name, age from person')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = db.select('select id, name, age from person where name=?', 'zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can use orm to operate a single table
+        class person(Model):
+            __pk__ = 'id'
+            __table__ = 'person'
+            __pk_seq__ = 'person_id_seq'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+        persons = person.query()
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # {'id': 4, 'name': 'lisi', 'age': 26}
+        # {'id': 5, 'name': 'wangwu', 'age': 38}
+
+        persons = person.query(name__eq='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from pgsqlx import with_transaction, transaction
```

### Comparing `pgsqlx-1.7.0/PKG-INFO` & `pgsqlx-1.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.7.0
+Version: 1.7.1
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -19,116 +19,131 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/pgsqlx/blob/master/dtd/mapper.dtd">
    <mapper namespace="person">
        <select id="select_all">
-       <![CDATA[
-            select id, name, age from person
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
+           select id, name, age from person
+        </select>
+
+        <select id="select_by_name">
+           select id, name, age from person where name = ?
+        </select>
+
+        <select id="select_by_name2">
+           select id, name, age from person where name = :name
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
 
-   from pgsqlx.orm import Model
-   from typing import List, Tuple, Mapping
-   from pgsqlx import mapper, sql, db, dbx, init_db
-
-   @mapper(namespace='person')
-   def select_all(): List
-
-   @mapper(namespace='person')
-   def select_by_name(name: str): List
-
-   @sql('select id, name, age from person')
-   def query_all(): List(Mapping)
-
-   @sql('select id, name, age from person where name=?')
-   def query_by_name(name: str): List(Mapping)
-
-
-   if __name__ == '__main__':
-       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
-       
-       persons = select_all()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = select_by_name(name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       persons = query_all()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       persons = query_by_name('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       
-       # you can use dbx execte mapper sql with full sql id: namespace join sql id
-       persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = dbx.select('person.select_by_name', name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can direct execte sql with db
-       persons = db.select('select id, name, age from person')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = db.select('select id, name, age from person where name=?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can use orm to operate a single table
-       class person(Model):
-           __pk__ = 'id'
-           __table__ = 'person'
-           __pk_seq__ = 'person_id_seq'
-
-           def __init__(self, id: int = None, name: str = None, age: int = None):
-               self.id = id
-               self.name = name
-               self.age = age
-                     
-       persons = person.query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       persons = person.query(name__eq='zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+    from pgsqlx.orm import Model
+    from typing import List, Tuple, Mapping
+    from pgsqlx import mapper, sql, db, dbx, init_db
+
+    @mapper(namespace='person')
+    def select_all(): List
+
+    @mapper(namespace='person')
+    def select_by_name(name: str): List
+
+    @mapper(namespace='person')
+    def select_by_name2(name: str): List
+
+    @mapper(namespace='person')
+    def select_include(name: str): List
+
+    @sql('select id, name, age from person where name = ?')
+    def query_by_name(name: str): List(Mapping)
+
+    @sql('select id, name, age from person where name = :name')
+    def query_by_name2(name: str): List(Mapping)
+
+    if __name__ == '__main__':
+        init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+
+        persons = select_all()
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = select_by_name('zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = select_by_name2(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = select_include(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = query_by_name('zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        persons = query_by_name2(name='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = dbx.select('person.select_by_name', name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can direct execte sql with db
+        persons = db.select('select id, name, age from person')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = db.select('select id, name, age from person where name=?', 'zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can use orm to operate a single table
+        class person(Model):
+            __pk__ = 'id'
+            __table__ = 'person'
+            __pk_seq__ = 'person_id_seq'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+        persons = person.query()
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # {'id': 4, 'name': 'lisi', 'age': 26}
+        # {'id': 5, 'name': 'wangwu', 'age': 38}
+
+        persons = person.query(name__eq='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from pgsqlx import with_transaction, transaction
```

### Comparing `pgsqlx-1.7.0/README.rst` & `pgsqlx-1.7.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -6,116 +6,131 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/pgsqlx/blob/master/dtd/mapper.dtd">
    <mapper namespace="person">
        <select id="select_all">
-       <![CDATA[
-            select id, name, age from person
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
+           select id, name, age from person
+        </select>
+
+        <select id="select_by_name">
+           select id, name, age from person where name = ?
+        </select>
+
+        <select id="select_by_name2">
+           select id, name, age from person where name = :name
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
 
-   from pgsqlx.orm import Model
-   from typing import List, Tuple, Mapping
-   from pgsqlx import mapper, sql, db, dbx, init_db
-
-   @mapper(namespace='person')
-   def select_all(): List
-
-   @mapper(namespace='person')
-   def select_by_name(name: str): List
-
-   @sql('select id, name, age from person')
-   def query_all(): List(Mapping)
-
-   @sql('select id, name, age from person where name=?')
-   def query_by_name(name: str): List(Mapping)
-
-
-   if __name__ == '__main__':
-       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
-       
-       persons = select_all()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = select_by_name(name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       persons = query_all()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       persons = query_by_name('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       
-       # you can use dbx execte mapper sql with full sql id: namespace join sql id
-       persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = dbx.select('person.select_by_name', name='zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can direct execte sql with db
-       persons = db.select('select id, name, age from person')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       
-       persons = db.select('select id, name, age from person where name=?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
-       
-       # you can use orm to operate a single table
-       class person(Model):
-           __pk__ = 'id'
-           __table__ = 'person'
-           __pk_seq__ = 'person_id_seq'
-
-           def __init__(self, id: int = None, name: str = None, age: int = None):
-               self.id = id
-               self.name = name
-               self.age = age
-                     
-       persons = person.query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       
-       persons = person.query(name__eq='zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+    from pgsqlx.orm import Model
+    from typing import List, Tuple, Mapping
+    from pgsqlx import mapper, sql, db, dbx, init_db
+
+    @mapper(namespace='person')
+    def select_all(): List
+
+    @mapper(namespace='person')
+    def select_by_name(name: str): List
+
+    @mapper(namespace='person')
+    def select_by_name2(name: str): List
+
+    @mapper(namespace='person')
+    def select_include(name: str): List
+
+    @sql('select id, name, age from person where name = ?')
+    def query_by_name(name: str): List(Mapping)
+
+    @sql('select id, name, age from person where name = :name')
+    def query_by_name2(name: str): List(Mapping)
+
+    if __name__ == '__main__':
+        init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+
+        persons = select_all()
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = select_by_name('zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = select_by_name2(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = select_include(name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        persons = query_by_name('zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        persons = query_by_name2(name='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+        # you can use dbx execte mapper sql with full sql id: namespace join sql id
+        persons = dbx.select('person.select_all')  # 'person' is namespace, 'select_all' is sql id
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = dbx.select('person.select_by_name', name='zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can direct execte sql with db
+        persons = db.select('select id, name, age from person')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+
+        persons = db.select('select id, name, age from person where name=?', 'zhangsan')
+        # result:
+        # (3, 'zhangsan', 15)
+
+        # you can use orm to operate a single table
+        class person(Model):
+            __pk__ = 'id'
+            __table__ = 'person'
+            __pk_seq__ = 'person_id_seq'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+        persons = person.query()
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
+        # {'id': 4, 'name': 'lisi', 'age': 26}
+        # {'id': 5, 'name': 'wangwu', 'age': 38}
+
+        persons = person.query(name__eq='zhangsan')
+        # result:
+        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from pgsqlx import with_transaction, transaction
```

### Comparing `pgsqlx-1.7.0/setup.py` & `pgsqlx-1.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     packages=['pgsqlx'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
         # 'psycopg2>=2.7.4',
-        'sqlx-batis>=0.1.3',
+        'sqlx-batis>=0.1.5',
     ],
-    version='1.7.0',
+    version='1.7.1',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

