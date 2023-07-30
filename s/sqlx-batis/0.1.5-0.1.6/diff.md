# Comparing `tmp/sqlx-batis-0.1.5.tar.gz` & `tmp/sqlx-batis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.5.tar", last modified: Sun Jul 30 01:51:05 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.6.tar", last modified: Sun Jul 30 06:49:08 2023, max compression
```

## Comparing `sqlx-batis-0.1.5.tar` & `sqlx-batis-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/
--rw-rw-rw-   0        0        0     3595 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3112 2023-07-30 01:49:27.000000 sqlx-batis-0.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-30 01:50:59.000000 sqlx-batis-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlbatis/
--rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.5/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.5/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.5/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.5/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.5/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.5/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.5/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.5/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.5/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.5/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.5/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.5/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3595 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 01:51:05.000000 sqlx-batis-0.1.5/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/
+-rw-rw-rw-   0        0        0     4149 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3650 2023-07-30 06:49:05.000000 sqlx-batis-0.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-30 06:46:35.000000 sqlx-batis-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlbatis/
+-rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.6/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.6/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.6/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.6/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.6/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.6/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.6/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.6/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.6/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.6/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.6/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.6/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4149 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.5/PKG-INFO` & `sqlx-batis-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.5
+Version: 0.1.6
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -19,103 +19,119 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/sqlx-batis/blob/master/dtd/mapper.dtd">
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
 
-   from typing import List, Tuple, Mapping
-   from sqlbatis import mapper, sql, dbx, Engin, init_db
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
-       # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
-       # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
-       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
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
+    from sqlbatis.orm import Model
+    from typing import List, Tuple, Mapping
+    from sqlbatis import mapper, sql, dbx, Engin, init_db
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
+        # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
+        # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
+        init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
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
 
 Transaction
 '''''''''''
 
 .. code:: python
 
-   from sqlbatis import with_transaction, transaction
+    from sqlbatis import with_transaction, transaction
 
-   @with_transaction
-   def test_transaction():
-       insert_func(....)
-       update_func(....)
+    @with_transaction
+    def test_transaction():
+        insert_func(....)
+        update_func(....)
 
 
-   def test_transaction2():
-       with transaction():
-           insert_func(....)
-           update_func(....)
+    def test_transaction2():
+        with transaction():
+            insert_func(....)
+            update_func(....)
 
 
 If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
 
 If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
 
 If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `sqlx-batis-0.1.5/README.rst` & `sqlx-batis-0.1.6/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -6,103 +6,119 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/sqlx-batis/blob/master/dtd/mapper.dtd">
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
 
-   from typing import List, Tuple, Mapping
-   from sqlbatis import mapper, sql, dbx, Engin, init_db
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
-       # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
-       # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
-       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
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
+    from sqlbatis.orm import Model
+    from typing import List, Tuple, Mapping
+    from sqlbatis import mapper, sql, dbx, Engin, init_db
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
+        # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
+        # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
+        init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
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
 
 Transaction
 '''''''''''
 
 .. code:: python
 
-   from sqlbatis import with_transaction, transaction
+    from sqlbatis import with_transaction, transaction
 
-   @with_transaction
-   def test_transaction():
-       insert_func(....)
-       update_func(....)
+    @with_transaction
+    def test_transaction():
+        insert_func(....)
+        update_func(....)
 
 
-   def test_transaction2():
-       with transaction():
-           insert_func(....)
-           update_func(....)
+    def test_transaction2():
+        with transaction():
+            insert_func(....)
+            update_func(....)
 
 
 If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
 
 If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
 
 If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `sqlx-batis-0.1.5/setup.py` & `sqlx-batis-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.3.1',
+        'sqlx-exec>=1.3.6',
     ],
-    version='0.1.5',
+    version='0.1.6',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.5/sqlbatis/constant.py` & `sqlx-batis-0.1.6/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/db.py` & `sqlx-batis-0.1.6/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/dbx.py` & `sqlx-batis-0.1.6/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/engine.py` & `sqlx-batis-0.1.6/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/log_support.py` & `sqlx-batis-0.1.6/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/orm.py` & `sqlx-batis-0.1.6/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/snowflake.py` & `sqlx-batis-0.1.6/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.6/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.6/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/sql_support.py` & `sqlx-batis-0.1.6/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlbatis/__init__.py` & `sqlx-batis-0.1.6/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.5/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.6/sqlx_batis.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.5
+Version: 0.1.6
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -19,103 +19,119 @@
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/sqlx-batis/blob/master/dtd/mapper.dtd">
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
 
-   from typing import List, Tuple, Mapping
-   from sqlbatis import mapper, sql, dbx, Engin, init_db
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
-       # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
-       # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
-       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
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
+    from sqlbatis.orm import Model
+    from typing import List, Tuple, Mapping
+    from sqlbatis import mapper, sql, dbx, Engin, init_db
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
+        # init_db('test.db', driver='sqlite3', show_sql=True, debug=True, mapper_path='./mapper')
+        # init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, mapper_path='./mapper')
+        init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
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
 
 Transaction
 '''''''''''
 
 .. code:: python
 
-   from sqlbatis import with_transaction, transaction
+    from sqlbatis import with_transaction, transaction
 
-   @with_transaction
-   def test_transaction():
-       insert_func(....)
-       update_func(....)
+    @with_transaction
+    def test_transaction():
+        insert_func(....)
+        update_func(....)
 
 
-   def test_transaction2():
-       with transaction():
-           insert_func(....)
-           update_func(....)
+    def test_transaction2():
+        with transaction():
+            insert_func(....)
+            update_func(....)
 
 
 If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
 
 If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
 
 If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

