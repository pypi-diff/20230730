# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230728.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230728.tar", last modified: Fri Jul 28 00:06:43 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230729.tar", last modified: Sat Jul 29 00:06:38 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230728.tar` & `jaxutils-nightly-0.0.8.dev20230729.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-28 00:06:43.831946 jaxutils-nightly-0.0.8.dev20230728/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-28 00:06:43.831946 jaxutils-nightly-0.0.8.dev20230728/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-28 00:06:43.835947 jaxutils-nightly-0.0.8.dev20230728/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-07-28 00:06:43.835947 jaxutils-nightly-0.0.8.dev20230728/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-28 00:06:43.831946 jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-28 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-07-28 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-28 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-07-28 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-07-28 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-07-28 00:06:43.835947 jaxutils-nightly-0.0.8.dev20230728/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-07-28 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230728/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 00:06:38.878146 jaxutils-nightly-0.0.8.dev20230729/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-29 00:06:38.878146 jaxutils-nightly-0.0.8.dev20230729/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 00:06:38.878146 jaxutils-nightly-0.0.8.dev20230729/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-07-29 00:06:38.878146 jaxutils-nightly-0.0.8.dev20230729/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 00:06:38.878146 jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-29 00:06:38.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-07-29 00:06:38.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-29 00:06:38.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-07-29 00:06:38.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-07-29 00:06:38.000000 jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-07-29 00:06:38.878146 jaxutils-nightly-0.0.8.dev20230729/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-07-29 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230729/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230728/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230729/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230728
+Version: 0.0.8.dev20230729
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230728/README.md` & `jaxutils-nightly-0.0.8.dev20230729/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230729/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230728
+Version: 0.0.8.dev20230729
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230728/setup.py` & `jaxutils-nightly-0.0.8.dev20230729/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230728/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230729/versioneer.py`

 * *Files identical despite different names*

