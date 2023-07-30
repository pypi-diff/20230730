# Comparing `tmp/gs_sql-0.0.3.tar.gz` & `tmp/gs_sql-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_sql-0.0.3.tar", last modified: Sun Jul 30 18:34:11 2023, max compression
+gzip compressed data, was "gs_sql-0.0.4.tar", last modified: Sun Jul 30 19:20:57 2023, max compression
```

## Comparing `gs_sql-0.0.3.tar` & `gs_sql-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.176723 gs_sql-0.0.3/
--rw-rw-rw-   0        0        0     7152 2023-07-30 18:34:11.176723 gs_sql-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6121 2023-07-30 13:16:07.000000 gs_sql-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.000702 gs_sql-0.0.3/gs_sql/
--rw-rw-rw-   0        0        0     1830 2023-07-04 18:01:38.000000 gs_sql-0.0.3/gs_sql/BaseData.py
--rw-rw-rw-   0        0        0     1361 2023-07-03 13:07:41.000000 gs_sql-0.0.3/gs_sql/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.154785 gs_sql-0.0.3/gs_sql/Tests/
--rw-rw-rw-   0        0        0        0 2023-07-03 17:18:10.000000 gs_sql-0.0.3/gs_sql/Tests/__init__.py
--rw-rw-rw-   0        0        0     1180 2023-07-08 19:26:49.000000 gs_sql-0.0.3/gs_sql/Tests/unit_tests.py
--rw-rw-rw-   0        0        0       30 2023-07-22 19:34:22.000000 gs_sql-0.0.3/gs_sql/__init__.py
--rw-rw-rw-   0        0        0     1110 2023-07-03 13:48:24.000000 gs_sql-0.0.3/gs_sql/authorization.py
--rw-rw-rw-   0        0        0      115 2023-07-22 18:33:44.000000 gs_sql-0.0.3/gs_sql/configuration.py
--rw-rw-rw-   0        0        0     8370 2023-07-07 20:07:54.000000 gs_sql-0.0.3/gs_sql/data_difinition.py
--rw-rw-rw-   0        0        0     8274 2023-07-22 18:32:10.000000 gs_sql-0.0.3/gs_sql/data_manipulation.py
--rw-rw-rw-   0        0        0      554 2023-07-08 11:58:11.000000 gs_sql-0.0.3/gs_sql/dataclasses.py
-drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.170420 gs_sql-0.0.3/gs_sql/pandasql/
--rw-rw-rw-   0        0        0      417 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/sqldf.py
-drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.176226 gs_sql-0.0.3/gs_sql/pandasql/tests/
--rw-rw-rw-   0        0        0        0 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/tests/__init__.py
--rw-rw-rw-   0        0        0     7352 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/tests/test_pandasql.py
--rw-rw-rw-   0        0        0     1180 2023-06-26 12:20:53.000000 gs_sql-0.0.3/gs_sql/pandasql/tests/test_utils.py
--rw-rw-rw-   0        0        0     1243 2023-07-08 19:45:30.000000 gs_sql-0.0.3/gs_sql/sheetsql.py
--rw-rw-rw-   0        0        0     8404 2023-07-22 18:32:58.000000 gs_sql-0.0.3/gs_sql/sql_parser.py
-drwxrwxrwx   0        0        0        0 2023-07-30 18:34:11.119843 gs_sql-0.0.3/gs_sql.egg-info/
--rw-rw-rw-   0        0        0     7152 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 18:30:11.000000 gs_sql-0.0.3/gs_sql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-30 18:34:10.000000 gs_sql-0.0.3/gs_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 18:34:11.196792 gs_sql-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1371 2023-07-30 18:34:04.000000 gs_sql-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:20:57.603649 gs_sql-0.0.4/
+-rw-rw-rw-   0        0        0     7142 2023-07-30 19:20:57.604024 gs_sql-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6111 2023-07-30 19:12:12.000000 gs_sql-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 19:20:57.588026 gs_sql-0.0.4/gs_sql/
+-rw-rw-rw-   0        0        0     1830 2023-07-04 18:01:38.000000 gs_sql-0.0.4/gs_sql/BaseData.py
+-rw-rw-rw-   0        0        0     1361 2023-07-03 13:07:41.000000 gs_sql-0.0.4/gs_sql/Exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:20:57.601261 gs_sql-0.0.4/gs_sql/Tests/
+-rw-rw-rw-   0        0        0        0 2023-07-03 17:18:10.000000 gs_sql-0.0.4/gs_sql/Tests/__init__.py
+-rw-rw-rw-   0        0        0     1180 2023-07-30 19:00:42.000000 gs_sql-0.0.4/gs_sql/Tests/unit_tests.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 19:10:05.000000 gs_sql-0.0.4/gs_sql/__init__.py
+-rw-rw-rw-   0        0        0     1110 2023-07-03 13:48:24.000000 gs_sql-0.0.4/gs_sql/authorization.py
+-rw-rw-rw-   0        0        0      115 2023-07-22 18:33:44.000000 gs_sql-0.0.4/gs_sql/configuration.py
+-rw-rw-rw-   0        0        0     8370 2023-07-07 20:07:54.000000 gs_sql-0.0.4/gs_sql/data_difinition.py
+-rw-rw-rw-   0        0        0     8274 2023-07-22 18:32:10.000000 gs_sql-0.0.4/gs_sql/data_manipulation.py
+-rw-rw-rw-   0        0        0      554 2023-07-08 11:58:11.000000 gs_sql-0.0.4/gs_sql/dataclasses.py
+-rw-rw-rw-   0        0        0     1243 2023-07-30 19:00:42.000000 gs_sql-0.0.4/gs_sql/sheetsql.py
+-rw-rw-rw-   0        0        0     8310 2023-07-29 17:39:30.000000 gs_sql-0.0.4/gs_sql/sql_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:20:57.598070 gs_sql-0.0.4/gs_sql.egg-info/
+-rw-rw-rw-   0        0        0     7142 2023-07-30 19:20:57.000000 gs_sql-0.0.4/gs_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-30 19:20:57.000000 gs_sql-0.0.4/gs_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 19:20:57.000000 gs_sql-0.0.4/gs_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 19:20:57.000000 gs_sql-0.0.4/gs_sql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-30 19:20:57.000000 gs_sql-0.0.4/gs_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 19:20:57.605670 gs_sql-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-30 19:20:41.000000 gs_sql-0.0.4/setup.py
```

### Comparing `gs_sql-0.0.3/PKG-INFO` & `gs_sql-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs_sql
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ability to use SQL when working with GoogleSheetAPI
 Home-page: https://github.com/EvgeniBondarev/PyGoogleSheetAPI
 Download-URL: https://github.com/EvgeniBondarev/PyGoogleSheetAPI/archive/refs/heads/main.zip
 Author: EvgeniBondarev
 Author-email: bondareff7@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,43 +33,43 @@
 
 ```python
 pip install gs-sql
 ```
 
 Or from Github:
 ```python
-https://github.com/EvgeniBondarev/PyGoogleSheetAPI/archive/refs/heads/main.zip
+https://github.com/EvgeniBondarev/gs-sql/archive/refs/heads/main.zip
 ```
 
 ## Usage
 
 At the first login, a browser window will open for confirmation, and a token.pickle file will be created in the directory where your credentials.json file is located to interact with the API.
 
 ```python
-from gs_api.sheetsql import SheetsQL
+from gs_sql.sheetsql import SheetsQL
 
 gs = SheetsQL()
 
 gs.authorization("files//credentials.json")
 ```
 Afterwards, you can create a table/database in Google Sheets either using standard methods or through SQL queries.
 ```python
-from gs_api.dataclasses import GsDataBase
+from gs_sql.dataclasses import GsDataBase
 
 new_base = gs.execute("""CREATE DATABASE NewBase""")
 
 gs.connect(new_base) # or gs.connect(GsDataBase(id="1fB_1uqU8FklXAQdn9XG4QK3HG4l5U0_vvM3abQ3aiuE", name="NewBase"))
 ```
 Finally, you can now create your first table.
 ```python
 query = gs.execute("CREATE TABLE Users (id, name)")
 ```
 Final code.
 ```python
-from gs_api.sheetsql import SheetsQL
+from gs_sql.sheetsql import SheetsQL
 
 
 gs = SheetsQL()
 
 gs.authorization("files//credentials.json")
 
 new_base = gs.execute("""CREATE DATABASE NewBase""")
```

