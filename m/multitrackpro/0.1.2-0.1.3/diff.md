# Comparing `tmp/multitrackpro-0.1.2.tar.gz` & `tmp/multitrackpro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multitrackpro-0.1.2.tar", last modified: Wed Jun 14 22:25:38 2023, max compression
+gzip compressed data, was "multitrackpro-0.1.3.tar", last modified: Sun Jul 30 15:37:51 2023, max compression
```

## Comparing `multitrackpro-0.1.2.tar` & `multitrackpro-0.1.3.tar`

### file list

```diff
@@ -1,69 +1,62 @@
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/
--rw-rw-r--   0 sk        (1000) sk        (1000)      165 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/AUTHORS.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     3611 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      230 2023-06-14 22:23:47.000000 multitrackpro-0.1.2/HISTORY.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     1613 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/LICENSE
--rw-rw-r--   0 sk        (1000) sk        (1000)      262 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/MANIFEST.in
--rw-rw-r--   0 sk        (1000) sk        (1000)     3304 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/PKG-INFO
--rw-rw-r--   0 sk        (1000) sk        (1000)     1658 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/README.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/
--rw-rw-r--   0 sk        (1000) sk        (1000)      613 2023-06-13 00:07:22.000000 multitrackpro-0.1.2/docs/Makefile
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/_build/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/_build/html/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/_build/html/_static/
--rw-rw-r--   0 sk        (1000) sk        (1000)      286 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/authors.rst
--rwxrwxr-x   0 sk        (1000) sk        (1000)     4865 2023-06-13 00:08:18.000000 multitrackpro-0.1.2/docs/conf.py
--rw-rw-r--   0 sk        (1000) sk        (1000)       33 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/contributing.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/history.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/html/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/docs/html/_static/
--rw-rw-r--   0 sk        (1000) sk        (1000)      286 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/html/_static/file.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/html/_static/minus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/html/_static/plus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)      313 2023-06-10 09:05:27.000000 multitrackpro-0.1.2/docs/index.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     1182 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/installation.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      811 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/make.bat
--rw-rw-r--   0 sk        (1000) sk        (1000)       73 2023-06-14 22:24:28.000000 multitrackpro-0.1.2/docs/modules.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      632 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.core.io.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      645 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.core.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      409 2023-06-13 00:08:47.000000 multitrackpro-0.1.2/docs/multitracker.core.tracker.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      374 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.qt.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      784 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       27 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/readme.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/usage.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/
--rw-rw-r--   0 sk        (1000) sk        (1000)      140 2023-06-14 22:24:11.000000 multitrackpro-0.1.2/multitracker/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)     6427 2023-06-14 20:58:57.000000 multitrackpro-0.1.2/multitracker/auto_annotate_pro.py
--rw-rw-r--   0 sk        (1000) sk        (1000)       20 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/config.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/core/
--rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)     1997 2023-06-13 19:14:44.000000 multitrackpro-0.1.2/multitracker/core/dataset_manager.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/core/io/
--rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/io/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)     2267 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/io/cached_video_reader.py
--rw-rw-r--   0 sk        (1000) sk        (1000)     1176 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/io/multi_video_manager.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/core/tracker/
--rw-rw-r--   0 sk        (1000) sk        (1000)      322 2023-06-13 00:02:34.000000 multitrackpro-0.1.2/multitracker/core/tracker/Tracker.py
--rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-12 21:05:37.000000 multitrackpro-0.1.2/multitracker/core/tracker/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)      411 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/video_utils.py
--rw-rw-r--   0 sk        (1000) sk        (1000)       19 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/multi_track_pro.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/qt/
--rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/qt/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)     7666 2023-06-13 00:02:34.000000 multitrackpro-0.1.2/multitracker/qt/my_main_window.py
--rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-13 12:52:14.000000 multitrackpro-0.1.2/multitracker/stackoverflow.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitrackpro.egg-info/
--rw-rw-r--   0 sk        (1000) sk        (1000)     3304 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/PKG-INFO
--rw-rw-r--   0 sk        (1000) sk        (1000)     1404 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/SOURCES.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/dependency_links.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)       61 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/entry_points.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/not-zip-safe
--rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/requires.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)       13 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/top_level.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)      407 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/setup.cfg
--rw-rw-r--   0 sk        (1000) sk        (1000)     2342 2023-06-14 22:24:14.000000 multitrackpro-0.1.2/setup.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/tests/
--rw-rw-r--   0 sk        (1000) sk        (1000)       43 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/tests/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)      376 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/tests/test_multitrackpro.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      165 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/AUTHORS.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3611 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/CONTRIBUTING.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      363 2023-07-30 15:35:53.000000 multitrackpro-0.1.3/HISTORY.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1614 2023-06-15 12:21:36.000000 multitrackpro-0.1.3/LICENSE
+-rw-rw-r--   0 sk        (1000) sk        (1000)      262 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/MANIFEST.in
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3943 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/PKG-INFO
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2163 2023-07-30 14:25:02.000000 multitrackpro-0.1.3/README.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.273470 multitrackpro-0.1.3/docs/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      613 2023-06-13 00:07:22.000000 multitrackpro-0.1.3/docs/Makefile
+-rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/authors.rst
+-rwxrwxr-x   0 sk        (1000) sk        (1000)     4865 2023-06-13 00:08:18.000000 multitrackpro-0.1.3/docs/conf.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)       33 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/contributing.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/history.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      313 2023-06-10 09:05:27.000000 multitrackpro-0.1.3/docs/index.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1182 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/installation.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      811 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/make.bat
+-rw-rw-r--   0 sk        (1000) sk        (1000)       73 2023-06-14 22:24:28.000000 multitrackpro-0.1.3/docs/modules.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      632 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/docs/multitracker.core.io.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      645 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/docs/multitracker.core.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      409 2023-06-13 00:08:47.000000 multitrackpro-0.1.3/docs/multitracker.core.tracker.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      374 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/docs/multitracker.qt.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      784 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/docs/multitracker.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       27 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/readme.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/docs/usage.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.273470 multitrackpro-0.1.3/multitracker/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      140 2023-07-30 15:35:53.000000 multitrackpro-0.1.3/multitracker/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     6746 2023-07-30 15:26:30.000000 multitrackpro-0.1.3/multitracker/auto_annotate_pro.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)       20 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/multitracker/config.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitracker/core/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/multitracker/core/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2729 2023-07-30 14:12:35.000000 multitrackpro-0.1.3/multitracker/core/dataset_manager.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitracker/core/detection/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-07-03 22:37:32.000000 multitrackpro-0.1.3/multitracker/core/detection/__init__.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitracker/core/io/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/multitracker/core/io/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2280 2023-07-30 14:27:52.000000 multitrackpro-0.1.3/multitracker/core/io/cached_video_reader.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1188 2023-07-03 17:32:45.000000 multitrackpro-0.1.3/multitracker/core/io/multi_video_manager.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitracker/core/tracker/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-12 21:05:37.000000 multitrackpro-0.1.3/multitracker/core/tracker/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2187 2023-07-30 15:35:47.000000 multitrackpro-0.1.3/multitracker/core/tracker/multi_tracker.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)      411 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/multitracker/core/video_utils.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitracker/core/visualization/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-06 22:07:52.000000 multitrackpro-0.1.3/multitracker/core/visualization/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)      885 2023-06-06 22:27:56.000000 multitrackpro-0.1.3/multitracker/core/visualization/plot_bounding_boxes.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1274 2023-07-06 11:29:58.000000 multitrackpro-0.1.3/multitracker/core/visualization/track_color_map.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitracker/qt/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/multitracker/qt/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     7666 2023-06-13 00:02:34.000000 multitrackpro-0.1.3/multitracker/qt/my_main_window.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/multitrackpro.egg-info/
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3943 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/PKG-INFO
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1353 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/SOURCES.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/dependency_links.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)       61 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/entry_points.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/not-zip-safe
+-rw-rw-r--   0 sk        (1000) sk        (1000)       72 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/requires.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)       13 2023-07-30 15:37:51.000000 multitrackpro-0.1.3/multitrackpro.egg-info/top_level.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)      407 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/setup.cfg
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2305 2023-07-30 15:35:53.000000 multitrackpro-0.1.3/setup.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-07-30 15:37:51.277469 multitrackpro-0.1.3/tests/
+-rw-rw-r--   0 sk        (1000) sk        (1000)       43 2023-06-09 10:59:19.000000 multitrackpro-0.1.3/tests/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)      376 2023-06-09 22:39:14.000000 multitrackpro-0.1.3/tests/test_multitrackpro.py
```

### Comparing `multitrackpro-0.1.2/CONTRIBUTING.rst` & `multitrackpro-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/LICENSE` & `multitrackpro-0.1.3/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007
 
