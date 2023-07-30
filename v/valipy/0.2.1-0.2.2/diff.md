# Comparing `tmp/valipy-0.2.1.tar.gz` & `tmp/valipy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valipy-0.2.1.tar", last modified: Sun Jul 30 09:18:31 2023, max compression
+gzip compressed data, was "valipy-0.2.2.tar", last modified: Sun Jul 30 09:21:07 2023, max compression
```

## Comparing `valipy-0.2.1.tar` & `valipy-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:18:31.385723 valipy-0.2.1/
--rw-r--r--   0 josevonchong   (501) staff       (20)     1440 2023-07-30 09:18:31.385823 valipy-0.2.1/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-30 09:18:31.386190 valipy-0.2.1/setup.cfg
--rw-r--r--   0 josevonchong   (501) staff       (20)     1311 2023-07-30 09:18:09.000000 valipy-0.2.1/setup.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:18:31.383641 valipy-0.2.1/test/
--rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.2.1/test/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      544 2023-07-30 08:51:40.000000 valipy-0.2.1/test/misc.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.2.1/test/test.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:18:31.384766 valipy-0.2.1/valipy/
--rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.2.1/valipy/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11818 2023-07-30 08:45:39.000000 valipy-0.2.1/valipy/exceptions.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11728 2023-07-30 08:35:33.000000 valipy-0.2.1/valipy/myFunctions.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:18:31.385587 valipy-0.2.1/valipy.egg-info/
--rw-r--r--   0 josevonchong   (501) staff       (20)     1440 2023-07-30 09:18:31.000000 valipy-0.2.1/valipy.egg-info/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)      243 2023-07-30 09:18:31.000000 valipy-0.2.1/valipy.egg-info/SOURCES.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-30 09:18:31.000000 valipy-0.2.1/valipy.egg-info/dependency_links.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-30 09:18:31.000000 valipy-0.2.1/valipy.egg-info/top_level.txt
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.478335 valipy-0.2.2/
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1463 2023-07-30 09:21:07.478452 valipy-0.2.2/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-30 09:21:07.478849 valipy-0.2.2/setup.cfg
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1311 2023-07-30 09:20:51.000000 valipy-0.2.2/setup.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.476366 valipy-0.2.2/test/
+-rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.2.2/test/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      544 2023-07-30 08:51:40.000000 valipy-0.2.2/test/misc.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.2.2/test/test.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.477352 valipy-0.2.2/valipy/
+-rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.2.2/valipy/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11818 2023-07-30 08:45:39.000000 valipy-0.2.2/valipy/exceptions.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11728 2023-07-30 08:35:33.000000 valipy-0.2.2/valipy/myFunctions.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.478175 valipy-0.2.2/valipy.egg-info/
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1463 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)      243 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/SOURCES.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/dependency_links.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/top_level.txt
```

### Comparing `valipy-0.2.1/PKG-INFO` & `valipy-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
 Keywords: validation,data,schema,schema validation
 Classifier: Development Status :: 4 - Beta
@@ -24,19 +24,20 @@
 ## Python Version Support
 
 Valipy currently only supports **python >3.11**. This is beacuse Valipy uses some features from the typing module only available for the newest python releases.
 
 ## Features
 
 1. Chainable API
-2. Plenty of validation rules  ())
+2. Plenty of validation rules  (20+)
 3. Create your own validation rules
 4. Reusable
 5. Can use Regex
 6. granular exceptions
+7. Schema Validation
 
 ## Instalation
 
 As easy as
 
 `pip install valipy`
```

### Comparing `valipy-0.2.1/setup.py` & `valipy-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 setup(
     name='valipy',
     packages=find_packages(),
-    version='0.2.1',
+    version='0.2.2',
     description='A chainable, fluent Python library for validating data',
     long_description_content_type='text/markdown',
     long_description=read_file('readme.md'),
 
     author='Joaquin Jose Von Chong',
     license='MIT',
     readme='readme.md',
```

### Comparing `valipy-0.2.1/test/misc.py` & `valipy-0.2.2/test/misc.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.1/valipy/exceptions.py` & `valipy-0.2.2/valipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.1/valipy/myFunctions.py` & `valipy-0.2.2/valipy/myFunctions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.1/valipy.egg-info/PKG-INFO` & `valipy-0.2.2/valipy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
 Keywords: validation,data,schema,schema validation
 Classifier: Development Status :: 4 - Beta
@@ -24,19 +24,20 @@
 ## Python Version Support
 
 Valipy currently only supports **python >3.11**. This is beacuse Valipy uses some features from the typing module only available for the newest python releases.
 
 ## Features
 
 1. Chainable API
-2. Plenty of validation rules  ())
+2. Plenty of validation rules  (20+)
 3. Create your own validation rules
 4. Reusable
 5. Can use Regex
 6. granular exceptions
+7. Schema Validation
 
 ## Instalation
 
 As easy as
 
 `pip install valipy`
```