### Comparing `gs_sql-0.0.3/README.md` & `gs_sql-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 
 ```python
 pip install gs-sql
 ```
 
 Or from Github:
 ```python
-https://github.com/EvgeniBondarev/PyGoogleSheetAPI/archive/refs/heads/main.zip
+https://github.com/EvgeniBondarev/gs-sql/archive/refs/heads/main.zip
 ```
 
 ## Usage
 
 At the first login, a browser window will open for confirmation, and a token.pickle file will be created in the directory where your credentials.json file is located to interact with the API.
 
 ```python
-from gs_api.sheetsql import SheetsQL
+from gs_sql.sheetsql import SheetsQL
 
 gs = SheetsQL()
 
 gs.authorization("files//credentials.json")
 ```
 Afterwards, you can create a table/database in Google Sheets either using standard methods or through SQL queries.
 ```python
-from gs_api.dataclasses import GsDataBase
+from gs_sql.dataclasses import GsDataBase
 
 new_base = gs.execute("""CREATE DATABASE NewBase""")
 
 gs.connect(new_base) # or gs.connect(GsDataBase(id="1fB_1uqU8FklXAQdn9XG4QK3HG4l5U0_vvM3abQ3aiuE", name="NewBase"))
 ```
 Finally, you can now create your first table.
 ```python
 query = gs.execute("CREATE TABLE Users (id, name)")
 ```
 Final code.
 ```python
-from gs_api.sheetsql import SheetsQL
+from gs_sql.sheetsql import SheetsQL
 
 
 gs = SheetsQL()
 
 gs.authorization("files//credentials.json")
 
 new_base = gs.execute("""CREATE DATABASE NewBase""")
```

