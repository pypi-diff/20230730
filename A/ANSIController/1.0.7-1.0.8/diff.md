# Comparing `tmp/ANSIController-1.0.7.tar.gz` & `tmp/ANSIController-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-1.0.7.tar", last modified: Sun Jul 30 09:46:58 2023, max compression
+gzip compressed data, was "ANSIController-1.0.8.tar", last modified: Sun Jul 30 09:51:15 2023, max compression
```

## Comparing `ANSIController-1.0.7.tar` & `ANSIController-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 09:46:58.721905 ANSIController-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-30 09:46:58.700527 ANSIController-1.0.7/ANSIController/
--rw-rw-rw-   0        0        0    10863 2023-07-30 09:46:20.000000 ANSIController-1.0.7/ANSIController/__init__.py
--rw-rw-rw-   0        0        0     2307 2023-07-30 09:37:17.000000 ANSIController-1.0.7/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.7/ANSIController/const.py
--rw-rw-rw-   0        0        0     8681 2023-07-30 09:32:45.000000 ANSIController-1.0.7/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3776 2023-07-30 08:38:37.000000 ANSIController-1.0.7/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      457 2023-07-30 09:32:51.000000 ANSIController-1.0.7/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-30 08:38:33.000000 ANSIController-1.0.7/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-30 09:46:58.721369 ANSIController-1.0.7/ANSIController.egg-info/
--rw-rw-rw-   0        0        0    11509 2023-07-30 09:46:58.000000 ANSIController-1.0.7/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-30 09:46:58.000000 ANSIController-1.0.7/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 09:46:58.000000 ANSIController-1.0.7/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-30 09:46:58.000000 ANSIController-1.0.7/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 09:46:58.000000 ANSIController-1.0.7/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 09:46:58.000000 ANSIController-1.0.7/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.7/LICENSE
--rw-rw-rw-   0        0        0    11509 2023-07-30 09:46:58.721905 ANSIController-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.7/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 09:46:58.724221 ANSIController-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1686 2023-07-30 09:46:54.000000 ANSIController-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:51:15.810635 ANSIController-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-30 09:51:15.785279 ANSIController-1.0.8/ANSIController/
+-rw-rw-rw-   0        0        0    10863 2023-07-30 09:46:20.000000 ANSIController-1.0.8/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0     2307 2023-07-30 09:37:17.000000 ANSIController-1.0.8/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.8/ANSIController/const.py
+-rw-rw-rw-   0        0        0     8681 2023-07-30 09:32:45.000000 ANSIController-1.0.8/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3776 2023-07-30 08:38:37.000000 ANSIController-1.0.8/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      457 2023-07-30 09:32:51.000000 ANSIController-1.0.8/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     2993 2023-07-30 08:38:33.000000 ANSIController-1.0.8/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:51:15.808870 ANSIController-1.0.8/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0    11509 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0    11509 2023-07-30 09:51:15.811157 ANSIController-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 09:51:15.812169 ANSIController-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-07-30 09:51:08.000000 ANSIController-1.0.8/setup.py
```

### Comparing `ANSIController-1.0.7/ANSIController/__init__.py` & `ANSIController-1.0.8/ANSIController/__init__.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/ANSIController/__main__.py` & `ANSIController-1.0.8/ANSIController/__main__.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/ANSIController/const.py` & `ANSIController-1.0.8/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/ANSIController/controls.py` & `ANSIController-1.0.8/ANSIController/controls.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/ANSIController/tcolor.py` & `ANSIController-1.0.8/ANSIController/tcolor.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/ANSIController/tstyles.py` & `ANSIController-1.0.8/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/ANSIController.egg-info/PKG-INFO` & `ANSIController-1.0.8/ANSIController.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.7
+Version: 1.0.8
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ANSIController-1.0.7/LICENSE` & `ANSIController-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/PKG-INFO` & `ANSIController-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.7
+Version: 1.0.8
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ANSIController-1.0.7/README.md` & `ANSIController-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.7/setup.py` & `ANSIController-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=__pkg_name__,
```

