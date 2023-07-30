# Comparing `tmp/dbhydra-1.1.0.tar.gz` & `tmp/dbhydra-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.1.0.tar", last modified: Thu Jul 20 01:12:21 2023, max compression
+gzip compressed data, was "dbhydra-1.2.0.tar", last modified: Sun Jul 30 15:29:26 2023, max compression
```

## Comparing `dbhydra-1.1.0.tar` & `dbhydra-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 01:12:21.941140 dbhydra-1.1.0/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-07-20 01:12:21.941140 dbhydra-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 01:12:21.905236 dbhydra-1.1.0/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.1.0/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.1.0/dbhydra/dbhydra_builder.py
--rw-rw-rw-   0        0        0    68321 2023-07-20 01:11:45.000000 dbhydra-1.1.0/dbhydra/dbhydra_core.py
--rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.1.0/dbhydra/dbhydra_liquibase.py
--rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.1.0/dbhydra/dbhydra_model.py
--rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.1.0/dbhydra/dbhydra_mysql_example - kopie.py
--rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.1.0/dbhydra/dbhydra_pandas_framework.py
--rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.1.0/dbhydra/mongo.py
--rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.1.0/dbhydra/test.py
-drwxrwxrwx   0        0        0        0 2023-07-20 01:12:21.940143 dbhydra-1.1.0/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.1.0/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.1.0/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.1.0/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.1.0/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-07-20 01:12:21.921193 dbhydra-1.1.0/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-07-20 01:12:21.000000 dbhydra-1.1.0/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2023-07-20 01:12:21.000000 dbhydra-1.1.0/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 01:12:21.000000 dbhydra-1.1.0/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-20 01:12:21.000000 dbhydra-1.1.0/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-20 01:12:21.000000 dbhydra-1.1.0/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 01:12:21.941140 dbhydra-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-07-20 01:12:04.000000 dbhydra-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:29:26.356331 dbhydra-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-07-30 15:29:26.355334 dbhydra-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 15:29:26.318432 dbhydra-1.2.0/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.2.0/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0    68981 2023-07-30 15:27:19.000000 dbhydra-1.2.0/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:29:26.354336 dbhydra-1.2.0/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.2.0/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.2.0/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.2.0/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.2.0/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:29:26.337381 dbhydra-1.2.0/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-07-30 15:29:25.000000 dbhydra-1.2.0/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-07-30 15:29:26.000000 dbhydra-1.2.0/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:29:25.000000 dbhydra-1.2.0/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-30 15:29:26.000000 dbhydra-1.2.0/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 15:29:26.000000 dbhydra-1.2.0/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 15:29:26.356331 dbhydra-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-07-30 15:29:09.000000 dbhydra-1.2.0/setup.py
```

### Comparing `dbhydra-1.1.0/LICENSE` & `dbhydra-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.1.0/PKG-INFO` & `dbhydra-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.1.0
+Version: 1.2.0
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.1.0/README.md` & `dbhydra-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.1.0/dbhydra/dbhydra_core.py` & `dbhydra-1.2.0/dbhydra/dbhydra_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -755,17 +755,19 @@
 
 
 class Joinable(Selectable):
     pass
 
 
 class AbstractTable(AbstractJoinable, abc.ABC):
-    def __init__(self, db1, name, columns=None, types=None):
+    def __init__(self, db1, name, columns = None, types = None, id_column_name = "id"):
+        """id_column_name -> name of predefined column with autoincrement + PK"""
         super().__init__(db1, name, columns)
         self.types = types
+        self.id_column_name = id_column_name
 
     # Temporary disabled, please make sure this is implemented where needed, don't introduce breaking changes please
     # @abc.abstractmethod
     def init_from_column_type_dict(db1, name, column_type_dict):
         pass
 
     def drop(self):
@@ -826,15 +828,15 @@
             
             inserted_columns=self.columns
             
         else:
             assert len(df.columns) + 1 == len(self.columns) # +1 because of id column
             
             inserted_columns=list(dict.fromkeys(self.columns)) #DEDUPLICATION preserving order -> better than inserted_columns = set(self.columns) 
