# Comparing `tmp/refineryframe-0.0.7.tar.gz` & `tmp/refineryframe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.7.tar", last modified: Sun Jul 30 03:56:19 2023, max compression
+gzip compressed data, was "refineryframe-0.0.8.tar", last modified: Sun Jul 30 04:31:19 2023, max compression
```

## Comparing `refineryframe-0.0.7.tar` & `refineryframe-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.193331 refineryframe-0.0.7/
--rw-r--r--   0 insani_dei   (501) staff       (20)     1061 2023-07-30 03:56:18.000000 refineryframe-0.0.7/LICENSE
--rw-r--r--   0 insani_dei   (501) staff       (20)    17444 2023-07-30 03:56:19.192803 refineryframe-0.0.7/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)    16711 2023-07-30 03:56:18.000000 refineryframe-0.0.7/README.md
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.186081 refineryframe-0.0.7/refineryframe/
--rwx------   0 insani_dei   (501) staff       (20)      163 2023-07-29 04:12:03.000000 refineryframe-0.0.7/refineryframe/__init__.py
--rwx------   0 insani_dei   (501) staff       (20)    34997 2023-07-29 04:57:45.000000 refineryframe-0.0.7/refineryframe/detect_unexpected.py
--rwx------   0 insani_dei   (501) staff       (20)    12527 2023-07-29 04:51:08.000000 refineryframe-0.0.7/refineryframe/other.py
--rwx------   0 insani_dei   (501) staff       (20)    17883 2023-07-30 03:02:21.000000 refineryframe-0.0.7/refineryframe/refiner.py
--rwx------   0 insani_dei   (501) staff       (20)    17400 2023-07-29 05:03:20.000000 refineryframe-0.0.7/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.188563 refineryframe-0.0.7/refineryframe.egg-info/
--rw-r--r--   0 insani_dei   (501) staff       (20)    17444 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)      413 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       46 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/requires.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       20 2023-07-30 03:56:19.000000 refineryframe-0.0.7/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-30 03:56:19.193477 refineryframe-0.0.7/setup.cfg
--rw-r--r--   0 insani_dei   (501) staff       (20)     1401 2023-07-30 03:56:18.000000 refineryframe-0.0.7/setup.py
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-30 03:56:19.191469 refineryframe-0.0.7/tests/
--rw-r--r--   0 insani_dei   (501) staff       (20)        0 2023-07-30 01:38:57.000000 refineryframe-0.0.7/tests/__init__.py
--rw-r--r--   0 insani_dei   (501) staff       (20)     5509 2023-07-30 03:07:43.000000 refineryframe-0.0.7/tests/conftest.py
--rw-r--r--   0 insani_dei   (501) staff       (20)     9530 2023-07-30 02:56:34.000000 refineryframe-0.0.7/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.072766 refineryframe-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 04:31:08.000000 refineryframe-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-30 04:31:19.072766 refineryframe-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-30 04:31:08.000000 refineryframe-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.068766 refineryframe-0.0.8/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34997 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17883 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17400 2023-07-30 04:31:08.000000 refineryframe-0.0.8/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.068766 refineryframe-0.0.8/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-30 04:31:19.000000 refineryframe-0.0.8/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 04:31:18.000000 refineryframe-0.0.8/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:31:19.072766 refineryframe-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-30 04:31:08.000000 refineryframe-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:19.072766 refineryframe-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:31:08.000000 refineryframe-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-30 04:31:08.000000 refineryframe-0.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-30 04:31:08.000000 refineryframe-0.0.8/tests/test_refiner.py
```

### Comparing `refineryframe-0.0.7/LICENSE` & `refineryframe-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/PKG-INFO` & `refineryframe-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Cleans data, best to be used as a part of initial preprocessor
+Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
+License: UNKNOWN
 Keywords: python,data cleaning,safeguards
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -630,7 +633,9 @@
 ```
 
     duv_score: 1.0
     ruv_score0: 0.8222
     ruv_score1: 0.8889
     ruv_score2: 0.9753
 
+
+
```

### Comparing `refineryframe-0.0.7/README.md` & `refineryframe-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/refineryframe/detect_unexpected.py` & `refineryframe-0.0.8/refineryframe/detect_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/refineryframe/other.py` & `refineryframe-0.0.8/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/refineryframe/refiner.py` & `refineryframe-0.0.8/refineryframe/refiner.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/refineryframe/replace_unexpected.py` & `refineryframe-0.0.8/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.0.8/refineryframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Cleans data, best to be used as a part of initial preprocessor
+Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
+License: UNKNOWN
 Keywords: python,data cleaning,safeguards
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -630,7 +633,9 @@
 ```
 
     duv_score: 1.0
     ruv_score0: 0.8222
     ruv_score1: 0.8889
     ruv_score2: 0.9753
 
+
+
```

### Comparing `refineryframe-0.0.7/setup.py` & `refineryframe-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     version=VERSION,
```

### Comparing `refineryframe-0.0.7/tests/conftest.py` & `refineryframe-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.7/tests/test_refiner.py` & `refineryframe-0.0.8/tests/test_refiner.py`

 * *Files identical despite different names*

