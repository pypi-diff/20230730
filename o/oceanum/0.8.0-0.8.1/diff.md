# Comparing `tmp/oceanum-0.8.0.tar.gz` & `tmp/oceanum-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.8.0.tar", last modified: Mon Jul 24 03:58:58 2023, max compression
+gzip compressed data, was "oceanum-0.8.1.tar", last modified: Sun Jul 30 21:26:15 2023, max compression
```

## Comparing `oceanum-0.8.0.tar` & `oceanum-0.8.1.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.823247 oceanum-0.8.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.8.0/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.8.0/HISTORY.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.8.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.8.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-07-24 03:58:58.823247 oceanum-0.8.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.8.0/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.811247 oceanum-0.8.0/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.811247 oceanum-0.8.0/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.811247 oceanum-0.8.0/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.807247 oceanum-0.8.0/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.815247 oceanum-0.8.0/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.8.0/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.8.0/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.8.0/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.815247 oceanum-0.8.0/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-07-24 02:08:43.000000 oceanum-0.8.0/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.819247 oceanum-0.8.0/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    21008 2023-07-24 03:18:35.000000 oceanum-0.8.0/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-24 03:03:59.000000 oceanum-0.8.0/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.8.0/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7849 2023-07-24 03:17:32.000000 oceanum-0.8.0/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.8.0/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.815247 oceanum-0.8.0/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-24 03:58:58.000000 oceanum-0.8.0/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-24 03:58:58.823247 oceanum-0.8.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.8.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.819247 oceanum-0.8.0/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-24 03:58:58.823247 oceanum-0.8.0/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.8.0/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.8.0/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.8.0/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.928190 oceanum-0.8.1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.8.1/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.8.1/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.8.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.8.1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1089 2023-07-30 21:26:15.928190 oceanum-0.8.1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.8.1/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.916190 oceanum-0.8.1/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.916190 oceanum-0.8.1/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.916190 oceanum-0.8.1/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.920190 oceanum-0.8.1/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.8.1/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.8.1/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.920190 oceanum-0.8.1/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-07-30 21:26:13.000000 oceanum-0.8.1/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.924190 oceanum-0.8.1/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.8.1/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-30 20:00:11.000000 oceanum-0.8.1/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7849 2023-07-30 20:00:11.000000 oceanum-0.8.1/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.8.1/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.920190 oceanum-0.8.1/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1089 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1372 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      133 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-30 21:26:15.932190 oceanum-0.8.1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1282 2023-07-30 21:04:55.000000 oceanum-0.8.1/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.924190 oceanum-0.8.1/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.928190 oceanum-0.8.1/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.8.1/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.8.1/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_video_compat.py
```

### Comparing `oceanum-0.8.0/CONTRIBUTING.rst` & `oceanum-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/LICENSE` & `oceanum-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/PKG-INFO` & `oceanum-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
@@ -38,17 +38,7 @@
 
 * Simple pythonic access to the Oceanum datamesh
 
 Credits
 -------
 
 This package was developed by `Oceanum Numerical <https://www.oceanum.science>`_, with input from our development partners and contributors.
-
-
-=======
-History
-=======
-
-0.4.2 (2022-05-20)
-------------------
-
-* First release on PyPI.
```

### Comparing `oceanum-0.8.0/README.rst` & `oceanum-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/Makefile` & `oceanum-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/api.rst` & `oceanum-0.8.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/conf.py` & `oceanum-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/index.rst` & `oceanum-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/installation.rst` & `oceanum-0.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/make.bat` & `oceanum-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/oceanum.datamesh.rst` & `oceanum-0.8.1/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/docs/usage.rst` & `oceanum-0.8.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/oceanum/datamesh/catalog.py` & `oceanum-0.8.1/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/oceanum/datamesh/connection.py` & `oceanum-0.8.1/oceanum/datamesh/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from .catalog import Catalog
 from .query import Query, Stage, Container, TimeFilter, GeoFilter
 from .zarr import zarr_write
 from .exceptions import DatameshConnectError, DatameshQueryError, DatameshWriteError
 
 DEFAULT_CONFIG = {"DATAMESH_SERVICE": "https://datamesh.oceanum.io"}
 
+DASK_QUERY_SIZE = 1000000000  # 1GB
+
 
 def json_serial(obj):
     """JSON serializer for objects not serializable by default json code"""
 
     if isinstance(obj, (datetime.datetime, datetime.date)):
         return obj.isoformat()
     raise TypeError("Type %s not serializable" % type(obj))
@@ -136,15 +138,18 @@
         else:
             resp = requests.post(
                 f"{self._proto}://{self._host}/datasource/",
                 data=datasource.json(by_alias=True),
                 headers={**self._auth_headers, "Content-Type": "application/json"},
             )
         if resp.status_code >= 300:
-            msg = resp.json()["detail"]
+            try:
+                msg = resp.json()["detail"]
+            except:
+                msg = resp.text
             raise DatameshConnectError(msg)
         return resp
 
     def _delete(self, datasource_id):
         resp = requests.delete(
             f"{self._gateway}/data/{datasource_id}",
             headers=self._auth_headers,
@@ -211,31 +216,36 @@
 
     def _stage_request(self, query, cache=False):
         qhash = hashlib.sha224(query.model_dump_json().encode()).hexdigest()
 
         resp = requests.post(
             f"{self._gateway}/oceanql/stage/",
             headers=self._auth_headers,
-            data=query.json(),
+            data=query.model_dump_json(),
         )
         if resp.status_code >= 400:
             msg = resp.json()["detail"]
             raise DatameshQueryError(msg)
         elif resp.status_code == 204:
             return None
         else:
             return Stage(**resp.json())
 
-    def _query(self, query, use_dask=True):
+    def _query(self, query, use_dask=False):
         if not isinstance(query, Query):
             query = Query(**query)
         stage = self._stage_request(query)
         if stage is None:
             warnings.warn("No data found for query")
             return None
+        elif stage.size > DASK_QUERY_SIZE:
+            warnings.warn(
+                "Query is too large for direct access, using lazy access with dask"
+            )
+            use_dask = True
         if use_dask and (stage.container == Container.Dataset):
             mapper = self._zarr_proxy(stage.qhash)
             return xarray.open_zarr(
                 mapper, consolidated=True, decode_coords="all", mask_and_scale=True
             )
         else:
             transfer_format = (
@@ -388,40 +398,40 @@
 
 
         Returns:
             coroutine<Union[:obj:`pandas.DataFrame`, :obj:`geopandas.GeoDataFrame`, :obj:`xarray.Dataset`]>: The datasource container
         """
         return self.load_datasource(datasource_id, parameters, use_dask)
 
-    def query(self, query=None, *, use_dask=True, **query_keys):
+    def query(self, query=None, *, use_dask=False, **query_keys):
         """Make a datamesh query
 
         Args:
             query (Union[:obj:`oceanum.datamesh.Query`, dict]): Datamesh query as a query object or a valid query dictionary
 
         Kwargs:
-            use_dask (bool, optional): Load datasource as a dask enabled datasource if possible. Defaults to True.
+            use_dask (bool, optional): Load datasource as a dask enabled datasource if possible. Defaults to False.
             **query_keys: Keywords form of query, for example datamesh.query(datasource="my_datasource")
 
         Returns:
             Union[:obj:`pandas.DataFrame`, :obj:`geopandas.GeoDataFrame`, :obj:`xarray.Dataset`]: The datasource container
         """
         if query is None:
             query = Query(**query_keys)
         return self._query(query, use_dask)
 
     @asyncwrapper
-    async def query_async(self, query, *, use_dask=True, **query_keys):
+    async def query_async(self, query, *, use_dask=False, **query_keys):
         """Make a datamesh query asynchronously
 
         Args:
             query (Union[:obj:`oceanum.datamesh.Query`, dict]): Datamesh query as a query object or a valid query dictionary
 
         Kwargs:
-            use_dask (bool, optional): Load datasource as a dask enabled datasource if possible. Defaults to True.
+            use_dask (bool, optional): Load datasource as a dask enabled datasource if possible. Defaults to False.
             loop: event loop. default=None will use :obj:`asyncio.get_running_loop()`
             executor: :obj:`concurrent.futures.Executor` instance. default=None will use the default executor
             **query_keys: Keywords form of query, for example datamesh.query(datasource="my_datasource")
 
 
         Returns:
             Coroutine<Union[:obj:`pandas.DataFrame`, :obj:`geopandas.GeoDataFrame`, :obj:`xarray.Dataset`]>: The datasource container
```

### Comparing `oceanum-0.8.0/oceanum/datamesh/datasource.py` & `oceanum-0.8.1/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/oceanum/datamesh/query.py` & `oceanum-0.8.1/oceanum/datamesh/query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/oceanum/datamesh/zarr.py` & `oceanum-0.8.1/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/oceanum.egg-info/PKG-INFO` & `oceanum-0.8.1/oceanum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
@@ -38,17 +38,7 @@
 
 * Simple pythonic access to the Oceanum datamesh
 
 Credits
 -------
 
 This package was developed by `Oceanum Numerical <https://www.oceanum.science>`_, with input from our development partners and contributors.
-
-
-=======
-History
-=======
-
-0.4.2 (2022-05-20)
-------------------
-
-* First release on PyPI.
```

### Comparing `oceanum-0.8.0/oceanum.egg-info/SOURCES.txt` & `oceanum-0.8.1/oceanum.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 AUTHORS.rst
 CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
 docs/about.rst
```

### Comparing `oceanum-0.8.0/setup.py` & `oceanum-0.8.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open("HISTORY.rst") as history_file:
-    history = history_file.read()
-
 import oceanum
 
 requirements = [
     "click",
     "aiohttp",
     "fsspec",
     "numpy",
@@ -24,15 +21,15 @@
     "zarr",
     "h5netcdf",
     "shapely",
     "orjson",
     "requests",
     "pyarrow",
     "python-snappy",
-    "geojson-pydantic",
+    "geojson-pydantic>=1.0",
 ]
 
 setup_requirements = [
     "pytest-runner",
 ]
 
 test_requirements = [
@@ -46,15 +43,15 @@
     entry_points={
         "console_scripts": [
             "oceanum=oceanum.cli:main",
         ],
     },
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + "\n\n" + history,
+    long_description=readme,
     include_package_data=True,
     keywords="oceanum",
     documentation="https://oceanum-python.readthedocs.io",
     name="oceanum",
     packages=find_packages(exclude=["tests", "docs"]),
     setup_requires=setup_requirements,
     test_suite="tests",
```

### Comparing `oceanum-0.8.0/tests/data/grid_data_1.nc` & `oceanum-0.8.1/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/data/ocean_test_1.mp4` & `oceanum-0.8.1/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/data/point_data_1.csv` & `oceanum-0.8.1/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_catalog.py` & `oceanum-0.8.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_datamesh_connect.py` & `oceanum-0.8.1/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_datamesh_load.py` & `oceanum-0.8.1/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_datamesh_query.py` & `oceanum-0.8.1/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_datamesh_write.py` & `oceanum-0.8.1/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_datasource.py` & `oceanum-0.8.1/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_query.py` & `oceanum-0.8.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.0/tests/test_video_compat.py` & `oceanum-0.8.1/tests/test_video_compat.py`

 * *Files identical despite different names*