-            id_index=inserted_columns.index("id")
+            id_index=inserted_columns.index(self.id_column_name)
             inserted_columns.pop(id_index)
             print(inserted_columns,df.columns)
             
             assert set(df.columns) == set(inserted_columns) #elements are matchin
             #df = df[inserted_columns]
         df = df[inserted_columns]
 
@@ -933,29 +935,29 @@
 
     @classmethod
     def init_all_columns(cls, db1, name):
         temporary_table = cls(db1, name)
         columns = temporary_table.get_all_columns()
         types = temporary_table.get_all_types()
 
-        if "id" in columns:
-            id_col_index = columns.index("id")
+        if temporary_table.id_column_name in columns:
+            id_col_index = columns.index(temporary_table.id_column_name)
             columns.pop(id_col_index)
-            columns.insert(0, "id")
+            columns.insert(0, temporary_table.id_column_name)
             types.pop(id_col_index)
             types.insert(0, "int")
 
         return (cls(db1, name, columns, types))
 
     # @save_migration
     def create(self, foreign_keys=None):
         assert len(self.columns) == len(self.types)
-        assert self.columns[0] == "id"
+        assert self.columns[0] == self.id_column_name
         assert self.types[0].lower() == "int" or self.types[0].lower() == "integer"
-        query = "CREATE TABLE " + self.name + "(id SERIAL PRIMARY KEY,"
+        query = "CREATE TABLE " + self.name + "("+self.id_column_name+" SERIAL PRIMARY KEY,"
         for i in range(1, len(self.columns)):
             query += self.columns[i] + " " + self.types[i] + ","
 
         query = query[:-1]
         query += ");"
         print(query)
         try:
@@ -1195,20 +1197,20 @@
     def init_all_columns(cls, db1, name):
 
         temporary_table = cls(db1, name)
         values = temporary_table.get_columns_types()
         columns = values[0][1:]
         types = values[1][1:]
 
-        if "id" in columns:
-            index = columns.index("id")
+        if temporary_table.id_column_name in columns:
+            index = columns.index(temporary_table.id_column_name)
             columns.pop(index)
             types.pop(index)
 
-        columns.insert(0, "id")
+        columns.insert(0, temporary_table.id_column_name)
         types.insert(0, "int")
         types = [x.lower() for x in types]
         types_ = [PYTHON_TO_MYSQL_DATA_MAPPING[x] for x in types]
         types = types_
         return (cls(db1, name, columns, types))
 
     def keys_exists(self, element, *keys):
