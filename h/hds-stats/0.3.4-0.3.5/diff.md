# Comparing `tmp/hds-stats-0.3.4.tar.gz` & `tmp/hds-stats-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.4.tar", last modified: Mon Jul 10 06:51:08 2023, max compression
+gzip compressed data, was "hds-stats-0.3.5.tar", last modified: Sat Jul 29 08:50:20 2023, max compression
```

## Comparing `hds-stats-0.3.4.tar` & `hds-stats-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:51:08.892924 hds-stats-0.3.4/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.4/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:51:08.892676 hds-stats-0.3.4/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.4/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:51:08.890733 hds-stats-0.3.4/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.4/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.4/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.4/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27181 2023-07-10 06:46:42.000000 hds-stats-0.3.4/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:51:08.892312 hds-stats-0.3.4/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.4/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:51:08.893016 hds-stats-0.3.4/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:50:53.000000 hds-stats-0.3.4/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-29 08:50:20.352482 hds-stats-0.3.5/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.5/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-29 08:50:20.352244 hds-stats-0.3.5/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.5/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-29 08:50:20.350298 hds-stats-0.3.5/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.5/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.5/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.5/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27182 2023-07-29 08:47:56.000000 hds-stats-0.3.5/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-29 08:50:20.351863 hds-stats-0.3.5/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-29 08:50:20.000000 hds-stats-0.3.5/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-29 08:50:20.000000 hds-stats-0.3.5/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-29 08:50:20.000000 hds-stats-0.3.5/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-29 08:50:20.000000 hds-stats-0.3.5/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-29 08:50:20.000000 hds-stats-0.3.5/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.5/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-29 08:50:20.352582 hds-stats-0.3.5/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-29 08:48:16.000000 hds-stats-0.3.5/setup.py
```

### Comparing `hds-stats-0.3.4/LICENSE` & `hds-stats-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.4/PKG-INFO` & `hds-stats-0.3.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.4
+Version: 0.3.5
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.4/hds_stats/ml.py` & `hds-stats-0.3.5/hds_stats/ml.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.4/hds_stats/plot.py` & `hds-stats-0.3.5/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.4/hds_stats/stat.py` & `hds-stats-0.3.5/hds_stats/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,15 @@
         y_true = y_true, 
         y_pred = y_pred
     )
     
     RMSE = mean_squared_error(
         y_true = y_true, 
         y_pred = y_pred, 
-        squared = True
+        squared = False
     )
     
     minus_count = pd.Series(data = y_pred).lt(0).sum()
     
     if minus_count > 0:
         MSLE = None
         RMSLE = None
```

### Comparing `hds-stats-0.3.4/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.5/hds_stats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.4
+Version: 0.3.5
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.4/setup.py` & `hds-stats-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.4',
+    version = '0.3.5',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

