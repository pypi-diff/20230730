# Comparing `tmp/calfcv-0.0.5.tar.gz` & `tmp/calfcv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.0.5.tar", last modified: Sat Jul 29 22:44:54 2023, max compression
+gzip compressed data, was "calfcv-0.0.6.tar", last modified: Sat Jul 29 22:49:30 2023, max compression
```

## Comparing `calfcv-0.0.5.tar` & `calfcv-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.5/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.5/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4844 2023-07-29 22:44:54.877823 calfcv-0.0.5/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4216 2023-07-29 22:44:22.000000 calfcv-0.0.5/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.5/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.5/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.5/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.5/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.5/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.5/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:44:54.877823 calfcv-0.0.5/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4844 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.5/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 22:44:54.000000 calfcv-0.0.5/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.5/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 22:44:54.881823 calfcv-0.0.5/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 22:34:53.000000 calfcv-0.0.5/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:49:30.718547 calfcv-0.0.6/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.6/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.6/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4839 2023-07-29 22:49:30.718547 calfcv-0.0.6/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4211 2023-07-29 22:47:39.000000 calfcv-0.0.6/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:49:30.718547 calfcv-0.0.6/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.6/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.6/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.6/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:49:30.718547 calfcv-0.0.6/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.6/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.6/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.6/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:49:30.718547 calfcv-0.0.6/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4839 2023-07-29 22:49:30.000000 calfcv-0.0.6/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 22:49:30.000000 calfcv-0.0.6/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 22:49:30.000000 calfcv-0.0.6/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.6/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 22:49:30.000000 calfcv-0.0.6/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 22:49:30.000000 calfcv-0.0.6/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.6/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 22:49:30.718547 calfcv-0.0.6/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 22:48:18.000000 calfcv-0.0.6/setup.py
```

### Comparing `calfcv-0.0.5/LICENSE` & `calfcv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.5/PKG-INFO` & `calfcv-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.5
+Version: 0.0.6
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -165,15 +165,15 @@
 
 .. parsed-literal::
 
     1.0
 
 
 
-Score using classes is lower than score than using probabilities
+Score using classes is lower than score using probabilities
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The ground truth is on the top and the predicted class is on the bottom. Sample 6 of y_test is predicted incorrectly but the others are correct.
 
 .. code:: ipython2
 
     y_pred = cls.predict(X_test)
```

### Comparing `calfcv-0.0.5/README.rst` & `calfcv-0.0.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 .. parsed-literal::
 
     1.0
 
 
 
-Score using classes is lower than score than using probabilities
+Score using classes is lower than score using probabilities
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The ground truth is on the top and the predicted class is on the bottom. Sample 6 of y_test is predicted incorrectly but the others are correct.
 
 .. code:: ipython2
 
     y_pred = cls.predict(X_test)
```

### Comparing `calfcv-0.0.5/calfcv/calfcv.py` & `calfcv-0.0.6/calfcv/calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.5/calfcv/tests/test_calfcv.py` & `calfcv-0.0.6/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.5/calfcv.egg-info/PKG-INFO` & `calfcv-0.0.6/calfcv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.5
+Version: 0.0.6
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -165,15 +165,15 @@
 
 .. parsed-literal::
 
     1.0
 
 
 
-Score using classes is lower than score than using probabilities
+Score using classes is lower than score using probabilities
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The ground truth is on the top and the predicted class is on the bottom. Sample 6 of y_test is predicted incorrectly but the others are correct.
 
 .. code:: ipython2
 
     y_pred = cls.predict(X_test)
```

### Comparing `calfcv-0.0.5/setup.py` & `calfcv-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Carlson Research, LLC'
 MAINTAINER_EMAIL = 'hrolfrc@gmail.com'
 URL = ''
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/project-template'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
```

