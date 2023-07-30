# Comparing `tmp/dbhydra-1.2.1.tar.gz` & `tmp/dbhydra-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.2.1.tar", last modified: Sun Jul 30 15:40:34 2023, max compression
+gzip compressed data, was "dbhydra-1.2.2.tar", last modified: Sun Jul 30 16:18:07 2023, max compression
```

## Comparing `dbhydra-1.2.1.tar` & `dbhydra-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 15:40:34.598984 dbhydra-1.2.1/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-07-30 15:40:34.598984 dbhydra-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 15:40:34.586019 dbhydra-1.2.1/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.1/dbhydra/__init__.py
--rw-rw-rw-   0        0        0    69064 2023-07-30 15:36:58.000000 dbhydra-1.2.1/dbhydra/dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:40:34.597987 dbhydra-1.2.1/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.1/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.1/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.1/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.1/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:40:34.595992 dbhydra-1.2.1/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-07-30 15:40:33.000000 dbhydra-1.2.1/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-07-30 15:40:34.000000 dbhydra-1.2.1/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 15:40:34.000000 dbhydra-1.2.1/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-30 15:40:34.000000 dbhydra-1.2.1/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 15:40:34.000000 dbhydra-1.2.1/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 15:40:34.598984 dbhydra-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-07-30 15:37:55.000000 dbhydra-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.980954 dbhydra-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-07-30 16:18:07.979956 dbhydra-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.964996 dbhydra-1.2.2/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.2/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0    69180 2023-07-30 16:17:27.000000 dbhydra-1.2.2/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.979956 dbhydra-1.2.2/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.2/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:18:07.976964 dbhydra-1.2.2/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 16:18:07.000000 dbhydra-1.2.2/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:18:07.980954 dbhydra-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-07-30 16:17:38.000000 dbhydra-1.2.2/setup.py
```

### Comparing `dbhydra-1.2.1/LICENSE` & `dbhydra-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.1/PKG-INFO` & `dbhydra-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.2.1
+Version: 1.2.2
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.2.1/README.md` & `dbhydra-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.1/dbhydra/dbhydra_core.py` & `dbhydra-1.2.2/dbhydra/dbhydra_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -763,15 +763,15 @@
         """id_column_name -> name of predefined column with autoincrement + PK"""
         super().__init__(db1, name, columns)
         self.types = types
         self.id_column_name = id_column_name
 
     # Temporary disabled, please make sure this is implemented where needed, don't introduce breaking changes please
     # @abc.abstractmethod
-    def init_from_column_type_dict(db1, name, column_type_dict):
+    def init_from_column_type_dict(db1, name, column_type_dict, init_from_column_type_dict="id"):
         pass
 
     def drop(self):
         query = "DROP TABLE " + self.name
         print(query)
         self.db1.execute(query)
 
@@ -1399,19 +1399,19 @@
 class MysqlTable(MysqlSelectable, AbstractTable):
     def __init__(self, db1, name, columns=None, types=None, id_column_name = "id"):
         super().__init__(db1, name, columns)
         self.types = types
         self.id_column_name = id_column_name
 
     @classmethod
-    def init_from_column_type_dict(cls, db1, name, column_type_dict):
+    def init_from_column_type_dict(cls, db1, name, column_type_dict, id_column_name="id"):
         column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
         columns = list(column_converted_type_dict.keys())
         types = list(column_converted_type_dict.values())
-        return cls(db1, name, columns, types)
+        return cls(db1, name, columns, types, id_column_name=id_column_name)
 
     def initialize_columns(self):
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS')
         query = f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = '{self.db1.DB_DATABASE}' AND  TABLE_NAME  = '" + self.name + "';"
         columns = information_schema_table.select(query)
         self.columns = columns
 
@@ -1799,15 +1799,15 @@
     return (df)
 
 
 class AbstractModel(abc.ABC, BaseModel):
     @classmethod
     def generate_dbhydra_table(cls, table_class: AbstractTable, db1, name, id_column_name="id"):
         column_type_dict = create_table_structure_dict(cls, id_column_name=id_column_name)
-        dbhydra_table = table_class.init_from_column_type_dict(db1, name, column_type_dict)
+        dbhydra_table = table_class.init_from_column_type_dict(db1, name, column_type_dict, id_column_name=id_column_name)
         return dbhydra_table
 
  
 
 def create_table_structure_dict(api_class_instance, id_column_name="id"):
     """
     Accepts instance of API data class (e.g. APIDatabase) and converts it to dictionary {attribute_name: attribute_type}
```

### Comparing `dbhydra-1.2.1/dbhydra/tests/test_mongo.py` & `dbhydra-1.2.2/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.1/dbhydra/tests/test_sql.py` & `dbhydra-1.2.2/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.2.1/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.2.2/dbhydra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.2.1
+Version: 1.2.2
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.2.1/setup.py` & `dbhydra-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.2.1',
+    version='1.2.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