-    A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
+    A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.
     Copyright (C) 2023  Saurabh Khanduja
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
```

### Comparing `multitrackpro-0.1.2/PKG-INFO` & `multitrackpro-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: multitrackpro
-Version: 0.1.2
-Summary: A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
+Version: 0.1.3
+Summary: A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.
 Home-page: https://github.com/saurabheights/multitrackpro
 Author: Saurabh Khanduja
 Author-email: pixelperceive@gmail.com
 License: GNU General Public License v3
 Keywords: multitrackpro,annotation,labelling,machine-learning,deep-learning,vision,ML,DL,AI,YOLO
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 .. image:: https://readthedocs.org/projects/multitrackpro/badge/?version=latest
         :target: https://multitrackpro.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
 
-A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
+A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://readthedocs.org/projects/multitrackpro/.
 
 
 Features
@@ -59,29 +59,39 @@
 .. code-block:: shell
 
    auto-annotate-pro
 
 Pending Tasks
 -------------
 
-* Integrate object detection and tracker.
-    * Store annotations of each frame in mem.
-    * Add display of bounding boxes as drawables.
+* Implement play of N number of video files (N != 4, but N <=4). Limit to 4 videos maximum.
+* Set play pause next frame, prev frame etc buttons to disabled stage when no video.
+* Add play pause icons to UI using `Google Material`_.
+
+* Integrate object detection.
+    * ☑ - Store annotations of each frame in memory.
+    * ☑ - Add display of bounding boxes.
+    * Replace BoundingBox as drawables.
+    * Add tracker.
     * Save/Load Annotations.
     * Save dataset-specific configuration.
