# Comparing `tmp/sql_constructor-1.0.6.tar.gz` & `tmp/sql_constructor-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_constructor-1.0.6.tar", last modified: Sun Jul 30 16:26:42 2023, max compression
+gzip compressed data, was "sql_constructor-1.0.7.tar", last modified: Sun Jul 30 16:34:41 2023, max compression
```

## Comparing `sql_constructor-1.0.6.tar` & `sql_constructor-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:26:42.639977 sql_constructor-1.0.6/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.6/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8377 2023-07-30 16:26:42.638977 sql_constructor-1.0.6/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     7624 2023-07-30 16:26:04.000000 sql_constructor-1.0.6/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      827 2023-07-30 13:54:22.000000 sql_constructor-1.0.6/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 16:26:42.639977 sql_constructor-1.0.6/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:26:42.637977 sql_constructor-1.0.6/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:26:42.638977 sql_constructor-1.0.6/src/sql_constructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.6/src/sql_constructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.6/src/sql_constructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.6/src/sql_constructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.6/src/sql_constructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.6/src/sql_constructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.6/src/sql_constructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.6/src/sql_constructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:26:42.638977 sql_constructor-1.0.6/src/sql_constructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8377 2023-07-30 16:26:42.000000 sql_constructor-1.0.6/src/sql_constructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 16:26:42.000000 sql_constructor-1.0.6/src/sql_constructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 16:26:42.000000 sql_constructor-1.0.6/src/sql_constructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 16:26:42.000000 sql_constructor-1.0.6/src/sql_constructor.egg-info/top_level.txt
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:34:41.753536 sql_constructor-1.0.7/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.7/LICENSE
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8403 2023-07-30 16:34:41.753536 sql_constructor-1.0.7/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     7650 2023-07-30 16:34:03.000000 sql_constructor-1.0.7/README.md
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      827 2023-07-30 16:34:14.000000 sql_constructor-1.0.7/pyproject.toml
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 16:34:41.753536 sql_constructor-1.0.7/setup.cfg
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:34:41.751536 sql_constructor-1.0.7/src/
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:34:41.753536 sql_constructor-1.0.7/src/sql_constructor/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.7/src/sql_constructor/__init__.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.7/src/sql_constructor/constants.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.7/src/sql_constructor/helpers.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.7/src/sql_constructor/sql_container.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.7/src/sql_constructor/sql_cte.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.7/src/sql_constructor/sql_query.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.7/src/sql_constructor/sql_section.py
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 16:34:41.753536 sql_constructor-1.0.7/src/sql_constructor.egg-info/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8403 2023-07-30 16:34:41.000000 sql_constructor-1.0.7/src/sql_constructor.egg-info/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 16:34:41.000000 sql_constructor-1.0.7/src/sql_constructor.egg-info/SOURCES.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 16:34:41.000000 sql_constructor-1.0.7/src/sql_constructor.egg-info/dependency_links.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 16:34:41.000000 sql_constructor-1.0.7/src/sql_constructor.egg-info/top_level.txt
```

### Comparing `sql_constructor-1.0.6/LICENSE` & `sql_constructor-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/PKG-INFO` & `sql_constructor-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql_constructor
-Version: 1.0.6
+Version: 1.0.7
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sql_constructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sql_constructor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,14 +45,15 @@
 )
 q['where'](
     "name = 'Smart'"
 )
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
+# get sql as string
 sql_text: str = str(container)
 ```
 ### Another portion of theory
 1) Because of sql headers ('select', 'from' and etc.) cannot be unique that's why it is only possible to append sql sections (but not get it back by index).
 2) We register (i.e. append) SqlSection by \_\_getitem\_\_ method of SqlQuery. It is possible to add sections with duplicate header. Header can be any string! SqlSection instances will be written in query in order you set them.
 3) When we call \_\_call\_\_ method of SqlSection we build SqlContainer of SqlSection (combining sql header with values passed by arguments).
 
@@ -83,17 +84,17 @@
 
 #### or later in SqlContainer
 ```python
 import sql_constructor as sc
 
 
 def main():
-	prod_q: sc.SqlContainer = get_product_query()
+	container: sc.SqlContainer = get_product_query()
 	# set variables to existing container
