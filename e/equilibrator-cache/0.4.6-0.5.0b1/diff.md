# Comparing `tmp/equilibrator-cache-0.4.6.tar.gz` & `tmp/equilibrator-cache-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-cache-0.4.6.tar", last modified: Sat Jul 29 14:13:12 2023, max compression
+gzip compressed data, was "equilibrator-cache-0.5.0b1.tar", last modified: Sun Jul 30 03:51:14 2023, max compression
```

## Comparing `equilibrator-cache-0.4.6.tar` & `equilibrator-cache-0.5.0b1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.717951 equilibrator-cache-0.4.6/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-29 14:13:12.717951 equilibrator-cache-0.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-07-29 14:13:12.718951 equilibrator-cache-0.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.710951 equilibrator-cache-0.4.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.718951 equilibrator-cache-0.4.6/src/equilibrator_cache/
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-29 14:13:12.718951 equilibrator-cache-0.4.6/src/equilibrator_cache/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/api.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)    12786 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/compound_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.717951 equilibrator-cache-0.4.6/src/equilibrator_cache/models/
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_identifier.py
--rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_microspecies.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/magnesium_dissociation_constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/models/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/reaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/thermodynamic_constants.py
--rwxrwxrwx   0 root         (0) root         (0)     6740 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/src/equilibrator_cache/zenodo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:13:12.715951 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      406 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:13:12.000000 equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-29 14:13:01.000000 equilibrator-cache-0.4.6/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.454778 equilibrator-cache-0.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-30 03:51:14.454778 equilibrator-cache-0.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-30 03:51:14.455778 equilibrator-cache-0.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.447778 equilibrator-cache-0.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.455778 equilibrator-cache-0.5.0b1/src/equilibrator_cache/
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 03:51:14.455778 equilibrator-cache-0.5.0b1/src/equilibrator_cache/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12832 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/compound_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.454778 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_microspecies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/magnesium_dissociation_constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/thermodynamic_constants.py
+-rwxrwxrwx   0 root         (0) root         (0)     6740 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache/zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 03:51:14.452777 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 03:51:14.000000 equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-30 03:51:02.000000 equilibrator-cache-0.5.0b1/versioneer.py
```

### Comparing `equilibrator-cache-0.4.6/LICENSE` & `equilibrator-cache-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/PKG-INFO` & `equilibrator-cache-0.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.6
+Version: 0.5.0b1
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
```

### Comparing `equilibrator-cache-0.4.6/README.md` & `equilibrator-cache-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/setup.cfg` & `equilibrator-cache-0.5.0b1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -59,18 +59,19 @@
 test = 
 	pytest
 	pytest-cov
 	pytest-raises
 	pytest-mock
 	hypothesis
 development = 
-	black~=23.3
+	black~=23.7
 	isort~=5.12
+	flake8~=6.1
 	safety~=2.3
-	tox~=4.6
+	tox==3.28
 	twine~=4.0
 deployment = 
 	click
 	click-log
 	openbabel
 	python-dateutil
```

### Comparing `equilibrator-cache-0.4.6/setup.py` & `equilibrator-cache-0.5.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/__init__.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/api.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/api.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/compatibility.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/compound_cache.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/compound_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,17 +243,19 @@
 
         atom_bags = {
             compound: compound.atom_bag or {} for compound in compounds
         }
 
         # create the elemental matrix, where each row is a compound and each
         # column is an element (or e-)
-        return pd.DataFrame.from_dict(
-            atom_bags, orient="columns", dtype=int
-        ).fillna(0)
+        return (
+            pd.DataFrame.from_dict(atom_bags, orient="columns", dtype=float)
+            .fillna(0.0)
+            .applymap(int)
+        )
 
     def get_compound_names(self, compound: Compound) -> Set[str]:
         """Return all names for this compound."""
         query = (
             self.session.query(CompoundIdentifier)
             .join(Registry)
             .filter(CompoundIdentifier.compound_id == compound.id)
```

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/exceptions.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/exceptions.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/__init__.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_identifier.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_identifier.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/compound_microspecies.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/compound_microspecies.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/magnesium_dissociation_constant.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/magnesium_dissociation_constant.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/mixins.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/mixins.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/models/registry.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/models/registry.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/reaction.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/reaction.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/thermodynamic_constants.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/thermodynamic_constants.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache/zenodo.py` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache/zenodo.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/PKG-INFO` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.6
+Version: 0.5.0b1
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
```

### Comparing `equilibrator-cache-0.4.6/src/equilibrator_cache.egg-info/SOURCES.txt` & `equilibrator-cache-0.5.0b1/src/equilibrator_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.6/versioneer.py` & `equilibrator-cache-0.5.0b1/versioneer.py`

 * *Files identical despite different names*