+* Add masking to the frames to discard object detection for certain areas.
 * Add object detection correction
 * Add tracking correction
 * Add mouse event capture to rearrange videos.
 * Add track integration between two frames.
-* Add play pause icons to UI.
-* Set play pause next fram, prev frame etc buttons to disabled stage when no video.
+
 * Add speed change option for playback.
 * Make frame number text label and slider work.
 * Integrate github action/circleci
-* Implement play of N number of video files (N != 4).
+* ToDo - See Live Preview of object detection and tracking. This will help user catch errors quickly, instead of running object detection completely.
+* Use platformdirs_
+
+.. _Google Material: https://fonts.google.com/icons?icon.category=Audio%26Video
+.. _platformdirs: https://github.com/platformdirs/platformdirs
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -102,7 +112,13 @@
 
 * Added video player that plays exactly 4 videos.
 
 0.1.2 (2023-06-15)
 ------------------
 
 * BugFixes
+
+0.1.3 (2023-07-30)
+------------------
+
+* Integrated Object Detection for all videos.
+* Added rendering of object detection results.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multitrackpro-0.1.2/README.rst` & `multitrackpro-0.1.3/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 .. image:: https://readthedocs.org/projects/multitrackpro/badge/?version=latest
         :target: https://multitrackpro.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
 
-A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
+A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://readthedocs.org/projects/multitrackpro/.
 
 
 Features
@@ -28,29 +28,39 @@
 .. code-block:: shell
 
    auto-annotate-pro
 
 Pending Tasks
 -------------
 
