# Comparing `tmp/PyColorimetry-1.0.0.tar.gz` & `tmp/PyColorimetry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyColorimetry-1.0.0.tar", last modified: Sun Jul 30 09:14:43 2023, max compression
+gzip compressed data, was "PyColorimetry-1.1.0.tar", last modified: Sun Jul 30 09:37:11 2023, max compression
```

## Comparing `PyColorimetry-1.0.0.tar` & `PyColorimetry-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 09:14:43.741455 PyColorimetry-1.0.0/
--rw-rw-rw-   0        0        0    20849 2022-04-17 01:00:14.000000 PyColorimetry-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4079 2023-07-30 09:14:43.740458 PyColorimetry-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 09:14:43.639257 PyColorimetry-1.0.0/PyColorimetry/
--rw-rw-rw-   0        0        0    42619 2023-07-30 06:08:40.000000 PyColorimetry-1.0.0/PyColorimetry/ColorimetricAnalysis.py
--rw-rw-rw-   0        0        0       56 2023-07-30 06:06:55.000000 PyColorimetry-1.0.0/PyColorimetry/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 09:14:43.737205 PyColorimetry-1.0.0/PyColorimetry.egg-info/
--rw-rw-rw-   0        0        0     4079 2023-07-30 09:14:42.000000 PyColorimetry-1.0.0/PyColorimetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-30 09:14:42.000000 PyColorimetry-1.0.0/PyColorimetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 09:14:42.000000 PyColorimetry-1.0.0/PyColorimetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-30 09:14:42.000000 PyColorimetry-1.0.0/PyColorimetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-30 09:14:42.000000 PyColorimetry-1.0.0/PyColorimetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3211 2023-07-29 23:10:47.000000 PyColorimetry-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 09:14:43.741455 PyColorimetry-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4028 2023-07-30 08:13:43.000000 PyColorimetry-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:37:11.515993 PyColorimetry-1.1.0/
+-rw-rw-rw-   0        0        0    20849 2022-04-17 01:00:14.000000 PyColorimetry-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4079 2023-07-30 09:37:11.513580 PyColorimetry-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 09:37:11.466440 PyColorimetry-1.1.0/PyColorimetry/
+-rw-rw-rw-   0        0        0    42619 2023-07-30 06:08:40.000000 PyColorimetry-1.1.0/PyColorimetry/ColorimetricAnalysis.py
+-rw-rw-rw-   0        0        0       56 2023-07-30 06:06:55.000000 PyColorimetry-1.1.0/PyColorimetry/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:37:11.511391 PyColorimetry-1.1.0/PyColorimetry.egg-info/
+-rw-rw-rw-   0        0        0     4079 2023-07-30 09:37:10.000000 PyColorimetry-1.1.0/PyColorimetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-30 09:37:11.000000 PyColorimetry-1.1.0/PyColorimetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:37:10.000000 PyColorimetry-1.1.0/PyColorimetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-07-30 09:37:10.000000 PyColorimetry-1.1.0/PyColorimetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-30 09:37:10.000000 PyColorimetry-1.1.0/PyColorimetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3211 2023-07-29 23:10:47.000000 PyColorimetry-1.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-30 09:37:11.517428 PyColorimetry-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4033 2023-07-30 09:34:21.000000 PyColorimetry-1.1.0/setup.py
```

### Comparing `PyColorimetry-1.0.0/LICENSE` & `PyColorimetry-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyColorimetry-1.0.0/PKG-INFO` & `PyColorimetry-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyColorimetry
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for colorimetric analysis
 Home-page: https://github.com/josorio398/PyColorimetry_Library
 Download-URL: https://github.com/josorio398/PyColorimetry_Library/blob/main/PyColorimetry/ColorimetricAnalysis.py
 Author: Prof. Jhonny Osorio Gallego, M.Sc.
 Author-email: osoriojohnny1986@gmail.com
 License: CC BY-NC-SA 4.0
 Keywords: colorimetry,color analysis,image segmentation,SAM,GroundingDino,RGB,XYZ,CIELAB
```

### Comparing `PyColorimetry-1.0.0/PyColorimetry/ColorimetricAnalysis.py` & `PyColorimetry-1.1.0/PyColorimetry/ColorimetricAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyColorimetry-1.0.0/PyColorimetry.egg-info/PKG-INFO` & `PyColorimetry-1.1.0/PyColorimetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyColorimetry
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for colorimetric analysis
 Home-page: https://github.com/josorio398/PyColorimetry_Library
 Download-URL: https://github.com/josorio398/PyColorimetry_Library/blob/main/PyColorimetry/ColorimetricAnalysis.py
 Author: Prof. Jhonny Osorio Gallego, M.Sc.
 Author-email: osoriojohnny1986@gmail.com
 License: CC BY-NC-SA 4.0
 Keywords: colorimetry,color analysis,image segmentation,SAM,GroundingDino,RGB,XYZ,CIELAB
```

### Comparing `PyColorimetry-1.0.0/README.rst` & `PyColorimetry-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyColorimetry-1.0.0/setup.py` & `PyColorimetry-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from os import path
 from setuptools import setup, find_packages
 from sys import version_info
 
-VERSION = "1.0.0"
+VERSION = "1.1.0"
 CURR_PATH = "{}{}".format(path.abspath(path.dirname(__file__)), '/')
 
 def path_format(file_path=None, file_name=None, is_abspath=False,
                 ignore_raises=False):
     """
     Get path joined checking before if path and filepath exist,
      if not, raise an Exception
@@ -79,15 +79,15 @@
     author='Prof. Jhonny Osorio Gallego, M.Sc.',
     author_email='osoriojohnny1986@gmail.com',
     url='https://github.com/josorio398/PyColorimetry_Library',
     download_url='https://github.com/josorio398/PyColorimetry_Library/blob/main/PyColorimetry/ColorimetricAnalysis.py'.format(
         VERSION),
     keywords=['colorimetry', 'color analysis', 'image segmentation', 'SAM', 'GroundingDino', 'RGB', 'XYZ', 'CIELAB'],
     install_requires=[
-        'pandas','numpy','matplotlib','scipy','skimage','scikit-learn','torch','groundingdino-py','segment-anything-py==1.0','opencv-python',
+        'pandas','numpy','matplotlib','scipy','scikit-image','scikit-learn','torch','groundingdino-py','segment-anything-py==1.0','opencv-python',
     ],
     setup_requires=['groundingdino-py','segment-anything-py==1.0','opencv-python'],
     tests_require=[
         'pytest',
         'pytest-cov',
         'pytest-html',
         'pytest-dependency',
```

