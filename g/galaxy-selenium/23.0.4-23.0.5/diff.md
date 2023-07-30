# Comparing `tmp/galaxy-selenium-23.0.4.tar.gz` & `tmp/galaxy-selenium-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/selenium/dist/.tmp-0qtlnd7z/galaxy-selenium-23.0.4.tar", last modified: Fri Jun 30 22:05:35 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/selenium/dist/.tmp-zc0n8_7n/galaxy-selenium-23.0.5.tar", last modified: Sun Jul 30 10:51:54 2023, max compression
```

## Comparing `galaxy-selenium-23.0.4.tar` & `galaxy-selenium-23.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-selenium-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/has_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/jupyter_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    88548 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/navigates_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy/selenium/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/scripts/dump_tour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/sizzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/smart_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy/selenium/toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/galaxy/selenium/toolbox/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/galaxy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-30 22:05:35.000000 galaxy-selenium-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:00:50.000000 galaxy-selenium-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-selenium-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/has_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/jupyter_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88548 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/navigates_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy/selenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/scripts/dump_tour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/sizzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/smart_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy/selenium/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/galaxy/selenium/toolbox/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/galaxy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-30 10:51:54.000000 galaxy-selenium-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:47:08.000000 galaxy-selenium-23.0.5/test-requirements.txt
```

### Comparing `galaxy-selenium-23.0.4/HISTORY.rst` & `galaxy-selenium-23.0.5/HISTORY.rst`

 * *Files 19% similar despite different names*

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
@@ -33,14 +39,15 @@
 
 ============
 Enhancements
 ============
 
 * 
 * 
+* 
 * Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
 
 -------------------
 20.9.0 (2020-10-15)
 -------------------
 
 * First release from the 20.09 branch of Galaxy.
```

### Comparing `galaxy-selenium-23.0.4/LICENSE` & `galaxy-selenium-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/PKG-INFO` & `galaxy-selenium-23.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
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
@@ -76,14 +82,15 @@
 
 ============
 Enhancements
 ============
 
 * 
 * 
+* 
 * Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
 
 -------------------
 20.9.0 (2020-10-15)
 -------------------
 
 * First release from the 20.09 branch of Galaxy.
```

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/cli.py` & `galaxy-selenium-23.0.5/galaxy/selenium/cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/context.py` & `galaxy-selenium-23.0.5/galaxy/selenium/context.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/driver_factory.py` & `galaxy-selenium-23.0.5/galaxy/selenium/driver_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/has_driver.py` & `galaxy-selenium-23.0.5/galaxy/selenium/has_driver.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/navigates_galaxy.py` & `galaxy-selenium-23.0.5/galaxy/selenium/navigates_galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/scripts/dump_tour.py` & `galaxy-selenium-23.0.5/galaxy/selenium/scripts/dump_tour.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/sizzle.py` & `galaxy-selenium-23.0.5/galaxy/selenium/sizzle.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy/selenium/smart_components.py` & `galaxy-selenium-23.0.5/galaxy/selenium/smart_components.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/galaxy_selenium.egg-info/PKG-INFO` & `galaxy-selenium-23.0.5/galaxy_selenium.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
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
@@ -76,14 +82,15 @@
 
 ============
 Enhancements
 ============
 
 * 
 * 
+* 
 * Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
 
 -------------------
 20.9.0 (2020-10-15)
 -------------------
 
 * First release from the 20.09 branch of Galaxy.
```

### Comparing `galaxy-selenium-23.0.4/galaxy_selenium.egg-info/SOURCES.txt` & `galaxy-selenium-23.0.5/galaxy_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.4/setup.cfg` & `galaxy-selenium-23.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-selenium
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	galaxy-util
 	PyYAML
```

