# Comparing `tmp/hds-stats-0.3.6.tar.gz` & `tmp/hds-stats-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.6.tar", last modified: Sun Jul 30 00:49:20 2023, max compression
+gzip compressed data, was "hds-stats-0.3.7.tar", last modified: Sun Jul 30 00:56:23 2023, max compression
```

## Comparing `hds-stats-0.3.6.tar` & `hds-stats-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:49:20.055197 hds-stats-0.3.6/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.6/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-30 00:49:20.054938 hds-stats-0.3.6/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.6/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:49:20.052730 hds-stats-0.3.6/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.6/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.6/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.6/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27202 2023-07-30 00:48:16.000000 hds-stats-0.3.6/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:49:20.054499 hds-stats-0.3.6/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-30 00:49:20.000000 hds-stats-0.3.6/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-30 00:49:20.000000 hds-stats-0.3.6/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-30 00:49:20.000000 hds-stats-0.3.6/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-30 00:49:20.000000 hds-stats-0.3.6/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-30 00:49:20.000000 hds-stats-0.3.6/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.6/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-30 00:49:20.055293 hds-stats-0.3.6/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-30 00:48:27.000000 hds-stats-0.3.6/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:56:23.396137 hds-stats-0.3.7/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.7/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-30 00:56:23.395888 hds-stats-0.3.7/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.7/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:56:23.393886 hds-stats-0.3.7/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.7/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.7/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.7/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27257 2023-07-30 00:55:30.000000 hds-stats-0.3.7/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:56:23.395483 hds-stats-0.3.7/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.7/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-30 00:56:23.396231 hds-stats-0.3.7/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-30 00:55:46.000000 hds-stats-0.3.7/setup.py
```

### Comparing `hds-stats-0.3.6/LICENSE` & `hds-stats-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.6/PKG-INFO` & `hds-stats-0.3.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.6
+Version: 0.3.7
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.6/hds_stats/ml.py` & `hds-stats-0.3.7/hds_stats/ml.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.6/hds_stats/plot.py` & `hds-stats-0.3.7/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.6/hds_stats/stat.py` & `hds-stats-0.3.7/hds_stats/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,16 @@
     from sklearn.metrics import mean_squared_error
     from sklearn.metrics import mean_squared_log_error
     from sklearn.metrics import mean_absolute_error
     from sklearn.metrics import mean_absolute_percentage_error
     
     MSE = mean_squared_error(
         y_true = y_true, 
-        y_pred = y_pred
+        y_pred = y_pred, 
+        squared = True
     )
     
     RMSE = mean_squared_error(
         y_true = y_true, 
         y_pred = y_pred, 
         squared = False
     )
@@ -622,21 +623,22 @@
     
     if minus_count > 0:
         MSLE = None
         RMSLE = None
     else:
         MSLE = mean_squared_log_error(
             y_true = y_true, 
-            y_pred = y_pred
+            y_pred = y_pred, 
+            squared = True
         )
         
         RMSLE = mean_squared_log_error(
             y_true = y_true, 
             y_pred = y_pred, 
-            squared = True
+            squared = False
         )
     
     MAE = mean_absolute_error(
         y_true = y_true, 
         y_pred = y_pred
     )
```

### Comparing `hds-stats-0.3.6/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.7/hds_stats.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.6
+Version: 0.3.7
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.6/setup.py` & `hds-stats-0.3.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.6',
+    version = '0.3.7',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