-* Integrate object detection and tracker.
-    * Store annotations of each frame in mem.
-    * Add display of bounding boxes as drawables.
+* Implement play of N number of video files (N != 4, but N <=4). Limit to 4 videos maximum.
+* Set play pause next frame, prev frame etc buttons to disabled stage when no video.
+* Add play pause icons to UI using `Google Material`_.
+
+* Integrate object detection.
+    * ☑ - Store annotations of each frame in memory.
+    * ☑ - Add display of bounding boxes.
+    * Replace BoundingBox as drawables.
+    * Add tracker.
     * Save/Load Annotations.
     * Save dataset-specific configuration.
+* Add masking to the frames to discard object detection for certain areas.
 * Add object detection correction
 * Add tracking correction
 * Add mouse event capture to rearrange videos.
 * Add track integration between two frames.
-* Add play pause icons to UI.
-* Set play pause next fram, prev frame etc buttons to disabled stage when no video.
+
 * Add speed change option for playback.
 * Make frame number text label and slider work.
 * Integrate github action/circleci
-* Implement play of N number of video files (N != 4).
+* ToDo - See Live Preview of object detection and tracking. This will help user catch errors quickly, instead of running object detection completely.
+* Use platformdirs_
+
+.. _Google Material: https://fonts.google.com/icons?icon.category=Audio%26Video
+.. _platformdirs: https://github.com/platformdirs/platformdirs
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multitrackpro-0.1.2/docs/Makefile` & `multitrackpro-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/docs/conf.py` & `multitrackpro-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/docs/installation.rst` & `multitrackpro-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/docs/make.bat` & `multitrackpro-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/docs/multitracker.core.io.rst` & `multitrackpro-0.1.3/docs/multitracker.core.io.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/docs/multitracker.core.rst` & `multitrackpro-0.1.3/docs/multitracker.core.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/docs/multitracker.rst` & `multitrackpro-0.1.3/docs/multitracker.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/multitracker/auto_annotate_pro.py` & `multitrackpro-0.1.3/multitracker/auto_annotate_pro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import logging
 import sys
-from datetime import datetime
-from typing import Optional, List
-
 from PyQt6.QtCore import Qt, QTimer
 from PyQt6.QtGui import QImage, QPixmap
 from PyQt6.QtWidgets import QApplication, QMainWindow, QFileDialog, QMessageBox, QProgressDialog
 from linetimer import linetimer, CodeTimer
+from typing import Optional, List
 
 from multitracker.config import PROFILE_CODE
 from multitracker.core.dataset_manager import DatasetManager
-from multitracker.core.tracker.Tracker import Tracker
+from multitracker.core.io.multi_video_manager import MultiVideoManager
+
+from multitracker.core.tracker.multi_tracker import MultiVideoTracker
 from multitracker.qt.my_main_window import Ui_MainWindow
 
 
 class VideoPlayer(QMainWindow, Ui_MainWindow):
     def __init__(self):
         super().__init__()
         self.setupUi(self)
         self.dataset_manager: Optional[DatasetManager] = None
         self.reinitialize()
         self.open_video_action.triggered.connect(self.open_video_folder)
-        self.open_video_folder()
 
     def connect_slot_and_signals(self):
         if self.dataset_manager is None:
             logging.warning("No dataset manager but various buttons are being enabled.")
 
         """ Enable media buttons once media is loaded. """
         self.video_play_pause_button.pressed.connect(self.toggle_play_video)
@@ -39,37 +38,37 @@
         """ Enable buttons """
         for button in [
             self.video_play_pause_button, self.video_prev_button, self.video_next_button,
             self.run_tracking_model_button, self.merge_tracks_button
         ]:
             button.setEnabled(True)
 
-    def reinitialize(self, video_files_path: Optional[List[str]] = None):
-        self.video_files_path = video_files_path
+    def reinitialize(self, video_files: Optional[List[str]] = None):
+        self.video_files = video_files
         self.pixmap = None
         self.current_frame_num = 0  # Move to dataset manager
         self.is_video_paused = True
         self.video_play_timer = QTimer()
         self.video_play_timer.timeout.connect(self.play_next_frame)  # execute `display_time`
         self.video_play_timer.setInterval(100)  # ToDo Set fps using video file.
 
         if self.dataset_manager is not None:
             pass  # Ask to save.
-        if video_files_path is None:
+        if video_files is None:
             self.dataset_manager = None
             return
 
