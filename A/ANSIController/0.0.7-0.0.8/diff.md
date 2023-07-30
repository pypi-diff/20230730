# Comparing `tmp/ANSIController-0.0.7.tar.gz` & `tmp/ANSIController-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-0.0.7.tar", last modified: Sun Jul 30 01:03:14 2023, max compression
+gzip compressed data, was "ANSIController-0.0.8.tar", last modified: Sun Jul 30 01:08:18 2023, max compression
```

## Comparing `ANSIController-0.0.7.tar` & `ANSIController-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 01:03:14.612609 ANSIController-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-30 01:03:14.579689 ANSIController-0.0.7/ANSIController/
--rw-rw-rw-   0        0        0     3196 2023-07-30 00:55:06.000000 ANSIController-0.0.7/ANSIController/__init__.py
--rw-rw-rw-   0        0        0     2268 2023-07-30 01:02:26.000000 ANSIController-0.0.7/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-0.0.7/ANSIController/const.py
--rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-0.0.7/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-0.0.7/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-0.0.7/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-0.0.7/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-30 01:03:14.610650 ANSIController-0.0.7/ANSIController.egg-info/
--rw-rw-rw-   0        0        0     9221 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     9221 2023-07-30 01:03:14.613587 ANSIController-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8461 2023-07-30 00:46:10.000000 ANSIController-0.0.7/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 01:03:14.616456 ANSIController-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-07-30 01:03:07.000000 ANSIController-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:08:18.596531 ANSIController-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-30 01:08:18.569610 ANSIController-0.0.8/ANSIController/
+-rw-rw-rw-   0        0        0     3218 2023-07-30 01:08:06.000000 ANSIController-0.0.8/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0     2290 2023-07-30 01:08:04.000000 ANSIController-0.0.8/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-0.0.8/ANSIController/const.py
+-rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-0.0.8/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-0.0.8/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-0.0.8/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-0.0.8/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:08:18.596022 ANSIController-0.0.8/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0     9221 2023-07-30 01:08:18.000000 ANSIController-0.0.8/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-30 01:08:18.000000 ANSIController-0.0.8/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:08:18.000000 ANSIController-0.0.8/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-30 01:08:18.000000 ANSIController-0.0.8/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 01:08:18.000000 ANSIController-0.0.8/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 01:08:18.000000 ANSIController-0.0.8/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9221 2023-07-30 01:08:18.596531 ANSIController-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8461 2023-07-30 00:46:10.000000 ANSIController-0.0.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 01:08:18.599228 ANSIController-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1383 2023-07-30 01:08:16.000000 ANSIController-0.0.8/setup.py
```

### Comparing `ANSIController-0.0.7/ANSIController/__init__.py` & `ANSIController-0.0.8/ANSIController/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+#!/usr/bin/env python3
 from time import sleep
 import keyboard
 from ANSIController.const import _256_FG,_256_BG,_1ATTR, _RESET, _print
 from ANSIController.controls import _ColorsControls, _CursorControls
 from ANSIController.tparser import _PARSER
```

### Comparing `ANSIController-0.0.7/ANSIController/__main__.py` & `ANSIController-0.0.8/ANSIController/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+#!/usr/bin/env python3
 from ANSIController.const import _print
 from ANSIController import Terminal
 
 ## more info `https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape`
 
 __author__ = 'JoOx01'
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
```

### Comparing `ANSIController-0.0.7/ANSIController/const.py` & `ANSIController-0.0.8/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.7/ANSIController/controls.py` & `ANSIController-0.0.8/ANSIController/controls.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.7/ANSIController/tcolor.py` & `ANSIController-0.0.8/ANSIController/tcolor.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.7/ANSIController/tstyles.py` & `ANSIController-0.0.8/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.7/ANSIController.egg-info/PKG-INFO` & `ANSIController-0.0.8/ANSIController.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 0.0.7
+Version: 0.0.8
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ANSIController-0.0.7/LICENSE` & `ANSIController-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.7/PKG-INFO` & `ANSIController-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 0.0.7
+Version: 0.0.8
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ANSIController-0.0.7/README.md` & `ANSIController-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.7/setup.py` & `ANSIController-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=__pkg_name__,
@@ -19,15 +19,15 @@
     long_description_content_type='text/markdown',
     author_email='forsell450@gmail.com',
     url='https://github.com/jo0x01/ansicontroller',
     keywords=['ansi', 'terminal', 'ansi_terminal'],
     install_requires=['keyboard'],
     entry_points={
         'console_scripts': [
-            'ansicontroller=ANSIController.__main__:main'
+            'ansicontroller = ANSIController.__main__:main'
         ]
     },
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

