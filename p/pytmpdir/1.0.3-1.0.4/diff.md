# Comparing `tmp/pytmpdir-1.0.3.tar.gz` & `tmp/pytmpdir-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmpdir-1.0.3.tar", last modified: Sat Feb 12 08:34:31 2022, max compression
+gzip compressed data, was "pytmpdir-1.0.4.tar", last modified: Sun Jul 30 12:44:37 2023, max compression
```

## Comparing `pytmpdir-1.0.3.tar` & `pytmpdir-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2022-02-12 08:34:31.394041 pytmpdir-1.0.3/
--rw-r--r--   0 jchesney   (501) staff       (20)      471 2022-02-12 08:34:31.394216 pytmpdir-1.0.3/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)      816 2021-09-22 06:19:18.000000 pytmpdir-1.0.3/README.rst
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2022-02-12 08:34:31.386530 pytmpdir-1.0.3/pytmpdir/
--rw-r--r--   0 jchesney   (501) staff       (20)      102 2022-02-12 08:34:25.000000 pytmpdir-1.0.3/pytmpdir/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)      139 2022-01-10 23:14:45.000000 pytmpdir-1.0.3/pytmpdir/dir_setting.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9027 2022-01-12 14:13:50.000000 pytmpdir-1.0.3/pytmpdir/directory_.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4034 2022-01-12 14:15:13.000000 pytmpdir-1.0.3/pytmpdir/directory_test.py
--rw-r--r--   0 jchesney   (501) staff       (20)     8335 2022-02-12 08:23:56.000000 pytmpdir-1.0.3/pytmpdir/file_.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2286 2022-01-10 23:27:28.000000 pytmpdir-1.0.3/pytmpdir/named_temp_file_reader.py
--rw-r--r--   0 jchesney   (501) staff       (20)      259 2022-01-10 23:14:45.000000 pytmpdir-1.0.3/pytmpdir/pytmpdir_exception.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3037 2022-01-12 13:04:58.000000 pytmpdir-1.0.3/pytmpdir/spooled_named_temporary_file.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2022-02-12 08:34:31.393472 pytmpdir-1.0.3/pytmpdir.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      471 2022-02-12 08:34:30.000000 pytmpdir-1.0.3/pytmpdir.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)      408 2022-02-12 08:34:30.000000 pytmpdir-1.0.3/pytmpdir.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2022-02-12 08:34:30.000000 pytmpdir-1.0.3/pytmpdir.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       26 2022-02-12 08:34:30.000000 pytmpdir-1.0.3/pytmpdir.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        9 2022-02-12 08:34:30.000000 pytmpdir-1.0.3/pytmpdir.egg-info/top_level.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       80 2022-02-12 08:34:31.396084 pytmpdir-1.0.3/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)      799 2022-02-12 08:34:25.000000 pytmpdir-1.0.3/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-07-30 12:44:37.460578 pytmpdir-1.0.4/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1068 2021-09-22 06:19:18.000000 pytmpdir-1.0.4/LICENSE.rst
+-rw-r--r--   0 jchesney   (501) staff       (20)      441 2023-07-30 12:44:37.460737 pytmpdir-1.0.4/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)      816 2021-09-22 06:19:18.000000 pytmpdir-1.0.4/README.rst
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-07-30 12:44:37.458723 pytmpdir-1.0.4/pytmpdir/
+-rw-r--r--   0 jchesney   (501) staff       (20)      102 2023-07-30 12:44:34.000000 pytmpdir-1.0.4/pytmpdir/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      222 2023-07-30 12:38:57.000000 pytmpdir-1.0.4/pytmpdir/dir_setting.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     9026 2022-02-12 23:54:48.000000 pytmpdir-1.0.4/pytmpdir/directory_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4034 2022-01-12 14:15:13.000000 pytmpdir-1.0.4/pytmpdir/directory_test.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8335 2022-02-12 08:23:56.000000 pytmpdir-1.0.4/pytmpdir/file_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2286 2022-01-10 23:27:28.000000 pytmpdir-1.0.4/pytmpdir/named_temp_file_reader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      259 2022-01-10 23:14:45.000000 pytmpdir-1.0.4/pytmpdir/pytmpdir_exception.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3037 2022-01-12 13:04:58.000000 pytmpdir-1.0.4/pytmpdir/spooled_named_temporary_file.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-07-30 12:44:37.460308 pytmpdir-1.0.4/pytmpdir.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      441 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)      420 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       26 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        9 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/top_level.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       80 2023-07-30 12:44:37.461374 pytmpdir-1.0.4/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)      799 2023-07-30 12:44:34.000000 pytmpdir-1.0.4/setup.py
```

### Comparing `pytmpdir-1.0.3/README.rst` & `pytmpdir-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.3/pytmpdir/directory_.py` & `pytmpdir-1.0.4/pytmpdir/directory_.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     Functions as a directory object to extract, archive and pass around code.
     Auto deletes when the directory falls out of scope.
     """
 
     def __init__(
         self,
-        initWithDir: bool = None,
+        initWithDir: str = None,
         autoDelete: bool = True,
         inDir: str = None,
     ):
         """Directory Initialise
 
         Creates a temporary directory if the directory doesn't exist.
```

### Comparing `pytmpdir-1.0.3/pytmpdir/directory_test.py` & `pytmpdir-1.0.4/pytmpdir/directory_test.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.3/pytmpdir/file_.py` & `pytmpdir-1.0.4/pytmpdir/file_.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.3/pytmpdir/named_temp_file_reader.py` & `pytmpdir-1.0.4/pytmpdir/named_temp_file_reader.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.3/pytmpdir/spooled_named_temporary_file.py` & `pytmpdir-1.0.4/pytmpdir/spooled_named_temporary_file.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.3/setup.py` & `pytmpdir-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 package_name = "pytmpdir"
-package_version = '1.0.3'
+package_version = '1.0.4'
 
 setup(
     name=package_name,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     install_requires=["sphinx_rtd_theme", "sphinx<4"],
     version=package_version,
     description='A class representing a file system directory, that deletes on '
```