-        self.video_files_path = list(filter(lambda video_file: "internal" not in video_file, self.video_files_path))
-        self.dataset_manager = DatasetManager(self.video_files_path)
+        self.video_files = list(filter(lambda video_file: "internal" not in video_file, self.video_files))
+        self.dataset_manager = DatasetManager(self.video_files)
         self.connect_slot_and_signals()
 
     def open_video_folder(self):
-        video_files_path, _ = QFileDialog.getOpenFileNames(self, 'Select Videos', "", "Video Files (*.avi *.mp4 *.mpg)")
-        if video_files_path:
-            self.reinitialize(video_files_path)
+        video_files, _ = QFileDialog.getOpenFileNames(self, 'Select Videos', "", "Video Files (*.avi *.mp4 *.mpg)")
+        if video_files:
+            self.reinitialize(video_files)
             self.update_frame(frame_num=0)  # Set the first frame to show video files are loaded.
 
     def toggle_play_video(self):
         self.is_video_paused = not self.is_video_paused
         if self.is_video_paused:
             self.video_play_timer.stop()
         else:
@@ -123,25 +122,32 @@
 
         # Run tracker on videos.
         update_progress_dialog_box = QProgressDialog(
             "Running tracker", "Stop tracking", 0, self.dataset_manager.get_video_length_in_frames(), self
         )
         update_progress_dialog_box.setWindowModality(Qt.WindowModality.WindowModal)
         update_progress_dialog_box.show()
-        tracker = Tracker()
-        tmp_dataset_manager = DatasetManager(video_files=self.video_files_path)
+        # ToDo - Move logic of loading video to tracker and pass progress_callback to tracker.
+        tracker = MultiVideoTracker(
+            video_files=self.video_files,
+            classes=[2, 5, 7]  # Only 2: 'car', 5: 'bus', 7: 'truck', Later allow customization.
+        )
+        tmp_dataset_manager = MultiVideoManager(video_files=self.video_files)
         for frame_num in range(self.dataset_manager.get_video_length_in_frames()):
-            frames = tmp_dataset_manager.get_data(frame_num=frame_num)
-            assert frames is not None, "Got None frames when fetching from tmp_dataset_manager"
+            frames = tmp_dataset_manager.read()
+            if frames is None:
+                logging.error(f"Got None frames when fetching from tmp_dataset_manager, frame number: {frame_num}")
+                continue
             tracker.track(frames)
             update_progress_dialog_box.setValue(frame_num)
             if update_progress_dialog_box.wasCanceled():
                 break
+        # Save all the values computed.
         update_progress_dialog_box.setValue(self.dataset_manager.get_video_length_in_frames())
-        self.dataset_manager.add_annotations(tracker.get_annotations())
+        self.dataset_manager.add_annotations(*tracker.get_annotations())
 
     def merge_tracks(self):
         pass
 
 
 def main():
     app = QApplication(sys.argv)
```

### Comparing `multitrackpro-0.1.2/multitracker/core/dataset_manager.py` & `multitrackpro-0.1.3/multitracker/core/dataset_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import logging
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 import numpy as np
+from ultralytics.yolo.utils.plotting import Annotator
 
 from multitracker.core.io.multi_video_manager import MultiVideoManager
 
 
 class DatasetManager:
 
     def __init__(self, video_files: List[str]):
         self.video_files = video_files
         self.videos_sync_reader = MultiVideoManager(video_files)
         self.current_frame_num = -1
         self.number_of_frames = self.videos_sync_reader.get_video_length_in_frames()
 
+        self.annotations = {}
+        self.label_to_name_map = None
+
     def tile_images(self, frames: List[np.ndarray]) -> np.ndarray:
         # ToDo Handle when number of images is not 4 or if image dimension are different.
 
         # Concatenate images horizontally
         row_1 = np.hstack(frames[:2])
         row_2 = np.hstack(frames[2:])
         return np.vstack([row_1, row_2])
