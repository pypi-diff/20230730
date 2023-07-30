# Comparing `tmp/hyko_sdk-0.3.0b0.tar.gz` & `tmp/hyko_sdk-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.3.0b0.tar", last modified: Sun Jul 30 13:40:56 2023, max compression
+gzip compressed data, was "hyko_sdk-0.3.0b1.tar", last modified: Sun Jul 30 15:05:20 2023, max compression
```

## Comparing `hyko_sdk-0.3.0b0.tar` & `hyko_sdk-0.3.0b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-30 13:40:56.216326 hyko_sdk-0.3.0b0/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-07-30 13:40:56.216326 hyko_sdk-0.3.0b0/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.3.0b0/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-30 13:40:56.212993 hyko_sdk-0.3.0b0/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b0/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b0/hyko_sdk/error.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    18854 2023-07-27 12:46:37.000000 hyko_sdk-0.3.0b0/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1160 2023-07-27 15:29:23.000000 hyko_sdk-0.3.0b0/hyko_sdk/metadata.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b0/hyko_sdk/utils.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-30 13:40:56.216326 hyko_sdk-0.3.0b0/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-07-30 13:40:56.000000 hyko_sdk-0.3.0b0/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-07-30 13:40:56.000000 hyko_sdk-0.3.0b0/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-07-30 13:40:56.000000 hyko_sdk-0.3.0b0/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       54 2023-07-30 13:40:56.000000 hyko_sdk-0.3.0b0/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-07-30 13:40:56.000000 hyko_sdk-0.3.0b0/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b0/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      381 2023-07-30 13:40:56.216326 hyko_sdk-0.3.0b0/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-30 15:05:20.571755 hyko_sdk-0.3.0b1/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-07-30 15:05:20.571755 hyko_sdk-0.3.0b1/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.3.0b1/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-30 15:05:20.571755 hyko_sdk-0.3.0b1/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b1/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b1/hyko_sdk/error.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    18854 2023-07-27 12:46:37.000000 hyko_sdk-0.3.0b1/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1402 2023-07-30 15:01:20.000000 hyko_sdk-0.3.0b1/hyko_sdk/metadata.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b1/hyko_sdk/utils.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-30 15:05:20.571755 hyko_sdk-0.3.0b1/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-07-30 15:05:20.000000 hyko_sdk-0.3.0b1/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-07-30 15:05:20.000000 hyko_sdk-0.3.0b1/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-07-30 15:05:20.000000 hyko_sdk-0.3.0b1/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       54 2023-07-30 15:05:20.000000 hyko_sdk-0.3.0b1/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-07-30 15:05:20.000000 hyko_sdk-0.3.0b1/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b1/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      381 2023-07-30 15:05:20.575088 hyko_sdk-0.3.0b1/setup.cfg
```

### Comparing `hyko_sdk-0.3.0b0/hyko_sdk/error.py` & `hyko_sdk-0.3.0b1/hyko_sdk/error.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b0/hyko_sdk/io.py` & `hyko_sdk-0.3.0b1/hyko_sdk/io.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b0/hyko_sdk/utils.py` & `hyko_sdk-0.3.0b1/hyko_sdk/utils.py`

 * *Files identical despite different names*

