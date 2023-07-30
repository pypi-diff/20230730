# Comparing `tmp/py3data-0.3.tar.gz` & `tmp/py3data-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3data-0.3.tar", last modified: Sun Jul 30 10:16:18 2023, max compression
+gzip compressed data, was "py3data-0.3.1.tar", last modified: Sun Jul 30 10:33:48 2023, max compression
```

## Comparing `py3data-0.3.tar` & `py3data-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:16:18.563661 py3data-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:16:18.563661 py3data-0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:16:18.563661 py3data-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-30 10:16:07.000000 py3data-0.3/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-30 10:16:07.000000 py3data-0.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-30 10:16:07.000000 py3data-0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-30 10:16:07.000000 py3data-0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-30 10:16:07.000000 py3data-0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 10:16:07.000000 py3data-0.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 10:16:07.000000 py3data-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-30 10:16:18.563661 py3data-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-30 10:16:07.000000 py3data-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:16:18.563661 py3data-0.3/py3data/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-30 10:16:07.000000 py3data-0.3/py3data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-30 10:16:18.000000 py3data-0.3/py3data/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-30 10:16:07.000000 py3data-0.3/py3data/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-30 10:16:07.000000 py3data-0.3/py3data/xmltodict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:16:18.563661 py3data-0.3/py3data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-30 10:16:18.000000 py3data-0.3/py3data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-30 10:16:18.000000 py3data-0.3/py3data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:16:18.000000 py3data-0.3/py3data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 10:16:18.000000 py3data-0.3/py3data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 10:16:18.000000 py3data-0.3/py3data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-30 10:16:07.000000 py3data-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 10:16:18.563661 py3data-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:16:18.563661 py3data-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-30 10:16:07.000000 py3data-0.3/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:33:48.308068 py3data-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:33:48.304068 py3data-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:33:48.304068 py3data-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-30 10:33:38.000000 py3data-0.3.1/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-30 10:33:38.000000 py3data-0.3.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-30 10:33:38.000000 py3data-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-30 10:33:38.000000 py3data-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-30 10:33:38.000000 py3data-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-30 10:33:38.000000 py3data-0.3.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 10:33:38.000000 py3data-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-30 10:33:48.308068 py3data-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-30 10:33:38.000000 py3data-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:33:48.304068 py3data-0.3.1/py3data/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-30 10:33:38.000000 py3data-0.3.1/py3data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 10:33:48.000000 py3data-0.3.1/py3data/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-30 10:33:38.000000 py3data-0.3.1/py3data/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-30 10:33:38.000000 py3data-0.3.1/py3data/xmltodict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:33:48.308068 py3data-0.3.1/py3data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-30 10:33:48.000000 py3data-0.3.1/py3data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-30 10:33:48.000000 py3data-0.3.1/py3data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:33:48.000000 py3data-0.3.1/py3data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 10:33:48.000000 py3data-0.3.1/py3data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 10:33:48.000000 py3data-0.3.1/py3data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-30 10:33:38.000000 py3data-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 10:33:48.308068 py3data-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:33:48.308068 py3data-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-30 10:33:38.000000 py3data-0.3.1/tests/test_api.py
```

### Comparing `py3data-0.3/.github/workflows/python-package.yml` & `py3data-0.3.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `py3data-0.3/.github/workflows/python-publish.yml` & `py3data-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `py3data-0.3/LICENSE` & `py3data-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3data-0.3/PKG-INFO` & `py3data-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3data
-Version: 0.3
+Version: 0.3.1
 Summary: A flexible and lightweight Python interface to the re3data.org database
 Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 # py3data
 
-![PyPI](https://img.shields.io/pypi/v/py3data) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
+[![PyPI](https://img.shields.io/pypi/v/py3data)](https://pypi.org/project/py3data/) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
 
 py3data is a Python library for [re3data](https://re3data.org/) registry.
 Re3data is a global registry of research data repositories that covers
 research data repositories from different academic disciplines. It includes
 repositories that enable permanent storage of and access to data sets to
 researchers, funding bodies, publishers, and scholarly institutions. Re3data
 offers an open and free [REST API](https://www.re3data.org/api/doc). py3data
```

### Comparing `py3data-0.3/README.md` & `py3data-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # py3data
 
-![PyPI](https://img.shields.io/pypi/v/py3data) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
+[![PyPI](https://img.shields.io/pypi/v/py3data)](https://pypi.org/project/py3data/) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
 
 py3data is a Python library for [re3data](https://re3data.org/) registry.
 Re3data is a global registry of research data repositories that covers
 research data repositories from different academic disciplines. It includes
 repositories that enable permanent storage of and access to data sets to
 researchers, funding bodies, publishers, and scholarly institutions. Re3data
 offers an open and free [REST API](https://www.re3data.org/api/doc). py3data
```

### Comparing `py3data-0.3/py3data/api.py` & `py3data-0.3.1/py3data/api.py`

 * *Files identical despite different names*

### Comparing `py3data-0.3/py3data/xmltodict.py` & `py3data-0.3.1/py3data/xmltodict.py`

 * *Files identical despite different names*

### Comparing `py3data-0.3/py3data.egg-info/PKG-INFO` & `py3data-0.3.1/py3data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3data
-Version: 0.3
+Version: 0.3.1
 Summary: A flexible and lightweight Python interface to the re3data.org database
 Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 # py3data
 
-![PyPI](https://img.shields.io/pypi/v/py3data) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
+[![PyPI](https://img.shields.io/pypi/v/py3data)](https://pypi.org/project/py3data/) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
 
 py3data is a Python library for [re3data](https://re3data.org/) registry.
 Re3data is a global registry of research data repositories that covers
 research data repositories from different academic disciplines. It includes
 repositories that enable permanent storage of and access to data sets to
 researchers, funding bodies, publishers, and scholarly institutions. Re3data
 offers an open and free [REST API](https://www.re3data.org/api/doc). py3data
```

### Comparing `py3data-0.3/pyproject.toml` & `py3data-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py3data-0.3/tests/test_api.py` & `py3data-0.3.1/tests/test_api.py`

 * *Files identical despite different names*

