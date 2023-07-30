# Comparing `tmp/DdlGeneric-1.0.2.tar.gz` & `tmp/DdlGeneric-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DdlGeneric-1.0.2.tar", last modified: Sun Jul 30 01:31:28 2023, max compression
+gzip compressed data, was "DdlGeneric-1.0.3.tar", last modified: Sun Jul 30 01:41:55 2023, max compression
```

## Comparing `DdlGeneric-1.0.2.tar` & `DdlGeneric-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:31:28.637623 DdlGeneric-1.0.2/
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:31:28.633168 DdlGeneric-1.0.2/DdlGeneric.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)      955 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      282 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       51 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/top_level.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneric-1.0.2/LICENSE
--rw-r--r--   0 caowenpeng   (501) staff       (20)      955 2023-07-30 01:31:28.637300 DdlGeneric-1.0.2/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:31:28.635956 DdlGeneric-1.0.2/ddl2pojo/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneric-1.0.2/ddl2pojo/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneric-1.0.2/ddl2pojo/ddl2pojo.tpl
--rw-r--r--   0 caowenpeng   (501) staff       (20)     3119 2023-07-29 14:13:06.000000 DdlGeneric-1.0.2/ddl2pojo/main.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-07-30 01:31:28.637842 DdlGeneric-1.0.2/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      830 2023-07-30 01:30:15.000000 DdlGeneric-1.0.2/setup.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:41:55.651569 DdlGeneric-1.0.3/
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:41:55.648398 DdlGeneric-1.0.3/DdlGeneric.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      863 2023-07-30 01:41:55.000000 DdlGeneric-1.0.3/DdlGeneric.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      282 2023-07-30 01:41:55.000000 DdlGeneric-1.0.3/DdlGeneric.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-07-30 01:41:55.000000 DdlGeneric-1.0.3/DdlGeneric.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       51 2023-07-30 01:41:55.000000 DdlGeneric-1.0.3/DdlGeneric.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-30 01:41:55.000000 DdlGeneric-1.0.3/DdlGeneric.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-30 01:41:55.000000 DdlGeneric-1.0.3/DdlGeneric.egg-info/top_level.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneric-1.0.3/LICENSE
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      863 2023-07-30 01:41:55.651017 DdlGeneric-1.0.3/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:41:55.650120 DdlGeneric-1.0.3/ddl2pojo/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneric-1.0.3/ddl2pojo/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneric-1.0.3/ddl2pojo/ddl2pojo.tpl
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     3119 2023-07-29 14:13:06.000000 DdlGeneric-1.0.3/ddl2pojo/main.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-07-30 01:41:55.651919 DdlGeneric-1.0.3/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      830 2023-07-30 01:41:41.000000 DdlGeneric-1.0.3/setup.py
```

### Comparing `DdlGeneric-1.0.2/LICENSE` & `DdlGeneric-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DdlGeneric-1.0.2/ddl2pojo/main.py` & `DdlGeneric-1.0.3/ddl2pojo/main.py`

 * *Files identical despite different names*

### Comparing `DdlGeneric-1.0.2/setup.py` & `DdlGeneric-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 readmepath = 'README.md'
 setup(
     name='DdlGeneric',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'DdlGeneric = ddl2pojo.main:main'
         ]
     },
     install_requires=[
```

