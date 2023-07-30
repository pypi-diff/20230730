# Comparing `tmp/xctools_kamaalio-0.0.4.tar.gz` & `tmp/xctools_kamaalio-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xctools_kamaalio-0.0.4.tar", last modified: Sat Jul 29 11:08:21 2023, max compression
+gzip compressed data, was "xctools_kamaalio-0.0.5.tar", last modified: Sun Jul 30 18:33:10 2023, max compression
```

## Comparing `xctools_kamaalio-0.0.4.tar` & `xctools_kamaalio-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.778981 xctools_kamaalio-0.0.4/
--rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-28 18:57:31.000000 xctools_kamaalio-0.0.4/LICENSE
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 11:08:21.778861 xctools_kamaalio-0.0.4/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-28 19:49:50.000000 xctools_kamaalio-0.0.4/README.md
--rw-r--r--   0 kamaal     (503) staff       (20)      653 2023-07-29 11:07:51.000000 xctools_kamaalio-0.0.4/pyproject.toml
--rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-29 11:08:21.779033 xctools_kamaalio-0.0.4/setup.cfg
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.777042 xctools_kamaalio-0.0.4/src/
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.777777 xctools_kamaalio-0.0.4/src/xctools_kamaalio/
--rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-29 11:03:49.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio/__init__.py
--rw-r--r--   0 kamaal     (503) staff       (20)       60 2023-07-29 11:04:53.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio/__main__.py
--rw-r--r--   0 kamaal     (503) staff       (20)       30 2023-07-29 11:03:05.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio/cli.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.778647 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)      349 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/SOURCES.txt
--rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/dependency_links.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/entry_points.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/top_level.txt
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.431031 xctools_kamaalio-0.0.5/
+-rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/LICENSE
+-rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-30 18:33:10.430902 xctools_kamaalio-0.0.5/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/README.md
+-rw-r--r--   0 kamaal     (503) staff       (20)      690 2023-07-30 17:09:34.000000 xctools_kamaalio-0.0.5/pyproject.toml
+-rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-30 18:33:10.431083 xctools_kamaalio-0.0.5/setup.cfg
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.427720 xctools_kamaalio-0.0.5/src/
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.428779 xctools_kamaalio-0.0.5/src/xctools_kamaalio/
+-rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/__init__.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.430670 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/
+-rw-r--r--   0 kamaal     (503) staff       (20)      875 2023-07-30 18:14:33.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/archive.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      340 2023-07-30 18:13:27.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/bump_version.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      358 2023-07-30 18:19:58.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/export_archive.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      496 2023-07-30 18:15:17.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/actions/upload.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      943 2023-07-30 18:15:34.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/cli.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      528 2023-07-30 14:55:07.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/list_utils.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     3470 2023-07-30 17:00:11.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/version_bumper.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     2239 2023-07-30 18:25:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio/xctools.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 18:33:10.429947 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/
+-rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)      636 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/SOURCES.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/dependency_links.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/entry_points.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       13 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/requires.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-30 18:33:10.000000 xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/top_level.txt
```

### Comparing `xctools_kamaalio-0.0.4/LICENSE` & `xctools_kamaalio-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.4/PKG-INFO` & `xctools_kamaalio-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools_kamaalio
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/kamaal111/xctools
 Project-URL: Bug Tracker, https://github.com/kamaal111/xctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/PKG-INFO` & `xctools_kamaalio-0.0.5/src/xctools_kamaalio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools-kamaalio
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/kamaal111/xctools
 Project-URL: Bug Tracker, https://github.com/kamaal111/xctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

