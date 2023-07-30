# Comparing `tmp/galaxy-navigation-23.0.4.tar.gz` & `tmp/galaxy-navigation-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/navigation/dist/.tmp-2px2ldfa/galaxy-navigation-23.0.4.tar", last modified: Fri Jun 30 22:03:31 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/navigation/dist/.tmp-eksaulmz/galaxy-navigation-23.0.5.tar", last modified: Sun Jul 30 10:49:46 2023, max compression
```

## Comparing `galaxy-navigation-23.0.4.tar` & `galaxy-navigation-23.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-navigation-23.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/galaxy/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/galaxy/navigation/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/galaxy/navigation/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-06-30 22:00:49.000000 galaxy-navigation-23.0.4/galaxy/navigation/navigation.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy_navigation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy_navigation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy_navigation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy_navigation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy_navigation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/galaxy_navigation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-30 22:03:31.000000 galaxy-navigation-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:00:50.000000 galaxy-navigation-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-navigation-23.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/galaxy/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/galaxy/navigation/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/galaxy/navigation/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-30 10:47:07.000000 galaxy-navigation-23.0.5/galaxy/navigation/navigation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy_navigation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy_navigation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy_navigation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy_navigation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy_navigation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/galaxy_navigation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-30 10:49:46.000000 galaxy-navigation-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:47:08.000000 galaxy-navigation-23.0.5/test-requirements.txt
```

### Comparing `galaxy-navigation-23.0.4/HISTORY.rst` & `galaxy-navigation-23.0.5/HISTORY.rst`

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

### Comparing `galaxy-navigation-23.0.4/LICENSE.txt` & `galaxy-navigation-23.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-23.0.4/PKG-INFO` & `galaxy-navigation-23.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-navigation
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy client DOM navigation framework
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

### Comparing `galaxy-navigation-23.0.4/galaxy/navigation/components.py` & `galaxy-navigation-23.0.5/galaxy/navigation/components.py`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-23.0.4/galaxy/navigation/navigation.yml` & `galaxy-navigation-23.0.5/galaxy/navigation/navigation.yml`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-23.0.4/galaxy_navigation.egg-info/PKG-INFO` & `galaxy-navigation-23.0.5/galaxy_navigation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-navigation
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy client DOM navigation framework
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

### Comparing `galaxy-navigation-23.0.4/setup.cfg` & `galaxy-navigation-23.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-navigation
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	PyYAML
 packages = find:
```

