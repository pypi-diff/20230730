# Comparing `tmp/refineryframe-0.0.8.tar.gz` & `tmp/refineryframe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.8.tar", last modified: Sun Jul 30 04:31:19 2023, max compression
+gzip compressed data, was "refineryframe-0.0.9.tar", last modified: Sun Jul 30 17:35:49 2023, max compression
```

## Comparing `refineryframe-0.0.8.tar` & `refineryframe-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.072766 refineryframe-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 04:31:08.000000 refineryframe-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-30 04:31:19.072766 refineryframe-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-30 04:31:08.000000 refineryframe-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.068766 refineryframe-0.0.8/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34997 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17883 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17400 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.068766 refineryframe-0.0.8/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-30 04:31:19.000000 refineryframe-0.0.8/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:31:19.072766 refineryframe-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-30 04:31:08.000000 refineryframe-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.072766 refineryframe-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:08.000000 refineryframe-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-30 04:31:08.000000 refineryframe-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-30 04:31:08.000000 refineryframe-0.0.8/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 17:35:36.000000 refineryframe-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-30 17:35:49.533758 refineryframe-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18622 2023-07-30 17:35:48.000000 refineryframe-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34997 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16129 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:35:49.533758 refineryframe-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 17:35:48.000000 refineryframe-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:36.000000 refineryframe-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-30 17:35:36.000000 refineryframe-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-30 17:35:36.000000 refineryframe-0.0.9/tests/test_refiner.py
```

### Comparing `refineryframe-0.0.8/LICENSE` & `refineryframe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.8/PKG-INFO` & `refineryframe-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-Metadata-Version: 2.1
-Name: refineryframe
-Version: 0.0.8
-Summary: Cleans data, best to be used as a part of initial preprocessor
-Home-page: UNKNOWN
-Author: Kyrylo Mordan
-Author-email: <parachute.repo@gmail.com>
-License: UNKNOWN
-Keywords: python,data cleaning,safeguards
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 [![Build status](https://github.com/Kiril-Mordan/refineryframe/workflows/Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/refineryframe)](https://pepy.tech/project/refineryframe)
 [![Version](https://img.shields.io/pypi/v/refineryframe)](https://pypi.org/project/refineryframe/)
 ![](https://img.shields.io/github/license/Kiril-Mordan/refineryframe)
+![](https://img.shields.io/pypi/pyversions/refineryframe)
 
 
 
-# refineryframe
-
-<a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
+# refineryframe
 
-Under construction! Not ready for use yet! Currently experimenting and planning!
+<a><img src="https://github.com/Kiril-Mordan/refineryframe/blob/main/images/logo.png" width="35%" height="35%" align="right" /></a>
 
-## Initial plans
 
-Goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
+The goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
 
 ## Installation
 
 Install `refineryframe` via pip with
 
 ```bash
 pip install refineryframe
 ```
 
 
+# Feature List
+
+- `refineryframe.refiner.Refiner.check_col_names_types` - checks if a given dataframe has the same column names as keys in a given dictionary
+and those columns have the same types as items in the dictionary.
+- `refineryframe.refiner.Refiner.check_date_format` - checks if the values in the datetime columns of the input dataframe
+have the expected 'YYYY-MM-DD' format.
+- `refineryframe.refiner.Refiner.check_date_range` - checks if dates are in expected ranges.
+- `refineryframe.refiner.Refiner.check_duplicates` - checks for duplicates in a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_inf_values` - counts the inf values in each column of a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_missing_types` - takes a DataFrame and a dictionary of missing types as input,
+and searches for any instances of these missing types in each column of the DataFrame.
+- `refineryframe.refiner.Refiner.check_missing_values` - counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_numeric_range` - checks if numeric values are in expected ranges.
+- `refineryframe.refiner.Refiner.detect_unexpected_values` - detects unexpected values in a pandas DataFrame.
+- `refineryframe.refiner.Refiner.get_type_dict_from_dataframe` - returns a dictionary or string representation of a dictionary containing the data types
+of each column in the given pandas DataFrame.
+- `refineryframe.refiner.Refiner.replace_unexpected_values` - replaces unexpected values in a pandas DataFrame with missing types.
+- `refineryframe.refiner.Refiner.set_type_dict` - changes the data types of the columns in the given DataFrame
+based on a dictionary of intended data types.
+- `refineryframe.refiner.Refiner.set_types` - changes the data types of the columns in the given DataFrame
+based on a dictionary of intended data types.
+
 ## Package usage example
 
 
 ```python
 import os 
 import sys 
 import numpy as np
@@ -633,9 +630,7 @@
 ```
 
     duv_score: 1.0
     ruv_score0: 0.8222
     ruv_score1: 0.8889
     ruv_score2: 0.9753
 
-
-
```

### Comparing `refineryframe-0.0.8/README.md` & `refineryframe-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,79 @@
+Metadata-Version: 2.1
+Name: refineryframe
+Version: 0.0.9
+Summary: Cleans data, best to be used as a part of initial preprocessor
+Home-page: UNKNOWN
+Author: Kyrylo Mordan
+Author-email: <parachute.repo@gmail.com>
+License: UNKNOWN
+Keywords: python,data cleaning,safeguards
+Platform: UNKNOWN
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
 [![Build status](https://github.com/Kiril-Mordan/refineryframe/workflows/Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/refineryframe)](https://pepy.tech/project/refineryframe)
 [![Version](https://img.shields.io/pypi/v/refineryframe)](https://pypi.org/project/refineryframe/)
 ![](https://img.shields.io/github/license/Kiril-Mordan/refineryframe)
+![](https://img.shields.io/pypi/pyversions/refineryframe)
 
 
 
-# refineryframe
-
-<a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
+# refineryframe
 
-Under construction! Not ready for use yet! Currently experimenting and planning!
+<a><img src="https://github.com/Kiril-Mordan/refineryframe/blob/main/images/logo.png" width="35%" height="35%" align="right" /></a>
 
-## Initial plans
 
-Goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
+The goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
 
 ## Installation
 
 Install `refineryframe` via pip with
 
 ```bash
 pip install refineryframe
 ```
 
 
+# Feature List
+
+- `refineryframe.refiner.Refiner.check_col_names_types` - checks if a given dataframe has the same column names as keys in a given dictionary
+and those columns have the same types as items in the dictionary.
+- `refineryframe.refiner.Refiner.check_date_format` - checks if the values in the datetime columns of the input dataframe
+have the expected 'YYYY-MM-DD' format.
+- `refineryframe.refiner.Refiner.check_date_range` - checks if dates are in expected ranges.
+- `refineryframe.refiner.Refiner.check_duplicates` - checks for duplicates in a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_inf_values` - counts the inf values in each column of a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_missing_types` - takes a DataFrame and a dictionary of missing types as input,
+and searches for any instances of these missing types in each column of the DataFrame.
+- `refineryframe.refiner.Refiner.check_missing_values` - counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_numeric_range` - checks if numeric values are in expected ranges.
+- `refineryframe.refiner.Refiner.detect_unexpected_values` - detects unexpected values in a pandas DataFrame.
+- `refineryframe.refiner.Refiner.get_type_dict_from_dataframe` - returns a dictionary or string representation of a dictionary containing the data types
+of each column in the given pandas DataFrame.
+- `refineryframe.refiner.Refiner.replace_unexpected_values` - replaces unexpected values in a pandas DataFrame with missing types.
+- `refineryframe.refiner.Refiner.set_type_dict` - changes the data types of the columns in the given DataFrame
+based on a dictionary of intended data types.
+- `refineryframe.refiner.Refiner.set_types` - changes the data types of the columns in the given DataFrame
+based on a dictionary of intended data types.
+
 ## Package usage example
 
 
 ```python
 import os 
 import sys 
 import numpy as np
@@ -610,7 +653,9 @@
 ```
 
     duv_score: 1.0
     ruv_score0: 0.8222
     ruv_score1: 0.8889
     ruv_score2: 0.9753
 
+
+
```

### Comparing `refineryframe-0.0.8/refineryframe/detect_unexpected.py` & `refineryframe-0.0.9/refineryframe/detect_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.8/refineryframe/other.py` & `refineryframe-0.0.9/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.8/refineryframe/refiner.py` & `refineryframe-0.0.9/refineryframe/refiner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,13 @@
 """
 refineryframe Module
 
 This module provides a Refiner class to encapsulate functions for data refinement
 and validation. The Refiner class is designed to work with pandas DataFrames and
 perform various checks and replacements for data preprocessing.
-
-Classes:
-    Refiner: A class that encapsulates functions for data refinement and validation.
-
-Functions:
-    shout(): Print a line of text with a specified length and format.
-    get_type_dict_from_dataframe(): Returns a string representation of a dictionary
-                                   containing the data types of each column in the given DataFrame.
-    set_type_dict(): Change the data types of the columns in the given DataFrame based on a dictionary of intended data types.
-    set_types(): Change the data types of the columns in the given DataFrame based on a dictionary of intended data types.
-    check_missing_types(): Search for missing types in each column of the DataFrame and log any instances found.
-    check_missing_values(): Count the number of NaN, None, and NaT values in each column of a pandas DataFrame.
-    check_inf_values(): Count the inf values in each column of a pandas DataFrame.
-    check_date_format(): Check if the values in the datetime columns of the input dataframe
-                            have the expected 'YYYY-MM-DD' format.
-    check_duplicates(): Check for duplicates in a pandas DataFrame.
-    check_col_names_types(): Check if a given dataframe has the same column names as keys in a given dictionary
-                                and those columns have the same types as items in the dictionary.
-    check_numeric_range(): Check if numeric values are in expected ranges.
-    check_date_range(): Check if dates are in expected ranges.
-    detect_unexpected_values(): Detect unexpected values in a pandas DataFrame.
-    replace_unexpected_values(): Replace unexpected values in a pandas DataFrame with missing types.
-
-Constants:
-    MISSING_TYPES: A dictionary containing default missing data types.
 """
 
 import logging
 import pandas as pd
 import attr
 from refineryframe.other import shoutOUT, get_type_dict, set_types
 from refineryframe.detect_unexpected import check_date_range, \
@@ -41,15 +16,15 @@
             check_missing_types, detect_unexpected_values
 from refineryframe.replace_unexpected import replace_unexpected_values
 
 @attr.s
 class Refiner:
 
     """
-    Refiner is a class that encapsulates funtions from refineframe.
+    Class that encapsulates funtions from refineryframe.
     """
 
 
     # inputs
     dataframe = attr.ib(type=pd.DataFrame)
     replace_dict = attr.ib(default=None, type=dict)
 
@@ -123,28 +98,28 @@
 
         self.logger = logger
 
 
     def shout(self):
 
         """
-        Print a line of text with a specified length and format.
+        Prints a line of text with a specified length and format.
         """
 
         shoutOUT(output_type=self.shout_type,
                  mess=self.mess,
                  dotline_length=self.dotline_length,
                  logger=self.logger)
 
     def get_type_dict_from_dataframe(self,
                       explicit=True,
                       stringout=False):
 
         """
-        Returns a string representation of a dictionary containing the data types
+        Returns a dictionary or string representation of a dictionary containing the data types
         of each column in the given pandas DataFrame.
 
         Numeric columns will have type 'numeric', date columns will have type 'date',
         character columns will have type 'category', and columns containing 'id' at
         the beginning or end of their name will have type 'index'.
         """
 
@@ -156,15 +131,15 @@
 
     def set_type_dict(self,
                       type_dict=None,
                       explicit=True,
                       stringout=False):
 
         """
-        Change the data types of the columns in the given DataFrame
+        Changes the data types of the columns in the given DataFrame
         based on a dictionary of intended data types.
         """
 
         if type_dict is None:
             type_dict = get_type_dict(dataframe=self.dataframe,
                                        explicit=explicit,
                                        stringout=stringout,
@@ -175,15 +150,15 @@
 
     def set_types(self,
                   type_dict=None,
                   replace_dict=None,
                   expected_date_format=None):
 
         """
-        Change the data types of the columns in the given DataFrame
+        Changes the data types of the columns in the given DataFrame
         based on a dictionary of intended data types.
         """
 
         if type_dict is None:
             type_dict = self.type_dict
         if replace_dict is None:
             replace_dict = self.replace_dict
@@ -195,61 +170,62 @@
                                   replace_dict=replace_dict,
                                   expected_date_format=expected_date_format,
                                       logger = self.logger)
 
     def check_missing_types(self):
 
         """
-        The function takes a DataFrame and a dictionary of missing types as input, and
-        searches for any instances of these missing types in each column of the DataFrame.
+        Takes a DataFrame and a dictionary of missing types as input,
+        and searches for any instances of these missing types in each column of the DataFrame.
+
         If any instances are found, a warning message is logged containing the column name,
         the missing value, and the count of missing values found.
         """
 
         self.MISSING_TYPES_TEST = check_missing_types(dataframe = self.dataframe,
                                                         MISSING_TYPES = self.MISSING_TYPES,
                                                         independent = True,
                                       logger = self.logger)
 
     def check_missing_values(self):
 
         """
-        Count the number of NaN, None, and NaT values in each column of a pandas DataFrame.
+        Counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
         """
 
         self.MISSING_COUNT_TEST = check_missing_values(dataframe = self.dataframe,
                                       logger = self.logger)
 
     def check_inf_values(self):
 
         """
-        Count the inf values in each column of a pandas DataFrame.
+        Counts the inf values in each column of a pandas DataFrame.
         """
 
         self.NUM_INF_TEST = check_inf_values(dataframe = self.dataframe,
                                              independent = True,
                                              logger = self.logger)
 
     def check_date_format(self):
 
         """
-        Check if the values in the datetime columns of the input dataframe
+        Checks if the values in the datetime columns of the input dataframe
         have the expected 'YYYY-MM-DD' format.
         """
 
         self.DATE_FORMAT_TEST = check_date_format(dataframe = self.dataframe,
                                                   expected_date_format = self.expected_date_format,
                                                   independent = True,
                                                   logger = self.logger)
 
     def check_duplicates(self,
                          subset = None):
 
         """
-        Check for duplicates in a pandas DataFrame.
+        Checks for duplicates in a pandas DataFrame.
         """
 
         self.DUPLICATES_TEST = check_duplicates(dataframe = self.dataframe,
                                                  subset = subset,
                                                  independent = True,
                                                  logger = self.logger)
 
@@ -268,15 +244,15 @@
     def check_numeric_range(self,
                             numeric_cols = None,
                             lower_bound = None,
                             upper_bound = None,
                             ignore_values = None):
 
         """
-        Check if numeric values are in expected ranges
+        Checks if numeric values are in expected ranges.
         """
 
         if lower_bound is None:
             lower_bound = self.lower_bound
         if upper_bound is None:
             upper_bound = self.upper_bound
         if ignore_values is None:
@@ -292,15 +268,15 @@
 
     def check_date_range(self,
                         earliest_date = None,
                         latest_date = None,
                         ignore_dates = None):
 
         """
-        Check if dates are in expected ranges
+        Checks if dates are in expected ranges.
         """
 
         if earliest_date is None:
             earliest_date = self.earliest_date
         if latest_date is None:
             latest_date = self.latest_date
         if ignore_dates is None:
@@ -324,15 +300,15 @@
                                  earliest_date = None,
                                  latest_date = None,
                                  numeric_lower_bound = None,
                                  numeric_upper_bound = None,
                                  print_score = True):
 
         """
-        Detect unexpected values in a pandas DataFrame.
+        Detects unexpected values in a pandas DataFrame.
         """
 
         if MISSING_TYPES is None:
             MISSING_TYPES = self.MISSING_TYPES
         if unexpected_exceptions is None:
             unexpected_exceptions = self.unexpected_exceptions_duv
         if unexpected_conditions is None:
@@ -372,15 +348,15 @@
                              TEST_RUV_FLAGS_PATH = None,
                              earliest_date = None,
                              latest_date = None,
                              numeric_lower_bound = None,
                              numeric_upper_bound = None):
 
         """
-        Replace unexpected values in a pandas DataFrame with missing types.
+        Replaces unexpected values in a pandas DataFrame with missing types.
         """
 
         if MISSING_TYPES is None:
             MISSING_TYPES = self.MISSING_TYPES
         if unexpected_exceptions is None:
             unexpected_exceptions = self.unexpected_exceptions_ruv
         if unexpected_conditions is None:
```

### Comparing `refineryframe-0.0.8/refineryframe/replace_unexpected.py` & `refineryframe-0.0.9/refineryframe/replace_unexpected.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,13 @@
 """
 replace_unexpected.py - Data Replacement Module
 
 This module contains a function to replace unexpected values in a pandas DataFrame with specified missing types.
 It covers various aspects of data validation, including replacing missing values, out-of-range numeric values,
 date values outside specified date ranges, and handling character-related issues such as capitalization and Unicode characters.
-
-Functions:
-1. replace_unexpected_values(dataframe, MISSING_TYPES=MISSING_TYPES,
-                             unexpected_exceptions={"irregular_values": "NONE",
-                                                   "date_range": "NONE",
-                                                   "numeric_range": "NONE",
-                                                   "capitalization": "NONE",
-                                                   "unicode_character": "NONE"},
-                             unexpected_conditions=None, TEST_RUV_FLAGS_PATH=None,
-                             earliest_date="1900-08-25", latest_date="2100-01-01",
-                             numeric_lower_bound=0, numeric_upper_bound=float("inf"),
-                             logger=logging) -> dict:
-    Replace unexpected values in a pandas DataFrame with specified missing types.
-    The function applies a series of data replacement checks, and the output includes
-    the data quality score before and after the replacement.
-
-Parameters:
------------
-- dataframe (pd.DataFrame): The DataFrame to be checked and processed.
-- MISSING_TYPES (dict): Dictionary that maps column names to the values considered as missing
-                        for that column. Default is set by the module-level variable MISSING_TYPES.
-- unexpected_exceptions (dict): Dictionary that lists column exceptions for each of the following checks:
-                                col_names_types, missing_values, missing_types, inf_values,
-                                date_format, duplicates, date_range, and numeric_range. Default is an empty dictionary.
-- unexpected_conditions (dict): Dictionary defining additional conditions to replace unexpected values.
-                                The dictionary includes keys 'set', 'description', 'group', 'features', and 'query'.
-                                Default is None.
-- TEST_RUV_FLAGS_PATH (str): Path for storing the corrected data quality score. Default is None.
-- earliest_date (str): The earliest acceptable date in the format 'YYYY-MM-DD'. Default is "1900-08-25".
-- latest_date (str): The latest acceptable date in the format 'YYYY-MM-DD'. Default is "2100-01-01".
-- numeric_lower_bound (float): The lowest acceptable value for numeric columns. Default is 0.
-- numeric_upper_bound (float): The highest acceptable value for numeric columns. Default is infinity.
-- logger (logging.Logger): Logger object to log messages. Default is the module-level logging object.
-
-Returns:
---------
-A dictionary containing the following keys:
-- 'dataframe': The DataFrame with replaced unexpected values.
-- 'ruv_score0': Data quality score before replacement, representing the percentage of usable values.
-- 'ruv_score1': Uncorrected data quality score after replacement, considering column and row medians.
-- 'ruv_score2': Corrected data quality score after replacement, considering column and row medians.
-
-Note:
-- The function replaces unexpected values with specified missing types based on the provided parameters.
-- Additional replacement conditions can be defined using the 'unexpected_conditions' parameter.
-- The function calculates data quality scores before and after replacement to assess data quality improvement.
-- If the 'TEST_RUV_FLAGS_PATH' parameter is provided, the corrected data quality score is saved to the specified path.
-
 """
 
 import logging
 from datetime import datetime
 import pandas as pd
 import numpy as np
 from unidecode import unidecode
```

### Comparing `refineryframe-0.0.8/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.0.9/refineryframe.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
@@ -21,39 +21,59 @@
 License-File: LICENSE
 
 
 [![Build status](https://github.com/Kiril-Mordan/refineryframe/workflows/Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/refineryframe)](https://pepy.tech/project/refineryframe)
 [![Version](https://img.shields.io/pypi/v/refineryframe)](https://pypi.org/project/refineryframe/)
 ![](https://img.shields.io/github/license/Kiril-Mordan/refineryframe)
+![](https://img.shields.io/pypi/pyversions/refineryframe)
 
 
 
-# refineryframe
-
-<a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
 
+# refineryframe
 
-Under construction! Not ready for use yet! Currently experimenting and planning!
+<a><img src="https://github.com/Kiril-Mordan/refineryframe/blob/main/images/logo.png" width="35%" height="35%" align="right" /></a>
 
-## Initial plans
 
-Goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
+The goal of the package is to simplify life for data scientists, that have to deal with imperfect raw data. The package suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
 
 ## Installation
 
 Install `refineryframe` via pip with
 
 ```bash
 pip install refineryframe
 ```
 
 
+# Feature List
+
+- `refineryframe.refiner.Refiner.check_col_names_types` - checks if a given dataframe has the same column names as keys in a given dictionary
+and those columns have the same types as items in the dictionary.
+- `refineryframe.refiner.Refiner.check_date_format` - checks if the values in the datetime columns of the input dataframe
+have the expected 'YYYY-MM-DD' format.
+- `refineryframe.refiner.Refiner.check_date_range` - checks if dates are in expected ranges.
+- `refineryframe.refiner.Refiner.check_duplicates` - checks for duplicates in a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_inf_values` - counts the inf values in each column of a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_missing_types` - takes a DataFrame and a dictionary of missing types as input,
+and searches for any instances of these missing types in each column of the DataFrame.
+- `refineryframe.refiner.Refiner.check_missing_values` - counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
+- `refineryframe.refiner.Refiner.check_numeric_range` - checks if numeric values are in expected ranges.
+- `refineryframe.refiner.Refiner.detect_unexpected_values` - detects unexpected values in a pandas DataFrame.
+- `refineryframe.refiner.Refiner.get_type_dict_from_dataframe` - returns a dictionary or string representation of a dictionary containing the data types
+of each column in the given pandas DataFrame.
+- `refineryframe.refiner.Refiner.replace_unexpected_values` - replaces unexpected values in a pandas DataFrame with missing types.
+- `refineryframe.refiner.Refiner.set_type_dict` - changes the data types of the columns in the given DataFrame
+based on a dictionary of intended data types.
+- `refineryframe.refiner.Refiner.set_types` - changes the data types of the columns in the given DataFrame
+based on a dictionary of intended data types.
+
 ## Package usage example
 
 
 ```python
 import os 
 import sys 
 import numpy as np
```

### Comparing `refineryframe-0.0.8/setup.py` & `refineryframe-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,22 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
+    #use_scm_version=True,
     version=VERSION,
     author="Kyrylo Mordan",
     author_email="<parachute.repo@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `refineryframe-0.0.8/tests/conftest.py` & `refineryframe-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.8/tests/test_refiner.py` & `refineryframe-0.0.9/tests/test_refiner.py`

 * *Files identical despite different names*

