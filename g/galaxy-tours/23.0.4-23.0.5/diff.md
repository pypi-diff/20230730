# Comparing `tmp/galaxy-tours-23.0.4.tar.gz` & `tmp/galaxy-tours-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tours/dist/.tmp-7lx3wwok/galaxy-tours-23.0.4.tar", last modified: Fri Jun 30 22:06:06 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tours/dist/.tmp-i0p0idi6/galaxy-tours-23.0.5.tar", last modified: Sun Jul 30 10:52:25 2023, max compression
```

## Comparing `galaxy-tours-23.0.4.tar` & `galaxy-tours-23.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-tours-23.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/galaxy/tours/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/tours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/tours/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/tours/_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/tours/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/galaxy/tours/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-30 22:06:05.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:06:05.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 22:06:05.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 22:06:05.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:06:05.000000 galaxy-tours-23.0.4/galaxy_tours.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-30 22:06:06.000000 galaxy-tours-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:00:50.000000 galaxy-tours-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-tours-23.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy/tours/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/tours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/tours/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/tours/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/tours/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/galaxy/tours/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/galaxy_tours.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-30 10:52:25.000000 galaxy-tours-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:47:08.000000 galaxy-tours-23.0.5/test-requirements.txt
```

### Comparing `galaxy-tours-23.0.4/HISTORY.rst` & `galaxy-tours-23.0.5/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-tours-23.0.4/LICENSE.txt` & `galaxy-tours-23.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.4/PKG-INFO` & `galaxy-tours-23.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy tours backend framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-tours-23.0.4/galaxy/tours/_impl.py` & `galaxy-tours-23.0.5/galaxy/tours/_impl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.4/galaxy/tours/_schema.py` & `galaxy-tours-23.0.5/galaxy/tours/_schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.4/galaxy/tours/validate.py` & `galaxy-tours-23.0.5/galaxy/tours/validate.py`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.4/galaxy_tours.egg-info/PKG-INFO` & `galaxy-tours-23.0.5/galaxy_tours.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy tours backend framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-tours-23.0.4/setup.cfg` & `galaxy-tours-23.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tours
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	pydantic<2
 	PyYAML
```

