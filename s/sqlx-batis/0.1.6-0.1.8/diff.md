# Comparing `tmp/sqlx-batis-0.1.6.tar.gz` & `tmp/sqlx-batis-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.6.tar", last modified: Sun Jul 30 06:49:08 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.8.tar", last modified: Sun Jul 30 08:46:15 2023, max compression
```

## Comparing `sqlx-batis-0.1.6.tar` & `sqlx-batis-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/
--rw-rw-rw-   0        0        0     4149 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3650 2023-07-30 06:49:05.000000 sqlx-batis-0.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-30 06:46:35.000000 sqlx-batis-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlbatis/
--rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.6/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.6/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.6/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.6/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.6/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.6/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.6/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.6/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.6/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.6/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.6/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.6/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4149 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 06:49:08.000000 sqlx-batis-0.1.6/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/
+-rw-rw-rw-   0        0        0     5701 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.1.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-07-30 08:39:58.000000 sqlx-batis-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlbatis/
+-rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.8/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.8/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.8/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.8/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.8/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.8/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.8/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.8/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.8/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.8/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.8/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.8/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 08:46:15.000000 sqlx-batis-0.1.8/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.6/README.rst` & `sqlx-batis-0.1.8/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
     from sqlbatis.orm import Model
     from typing import List, Tuple, Mapping
-    from sqlbatis import mapper, sql, dbx, Engin, init_db
+    from sqlbatis import mapper, sql, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
     def select_by_name(name: str): List
 
@@ -83,25 +83,66 @@
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
 
+        # you can direct execute sql with db
+        effected_rowcount = db.insert(table='person', name='zhaoliu', age=66)
+
+        persons = db.select('select id, name, age from person')
+        # result:
+        # (3, 'zhangsan', 15)
+        # (4, 'lisi', 26)
+        # (5, 'wangwu', 38)
+        # (6, 'zhaoliu', 45)
+
+        persons = db.query('select id, name, age from person name = :name', name='zhangsan')
+        # result:
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+        persons = db.select('select id, name, age from person where name = ?', 'zhangsan')
+        # result:
+        # [(3, 'zhangsan', 15)]
+
+        # you can use orm to operate a single table
+        class Person(Model):
+            __pk__ = 'id'
+            __table__ = 'person'
+
+            def __init__(self, id: int = None, name: str = None, age: int = None):
+                self.id = id
+                self.name = name
+                self.age = age
+
+
+        effected_rowcount = Person.insert(name='tianqi', age=77)
+
+        persons = Person.query(name='tianqi')
+        # select id, name, age from person where name = :name
+        # result:
+        # {'id': 7, 'name': 'tianqi', 'age': 77}
+
+        persons = Person.query(name__eq='zhangsan')
+        # select id, name, age from person where name = :name
+        # result:
+        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
 Transaction
 '''''''''''
 
 .. code:: python
 
     from sqlbatis import with_transaction, transaction
```

### Comparing `sqlx-batis-0.1.6/setup.py` & `sqlx-batis-0.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='sqlx-batis',
     packages=['sqlbatis'],
-    description="sqlx-batis is a sql executor for Python like MyBatis.",
+    description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.3.6',
+        'sqlx-exec>=1.3.9',
     ],
-    version='0.1.6',
+    version='0.1.8',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.6/sqlbatis/constant.py` & `sqlx-batis-0.1.8/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/db.py` & `sqlx-batis-0.1.8/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/dbx.py` & `sqlx-batis-0.1.8/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/engine.py` & `sqlx-batis-0.1.8/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/log_support.py` & `sqlx-batis-0.1.8/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/orm.py` & `sqlx-batis-0.1.8/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/snowflake.py` & `sqlx-batis-0.1.8/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.8/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.8/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/sql_support.py` & `sqlx-batis-0.1.8/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.6/sqlbatis/__init__.py` & `sqlx-batis-0.1.8/sqlbatis/__init__.py`

 * *Files identical despite different names*

