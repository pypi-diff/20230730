# Comparing `tmp/tensorage-0.0.1.tar.gz` & `tmp/tensorage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.1.tar", last modified: Sat Jul 29 17:51:59 2023, max compression
+gzip compressed data, was "tensorage-0.0.2.tar", last modified: Sun Jul 30 05:10:26 2023, max compression
```

## Comparing `tensorage-0.0.1.tar` & `tensorage-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-07-29 17:51:59.438138 tensorage-0.0.1/
--rw-r--r--   0 mirko      (501) staff       (20)    35149 2023-07-29 15:00:46.000000 tensorage-0.0.1/LICENSE
--rw-r--r--   0 mirko      (501) staff       (20)       58 2023-07-29 15:04:38.000000 tensorage-0.0.1/MANIFEST.in
--rw-r--r--   0 mirko      (501) staff       (20)      277 2023-07-29 17:51:59.437977 tensorage-0.0.1/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)       58 2023-07-29 15:00:46.000000 tensorage-0.0.1/README.md
--rw-r--r--   0 mirko      (501) staff       (20)       22 2023-07-29 16:30:42.000000 tensorage-0.0.1/requirements.txt
--rw-r--r--   0 mirko      (501) staff       (20)       38 2023-07-29 17:51:59.438194 tensorage-0.0.1/setup.cfg
--rw-r--r--   0 mirko      (501) staff       (20)      703 2023-07-29 17:51:24.000000 tensorage-0.0.1/setup.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-07-29 17:51:59.436849 tensorage-0.0.1/tensorage/
--rw-r--r--   0 mirko      (501) staff       (20)       64 2023-07-29 16:34:15.000000 tensorage-0.0.1/tensorage/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)       21 2023-07-29 16:34:11.000000 tensorage-0.0.1/tensorage/__version__.py
--rw-r--r--   0 mirko      (501) staff       (20)     2277 2023-07-29 17:33:50.000000 tensorage-0.0.1/tensorage/session.py
--rw-r--r--   0 mirko      (501) staff       (20)      883 2023-07-29 17:44:45.000000 tensorage-0.0.1/tensorage/store.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-07-29 17:51:59.437765 tensorage-0.0.1/tensorage.egg-info/
--rw-r--r--   0 mirko      (501) staff       (20)      277 2023-07-29 17:51:59.000000 tensorage-0.0.1/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)      306 2023-07-29 17:51:59.000000 tensorage-0.0.1/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2023-07-29 17:51:59.000000 tensorage-0.0.1/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 mirko      (501) staff       (20)       23 2023-07-29 17:51:59.000000 tensorage-0.0.1/tensorage.egg-info/requires.txt
--rw-r--r--   0 mirko      (501) staff       (20)       10 2023-07-29 17:51:59.000000 tensorage-0.0.1/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 05:10:26.569426 tensorage-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-30 05:10:15.000000 tensorage-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 05:10:15.000000 tensorage-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 05:10:26.569426 tensorage-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 05:10:15.000000 tensorage-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-30 05:10:15.000000 tensorage-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 05:10:26.569426 tensorage-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-30 05:10:15.000000 tensorage-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 05:10:26.569426 tensorage-0.0.2/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-30 05:10:15.000000 tensorage-0.0.2/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 05:10:26.569426 tensorage-0.0.2/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-30 05:10:26.000000 tensorage-0.0.2/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.1/LICENSE` & `tensorage-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.1/setup.py` & `tensorage-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.1/tensorage/session.py` & `tensorage-0.0.2/tensorage/session.py`

 * *Files identical despite different names*

