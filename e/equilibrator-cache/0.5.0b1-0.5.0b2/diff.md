# Comparing `tmp/equilibrator-cache-0.5.0b1.tar.gz` & `tmp/equilibrator-cache-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-cache-0.5.0b1.tar", last modified: Sun Jul 30 03:51:14 2023, max compression
+gzip compressed data, was "equilibrator-cache-0.5.0b2.tar", last modified: Sun Jul 30 08:43:44 2023, max compression
```

## Comparing `equilibrator-cache-0.5.0b1.tar` & `equilibrator-cache-0.5.0b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.454778 equilibrator-cache-0.5.0b1/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2480 2023-07-30 03:51:14.454778 equilibrator-cache-0.5.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-30 03:51:14.455778 equilibrator-cache-0.5.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.447778 equilibrator-cache-0.5.0b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.455778 equilibrator-cache-0.5.0b1/src/equilibrator_cache/
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 03:51:14.455778 equilibrator-cache-0.5.0b1/src/equilibrator_cache/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/api.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)    12832 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/compound_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.454778 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_identifier.py
--rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_microspecies.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/magnesium_dissociation_constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/reaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/thermodynamic_constants.py
--rwxrwxrwx   0 root         (0) root         (0)     6740 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/zenodo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.452777 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2480 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:43:44.893598 equilibrator-cache-0.5.0b2/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-30 08:43:44.893598 equilibrator-cache-0.5.0b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-07-30 08:43:44.894598 equilibrator-cache-0.5.0b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:43:44.886598 equilibrator-cache-0.5.0b2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:43:44.894598 equilibrator-cache-0.5.0b2/src/equilibrator_cache/
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 08:43:44.894598 equilibrator-cache-0.5.0b2/src/equilibrator_cache/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12832 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/compound_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:43:44.893598 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/compound.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/compound_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/compound_microspecies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/magnesium_dissociation_constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/thermodynamic_constants.py
+-rwxrwxrwx   0 root         (0) root         (0)     6740 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache/zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:43:44.891598 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-30 08:43:44.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-30 08:43:44.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 08:43:44.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-30 08:43:44.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-30 08:43:44.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 08:43:44.000000 equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-30 08:43:32.000000 equilibrator-cache-0.5.0b2/versioneer.py
```

### Comparing `equilibrator-cache-0.5.0b1/LICENSE` & `equilibrator-cache-0.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/PKG-INFO` & `equilibrator-cache-0.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
```

### Comparing `equilibrator-cache-0.5.0b1/README.md` & `equilibrator-cache-0.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/setup.cfg` & `equilibrator-cache-0.5.0b2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 	eQuilibrator
 	cache
 
 [options]
 zip_safe = True
 install_requires = 
 	importlib_resources; python_version <'3.9'
-	tqdm~=4.65
-	appdirs~=1.4
-	numpy~=1.25
-	pandas~=2.0
-	python-Levenshtein-wheels~=0.13
-	scipy~=1.11
-	sqlalchemy>=1.3,<1.4
-	pint~=0.22
-	periodictable~=1.6
-	httpx~=0.24
-	tenacity~=6.3
+	sqlalchemy >=1.3,<1.4
+	numpy >=1.13
+	scipy >=1.11
+	pandas ~=1.0
+	python-Levenshtein-wheels ~=0.13
+	pint ~=0.22
+	periodictable ~=1.6
+	httpx ~=0.24
+	tenacity ~=6.3
+	tqdm ~=4.0
+	appdirs ~=1.4
 python_requires = >=3.8
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
```

### Comparing `equilibrator-cache-0.5.0b1/setup.py` & `equilibrator-cache-0.5.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/__init__.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/api.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/api.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/compatibility.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/compound_cache.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/compound_cache.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/exceptions.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/exceptions.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/__init__.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_identifier.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/compound_identifier.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_microspecies.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/compound_microspecies.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/magnesium_dissociation_constant.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/magnesium_dissociation_constant.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/mixins.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/mixins.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/registry.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/models/registry.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/reaction.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/reaction.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/thermodynamic_constants.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/thermodynamic_constants.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache/zenodo.py` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache/zenodo.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/PKG-INFO` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
```

### Comparing `equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/SOURCES.txt` & `equilibrator-cache-0.5.0b2/src/equilibrator_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.5.0b1/versioneer.py` & `equilibrator-cache-0.5.0b2/versioneer.py`

 * *Files identical despite different names*

