# Comparing `tmp/fshare-1.1.1.tar.gz` & `tmp/fshare-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fshare-1.1.1.tar", last modified: Sun Jul 30 15:46:40 2023, max compression
+gzip compressed data, was "fshare-1.1.2.tar", last modified: Sun Jul 30 15:49:55 2023, max compression
```

## Comparing `fshare-1.1.1.tar` & `fshare-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:46:40.437017 fshare-1.1.1/
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3967 2023-07-30 15:46:40.436017 fshare-1.1.1/PKG-INFO
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3260 2023-07-30 15:14:46.000000 fshare-1.1.1/README.md
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1034 2023-07-30 15:46:02.000000 fshare-1.1.1/pyproject.toml
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       38 2023-07-30 15:46:40.437017 fshare-1.1.1/setup.cfg
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:46:40.433017 fshare-1.1.1/src/
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:46:40.435017 fshare-1.1.1/src/fshare/
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       30 2023-07-29 20:52:17.000000 fshare-1.1.1/src/fshare/__init__.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       60 2023-07-30 14:52:01.000000 fshare-1.1.1/src/fshare/__main__.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      740 2023-07-30 14:56:26.000000 fshare-1.1.1/src/fshare/cli.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1636 2023-07-28 22:50:43.000000 fshare-1.1.1/src/fshare/filemanager.py
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3205 2023-07-28 22:46:37.000000 fshare-1.1.1/src/fshare/index.html
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      715 2023-07-28 22:35:20.000000 fshare-1.1.1/src/fshare/index.js
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1707 2023-07-30 14:51:23.000000 fshare-1.1.1/src/fshare/main.py
-drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:46:40.436017 fshare-1.1.1/src/fshare.egg-info/
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3967 2023-07-30 15:46:40.000000 fshare-1.1.1/src/fshare.egg-info/PKG-INFO
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      311 2023-07-30 15:46:40.000000 fshare-1.1.1/src/fshare.egg-info/SOURCES.txt
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        1 2023-07-30 15:46:40.000000 fshare-1.1.1/src/fshare.egg-info/dependency_links.txt
--rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        7 2023-07-30 15:46:40.000000 fshare-1.1.1/src/fshare.egg-info/top_level.txt
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:49:55.143548 fshare-1.1.2/
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3967 2023-07-30 15:49:55.143548 fshare-1.1.2/PKG-INFO
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3260 2023-07-30 15:14:46.000000 fshare-1.1.2/README.md
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1066 2023-07-30 15:49:43.000000 fshare-1.1.2/pyproject.toml
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       38 2023-07-30 15:49:55.143548 fshare-1.1.2/setup.cfg
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:49:55.138548 fshare-1.1.2/src/
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:49:55.141548 fshare-1.1.2/src/fshare/
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       30 2023-07-29 20:52:17.000000 fshare-1.1.2/src/fshare/__init__.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)       60 2023-07-30 14:52:01.000000 fshare-1.1.2/src/fshare/__main__.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      740 2023-07-30 14:56:26.000000 fshare-1.1.2/src/fshare/cli.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1636 2023-07-28 22:50:43.000000 fshare-1.1.2/src/fshare/filemanager.py
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3205 2023-07-28 22:46:37.000000 fshare-1.1.2/src/fshare/index.html
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      715 2023-07-28 22:35:20.000000 fshare-1.1.2/src/fshare/index.js
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     1707 2023-07-30 14:51:23.000000 fshare-1.1.2/src/fshare/main.py
+drwxr-xr-x   0 stevomitric  (1000) stevomitric  (1000)        0 2023-07-30 15:49:55.142548 fshare-1.1.2/src/fshare.egg-info/
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)     3967 2023-07-30 15:49:55.000000 fshare-1.1.2/src/fshare.egg-info/PKG-INFO
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)      311 2023-07-30 15:49:55.000000 fshare-1.1.2/src/fshare.egg-info/SOURCES.txt
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        1 2023-07-30 15:49:55.000000 fshare-1.1.2/src/fshare.egg-info/dependency_links.txt
+-rw-r--r--   0 stevomitric  (1000) stevomitric  (1000)        7 2023-07-30 15:49:55.000000 fshare-1.1.2/src/fshare.egg-info/top_level.txt
```

### Comparing `fshare-1.1.1/PKG-INFO` & `fshare-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fshare
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python package that serves as an easy file sharing application over local network
 Author-email: Stevo Mitric <stevomitric2000@gmail.com>
 Maintainer-email: Stevo Mitric <stevomitric2000@gmail.com>
 Project-URL: Homepage, https://github.com/stevomitric/fshare
 Project-URL: Bug Tracker, https://github.com/stevomitric/fshare/issues
 Keywords: file,share
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fshare-1.1.1/README.md` & `fshare-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fshare-1.1.1/pyproject.toml` & `fshare-1.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fshare"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Stevo Mitric", email="stevomitric2000@gmail.com" },
 ]
 maintainers = [
   { name="Stevo Mitric", email="stevomitric2000@gmail.com" },
 ]
 description = "A python package that serves as an easy file sharing application over local network"
@@ -31,11 +31,11 @@
 include-package-data = true
 
 [tool.setuptools.package-data]
 where = ["src"]
 fshare = ["*.html", "*.js"]
 
 [tool.poetry.dependencies]
-flask = "*"
+flask = { version = "*", python = ">=3.0" }
 
 [tool.poetry.scripts]
 fshare = 'fshare.main:run'
```

### Comparing `fshare-1.1.1/src/fshare/cli.py` & `fshare-1.1.2/src/fshare/cli.py`

 * *Files identical despite different names*

### Comparing `fshare-1.1.1/src/fshare/filemanager.py` & `fshare-1.1.2/src/fshare/filemanager.py`

 * *Files identical despite different names*

### Comparing `fshare-1.1.1/src/fshare/index.html` & `fshare-1.1.2/src/fshare/index.html`

 * *Files identical despite different names*

### Comparing `fshare-1.1.1/src/fshare/index.js` & `fshare-1.1.2/src/fshare/index.js`

 * *Files identical despite different names*

### Comparing `fshare-1.1.1/src/fshare/main.py` & `fshare-1.1.2/src/fshare/main.py`

 * *Files identical despite different names*

### Comparing `fshare-1.1.1/src/fshare.egg-info/PKG-INFO` & `fshare-1.1.2/src/fshare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fshare
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python package that serves as an easy file sharing application over local network
 Author-email: Stevo Mitric <stevomitric2000@gmail.com>
 Maintainer-email: Stevo Mitric <stevomitric2000@gmail.com>
 Project-URL: Homepage, https://github.com/stevomitric/fshare
 Project-URL: Bug Tracker, https://github.com/stevomitric/fshare/issues
 Keywords: file,share
 Classifier: Programming Language :: Python :: 3
```

