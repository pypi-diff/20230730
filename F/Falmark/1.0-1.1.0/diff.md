# Comparing `tmp/Falmark-1.0.tar.gz` & `tmp/Falmark-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Falmark-1.0.tar", last modified: Wed Jul 26 03:10:45 2023, max compression
+gzip compressed data, was "Falmark-1.1.0.tar", last modified: Sun Jul 30 16:09:17 2023, max compression
```

## Comparing `Falmark-1.0.tar` & `Falmark-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-07-26 03:10:45.468000 Falmark-1.0/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-07-26 03:10:45.466570 Falmark-1.0/Falmark/
--rw-r--r--   0 owner      (501) staff       (20)        0 2023-07-26 02:15:31.000000 Falmark-1.0/Falmark/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-07-26 03:10:45.467583 Falmark-1.0/Falmark.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)       49 2023-07-26 03:10:45.000000 Falmark-1.0/Falmark.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      228 2023-07-26 03:10:45.000000 Falmark-1.0/Falmark.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-07-26 03:10:45.000000 Falmark-1.0/Falmark.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)       42 2023-07-26 03:10:45.000000 Falmark-1.0/Falmark.egg-info/entry_points.txt
--rw-r--r--   0 owner      (501) staff       (20)        9 2023-07-26 03:10:45.000000 Falmark-1.0/Falmark.egg-info/requires.txt
--rw-r--r--   0 owner      (501) staff       (20)       17 2023-07-26 03:10:45.000000 Falmark-1.0/Falmark.egg-info/top_level.txt
--rw-r--r--   0 owner      (501) staff       (20)       49 2023-07-26 03:10:45.467821 Falmark-1.0/PKG-INFO
--rwxr-xr-x   0 owner      (501) staff       (20)     7584 2023-07-03 01:44:24.000000 Falmark-1.0/falmark4.py
--rw-r--r--   0 owner      (501) staff       (20)       38 2023-07-26 03:10:45.468056 Falmark-1.0/setup.cfg
--rw-r--r--   0 owner      (501) staff       (20)      449 2023-07-26 02:07:11.000000 Falmark-1.0/setup.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-07-30 16:09:17.803181 Falmark-1.1.0/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-07-30 16:09:17.801760 Falmark-1.1.0/Falmark/
+-rw-r--r--   0 owner      (501) staff       (20)        0 2023-07-26 02:15:31.000000 Falmark-1.1.0/Falmark/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-07-30 16:09:17.802756 Falmark-1.1.0/Falmark.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)       51 2023-07-30 16:09:17.000000 Falmark-1.1.0/Falmark.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      228 2023-07-30 16:09:17.000000 Falmark-1.1.0/Falmark.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-07-30 16:09:17.000000 Falmark-1.1.0/Falmark.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)       42 2023-07-30 16:09:17.000000 Falmark-1.1.0/Falmark.egg-info/entry_points.txt
+-rw-r--r--   0 owner      (501) staff       (20)       21 2023-07-30 16:09:17.000000 Falmark-1.1.0/Falmark.egg-info/requires.txt
+-rw-r--r--   0 owner      (501) staff       (20)       17 2023-07-30 16:09:17.000000 Falmark-1.1.0/Falmark.egg-info/top_level.txt
+-rw-r--r--   0 owner      (501) staff       (20)       51 2023-07-30 16:09:17.802995 Falmark-1.1.0/PKG-INFO
+-rwxr-xr-x   0 owner      (501) staff       (20)     7584 2023-07-03 01:44:24.000000 Falmark-1.1.0/falmark4.py
+-rw-r--r--   0 owner      (501) staff       (20)       38 2023-07-30 16:09:17.803243 Falmark-1.1.0/setup.cfg
+-rw-r--r--   0 owner      (501) staff       (20)      463 2023-07-30 16:07:43.000000 Falmark-1.1.0/setup.py
```

### Comparing `Falmark-1.0/falmark4.py` & `Falmark-1.1.0/falmark4.py`

 * *Files identical despite different names*

