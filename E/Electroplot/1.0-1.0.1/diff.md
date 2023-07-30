# Comparing `tmp/Electroplot-1.0.tar.gz` & `tmp/Electroplot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Electroplot-1.0.tar", last modified: Sun Jul 30 14:59:25 2023, max compression
+gzip compressed data, was "dist\Electroplot-1.0.1.tar", last modified: Sun Jul 30 15:40:18 2023, max compression
```

## Comparing `Electroplot-1.0.tar` & `Electroplot-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:59:25.000000 Electroplot-1.0/
-drwxrwxrwx   0        0        0        0 2023-07-30 14:59:24.000000 Electroplot-1.0/Electroplot/
--rw-rw-rw-   0        0        0    10772 2022-08-05 12:47:38.000000 Electroplot-1.0/Electroplot/Electroplot.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:59:25.000000 Electroplot-1.0/Electroplot/Functions/
--rw-rw-rw-   0        0        0     3739 2022-08-02 14:32:14.000000 Electroplot-1.0/Electroplot/Functions/Arranger.py
--rw-rw-rw-   0        0        0      715 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/Functions/Graphical.py
--rw-rw-rw-   0        0        0        0 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/Functions/__init__.py
--rw-rw-rw-   0        0        0     3058 2022-08-19 15:50:57.000000 Electroplot-1.0/Electroplot/Functions/dataGrabber.py
--rw-rw-rw-   0        0        0     1802 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/Functions/masks.py
--rw-rw-rw-   0        0        0     1354 2022-08-03 12:39:32.000000 Electroplot-1.0/Electroplot/Functions/models.py
--rw-rw-rw-   0        0        0        0 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/__init__.py
--rw-rw-rw-   0        0        0     3096 2023-07-28 08:10:51.000000 Electroplot-1.0/Electroplot/example.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:59:24.000000 Electroplot-1.0/Electroplot.egg-info/
--rw-rw-rw-   0        0        0      727 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-07-30 14:59:23.000000 Electroplot-1.0/Electroplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2023-07-30 14:59:25.000000 Electroplot-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2020-10-05 19:39:06.000000 Electroplot-1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 14:59:25.000000 Electroplot-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1571 2023-07-30 14:57:56.000000 Electroplot-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:40:18.000000 Electroplot-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-30 15:40:18.000000 Electroplot-1.0.1/Electroplot.egg-info/
+-rw-rw-rw-   0        0        0      729 2023-07-30 15:40:17.000000 Electroplot-1.0.1/Electroplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-30 15:40:17.000000 Electroplot-1.0.1/Electroplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:40:17.000000 Electroplot-1.0.1/Electroplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-30 15:40:17.000000 Electroplot-1.0.1/Electroplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:40:17.000000 Electroplot-1.0.1/Electroplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      729 2023-07-30 15:40:18.000000 Electroplot-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2020-07-03 17:04:22.000000 Electroplot-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 15:40:18.000000 Electroplot-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1573 2023-07-30 15:38:52.000000 Electroplot-1.0.1/setup.py
```

### Comparing `Electroplot-1.0/Electroplot.egg-info/PKG-INFO` & `Electroplot-1.0.1/Electroplot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Electroplot
-Version: 1.0
+Version: 1.0.1
 Summary: Handling TIFF files and figure generation from timelapse experiments.
 Home-page: https://github.com/ConorEd/
 Author: Conor Edwards
 Author-email: conorlo@hotmail.co.uk
 License: MIT
 Description: UNKNOWN
 Keywords: IMAGE ANALYSIS,TIFF,TIMELAPSE
```

### Comparing `Electroplot-1.0/PKG-INFO` & `Electroplot-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Electroplot
-Version: 1.0
+Version: 1.0.1
 Summary: Handling TIFF files and figure generation from timelapse experiments.
 Home-page: https://github.com/ConorEd/
 Author: Conor Edwards
 Author-email: conorlo@hotmail.co.uk
 License: MIT
 Description: UNKNOWN
 Keywords: IMAGE ANALYSIS,TIFF,TIMELAPSE
```

### Comparing `Electroplot-1.0/setup.py` & `Electroplot-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 #from distutils.core import setup, find_packages
 from setuptools import setup, find_packages
 setup(
   name = 'Electroplot',         # How you named your package folder (MyLib)
   packages = find_packages(include=['Electroplot', 'Electroplot.*']), 
-  version = '1.0',      # Start with a small number and increase it with every change you make
+  version = '1.0.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Handling TIFF files and figure generation from timelapse experiments.',   # Give a short description about your library
   author = 'Conor Edwards',                   # Type in your name
   author_email = 'conorlo@hotmail.co.uk',      # Type in your E-Mail
   url = 'https://github.com/ConorEd/',   # Provide either the link to your github or to your website
   #download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['IMAGE ANALYSIS', 'TIFF', 'TIMELAPSE'],   # Keywords that define your package best
```

