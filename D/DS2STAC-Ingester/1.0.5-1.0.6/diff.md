# Comparing `tmp/DS2STAC-Ingester-1.0.5.tar.gz` & `tmp/DS2STAC-Ingester-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DS2STAC-Ingester-1.0.5.tar", last modified: Sun Jul 30 18:51:25 2023, max compression
+gzip compressed data, was "DS2STAC-Ingester-1.0.6.tar", last modified: Sun Jul 30 19:23:43 2023, max compression
```

## Comparing `DS2STAC-Ingester-1.0.5.tar` & `DS2STAC-Ingester-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 18:51:25.269732 DS2STAC-Ingester-1.0.5/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/CONTRIBUTING.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 18:51:25.266013 DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 18:51:25.000000 DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 18:51:25.000000 DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 18:51:25.000000 DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 18:51:25.000000 DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 18:51:25.000000 DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/top_level.txt
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 18:51:25.269838 DS2STAC-Ingester-1.0.5/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 18:51:25.268216 DS2STAC-Ingester-1.0.5/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/docs/usage.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 18:51:25.270646 DS2STAC-Ingester-1.0.5/ds2stac_ingester/
--rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/ds2stac_ingester/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 18:51:25.270686 DS2STAC-Ingester-1.0.5/ds2stac_ingester/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/ds2stac_ingester/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/ds2stac_ingester/config_pgstac.py
--rw-r--r--   0 hadizadeh-m (15144)      901    12403 2023-07-30 18:51:03.000000 DS2STAC-Ingester-1.0.5/ds2stac_ingester/ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1962 2023-07-30 18:51:25.270360 DS2STAC-Ingester-1.0.5/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.5/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 18:51:25.269589 DS2STAC-Ingester-1.0.5/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/tests/test_ds2stac_ingester.py
--rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.5/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 19:23:43.369497 DS2STAC-Ingester-1.0.6/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3707 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/CONTRIBUTING.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 19:23:43.366289 DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 19:23:43.000000 DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      694 2023-07-30 19:23:43.000000 DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-30 19:23:43.000000 DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      462 2023-07-30 19:23:43.000000 DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901       17 2023-07-30 19:23:43.000000 DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/top_level.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      383 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901     2660 2023-07-30 19:23:43.369592 DS2STAC-Ingester-1.0.6/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     1175 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 19:23:43.368108 DS2STAC-Ingester-1.0.6/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      617 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4910 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      304 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1238 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      814 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       87 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/docs/usage.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 19:23:43.370339 DS2STAC-Ingester-1.0.6/ds2stac_ingester/
+-rw-r--r--   0 hadizadeh-m (15144)      901      408 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/ds2stac_ingester/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-30 19:23:43.370378 DS2STAC-Ingester-1.0.6/ds2stac_ingester/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      434 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/ds2stac_ingester/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/ds2stac_ingester/config_pgstac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    12474 2023-07-30 19:20:33.000000 DS2STAC-Ingester-1.0.6/ds2stac_ingester/ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      197 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      136 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1969 2023-07-30 19:23:43.370057 DS2STAC-Ingester-1.0.6/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      447 2023-07-30 10:06:00.000000 DS2STAC-Ingester-1.0.6/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-30 19:23:43.369354 DS2STAC-Ingester-1.0.6/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       46 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1028 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/tests/test_ds2stac_ingester.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    80403 2023-07-30 09:42:47.000000 DS2STAC-Ingester-1.0.6/versioneer.py
```

### Comparing `DS2STAC-Ingester-1.0.5/CONTRIBUTING.rst` & `DS2STAC-Ingester-1.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/PKG-INFO` & `DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-1.0.5/DS2STAC_Ingester.egg-info/SOURCES.txt` & `DS2STAC-Ingester-1.0.6/DS2STAC_Ingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/LICENSE` & `DS2STAC-Ingester-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/PKG-INFO` & `DS2STAC-Ingester-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DS2STAC-Ingester
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python-based module to ingest STAC metadata catalogs into STAC-databases like pgSTAC
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://ds2stac-ingester.readthedocs.io
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/ds2stac_ingester
```

### Comparing `DS2STAC-Ingester-1.0.5/README.rst` & `DS2STAC-Ingester-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/docs/Makefile` & `DS2STAC-Ingester-1.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/docs/conf.py` & `DS2STAC-Ingester-1.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/docs/installation.rst` & `DS2STAC-Ingester-1.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/docs/make.bat` & `DS2STAC-Ingester-1.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/ds2stac_ingester/config_pgstac.py` & `DS2STAC-Ingester-1.0.6/ds2stac_ingester/config_pgstac.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/ds2stac_ingester/ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.6/ds2stac_ingester/ds2stac_ingester.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,13 +312,16 @@
                             "%s : %s" % (ex_type.__name__, ex_value)
                         )
                         continue
         print(
             "collection_json_path.replace(collection.json, )",
             param.replace("/collection.json", "").replace("./", ""),
         )
-        gen_collections = self.db.func(
-            "delete_collection",
-            param.replace("/collection.json", "").replace("./", ""),
-        )
-        for e in gen_collections:
-            print('e',e)
+        try:
+            gen_collections = self.db.func(
+                "delete_collection",
+                param.replace("/collection.json", "").replace("./", ""),
+            )
+            for e in gen_collections:
+                print("e", e)
+        except:
+            pass
```

### Comparing `DS2STAC-Ingester-1.0.5/setup.cfg` & `DS2STAC-Ingester-1.0.6/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 exclude = docs
 ignore = 
 	E203,
 	E402,
 	E501,
 	W503,
 	F541,
+	E722,
 
 [tool:pytest]
 collect_ignore = ['setup.py']
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `DS2STAC-Ingester-1.0.5/tests/test_ds2stac_ingester.py` & `DS2STAC-Ingester-1.0.6/tests/test_ds2stac_ingester.py`

 * *Files identical despite different names*

### Comparing `DS2STAC-Ingester-1.0.5/versioneer.py` & `DS2STAC-Ingester-1.0.6/versioneer.py`

 * *Files identical despite different names*