@@ -1299,20 +1301,20 @@
         information_schema_table = Table(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
         query = "SELECT DATA_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME  = '" + self.name + "'"
         types = information_schema_table.select(query)
         return (types)
 
     def create(self):
         assert len(self.columns) == len(self.types)
-        assert self.columns[0] == "id"
+        assert self.columns[0] == self.id_column_name
         assert self.types[0].lower() == "int"
-        query = "CREATE TABLE " + self.name + "(id INT IDENTITY(1,1) NOT NULL,"
+        query = "CREATE TABLE " + self.name + "("+self.id_column_name+" INT IDENTITY(1,1) NOT NULL,"
         for i in range(1, len(self.columns)):
             query += self.columns[i] + " " + self.types[i] + ","
-        query += "PRIMARY KEY(id))"
+        query += "PRIMARY KEY("+self.id_column_name+"))"
 
         print(query)
         try:
             self.db1.execute(query)
         except Exception as e:
             print("Table " + self.name + " already exists:", e)
             print("Check the specification of table columns and their types")
@@ -1391,17 +1393,18 @@
                     parent_foreign_keys.append(fk)
                 except IndexError as e:
                     print("Warning: IndexError for foreign key self.columns[fk[parent_column_id]]:", e)
         return (parent_foreign_keys)
 
 
 class MysqlTable(MysqlSelectable, AbstractTable):
-    def __init__(self, db1, name, columns=None, types=None):
+    def __init__(self, db1, name, columns=None, types=None, id_column_name = "id"):
         super().__init__(db1, name, columns)
         self.types = types
+        self.id_column_name = id_column_name
 
     @classmethod
     def init_from_column_type_dict(cls, db1, name, column_type_dict):
         column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
         columns = list(column_converted_type_dict.keys())
         types = list(column_converted_type_dict.values())
         return cls(db1, name, columns, types)
@@ -1471,31 +1474,31 @@
 
     @classmethod
     def init_all_columns(cls, db1, name):
         temporary_table = cls(db1, name)
         columns = temporary_table.get_all_columns()
         types = temporary_table.get_all_types()
 
-        if "id" in columns:
-            id_col_index = columns.index("id")
+        if temporary_table.id_column_name in columns:
+            id_col_index = columns.index(temporary_table.id_column_name)
             columns.pop(id_col_index)
-            columns.insert(0, "id")
+            columns.insert(0, temporary_table.id_column_name)
             types.pop(id_col_index)
             types.insert(0, "int")
 
 
 
         return (cls(db1, name, columns, types))
 
     def get_last_id(self):
         """
         Returns the biggest id from table
         """
 
-        last_id = self.select(f"SELECT id FROM {self.name} ORDER BY id DESC LIMIT 1;")
+        last_id = self.select(f"SELECT {self.id_column_name} FROM {self.name} ORDER BY {self.id_column_name} DESC LIMIT 1;")
 
         return last_id[0][0]
 
     def get_num_of_records(self):
         """
         Returns the number of records in table
         """
@@ -1508,22 +1511,22 @@
         query = "DROP TABLE " + self.name + ";"
         print(query)
         self.db1.execute(query)
 
     # @save_migration #TODO: Uncomment
     def create(self, foreign_keys=None):
         assert len(self.columns) == len(self.types)
-        assert self.columns[0] == "id"
+        assert self.columns[0] == self.id_column_name
         assert self.types[0].lower() == "int"
 
         column_type_pairs = list(zip(self.columns, self.types))[1:]
         fields = ", ".join(
             [f"{column} {type_.upper()}" for column, type_ in column_type_pairs]
         )
-        query = f"CREATE TABLE {self.name} (id INT UNSIGNED AUTO_INCREMENT PRIMARY KEY, {fields})"
+        query = f"CREATE TABLE {self.name} ({self.id_column_name} INT UNSIGNED AUTO_INCREMENT PRIMARY KEY, {fields})"
 
         print(query)
         try:
             self.db1.execute(query)
         except Exception as e:
             print("Table " + self.name + " already exists:", e)
             print("Check the specification of table columns and their types")
@@ -1603,15 +1606,15 @@
 
     def add_foreign_key(self, foreign_key):
         parent_id = foreign_key['parent_id']
         parent = foreign_key['parent']
         query = "ALTER TABLE " + self.name + " MODIFY " + parent_id + " INT UNSIGNED"
         print(query)
         self.db1.execute(query)
-        query = "ALTER TABLE " + self.name + " ADD FOREIGN KEY (" + parent_id + ") REFERENCES " + parent + "(id)"
+        query = "ALTER TABLE " + self.name + " ADD FOREIGN KEY (" + parent_id + ") REFERENCES " + parent + "("+self.id_column_name+")"
         print(query)
         self.db1.execute(query)
 
     @save_migration
     def add_column(self, column_name, column_type):
         assert len(column_name) > 1
         command = "ALTER TABLE " + self.name + " ADD COLUMN " + column_name + " " + column_type
```

### Comparing `dbhydra-1.1.0/dbhydra/tests/test_mongo.py` & `dbhydra-1.2.0/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.1.0/dbhydra/tests/test_sql.py` & `dbhydra-1.2.0/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.1.0/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.2.0/dbhydra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.1.0
+Version: 1.2.0
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.1.0/setup.py` & `dbhydra-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.1.0',
+    version='1.2.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

