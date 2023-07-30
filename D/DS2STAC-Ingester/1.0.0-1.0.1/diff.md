# Comparing `tmp/DS2STAC-Ingester-1.0.0.tar.gz` & `tmp/DS2STAC-Ingester-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DS2STAC-Ingester-1.0.0.tar", last modified: Sun Jul 30 10:07:43 2023, max compression
+gzip compressed data, was "DS2STAC-Ingester-1.0.1.tar", last modified: Sun Jul 30 10:28:00 2023, max compression
```

## Comparing `DS2STAC-Ingester-1.0.0.tar` & `DS2STAC-Ingester-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.879797 DS2STAC-Ingester-1.0.0/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/CONTRIBUTING.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.877569 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 10:07:43.000000 DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/top_level.txt
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:07:43.879880 DS2STAC-Ingester-1.0.0/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.878814 DS2STAC-Ingester-1.0.0/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/docs/usage.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.880421 DS2STAC-Ingester-1.0.0/ds2stac_ingester/
--rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 10:07:43.880452 DS2STAC-Ingester-1.0.0/ds2stac_ingester/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/config_pgstac.py
--rw-r--r--   0 hadizadeh-m (15144)      901     6011 2023-07-30 10:03:14.000000 DS2STAC-Ingester-1.0.0/ds2stac_ingester/ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1962 2023-07-30 10:07:43.880269 DS2STAC-Ingester-1.0.0/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.0/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:07:43.879687 DS2STAC-Ingester-1.0.0/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/tests/test_ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.0/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.842276 DS2STAC-Ingester-1.0.1/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/CONTRIBUTING.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.839311 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/top_level.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:28:00.842372 DS2STAC-Ingester-1.0.1/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.840986 DS2STAC-Ingester-1.0.1/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/usage.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.843060 DS2STAC-Ingester-1.0.1/ds2stac_ingester/
+-rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 10:28:00.843098 DS2STAC-Ingester-1.0.1/ds2stac_ingester/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/config_pgstac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     6090 2023-07-30 10:27:14.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1962 2023-07-30 10:28:00.842785 DS2STAC-Ingester-1.0.1/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.1/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.842045 DS2STAC-Ingester-1.0.1/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/tests/test_ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/versioneer.py
```

### Comparing `DS2STAC-Ingester-1.0.0/CONTRIBUTING.rst` & `DS2STAC-Ingester-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/PKG-INFO` & `DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-1.0.0/DS2STAC_Ingester.egg-info/SOURCES.txt` & `DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/LICENSE` & `DS2STAC-Ingester-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/PKG-INFO` & `DS2STAC-Ingester-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-1.0.0/README.rst` & `DS2STAC-Ingester-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/docs/Makefile` & `DS2STAC-Ingester-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/docs/conf.py` & `DS2STAC-Ingester-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/docs/installation.rst` & `DS2STAC-Ingester-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/docs/make.bat` & `DS2STAC-Ingester-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/ds2stac_ingester/config_pgstac.py` & `DS2STAC-Ingester-1.0.1/ds2stac_ingester/config_pgstac.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/ds2stac_ingester/ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.1/ds2stac_ingester/ds2stac_ingester.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
                     self.ingest(
                         loader,
                         dc["href"],
                         stac_dir,
                         "stac/" + dc["href"].replace("./", ""),
                     )
         self.logger.info("Ingesting catalogs is finished")
+        self.logger.info("Job finished successfully! STAC catalog is created")
 
     def ingest(self, loaderx, param, stac_dirx, address_coll):
         """This is a function for ingesting collections
         into pgSTAC specifically for nested datasets"""
 
         f = open(os.path.join(stac_dirx, address_coll))
         collection_josn_path = os.path.join(stac_dirx, address_coll)
```

### Comparing `DS2STAC-Ingester-1.0.0/setup.cfg` & `DS2STAC-Ingester-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/tests/test_ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.1/tests/test_ds2stac_ingester.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.0/versioneer.py` & `DS2STAC-Ingester-1.0.1/versioneer.py`

 * *Files identical despite different names*

