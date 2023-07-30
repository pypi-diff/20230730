# Comparing `tmp/anakin-1.0.0.tar.gz` & `tmp/anakin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anakin-1.0.0.tar", last modified: Sun Jul 30 19:30:30 2023, max compression
+gzip compressed data, was "anakin-1.0.1.tar", last modified: Sun Jul 30 19:44:57 2023, max compression
```

## Comparing `anakin-1.0.0.tar` & `anakin-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-07-30 19:30:30.372247 anakin-1.0.0/
--rw-r--r--   0 developer   (501) staff       (20)      370 2023-07-30 19:30:30.371811 anakin-1.0.0/PKG-INFO
-drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-07-30 19:30:30.370550 anakin-1.0.0/anakin.egg-info/
--rw-r--r--   0 developer   (501) staff       (20)      370 2023-07-30 19:30:30.000000 anakin-1.0.0/anakin.egg-info/PKG-INFO
--rw-r--r--   0 developer   (501) staff       (20)      190 2023-07-30 19:30:30.000000 anakin-1.0.0/anakin.egg-info/SOURCES.txt
--rw-r--r--   0 developer   (501) staff       (20)        1 2023-07-30 19:30:30.000000 anakin-1.0.0/anakin.egg-info/dependency_links.txt
--rw-r--r--   0 developer   (501) staff       (20)       46 2023-07-30 19:30:30.000000 anakin-1.0.0/anakin.egg-info/entry_points.txt
--rw-r--r--   0 developer   (501) staff       (20)        9 2023-07-30 19:30:30.000000 anakin-1.0.0/anakin.egg-info/requires.txt
--rw-r--r--   0 developer   (501) staff       (20)        1 2023-07-30 19:30:30.000000 anakin-1.0.0/anakin.egg-info/top_level.txt
--rw-r--r--   0 developer   (501) staff       (20)       38 2023-07-30 19:30:30.372757 anakin-1.0.0/setup.cfg
--rw-r--r--   0 developer   (501) staff       (20)      702 2023-07-30 19:24:01.000000 anakin-1.0.0/setup.py
+drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-07-30 19:44:57.029047 anakin-1.0.1/
+-rw-r--r--   0 developer   (501) staff       (20)      370 2023-07-30 19:44:57.028235 anakin-1.0.1/PKG-INFO
+drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-07-30 19:44:57.027461 anakin-1.0.1/anakin.egg-info/
+-rw-r--r--   0 developer   (501) staff       (20)      370 2023-07-30 19:44:56.000000 anakin-1.0.1/anakin.egg-info/PKG-INFO
+-rw-r--r--   0 developer   (501) staff       (20)      190 2023-07-30 19:44:56.000000 anakin-1.0.1/anakin.egg-info/SOURCES.txt
+-rw-r--r--   0 developer   (501) staff       (20)        1 2023-07-30 19:44:56.000000 anakin-1.0.1/anakin.egg-info/dependency_links.txt
+-rw-r--r--   0 developer   (501) staff       (20)       39 2023-07-30 19:44:56.000000 anakin-1.0.1/anakin.egg-info/entry_points.txt
+-rw-r--r--   0 developer   (501) staff       (20)        9 2023-07-30 19:44:56.000000 anakin-1.0.1/anakin.egg-info/requires.txt
+-rw-r--r--   0 developer   (501) staff       (20)        1 2023-07-30 19:44:56.000000 anakin-1.0.1/anakin.egg-info/top_level.txt
+-rw-r--r--   0 developer   (501) staff       (20)       38 2023-07-30 19:44:57.029388 anakin-1.0.1/setup.cfg
+-rw-r--r--   0 developer   (501) staff       (20)      695 2023-07-30 19:43:50.000000 anakin-1.0.1/setup.py
```

### Comparing `anakin-1.0.0/setup.py` & `anakin-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anakin',
-    version='1.0.0',
+    version='1.0.1',
     description='Anakin Command Line Utility',
     long_description='Add a long description here if you want.',
     author='z10mx7',
     author_email='z10mx7@protonmail.com',
     url='https://github.com/z10mx7/anakin',   
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'anakin = anakin.anakin:main',
+            'anakin = anakin:main',
         ],
     },
     install_requires=[
         'colorama',  # Add any dependencies here
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
```

