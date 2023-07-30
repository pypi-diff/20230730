# Comparing `tmp/tensorage-0.0.2.tar.gz` & `tmp/tensorage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.2.tar", last modified: Sun Jul 30 05:10:26 2023, max compression
+gzip compressed data, was "tensorage-0.0.3.tar", last modified: Sun Jul 30 06:41:21 2023, max compression
```

## Comparing `tensorage-0.0.2.tar` & `tensorage-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 05:10:26.569426 tensorage-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-30 05:10:15.000000 tensorage-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 05:10:15.000000 tensorage-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 05:10:26.569426 tensorage-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 05:10:15.000000 tensorage-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-30 05:10:15.000000 tensorage-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 05:10:26.569426 tensorage-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-30 05:10:15.000000 tensorage-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 05:10:26.569426 tensorage-0.0.2/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 05:10:26.569426 tensorage-0.0.2/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 06:41:21.534192 tensorage-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-30 06:41:11.000000 tensorage-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 06:41:11.000000 tensorage-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 06:41:21.534192 tensorage-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 06:41:11.000000 tensorage-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-30 06:41:11.000000 tensorage-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 06:41:21.534192 tensorage-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-30 06:41:11.000000 tensorage-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 06:41:21.530192 tensorage-0.0.3/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-30 06:41:11.000000 tensorage-0.0.3/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 06:41:11.000000 tensorage-0.0.3/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-30 06:41:11.000000 tensorage-0.0.3/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3067 2023-07-30 06:41:11.000000 tensorage-0.0.3/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-30 06:41:11.000000 tensorage-0.0.3/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 06:41:21.534192 tensorage-0.0.3/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 06:41:21.000000 tensorage-0.0.3/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-30 06:41:21.000000 tensorage-0.0.3/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 06:41:21.000000 tensorage-0.0.3/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 06:41:21.000000 tensorage-0.0.3/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-30 06:41:21.000000 tensorage-0.0.3/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.2/LICENSE` & `tensorage-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.2/setup.py` & `tensorage-0.0.3/setup.py`

 * *Files identical despite different names*

