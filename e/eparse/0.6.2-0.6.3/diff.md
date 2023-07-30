# Comparing `tmp/eparse-0.6.2.tar.gz` & `tmp/eparse-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.6.2.tar", last modified: Sun Jul  2 23:51:28 2023, max compression
+gzip compressed data, was "eparse-0.6.3.tar", last modified: Sun Jul 30 15:20:17 2023, max compression
```

## Comparing `eparse-0.6.2.tar` & `eparse-0.6.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.647887 eparse-0.6.2/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.2/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.2/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      681 2023-06-22 18:56:31.000000 eparse-0.6.2/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.2/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.2/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13150 2023-07-02 23:51:28.647887 eparse-0.6.2/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11620 2023-06-16 03:28:39.000000 eparse-0.6.2/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.637887 eparse-0.6.2/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.637887 eparse-0.6.2/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-07-02 23:50:14.000000 eparse-0.6.2/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.2/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5771 2023-07-02 23:45:12.000000 eparse-0.6.2/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.2/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.2/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.637887 eparse-0.6.2/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13150 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-07-02 23:51:28.647887 eparse-0.6.2/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1698 2023-07-02 23:49:16.000000 eparse-0.6.2/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.647887 eparse-0.6.2/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.2/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.2/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.2/tests/fixtures.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.2/tests/test.db
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.2/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-07-02 23:45:12.000000 eparse-0.6.2/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.2/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-30 15:20:17.055510 eparse-0.6.3/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.3/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.3/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      780 2023-07-30 15:18:52.000000 eparse-0.6.3/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.3/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.3/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13249 2023-07-30 15:20:17.055510 eparse-0.6.3/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11620 2023-06-16 03:28:39.000000 eparse-0.6.3/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-30 15:20:17.045510 eparse-0.6.3/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.3/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-30 15:20:17.045510 eparse-0.6.3/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-07-30 15:17:52.000000 eparse-0.6.3/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.3/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5754 2023-07-30 15:05:09.000000 eparse-0.6.3/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.3/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.3/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-30 15:20:17.055510 eparse-0.6.3/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13249 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-07-30 15:20:17.000000 eparse-0.6.3/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-07-30 15:20:17.055510 eparse-0.6.3/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1698 2023-07-30 15:17:43.000000 eparse-0.6.3/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-30 15:20:17.055510 eparse-0.6.3/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.3/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.3/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.3/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.3/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.3/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1443 2023-07-30 15:13:02.000000 eparse-0.6.3/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.3/tests/test_interfaces.py
```

### Comparing `eparse-0.6.2/CONTRIBUTING.rst` & `eparse-0.6.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/HISTORY.rst` & `eparse-0.6.3/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -41,7 +41,12 @@
 * Optimized database interfaces
 
 0.6.1 (2023-06-22)
 ==================
 
 * Added get_df_from_file helper function
 * Added contrib with unstructured partition handler
+
+0.6.3 (2023-06-22)
+==================
+
+* updated get_df_from_file to accept filename or io object
```

### Comparing `eparse-0.6.2/LICENSE` & `eparse-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/PKG-INFO` & `eparse-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.6.2
+Version: 0.6.3
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
@@ -417,7 +417,12 @@
 * Optimized database interfaces
 
 0.6.1 (2023-06-22)
 ==================
 
 * Added get_df_from_file helper function
 * Added contrib with unstructured partition handler
+
+0.6.3 (2023-06-22)
+==================
+
+* updated get_df_from_file to accept filename or io object
```

### Comparing `eparse-0.6.2/README.rst` & `eparse-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/docs/Makefile` & `eparse-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/docs/conf.py` & `eparse-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/docs/installation.rst` & `eparse-0.6.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/docs/make.bat` & `eparse-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/eparse/cli.py` & `eparse-0.6.3/eparse/cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/eparse/core.py` & `eparse-0.6.3/eparse/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -207,25 +207,25 @@
                 )
             )
 
     return result
 
 
 def get_df_from_file(
-    filename: str,
+    io,
     loose: bool = True,
     sheet: Iterable = [],
     table: str = None,
 ):
     '''
     helper function to yield tables from a file
     '''
 
     f = pd.read_excel(
-        filename,
+        io,
         sheet_name=list(sheet) or None,
         header=None,
         index_col=None,
     )
 
     # convert to dict if single sheet
     if type(f) is not dict:
```

### Comparing `eparse-0.6.2/eparse/interfaces.py` & `eparse-0.6.3/eparse/interfaces.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/eparse/migrations.py` & `eparse-0.6.3/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/eparse.egg-info/PKG-INFO` & `eparse-0.6.3/eparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.6.2
+Version: 0.6.3
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
@@ -417,7 +417,12 @@
 * Optimized database interfaces
 
 0.6.1 (2023-06-22)
 ==================
 
 * Added get_df_from_file helper function
 * Added contrib with unstructured partition handler
+
+0.6.3 (2023-06-22)
+==================
+
+* updated get_df_from_file to accept filename or io object
```

### Comparing `eparse-0.6.2/eparse.egg-info/SOURCES.txt` & `eparse-0.6.3/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/setup.py` & `eparse-0.6.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,10 +59,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.6.2',
+    version='0.6.3',
     zip_safe=False,
 )
```

### Comparing `eparse-0.6.2/tests/eparse_unit_test_data.xlsx` & `eparse-0.6.3/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/tests/fixtures.py` & `eparse-0.6.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/tests/test.db` & `eparse-0.6.3/tests/test.db`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/tests/test_cli.py` & `eparse-0.6.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.2/tests/test_core.py` & `eparse-0.6.3/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pandas as pd
 import pytest
 
 from eparse.core import (
     df_find_tables,
     df_parse_table,
     df_serialize_table,
+    get_df_from_file,
 )
 
 
 @pytest.fixture
 def xlsx():
     '''
     excel file fixture
@@ -48,7 +49,17 @@
 
 def test_df_serialize_table(xlsx):
     t = df_serialize_table(df_parse_table(xlsx, 102, 2), foo='bar')
     assert len(t) == 11 * 8
     assert isinstance(t[22], dict)
     assert 'c_header' in t[22].keys()
     assert t[22]['c_header'] == 'Date'
+
+
+def test_get_df_from_file():
+    filename = 'tests/eparse_unit_test_data.xlsx'
+    df_a, *_ = next(get_df_from_file(filename))
+    with open(filename, 'rb') as file:
+        df_b, *_ = next(get_df_from_file(file))
+    assert isinstance(df_a, pd.DataFrame)
+    assert isinstance(df_b, pd.DataFrame)
+    assert df_a.shape == df_b.shape
```

### Comparing `eparse-0.6.2/tests/test_interfaces.py` & `eparse-0.6.3/tests/test_interfaces.py`

 * *Files identical despite different names*

