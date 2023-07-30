# Comparing `tmp/pyepsilla-0.0.9.tar.gz` & `tmp/pyepsilla-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.9.tar", last modified: Sun Jul 30 04:35:11 2023, max compression
+gzip compressed data, was "pyepsilla-0.1.0.tar", last modified: Sun Jul 30 14:40:26 2023, max compression
```

## Comparing `pyepsilla-0.0.9.tar` & `pyepsilla-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/pyepsilla/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/simple_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/pyepsilla/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/vectordb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/pyepsilla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/pyepsilla/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/simple_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/pyepsilla/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/vectordb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/pyepsilla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/setup.py
```

### Comparing `pyepsilla-0.0.9/LICENSE` & `pyepsilla-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.9/README.md` & `pyepsilla-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.9/pyepsilla/simple_example.py` & `pyepsilla-0.1.0/pyepsilla/simple_example.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.9/pyepsilla/vectordb/client.py` & `pyepsilla-0.1.0/pyepsilla/vectordb/client.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.9/pyepsilla/vectordb/field.py` & `pyepsilla-0.1.0/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.9/setup.py` & `pyepsilla-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.9',
+    version= '0.1.0',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     long_description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
@@ -17,8 +17,8 @@
     install_requires=[
         'requests>=2.19.1'
     ],
     url='https://github.com/epsilla-cloud/pyepsilla',
     project_urls={
         'Source': 'https://github.com/epsilla-cloud/pyepsilla',
     },
-)
+)
```

