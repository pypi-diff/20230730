# Comparing `tmp/DS2STAC-Ingester-0.8.tar.gz` & `tmp/DS2STAC-Ingester-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DS2STAC-Ingester-0.8.tar", last modified: Thu Jul  6 07:42:03 2023, max compression
+gzip compressed data, was "DS2STAC-Ingester-1.0.0.tar", last modified: Sun Jul 30 10:07:43 2023, max compression
```

## Comparing `DS2STAC-Ingester-0.8.tar` & `DS2STAC-Ingester-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-06 07:42:03.464143 DS2STAC-Ingester-0.8/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/CONTRIBUTING.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-06 07:42:03.461400 DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901     2658 2023-07-06 07:42:03.000000 DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-06 07:42:03.000000 DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-06 07:42:03.000000 DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      326 2023-07-06 07:42:03.000000 DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901       23 2023-07-06 07:42:03.000000 DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/top_level.txt
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901     2658 2023-07-06 07:42:03.464230 DS2STAC-Ingester-0.8/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-06 07:42:03.462924 DS2STAC-Ingester-0.8/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/docs/usage.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-06 07:42:03.464889 DS2STAC-Ingester-0.8/ds2stac_ingester/
--rw-r--r--   0 hadizadeh-m (15144)      901      481 2023-07-06 07:39:35.000000 DS2STAC-Ingester-0.8/ds2stac_ingester/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      495 2023-07-06 07:42:03.464925 DS2STAC-Ingester-0.8/ds2stac_ingester/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/ds2stac_ingester/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/ds2stac_ingester/config_pgstac.py
--rw-r--r--   0 hadizadeh-m (15144)      901     4125 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/ds2stac_ingester/ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1955 2023-07-06 07:42:03.464733 DS2STAC-Ingester-0.8/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      307 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-06 07:42:03.464016 DS2STAC-Ingester-0.8/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-06 07:37:59.000000 DS2STAC-Ingester-0.8/tests/test_ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901    83607 2023-07-06 07:39:35.000000 DS2STAC-Ingester-0.8/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.879797 DS2STAC-Ingester-1.0.0/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/CONTRIBUTING.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.877569 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/top_level.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:07:43.879880 DS2STAC-Ingester-1.0.0/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.878814 DS2STAC-Ingester-1.0.0/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/usage.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.880421 DS2STAC-Ingester-1.0.0/ds2stac_ingester/
+-rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 10:07:43.880452 DS2STAC-Ingester-1.0.0/ds2stac_ingester/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/config_pgstac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     6011 2023-07-30 10:03:14.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1962 2023-07-30 10:07:43.880269 DS2STAC-Ingester-1.0.0/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.0/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.879687 DS2STAC-Ingester-1.0.0/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/tests/test_ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/versioneer.py
```

### Comparing `DS2STAC-Ingester-0.8/CONTRIBUTING.rst` & `DS2STAC-Ingester-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/PKG-INFO` & `DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 0.8
+Version: 1.0.0
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-0.8/DS2STAC_Ingester.egg-info/SOURCES.txt` & `DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/LICENSE` & `DS2STAC-Ingester-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/PKG-INFO` & `DS2STAC-Ingester-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 0.8
+Version: 1.0.0
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-0.8/README.rst` & `DS2STAC-Ingester-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/docs/Makefile` & `DS2STAC-Ingester-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/docs/conf.py` & `DS2STAC-Ingester-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/docs/installation.rst` & `DS2STAC-Ingester-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/docs/make.bat` & `DS2STAC-Ingester-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/ds2stac_ingester/config_pgstac.py` & `DS2STAC-Ingester-1.0.0/ds2stac_ingester/config_pgstac.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/setup.cfg` & `DS2STAC-Ingester-1.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 [flake8]
 exclude = docs
 ignore = 
 	E203,
 	E402,
 	E501,
 	W503,
+	F541,
 
 [tool:pytest]
 collect_ignore = ['setup.py']
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `DS2STAC-Ingester-0.8/tests/test_ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.0/tests/test_ds2stac_ingester.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-0.8/versioneer.py` & `DS2STAC-Ingester-1.0.0/versioneer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,35 @@
-
-# Version: 0.28
+# Version: 0.21
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain (Unlicense)
-* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* License: Public Domain
+* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in setuptools-based
+This is a tool for managing a recorded version number in distutils-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-Versioneer provides two installation modes. The "classic" vendored mode installs
-a copy of versioneer into your repository. The experimental build-time dependency mode
-is intended to allow you to skip this step and simplify the process of upgrading.
-
-### Vendored mode
-
-* `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-   * Note that you will need to add `tomli; python_version < "3.11"` to your
-     build-time dependencies if you use `pyproject.toml`
-* run `versioneer install --vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
-
-### Build-time dependency mode
-
 * `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
