# Comparing `tmp/SGtSNEpiPy-1.0.7.tar.gz` & `tmp/SGtSNEpiPy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.7.tar", last modified: Fri Jul 28 17:37:48 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.0.8.tar", last modified: Sun Jul 30 03:47:29 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.7.tar` & `SGtSNEpiPy-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-28 17:37:48.122972 SGtSNEpiPy-1.0.7/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-28 17:37:48.123089 SGtSNEpiPy-1.0.7/PKG-INFO
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-28 17:37:48.121786 SGtSNEpiPy-1.0.7/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy/SGtSNEpiPy.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy/__init__.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-28 17:37:48.122805 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      235 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/top_level.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-28 17:37:48.123406 SGtSNEpiPy-1.0.7/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      830 2023-07-28 17:34:53.000000 SGtSNEpiPy-1.0.7/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.486358 SGtSNEpiPy-1.0.8/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8654 2023-07-30 03:47:29.486465 SGtSNEpiPy-1.0.8/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8261 2023-07-30 03:11:14.000000 SGtSNEpiPy-1.0.8/README.md
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-30 03:47:29.486927 SGtSNEpiPy-1.0.8/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      785 2023-07-30 03:46:32.000000 SGtSNEpiPy-1.0.8/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.484196 SGtSNEpiPy-1.0.8/src/
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.485208 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/SGtSNEpiPy.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/__init__.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.486205 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8654 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/top_level.txt
```

### Comparing `SGtSNEpiPy-1.0.7/SGtSNEpiPy/SGtSNEpiPy.py` & `SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/SGtSNEpiPy.py`

 * *Files identical despite different names*

