# Comparing `tmp/refineryframe-0.0.6.tar.gz` & `tmp/refineryframe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.6.tar", last modified: Sat Jul 29 05:32:45 2023, max compression
+gzip compressed data, was "refineryframe-0.0.7.tar", last modified: Sun Jul 30 03:56:19 2023, max compression
```

## Comparing `refineryframe-0.0.6.tar` & `refineryframe-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-29 05:32:45.672330 refineryframe-0.0.6/
--rw-r--r--   0 insani_dei   (501) staff       (20)    18296 2023-07-29 05:32:45.671396 refineryframe-0.0.6/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)    17742 2023-07-29 05:32:44.000000 refineryframe-0.0.6/README.md
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-29 05:32:45.666977 refineryframe-0.0.6/refineryframe/
--rwx------   0 insani_dei   (501) staff       (20)      163 2023-07-29 04:12:03.000000 refineryframe-0.0.6/refineryframe/__init__.py
--rwx------   0 insani_dei   (501) staff       (20)    34997 2023-07-29 04:57:45.000000 refineryframe-0.0.6/refineryframe/detect_unexpected.py
--rwx------   0 insani_dei   (501) staff       (20)    12527 2023-07-29 04:51:08.000000 refineryframe-0.0.6/refineryframe/other.py
--rwx------   0 insani_dei   (501) staff       (20)    17883 2023-07-29 04:48:17.000000 refineryframe-0.0.6/refineryframe/refiner.py
--rwx------   0 insani_dei   (501) staff       (20)    17400 2023-07-29 05:03:20.000000 refineryframe-0.0.6/refineryframe/replace_unexpected.py
--rwx------   0 insani_dei   (501) staff       (20)    72796 2023-07-29 03:18:37.000000 refineryframe-0.0.6/refineryframe/tns.py
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-29 05:32:45.670695 refineryframe-0.0.6/refineryframe.egg-info/
--rw-r--r--   0 insani_dei   (501) staff       (20)    18296 2023-07-29 05:32:45.000000 refineryframe-0.0.6/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)      368 2023-07-29 05:32:45.000000 refineryframe-0.0.6/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-29 05:32:45.000000 refineryframe-0.0.6/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       37 2023-07-29 05:32:45.000000 refineryframe-0.0.6/refineryframe.egg-info/requires.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-29 05:32:45.000000 refineryframe-0.0.6/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-29 05:32:45.672456 refineryframe-0.0.6/setup.cfg
--rw-r--r--   0 insani_dei   (501) staff       (20)     1181 2023-07-29 05:32:45.000000 refineryframe-0.0.6/setup.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.193331 refineryframe-0.0.7/
+-rw-r--r--   0 insani_dei   (501) staff       (20)     1061 2023-07-30 03:56:18.000000 refineryframe-0.0.7/LICENSE
+-rw-r--r--   0 insani_dei   (501) staff       (20)    17444 2023-07-30 03:56:19.192803 refineryframe-0.0.7/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)    16711 2023-07-30 03:56:18.000000 refineryframe-0.0.7/README.md
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.186081 refineryframe-0.0.7/refineryframe/
+-rwx------   0 insani_dei   (501) staff       (20)      163 2023-07-29 04:12:03.000000 refineryframe-0.0.7/refineryframe/__init__.py
+-rwx------   0 insani_dei   (501) staff       (20)    34997 2023-07-29 04:57:45.000000 refineryframe-0.0.7/refineryframe/detect_unexpected.py
+-rwx------   0 insani_dei   (501) staff       (20)    12527 2023-07-29 04:51:08.000000 refineryframe-0.0.7/refineryframe/other.py
+-rwx------   0 insani_dei   (501) staff       (20)    17883 2023-07-30 03:02:21.000000 refineryframe-0.0.7/refineryframe/refiner.py
+-rwx------   0 insani_dei   (501) staff       (20)    17400 2023-07-29 05:03:20.000000 refineryframe-0.0.7/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.188563 refineryframe-0.0.7/refineryframe.egg-info/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    17444 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)      413 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       46 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       20 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-30 03:56:19.193477 refineryframe-0.0.7/setup.cfg
+-rw-r--r--   0 insani_dei   (501) staff       (20)     1401 2023-07-30 03:56:18.000000 refineryframe-0.0.7/setup.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.191469 refineryframe-0.0.7/tests/
+-rw-r--r--   0 insani_dei   (501) staff       (20)        0 2023-07-30 01:38:57.000000 refineryframe-0.0.7/tests/__init__.py
+-rw-r--r--   0 insani_dei   (501) staff       (20)     5509 2023-07-30 03:07:43.000000 refineryframe-0.0.7/tests/conftest.py
+-rw-r--r--   0 insani_dei   (501) staff       (20)     9530 2023-07-30 02:56:34.000000 refineryframe-0.0.7/tests/test_refiner.py
```

### Comparing `refineryframe-0.0.6/PKG-INFO` & `refineryframe-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-Metadata-Version: 2.1
-Name: refineryframe
-Version: 0.0.6
-Summary: Cleans data, best to be used as a part of initial preprocessor
-Author: Kyrylo Mordan
-Author-email: <parachute.repo@gmail.com>
-Keywords: python,data cleaning,safeguards
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
+[![Build status](https://github.com/Kiril-Mordan/refineryframe/workflows/Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/refineryframe)](https://pepy.tech/project/refineryframe)
+[![Version](https://img.shields.io/pypi/v/refineryframe)](https://pypi.org/project/refineryframe/)
+![](https://img.shields.io/github/license/Kiril-Mordan/refineryframe)
+
 
 
 # refineryframe
 
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
@@ -244,24 +235,48 @@
                    'NumericColumn3' : 'int64', 
                    'DateColumn' : 'datetime64[ns]', 
                    'DateColumn2' : 'datetime64[ns]', 
                    'DateColumn3' : 'datetime64[ns]', 
                    'CharColumn' : 'object'}
 ```
 
+#### Check independent conditions
+
+
+```python
+tns.check_missing_types()
+tns.check_missing_values()
+tns.check_inf_values()
+tns.check_col_names_types()
+tns.check_date_format()
+tns.check_duplicates()
+tns.check_numeric_range()
+```
+
+    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 1 : 20.00%
+    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
+    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
+
+
 ##### moulding types
 
 
 ```python
 tns.set_types(type_dict = types_dict_str)
 ```
 
 
 ```python
-tns.get_type_dict_from_dataframe()
+tns.get_type_dict_from_dataframe() 
 ```
 
 
 
 
     {'num_id': 'int64',
      'NumericColumn': 'float64',
@@ -271,39 +286,14 @@
      'DateColumn': 'datetime64[ns]',
      'DateColumn2': 'datetime64[ns]',
      'DateColumn3': 'datetime64[ns]',
      'CharColumn': 'object'}
 
 
 
-#### Check independent conditions
-
-
-```python
-tns.check_missing_types()
-tns.check_missing_values()
-tns.check_inf_values()
-tns.check_col_names_types()
-tns.check_date_format()
-tns.check_duplicates()
-tns.check_numeric_range()
-```
-
-    WARNING:Refiner:Column NumericColumn_exepted: (-999) : 1 : 20.00%
-    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
-    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
-    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
-    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
-
-
 #### Using the main function to detect unexpected values
 
 
 ```python
 tns.detect_unexpected_values(earliest_date = "1920-01-01",
                          latest_date = "DateColumn3")
 ```
@@ -367,113 +357,30 @@
     DEBUG:Refiner:** Usable values in the dataframe:  44.44%
     DEBUG:Refiner:** Uncorrected data quality score:  32.22%
     DEBUG:Refiner:** Corrected data quality score:  52.57%
 
 
 
 ```python
-tns.dataframe
+tns.dataframe.dtypes
 ```
 
 
 
 
-<div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
-<table border="1" class="dataframe">
-  <thead>
-    <tr style="text-align: right;">
-      <th></th>
-      <th>num_id</th>
-      <th>NumericColumn</th>
-      <th>NumericColumn_exepted</th>
-      <th>NumericColumn2</th>
-      <th>NumericColumn3</th>
-      <th>DateColumn</th>
-      <th>DateColumn2</th>
-      <th>DateColumn3</th>
-      <th>CharColumn</th>
-    </tr>
-  </thead>
-  <tbody>
-    <tr>
-      <th>0</th>
-      <td>1</td>
-      <td>1.0</td>
-      <td>1.0</td>
-      <td>-999.0</td>
-      <td>1</td>
-      <td>2022-01-01</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>fol</td>
-    </tr>
-    <tr>
-      <th>1</th>
-      <td>2</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>2</td>
-      <td>2022-01-02</td>
-      <td>2022-01-01</td>
-      <td>2022-01-01</td>
-      <td>missing</td>
-    </tr>
-    <tr>
-      <th>2</th>
-      <td>3</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>3</td>
-      <td>2022-01-03</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>missing</td>
-    </tr>
-    <tr>
-      <th>3</th>
-      <td>4</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>4</td>
-      <td>2022-01-04</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>not expected</td>
-    </tr>
-    <tr>
-      <th>4</th>
-      <td>5</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999</td>
-      <td>2022-01-05</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>missing</td>
-    </tr>
-  </tbody>
-</table>
-</div>
+    num_id                           object
+    NumericColumn                   float64
+    NumericColumn_exepted           float64
+    NumericColumn2                  float64
+    NumericColumn3                    int64
+    DateColumn               datetime64[ns]
+    DateColumn2              datetime64[ns]
+    DateColumn3              datetime64[ns]
+    CharColumn                       object
+    dtype: object
 
 
 
 #### Use complex targeted conditions
 
 
 ```python
```

### Comparing `refineryframe-0.0.6/README.md` & `refineryframe-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: refineryframe
+Version: 0.0.7
+Summary: Cleans data, best to be used as a part of initial preprocessor
+Author: Kyrylo Mordan
+Author-email: <parachute.repo@gmail.com>
+Keywords: python,data cleaning,safeguards
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Build status](https://github.com/Kiril-Mordan/refineryframe/workflows/Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/refineryframe)](https://pepy.tech/project/refineryframe)
+[![Version](https://img.shields.io/pypi/v/refineryframe)](https://pypi.org/project/refineryframe/)
+![](https://img.shields.io/github/license/Kiril-Mordan/refineryframe)
+
+
+
 # refineryframe
 
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
@@ -228,24 +255,48 @@
                    'NumericColumn3' : 'int64', 
                    'DateColumn' : 'datetime64[ns]', 
                    'DateColumn2' : 'datetime64[ns]', 
                    'DateColumn3' : 'datetime64[ns]', 
                    'CharColumn' : 'object'}
 ```
 
+#### Check independent conditions
+
+
+```python
+tns.check_missing_types()
+tns.check_missing_values()
+tns.check_inf_values()
+tns.check_col_names_types()
+tns.check_date_format()
+tns.check_duplicates()
+tns.check_numeric_range()
+```
+
+    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 1 : 20.00%
+    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
+    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
+
+
 ##### moulding types
 
 
 ```python
 tns.set_types(type_dict = types_dict_str)
 ```
 
 
 ```python
-tns.get_type_dict_from_dataframe()
+tns.get_type_dict_from_dataframe() 
 ```
 
 
 
 
     {'num_id': 'int64',
      'NumericColumn': 'float64',
@@ -255,39 +306,14 @@
      'DateColumn': 'datetime64[ns]',
      'DateColumn2': 'datetime64[ns]',
      'DateColumn3': 'datetime64[ns]',
      'CharColumn': 'object'}
 
 
 
-#### Check independent conditions
-
-
-```python
-tns.check_missing_types()
-tns.check_missing_values()
-tns.check_inf_values()
-tns.check_col_names_types()
-tns.check_date_format()
-tns.check_duplicates()
-tns.check_numeric_range()
-```
-
-    WARNING:Refiner:Column NumericColumn_exepted: (-999) : 1 : 20.00%
-    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
-    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
-    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
-    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
-
-
 #### Using the main function to detect unexpected values
 
 
 ```python
 tns.detect_unexpected_values(earliest_date = "1920-01-01",
                          latest_date = "DateColumn3")
 ```
@@ -351,113 +377,30 @@
     DEBUG:Refiner:** Usable values in the dataframe:  44.44%
     DEBUG:Refiner:** Uncorrected data quality score:  32.22%
     DEBUG:Refiner:** Corrected data quality score:  52.57%
 
 
 
 ```python
-tns.dataframe
+tns.dataframe.dtypes
 ```
 
 
 
 
-<div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
-<table border="1" class="dataframe">
-  <thead>
-    <tr style="text-align: right;">
-      <th></th>
-      <th>num_id</th>
-      <th>NumericColumn</th>
-      <th>NumericColumn_exepted</th>
-      <th>NumericColumn2</th>
-      <th>NumericColumn3</th>
-      <th>DateColumn</th>
-      <th>DateColumn2</th>
-      <th>DateColumn3</th>
-      <th>CharColumn</th>
-    </tr>
-  </thead>
-  <tbody>
-    <tr>
-      <th>0</th>
-      <td>1</td>
-      <td>1.0</td>
-      <td>1.0</td>
-      <td>-999.0</td>
-      <td>1</td>
-      <td>2022-01-01</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>fol</td>
-    </tr>
-    <tr>
-      <th>1</th>
-      <td>2</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>2</td>
-      <td>2022-01-02</td>
-      <td>2022-01-01</td>
-      <td>2022-01-01</td>
-      <td>missing</td>
-    </tr>
-    <tr>
-      <th>2</th>
-      <td>3</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>3</td>
-      <td>2022-01-03</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>missing</td>
-    </tr>
-    <tr>
-      <th>3</th>
-      <td>4</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>4</td>
-      <td>2022-01-04</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>not expected</td>
-    </tr>
-    <tr>
-      <th>4</th>
-      <td>5</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999</td>
-      <td>2022-01-05</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>missing</td>
-    </tr>
-  </tbody>
-</table>
-</div>
+    num_id                           object
+    NumericColumn                   float64
+    NumericColumn_exepted           float64
+    NumericColumn2                  float64
+    NumericColumn3                    int64
+    DateColumn               datetime64[ns]
+    DateColumn2              datetime64[ns]
+    DateColumn3              datetime64[ns]
+    CharColumn                       object
+    dtype: object
 
 
 
 #### Use complex targeted conditions
 
 
 ```python
```

### Comparing `refineryframe-0.0.6/refineryframe/detect_unexpected.py` & `refineryframe-0.0.7/refineryframe/detect_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.6/refineryframe/other.py` & `refineryframe-0.0.7/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.6/refineryframe/refiner.py` & `refineryframe-0.0.7/refineryframe/refiner.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.6/refineryframe/replace_unexpected.py` & `refineryframe-0.0.7/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.6/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.0.7/refineryframe.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Build status](https://github.com/Kiril-Mordan/refineryframe/workflows/Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/refineryframe)](https://pepy.tech/project/refineryframe)
+[![Version](https://img.shields.io/pypi/v/refineryframe)](https://pypi.org/project/refineryframe/)
+![](https://img.shields.io/github/license/Kiril-Mordan/refineryframe)
+
 
 
 # refineryframe
 
 <a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
 
@@ -244,24 +255,48 @@
                    'NumericColumn3' : 'int64', 
                    'DateColumn' : 'datetime64[ns]', 
                    'DateColumn2' : 'datetime64[ns]', 
                    'DateColumn3' : 'datetime64[ns]', 
                    'CharColumn' : 'object'}
 ```
 
+#### Check independent conditions
+
+
+```python
+tns.check_missing_types()
+tns.check_missing_values()
+tns.check_inf_values()
+tns.check_col_names_types()
+tns.check_date_format()
+tns.check_duplicates()
+tns.check_numeric_range()
+```
+
+    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 1 : 20.00%
+    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
+    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
+
+
 ##### moulding types
 
 
 ```python
 tns.set_types(type_dict = types_dict_str)
 ```
 
 
 ```python
-tns.get_type_dict_from_dataframe()
+tns.get_type_dict_from_dataframe() 
 ```
 
 
 
 
     {'num_id': 'int64',
      'NumericColumn': 'float64',
@@ -271,39 +306,14 @@
      'DateColumn': 'datetime64[ns]',
      'DateColumn2': 'datetime64[ns]',
      'DateColumn3': 'datetime64[ns]',
      'CharColumn': 'object'}
 
 
 
-#### Check independent conditions
-
-
-```python
-tns.check_missing_types()
-tns.check_missing_values()
-tns.check_inf_values()
-tns.check_col_names_types()
-tns.check_date_format()
-tns.check_duplicates()
-tns.check_numeric_range()
-```
-
-    WARNING:Refiner:Column NumericColumn_exepted: (-999) : 1 : 20.00%
-    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
-    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
-    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
-    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
-    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
-
-
 #### Using the main function to detect unexpected values
 
 
 ```python
 tns.detect_unexpected_values(earliest_date = "1920-01-01",
                          latest_date = "DateColumn3")
 ```
@@ -367,113 +377,30 @@
     DEBUG:Refiner:** Usable values in the dataframe:  44.44%
     DEBUG:Refiner:** Uncorrected data quality score:  32.22%
     DEBUG:Refiner:** Corrected data quality score:  52.57%
 
 
 
 ```python
-tns.dataframe
+tns.dataframe.dtypes
 ```
 
 
 
 
-<div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
-<table border="1" class="dataframe">
-  <thead>
-    <tr style="text-align: right;">
-      <th></th>
-      <th>num_id</th>
-      <th>NumericColumn</th>
-      <th>NumericColumn_exepted</th>
-      <th>NumericColumn2</th>
-      <th>NumericColumn3</th>
-      <th>DateColumn</th>
-      <th>DateColumn2</th>
-      <th>DateColumn3</th>
-      <th>CharColumn</th>
-    </tr>
-  </thead>
-  <tbody>
-    <tr>
-      <th>0</th>
-      <td>1</td>
-      <td>1.0</td>
-      <td>1.0</td>
-      <td>-999.0</td>
-      <td>1</td>
-      <td>2022-01-01</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>fol</td>
-    </tr>
-    <tr>
-      <th>1</th>
-      <td>2</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>2</td>
-      <td>2022-01-02</td>
-      <td>2022-01-01</td>
-      <td>2022-01-01</td>
-      <td>missing</td>
-    </tr>
-    <tr>
-      <th>2</th>
-      <td>3</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>3</td>
-      <td>2022-01-03</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>missing</td>
-    </tr>
-    <tr>
-      <th>3</th>
-      <td>4</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>4</td>
-      <td>2022-01-04</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>not expected</td>
-    </tr>
-    <tr>
-      <th>4</th>
-      <td>5</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999.0</td>
-      <td>-999</td>
-      <td>2022-01-05</td>
-      <td>1850-01-09</td>
-      <td>1850-01-09</td>
-      <td>missing</td>
-    </tr>
-  </tbody>
-</table>
-</div>
+    num_id                           object
+    NumericColumn                   float64
+    NumericColumn_exepted           float64
+    NumericColumn2                  float64
+    NumericColumn3                    int64
+    DateColumn               datetime64[ns]
+    DateColumn2              datetime64[ns]
+    DateColumn3              datetime64[ns]
+    CharColumn                       object
+    dtype: object
 
 
 
 #### Use complex targeted conditions
 
 
 ```python
```

### Comparing `refineryframe-0.0.6/setup.py` & `refineryframe-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,32 +3,43 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+base_packages = [
+    "attrs>=22.2.0",
+    "datetime",
+    "pandas",
+    "numpy",
+    "unidecode"
+]
+
+VERSION = '0.0.7'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     version=VERSION,
     author="Kyrylo Mordan",
     author_email="<parachute.repo@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['datetime','pandas','numpy','unidecode','attr'],
+    install_requires=base_packages,
     keywords=['python', 'data cleaning', 'safeguards'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: MIT License",
+        "Topic :: Scientific/Engineering",
     ]
 )
```

