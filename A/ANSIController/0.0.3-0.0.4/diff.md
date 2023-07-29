# Comparing `tmp/ANSIController-0.0.3.tar.gz` & `tmp/ANSIController-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-0.0.3.tar", last modified: Sat Jul 29 23:16:51 2023, max compression
+gzip compressed data, was "ANSIController-0.0.4.tar", last modified: Sat Jul 29 23:19:33 2023, max compression
```

## Comparing `ANSIController-0.0.3.tar` & `ANSIController-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 23:16:51.336728 ANSIController-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-29 23:16:51.315039 ANSIController-0.0.3/ANSIController/
--rw-rw-rw-   0        0        0     5208 2023-07-29 23:15:55.000000 ANSIController-0.0.3/ANSIController/__init__.py
--rw-rw-rw-   0        0        0      190 2023-07-29 23:10:08.000000 ANSIController-0.0.3/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-0.0.3/ANSIController/const.py
--rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-0.0.3/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-0.0.3/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-0.0.3/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-0.0.3/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-29 23:16:51.335733 ANSIController-0.0.3/ANSIController.egg-info/
--rw-rw-rw-   0        0        0      717 2023-07-29 23:16:51.000000 ANSIController-0.0.3/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-29 23:16:51.000000 ANSIController-0.0.3/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 23:16:51.000000 ANSIController-0.0.3/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-07-29 23:16:51.000000 ANSIController-0.0.3/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 23:16:51.000000 ANSIController-0.0.3/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 23:16:51.000000 ANSIController-0.0.3/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      717 2023-07-29 23:16:51.336728 ANSIController-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8198 2023-07-29 23:07:12.000000 ANSIController-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-07-29 23:16:51.338731 ANSIController-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1298 2023-07-29 23:16:00.000000 ANSIController-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:19:33.727363 ANSIController-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-29 23:19:33.702870 ANSIController-0.0.4/ANSIController/
+-rw-rw-rw-   0        0        0     5208 2023-07-29 23:15:55.000000 ANSIController-0.0.4/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-07-29 23:10:08.000000 ANSIController-0.0.4/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-0.0.4/ANSIController/const.py
+-rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-0.0.4/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-0.0.4/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-0.0.4/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-0.0.4/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-29 23:19:33.725368 ANSIController-0.0.4/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0     8958 2023-07-29 23:19:33.000000 ANSIController-0.0.4/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-29 23:19:33.000000 ANSIController-0.0.4/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 23:19:33.000000 ANSIController-0.0.4/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-29 23:19:33.000000 ANSIController-0.0.4/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 23:19:33.000000 ANSIController-0.0.4/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 23:19:33.000000 ANSIController-0.0.4/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     8958 2023-07-29 23:19:33.728365 ANSIController-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8198 2023-07-29 23:07:12.000000 ANSIController-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-29 23:19:33.729834 ANSIController-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1476 2023-07-29 23:19:24.000000 ANSIController-0.0.4/setup.py
```

### Comparing `ANSIController-0.0.3/ANSIController/__init__.py` & `ANSIController-0.0.4/ANSIController/__init__.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/ANSIController/const.py` & `ANSIController-0.0.4/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/ANSIController/controls.py` & `ANSIController-0.0.4/ANSIController/controls.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/ANSIController/tcolor.py` & `ANSIController-0.0.4/ANSIController/tcolor.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/ANSIController/tstyles.py` & `ANSIController-0.0.4/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/LICENSE` & `ANSIController-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/README.md` & `ANSIController-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.3/setup.py` & `ANSIController-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name=__pkg_name__,
     packages=[__pkg_name__],
     version=__version__,
     license='MIT',
     description=__desc__,
     author=__author__,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author_email='forsell450@gmail.com',
     url='https://github.com/jo0x01/ansicontroller',
     # download_url='https://github.com/jo0x01/ansiterminal/archive/ANSITerminal-0.1.tar.gz',
     keywords=['ansi', 'terminal', 'ansi_terminal'],
     install_requires=['keyboard'],
     entry_points={
         'console_scripts': [
```

