# Comparing `tmp/calfcv-0.0.3.tar.gz` & `tmp/calfcv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.0.3.tar", last modified: Sat Jul 29 01:59:55 2023, max compression
+gzip compressed data, was "calfcv-0.0.4.tar", last modified: Sat Jul 29 22:16:32 2023, max compression
```

## Comparing `calfcv-0.0.3.tar` & `calfcv-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.3/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.3/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2229 2023-07-29 01:59:55.887296 calfcv-0.0.3/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1601 2023-07-29 01:03:54.000000 calfcv-0.0.3/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.3/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.3/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8413 2023-07-28 22:24:41.000000 calfcv-0.0.3/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.3/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.3/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.3/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2229 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.3/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.3/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 01:59:55.887296 calfcv-0.0.3/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1775 2023-07-29 01:59:39.000000 calfcv-0.0.3/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.133685 calfcv-0.0.4/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.4/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.4/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4964 2023-07-29 22:16:32.133685 calfcv-0.0.4/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4336 2023-07-29 20:32:45.000000 calfcv-0.0.4/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.129685 calfcv-0.0.4/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.4/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.4/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.4/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.133685 calfcv-0.0.4/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.4/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.4/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.4/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 22:16:32.133685 calfcv-0.0.4/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4964 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.4/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 22:16:32.000000 calfcv-0.0.4/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.4/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 22:16:32.133685 calfcv-0.0.4/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 22:14:36.000000 calfcv-0.0.4/setup.py
```

### Comparing `calfcv-0.0.3/LICENSE` & `calfcv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.3/calfcv/calfcv.py` & `calfcv-0.0.4/calfcv/calfcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,17 +226,18 @@
             steps=[
                 ('scaler', StandardScaler()),
                 ('classifier', Calf())
             ]
         )
 
         # setting n_jobs somehow cause y_true to have one class.
-        # The error will look like a cv problem. Do not set n_jobs
-        # until resolved.  Setting n_jobs may require joblib.
-        # https://stackoverflow.com/a/52738830/12865125
+        # The error will look like a cv problem, but the "culprit is
+        # Python’s multiprocessing that does fork without exec"
+        # Do not set n_jobs in GridSearchCV until resolved.
+        # https://scikit-learn.org/stable/faq.html#id27
         self.model_ = GridSearchCV(
             estimator=self.pipeline_,
             param_grid={'classifier__grid': [self.grid]},
             scoring="roc_auc",
             verbose=self.verbose
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `calfcv-0.0.3/calfcv/tests/test_calfcv.py` & `calfcv-0.0.4/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.3/setup.py` & `calfcv-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 #! /usr/bin/env python
-"""A template for scikit-learn compatible packages."""
+""" The calfcv package setup file.
+
+To build and upload a new distribution
+1.  Update the version
+
+2. cd to calfcv and build the dist folder with
+python setup.py sdist bdist_wheel
+
+3. twine upload dist/*
+
+"""
 
 import codecs
 import os
 
 from setuptools import find_packages, setup
 
 # get __version__ from _version.py
@@ -16,15 +26,15 @@
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Carlson Research, LLC'
 MAINTAINER_EMAIL = 'hrolfrc@gmail.com'
 URL = ''
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/project-template'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
```

