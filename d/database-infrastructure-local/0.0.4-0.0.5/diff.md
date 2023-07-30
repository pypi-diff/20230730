# Comparing `tmp/database-infrastructure-local-0.0.4.tar.gz` & `tmp/database-infrastructure-local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-infrastructure-local-0.0.4.tar", last modified: Sun Jul 16 10:51:32 2023, max compression
+gzip compressed data, was "database-infrastructure-local-0.0.5.tar", last modified: Sun Jul 30 11:26:24 2023, max compression
```

## Comparing `database-infrastructure-local-0.0.4.tar` & `database-infrastructure-local-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:51:32.444152 database-infrastructure-local-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:51:32.444152 database-infrastructure-local-0.0.4/CirclesNumberGenerator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:51:17.000000 database-infrastructure-local-0.0.4/CirclesNumberGenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-16 10:51:17.000000 database-infrastructure-local-0.0.4/CirclesNumberGenerator/number_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-16 10:51:32.444152 database-infrastructure-local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-16 10:51:17.000000 database-infrastructure-local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:51:32.444152 database-infrastructure-local-0.0.4/database_infrastructure_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-16 10:51:32.000000 database-infrastructure-local-0.0.4/database_infrastructure_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 10:51:32.000000 database-infrastructure-local-0.0.4/database_infrastructure_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 10:51:32.000000 database-infrastructure-local-0.0.4/database_infrastructure_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 10:51:32.000000 database-infrastructure-local-0.0.4/database_infrastructure_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-16 10:51:17.000000 database-infrastructure-local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 10:51:32.444152 database-infrastructure-local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-16 10:51:17.000000 database-infrastructure-local-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:51:32.444152 database-infrastructure-local-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-16 10:51:17.000000 database-infrastructure-local-0.0.4/tests/test_number_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:26:24.279282 database-infrastructure-local-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:26:24.279282 database-infrastructure-local-0.0.5/CirclesNumberGenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 11:25:59.000000 database-infrastructure-local-0.0.5/CirclesNumberGenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-30 11:25:59.000000 database-infrastructure-local-0.0.5/CirclesNumberGenerator/number_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-30 11:26:24.279282 database-infrastructure-local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-30 11:25:59.000000 database-infrastructure-local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:26:24.279282 database-infrastructure-local-0.0.5/database_infrastructure_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-30 11:26:24.000000 database-infrastructure-local-0.0.5/database_infrastructure_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-30 11:26:24.000000 database-infrastructure-local-0.0.5/database_infrastructure_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:26:24.000000 database-infrastructure-local-0.0.5/database_infrastructure_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 11:26:24.000000 database-infrastructure-local-0.0.5/database_infrastructure_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 11:25:59.000000 database-infrastructure-local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:26:24.279282 database-infrastructure-local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-30 11:25:59.000000 database-infrastructure-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:26:24.279282 database-infrastructure-local-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-30 11:25:59.000000 database-infrastructure-local-0.0.5/tests/test_number_generator.py
```

### Comparing `database-infrastructure-local-0.0.4/README.md` & `database-infrastructure-local-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `database-infrastructure-local-0.0.4/setup.py` & `database-infrastructure-local-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='database-infrastructure-local',  
-     version='0.0.4',
+     version='0.0.5',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles Database Infrastructure Local Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `database-infrastructure-local-0.0.4/tests/test_number_generator.py` & `database-infrastructure-local-0.0.5/tests/test_number_generator.py`

 * *Files identical despite different names*