@@ -36,19 +40,27 @@
             # Set frame calls are slow and will cause issue when user is trying to rewind back.
             # ToDo - Instead of using queue to store next frames, use cache that stores previous 60 and next 60 frames.
             self.videos_sync_reader.set_frame(self.current_frame_num)
             all_video_frames = self.videos_sync_reader.read()
 
         self.current_frame_num = frame_num
 
+        if self.annotations:
+            for (frame, video_filename) in zip(all_video_frames, self.video_files):
+                if len(self.annotations[video_filename]) >= frame_num+1:
+                    annotator = Annotator(frame)
+                    frame_annotations = self.annotations[video_filename][frame_num]
+                    for frame_annotation in frame_annotations:
+                        annotator.box_label(frame_annotation[:4], self.label_to_name_map[int(frame_annotation[5])])
+
         if all_video_frames is None:
             logging.error("all_video_frames are None, video read failed.")
             return None
         tiled_image = self.tile_images(all_video_frames)
         return tiled_image
 
     def get_video_length_in_frames(self) -> int:
         return self.videos_sync_reader.MIN_FRAME_COUNT
 
-    def add_annotations(self, annotations):
-        return None
-
+    def add_annotations(self, annotations, label_to_name_map: Dict[int, str]):
+        self.annotations = annotations
+        self.label_to_name_map = label_to_name_map
```

### Comparing `multitrackpro-0.1.2/multitracker/core/io/cached_video_reader.py` & `multitrackpro-0.1.3/multitracker/core/io/cached_video_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from queue import Queue
 from threading import Thread, Lock
 
 import cv2
 
 
 class CachedVideoReader:
-    def __init__(self, path, threaded_capture=True, queue_size=128):
-        self.stream = cv2.VideoCapture(str(path))
+    def __init__(self, video_file, threaded_capture=True, queue_size=128):
+        self.stream = cv2.VideoCapture(str(video_file))
         self.size = int(self.stream.get(cv2.CAP_PROP_FRAME_COUNT))
         self.stopped = False
         self.is_rewinds = False
         self.threaded_capture = threaded_capture
 
         if threaded_capture:
             self.lock = Lock()
@@ -43,24 +43,24 @@
 
     def read(self):
         if self.threaded_capture:
             return not self.stopped, self.Q.get()
         else:
             return self.stream.read()
 
+    def is_opened(self):
+        return self.stream.isOpened()
+
     def release(self):
         if self.threaded_capture:
             self.stopped = True
             self.thread.join()
         else:
             self.stream.release()
 
-    def isOpened(self):
-        return self.stream.isOpened()
-
     def set_frame(self, frame_num: int):
         logging.debug(f"Changing frame number to {frame_num}")
         if self.threaded_capture:
             self.is_rewinds = True
             with self.lock:
                 self.stream.set(cv2.CAP_PROP_POS_FRAMES, frame_num)
                 while not self.Q.empty():  # Empty the queue
```

### Comparing `multitrackpro-0.1.2/multitracker/core/io/multi_video_manager.py` & `multitrackpro-0.1.3/multitracker/core/io/multi_video_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import numpy as np
 
 from multitracker.core.io.cached_video_reader import CachedVideoReader
 
 
 class MultiVideoManager:
-    def __init__(self, paths: List[str], threaded_capture=True, queue_size=128):
+    def __init__(self, video_files: List[str], threaded_capture=True, queue_size=128):
         self.file_video_streamers: List[CachedVideoReader] = list(map(
-            lambda x: CachedVideoReader(x, threaded_capture=threaded_capture, queue_size=queue_size), paths
+            lambda x: CachedVideoReader(x, threaded_capture=threaded_capture, queue_size=queue_size), video_files
         ))
         self.MIN_FRAME_COUNT = min(list(map(lambda x: x.size, self.file_video_streamers)))
         print(self.MIN_FRAME_COUNT)
 
     def get_video_length_in_frames(self) -> int:
         return self.MIN_FRAME_COUNT
