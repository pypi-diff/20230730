# Comparing `tmp/cohpy-1.1.2.tar.gz` & `tmp/cohpy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohpy-1.1.2.tar", max compression
+gzip compressed data, was "cohpy-1.1.3.tar", max compression
```

## Comparing `cohpy-1.1.2.tar` & `cohpy-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-04-03 15:10:15.179778 cohpy-1.1.2/LICENSE
--rw-r--r--   0        0        0     4725 2023-04-03 15:10:15.179778 cohpy-1.1.2/README.md
--rw-r--r--   0        0        0      542 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/__init__.py
--rw-r--r--   0        0        0     3755 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/client.py
--rw-r--r--   0        0        0      112 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/constants.py
--rw-r--r--   0        0        0     5437 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/endpoint.py
--rw-r--r--   0        0        0     1453 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/exceptions.py
--rw-r--r--   0        0        0      638 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/leaderboards.py
--rw-r--r--   0        0        0        0 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/tests/__init__.py
--rw-r--r--   0        0        0      856 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/tests/test_all_leaderboards.py
--rw-r--r--   0        0        0     3468 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/tests/test_personal_stat.py
--rw-r--r--   0        0        0     3276 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/tests/test_player_match_history.py
--rw-r--r--   0        0        0     3076 2023-04-03 15:10:15.179778 cohpy-1.1.2/cohpy/tests/test_specific_leaderboard.py
--rw-r--r--   0        0        0      361 2023-04-03 15:10:15.179778 cohpy-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 cohpy-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-30 20:00:45.343585 cohpy-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4725 2023-07-30 20:00:45.343585 cohpy-1.1.3/README.md
+-rw-r--r--   0        0        0      542 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/client.py
+-rw-r--r--   0        0        0      112 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/constants.py
+-rw-r--r--   0        0        0     5437 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/endpoint.py
+-rw-r--r--   0        0        0     1453 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/exceptions.py
+-rw-r--r--   0        0        0      638 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/leaderboards.py
+-rw-r--r--   0        0        0        0 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/tests/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/tests/test_all_leaderboards.py
+-rw-r--r--   0        0        0     3468 2023-07-30 20:00:45.347585 cohpy-1.1.3/cohpy/tests/test_personal_stat.py
+-rw-r--r--   0        0        0     3276 2023-07-30 20:00:45.347585 cohpy-1.1.3/cohpy/tests/test_player_match_history.py
+-rw-r--r--   0        0        0     3076 2023-07-30 20:00:45.347585 cohpy-1.1.3/cohpy/tests/test_specific_leaderboard.py
+-rw-r--r--   0        0        0      361 2023-07-30 20:00:45.347585 cohpy-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 cohpy-1.1.3/PKG-INFO
```

### Comparing `cohpy-1.1.2/LICENSE` & `cohpy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/README.md` & `cohpy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/__init__.py` & `cohpy-1.1.3/cohpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/client.py` & `cohpy-1.1.3/cohpy/client.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/endpoint.py` & `cohpy-1.1.3/cohpy/endpoint.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/exceptions.py` & `cohpy-1.1.3/cohpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/leaderboards.py` & `cohpy-1.1.3/cohpy/leaderboards.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     UKF1v1 = 2130257
     GER1v1 = 2130261
     DAK1v1 = 2130259
 
     USF2v2 = 2130300
     UKF2v2 = 2130302
     GER2v2 = 2130306
-    DAK2v2 = 2130306
+    DAK2v2 = 2130304
 
     USF3v3 = 2130329
     UKF3v3 = 2130331
     GER3v3 = 2130335
-    DAK3v3 = 2130334
+    DAK3v3 = 2130333
 
     USF4v4 = 2130353
     UKF4v4 = 2130356
     GER4v4 = 2130360
     DAK4v4 = 2130358
```

### Comparing `cohpy-1.1.2/cohpy/tests/test_all_leaderboards.py` & `cohpy-1.1.3/cohpy/tests/test_all_leaderboards.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/tests/test_personal_stat.py` & `cohpy-1.1.3/cohpy/tests/test_personal_stat.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/tests/test_player_match_history.py` & `cohpy-1.1.3/cohpy/tests/test_player_match_history.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/cohpy/tests/test_specific_leaderboard.py` & `cohpy-1.1.3/cohpy/tests/test_specific_leaderboard.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.2/PKG-INFO` & `cohpy-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: Andres Garrido
 Author-email: andreslp0001@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cohpy Version: 1.1.2 Summary: Author: Andres
+Metadata-Version: 2.1 Name: cohpy Version: 1.1.3 Summary: Author: Andres
 Garrido Author-email: andreslp0001@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coverage (>=7.2.2,<8.0.0) Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: flake8-import-order (>=0.18.2,<0.19.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Description-Content-Type: text/markdown
 ****** COHPY ******
```