### Comparing `gs_sql-0.0.3/gs_sql/BaseData.py` & `gs_sql-0.0.4/gs_sql/BaseData.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.3/gs_sql/Exceptions.py` & `gs_sql-0.0.4/gs_sql/Exceptions.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.3/gs_sql/Tests/unit_tests.py` & `gs_sql-0.0.4/gs_sql/Tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase, main
 
-from gs_api.sheetsql import SheetsQL
-from gs_api.dataclasses import GsDataBase, ResponseType
+from gs_sql.sheetsql import SheetsQL
+from gs_sql.dataclasses import GsDataBase, ResponseType
 
 
 
 class SheetsQLTests(TestCase):
     def setUp(self):
         self.sheetsql = SheetsQL()
```

### Comparing `gs_sql-0.0.3/gs_sql/authorization.py` & `gs_sql-0.0.4/gs_sql/authorization.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.3/gs_sql/data_difinition.py` & `gs_sql-0.0.4/gs_sql/data_difinition.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.3/gs_sql/data_manipulation.py` & `gs_sql-0.0.4/gs_sql/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.3/gs_sql/dataclasses.py` & `gs_sql-0.0.4/gs_sql/dataclasses.py`

 * *Files identical despite different names*

### Comparing `gs_sql-0.0.3/gs_sql/sheetsql.py` & `gs_sql-0.0.4/gs_sql/sheetsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional, Tuple
 
 from .data_difinition import DataDefinition
 from .data_manipulation import DataManipulation
 from .sql_parser import SQLParser
 from .dataclasses import GsDataBase, Answer, ResponseType
-import gs_api.configuration as  configuration
+import gs_sql.configuration as  configuration
 
 
 class SheetsQL:
     def __init__(self):
         self.data_difinition = None
         self.data_manipulation = None
         self.sql_processor = None