```

### Comparing `multitrackpro-0.1.2/multitracker/qt/my_main_window.py` & `multitrackpro-0.1.3/multitracker/qt/my_main_window.py`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.2/multitrackpro.egg-info/PKG-INFO` & `multitrackpro-0.1.3/multitrackpro.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: multitrackpro
-Version: 0.1.2
-Summary: A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
+Version: 0.1.3
+Summary: A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.
 Home-page: https://github.com/saurabheights/multitrackpro
 Author: Saurabh Khanduja
 Author-email: pixelperceive@gmail.com
 License: GNU General Public License v3
 Keywords: multitrackpro,annotation,labelling,machine-learning,deep-learning,vision,ML,DL,AI,YOLO
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 .. image:: https://readthedocs.org/projects/multitrackpro/badge/?version=latest
         :target: https://multitrackpro.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
 
-A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
+A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://readthedocs.org/projects/multitrackpro/.
 
 
 Features
@@ -59,29 +59,39 @@
 .. code-block:: shell
 
    auto-annotate-pro
 
 Pending Tasks
 -------------
 
-* Integrate object detection and tracker.
-    * Store annotations of each frame in mem.
-    * Add display of bounding boxes as drawables.
+* Implement play of N number of video files (N != 4, but N <=4). Limit to 4 videos maximum.
+* Set play pause next frame, prev frame etc buttons to disabled stage when no video.
+* Add play pause icons to UI using `Google Material`_.
+
+* Integrate object detection.
+    * ☑ - Store annotations of each frame in memory.
+    * ☑ - Add display of bounding boxes.
+    * Replace BoundingBox as drawables.
+    * Add tracker.
     * Save/Load Annotations.
     * Save dataset-specific configuration.
+* Add masking to the frames to discard object detection for certain areas.
 * Add object detection correction
 * Add tracking correction
 * Add mouse event capture to rearrange videos.
 * Add track integration between two frames.
-* Add play pause icons to UI.
-* Set play pause next fram, prev frame etc buttons to disabled stage when no video.
+
 * Add speed change option for playback.
 * Make frame number text label and slider work.
 * Integrate github action/circleci
-* Implement play of N number of video files (N != 4).
+* ToDo - See Live Preview of object detection and tracking. This will help user catch errors quickly, instead of running object detection completely.
+* Use platformdirs_
+
+.. _Google Material: https://fonts.google.com/icons?icon.category=Audio%26Video
+.. _platformdirs: https://github.com/platformdirs/platformdirs
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -102,7 +112,13 @@
 
 * Added video player that plays exactly 4 videos.
 
 0.1.2 (2023-06-15)
 ------------------
 
 * BugFixes
+
+0.1.3 (2023-07-30)
+------------------
+
+* Integrated Object Detection for all videos.
+* Added rendering of object detection results.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multitrackpro-0.1.2/setup.py` & `multitrackpro-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python
-
-"""The setup script."""
-
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
-    "boxmot>=10.0.13",
+    "ultralytics>=8.0.125",  # For object detection
     "linetimer>=0.1.5",
-    "numpy==1.23.1",  # See https://github.com/mikel-brostrom/yolo_tracking/blame/master/requirements.txt
     "opencv-python>=4.7.0",
     "pyqt6>=6.5.1",
 ]
 
 test_requirements = [ ]
 
 setup(
+    # Often evolving fields first
+    name='multitrackpro',
+    version='0.1.3',
+    description="A multi-camera multi-object tracking software with its own labelling tool to annotate datasets.",
+    # Almost static fields below
     author="Saurabh Khanduja",
     author_email='pixelperceive@gmail.com',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
@@ -38,27 +39,24 @@
         'Programming Language :: Python :: 3.10',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Recognition',
         'Topic :: Scientific/Engineering :: Image Processing',
     ],
-    description="A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.",
     entry_points = {
         'console_scripts': ['auto-annotate-pro=auto_annotate_pro:main'],
     },
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     include_package_data=True,
     keywords='multitrackpro, annotation, labelling, machine-learning, deep-learning, vision, ML, DL, AI, YOLO',
-    name='multitrackpro',
     packages=find_packages(include=['multitracker', 'multitracker.*']),
     python_requires='>=3.6',
     scripts=['multitracker/auto_annotate_pro.py'],
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/saurabheights/multitrackpro',
-    version='0.1.2  ',
     zip_safe=False,
 )
```

