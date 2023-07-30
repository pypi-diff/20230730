# Comparing `tmp/assamer-1.3.0.tar.gz` & `tmp/assamer-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assamer-1.3.0.tar", last modified: Sun Jul 30 13:54:53 2023, max compression
+gzip compressed data, was "assamer-1.3.5.tar", last modified: Sun Jul 30 14:00:41 2023, max compression
```

## Comparing `assamer-1.3.0.tar` & `assamer-1.3.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 13:54:53.843746 assamer-1.3.0/
--rw-rw-rw-   0        0        0     8586 2023-07-10 19:24:19.000000 assamer-1.3.0/A2L.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 13:49:48.000000 assamer-1.3.0/ASSAM.py
--rw-rw-rw-   0        0        0      229 2023-07-30 13:54:53.842757 assamer-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2822 2023-07-09 02:17:04.000000 assamer-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 13:54:53.840817 assamer-1.3.0/assamer.egg-info/
--rw-rw-rw-   0        0        0      229 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3719 2023-07-09 02:22:57.000000 assamer-1.3.0/hexa2l.py
--rw-rw-rw-   0        0        0       42 2023-07-30 13:54:53.843746 assamer-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      374 2023-07-30 13:54:45.000000 assamer-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:00:41.987387 assamer-1.3.5/
+-rw-rw-rw-   0        0        0     8586 2023-07-10 19:24:19.000000 assamer-1.3.5/A2L.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 13:49:48.000000 assamer-1.3.5/ASSAM.py
+-rw-rw-rw-   0        0        0      229 2023-07-30 14:00:41.986362 assamer-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2816 2023-07-30 13:59:45.000000 assamer-1.3.5/README.md
+-rw-rw-rw-   0        0        0     5931 2023-07-09 02:00:41.000000 assamer-1.3.5/TrackA2L.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:00:41.985427 assamer-1.3.5/assamer.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3719 2023-07-09 02:22:57.000000 assamer-1.3.5/hexa2l.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:00:41.987387 assamer-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      442 2023-07-30 14:00:28.000000 assamer-1.3.5/setup.py
```

### Comparing `assamer-1.3.0/A2L.py` & `assamer-1.3.5/A2L.py`

 * *Files identical despite different names*

### Comparing `assamer-1.3.0/ASSAM.py` & `assamer-1.3.5/ASSAM.py`

 * *Files identical despite different names*

### Comparing `assamer-1.3.0/README.md` & `assamer-1.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 Assamer library provides classes and functions for reading ASAP2 files, parsing HEX files, and performing ASSAM analysis.
 
 ### Reading ASAP2 Files
 
 To read an ASAP2 file, you can use the `A2L` class. For example:
 
 ```python
-from assamer import A2L
+from ASSAM import A2L
 
 a2l = A2L("path/to/a2l_file.a2l")
 data = a2l.data
 compu_methods = a2l.getArea(COMPU_METHOD)
 characteristics = a2l.getArea(CHARACTERISTIC)
 # Other operations
 ```
 
 ### Parsing HEX Files
 
 To parse a HEX file, you can use the `A2LHex` class. For example:
 
 ```python
-from assamer import A2LHex
+from ASSAM import A2LHex
 
 hexa2l = A2LHex("path/to/hex_file.hex")
 hex_data = hexa2l.data
 value = hexa2l.readValue(0x8040CD34, FLOAT32_IEEE, 5)
 # Other operations
 ```
 
 ### ASSAM Analysis
 
 To perform ASSAM analysis, you can use the `ASSAM` class. For example:
 
 ```python
-from assamer import ASSAM, TrackA2L
+from ASSAM import ASSAM, TrackA2L
 
 a2l = A2L("path/to/a2l_file.a2l")
 hexa2l = A2LHex("path/to/hex_file.hex")
 assam = ASSAM(A2L_Object=a2l, HEX_Object=hexa2l)
 # Other operations
 ```
```

### Comparing `assamer-1.3.0/hexa2l.py` & `assamer-1.3.5/hexa2l.py`

 * *Files identical despite different names*

