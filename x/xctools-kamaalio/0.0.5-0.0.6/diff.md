# Comparing `tmp/xctools_kamaalio-0.0.5.tar.gz` & `tmp/xctools_kamaalio-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xctools_kamaalio-0.0.5.tar", last modified: Sun Jul 30 18:33:10 2023, max compression
+gzip compressed data, was "xctools_kamaalio-0.0.6.tar", last modified: Sun Jul 30 19:04:52 2023, max compression
```

## Comparing `xctools_kamaalio-0.0.5.tar` & `xctools_kamaalio-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.431031 xctools_kamaalio-0.0.5/
--rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/LICENSE
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-30 18:33:10.430902 xctools_kamaalio-0.0.5/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/README.md
--rw-r--r--   0 kamaal     (503) staff       (20)      690 2023-07-30 17:09:34.000000 xctools_kamaalio-0.0.5/pyproject.toml
--rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-30 18:33:10.431083 xctools_kamaalio-0.0.5/setup.cfg
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.427720 xctools_kamaalio-0.0.5/src/
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.428779 xctools_kamaalio-0.0.5/src/xctools_kamaalio/
--rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/__init__.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.430670 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/
--rw-r--r--   0 kamaal     (503) staff       (20)      875 2023-07-30 18:14:33.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/archive.py
--rw-r--r--   0 kamaal     (503) staff       (20)      340 2023-07-30 18:13:27.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/bump_version.py
--rw-r--r--   0 kamaal     (503) staff       (20)      358 2023-07-30 18:19:58.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/export_archive.py
--rw-r--r--   0 kamaal     (503) staff       (20)      496 2023-07-30 18:15:17.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/upload.py
--rw-r--r--   0 kamaal     (503) staff       (20)      943 2023-07-30 18:15:34.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/cli.py
--rw-r--r--   0 kamaal     (503) staff       (20)      528 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/list_utils.py
--rw-r--r--   0 kamaal     (503) staff       (20)     3470 2023-07-30 17:00:11.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/version_bumper.py
--rw-r--r--   0 kamaal     (503) staff       (20)     2239 2023-07-30 18:25:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/xctools.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.429947 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)      636 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/SOURCES.txt
--rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/dependency_links.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/entry_points.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       13 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/requires.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/top_level.txt
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.379246 xctools_kamaalio-0.0.6/
+-rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/LICENSE
+-rw-r--r--   0 kamaal     (503) staff       (20)      532 2023-07-30 19:04:52.379135 xctools_kamaalio-0.0.6/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/README.md
+-rw-r--r--   0 kamaal     (503) staff       (20)      688 2023-07-30 19:04:14.000000 xctools_kamaalio-0.0.6/pyproject.toml
+-rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-30 19:04:52.379292 xctools_kamaalio-0.0.6/setup.cfg
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.376607 xctools_kamaalio-0.0.6/src/
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.377619 xctools_kamaalio-0.0.6/src/xctools_kamaalio/
+-rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/__init__.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.378970 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/
+-rw-r--r--   0 kamaal     (503) staff       (20)      875 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/archive.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      340 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/bump_version.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      358 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/export_archive.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      496 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/upload.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      943 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/cli.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      528 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/list_utils.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     3470 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/version_bumper.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     2239 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/xctools.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.378428 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/
+-rw-r--r--   0 kamaal     (503) staff       (20)      532 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)      636 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/SOURCES.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/dependency_links.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/entry_points.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       13 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/requires.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/top_level.txt
```

### Comparing `xctools_kamaalio-0.0.5/LICENSE` & `xctools_kamaalio-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.5/pyproject.toml` & `xctools_kamaalio-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 [project.scripts]
 xctools = "xctools_kamaalio:cli.cli"
 
 
 [project]
 name = "xctools_kamaalio"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "Kamaal Farah", email = "kamaal.f1@gmail.com" }]
 description = "A package to help deal with Xcode projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["click >= 8.1.6"]
 
 
 [project.urls]
-"Homepage" = "https://github.com/kamaal111/xctools"
-"Bug Tracker" = "https://github.com/kamaal111/xctools/issues"
+"Homepage" = "https://github.com/Kamaalio/XcTools"
+"Bug Tracker" = "https://github.com/Kamaalio/XcTools/issues"
```

### Comparing `xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/archive.py` & `xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/archive.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.5/src/xctools_kamaalio/cli.py` & `xctools_kamaalio-0.0.6/src/xctools_kamaalio/cli.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.5/src/xctools_kamaalio/list_utils.py` & `xctools_kamaalio-0.0.6/src/xctools_kamaalio/list_utils.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.5/src/xctools_kamaalio/version_bumper.py` & `xctools_kamaalio-0.0.6/src/xctools_kamaalio/version_bumper.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.5/src/xctools_kamaalio/xctools.py` & `xctools_kamaalio-0.0.6/src/xctools_kamaalio/xctools.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/SOURCES.txt` & `xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

