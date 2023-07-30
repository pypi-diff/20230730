# Comparing `tmp/DS2STAC-Ingester-1.0.1.tar.gz` & `tmp/DS2STAC-Ingester-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DS2STAC-Ingester-1.0.1.tar", last modified: Sun Jul 30 10:28:00 2023, max compression
+gzip compressed data, was "DS2STAC-Ingester-1.0.2.tar", last modified: Sun Jul 30 10:40:10 2023, max compression
```

## Comparing `DS2STAC-Ingester-1.0.1.tar` & `DS2STAC-Ingester-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.842276 DS2STAC-Ingester-1.0.1/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/CONTRIBUTING.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.839311 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 10:28:00.000000 DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/top_level.txt
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:28:00.842372 DS2STAC-Ingester-1.0.1/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.840986 DS2STAC-Ingester-1.0.1/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/docs/usage.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.843060 DS2STAC-Ingester-1.0.1/ds2stac_ingester/
--rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 10:28:00.843098 DS2STAC-Ingester-1.0.1/ds2stac_ingester/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/config_pgstac.py
--rw-r--r--   0 hadizadeh-m (15144)      901     6090 2023-07-30 10:27:14.000000 DS2STAC-Ingester-1.0.1/ds2stac_ingester/ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1962 2023-07-30 10:28:00.842785 DS2STAC-Ingester-1.0.1/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.1/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:28:00.842045 DS2STAC-Ingester-1.0.1/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/tests/test_ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.1/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:40:10.860595 DS2STAC-Ingester-1.0.2/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/CONTRIBUTING.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:40:10.857485 DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:40:10.000000 DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 10:40:10.000000 DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 10:40:10.000000 DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 10:40:10.000000 DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 10:40:10.000000 DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/top_level.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 10:40:10.860677 DS2STAC-Ingester-1.0.2/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:40:10.859347 DS2STAC-Ingester-1.0.2/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/docs/usage.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:40:10.861321 DS2STAC-Ingester-1.0.2/ds2stac_ingester/
+-rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/ds2stac_ingester/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 10:40:10.861358 DS2STAC-Ingester-1.0.2/ds2stac_ingester/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/ds2stac_ingester/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/ds2stac_ingester/config_pgstac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     6090 2023-07-30 10:38:25.000000 DS2STAC-Ingester-1.0.2/ds2stac_ingester/ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1962 2023-07-30 10:40:10.861080 DS2STAC-Ingester-1.0.2/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.2/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 10:40:10.860434 DS2STAC-Ingester-1.0.2/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/tests/test_ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.2/versioneer.py
```

### Comparing `DS2STAC-Ingester-1.0.1/CONTRIBUTING.rst` & `DS2STAC-Ingester-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/PKG-INFO` & `DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-1.0.1/DS2STAC_Ingester.egg-info/SOURCES.txt` & `DS2STAC-Ingester-1.0.2/DS2STAC_Ingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/LICENSE` & `DS2STAC-Ingester-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/PKG-INFO` & `DS2STAC-Ingester-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-1.0.1/README.rst` & `DS2STAC-Ingester-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/docs/Makefile` & `DS2STAC-Ingester-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/docs/conf.py` & `DS2STAC-Ingester-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/docs/installation.rst` & `DS2STAC-Ingester-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/docs/make.bat` & `DS2STAC-Ingester-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/ds2stac_ingester/config_pgstac.py` & `DS2STAC-Ingester-1.0.2/ds2stac_ingester/config_pgstac.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/ds2stac_ingester/ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.2/ds2stac_ingester/ds2stac_ingester.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                             "%s : %s" % (ex_type.__name__, ex_value)
                         )
                         continue
         else:
             item_collection_list = []  # Considered empty to prevent recursion
             loaderx.load_collections(
                 str(os.path.join(stac_dirx, collection_josn_path)),
-                Methods.insert,
+                Methods.upsert,
             )
             print(param)
             for ci in collection_josn_data["links"]:
                 if ci["rel"] == "item":
                     try:
                         loaderx.load_items(
                             str(
@@ -141,15 +141,15 @@
                                     stac_dirx,
                                     collection_josn_path.replace(
                                         "collection.json", "/"
                                     )
                                     + ci["href"].replace("./", ""),
                                 )
                             ),
-                            Methods.insert,
+                            Methods.upsert,
                         )
                         print("|____", ci["href"])
                     except Exception:
                         (
                             ex_type,
                             ex_value,
                             ex_traceback,
```

### Comparing `DS2STAC-Ingester-1.0.1/setup.cfg` & `DS2STAC-Ingester-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/tests/test_ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.2/tests/test_ds2stac_ingester.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.1/versioneer.py` & `DS2STAC-Ingester-1.0.2/versioneer.py`

 * *Files identical despite different names*

