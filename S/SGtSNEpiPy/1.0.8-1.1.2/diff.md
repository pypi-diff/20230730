# Comparing `tmp/SGtSNEpiPy-1.0.8.tar.gz` & `tmp/SGtSNEpiPy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.8.tar", last modified: Sun Jul 30 03:47:29 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.1.2.tar", last modified: Sun Jul 30 04:17:01 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.8.tar` & `SGtSNEpiPy-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.486358 SGtSNEpiPy-1.0.8/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8654 2023-07-30 03:47:29.486465 SGtSNEpiPy-1.0.8/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8261 2023-07-30 03:11:14.000000 SGtSNEpiPy-1.0.8/README.md
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-30 03:47:29.486927 SGtSNEpiPy-1.0.8/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      785 2023-07-30 03:46:32.000000 SGtSNEpiPy-1.0.8/setup.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.484196 SGtSNEpiPy-1.0.8/src/
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.485208 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/SGtSNEpiPy.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/__init__.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 03:47:29.486205 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8654 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-30 03:47:29.000000 SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/top_level.txt
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:17:01.725007 SGtSNEpiPy-1.1.2/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8654 2023-07-30 04:17:01.725119 SGtSNEpiPy-1.1.2/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8261 2023-07-30 03:11:14.000000 SGtSNEpiPy-1.1.2/README.md
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-30 04:17:01.725743 SGtSNEpiPy-1.1.2/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      808 2023-07-30 04:16:34.000000 SGtSNEpiPy-1.1.2/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:17:01.722991 SGtSNEpiPy-1.1.2/src/
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:17:01.724097 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy/SGtSNEpiPy.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy/__init__.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:17:01.724851 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8654 2023-07-30 04:17:01.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-07-30 04:17:01.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-30 04:17:01.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-07-30 04:17:01.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-30 04:17:01.000000 SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/top_level.txt
```

### Comparing `SGtSNEpiPy-1.0.8/PKG-INFO` & `SGtSNEpiPy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.0.8
+Version: 1.1.2
 Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `SGtSNEpiPy-1.0.8/README.md` & `SGtSNEpiPy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `SGtSNEpiPy-1.0.8/src/SGtSNEpiPy/SGtSNEpiPy.py` & `SGtSNEpiPy-1.1.2/src/SGtSNEpiPy/SGtSNEpiPy.py`

 * *Files identical despite different names*

### Comparing `SGtSNEpiPy-1.0.8/src/SGtSNEpiPy.egg-info/PKG-INFO` & `SGtSNEpiPy-1.1.2/src/SGtSNEpiPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.0.8
+Version: 1.1.2
 Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

