# Comparing `tmp/assamer-1.3.5.tar.gz` & `tmp/assamer-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assamer-1.3.5.tar", last modified: Sun Jul 30 14:00:41 2023, max compression
+gzip compressed data, was "assamer-1.3.7.tar", last modified: Sun Jul 30 14:18:59 2023, max compression
```

## Comparing `assamer-1.3.5.tar` & `assamer-1.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:00:41.987387 assamer-1.3.5/
--rw-rw-rw-   0        0        0     8586 2023-07-10 19:24:19.000000 assamer-1.3.5/A2L.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 13:49:48.000000 assamer-1.3.5/ASSAM.py
--rw-rw-rw-   0        0        0      229 2023-07-30 14:00:41.986362 assamer-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2816 2023-07-30 13:59:45.000000 assamer-1.3.5/README.md
--rw-rw-rw-   0        0        0     5931 2023-07-09 02:00:41.000000 assamer-1.3.5/TrackA2L.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:00:41.985427 assamer-1.3.5/assamer.egg-info/
--rw-rw-rw-   0        0        0      229 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-30 14:00:41.000000 assamer-1.3.5/assamer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3719 2023-07-09 02:22:57.000000 assamer-1.3.5/hexa2l.py
--rw-rw-rw-   0        0        0       42 2023-07-30 14:00:41.987387 assamer-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      442 2023-07-30 14:00:28.000000 assamer-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:18:59.038782 assamer-1.3.7/
+-rw-rw-rw-   0        0        0     8586 2023-07-10 19:24:19.000000 assamer-1.3.7/A2L.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 13:49:48.000000 assamer-1.3.7/ASSAM.py
+-rw-rw-rw-   0        0        0     3324 2023-07-30 14:18:59.038782 assamer-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2816 2023-07-30 13:59:45.000000 assamer-1.3.7/README.md
+-rw-rw-rw-   0        0        0     5931 2023-07-09 02:00:41.000000 assamer-1.3.7/TrackA2L.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:18:59.037783 assamer-1.3.7/assamer.egg-info/
+-rw-rw-rw-   0        0        0     3324 2023-07-30 14:18:58.000000 assamer-1.3.7/assamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-30 14:18:58.000000 assamer-1.3.7/assamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:18:58.000000 assamer-1.3.7/assamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 14:18:58.000000 assamer-1.3.7/assamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-30 14:18:58.000000 assamer-1.3.7/assamer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3719 2023-07-09 02:22:57.000000 assamer-1.3.7/hexa2l.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:18:59.039784 assamer-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      678 2023-07-30 14:18:56.000000 assamer-1.3.7/setup.py
```

### Comparing `assamer-1.3.5/A2L.py` & `assamer-1.3.7/A2L.py`

 * *Files identical despite different names*

### Comparing `assamer-1.3.5/ASSAM.py` & `assamer-1.3.7/ASSAM.py`

 * *Files identical despite different names*

### Comparing `assamer-1.3.5/README.md` & `assamer-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `assamer-1.3.5/TrackA2L.py` & `assamer-1.3.7/TrackA2L.py`

 * *Files identical despite different names*

### Comparing `assamer-1.3.5/hexa2l.py` & `assamer-1.3.7/hexa2l.py`

 * *Files identical despite different names*