-  to the `requires` key of the `build-system` table in `pyproject.toml`:
-  ```toml
-  [build-system]
-  requires = ["setuptools", "versioneer[toml]"]
-  build-backend = "setuptools.build_meta"
-  ```
-* run `versioneer install --no-vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
+* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
+* run `versioneer install` in your source tree, commit the results
+* Verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -255,18 +226,17 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg` and `pyproject.toml`, if necessary,
-  to include any new configuration settings indicated by the release notes.
-  See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install --[no-]vendor` in your source tree, to replace
+* edit `setup.cfg`, if necessary, to include any new configuration settings
+  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -288,16 +258,17 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the "Unlicense", as described in
-https://unlicense.org/.
+Specifically, both are released under the Creative Commons "Public Domain
+Dedication" license (CC0-1.0), as described in
+https://creativecommons.org/publicdomain/zero/1.0/ .
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
@@ -311,26 +282,15 @@
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
-from pathlib import Path
 from typing import Callable, Dict
-import functools
-
-have_tomllib = True
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    try:
-        import tomli as tomllib
-    except ImportError:
-        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -344,70 +304,64 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+        if me_dir != vsr_dir:
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    root = Path(root)
-    pyproject_toml = root / "pyproject.toml"
-    setup_cfg = root / "setup.cfg"
-    section = None
-    if pyproject_toml.exists() and have_tomllib:
-        try:
-            with open(pyproject_toml, 'rb') as fobj:
-                pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
-        except (tomllib.TOMLDecodeError, KeyError):
-            pass
-    if not section:
-        parser = configparser.ConfigParser()
-        with open(setup_cfg) as cfg_file:
-            parser.read_file(cfg_file)
-        parser.get("versioneer", "VCS")  # raise error if missing
+    setup_cfg = os.path.join(root, "setup.cfg")
+    parser = configparser.ConfigParser()
+    with open(setup_cfg, "r") as cfg_file:
+        parser.read_file(cfg_file)
+    VCS = parser.get("versioneer", "VCS")  # mandatory
 
-        section = parser["versioneer"]
+    # Dict-like interface for non-mandatory entries
+    section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
+    cfg.VCS = VCS
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""', None):
+    if cfg.tag_prefix in ("''", '""'):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
     cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
@@ -417,42 +371,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands, args, cwd=None, verbose=False, hide_stderr=False, env=None
+):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -467,34 +419,34 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain.
-# Generated by versioneer-0.28
-# https://github.com/python-versioneer/python-versioneer
+# This file is released into the public domain. Generated by
+# versioneer-0.21 (https://github.com/python-versioneer/python-versioneer)
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
 from typing import Callable, Dict
-import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -544,30 +496,22 @@
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+                                               else None))
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
@@ -707,37 +651,33 @@
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
+    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
+        TAG_PREFIX_REGEX = r"\*"
 
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+                   hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
+                                     "--always", "--long",
+                                     "--match",
+                                     "%%s%%s" %% (tag_prefix, TAG_PREFIX_REGEX)],
+                              cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -818,16 +758,16 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
@@ -915,15 +855,15 @@
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
             tag_version, post_version = pep440_split_post(pieces["closest-tag"])
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+                rendered += ".post%%d.dev%%d" %% (post_version+1, pieces["distance"])
             else:
                 rendered += ".post0.dev%%d" %% (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1183,99 +1123,112 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r'\d', r):
+            if not re.match(r"\d", r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
+    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
+        TAG_PREFIX_REGEX = r"\*"
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    _, rc = runner(
+        GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True
+    )
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            "%s%s" % (tag_prefix, TAG_PREFIX_REGEX),
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
+    branch_name, rc = runner(
+        GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root
+    )
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1307,81 +1260,85 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = (
+                "unable to parse git-describe output: '%s'" % describe_out
+            )
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(versionfile_source, ipy):
+def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [versionfile_source]
+    files = [manifest_in, versionfile_source]
     if ipy:
         files.append(ipy)
-    if "VERSIONEER_PEP518" not in globals():
-        try:
-            my_path = __file__
-            if my_path.endswith((".pyc", ".pyo")):
-                my_path = os.path.splitext(my_path)[0] + ".py"
-            versioneer_file = os.path.relpath(my_path)
-        except NameError:
-            versioneer_file = "versioneer.py"
-        files.append(versioneer_file)
+    try:
+        my_path = __file__
+        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
+            my_path = os.path.splitext(my_path)[0] + ".py"
+        versioneer_file = os.path.relpath(my_path)
+    except NameError:
+        versioneer_file = "versioneer.py"
+    files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
@@ -1403,28 +1360,34 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.28) from
+# This file was generated by 'versioneer.py' (0.21) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1440,29 +1403,36 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+        contents,
+        re.M | re.S,
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+            contents,
+            re.M | re.S,
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(
+        versions, sort_keys=True, indent=1, separators=(",", ": ")
+    )
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1486,16 +1456,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1516,16 +1485,15 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
@@ -1542,18 +1510,23 @@
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            tag_version, post_version = pep440_split_post(
+                pieces["closest-tag"]
+            )
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+                rendered += ".post%d.dev%d" % (
+                    post_version + 1,
+                    pieces["distance"],
+                )
             else:
                 rendered += ".post0.dev%d" % (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1678,19 +1651,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1706,17 +1681,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1731,16 +1710,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1786,26 +1766,30 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
 def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools subclasses used by Versioneer.
+    """Get the custom setuptools/distutils subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1819,16 +1803,16 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to setuptools
-    from setuptools import Command
+    # we add "version" to both distutils and setuptools
+    from distutils.core import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1841,63 +1825,63 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
-    # we override "build_py" in setuptools
+    # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
-    # pip install -e . and setuptool/editable_wheel will invoke build_py
-    # but the build_py command is not expected to copy any files.
-
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py = cmds['build_py']
-    else:
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
+    elif "setuptools" in sys.modules:
         from setuptools.command.build_py import build_py as _build_py
+    else:
+        from distutils.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
-            if getattr(self, "editable_mode", False):
-                # During editable installs `.py` and data files are
-                # not copied to build_lib
-                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(
+                    self.build_lib, cfg.versionfile_build
+                )
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
-    else:
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
+    elif "setuptools" in sys.modules:
         from setuptools.command.build_ext import build_ext as _build_ext
+    else:
+        from distutils.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
@@ -1905,29 +1889,25 @@
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
-            if not cfg.versionfile_build:
-                return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
-            if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
-                return
+            target_versionfile = os.path.join(
+                self.build_lib, cfg.versionfile_build
+            )
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
+
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1940,94 +1920,64 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
-        try:
-            from py2exe.setuptools_buildexe import py2exe as _py2exe
-        except ImportError:
-            from py2exe.distutils_buildexe import py2exe as _py2exe
+    if "py2exe" in sys.modules:  # py2exe enabled?
+        from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
-        cmds["py2exe"] = cmd_py2exe
-
-    # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info = cmds['egg_info']
-    else:
-        from setuptools.command.egg_info import egg_info as _egg_info
-
-    class cmd_egg_info(_egg_info):
-        def find_sources(self):
-            # egg_info.find_sources builds the manifest list and writes it
-            # in one shot
-            super().find_sources()
-
-            # Modify the filelist and normalize it
-            root = get_root()
-            cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
-            if cfg.versionfile_source:
-                # There are rare cases where versionfile_source might not be
-                # included by default, so we must be explicit
-                self.filelist.append(cfg.versionfile_source)
-            self.filelist.sort()
-            self.filelist.remove_duplicates()
-
-            # The write method is hidden in the manifest_maker instance that
-            # generated the filelist and was thrown away
-            # We will instead replicate their final normalization (to unicode,
-            # and POSIX-style paths)
-            from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
-
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
 
-    cmds['egg_info'] = cmd_egg_info
+        cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist = cmds['sdist']
-    else:
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
+    elif "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
+    else:
+        from distutils.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -2039,16 +1989,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2100,36 +2052,43 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        OSError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print(
+                "Adding sample versioneer config to setup.cfg", file=sys.stderr
+            )
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
@@ -2144,18 +2103,52 @@
                 f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
+    # Make sure both the top-level "versioneer.py" and versionfile_source
+    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
+    # they'll be copied into source distributions. Pip won't be able to
+    # install the package without this.
+    manifest_in = os.path.join(root, "MANIFEST.in")
+    simple_includes = set()
+    try:
+        with open(manifest_in, "r") as f:
+            for line in f:
+                if line.startswith("include "):
+                    for include in line.split()[1:]:
+                        simple_includes.add(include)
+    except OSError:
+        pass
+    # That doesn't cover everything MANIFEST.in can do
+    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
+    # it might give some false negatives. Appending redundant 'include'
+    # lines is safe, though.
+    if "versioneer.py" not in simple_includes:
+        print(" appending 'versioneer.py' to MANIFEST.in")
+        with open(manifest_in, "a") as f:
+            f.write("include versioneer.py\n")
+    else:
+        print(" 'versioneer.py' already in MANIFEST.in")
+    if cfg.versionfile_source not in simple_includes:
+        print(
+            " appending versionfile_source ('%s') to MANIFEST.in"
+            % cfg.versionfile_source
+        )
+        with open(manifest_in, "a") as f:
+            f.write("include %s\n" % cfg.versionfile_source)
+    else:
+        print(" versionfile_source already in MANIFEST.in")
+
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(cfg.versionfile_source, ipy)
+    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -2188,18 +2181,14 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
-def setup_command():
-    """Set up Versioneer and exit with appropriate error code."""
-    errors = do_setup()
-    errors += scan_setup_py()
-    sys.exit(1 if errors else 0)
-
-
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        setup_command()
+        errors = do_setup()
+        errors += scan_setup_py()
+        if errors:
+            sys.exit(1)
```

