# Comparing `tmp/opet-0.0.3.tar.gz` & `tmp/opet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opet-0.0.3.tar", last modified: Sun Jul 30 15:45:33 2023, max compression
+gzip compressed data, was "opet-0.0.4.tar", last modified: Sun Jul 30 15:55:27 2023, max compression
```

## Comparing `opet-0.0.3.tar` & `opet-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 15:45:33.821071 opet-0.0.3/
--rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.3/LICENSE
--rw-r--r--   0 btcyz255   (501) staff       (20)      565 2023-07-30 15:45:33.820809 opet-0.0.3/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)       91 2023-07-30 13:14:54.000000 opet-0.0.3/README.md
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 15:45:33.818164 opet-0.0.3/opet/
--rw-r--r--   0 btcyz255   (501) staff       (20)        0 2023-07-30 13:15:36.000000 opet-0.0.3/opet/__init__.py
--rw-r--r--   0 btcyz255   (501) staff       (20)      873 2023-07-30 14:21:02.000000 opet-0.0.3/opet/api.py
--rw-r--r--   0 btcyz255   (501) staff       (20)       79 2023-07-30 14:21:02.000000 opet-0.0.3/opet/exceptions.py
--rw-r--r--   0 btcyz255   (501) staff       (20)      586 2023-07-30 14:06:55.000000 opet-0.0.3/opet/utils.py
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 15:45:33.820445 opet-0.0.3/opet.egg-info/
--rw-r--r--   0 btcyz255   (501) staff       (20)      565 2023-07-30 15:45:33.000000 opet-0.0.3/opet.egg-info/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)      227 2023-07-30 15:45:33.000000 opet-0.0.3/opet.egg-info/SOURCES.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 15:45:33.000000 opet-0.0.3/opet.egg-info/dependency_links.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        9 2023-07-30 15:45:33.000000 opet-0.0.3/opet.egg-info/requires.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        5 2023-07-30 15:45:33.000000 opet-0.0.3/opet.egg-info/top_level.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 15:45:33.821137 opet-0.0.3/setup.cfg
--rw-r--r--   0 btcyz255   (501) staff       (20)      769 2023-07-30 15:45:25.000000 opet-0.0.3/setup.py
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 15:55:27.382614 opet-0.0.4/
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.4/LICENSE
+-rw-r--r--   0 btcyz255   (501) staff       (20)      565 2023-07-30 15:55:27.382409 opet-0.0.4/PKG-INFO
+-rw-r--r--   0 btcyz255   (501) staff       (20)       91 2023-07-30 13:14:54.000000 opet-0.0.4/README.md
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 15:55:27.379715 opet-0.0.4/opet/
+-rw-r--r--   0 btcyz255   (501) staff       (20)        0 2023-07-30 13:15:36.000000 opet-0.0.4/opet/__init__.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)      873 2023-07-30 14:21:02.000000 opet-0.0.4/opet/api.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)       79 2023-07-30 14:21:02.000000 opet-0.0.4/opet/exceptions.py
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 15:55:27.381974 opet-0.0.4/opet/opet.egg-info/
+-rw-r--r--   0 btcyz255   (501) staff       (20)      565 2023-07-30 15:55:27.000000 opet-0.0.4/opet/opet.egg-info/PKG-INFO
+-rw-r--r--   0 btcyz255   (501) staff       (20)      252 2023-07-30 15:55:27.000000 opet-0.0.4/opet/opet.egg-info/SOURCES.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 15:55:27.000000 opet-0.0.4/opet/opet.egg-info/dependency_links.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        9 2023-07-30 15:55:27.000000 opet-0.0.4/opet/opet.egg-info/requires.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)       30 2023-07-30 15:55:27.000000 opet-0.0.4/opet/opet.egg-info/top_level.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)      586 2023-07-30 14:06:55.000000 opet-0.0.4/opet/utils.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 15:55:27.382658 opet-0.0.4/setup.cfg
+-rw-r--r--   0 btcyz255   (501) staff       (20)      918 2023-07-30 15:55:10.000000 opet-0.0.4/setup.py
```

### Comparing `opet-0.0.3/LICENSE` & `opet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opet-0.0.3/PKG-INFO` & `opet-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package that allows you to view fuel prices in Turkey based on cities.
 Home-page: https://github.com/sinanerdinc/opet
 Author: Sinan Erdinc
 Author-email: hello@sinanerdinc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opet-0.0.3/opet/api.py` & `opet-0.0.4/opet/api.py`

 * *Files identical despite different names*

### Comparing `opet-0.0.3/opet/utils.py` & `opet-0.0.4/opet/utils.py`

 * *Files identical despite different names*

### Comparing `opet-0.0.3/opet.egg-info/PKG-INFO` & `opet-0.0.4/opet/opet.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package that allows you to view fuel prices in Turkey based on cities.
 Home-page: https://github.com/sinanerdinc/opet
 Author: Sinan Erdinc
 Author-email: hello@sinanerdinc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

