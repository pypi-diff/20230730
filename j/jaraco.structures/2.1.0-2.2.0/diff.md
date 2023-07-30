# Comparing `tmp/jaraco.structures-2.1.0.tar.gz` & `tmp/jaraco.structures-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.structures-2.1.0.tar", last modified: Sun Feb  7 23:19:40 2021, max compression
+gzip compressed data, was "jaraco.structures-2.2.0.tar", last modified: Sun Jul 30 01:06:43 2023, max compression
```

## Comparing `jaraco.structures-2.1.0.tar` & `jaraco.structures-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/jaraco/structures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/jaraco/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3891 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/jaraco/structures/binary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 23:19:40.405922 jaraco.structures-2.1.0/jaraco.structures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-02-07 23:19:40.000000 jaraco.structures-2.1.0/jaraco.structures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      531 2021-02-07 23:19:40.000000 jaraco.structures-2.1.0/jaraco.structures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-07 23:19:40.000000 jaraco.structures-2.1.0/jaraco.structures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-02-07 23:19:40.000000 jaraco.structures-2.1.0/jaraco.structures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-02-07 23:19:40.000000 jaraco.structures-2.1.0/jaraco.structures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-02-07 23:19:40.409922 jaraco.structures-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/skeleton.md
--rw-r--r--   0 runner    (1001) docker     (121)      719 2021-02-07 23:19:17.000000 jaraco.structures-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.305197 jaraco.structures-2.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/jaraco/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/jaraco/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/jaraco/structures/binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/jaraco.structures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-30 01:06:43.000000 jaraco.structures-2.2.0/jaraco.structures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-30 01:06:43.000000 jaraco.structures-2.2.0/jaraco.structures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:06:43.000000 jaraco.structures-2.2.0/jaraco.structures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-30 01:06:43.000000 jaraco.structures-2.2.0/jaraco.structures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 01:06:43.000000 jaraco.structures-2.2.0/jaraco.structures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-30 01:06:43.309197 jaraco.structures-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-30 01:06:20.000000 jaraco.structures-2.2.0/tox.ini
```

### Comparing `jaraco.structures-2.1.0/CHANGES.rst` & `jaraco.structures-2.2.0/NEWS.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.2.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v2.1.0
 ======
 
 Refresh packaging. Require Python 3.6 or later. Switch to PEP 420 package.
 
 2.0
 ===
```

### Comparing `jaraco.structures-2.1.0/LICENSE` & `jaraco.structures-2.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.structures-2.1.0/PKG-INFO` & `jaraco.structures-2.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.structures
-Version: 2.1.0
+Version: 2.2.0
 Summary: Data structures by jaraco
 Home-page: https://github.com/jaraco/jaraco.structures
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.structures.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.structures.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.structures
-        
-        .. image:: https://github.com/jaraco/jaraco.structures/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.structures/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/jaracostructures/badge/?version=latest
-           :target: https://jaracostructures.readthedocs.io/en/latest/?badge=latest
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/jaraco.structures.svg
+   :target: https://pypi.org/project/jaraco.structures
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.structures.svg
+
+.. image:: https://github.com/jaraco/jaraco.structures/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.structures/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. image:: https://readthedocs.org/projects/jaracostructures/badge/?version=latest
+   :target: https://jaracostructures.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.structures-2.1.0/docs/conf.py` & `jaraco.structures-2.2.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `jaraco.structures-2.1.0/jaraco/structures/binary.py` & `jaraco.structures-2.2.0/jaraco/structures/binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     >>> get_bit_values(0x3, 2)
     [1, 1]
 
     >>> get_bit_values(0x3, 4)
     [0, 0, 1, 1]
     """
-    number += 2 ** size
+    number += 2**size
     return list(map(int, bin(number)[-size:]))
 
 
 def gen_bit_values(number):
     """
     Return a zero or one for each bit of a numeric value up to the most
     significant 1 bit, beginning with the least significant bit.
@@ -146,11 +146,9 @@
 
     def __new__(cls, name, bases, attrs):
         def make_property(name, value):
             if name.startswith('_') or not isinstance(value, numbers.Number):
                 return value
             return property(lambda self, value=value: bool(self & value))
 
-        newattrs = dict(
-            (name, make_property(name, value)) for name, value in attrs.items()
-        )
+        newattrs = {name: make_property(name, value) for name, value in attrs.items()}
         return type.__new__(cls, name, bases, newattrs)
```

### Comparing `jaraco.structures-2.1.0/jaraco.structures.egg-info/PKG-INFO` & `jaraco.structures-2.2.0/jaraco.structures.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.structures
-Version: 2.1.0
+Version: 2.2.0
 Summary: Data structures by jaraco
 Home-page: https://github.com/jaraco/jaraco.structures
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.structures.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.structures.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.structures
-        
-        .. image:: https://github.com/jaraco/jaraco.structures/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.structures/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/jaracostructures/badge/?version=latest
-           :target: https://jaracostructures.readthedocs.io/en/latest/?badge=latest
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/jaraco.structures.svg
+   :target: https://pypi.org/project/jaraco.structures
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.structures.svg
+
+.. image:: https://github.com/jaraco/jaraco.structures/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.structures/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. image:: https://readthedocs.org/projects/jaracostructures/badge/?version=latest
+   :target: https://jaracostructures.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.structures-2.1.0/jaraco.structures.egg-info/SOURCES.txt` & `jaraco.structures-2.2.0/jaraco.structures.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 .coveragerc
-.flake8
+.editorconfig
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
-.github/workflows/automerge.yml
+.github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.structures.egg-info/PKG-INFO
 jaraco.structures.egg-info/SOURCES.txt
 jaraco.structures.egg-info/dependency_links.txt
```

### Comparing `jaraco.structures-2.1.0/setup.cfg` & `jaraco.structures-2.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = jaraco.structures
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Data structures by jaraco
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.structures
 classifiers = 
@@ -13,37 +11,41 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
-setup_requires = setuptools_scm[toml] >= 3.4.1
 
 [options.packages.find]
 exclude = 
 	build*
+	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs >= 1.2.3
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy"
+	pytest >= 6
+	pytest-checkdocs >= 2.4
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy"
-	pytest-enabler
+	pytest-mypy >= 0.9.1; \
+	python_implementation != "PyPy"
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

