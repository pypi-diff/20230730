# Comparing `tmp/ezgpx-0.1.5.tar.gz` & `tmp/ezgpx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezgpx-0.1.5.tar", last modified: Mon Jul 24 14:29:50 2023, max compression
+gzip compressed data, was "ezgpx-0.1.6.tar", last modified: Sun Jul 30 13:41:29 2023, max compression
```

## Comparing `ezgpx-0.1.5.tar` & `ezgpx-0.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.5/LICENSE
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-24 14:29:50.091924 ezgpx-0.1.5/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1179 2023-07-19 12:57:20.000000 ezgpx-0.1.5/README.md
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.083924 ezgpx-0.1.5/ezgpx/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.5/ezgpx/__init__.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.083924 ezgpx-0.1.5/ezgpx/gpx/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       18 2023-06-08 09:30:14.000000 ezgpx-0.1.5/ezgpx/gpx/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    35639 2023-07-24 13:31:56.000000 ezgpx-0.1.5/ezgpx/gpx/gpx.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.087924 ezgpx-0.1.5/ezgpx/gpx_elements/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      324 2023-07-03 09:39:46.000000 ezgpx-0.1.5/ezgpx/gpx_elements/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      892 2023-07-03 09:53:44.000000 ezgpx-0.1.5/ezgpx/gpx_elements/bounds.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      717 2023-07-03 09:49:36.000000 ezgpx-0.1.5/ezgpx/gpx_elements/copyright.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      553 2023-07-03 09:50:23.000000 ezgpx-0.1.5/ezgpx/gpx_elements/email.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2855 2023-07-03 09:50:51.000000 ezgpx-0.1.5/ezgpx/gpx_elements/extensions.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    24767 2023-07-24 13:47:37.000000 ezgpx-0.1.5/ezgpx/gpx_elements/gpx.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      680 2023-07-03 09:51:43.000000 ezgpx-0.1.5/ezgpx/gpx_elements/link.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1596 2023-07-03 09:52:07.000000 ezgpx-0.1.5/ezgpx/gpx_elements/metadata.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      730 2023-07-03 09:52:28.000000 ezgpx-0.1.5/ezgpx/gpx_elements/person.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1026 2023-07-03 12:48:14.000000 ezgpx-0.1.5/ezgpx/gpx_elements/point.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      595 2023-07-23 14:49:38.000000 ezgpx-0.1.5/ezgpx/gpx_elements/point_segment.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1637 2023-07-23 14:50:06.000000 ezgpx-0.1.5/ezgpx/gpx_elements/route.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1892 2023-07-23 14:51:01.000000 ezgpx-0.1.5/ezgpx/gpx_elements/track.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1030 2023-07-23 14:50:40.000000 ezgpx-0.1.5/ezgpx/gpx_elements/track_segment.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     4143 2023-07-24 13:15:21.000000 ezgpx-0.1.5/ezgpx/gpx_elements/way_point.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.087924 ezgpx-0.1.5/ezgpx/gpx_parser/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 12:15:07.000000 ezgpx-0.1.5/ezgpx/gpx_parser/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    24702 2023-07-23 14:46:38.000000 ezgpx-0.1.5/ezgpx/gpx_parser/parser.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.087924 ezgpx-0.1.5/ezgpx/gpx_writer/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 08:52:43.000000 ezgpx-0.1.5/ezgpx/gpx_writer/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    24325 2023-07-22 13:28:10.000000 ezgpx-0.1.5/ezgpx/gpx_writer/writer.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/ezgpx/utils/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       76 2023-06-27 12:31:11.000000 ezgpx-0.1.5/ezgpx/utils/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1494 2023-06-28 13:57:41.000000 ezgpx-0.1.5/ezgpx/utils/algorithms.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2633 2023-07-18 15:26:00.000000 ezgpx-0.1.5/ezgpx/utils/distance.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2672 2023-07-14 14:27:06.000000 ezgpx-0.1.5/ezgpx/utils/projections.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.083924 ezgpx-0.1.5/ezgpx.egg-info/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      978 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/SOURCES.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/dependency_links.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       47 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/requires.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/top_level.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-24 14:29:50.091924 ezgpx-0.1.5/setup.cfg
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1727 2023-07-24 14:29:43.000000 ezgpx-0.1.5/setup.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/tests/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:09.000000 ezgpx-0.1.5/tests/__init__.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/tests/dev_tests/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:13.000000 ezgpx-0.1.5/tests/dev_tests/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     4634 2023-07-22 13:05:48.000000 ezgpx-0.1.5/tests/test_GPX.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1922 2023-07-24 13:53:40.000000 ezgpx-0.1.5/tests/test_utils.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.204293 ezgpx-0.1.6/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.6/LICENSE
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2257 2023-07-30 13:41:29.204293 ezgpx-0.1.6/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1176 2023-07-30 13:23:41.000000 ezgpx-0.1.6/README.md
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.192293 ezgpx-0.1.6/ezgpx/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.6/ezgpx/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.196293 ezgpx-0.1.6/ezgpx/gpx/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       18 2023-06-08 09:30:14.000000 ezgpx-0.1.6/ezgpx/gpx/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    35639 2023-07-24 20:58:41.000000 ezgpx-0.1.6/ezgpx/gpx/gpx.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.200293 ezgpx-0.1.6/ezgpx/gpx_elements/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      324 2023-07-03 09:39:46.000000 ezgpx-0.1.6/ezgpx/gpx_elements/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      892 2023-07-03 09:53:44.000000 ezgpx-0.1.6/ezgpx/gpx_elements/bounds.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      717 2023-07-03 09:49:36.000000 ezgpx-0.1.6/ezgpx/gpx_elements/copyright.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      553 2023-07-03 09:50:23.000000 ezgpx-0.1.6/ezgpx/gpx_elements/email.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2855 2023-07-03 09:50:51.000000 ezgpx-0.1.6/ezgpx/gpx_elements/extensions.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    24767 2023-07-24 13:47:37.000000 ezgpx-0.1.6/ezgpx/gpx_elements/gpx.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      680 2023-07-03 09:51:43.000000 ezgpx-0.1.6/ezgpx/gpx_elements/link.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1596 2023-07-03 09:52:07.000000 ezgpx-0.1.6/ezgpx/gpx_elements/metadata.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      730 2023-07-03 09:52:28.000000 ezgpx-0.1.6/ezgpx/gpx_elements/person.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1026 2023-07-03 12:48:14.000000 ezgpx-0.1.6/ezgpx/gpx_elements/point.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      595 2023-07-23 14:49:38.000000 ezgpx-0.1.6/ezgpx/gpx_elements/point_segment.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1637 2023-07-23 14:50:06.000000 ezgpx-0.1.6/ezgpx/gpx_elements/route.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1892 2023-07-23 14:51:01.000000 ezgpx-0.1.6/ezgpx/gpx_elements/track.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1030 2023-07-23 14:50:40.000000 ezgpx-0.1.6/ezgpx/gpx_elements/track_segment.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     4143 2023-07-24 13:15:21.000000 ezgpx-0.1.6/ezgpx/gpx_elements/way_point.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.200293 ezgpx-0.1.6/ezgpx/gpx_parser/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 12:15:07.000000 ezgpx-0.1.6/ezgpx/gpx_parser/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    24702 2023-07-23 14:46:38.000000 ezgpx-0.1.6/ezgpx/gpx_parser/parser.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.200293 ezgpx-0.1.6/ezgpx/gpx_writer/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 08:52:43.000000 ezgpx-0.1.6/ezgpx/gpx_writer/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    24325 2023-07-22 13:28:10.000000 ezgpx-0.1.6/ezgpx/gpx_writer/writer.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.200293 ezgpx-0.1.6/ezgpx/utils/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       76 2023-06-27 12:31:11.000000 ezgpx-0.1.6/ezgpx/utils/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1494 2023-06-28 13:57:41.000000 ezgpx-0.1.6/ezgpx/utils/algorithms.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2633 2023-07-18 15:26:00.000000 ezgpx-0.1.6/ezgpx/utils/distance.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2672 2023-07-14 14:27:06.000000 ezgpx-0.1.6/ezgpx/utils/projections.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.196293 ezgpx-0.1.6/ezgpx.egg-info/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2257 2023-07-30 13:41:28.000000 ezgpx-0.1.6/ezgpx.egg-info/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      978 2023-07-30 13:41:29.000000 ezgpx-0.1.6/ezgpx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-30 13:41:28.000000 ezgpx-0.1.6/ezgpx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       47 2023-07-30 13:41:28.000000 ezgpx-0.1.6/ezgpx.egg-info/requires.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-30 13:41:28.000000 ezgpx-0.1.6/ezgpx.egg-info/top_level.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-30 13:41:29.204293 ezgpx-0.1.6/setup.cfg
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1827 2023-07-30 13:41:18.000000 ezgpx-0.1.6/setup.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.204293 ezgpx-0.1.6/tests/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:09.000000 ezgpx-0.1.6/tests/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-30 13:41:29.204293 ezgpx-0.1.6/tests/dev_tests/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:13.000000 ezgpx-0.1.6/tests/dev_tests/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     4634 2023-07-22 13:05:48.000000 ezgpx-0.1.6/tests/test_GPX.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1922 2023-07-24 13:53:40.000000 ezgpx-0.1.6/tests/test_utils.py
```

### Comparing `ezgpx-0.1.5/LICENSE` & `ezgpx-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/PKG-INFO` & `ezgpx-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezgpx
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy to use Python GPX library
 Home-page: https://pypi.org/project/ezgpx/
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗺️ ezGPX
 
 ## 🔎 Description
