# Comparing `tmp/datarails-0.3.0.tar.gz` & `tmp/datarails-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.3.0.tar", last modified: Sun Jul 30 06:15:36 2023, max compression
+gzip compressed data, was "datarails-0.3.1.tar", last modified: Sun Jul 30 06:19:28 2023, max compression
```

## Comparing `datarails-0.3.0.tar` & `datarails-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.851199 datarails-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-30 06:15:36.851199 datarails-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-30 06:15:25.000000 datarails-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.847199 datarails-0.3.0/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 06:15:25.000000 datarails-0.3.0/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-30 06:15:11.000000 datarails-0.3.0/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.851199 datarails-0.3.0/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 06:15:36.000000 datarails-0.3.0/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-30 06:15:25.000000 datarails-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:15:36.851199 datarails-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 06:15:11.000000 datarails-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:15:36.851199 datarails-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-30 06:15:11.000000 datarails-0.3.0/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:19:28.518856 datarails-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-30 06:19:28.518856 datarails-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-30 06:19:19.000000 datarails-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:19:28.514855 datarails-0.3.1/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 06:19:19.000000 datarails-0.3.1/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-30 06:19:08.000000 datarails-0.3.1/datarails/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-30 06:19:08.000000 datarails-0.3.1/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-30 06:19:08.000000 datarails-0.3.1/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-30 06:19:08.000000 datarails-0.3.1/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:19:28.518856 datarails-0.3.1/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-30 06:19:28.000000 datarails-0.3.1/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-30 06:19:28.000000 datarails-0.3.1/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:19:28.000000 datarails-0.3.1/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 06:19:28.000000 datarails-0.3.1/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 06:19:28.000000 datarails-0.3.1/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-30 06:19:19.000000 datarails-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:19:28.518856 datarails-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 06:19:08.000000 datarails-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:19:28.518856 datarails-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-30 06:19:08.000000 datarails-0.3.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-30 06:19:08.000000 datarails-0.3.1/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 06:19:08.000000 datarails-0.3.1/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-30 06:19:08.000000 datarails-0.3.1/tests/test_step.py
```

### Comparing `datarails-0.3.0/PKG-INFO` & `datarails-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: datarails
-Version: 0.3.0
+Version: 0.3.1
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 
 [![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.3.0 --
+####  -- VERSION 0.3.1 --
 
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
 ## Example Project
 There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
```

### Comparing `datarails-0.3.0/README.md` & `datarails-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.3.0 --
+####  -- VERSION 0.3.1 --
 
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
 ## Example Project
 There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
```

### Comparing `datarails-0.3.0/datarails/contexts.py` & `datarails-0.3.1/datarails/contexts.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.0/datarails/runner.py` & `datarails-0.3.1/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.0/datarails/step.py` & `datarails-0.3.1/datarails/step.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.0/datarails.egg-info/PKG-INFO` & `datarails-0.3.1/datarails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: datarails
-Version: 0.3.0
+Version: 0.3.1
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 
 [![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.3.0 --
+####  -- VERSION 0.3.1 --
 
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
 ## Example Project
 There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
```

### Comparing `datarails-0.3.0/pyproject.toml` & `datarails-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.3.0/tests/test_context.py` & `datarails-0.3.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.0/tests/test_databox.py` & `datarails-0.3.1/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.0/tests/test_runner.py` & `datarails-0.3.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.0/tests/test_step.py` & `datarails-0.3.1/tests/test_step.py`

 * *Files identical despite different names*