```

### Comparing `gs_sql-0.0.3/gs_sql/sql_parser.py` & `gs_sql-0.0.4/gs_sql/sql_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,16 +88,14 @@
                     result = self.data_difinition.create_table(table_name, columns)
                     return result
 
                 except HttpError:
                     return None
 
 
-
-
         table_pattern = r'CREATE TABLE (\w+)'
         table_match = re.search(table_pattern, sql_query)
         if table_match:
             table_name = table_match.group(1)
 
             column_pattern = r'\((.*?)\)'
             column_match = re.search(column_pattern, sql_query)
@@ -115,17 +113,14 @@
         if table_match:
             base_name = table_match.group(1)
 
             result = self.data_difinition.create_database(base_name)
 
             return result
 
-
-
-
     def __execute_alert(self, sql_query):
         table_pattern = r'ALTER TABLE (\w+)'
         table_match = re.search(table_pattern, sql_query)
         if table_match:
             table_name = table_match.group(1)
 
             columns_pattern = r'ALTER COLUMN (.*?);'
@@ -179,16 +174,14 @@
         table_match = re.search(table_pattern, sql_query)
         if table_match:
             table_name = table_match.group(1)
             if re.search(r"\bINNER\s+JOIN\b", sql_query, re.IGNORECASE):
                 dependent_tables = re.findall(r"\bINNER\s+JOIN\s+(\w+)\b", sql_query, re.IGNORECASE)
 
                 if dependent_tables:
-                    print(table_name)
-                    print(dependent_tables)
                     result = self.data_manipulation.select_join_data(sql_query, table_name, dependent_tables)
                     return result
 
             else:
                 result = self.data_manipulation.select_data(table_name, sql_query)
                 return result
```

### Comparing `gs_sql-0.0.3/gs_sql.egg-info/PKG-INFO` & `gs_sql-0.0.4/gs_sql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-sql
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ability to use SQL when working with GoogleSheetAPI
 Home-page: https://github.com/EvgeniBondarev/PyGoogleSheetAPI
 Download-URL: https://github.com/EvgeniBondarev/PyGoogleSheetAPI/archive/refs/heads/main.zip
 Author: EvgeniBondarev
 Author-email: bondareff7@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,43 +33,43 @@
 
 ```python
 pip install gs-sql
 ```
 
 Or from Github:
 ```python
-https://github.com/EvgeniBondarev/PyGoogleSheetAPI/archive/refs/heads/main.zip
+https://github.com/EvgeniBondarev/gs-sql/archive/refs/heads/main.zip
 ```
 
 ## Usage
 
 At the first login, a browser window will open for confirmation, and a token.pickle file will be created in the directory where your credentials.json file is located to interact with the API.
 
 ```python
-from gs_api.sheetsql import SheetsQL
+from gs_sql.sheetsql import SheetsQL
 
 gs = SheetsQL()
 
 gs.authorization("files//credentials.json")
 ```
 Afterwards, you can create a table/database in Google Sheets either using standard methods or through SQL queries.
 ```python
-from gs_api.dataclasses import GsDataBase
+from gs_sql.dataclasses import GsDataBase
 
 new_base = gs.execute("""CREATE DATABASE NewBase""")
 
 gs.connect(new_base) # or gs.connect(GsDataBase(id="1fB_1uqU8FklXAQdn9XG4QK3HG4l5U0_vvM3abQ3aiuE", name="NewBase"))
 ```
 Finally, you can now create your first table.
 ```python
 query = gs.execute("CREATE TABLE Users (id, name)")
 ```
 Final code.
 ```python
-from gs_api.sheetsql import SheetsQL
+from gs_sql.sheetsql import SheetsQL
 
 
 gs = SheetsQL()
 
 gs.authorization("files//credentials.json")
 
 new_base = gs.execute("""CREATE DATABASE NewBase""")
```

### Comparing `gs_sql-0.0.3/setup.py` & `gs_sql-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from io import open
 from setuptools import setup
 
-version = '0.0.3'
+version = '0.0.4'
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(name='gs_sql',
       author='EvgeniBondarev',
       author_email='bondareff7@gmail.com',
```