-	prod_q.vars['product_name'] = 'Smart'
+	container.vars['product_name'] = 'Smart'
 
 
 def get_product_query() -> sc.SqlContainer:
 	q = sc.SqlQuery()
 	q['select'](
 	    'id',
 	    'name',
@@ -157,46 +158,46 @@
 You could make query as nested as you would like to.
 ```python
 import sql_constructor as sc
 from typing import List
 
 
 def main():
-	r = sc.SqlQuery()
-    r['select'](
+	q = sc.SqlQuery()
+    q['select'](
         'c.id',
         'c.name',
     )
-    r['from'](
+    q['from'](
         'catalog as c',
     )
-    r['left join lateral'](
+    q['left join lateral'](
         get_left_join_lateral(),
     )
-    r['where']('c.name = !product_name')(product_name='Smart')
+    q['where']('c.name = !product_name')(product_name='Smart')
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
-    r = SqlQuery()
-    r['select'](
+    j = SqlQuery()
+    j['select'](
         'id',
         'expiration_date',
     )
-    r['from']('expiration as e')
-    r['where'](*get_filters())
-    r['limit'](100)
+    j['from']('expiration as e')
+    j['where'](*get_filters())
+    j['limit'](100)
     """
     You could get SqlContainer with wrapped subquery 
     in some different ways:
     # return r('AS exp ON TRUE')
     or
     # return r(wrap='AS exp ON TRUE')
     """
     # or more explicit
-    return r().wrap('AS exp ON TRUE')
+    return j().wrap('AS exp ON TRUE')
 
 
 def get_filters() -> List[str]:
     """Create filters"""
     where = []
     where.append('c.id = e.id')
     where.append('AND expiration_date <= now()')
@@ -206,33 +207,33 @@
 
 It is possible to append string or any SqlContainer to query as new SqlSection without header in this way:
 ```python
 import sql_constructor as sc
 
 
 def main():
-	r = sc.SqlQuery()
-	r += '-- some comment here'
-    r['select'](
+	q = sc.SqlQuery()
+	q += '-- some comment here'
+    q['select'](
         'c.id',
         'c.name',
     )
 ```
 ### Append nested sql statements or subqueries to query
 ```python
 import sql_constructor as sc
 
 
 def main():
-	r = sc.SqlQuery()
-	r['select'](
+	q = sc.SqlQuery()
+	q['select'](
 	    'c.id',
         'c.name',
     )
-	r += get_from_statement()
+	q += get_from_statement()
 	...
 
 
 def get_from_statement() -> sc.SqlContainer:
 	...
 ```
 
@@ -275,42 +276,42 @@
 	"""
     ctes = sc.SqlCte()
     ctes['warehouse_cte'] = get_warehouse_cte()
     # or
     # ctes.reg('warehouse_cte', get_warehouse_cte())
 
 	# you could also get certain cte by name and append new SqlSection to it
-	q = ctes['warehouse_cte']
-	q['limit'](1)
+	a = ctes['warehouse_cte']
+	a['limit'](1)
     
     return ctes()
     
 def get_warehouse_cte() -> sc.SqlQuery:
-	q = sc.SqlQuery()
-    q['select'](
+	a = sc.SqlQuery()
+    a['select'](
         'id',
         'quantity',
     )
-    q['from']('warehouse')
-    q['where'](
+    a['from']('warehouse')
+    a['where'](
         'id = !id',
         'AND quantity > !quantity',
     )(id=11, quantity=10)
-	return q
+	return a
 ```
 
 #### Add ctes to query
 It is so easy!
 ```python
 import sql_constructor as sc
 
 def main():
-	r = sc.SqlQuery()
-    r += get_ctes()
-    r['select'](
+	q = sc.SqlQuery()
+    q += get_ctes()
+    q['select'](
 	    'id',
 	    'name'
     )
     ...
 
 
 def get_ctes() -> sc.SqlContainer:
@@ -318,25 +319,25 @@
 ```
 ### Debugging
 
 #### How to find piece of code by produced sql
 If you would like to find your piece of code in editor by sql produced by sql_constructor then you could mark SqlQuery instances by 'sql_id' parameter before you produce ready sql:
 ```python
 def main():
-	r = sc.SqlQuery()
-    r += get_part_of_query()
-    r['select'](
+	q = sc.SqlQuery()
+    q += get_part_of_query()
+    q['select'](
 	    'id',
 	    'name'
     )
     ...
 
 
 def get_part_of_query() -> sc.SqlContainer:
-	q = SqlQuery(sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b')
+	p = SqlQuery(sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b')
 	...
 ```
 It add comment to produced sql as
 ```sql
 -- sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b'
 ...
 ```
```

### Comparing `sql_constructor-1.0.6/README.md` & `sql_constructor-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 )
 q['where'](
     "name = 'Smart'"
 )
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
+# get sql as string
 sql_text: str = str(container)
 ```
 ### Another portion of theory
 1) Because of sql headers ('select', 'from' and etc.) cannot be unique that's why it is only possible to append sql sections (but not get it back by index).
 2) We register (i.e. append) SqlSection by \_\_getitem\_\_ method of SqlQuery. It is possible to add sections with duplicate header. Header can be any string! SqlSection instances will be written in query in order you set them.
 3) When we call \_\_call\_\_ method of SqlSection we build SqlContainer of SqlSection (combining sql header with values passed by arguments).
 
@@ -69,17 +70,17 @@
 
 #### or later in SqlContainer
 ```python
 import sql_constructor as sc
 
 
 def main():
-	prod_q: sc.SqlContainer = get_product_query()
+	container: sc.SqlContainer = get_product_query()
 	# set variables to existing container
-	prod_q.vars['product_name'] = 'Smart'
+	container.vars['product_name'] = 'Smart'
 
 
 def get_product_query() -> sc.SqlContainer:
 	q = sc.SqlQuery()
 	q['select'](
 	    'id',
 	    'name',
@@ -143,46 +144,46 @@
 You could make query as nested as you would like to.
 ```python
 import sql_constructor as sc
 from typing import List
 
 
 def main():
-	r = sc.SqlQuery()
-    r['select'](
+	q = sc.SqlQuery()
+    q['select'](
         'c.id',
         'c.name',
     )
-    r['from'](
+    q['from'](
         'catalog as c',
     )
-    r['left join lateral'](
+    q['left join lateral'](
         get_left_join_lateral(),
     )
-    r['where']('c.name = !product_name')(product_name='Smart')
+    q['where']('c.name = !product_name')(product_name='Smart')
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
-    r = SqlQuery()
-    r['select'](
+    j = SqlQuery()
+    j['select'](
         'id',
         'expiration_date',
     )
-    r['from']('expiration as e')
-    r['where'](*get_filters())
-    r['limit'](100)
+    j['from']('expiration as e')
+    j['where'](*get_filters())
+    j['limit'](100)
     """
     You could get SqlContainer with wrapped subquery 
     in some different ways:
     # return r('AS exp ON TRUE')
     or
     # return r(wrap='AS exp ON TRUE')
     """
     # or more explicit
-    return r().wrap('AS exp ON TRUE')
+    return j().wrap('AS exp ON TRUE')
 
 
 def get_filters() -> List[str]:
     """Create filters"""
     where = []
     where.append('c.id = e.id')
     where.append('AND expiration_date <= now()')
@@ -192,33 +193,33 @@
 
 It is possible to append string or any SqlContainer to query as new SqlSection without header in this way:
 ```python
 import sql_constructor as sc
 
 
 def main():
-	r = sc.SqlQuery()
-	r += '-- some comment here'
-    r['select'](
+	q = sc.SqlQuery()
+	q += '-- some comment here'
+    q['select'](
         'c.id',
         'c.name',
     )
 ```
 ### Append nested sql statements or subqueries to query
 ```python
 import sql_constructor as sc
 
 
 def main():
-	r = sc.SqlQuery()
-	r['select'](
+	q = sc.SqlQuery()
+	q['select'](
 	    'c.id',
         'c.name',
     )
-	r += get_from_statement()
+	q += get_from_statement()
 	...
 
 
 def get_from_statement() -> sc.SqlContainer:
 	...
 ```
 
@@ -261,42 +262,42 @@
 	"""
     ctes = sc.SqlCte()
     ctes['warehouse_cte'] = get_warehouse_cte()
     # or
     # ctes.reg('warehouse_cte', get_warehouse_cte())
 
 	# you could also get certain cte by name and append new SqlSection to it
-	q = ctes['warehouse_cte']
-	q['limit'](1)
+	a = ctes['warehouse_cte']
+	a['limit'](1)
     
     return ctes()
     
 def get_warehouse_cte() -> sc.SqlQuery:
-	q = sc.SqlQuery()
-    q['select'](
+	a = sc.SqlQuery()
+    a['select'](
         'id',
         'quantity',
     )
-    q['from']('warehouse')
-    q['where'](
+    a['from']('warehouse')
+    a['where'](
         'id = !id',
         'AND quantity > !quantity',
     )(id=11, quantity=10)
-	return q
+	return a
 ```
 
 #### Add ctes to query
 It is so easy!
 ```python
 import sql_constructor as sc
 
 def main():
-	r = sc.SqlQuery()
-    r += get_ctes()
-    r['select'](
+	q = sc.SqlQuery()
+    q += get_ctes()
+    q['select'](
 	    'id',
 	    'name'
     )
     ...
 
 
 def get_ctes() -> sc.SqlContainer:
@@ -304,25 +305,25 @@
 ```
 ### Debugging
 
 #### How to find piece of code by produced sql
 If you would like to find your piece of code in editor by sql produced by sql_constructor then you could mark SqlQuery instances by 'sql_id' parameter before you produce ready sql:
 ```python
 def main():
-	r = sc.SqlQuery()
-    r += get_part_of_query()
-    r['select'](
+	q = sc.SqlQuery()
+    q += get_part_of_query()
+    q['select'](
 	    'id',
 	    'name'
     )
     ...
 
 
 def get_part_of_query() -> sc.SqlContainer:
-	q = SqlQuery(sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b')
+	p = SqlQuery(sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b')
 	...
 ```
 It add comment to produced sql as
 ```sql
 -- sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b'
 ...
 ```
```

### Comparing `sql_constructor-1.0.6/pyproject.toml` & `sql_constructor-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sql_constructor"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sql_constructor-1.0.6/src/sql_constructor/constants.py` & `sql_constructor-1.0.7/src/sql_constructor/constants.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/src/sql_constructor/helpers.py` & `sql_constructor-1.0.7/src/sql_constructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/src/sql_constructor/sql_container.py` & `sql_constructor-1.0.7/src/sql_constructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/src/sql_constructor/sql_cte.py` & `sql_constructor-1.0.7/src/sql_constructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/src/sql_constructor/sql_query.py` & `sql_constructor-1.0.7/src/sql_constructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/src/sql_constructor/sql_section.py` & `sql_constructor-1.0.7/src/sql_constructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.6/src/sql_constructor.egg-info/PKG-INFO` & `sql_constructor-1.0.7/src/sql_constructor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-constructor
-Version: 1.0.6
+Version: 1.0.7
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sql_constructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sql_constructor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,14 +45,15 @@
 )
 q['where'](
     "name = 'Smart'"
 )
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
+# get sql as string
 sql_text: str = str(container)
 ```
 ### Another portion of theory
 1) Because of sql headers ('select', 'from' and etc.) cannot be unique that's why it is only possible to append sql sections (but not get it back by index).
 2) We register (i.e. append) SqlSection by \_\_getitem\_\_ method of SqlQuery. It is possible to add sections with duplicate header. Header can be any string! SqlSection instances will be written in query in order you set them.
 3) When we call \_\_call\_\_ method of SqlSection we build SqlContainer of SqlSection (combining sql header with values passed by arguments).
 
@@ -83,17 +84,17 @@
 
 #### or later in SqlContainer
 ```python
 import sql_constructor as sc
 
 
 def main():
-	prod_q: sc.SqlContainer = get_product_query()
+	container: sc.SqlContainer = get_product_query()
 	# set variables to existing container
-	prod_q.vars['product_name'] = 'Smart'
+	container.vars['product_name'] = 'Smart'
 
 
 def get_product_query() -> sc.SqlContainer:
 	q = sc.SqlQuery()
 	q['select'](
 	    'id',
 	    'name',
@@ -157,46 +158,46 @@
 You could make query as nested as you would like to.
 ```python
 import sql_constructor as sc
 from typing import List
 
 
 def main():
-	r = sc.SqlQuery()
-    r['select'](
+	q = sc.SqlQuery()
+    q['select'](
         'c.id',
         'c.name',
     )
-    r['from'](
+    q['from'](
         'catalog as c',
     )
-    r['left join lateral'](
+    q['left join lateral'](
         get_left_join_lateral(),
     )
-    r['where']('c.name = !product_name')(product_name='Smart')
+    q['where']('c.name = !product_name')(product_name='Smart')
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
-    r = SqlQuery()
-    r['select'](
+    j = SqlQuery()
+    j['select'](
         'id',
         'expiration_date',
     )
-    r['from']('expiration as e')
-    r['where'](*get_filters())
-    r['limit'](100)
+    j['from']('expiration as e')
+    j['where'](*get_filters())
+    j['limit'](100)
     """
     You could get SqlContainer with wrapped subquery 
     in some different ways:
     # return r('AS exp ON TRUE')
     or
     # return r(wrap='AS exp ON TRUE')
     """
     # or more explicit
-    return r().wrap('AS exp ON TRUE')
+    return j().wrap('AS exp ON TRUE')
 
 
 def get_filters() -> List[str]:
     """Create filters"""
     where = []
     where.append('c.id = e.id')
     where.append('AND expiration_date <= now()')
@@ -206,33 +207,33 @@
 
 It is possible to append string or any SqlContainer to query as new SqlSection without header in this way:
 ```python
 import sql_constructor as sc
 
 
 def main():
-	r = sc.SqlQuery()
-	r += '-- some comment here'
-    r['select'](
+	q = sc.SqlQuery()
+	q += '-- some comment here'
+    q['select'](
         'c.id',
         'c.name',
     )
 ```
 ### Append nested sql statements or subqueries to query
 ```python
 import sql_constructor as sc
 
 
 def main():
-	r = sc.SqlQuery()
-	r['select'](
+	q = sc.SqlQuery()
+	q['select'](
 	    'c.id',
         'c.name',
     )
-	r += get_from_statement()
+	q += get_from_statement()
 	...
 
 
 def get_from_statement() -> sc.SqlContainer:
 	...
 ```
 
@@ -275,42 +276,42 @@
 	"""
     ctes = sc.SqlCte()
     ctes['warehouse_cte'] = get_warehouse_cte()
     # or
     # ctes.reg('warehouse_cte', get_warehouse_cte())
 
 	# you could also get certain cte by name and append new SqlSection to it
-	q = ctes['warehouse_cte']
-	q['limit'](1)
+	a = ctes['warehouse_cte']
+	a['limit'](1)
     
     return ctes()
     
 def get_warehouse_cte() -> sc.SqlQuery:
-	q = sc.SqlQuery()
-    q['select'](
+	a = sc.SqlQuery()
+    a['select'](
         'id',
         'quantity',
     )
-    q['from']('warehouse')
-    q['where'](
+    a['from']('warehouse')
+    a['where'](
         'id = !id',
         'AND quantity > !quantity',
     )(id=11, quantity=10)
-	return q
+	return a
 ```
 
 #### Add ctes to query
 It is so easy!
 ```python
 import sql_constructor as sc
 
 def main():
-	r = sc.SqlQuery()
-    r += get_ctes()
-    r['select'](
+	q = sc.SqlQuery()
+    q += get_ctes()
+    q['select'](
 	    'id',
 	    'name'
     )
     ...
 
 
 def get_ctes() -> sc.SqlContainer:
@@ -318,25 +319,25 @@
 ```
 ### Debugging
 
 #### How to find piece of code by produced sql
 If you would like to find your piece of code in editor by sql produced by sql_constructor then you could mark SqlQuery instances by 'sql_id' parameter before you produce ready sql:
 ```python
 def main():
-	r = sc.SqlQuery()
-    r += get_part_of_query()
-    r['select'](
+	q = sc.SqlQuery()
+    q += get_part_of_query()
+    q['select'](
 	    'id',
 	    'name'
     )
     ...
 
 
 def get_part_of_query() -> sc.SqlContainer:
-	q = SqlQuery(sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b')
+	p = SqlQuery(sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b')
 	...
 ```
 It add comment to produced sql as
 ```sql
 -- sql_id='25b11c69-ae05-4804-89ea-8ee405f6be8b'
 ...
 ```
```