@@ -46,15 +48,15 @@
 # Parse GPX file
 gpx = ezgpx.GPX("file.gpx")
 
 # Simplify (using Ramer-Dougle-Peucker algorithm)
 gpx.simplify()
 
 # Plot with Matplotlib
-gpx.matplotlib_plot(elevation_color=True,
+gpx.matplotlib_plot(color="elevation",
                     start_stop_colors=("green", "red"),
                     way_points_color="blue",
                     title=gpx.name(),
                     duration=(0, 0),
                     distance=(0.5, 0),
                     ascent=None,
                     pace=(1, 0),
```

### Comparing `ezgpx-0.1.5/README.md` & `ezgpx-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # Parse GPX file
 gpx = ezgpx.GPX("file.gpx")
 
 # Simplify (using Ramer-Dougle-Peucker algorithm)
 gpx.simplify()
 
 # Plot with Matplotlib
-gpx.matplotlib_plot(elevation_color=True,
+gpx.matplotlib_plot(color="elevation",
                     start_stop_colors=("green", "red"),
                     way_points_color="blue",
                     title=gpx.name(),
                     duration=(0, 0),
                     distance=(0.5, 0),
                     ascent=None,
                     pace=(1, 0),
```

### Comparing `ezgpx-0.1.5/ezgpx/gpx/gpx.py` & `ezgpx-0.1.6/ezgpx/gpx/gpx.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/bounds.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/bounds.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/copyright.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/copyright.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/email.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/email.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/extensions.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/extensions.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/gpx.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/gpx.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/link.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/link.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/metadata.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/metadata.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/person.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/person.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/point.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/point.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/point_segment.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/point_segment.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/route.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/route.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/track.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/track.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/track_segment.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/track_segment.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_elements/way_point.py` & `ezgpx-0.1.6/ezgpx/gpx_elements/way_point.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_parser/parser.py` & `ezgpx-0.1.6/ezgpx/gpx_parser/parser.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/gpx_writer/writer.py` & `ezgpx-0.1.6/ezgpx/gpx_writer/writer.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/utils/algorithms.py` & `ezgpx-0.1.6/ezgpx/utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/utils/distance.py` & `ezgpx-0.1.6/ezgpx/utils/distance.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx/utils/projections.py` & `ezgpx-0.1.6/ezgpx/utils/projections.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/ezgpx.egg-info/PKG-INFO` & `ezgpx-0.1.6/ezgpx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezgpx
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy to use Python GPX library
 Home-page: https://pypi.org/project/ezgpx/
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗺️ ezGPX
 
 ## 🔎 Description
@@ -46,15 +48,15 @@
 # Parse GPX file
 gpx = ezgpx.GPX("file.gpx")
 
 # Simplify (using Ramer-Dougle-Peucker algorithm)
 gpx.simplify()
 
 # Plot with Matplotlib
-gpx.matplotlib_plot(elevation_color=True,
+gpx.matplotlib_plot(color="elevation",
                     start_stop_colors=("green", "red"),
                     way_points_color="blue",
                     title=gpx.name(),
                     duration=(0, 0),
                     distance=(0.5, 0),
                     ascent=None,
                     pace=(1, 0),
```

### Comparing `ezgpx-0.1.5/ezgpx.egg-info/SOURCES.txt` & `ezgpx-0.1.6/ezgpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/setup.py` & `ezgpx-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ezgpx',
-    version='0.1.5',
+    version='0.1.6',
     description='Easy to use Python GPX library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['gpx', 'gpx-files', 'gpx-parser', 'gpx-reader', 'gpx-writer', 'gpx-data'],
     url='https://pypi.org/project/ezgpx/',
     download_url='https://github.com/FABallemand/ezGPX',
     project_urls={
@@ -30,14 +30,16 @@
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent'
     ],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pandas',
         'matplotlib',
```

### Comparing `ezgpx-0.1.5/tests/test_GPX.py` & `ezgpx-0.1.6/tests/test_GPX.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.5/tests/test_utils.py` & `ezgpx-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

