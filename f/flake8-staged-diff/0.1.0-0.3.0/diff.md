# Comparing `tmp/flake8-staged-diff-0.1.0.tar.gz` & `tmp/flake8-staged-diff-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-staged-diff-0.1.0.tar", last modified: Sun Jul 23 20:32:58 2023, max compression
+gzip compressed data, was "flake8-staged-diff-0.3.0.tar", last modified: Sat Jul 29 22:04:59 2023, max compression
```

## Comparing `flake8-staged-diff-0.1.0.tar` & `flake8-staged-diff-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:32:58.924396 flake8-staged-diff-0.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-23 20:32:55.000000 flake8-staged-diff-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-23 20:32:58.924396 flake8-staged-diff-0.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-23 20:32:55.000000 flake8-staged-diff-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:32:58.924396 flake8-staged-diff-0.1.0/flake8_staged_diff/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:32:55.000000 flake8-staged-diff-0.1.0/flake8_staged_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-23 20:32:55.000000 flake8-staged-diff-0.1.0/flake8_staged_diff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:32:58.924396 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-23 20:32:58.000000 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-23 20:32:58.000000 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 20:32:58.000000 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-23 20:32:58.000000 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-23 20:32:58.000000 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-23 20:32:58.000000 flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-07-23 20:32:58.924396 flake8-staged-diff-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-07-23 20:32:55.000000 flake8-staged-diff-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:59.368514 flake8-staged-diff-0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-29 22:04:52.000000 flake8-staged-diff-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-29 22:04:59.368514 flake8-staged-diff-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-29 22:04:52.000000 flake8-staged-diff-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:59.368514 flake8-staged-diff-0.3.0/flake8_staged_diff/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:52.000000 flake8-staged-diff-0.3.0/flake8_staged_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-29 22:04:52.000000 flake8-staged-diff-0.3.0/flake8_staged_diff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:59.368514 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-29 22:04:59.000000 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-29 22:04:59.000000 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:04:59.000000 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-29 22:04:59.000000 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 22:04:59.000000 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 22:04:59.000000 flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-07-29 22:04:59.372514 flake8-staged-diff-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-07-29 22:04:52.000000 flake8-staged-diff-0.3.0/setup.py
```

### Comparing `flake8-staged-diff-0.1.0/LICENSE` & `flake8-staged-diff-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-staged-diff-0.1.0/PKG-INFO` & `flake8-staged-diff-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-staged-diff
-Version: 0.1.0
+Version: 0.3.0
 Summary: flake8 wrapper to run only on modified/staged code
 Home-page: https://github.com/bagerard/flake8-staged-diff
 Maintainer: Bastien Gerard
 Maintainer-email: bast.gerard@gmail.com
 License: MIT License
 Keywords: flake8 diff linter pre-commit
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flake8-staged-diff-0.1.0/README.md` & `flake8-staged-diff-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8-staged-diff-0.1.0/flake8_staged_diff/main.py` & `flake8-staged-diff-0.3.0/flake8_staged_diff/main.py`

 * *Files identical despite different names*

### Comparing `flake8-staged-diff-0.1.0/flake8_staged_diff.egg-info/PKG-INFO` & `flake8-staged-diff-0.3.0/flake8_staged_diff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-staged-diff
-Version: 0.1.0
+Version: 0.3.0
 Summary: flake8 wrapper to run only on modified/staged code
 Home-page: https://github.com/bagerard/flake8-staged-diff
 Maintainer: Bastien Gerard
 Maintainer-email: bast.gerard@gmail.com
 License: MIT License
 Keywords: flake8 diff linter pre-commit
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flake8-staged-diff-0.1.0/setup.py` & `flake8-staged-diff-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 INSTALL_REQUIRES = [
     "flake8",
 ]
 
-VERSION = "0.1.0"
+VERSION = "0.3.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="flake8-staged-diff",
     version=VERSION,
```

