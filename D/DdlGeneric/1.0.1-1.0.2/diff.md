# Comparing `tmp/DdlGeneric-1.0.1.tar.gz` & `tmp/DdlGeneric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DdlGeneric-1.0.1.tar", last modified: Sat Jul 29 15:11:09 2023, max compression
+gzip compressed data, was "DdlGeneric-1.0.2.tar", last modified: Sun Jul 30 01:31:28 2023, max compression
```

## Comparing `DdlGeneric-1.0.1.tar` & `DdlGeneric-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-29 15:11:09.906514 DdlGeneric-1.0.1/
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-29 15:11:09.901380 DdlGeneric-1.0.1/DdlGeneric.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)      424 2023-07-29 15:11:09.000000 DdlGeneric-1.0.1/DdlGeneric.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      282 2023-07-29 15:11:09.000000 DdlGeneric-1.0.1/DdlGeneric.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-07-29 15:11:09.000000 DdlGeneric-1.0.1/DdlGeneric.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       51 2023-07-29 15:11:09.000000 DdlGeneric-1.0.1/DdlGeneric.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-29 15:11:09.000000 DdlGeneric-1.0.1/DdlGeneric.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-29 15:11:09.000000 DdlGeneric-1.0.1/DdlGeneric.egg-info/top_level.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneric-1.0.1/LICENSE
--rw-r--r--   0 caowenpeng   (501) staff       (20)      424 2023-07-29 15:11:09.905958 DdlGeneric-1.0.1/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-29 15:11:09.904330 DdlGeneric-1.0.1/ddl2pojo/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneric-1.0.1/ddl2pojo/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneric-1.0.1/ddl2pojo/ddl2pojo.tpl
--rw-r--r--   0 caowenpeng   (501) staff       (20)     3119 2023-07-29 14:13:06.000000 DdlGeneric-1.0.1/ddl2pojo/main.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-07-29 15:11:09.906742 DdlGeneric-1.0.1/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      690 2023-07-29 15:10:32.000000 DdlGeneric-1.0.1/setup.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:31:28.637623 DdlGeneric-1.0.2/
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:31:28.633168 DdlGeneric-1.0.2/DdlGeneric.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      955 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      282 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       51 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-07-30 01:31:28.000000 DdlGeneric-1.0.2/DdlGeneric.egg-info/top_level.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneric-1.0.2/LICENSE
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      955 2023-07-30 01:31:28.637300 DdlGeneric-1.0.2/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-07-30 01:31:28.635956 DdlGeneric-1.0.2/ddl2pojo/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneric-1.0.2/ddl2pojo/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneric-1.0.2/ddl2pojo/ddl2pojo.tpl
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     3119 2023-07-29 14:13:06.000000 DdlGeneric-1.0.2/ddl2pojo/main.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-07-30 01:31:28.637842 DdlGeneric-1.0.2/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      830 2023-07-30 01:30:15.000000 DdlGeneric-1.0.2/setup.py
```

### Comparing `DdlGeneric-1.0.1/LICENSE` & `DdlGeneric-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DdlGeneric-1.0.1/ddl2pojo/main.py` & `DdlGeneric-1.0.2/ddl2pojo/main.py`

 * *Files identical despite different names*

### Comparing `DdlGeneric-1.0.1/setup.py` & `DdlGeneric-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import setup, find_packages
 
+readmepath = 'README.md'
 setup(
     name='DdlGeneric',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'DdlGeneric = ddl2pojo.main:main'
         ]
     },
     install_requires=[
         'argparse'
     ],
     author='visonforcoding',
     author_email='visonforcoding@gmail.com',
     description='DDL文件解析程序',
+    long_description=open(readmepath, encoding='utf-8').read(),
+    long_description_content_type='text/markdown',
     url='https://gitee.com/visonforcoding/code-template-tools',
     package_data={
         "": ["ddl2pojo.tpl"],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

