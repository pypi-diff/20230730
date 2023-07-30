# Comparing `tmp/switchblade-0.0.4.tar.gz` & `tmp/switchblade-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switchblade-0.0.4.tar", last modified: Fri Jul 21 18:43:52 2023, max compression
+gzip compressed data, was "switchblade-0.0.5.tar", last modified: Sun Jul 30 01:02:03 2023, max compression
```

## Comparing `switchblade-0.0.4.tar` & `switchblade-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-21 18:43:52.523076 switchblade-0.0.4/
--rw-r--r--   0 oriyonay   (501) staff       (20)     1066 2023-03-07 22:38:54.000000 switchblade-0.0.4/LICENSE
--rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-21 18:43:52.522736 switchblade-0.0.4/PKG-INFO
--rw-r--r--   0 oriyonay   (501) staff       (20)      177 2023-03-07 23:09:24.000000 switchblade-0.0.4/README.md
--rw-r--r--   0 oriyonay   (501) staff       (20)      590 2023-07-21 18:41:03.000000 switchblade-0.0.4/pyproject.toml
--rw-r--r--   0 oriyonay   (501) staff       (20)       38 2023-07-21 18:43:52.523320 switchblade-0.0.4/setup.cfg
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-21 18:43:52.517389 switchblade-0.0.4/src/
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-21 18:43:52.520738 switchblade-0.0.4/src/switchblade/
--rw-r--r--   0 oriyonay   (501) staff       (20)        4 2023-03-07 22:39:57.000000 switchblade-0.0.4/src/switchblade/__init__.py
--rw-r--r--   0 oriyonay   (501) staff       (20)      425 2023-07-21 18:23:56.000000 switchblade-0.0.4/src/switchblade/debugging.py
--rw-r--r--   0 oriyonay   (501) staff       (20)      540 2023-03-07 22:43:17.000000 switchblade-0.0.4/src/switchblade/logging.py
--rw-r--r--   0 oriyonay   (501) staff       (20)       30 2023-03-07 22:43:42.000000 switchblade-0.0.4/src/switchblade/modules.py
--rw-r--r--   0 oriyonay   (501) staff       (20)     2550 2023-07-21 18:39:35.000000 switchblade-0.0.4/src/switchblade/utils.py
-drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-21 18:43:52.522126 switchblade-0.0.4/src/switchblade.egg-info/
--rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-21 18:43:52.000000 switchblade-0.0.4/src/switchblade.egg-info/PKG-INFO
--rw-r--r--   0 oriyonay   (501) staff       (20)      324 2023-07-21 18:43:52.000000 switchblade-0.0.4/src/switchblade.egg-info/SOURCES.txt
--rw-r--r--   0 oriyonay   (501) staff       (20)        1 2023-07-21 18:43:52.000000 switchblade-0.0.4/src/switchblade.egg-info/dependency_links.txt
--rw-r--r--   0 oriyonay   (501) staff       (20)       12 2023-07-21 18:43:52.000000 switchblade-0.0.4/src/switchblade.egg-info/top_level.txt
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.286813 switchblade-0.0.5/
+-rw-r--r--   0 oriyonay   (501) staff       (20)     1066 2023-07-30 01:00:20.000000 switchblade-0.0.5/LICENSE
+-rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-30 01:02:03.286475 switchblade-0.0.5/PKG-INFO
+-rw-r--r--   0 oriyonay   (501) staff       (20)      177 2023-07-30 01:00:20.000000 switchblade-0.0.5/README.md
+-rw-r--r--   0 oriyonay   (501) staff       (20)      590 2023-07-30 01:01:16.000000 switchblade-0.0.5/pyproject.toml
+-rw-r--r--   0 oriyonay   (501) staff       (20)       38 2023-07-30 01:02:03.286940 switchblade-0.0.5/setup.cfg
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.278543 switchblade-0.0.5/src/
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.282289 switchblade-0.0.5/src/switchblade/
+-rw-r--r--   0 oriyonay   (501) staff       (20)        4 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/__init__.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)      425 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/debugging.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)      540 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/logging.py
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.286087 switchblade-0.0.5/src/switchblade/modules/
+-rw-r--r--   0 oriyonay   (501) staff       (20)     3747 2023-07-29 23:03:04.000000 switchblade-0.0.5/src/switchblade/modules/ResNetIA.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)       30 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/modules/__init__.py
+-rw-r--r--   0 oriyonay   (501) staff       (20)     2550 2023-07-30 01:00:20.000000 switchblade-0.0.5/src/switchblade/utils.py
+drwxr-xr-x   0 oriyonay   (501) staff       (20)        0 2023-07-30 01:02:03.285339 switchblade-0.0.5/src/switchblade.egg-info/
+-rw-r--r--   0 oriyonay   (501) staff       (20)      692 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/PKG-INFO
+-rw-r--r--   0 oriyonay   (501) staff       (20)      369 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/SOURCES.txt
+-rw-r--r--   0 oriyonay   (501) staff       (20)        1 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/dependency_links.txt
+-rw-r--r--   0 oriyonay   (501) staff       (20)       12 2023-07-30 01:02:03.000000 switchblade-0.0.5/src/switchblade.egg-info/top_level.txt
```

### Comparing `switchblade-0.0.4/LICENSE` & `switchblade-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `switchblade-0.0.4/PKG-INFO` & `switchblade-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchblade
-Version: 0.0.4
+Version: 0.0.5
 Summary: Deep learning utilities for PyTorch
 Author-email: Ori Yonay <oriyonay12@gmail.com>
 Project-URL: Homepage, https://github.com/oriyonay/switchblade
 Project-URL: Bug Tracker, https://github.com/oriyonay/switchblade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `switchblade-0.0.4/pyproject.toml` & `switchblade-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "switchblade"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ori Yonay", email="oriyonay12@gmail.com" },
 ]
 description = "Deep learning utilities for PyTorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `switchblade-0.0.4/src/switchblade/logging.py` & `switchblade-0.0.5/src/switchblade/logging.py`

 * *Files identical despite different names*

### Comparing `switchblade-0.0.4/src/switchblade/utils.py` & `switchblade-0.0.5/src/switchblade/utils.py`

 * *Files identical despite different names*

### Comparing `switchblade-0.0.4/src/switchblade.egg-info/PKG-INFO` & `switchblade-0.0.5/src/switchblade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchblade
-Version: 0.0.4
+Version: 0.0.5
 Summary: Deep learning utilities for PyTorch
 Author-email: Ori Yonay <oriyonay12@gmail.com>
 Project-URL: Homepage, https://github.com/oriyonay/switchblade
 Project-URL: Bug Tracker, https://github.com/oriyonay/switchblade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

