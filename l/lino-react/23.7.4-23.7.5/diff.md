# Comparing `tmp/lino_react-23.7.4.tar.gz` & `tmp/lino_react-23.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.7.4.tar", last modified: Wed Jul 19 05:45:05 2023, max compression
+gzip compressed data, was "lino_react-23.7.5.tar", last modified: Sun Jul 30 09:57:59 2023, max compression
```

## Comparing `lino_react-23.7.4.tar` & `lino_react-23.7.5.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.702385 lino_react-23.7.4/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.7.4/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.7.4/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-07-19 05:45:05.702385 lino_react-23.7.4/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.7.4/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.7.4/lino_react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.7.4/lino_react/react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react/react/__pycache__/
--rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-23 05:20:50.000000 lino_react-23.7.4/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)     4010 2023-07-05 02:47:39.000000 lino_react-23.7.4/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-06-23 05:20:51.000000 lino_react-23.7.4/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    18481 2023-07-18 09:49:19.000000 lino_react-23.7.4/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-06-23 08:10:05.000000 lino_react-23.7.4/lino_react/react/__pycache__/views.cpython-310.pyc
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react/react/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react/react/config/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.7.4/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.7.4/lino_react/react/config/react/main.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.7.4/lino_react/react/config/react/service-worker.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3952 2023-07-05 02:47:35.000000 lino_react-23.7.4/lino_react/react/icons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.7.4/lino_react/react/index.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.7.4/lino_react/react/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    29449 2023-07-18 09:49:16.000000 lino_react-23.7.4/lino_react/react/renderer.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react/react/static/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.702385 lino_react-23.7.4/lino_react/react/static/media/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.7.4/lino_react/react/static/media/color.6441e63a.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.7.4/lino_react/react/static/media/color.c7a33805.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.7.4/lino_react/react/static/media/line.567f5738.gif
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.7.4/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.702385 lino_react-23.7.4/lino_react/react/static/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)  1788256 2023-07-19 00:18:09.000000 lino_react-23.7.4/lino_react/react/static/react/main.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.7.4/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.7.4/lino_react/react/views.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-07-19 05:44:37.000000 lino_react-23.7.4/lino_react/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-19 05:45:05.698385 lino_react-23.7.4/lino_react.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-07-19 05:45:05.000000 lino_react-23.7.4/lino_react.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-07-19 05:45:05.000000 lino_react-23.7.4/lino_react.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-19 05:45:05.000000 lino_react-23.7.4/lino_react.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.7.4/lino_react.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-07-19 05:45:05.000000 lino_react-23.7.4/lino_react.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-07-19 05:45:05.000000 lino_react-23.7.4/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-19 05:45:05.702385 lino_react-23.7.4/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.7.4/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.7.4/tasks.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.713161 lino_react-23.7.5/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.7.5/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.7.5/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-07-30 09:57:59.713161 lino_react-23.7.5/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.7.5/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4628 2023-06-13 10:46:31.000000 lino_react-23.7.5/lino_react/react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/react/__pycache__/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3382 2023-06-15 05:49:26.000000 lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4030 2023-07-10 10:58:39.000000 lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      160 2023-03-30 05:54:52.000000 lino_react-23.7.5/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/models.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18587 2023-07-24 14:50:37.000000 lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-06-12 10:17:24.000000 lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-38.pyc
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.701161 lino_react-23.7.5/lino_react/react/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/react/config/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1910 2023-07-24 06:45:56.000000 lino_react-23.7.5/lino_react/react/config/react/main.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-07-30 07:00:19.000000 lino_react-23.7.5/lino_react/react/config/react/service-worker.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3952 2023-07-10 10:58:36.000000 lino_react-23.7.5/lino_react/react/icons.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/index.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-03-30 05:51:42.000000 lino_react-23.7.5/lino_react/react/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    29603 2023-07-24 14:50:33.000000 lino_react-23.7.5/lino_react/react/renderer.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.701161 lino_react-23.7.5/lino_react/react/static/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.709161 lino_react-23.7.5/lino_react/react/static/media/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.713161 lino_react-23.7.5/lino_react/react/static/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)  1790540 2023-07-30 07:00:19.000000 lino_react-23.7.5/lino_react/react/static/react/main.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-07-30 07:00:19.000000 lino_react-23.7.5/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-06-11 15:16:59.000000 lino_react-23.7.5/lino_react/react/views.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-07-30 09:57:19.000000 lino_react-23.7.5/lino_react/setup_info.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.7.5/lino_react.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-07-30 09:57:59.713161 lino_react-23.7.5/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.7.5/setup.py
```

### Comparing `lino_react-23.7.4/COPYING` & `lino_react-23.7.5/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/PKG-INFO` & `lino_react-23.7.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino_react
-Version: 23.7.4
+Version: 23.7.5
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
 Classifier:   Environment :: Web Environment
 Classifier:   Framework :: Django
 Classifier:   Intended Audience :: Developers
 Classifier:   Intended Audience :: System Administrators
@@ -25,9 +23,7 @@
 
 
 The React front end for Lino
 
 Project homepage is https://gitlab.com/lino-framework/react
 
 
-
-
```

### Comparing `lino_react-23.7.4/lino_react/react/__init__.py` & `lino_react-23.7.5/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/__pycache__/__init__.cpython-310.pyc` & `lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 10:30:58 2023 UTC, .py size: 4628 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6245 8864 1412 0000  o.......bE.d....
+00000000: 6f0d 0d0a 0000 0000 0749 8864 1412 0000  o........I.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6506 8303 5a06 6407 5300 2908 7a93 0a41  e...Z.d.S.).z..A
 00000070: 2075 7365 7220 696e 7465 7266 6163 6520   user interface 
@@ -31,181 +31,182 @@
 000001e0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
 000001f0: 0043 0000 0073 1a00 0000 6401 6402 6c00  .C...s....d.d.l.
 00000200: 6d01 7d02 0100 7c02 7c00 8301 7c00 5f00  m.}...|.|...|._.
 00000210: 6400 5300 2903 4ee9 0100 0000 2901 da08  d.S.).N.....)...
 00000220: 5265 6e64 6572 6572 2902 da08 7265 6e64  Renderer)...rend
 00000230: 6572 6572 7208 0000 0029 03da 0473 656c  ererr....)...sel
 00000240: 66da 066b 6572 6e65 6c72 0800 0000 a900  f..kernelr......
-00000250: 720c 0000 00fa 312f 686f 6d65 2f6c 7563  r.....1/home/luc
-00000260: 2f77 6f72 6b2f 7265 6163 742f 6c69 6e6f  /work/react/lino
-00000270: 5f72 6561 6374 2f72 6561 6374 2f5f 5f69  _react/react/__i
-00000280: 6e69 745f 5f2e 7079 da0a 6f6e 5f75 695f  nit__.py..on_ui_
-00000290: 696e 6974 2500 0000 7304 0000 000c 010e  init%...s.......
-000002a0: 017a 1150 6c75 6769 6e2e 6f6e 5f75 695f  .z.Plugin.on_ui_
-000002b0: 696e 6974 6302 0000 0000 0000 0000 0000  initc...........
-000002c0: 0008 0000 0009 0000 0043 0000 0073 7a00  .........C...sz.
-000002d0: 0000 7400 7c00 6a01 7c00 6a02 7c01 7c00  ..t.|.j.|.j.|.|.
-000002e0: 6a02 6a03 6a04 7405 a006 a100 7407 6400  j.j.j.t.....t.d.
-000002f0: 6401 8d07 7d02 6402 7d03 7c00 6a02 6a03  d...}.d.}.|.j.j.
-00000300: 6a08 6a01 6a09 7d04 7c00 6a02 6a0a 4400  j.j.j.}.|.j.j.D.
-00000310: 5d1b 7d05 7c05 6a0b 4400 5d15 7d06 7c04  ].}.|.j.D.].}.|.
-00000320: a00c 7c06 a101 7d07 7c03 6403 7c07 6a0d  ..|...}.|.d.|.j.
-00000330: 6405 6900 7c02 a401 8e01 9b00 6404 9d03  d.i.|.......d...
-00000340: 3700 7d03 7124 711f 7c03 5300 2906 4e29  7.}.q$q.|.S.).N)
-00000350: 07da 0e65 7874 6a73 5f72 656e 6465 7265  ...extjs_rendere
-00000360: 72da 0473 6974 65da 0873 6574 7469 6e67  r..site..setting
-00000370: 73da 046c 696e 6fda 086c 616e 6775 6167  s..lino..languag
-00000380: 6572 0300 0000 da05 6578 746a 73da 007a  er......extjs..z
-00000390: 083c 7363 7269 7074 3e7a 093c 2f73 6372  .<script>z.</scr
-000003a0: 6970 743e 720c 0000 0029 0eda 0464 6963  ipt>r....)...dic
-000003b0: 7472 0900 0000 7210 0000 00da 0770 6c75  tr....r......plu
-000003c0: 6769 6e73 7212 0000 0072 0200 0000 da0c  ginsr....r......
-000003d0: 6765 745f 6c61 6e67 7561 6765 7203 0000  get_languager...
-000003e0: 00da 056a 696e 6a61 da09 6a69 6e6a 615f  ...jinja..jinja_
-000003f0: 656e 76da 0e73 6f72 7465 645f 706c 7567  env..sorted_plug
-00000400: 696e 73da 1073 6974 655f 6a73 5f73 6e69  ins..site_js_sni
-00000410: 7070 6574 73da 0c67 6574 5f74 656d 706c  ppets..get_templ
-00000420: 6174 65da 0672 656e 6465 7229 0872 0a00  ate..render).r..
-00000430: 0000 7211 0000 00da 0763 6f6e 7465 7874  ..r......context
-00000440: da02 6a73 da03 656e 76da 0170 da07 736e  ..js..env..p..sn
-00000450: 6970 7065 74da 0874 656d 706c 6174 6572  ippet..templater
-00000460: 0c00 0000 720c 0000 0072 0d00 0000 da15  ....r....r......
-00000470: 6c6f 6164 5f73 6974 655f 6a73 5f73 6e69  load_site_js_sni
-00000480: 7070 6574 732b 0000 0073 2200 0000 0201  ppets+...s".....
-00000490: 0401 0401 0201 0801 0601 0201 0201 06f9  ................
-000004a0: 040a 0e01 0c02 0a01 0a01 1e01 02fe 0404  ................
-000004b0: 7a1c 506c 7567 696e 2e6c 6f61 645f 7369  z.Plugin.load_si
-000004c0: 7465 5f6a 735f 736e 6970 7065 7473 6301  te_js_snippetsc.
-000004d0: 0000 0000 0000 0000 0000 0006 0000 0014  ................
-000004e0: 0000 0043 0000 0073 5a01 0000 6401 6402  ...C...sZ...d.d.
-000004f0: 6c00 6d01 7d01 0100 6401 6403 6c00 6d02  l.m.}...d.d.l.m.
-00000500: 7d02 0100 6404 6405 6c03 6d04 7d03 0100  }...d.d.l.m.}...
-00000510: 6406 7d04 7c01 7c04 6407 1700 7c03 6a05  d.}.|.|.d...|.j.
-00000520: a006 a100 8302 7c01 7c04 6408 1700 7c03  ......|.|.d...|.
-00000530: 6a07 a006 a100 8302 7c01 7c04 6409 1700  j.......|.|.d...
-00000540: 7c03 6a08 a006 a100 8302 7c01 7c04 640a  |.j.......|.|.d.
-00000550: 1700 7c03 6a09 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
-00000560: 640b 1700 7c03 6a0a a006 a100 8302 7c01  d...|.j.......|.
-00000570: 640c 7c03 6a0b a006 a100 8302 7c01 7c04  d.|.j.......|.|.
-00000580: 640d 1700 7c03 6a0c a006 a100 8302 7c02  d...|.j.......|.
-00000590: 640e 7c03 6a0d a006 a100 8302 7c01 7c04  d.|.j.......|.|.
-000005a0: 640f 1700 7c03 6a0e a006 a100 8302 7c01  d...|.j.......|.
-000005b0: 7c04 6410 1700 7c03 6a0f a006 a100 8302  |.d...|.j.......
-000005c0: 7c01 7c04 6411 1700 7c03 6a0e a006 a100  |.|.d...|.j.....
-000005d0: 8302 7c01 7c04 6412 1700 7c03 6a0f a006  ..|.|.d...|.j...
-000005e0: a100 8302 7c01 7c04 6413 1700 7c03 6a10  ....|.|.d...|.j.
-000005f0: a006 a100 8302 7c01 7c04 6414 1700 7c03  ......|.|.d...|.
-00000600: 6a11 a006 a100 8302 7c01 7c04 6415 1700  j.......|.|.d...
-00000610: 7c03 6a11 a006 a100 8302 7c01 7c04 6416  |.j.......|.|.d.
-00000620: 1700 7c03 6a12 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
-00000630: 6417 1700 7c03 6a13 a006 a100 8302 6711  d...|.j.......g.
-00000640: 7d05 7c05 5300 2918 4e72 0100 0000 2901  }.|.S.).Nr....).
-00000650: da07 7265 5f70 6174 6829 01da 0470 6174  ..re_path)...pat
-00000660: 6872 0700 0000 2901 da05 7669 6577 73fa  hr....)...views.
-00000670: 015e fa01 247a 0d75 7365 722f 7365 7474  .^..$z.user/sett
-00000680: 696e 6773 7a05 6175 7468 247a 056e 756c  ingsz.auth$z.nul
-00000690: 6c2f 7a25 283f 503c 776f 726b 626f 783e  l/z%(?P<workbox>
-000006a0: 776f 726b 626f 782d 5b61 2d7a 412d 5a30  workbox-[a-zA-Z0
-000006b0: 2d39 5d2a 2e6a 7329 247a 1173 6572 7669  -9]*.js)$z.servi
-000006c0: 6365 2d77 6f72 6b65 722e 6a73 7a0e 6170  ce-worker.jsz.ap
-000006d0: 692f 6d61 696e 5f68 746d 6c24 7a15 6461  i/main_html$z.da
-000006e0: 7368 626f 6172 642f 3c69 6e74 3a69 6e64  shboard/<int:ind
-000006f0: 6578 3e7a 2a72 6573 7466 756c 2f28 3f50  ex>z*restful/(?P
-00000700: 3c61 7070 5f6c 6162 656c 3e5c 772b 292f  <app_label>\w+)/
-00000710: 283f 503c 6163 746f 723e 5c77 2b29 247a  (?P<actor>\w+)$z
-00000720: 3572 6573 7466 756c 2f28 3f50 3c61 7070  5restful/(?P<app
-00000730: 5f6c 6162 656c 3e5c 772b 292f 283f 503c  _label>\w+)/(?P<
-00000740: 6163 746f 723e 5c77 2b29 2f28 3f50 3c70  actor>\w+)/(?P<p
-00000750: 6b3e 2e2b 2924 7a26 6170 692f 283f 503c  k>.+)$z&api/(?P<
-00000760: 6170 705f 6c61 6265 6c3e 5c77 2b29 2f28  app_label>\w+)/(
-00000770: 3f50 3c61 6374 6f72 3e5c 772b 2924 7a34  ?P<actor>\w+)$z4
-00000780: 6170 692f 283f 503c 6170 705f 6c61 6265  api/(?P<app_labe
-00000790: 6c3e 5c77 2b29 2f28 3f50 3c61 6374 6f72  l>\w+)/(?P<actor
-000007a0: 3e5c 772b 292f 283f 503c 706b 3e5b 5e2f  >\w+)/(?P<pk>[^/
-000007b0: 5d2b 2924 7a42 7661 6c75 6573 2f28 3f50  ]+)$zBvalues/(?P
-000007c0: 3c61 7070 5f6c 6162 656c 3e5c 772b 292f  <app_label>\w+)/
-000007d0: 283f 503c 6163 746f 723e 5c77 2b29 2f28  (?P<actor>\w+)/(
-000007e0: 3f50 3c70 6b3e 2e2b 292f 283f 503c 6669  ?P<pk>.+)/(?P<fi
-000007f0: 656c 643e 2e2b 2924 7a2a 6368 6f69 6365  eld>.+)$z*choice
-00000800: 732f 283f 503c 6170 705f 6c61 6265 6c3e  s/(?P<app_label>
-00000810: 5c77 2b29 2f28 3f50 3c61 6374 6f72 3e5c  \w+)/(?P<actor>\
-00000820: 772b 2924 7a39 6368 6f69 6365 732f 283f  w+)$z9choices/(?
-00000830: 503c 6170 705f 6c61 6265 6c3e 5c77 2b29  P<app_label>\w+)
-00000840: 2f28 3f50 3c61 6374 6f72 3e5c 772b 292f  /(?P<actor>\w+)/
-00000850: 283f 503c 6669 656c 643e 5c77 2b29 247a  (?P<field>\w+)$z
-00000860: 4761 7063 686f 6963 6573 2f28 3f50 3c61  Gapchoices/(?P<a
-00000870: 7070 5f6c 6162 656c 3e5c 772b 292f 283f  pp_label>\w+)/(?
-00000880: 503c 6163 746f 723e 5c77 2b29 2f28 3f50  P<actor>\w+)/(?P
-00000890: 3c61 6e3e 5c77 2b29 2f28 3f50 3c66 6965  <an>\w+)/(?P<fie
-000008a0: 6c64 3e5c 772b 2924 7a0c 6368 6f69 6365  ld>\w+)$z.choice
-000008b0: 6c69 7374 732f 2914 da0b 646a 616e 676f  lists/)...django
-000008c0: 2e75 726c 7372 2600 0000 7227 0000 0072  .urlsr&...r'...r
-000008d0: 1500 0000 7228 0000 00da 0549 6e64 6578  ....r(.....Index
-000008e0: da07 6173 5f76 6965 77da 0c55 7365 7253  ..as_view..UserS
-000008f0: 6574 7469 6e67 73da 0c41 7574 6865 6e74  ettings..Authent
-00000900: 6963 6174 65da 044e 756c 6cda 0657 4256  icate..Null..WBV
-00000910: 6965 77da 0653 5756 6965 77da 084d 6169  iew..SWView..Mai
-00000920: 6e48 746d 6cda 0d44 6173 6862 6f61 7264  nHtml..Dashboard
-00000930: 4974 656d da07 4170 694c 6973 74da 0a41  Item..ApiList..A
-00000940: 7069 456c 656d 656e 74da 0c44 656c 6179  piElement..Delay
-00000950: 6564 5661 6c75 65da 0743 686f 6963 6573  edValue..Choices
-00000960: da12 4163 7469 6f6e 5061 7261 6d43 686f  ..ActionParamCho
-00000970: 6963 6573 da0f 4368 6f69 6365 4c69 7374  ices..ChoiceList
-00000980: 4d6f 6465 6c29 0672 0a00 0000 da03 7572  Model).r......ur
-00000990: 6c72 2700 0000 7228 0000 00da 0272 78da  lr'...r(.....rx.
-000009a0: 0475 726c 7372 0c00 0000 720c 0000 0072  .urlsr....r....r
-000009b0: 0d00 0000 da0c 6765 745f 7061 7474 6572  ......get_patter
-000009c0: 6e73 4000 0000 7356 0000 000c 030c 010c  ns@...sV........
-000009d0: 0104 0212 0612 0112 0112 0108 0208 0102  ................
-000009e0: ff0e 0212 020e 0208 0308 0102 ff08 0208  ................
-000009f0: 0102 ff08 0308 0102 ff08 0208 0102 ff08  ................
-00000a00: 0408 0102 ff08 0208 0102 ff08 0208 0202  ................
-00000a10: fe08 0308 0202 fe08 0808 0102 ff04 d704  ................
-00000a20: 2d7a 1350 6c75 6769 6e2e 6765 745f 7061  -z.Plugin.get_pa
-00000a30: 7474 6572 6e73 6304 0000 0000 0000 0000  tternsc.........
-00000a40: 0000 0006 0000 0007 0000 004f 0000 0073  ...........O...s
-00000a50: 2c00 0000 7c00 6a00 6401 6402 7c02 6a01  ,...|.j.d.d.|.j.
-00000a60: a002 6403 6404 a102 7403 7c03 8301 6704  ..d.d...t.|...g.
-00000a70: 7c04 a201 5200 6900 7c05 a401 8e01 5300  |...R.i.|.....S.
-00000a80: 2905 4efa 0123 da03 6170 69da 012e fa01  ).N..#..api.....
-00000a90: 2f29 04da 0f62 7569 6c64 5f70 6c61 696e  /)...build_plain
-00000aa0: 5f75 726c da08 6163 746f 725f 6964 da07  _url..actor_id..
-00000ab0: 7265 706c 6163 65da 0373 7472 2906 720a  replace..str).r.
-00000ac0: 0000 00da 0261 72da 0561 6374 6f72 da02  .....ar..actor..
-00000ad0: 706b da04 6172 6773 da02 6b77 720c 0000  pk..args..kwr...
-00000ae0: 0072 0c00 0000 720d 0000 00da 0e67 6574  .r....r......get
-00000af0: 5f64 6574 6169 6c5f 7572 6c7b 0000 0073  _detail_url{...s
-00000b00: 1400 0000 0401 0201 0201 0c01 0601 02fc  ................
-00000b10: 0204 06fc 0204 06fc 7a15 506c 7567 696e  ........z.Plugin
-00000b20: 2e67 6574 5f64 6574 6169 6c5f 7572 6c46  .get_detail_urlF
-00000b30: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b40: 0002 0000 0063 0000 0073 1800 0000 8100  .....c...s......
-00000b50: 7c01 6400 7501 720a 6401 5600 0100 6400  |.d.u.r.d.V...d.
-00000b60: 5300 6400 5300 2902 4e29 03da 0552 6561  S.d.S.).N)...Rea
-00000b70: 6374 7a04 3136 2e36 7a14 6874 7470 733a  ctz.16.6z.https:
-00000b80: 2f2f 7265 6163 746a 732e 6f72 672f 720c  //reactjs.org/r.
-00000b90: 0000 0029 0272 0a00 0000 da04 6874 6d6c  ...).r......html
-00000ba0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000bb0: 0d67 6574 5f75 7365 645f 6c69 6273 8200  .get_used_libs..
-00000bc0: 0000 7308 0000 0002 8008 010a 0104 ff7a  ..s............z
-00000bd0: 1450 6c75 6769 6e2e 6765 745f 7573 6564  .Plugin.get_used
-00000be0: 5f6c 6962 734e 2901 4629 0dda 085f 5f6e  _libsN).F)...__n
-00000bf0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000c00: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000c10: 1375 695f 6861 6e64 6c65 5f61 7474 725f  .ui_handle_attr_
-00000c20: 6e61 6d65 da0d 6e65 6564 735f 706c 7567  name..needs_plug
-00000c30: 696e 73da 0a75 726c 5f70 7265 6669 78da  ins..url_prefix.
-00000c40: 0a6d 6564 6961 5f6e 616d 65da 0d73 7570  .media_name..sup
-00000c50: 706f 7274 5f61 7379 6e63 720e 0000 0072  port_asyncr....r
-00000c60: 2500 0000 723e 0000 0072 4c00 0000 724f  %...r>...rL...rO
-00000c70: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000c80: 0000 720d 0000 0072 0400 0000 1600 0000  ..r....r........
-00000c90: 7316 0000 0008 0004 0208 0304 0304 0204  s...............
-00000ca0: 0108 0408 0608 1508 3b0e 0772 0400 0000  ........;..r....
-00000cb0: 4e29 07da 075f 5f64 6f63 5f5f da0c 646a  N)...__doc__..dj
-00000cc0: 616e 676f 2e75 7469 6c73 7202 0000 00da  ango.utilsr.....
-00000cd0: 096c 696e 6f2e 636f 7265 7203 0000 00da  .lino.corer.....
-00000ce0: 0b6c 696e 6f2e 6170 692e 6164 7204 0000  .lino.api.adr...
-00000cf0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000d00: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000d10: 0000 0073 0a00 0000 0404 0c0c 0c01 0c01  ...s............
-00000d20: 1403                                     ..
+00000250: 720c 0000 00fa 452f 686f 6d65 2f62 6c75  r.....E/home/blu
+00000260: 7272 792f 6c69 6e6f 2f65 6e76 2f72 6570  rry/lino/env/rep
+00000270: 6f73 6974 6f72 6965 732f 7265 6163 742f  ositories/react/
+00000280: 6c69 6e6f 5f72 6561 6374 2f72 6561 6374  lino_react/react
+00000290: 2f5f 5f69 6e69 745f 5f2e 7079 da0a 6f6e  /__init__.py..on
+000002a0: 5f75 695f 696e 6974 2500 0000 7304 0000  _ui_init%...s...
+000002b0: 000c 010e 017a 1150 6c75 6769 6e2e 6f6e  .....z.Plugin.on
+000002c0: 5f75 695f 696e 6974 6302 0000 0000 0000  _ui_initc.......
+000002d0: 0000 0000 0008 0000 0009 0000 0043 0000  .............C..
+000002e0: 0073 7a00 0000 7400 7c00 6a01 7c00 6a02  .sz...t.|.j.|.j.
+000002f0: 7c01 7c00 6a02 6a03 6a04 7405 a006 a100  |.|.j.j.j.t.....
+00000300: 7407 6400 6401 8d07 7d02 6402 7d03 7c00  t.d.d...}.d.}.|.
+00000310: 6a02 6a03 6a08 6a01 6a09 7d04 7c00 6a02  j.j.j.j.j.}.|.j.
+00000320: 6a0a 4400 5d1b 7d05 7c05 6a0b 4400 5d15  j.D.].}.|.j.D.].
+00000330: 7d06 7c04 a00c 7c06 a101 7d07 7c03 6403  }.|...|...}.|.d.
+00000340: 7c07 6a0d 6405 6900 7c02 a401 8e01 9b00  |.j.d.i.|.......
+00000350: 6404 9d03 3700 7d03 7124 711f 7c03 5300  d...7.}.q$q.|.S.
+00000360: 2906 4e29 07da 0e65 7874 6a73 5f72 656e  ).N)...extjs_ren
+00000370: 6465 7265 72da 0473 6974 65da 0873 6574  derer..site..set
+00000380: 7469 6e67 73da 046c 696e 6fda 086c 616e  tings..lino..lan
+00000390: 6775 6167 6572 0300 0000 da05 6578 746a  guager......extj
+000003a0: 73da 007a 083c 7363 7269 7074 3e7a 093c  s..z.<script>z.<
+000003b0: 2f73 6372 6970 743e 720c 0000 0029 0eda  /script>r....)..
+000003c0: 0464 6963 7472 0900 0000 7210 0000 00da  .dictr....r.....
+000003d0: 0770 6c75 6769 6e73 7212 0000 0072 0200  .pluginsr....r..
+000003e0: 0000 da0c 6765 745f 6c61 6e67 7561 6765  ....get_language
+000003f0: 7203 0000 00da 056a 696e 6a61 da09 6a69  r......jinja..ji
+00000400: 6e6a 615f 656e 76da 0e73 6f72 7465 645f  nja_env..sorted_
+00000410: 706c 7567 696e 73da 1073 6974 655f 6a73  plugins..site_js
+00000420: 5f73 6e69 7070 6574 73da 0c67 6574 5f74  _snippets..get_t
+00000430: 656d 706c 6174 65da 0672 656e 6465 7229  emplate..render)
+00000440: 0872 0a00 0000 7211 0000 00da 0763 6f6e  .r....r......con
+00000450: 7465 7874 da02 6a73 da03 656e 76da 0170  text..js..env..p
+00000460: da07 736e 6970 7065 74da 0874 656d 706c  ..snippet..templ
+00000470: 6174 6572 0c00 0000 720c 0000 0072 0d00  ater....r....r..
+00000480: 0000 da15 6c6f 6164 5f73 6974 655f 6a73  ....load_site_js
+00000490: 5f73 6e69 7070 6574 732b 0000 0073 2200  _snippets+...s".
+000004a0: 0000 0201 0401 0401 0201 0801 0601 0201  ................
+000004b0: 0201 06f9 040a 0e01 0c02 0a01 0a01 1e01  ................
+000004c0: 02fe 0404 7a1c 506c 7567 696e 2e6c 6f61  ....z.Plugin.loa
+000004d0: 645f 7369 7465 5f6a 735f 736e 6970 7065  d_site_js_snippe
+000004e0: 7473 6301 0000 0000 0000 0000 0000 0006  tsc.............
+000004f0: 0000 0014 0000 0043 0000 0073 5a01 0000  .......C...sZ...
+00000500: 6401 6402 6c00 6d01 7d01 0100 6401 6403  d.d.l.m.}...d.d.
+00000510: 6c00 6d02 7d02 0100 6404 6405 6c03 6d04  l.m.}...d.d.l.m.
+00000520: 7d03 0100 6406 7d04 7c01 7c04 6407 1700  }...d.}.|.|.d...
+00000530: 7c03 6a05 a006 a100 8302 7c01 7c04 6408  |.j.......|.|.d.
+00000540: 1700 7c03 6a07 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
+00000550: 6409 1700 7c03 6a08 a006 a100 8302 7c01  d...|.j.......|.
+00000560: 7c04 640a 1700 7c03 6a09 a006 a100 8302  |.d...|.j.......
+00000570: 7c01 7c04 640b 1700 7c03 6a0a a006 a100  |.|.d...|.j.....
+00000580: 8302 7c01 640c 7c03 6a0b a006 a100 8302  ..|.d.|.j.......
+00000590: 7c01 7c04 640d 1700 7c03 6a0c a006 a100  |.|.d...|.j.....
+000005a0: 8302 7c02 640e 7c03 6a0d a006 a100 8302  ..|.d.|.j.......
+000005b0: 7c01 7c04 640f 1700 7c03 6a0e a006 a100  |.|.d...|.j.....
+000005c0: 8302 7c01 7c04 6410 1700 7c03 6a0f a006  ..|.|.d...|.j...
+000005d0: a100 8302 7c01 7c04 6411 1700 7c03 6a0e  ....|.|.d...|.j.
+000005e0: a006 a100 8302 7c01 7c04 6412 1700 7c03  ......|.|.d...|.
+000005f0: 6a0f a006 a100 8302 7c01 7c04 6413 1700  j.......|.|.d...
+00000600: 7c03 6a10 a006 a100 8302 7c01 7c04 6414  |.j.......|.|.d.
+00000610: 1700 7c03 6a11 a006 a100 8302 7c01 7c04  ..|.j.......|.|.
+00000620: 6415 1700 7c03 6a11 a006 a100 8302 7c01  d...|.j.......|.
+00000630: 7c04 6416 1700 7c03 6a12 a006 a100 8302  |.d...|.j.......
+00000640: 7c01 7c04 6417 1700 7c03 6a13 a006 a100  |.|.d...|.j.....
+00000650: 8302 6711 7d05 7c05 5300 2918 4e72 0100  ..g.}.|.S.).Nr..
+00000660: 0000 2901 da07 7265 5f70 6174 6829 01da  ..)...re_path)..
+00000670: 0470 6174 6872 0700 0000 2901 da05 7669  .pathr....)...vi
+00000680: 6577 73fa 015e fa01 247a 0d75 7365 722f  ews..^..$z.user/
+00000690: 7365 7474 696e 6773 7a05 6175 7468 247a  settingsz.auth$z
+000006a0: 056e 756c 6c2f 7a25 283f 503c 776f 726b  .null/z%(?P<work
+000006b0: 626f 783e 776f 726b 626f 782d 5b61 2d7a  box>workbox-[a-z
+000006c0: 412d 5a30 2d39 5d2a 2e6a 7329 247a 1173  A-Z0-9]*.js)$z.s
+000006d0: 6572 7669 6365 2d77 6f72 6b65 722e 6a73  ervice-worker.js
+000006e0: 7a0e 6170 692f 6d61 696e 5f68 746d 6c24  z.api/main_html$
+000006f0: 7a15 6461 7368 626f 6172 642f 3c69 6e74  z.dashboard/<int
+00000700: 3a69 6e64 6578 3e7a 2a72 6573 7466 756c  :index>z*restful
+00000710: 2f28 3f50 3c61 7070 5f6c 6162 656c 3e5c  /(?P<app_label>\
+00000720: 772b 292f 283f 503c 6163 746f 723e 5c77  w+)/(?P<actor>\w
+00000730: 2b29 247a 3572 6573 7466 756c 2f28 3f50  +)$z5restful/(?P
+00000740: 3c61 7070 5f6c 6162 656c 3e5c 772b 292f  <app_label>\w+)/
+00000750: 283f 503c 6163 746f 723e 5c77 2b29 2f28  (?P<actor>\w+)/(
+00000760: 3f50 3c70 6b3e 2e2b 2924 7a26 6170 692f  ?P<pk>.+)$z&api/
+00000770: 283f 503c 6170 705f 6c61 6265 6c3e 5c77  (?P<app_label>\w
+00000780: 2b29 2f28 3f50 3c61 6374 6f72 3e5c 772b  +)/(?P<actor>\w+
+00000790: 2924 7a34 6170 692f 283f 503c 6170 705f  )$z4api/(?P<app_
+000007a0: 6c61 6265 6c3e 5c77 2b29 2f28 3f50 3c61  label>\w+)/(?P<a
+000007b0: 6374 6f72 3e5c 772b 292f 283f 503c 706b  ctor>\w+)/(?P<pk
+000007c0: 3e5b 5e2f 5d2b 2924 7a42 7661 6c75 6573  >[^/]+)$zBvalues
+000007d0: 2f28 3f50 3c61 7070 5f6c 6162 656c 3e5c  /(?P<app_label>\
+000007e0: 772b 292f 283f 503c 6163 746f 723e 5c77  w+)/(?P<actor>\w
+000007f0: 2b29 2f28 3f50 3c70 6b3e 2e2b 292f 283f  +)/(?P<pk>.+)/(?
+00000800: 503c 6669 656c 643e 2e2b 2924 7a2a 6368  P<field>.+)$z*ch
+00000810: 6f69 6365 732f 283f 503c 6170 705f 6c61  oices/(?P<app_la
+00000820: 6265 6c3e 5c77 2b29 2f28 3f50 3c61 6374  bel>\w+)/(?P<act
+00000830: 6f72 3e5c 772b 2924 7a39 6368 6f69 6365  or>\w+)$z9choice
+00000840: 732f 283f 503c 6170 705f 6c61 6265 6c3e  s/(?P<app_label>
+00000850: 5c77 2b29 2f28 3f50 3c61 6374 6f72 3e5c  \w+)/(?P<actor>\
+00000860: 772b 292f 283f 503c 6669 656c 643e 5c77  w+)/(?P<field>\w
+00000870: 2b29 247a 4761 7063 686f 6963 6573 2f28  +)$zGapchoices/(
+00000880: 3f50 3c61 7070 5f6c 6162 656c 3e5c 772b  ?P<app_label>\w+
+00000890: 292f 283f 503c 6163 746f 723e 5c77 2b29  )/(?P<actor>\w+)
+000008a0: 2f28 3f50 3c61 6e3e 5c77 2b29 2f28 3f50  /(?P<an>\w+)/(?P
+000008b0: 3c66 6965 6c64 3e5c 772b 2924 7a0c 6368  <field>\w+)$z.ch
+000008c0: 6f69 6365 6c69 7374 732f 2914 da0b 646a  oicelists/)...dj
+000008d0: 616e 676f 2e75 726c 7372 2600 0000 7227  ango.urlsr&...r'
+000008e0: 0000 0072 1500 0000 7228 0000 00da 0549  ...r....r(.....I
+000008f0: 6e64 6578 da07 6173 5f76 6965 77da 0c55  ndex..as_view..U
+00000900: 7365 7253 6574 7469 6e67 73da 0c41 7574  serSettings..Aut
+00000910: 6865 6e74 6963 6174 65da 044e 756c 6cda  henticate..Null.
+00000920: 0657 4256 6965 77da 0653 5756 6965 77da  .WBView..SWView.
+00000930: 084d 6169 6e48 746d 6cda 0d44 6173 6862  .MainHtml..Dashb
+00000940: 6f61 7264 4974 656d da07 4170 694c 6973  oardItem..ApiLis
+00000950: 74da 0a41 7069 456c 656d 656e 74da 0c44  t..ApiElement..D
+00000960: 656c 6179 6564 5661 6c75 65da 0743 686f  elayedValue..Cho
+00000970: 6963 6573 da12 4163 7469 6f6e 5061 7261  ices..ActionPara
+00000980: 6d43 686f 6963 6573 da0f 4368 6f69 6365  mChoices..Choice
+00000990: 4c69 7374 4d6f 6465 6c29 0672 0a00 0000  ListModel).r....
+000009a0: da03 7572 6c72 2700 0000 7228 0000 00da  ..urlr'...r(....
+000009b0: 0272 78da 0475 726c 7372 0c00 0000 720c  .rx..urlsr....r.
+000009c0: 0000 0072 0d00 0000 da0c 6765 745f 7061  ...r......get_pa
+000009d0: 7474 6572 6e73 4000 0000 7356 0000 000c  tterns@...sV....
+000009e0: 030c 010c 0104 0212 0612 0112 0112 0108  ................
+000009f0: 0208 0102 ff0e 0212 020e 0208 0308 0102  ................
+00000a00: ff08 0208 0102 ff08 0308 0102 ff08 0208  ................
+00000a10: 0102 ff08 0408 0102 ff08 0208 0102 ff08  ................
+00000a20: 0208 0202 fe08 0308 0202 fe08 0808 0102  ................
+00000a30: ff04 d704 2d7a 1350 6c75 6769 6e2e 6765  ....-z.Plugin.ge
+00000a40: 745f 7061 7474 6572 6e73 6304 0000 0000  t_patternsc.....
+00000a50: 0000 0000 0000 0006 0000 0007 0000 004f  ...............O
+00000a60: 0000 0073 2c00 0000 7c00 6a00 6401 6402  ...s,...|.j.d.d.
+00000a70: 7c02 6a01 a002 6403 6404 a102 7403 7c03  |.j...d.d...t.|.
+00000a80: 8301 6704 7c04 a201 5200 6900 7c05 a401  ..g.|...R.i.|...
+00000a90: 8e01 5300 2905 4efa 0123 da03 6170 69da  ..S.).N..#..api.
+00000aa0: 012e fa01 2f29 04da 0f62 7569 6c64 5f70  ..../)...build_p
+00000ab0: 6c61 696e 5f75 726c da08 6163 746f 725f  lain_url..actor_
+00000ac0: 6964 da07 7265 706c 6163 65da 0373 7472  id..replace..str
+00000ad0: 2906 720a 0000 00da 0261 72da 0561 6374  ).r......ar..act
+00000ae0: 6f72 da02 706b da04 6172 6773 da02 6b77  or..pk..args..kw
+00000af0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000b00: 0e67 6574 5f64 6574 6169 6c5f 7572 6c7b  .get_detail_url{
+00000b10: 0000 0073 1400 0000 0401 0201 0201 0c01  ...s............
+00000b20: 0601 02fc 0204 06fc 0204 06fc 7a15 506c  ............z.Pl
+00000b30: 7567 696e 2e67 6574 5f64 6574 6169 6c5f  ugin.get_detail_
+00000b40: 7572 6c46 6302 0000 0000 0000 0000 0000  urlFc...........
+00000b50: 0002 0000 0002 0000 0063 0000 0073 1800  .........c...s..
+00000b60: 0000 8100 7c01 6400 7501 720a 6401 5600  ....|.d.u.r.d.V.
+00000b70: 0100 6400 5300 6400 5300 2902 4e29 03da  ..d.S.d.S.).N)..
+00000b80: 0552 6561 6374 7a04 3136 2e36 7a14 6874  .Reactz.16.6z.ht
+00000b90: 7470 733a 2f2f 7265 6163 746a 732e 6f72  tps://reactjs.or
+00000ba0: 672f 720c 0000 0029 0272 0a00 0000 da04  g/r....).r......
+00000bb0: 6874 6d6c 720c 0000 0072 0c00 0000 720d  htmlr....r....r.
+00000bc0: 0000 00da 0d67 6574 5f75 7365 645f 6c69  .....get_used_li
+00000bd0: 6273 8200 0000 7308 0000 0002 8008 010a  bs....s.........
+00000be0: 0104 ff7a 1450 6c75 6769 6e2e 6765 745f  ...z.Plugin.get_
+00000bf0: 7573 6564 5f6c 6962 734e 2901 4629 0dda  used_libsN).F)..
+00000c00: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000c10: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000c20: 655f 5fda 1375 695f 6861 6e64 6c65 5f61  e__..ui_handle_a
+00000c30: 7474 725f 6e61 6d65 da0d 6e65 6564 735f  ttr_name..needs_
+00000c40: 706c 7567 696e 73da 0a75 726c 5f70 7265  plugins..url_pre
+00000c50: 6669 78da 0a6d 6564 6961 5f6e 616d 65da  fix..media_name.
+00000c60: 0d73 7570 706f 7274 5f61 7379 6e63 720e  .support_asyncr.
+00000c70: 0000 0072 2500 0000 723e 0000 0072 4c00  ...r%...r>...rL.
+00000c80: 0000 724f 0000 0072 0c00 0000 720c 0000  ..rO...r....r...
+00000c90: 0072 0c00 0000 720d 0000 0072 0400 0000  .r....r....r....
+00000ca0: 1600 0000 7316 0000 0008 0004 0208 0304  ....s...........
+00000cb0: 0304 0204 0108 0408 0608 1508 3b0e 0772  ............;..r
+00000cc0: 0400 0000 4e29 07da 075f 5f64 6f63 5f5f  ....N)...__doc__
+00000cd0: da0c 646a 616e 676f 2e75 7469 6c73 7202  ..django.utilsr.
+00000ce0: 0000 00da 096c 696e 6f2e 636f 7265 7203  .....lino.corer.
+00000cf0: 0000 00da 0b6c 696e 6f2e 6170 692e 6164  .....lino.api.ad
+00000d00: 7204 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000d10: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
+00000d20: 6c65 3e01 0000 0073 0a00 0000 0404 0c0c  le>....s........
+00000d30: 0c01 0c01 1403                           ......
```

### Comparing `lino_react-23.7.4/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 02:47:35 2023 UTC, .py size: 3952 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7d9 a464 700f 0000  o..........dp...
+00000000: 6f0d 0d0a 0000 0000 5ce4 ab64 700f 0000  o.......\..dp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 a002 a100  d.l.m.Z...d.....
 00000040: 5a03 6900 6403 6404 9301 6405 6406 9301  Z.i.d.d...d.d...
 00000050: 6407 6408 9301 6409 640a 9301 640b 640c  d.d...d.d...d.d.
 00000060: 9301 640d 640e 9301 640f 6410 9301 6411  ..d.d...d.d...d.
 00000070: 6412 9301 6413 6404 9301 6414 6415 9301  d...d.d...d.d...
@@ -221,31 +221,32 @@
 00000dc0: 6570 74da 0d64 6174 6162 6173 655f 6765  ept..database_ge
 00000dd0: 6172 da06 6361 6e63 656c da0a 666c 6167  ar..cancel..flag
 00000de0: 5f67 7265 656e da09 6461 7465 5f6e 6578  _green..date_nex
 00000df0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
 00000e00: 0000 0400 0000 4300 0000 7312 0000 0069  ......C...s....i
 00000e10: 007c 005d 057d 017c 017c 0193 0271 0253  .|.].}.|.|...q.S
 00000e20: 00a9 0072 2b00 0000 2902 da02 2e30 da04  ...r+...)....0..
-00000e30: 6963 6f6e 722b 0000 0072 2b00 0000 fa2e  iconr+...r+.....
-00000e40: 2f68 6f6d 652f 6c75 632f 776f 726b 2f72  /home/luc/work/r
-00000e50: 6561 6374 2f6c 696e 6f5f 7265 6163 742f  eact/lino_react/
-00000e60: 7265 6163 742f 6963 6f6e 732e 7079 da0a  react/icons.py..
-00000e70: 3c64 6963 7463 6f6d 703e e600 0000 7302  <dictcomp>....s.
-00000e80: 0000 0012 0072 2f00 0000 2906 da13 6c69  .....r/...)...li
-00000e90: 6e6f 2e63 6f72 652e 636f 6e73 7461 6e74  no.core.constant
-00000ea0: 7372 0200 0000 da05 7370 6c69 74da 1052  sr......split..R
-00000eb0: 4541 4354 5f49 434f 4e5f 4e41 4d45 53da  EACT_ICON_NAMES.
-00000ec0: 1252 4541 4354 5f49 434f 4e5f 4d41 5050  .REACT_ICON_MAPP
-00000ed0: 494e 47da 0675 7064 6174 6572 2b00 0000  ING..updater+...
-00000ee0: 722b 0000 0072 2b00 0000 722e 0000 00da  r+...r+...r.....
-00000ef0: 083c 6d6f 6475 6c65 3e01 0000 0073 a800  .<module>....s..
-00000f00: 0000 0c00 0204 007f 0434 0081 02cc 007f  .........4......
-00000f10: 0236 0401 02ff 0402 02fe 0403 02fd 0404  .6..............
-00000f20: 02fc 0405 02fb 0406 02fa 0407 02f9 0408  ................
-00000f30: 02f8 0409 02f7 040a 02f6 040b 02f5 040c  ................
-00000f40: 02f4 040d 02f3 040e 02f2 040f 02f1 0410  ................
-00000f50: 02f0 0411 04ef 0412 02ee 0413 02ed 0414  ................
-00000f60: 02ec 0415 02eb 0416 02ea 0417 02e9 0418  ................
-00000f70: 02e8 0419 02e7 041a 02e6 041b 02e5 041c  ................
-00000f80: 02e4 041d 02e3 041e 02e2 041f 02e1 0420  ............... 
-00000f90: 02e0 0421 02df 0422 04de 0223 0201 0201  ...!..."...#....
-00000fa0: 0201 0201 0201 08d8 182c                 .........,
+00000e30: 6963 6f6e 722b 0000 0072 2b00 0000 fa42  iconr+...r+....B
+00000e40: 2f68 6f6d 652f 626c 7572 7279 2f6c 696e  /home/blurry/lin
+00000e50: 6f2f 656e 762f 7265 706f 7369 746f 7269  o/env/repositori
+00000e60: 6573 2f72 6561 6374 2f6c 696e 6f5f 7265  es/react/lino_re
+00000e70: 6163 742f 7265 6163 742f 6963 6f6e 732e  act/react/icons.
+00000e80: 7079 da0a 3c64 6963 7463 6f6d 703e e600  py..<dictcomp>..
+00000e90: 0000 7302 0000 0012 0072 2f00 0000 2906  ..s......r/...).
+00000ea0: da13 6c69 6e6f 2e63 6f72 652e 636f 6e73  ..lino.core.cons
+00000eb0: 7461 6e74 7372 0200 0000 da05 7370 6c69  tantsr......spli
+00000ec0: 74da 1052 4541 4354 5f49 434f 4e5f 4e41  t..REACT_ICON_NA
+00000ed0: 4d45 53da 1252 4541 4354 5f49 434f 4e5f  MES..REACT_ICON_
+00000ee0: 4d41 5050 494e 47da 0675 7064 6174 6572  MAPPING..updater
+00000ef0: 2b00 0000 722b 0000 0072 2b00 0000 722e  +...r+...r+...r.
+00000f00: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000f10: 0073 a800 0000 0c00 0204 007f 0434 0081  .s...........4..
+00000f20: 02cc 007f 0236 0401 02ff 0402 02fe 0403  .....6..........
+00000f30: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
+00000f40: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
+00000f50: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
+00000f60: 02f1 0410 02f0 0411 04ef 0412 02ee 0413  ................
+00000f70: 02ed 0414 02ec 0415 02eb 0416 02ea 0417  ................
+00000f80: 02e9 0418 02e8 0419 02e7 041a 02e6 041b  ................
+00000f90: 02e5 041c 02e4 041d 02e3 041e 02e2 041f  ................
+00000fa0: 02e1 0420 02e0 0421 02df 0422 04de 0223  ... ...!..."...#
+00000fb0: 0201 0201 0201 0201 0201 08d8 182c       .............,
```

### Comparing `lino_react-23.7.4/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 18 09:49:16 2023 UTC, .py size: 29449 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,1156 +1,1162 @@
-00000000: 6f0d 0d0a 0000 0000 1c60 b664 0973 0000  o........`.d.s..
+00000000: 6f0d 0d0a 0000 0000 b98f be64 a373 0000  o..........d.s..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6408 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6400  d.l.m.Z.m.Z...d.
-00000090: 6409 6c10 6d11 5a11 6d12 5a12 0100 6400  d.l.m.Z.m.Z...d.
-000000a0: 640a 6c13 6d14 5a14 0100 6400 640b 6c13  d.l.m.Z...d.d.l.
-000000b0: 6d15 5a15 0100 6400 640c 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 640d 6c18 6d19 5a19 0100 6400  ..d.d.l.m.Z...d.
-000000d0: 640e 6c1a 6d1b 5a1b 6d1c 5a1c 6d1d 5a1d  d.l.m.Z.m.Z.m.Z.
-000000e0: 6d1e 5a1e 6d1f 5a1f 6d20 5a20 6d21 5a21  m.Z.m.Z.m Z m!Z!
-000000f0: 6d22 5a22 0100 6400 640f 6c23 6d24 5a24  m"Z"..d.d.l#m$Z$
-00000100: 0100 6400 6410 6c25 6d26 5a26 0100 6400  ..d.d.l%m&Z&..d.
-00000110: 6411 6c27 6d28 5a28 0100 6400 6412 6c29  d.l'm(Z(..d.d.l)
-00000120: 6d2a 5a2a 0100 6400 6413 6c2b 6d2c 5a2c  m*Z*..d.d.l+m,Z,
-00000130: 6d2d 5a2d 0100 6400 6414 6c2e 6d2f 5a2f  m-Z-..d.d.l.m/Z/
-00000140: 6d30 5a30 6d31 5a31 6d32 5a32 6d33 5a33  m0Z0m1Z1m2Z2m3Z3
-00000150: 0100 6400 6415 6c13 6d34 5a34 0100 6400  ..d.d.l.m4Z4..d.
-00000160: 6416 6c35 6d36 5a36 0100 6400 6417 6c37  d.l5m6Z6..d.d.l7
-00000170: 6d38 5a38 0100 6400 6418 6c39 6d3a 5a3a  m8Z8..d.d.l9m:Z:
-00000180: 6d3b 5a3b 6d3c 5a3c 0100 6400 6419 6c3d  m;Z;m<Z<..d.d.l=
-00000190: 6d3e 5a3e 6d3f 5a3f 0100 6400 641a 6c40  m>Z>m?Z?..d.d.l@
-000001a0: 6d41 5a41 0100 6400 641b 6c42 6d43 5a43  mAZA..d.d.lBmCZC
-000001b0: 0100 641c 641d 6c44 6d45 5a45 0100 6422  ..d.d.lDmEZE..d"
-000001c0: 641e 641f 8401 5a46 4700 6420 6421 8400  d.d...ZFG.d d!..
-000001d0: 6421 650f 8303 5a47 6401 5300 2923 e900  d!e...ZGd.S.)#..
-000001e0: 0000 004e 2901 da04 5061 7468 2901 da06  ...N)...Path)...
-000001f0: 6573 6361 7065 2901 da08 7365 7474 696e  escape)...settin
-00000200: 6773 2901 da06 6d6f 6465 6c73 2901 da0b  gs)...models)...
-00000210: 666f 726d 6174 5f6c 617a 7929 01da 0b74  format_lazy)...t
-00000220: 7261 6e73 6c61 7469 6f6e 2902 da11 6164  ranslation)...ad
-00000230: 645f 7573 6572 5f6c 616e 6775 6167 65da  d_user_language.
-00000240: 0f4a 7343 6163 6865 5265 6e64 6572 6572  .JsCacheRenderer
-00000250: 2902 da04 4d65 6e75 da08 4d65 6e75 4974  )...Menu..MenuIt
-00000260: 656d 2901 da09 636f 6e73 7461 6e74 7329  em)...constants)
-00000270: 01da 0b63 686f 6963 656c 6973 7473 2901  ...choicelists).
-00000280: da0b 436f 6e74 656e 7454 7970 6529 01da  ..ContentType)..
-00000290: 0b45 7874 5265 6e64 6572 6572 2908 da0e  .ExtRenderer)...
-000002a0: 5368 6f77 456d 7074 7954 6162 6c65 da0a  ShowEmptyTable..
-000002b0: 5368 6f77 4465 7461 696c da0d 5772 6170  ShowDetail..Wrap
-000002c0: 7065 6441 6374 696f 6eda 0a53 686f 7749  pedAction..ShowI
-000002d0: 6e73 6572 74da 0953 686f 7754 6162 6c65  nsert..ShowTable
-000002e0: da0c 5375 626d 6974 4465 7461 696c da0c  ..SubmitDetail..
-000002f0: 5375 626d 6974 496e 7365 7274 da06 4163  SubmitInsert..Ac
-00000300: 7469 6f6e 2901 da0b 426f 756e 6441 6374  tion)...BoundAct
-00000310: 696f 6e29 01da 0e43 686f 6963 654c 6973  ion)...ChoiceLis
-00000320: 744d 6574 6129 01da 1044 6173 6862 6f61  tMeta)...Dashboa
-00000330: 7264 4c61 796f 7574 7329 01da 0541 6374  rdLayouts)...Act
-00000340: 6f72 2902 da0c 4c61 796f 7574 4861 6e64  or)...LayoutHand
-00000350: 6c65 da0a 4261 7365 4c61 796f 7574 2905  le..BaseLayout).
-00000360: da0d 4c61 796f 7574 456c 656d 656e 74da  ..LayoutElement.
-00000370: 1143 6f6d 626f 4669 656c 6445 6c65 6d65  .ComboFieldEleme
-00000380: 6e74 da1d 5369 6d70 6c65 5265 6d6f 7465  nt..SimpleRemote
-00000390: 436f 6d62 6f46 6965 6c64 456c 656d 656e  ComboFieldElemen
-000003a0: 74da 0c46 6965 6c64 456c 656d 656e 74da  t..FieldElement.
-000003b0: 1750 7265 7669 6577 5465 7874 4669 656c  .PreviewTextFiel
-000003c0: 6445 6c65 6d65 6e74 2901 da06 6b65 726e  dElement)...kern
-000003d0: 656c 2901 da01 4529 01da 056a 7367 656e  el)...E)...jsgen
-000003e0: 2903 da05 7079 326a 73da 076a 735f 636f  )...py2js..js_co
-000003f0: 6465 da08 6f62 6a32 6469 6374 2902 da10  de..obj2dict)...
-00000400: 6765 745f 7573 6572 5f70 726f 6669 6c65  get_user_profile
-00000410: da11 7769 7468 5f75 7365 725f 7072 6f66  ..with_user_prof
-00000420: 696c 6529 01da 0845 6469 7453 6166 6529  ile)...EditSafe)
-00000430: 01da 0769 7363 6c61 7373 e901 0000 0029  ...isclass.....)
-00000440: 01da 1252 4541 4354 5f49 434f 4e5f 4d41  ...REACT_ICON_MA
-00000450: 5050 494e 4763 0300 0000 0000 0000 0000  PPINGc..........
-00000460: 0000 0500 0000 0300 0000 4300 0000 734a  ..........C...sJ
-00000470: 0000 007c 0264 016b 0273 0c74 007c 0283  ...|.d.k.s.t.|..
-00000480: 0173 0c4a 0064 0283 0182 0174 017c 0083  .s.J.d.....t.|..
-00000490: 0144 005d 125c 027d 037d 047c 0272 1a7c  .D.].\.}.}.|.r.|
-000004a0: 027c 0483 017d 047c 047c 016b 0272 227c  .|...}.|.|.k.r"|
-000004b0: 0302 0001 0053 0071 1064 0353 0029 047a  .....S.q.d.S.).z
-000004c0: 4d52 6574 7572 6e73 2074 6865 2069 6e64  MReturns the ind
-000004d0: 6578 206f 6620 616e 2065 6c65 6d65 6e74  ex of an element
-000004e0: 2069 6e20 6120 6361 6c6c 6162 6c65 2077   in a callable w
-000004f0: 6869 6368 2063 616e 2062 6520 7573 6520  hich can be use 
-00000500: 6120 6b65 7920 6675 6e63 7469 6f6e 4e7a  a key functionNz
-00000510: 586b 6579 2073 686f 6c64 2062 6520 6120  Xkey shold be a 
-00000520: 6675 6e63 7469 6f6e 2074 6861 7420 7461  function that ta
-00000530: 6b65 7320 7468 6520 6974 7465 7227 7320  kes the itter's 
-00000540: 6974 656d 2061 6e64 2072 6574 7572 6e73  item and returns
-00000550: 2074 6861 7420 7761 6e74 6564 206d 6174   that wanted mat
-00000560: 6368 6564 2069 7465 6de9 ffff ffff 2902  ched item.....).
-00000570: da08 6361 6c6c 6162 6c65 da09 656e 756d  ..callable..enum
-00000580: 6572 6174 6529 05da 0569 7474 6572 da06  erate)...itter..
-00000590: 7461 7267 6574 da03 6b65 79da 0169 da01  target..key..i..
-000005a0: 78a9 0072 3700 0000 fa31 2f68 6f6d 652f  x..r7....1/home/
-000005b0: 6c75 632f 776f 726b 2f72 6561 6374 2f6c  luc/work/react/l
-000005c0: 696e 6f5f 7265 6163 742f 7265 6163 742f  ino_react/react/
-000005d0: 7265 6e64 6572 6572 2e70 79da 0466 696e  renderer.py..fin
-000005e0: 642e 0000 0073 1000 0000 1802 1002 0401  d....s..........
-000005f0: 0801 0801 0801 02ff 0403 7239 0000 0063  ..........r9...c
-00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000610: 0300 0000 0000 0000 73e6 0000 0065 005a  ........s....e.Z
-00000620: 0164 005a 0264 015a 0364 025a 0464 025a  .d.Z.d.Z.d.Z.d.Z
-00000630: 0564 035a 0664 045a 0764 025a 0887 0066  .d.Z.d.Z.d.Z...f
-00000640: 0164 0564 0684 085a 0964 0764 0884 005a  .d.d...Z.d.d...Z
-00000650: 0a64 0964 0a84 005a 0b64 0b64 0c84 005a  .d.d...Z.d.d...Z
-00000660: 0c64 0d64 0e84 005a 0d64 0f64 1084 005a  .d.d...Z.d.d...Z
-00000670: 0e64 1164 1284 005a 0f64 3264 1464 1584  .d.d...Z.d2d.d..
-00000680: 015a 1069 0066 0164 1664 1784 015a 1164  .Z.i.f.d.d...Z.d
-00000690: 1864 1984 005a 1264 1a64 1b84 005a 1364  .d...Z.d.d...Z.d
-000006a0: 1c64 1d84 005a 1464 1e64 1f84 005a 1564  .d...Z.d.d...Z.d
-000006b0: 2064 2184 005a 1664 2264 2384 005a 1764   d!..Z.d"d#..Z.d
-000006c0: 2464 2584 005a 1864 2664 2784 005a 1964  $d%..Z.d&d'..Z.d
-000006d0: 2864 2984 005a 1a64 2a64 2b84 005a 1b64  (d)..Z.d*d+..Z.d
-000006e0: 2c64 2d84 005a 1c64 2e64 2f84 005a 1d87  ,d-..Z.d.d/..Z..
-000006f0: 0066 0164 3064 3184 085a 1e87 0004 005a  .f.d0d1..Z.....Z
-00000700: 1f53 0029 33da 0852 656e 6465 7265 727a  .S.)3..Rendererz
-00000710: 480a 2020 2020 4120 6672 6f6e 742d 656e  H.    A front-en
-00000720: 6420 7265 6e64 6572 6572 2074 6861 7420  d renderer that 
-00000730: 7573 6573 2074 6865 2052 6561 6374 204a  uses the React J
-00000740: 6176 6173 6372 6970 7420 6672 616d 6577  avascript framew
-00000750: 6f72 6b2e 0a20 2020 2054 7a12 7265 6163  ork..    Tz.reac
-00000760: 742f 6c69 6e6f 7765 622e 6a73 6f6e 7a05  t/linoweb.jsonz.
-00000770: 2e6a 736f 6e63 0200 0000 0000 0000 0000  .jsonc..........
-00000780: 0000 0200 0000 0300 0000 0300 0000 731c  ..............s.
-00000790: 0000 0074 0083 00a0 017c 01a1 0101 0074  ...t.....|.....t
-000007a0: 02a0 037c 006a 04a1 0101 0064 0053 00a9  ...|.j.....d.S..
-000007b0: 014e 2905 da05 7375 7065 72da 085f 5f69  .N)...super..__i
-000007c0: 6e69 745f 5f72 2500 0000 da12 7265 6769  nit__r%.....regi
-000007d0: 7374 6572 5f63 6f6e 7665 7274 6572 da0f  ster_converter..
-000007e0: 7079 326a 735f 636f 6e76 6572 7465 7229  py2js_converter)
-000007f0: 02da 0473 656c 66da 0966 726f 6e74 5f65  ...self..front_e
-00000800: 6e64 a901 da09 5f5f 636c 6173 735f 5f72  nd....__class__r
-00000810: 3700 0000 7238 0000 0072 3d00 0000 4600  7...r8...r=...F.
-00000820: 0000 7304 0000 000c 0110 017a 1152 656e  ..s........z.Ren
-00000830: 6465 7265 722e 5f5f 696e 6974 5f5f 6302  derer.__init__c.
-00000840: 0000 0000 0000 0000 0000 000c 0000 0008  ................
-00000850: 0000 0003 0000 0073 7002 0000 6401 6402  .......sp...d.d.
-00000860: 8400 7400 6a01 a002 a100 4400 8301 7d02  ..t.j.....D...}.
-00000870: 7403 8300 7d03 8800 6a04 4400 5d14 7d04  t...}...j.D.].}.
-00000880: 7c04 a005 a100 4400 5d0d 7d05 7c05 6a06  |.....D.].}.|.j.
-00000890: 7c03 7601 7223 7c03 a007 7c05 6a06 a101  |.v.r#|...|.j...
-000008a0: 0100 7116 7110 6403 8800 5f08 7409 6a0a  ..q.q.d..._.t.j.
-000008b0: 6a0b 7d06 740c 8700 6601 6404 6402 8408  j.}.t...f.d.d...
-000008c0: 7c03 4400 8301 7409 6a0a a00d 740e 8300  |.D...t.j...t...
-000008d0: a101 7c06 6a0f 6a10 7409 6a0a 6a11 8800  ..|.j.j.t.j.j...
-000008e0: 6a12 6a13 6405 7501 6406 6402 8400 7409  j.j.d.u.d.d...t.
-000008f0: 6a0a 6a14 4400 8301 6407 8d06 7d07 7409  j.j.D...d...}.t.
-00000900: 6a0a a015 6408 a101 7264 7c07 6a16 7417  j...d...rd|.j.t.
-00000910: 7c06 6a18 6a19 6a1a a01b a100 8301 6409  |.j.j.j.......d.
-00000920: 8d01 0100 7c07 6a16 7409 6a0a 6a00 6a1c  ....|.j.t.j.j.j.
-00000930: 640a 8d01 0100 7a12 741d a01e 741f 7409  d.....z.t...t.t.
-00000940: 6a20 8301 640b 1b00 640c 1b00 a101 6a21  j ..d...d.....j!
-00000950: 7c07 7422 6a23 3c00 5700 6e09 0400 7424  |.t"j#<.W.n...t$
-00000960: 7988 0100 0100 0100 5900 6e01 7700 7425  y.......Y.n.w.t%
-00000970: 7409 6a0a 640d 8302 7297 7c07 6a16 7409  t.j.d...r.|.j.t.
-00000980: 6a0a 6a26 640e 8d01 0100 7409 6a0a 6a27  j.j&d.....t.j.j'
-00000990: 6405 6b02 72a4 7c07 6a16 6403 640f 8d01  d.k.r.|.j.d.d...
-000009a0: 0100 6e0e 7425 7c06 6a28 6410 8302 72b2  ..n.t%|.j(d...r.
-000009b0: 7c07 6a16 7c06 6a28 6a29 6411 8d01 0100  |.j.|.j(j)d.....
-000009c0: 7409 6a0a a015 6412 a101 72c4 7c07 6a16  t.j...d...r.|.j.
-000009d0: 7c06 6a2a 6a2b 6fc1 7409 6a0a 6a2c 6413  |.j*j+o.t.j.j,d.
-000009e0: 8d01 0100 6900 7d08 8800 6a2d 4400 5d2f  ....i.}...j-D.]/
-000009f0: 7d09 8800 a02e 7c09 a101 7c08 7c09 6a2f  }.....|...|.|.j/
-00000a00: 3c00 7425 7c09 6414 8302 72f8 6415 7c09  <.t%|.d...r.d.|.
-00000a10: 6a2f 7600 72f8 7430 7c02 6416 1900 8301  j/v.r.t0|.d.....
-00000a20: 4400 5d14 5c02 7d0a 7d0b 7c0b 6417 1900  D.].\.}.}.|.d...
-00000a30: 7c09 6a31 6b02 72f7 7c09 6a2f 7c02 6416  |.j1k.r.|.j/|.d.
-00000a40: 1900 7c0a 1900 6418 3c00 71e3 71c9 8800  ..|...d.<.q.q...
-00000a50: 6a32 4400 5d0a 7d09 8800 a02e 7c09 a101  j2D.].}.....|...
-00000a60: 7c08 7c09 6a2f 3c00 71fc 8800 6a33 4400  |.|.j/<.q...j3D.
-00000a70: 5d0b 7d09 8800 a02e 7c09 a101 7c08 7c09  ].}.....|...|.|.
-00000a80: 6a2f 3c00 9001 710a 8800 6a34 4400 5d0b  j/<...q...j4D.].
-00000a90: 7d09 8800 a02e 7c09 a101 7c08 7c09 6a2f  }.....|...|.|.j/
-00000aa0: 3c00 9001 7119 7c07 6a16 7c08 7c02 6419  <...q.|.j.|.|.d.
-00000ab0: 8d02 0100 7c01 a035 7436 7c07 8301 a101  ....|..5t6|.....
-00000ac0: 0100 641a 8800 5f08 641b 5300 291c 7a86  ..d..._.d.S.).z.
-00000ad0: 0a20 2020 2020 2020 2043 7265 6174 6573  .        Creates
-00000ae0: 2077 6861 7420 6973 206b 6e6f 776e 2061   what is known a
-00000af0: 7320 7769 6e64 6f77 2e41 7070 2e73 7461  s window.App.sta
-00000b00: 7465 2e73 6974 655f 6461 7461 2069 6e20  te.site_data in 
-00000b10: 5265 6163 7420 636f 6465 2e0a 0a20 2020  React code...   
-00000b20: 2020 2020 203a 7061 7261 6d20 663a 2046       :param f: F
-00000b30: 696c 6520 6f62 6a65 6374 0a20 2020 2020  ile object.     
-00000b40: 2020 203a 7265 7475 726e 3a20 310a 2020     :return: 1.  
-00000b50: 2020 2020 2020 6301 0000 0000 0000 0000        c.........
-00000b60: 0000 0003 0000 0006 0000 0053 0000 0073  ...........S...s
-00000b70: 2400 0000 6900 7c00 5d0e 5c02 7d01 7d02  $...i.|.].\.}.}.
-00000b80: 7c01 6400 6401 8400 7c02 a000 a100 4400  |.d.d...|.....D.
-00000b90: 8301 9302 7102 5300 2902 6301 0000 0000  ....q.S.).c.....
-00000ba0: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
-00000bb0: 0000 0073 2400 0000 6700 7c00 5d0e 7d01  ...s$...g.|.].}.
-00000bc0: 7c01 6400 1900 6a00 7401 7c01 6401 1900  |.d...j.t.|.d...
-00000bd0: 8301 6402 9c02 9102 7102 5300 2903 7201  ..d.....q.S.).r.
-00000be0: 0000 0072 2d00 0000 2902 da05 7661 6c75  ...r-...)...valu
-00000bf0: 65da 0474 6578 7429 0272 4400 0000 da03  e..text).rD.....
-00000c00: 7374 7229 02da 022e 30da 0163 7237 0000  str)....0..cr7..
-00000c10: 0072 3700 0000 7238 0000 00da 0a3c 6c69  .r7...r8.....<li
-00000c20: 7374 636f 6d70 3e53 0000 0073 0200 0000  stcomp>S...s....
-00000c30: 2400 7a35 5265 6e64 6572 6572 2e77 7269  $.z5Renderer.wri
-00000c40: 7465 5f6c 696e 6f5f 6a73 2e3c 6c6f 6361  te_lino_js.<loca
-00000c50: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2e3c  ls>.<dictcomp>.<
-00000c60: 6c69 7374 636f 6d70 3e29 01da 0b67 6574  listcomp>)...get
-00000c70: 5f63 686f 6963 6573 2903 7247 0000 00da  _choices).rG....
-00000c80: 0249 44da 0263 6c72 3700 0000 7237 0000  .ID..clr7...r7..
-00000c90: 0072 3800 0000 da0a 3c64 6963 7463 6f6d  .r8.....<dictcom
-00000ca0: 703e 5100 0000 7308 0000 0006 0006 0312  p>Q...s.........
-00000cb0: ff06 fe7a 2a52 656e 6465 7265 722e 7772  ...z*Renderer.wr
-00000cc0: 6974 655f 6c69 6e6f 5f6a 732e 3c6c 6f63  ite_lino_js.<loc
-00000cd0: 616c 733e 2e3c 6469 6374 636f 6d70 3e54  als>.<dictcomp>T
-00000ce0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000cf0: 0006 0000 0013 0000 0073 1a00 0000 6900  .........s....i.
-00000d00: 7c00 5d09 7d01 7c01 6a00 8800 a001 7c01  |.].}.|.j.....|.
-00000d10: a101 9302 7102 5300 7237 0000 0029 02da  ....q.S.r7...)..
-00000d20: 0b61 6374 696f 6e5f 6e61 6d65 da0b 6163  .action_name..ac
-00000d30: 7469 6f6e 326a 736f 6e29 0272 4700 0000  tion2json).rG...
-00000d40: da01 61a9 0172 4000 0000 7237 0000 0072  ..a..r@...r7...r
-00000d50: 3800 0000 724d 0000 0060 0000 0073 0200  8...rM...`...s..
-00000d60: 0000 1a00 4e63 0100 0000 0000 0000 0000  ....Nc..........
-00000d70: 0000 0200 0000 0400 0000 5300 0000 7316  ..........S...s.
-00000d80: 0000 0069 007c 005d 077d 017c 016a 007c  ...i.|.].}.|.j.|
-00000d90: 016a 0193 0271 0253 0072 3700 0000 2902  .j...q.S.r7...).
-00000da0: da0b 646a 616e 676f 5f63 6f64 65da 046e  ..django_code..n
-00000db0: 616d 6529 0272 4700 0000 da04 6c61 6e67  ame).rG.....lang
-00000dc0: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
-00000dd0: 4d00 0000 6600 0000 7302 0000 0016 0029  M...f...s......)
-00000de0: 06da 0761 6374 696f 6e73 da04 6d65 6e75  ...actions..menu
-00000df0: da15 7573 655f 6461 7368 626f 6172 645f  ..use_dashboard_
-00000e00: 6c61 796f 7574 73da 0a73 6974 655f 7469  layouts..site_ti
-00000e10: 746c 65da 1065 6469 7469 6e67 5f66 726f  tle..editing_fro
-00000e20: 6e74 656e 64da 096c 616e 6775 6167 6573  ntend..languages
-00000e30: da04 6d65 6d6f 2901 da0a 7375 6767 6573  ..memo)...sugges
-00000e40: 746f 7273 2901 da0f 7265 7669 7369 6f6e  tors)...revision
-00000e50: 5f6e 756d 6265 72da 0572 6561 6374 7a07  _number..reactz.
-00000e60: 6d61 696e 2e6a 73da 0a74 6865 6d65 5f6e  main.js..theme_n
-00000e70: 616d 6529 0172 5f00 0000 2901 da0d 6e6f  ame).r_...)...no
-00000e80: 5f75 7365 725f 6d6f 6465 6cda 1961 6c6c  _user_model..all
-00000e90: 6f77 5f6f 6e6c 696e 655f 7265 6769 7374  ow_online_regist
-00000ea0: 7261 7469 6f6e 2901 7261 0000 00da 066e  ration).ra.....n
-00000eb0: 6f74 6966 7929 01da 0c75 7365 5f70 7573  otify)...use_pus
-00000ec0: 685f 6170 69da 0b63 686f 6963 655f 6e61  h_api..choice_na
-00000ed0: 6d65 7a10 7379 7374 656d 2e44 6173 6862  mez.system.Dashb
-00000ee0: 6f61 7264 7a17 7379 7374 656d 2e44 6173  oardz.system.Das
-00000ef0: 6862 6f61 7264 4c61 796f 7574 7372 4400  hboardLayoutsrD.
-00000f00: 0000 da0d 7769 6e64 6f77 5f6c 6179 6f75  ....window_layou
-00000f10: 7429 02da 0b66 6f72 6d5f 7061 6e65 6c73  t)...form_panels
-00000f20: 720d 0000 0046 722d 0000 0029 3772 2300  r....Fr-...)7r#.
-00000f30: 0000 da0b 4348 4f49 4345 4c49 5354 53da  ....CHOICELISTS.
-00000f40: 0569 7465 6d73 da03 7365 74da 0b61 6374  .items..set..act
-00000f50: 6f72 735f 6c69 7374 da0b 6765 745f 6163  ors_list..get_ac
-00000f60: 7469 6f6e 73da 0661 6374 696f 6eda 0361  tions..action..a
-00000f70: 6464 da11 7365 7269 616c 6973 655f 6a73  dd..serialise_js
-00000f80: 5f63 6f64 6572 0400 0000 da04 5349 5445  _coder......SITE
-00000f90: da07 706c 7567 696e 73da 0464 6963 74da  ..plugins..dict.
-00000fa0: 0d67 6574 5f73 6974 655f 6d65 6e75 7229  .get_site_menur)
-00000fb0: 0000 00da 0673 7973 7465 6d72 5700 0000  .....systemrW...
-00000fc0: da05 7469 746c 6572 4100 0000 da0a 7572  ..titlerA.....ur
-00000fd0: 6c5f 7072 6566 6978 725a 0000 00da 0c69  l_prefixrZ.....i
-00000fe0: 735f 696e 7374 616c 6c65 64da 0675 7064  s_installed..upd
-00000ff0: 6174 65da 046c 6973 7472 5b00 0000 da06  ate..listr[.....
-00001000: 7061 7273 6572 da0a 7375 6767 6573 7465  parser..suggeste
-00001010: 7273 da04 6b65 7973 da0a 636f 6465 5f6d  rs..keys..code_m
-00001020: 7469 6d65 da02 6f73 da04 7374 6174 7202  time..os..statr.
-00001030: 0000 00da 0b53 5441 5449 435f 524f 4f54  .....STATIC_ROOT
-00001040: da08 7374 5f6d 7469 6d65 720c 0000 00da  ..st_mtimer.....
-00001050: 1b55 524c 5f50 4152 414d 5f4d 4149 4e5f  .URL_PARAM_MAIN_
-00001060: 4a53 5f54 494d 4553 5441 4d50 da11 4669  JS_TIMESTAMP..Fi
-00001070: 6c65 4e6f 7446 6f75 6e64 4572 726f 72da  leNotFoundError.
-00001080: 0768 6173 6174 7472 725f 0000 00da 0a75  .hasattrr_.....u
-00001090: 7365 725f 6d6f 6465 6cda 0575 7365 7273  ser_model..users
-000010a0: 7261 0000 0072 6200 0000 7263 0000 00da  ra...rb...rc....
-000010b0: 0975 7365 5f6c 696e 6f64 7266 0000 00da  .use_linodrf....
-000010c0: 0a70 616e 656c 326a 736f 6eda 0f5f 666f  .panel2json.._fo
-000010d0: 726d 7061 6e65 6c5f 6e61 6d65 7231 0000  rmpanel_namer1..
-000010e0: 0072 6400 0000 da0c 7061 7261 6d5f 7061  .rd.....param_pa
-000010f0: 6e65 6c73 da13 6163 7469 6f6e 5f70 6172  nels..action_par
-00001100: 616d 5f70 616e 656c 73da 0c6f 7468 6572  am_panels..other
-00001110: 5f70 616e 656c 73da 0577 7269 7465 7226  _panels..writer&
-00001120: 0000 0029 0c72 4000 0000 da01 66da 1063  ...).r@.....f..c
-00001130: 686f 6963 656c 6973 7473 5f64 6174 6172  hoicelists_datar
-00001140: 5500 0000 da03 7270 74da 0262 6172 7000  U.....rpt..barp.
-00001150: 0000 da04 6461 7461 7266 0000 00da 0170  ....datarf.....p
-00001160: 7235 0000 00da 0469 7465 6d72 3700 0000  r5.....itemr7...
-00001170: 7251 0000 0072 3800 0000 da0d 7772 6974  rQ...r8.....writ
-00001180: 655f 6c69 6e6f 5f6a 734a 0000 0073 7800  e_lino_jsJ...sx.
-00001190: 0000 0607 0803 06fd 0605 0a01 0c02 0a01  ................
-000011a0: 0c01 0280 02fe 0604 0801 0201 1001 0c02  ................
-000011b0: 0601 0601 0a01 1001 06f9 0c09 0402 1001  ................
-000011c0: 06ff 1206 0201 0401 1001 02ff 0202 0cfe  ................
-000011d0: 0c03 0401 02ff 0c03 1001 0c02 0e01 0c01  ................
-000011e0: 1001 0c02 1801 0409 0a01 1001 1401 1401  ................
-000011f0: 0e01 1201 0480 0a01 1201 0a01 1401 0a01  ................
-00001200: 1401 0e01 0e05 0602 0401 7a16 5265 6e64  ..........z.Rend
-00001210: 6572 6572 2e77 7269 7465 5f6c 696e 6f5f  erer.write_lino_
-00001220: 6a73 6302 0000 0000 0000 0000 0000 0004  jsc.............
-00001230: 0000 0006 0000 0043 0000 0073 c600 0000  .......C...s....
-00001240: 7400 7c01 7401 8302 7307 4a00 8201 7402  t.|.t...s.J...t.
-00001250: 7c01 6a03 7c01 a004 a100 7c01 a005 a100  |.j.|.....|.....
-00001260: 7c01 6a06 6401 8d04 7d02 7400 7c01 7407  |.j.d...}.t.|.t.
-00001270: 8302 7229 7c01 6a08 6a09 6a03 7c02 6402  ..r)|.j.j.j.|.d.
-00001280: 3c00 740a 7c01 6a08 6a0b 8301 7c02 6403  <.t.|.j.j...|.d.
-00001290: 3c00 7c01 6a0c 7231 7c01 6a0c 7c02 6404  <.|.j.r1|.j.|.d.
-000012a0: 3c00 7c01 6a0d 7239 7c01 6a0d 7c02 6405  <.|.j.r9|.j.|.d.
-000012b0: 3c00 7c01 6a0e 7240 6406 7c02 6407 3c00  <.|.j.r@d.|.d.<.
-000012c0: 7c01 6a0f 7248 7c01 6a0f 7c02 6408 3c00  |.j.rH|.j.|.d.<.
-000012d0: 7c01 6a10 724f 6406 7c02 6409 3c00 7c01  |.j.rOd.|.d.<.|.
-000012e0: 6a11 7256 6406 7c02 640a 3c00 7c00 a012  j.rVd.|.d.<.|...
-000012f0: 7c01 a101 7d03 7c03 7261 7c03 7c02 640b  |...}.|.ra|.|.d.
-00001300: 3c00 7c02 5300 290c 7a33 436f 6e76 6572  <.|.S.).z3Conver
-00001310: 7473 2067 6c6f 6261 6c20 6c69 7374 206f  ts global list o
-00001320: 6620 616c 6c20 6163 7469 6f6e 7320 746f  f all actions to
-00001330: 206a 736f 6e20 666f 726d 6174 2e29 04da   json format.)..
-00001340: 0261 6eda 056c 6162 656c da0d 7769 6e64  .an..label..wind
-00001350: 6f77 5f61 6374 696f 6eda 0b68 7474 705f  ow_action..http_
-00001360: 6d65 7468 6f64 7295 0000 00da 0561 6374  methodr......act
-00001370: 6f72 da0c 7072 6570 726f 6365 7373 6f72  or..preprocessor
-00001380: da0b 7365 6c65 6374 5f72 6f77 7354 da10  ..select_rowsT..
-00001390: 7375 626d 6974 5f66 6f72 6d5f 6461 7461  submit_form_data
-000013a0: da0b 6275 7474 6f6e 5f74 6578 74da 1473  ..button_text..s
-000013b0: 686f 775f 696e 5f73 6964 655f 746f 6f6c  how_in_side_tool
-000013c0: 6261 72da 0e6e 6576 6572 5f63 6f6c 6c61  bar..never_colla
-000013d0: 7073 65da 0469 636f 6e29 13da 0a69 7369  pse..icon)...isi
-000013e0: 6e73 7461 6e63 6572 1700 0000 7271 0000  nstancer....rq..
-000013f0: 0072 4e00 0000 da09 6765 745f 6c61 6265  .rN.....get_labe
-00001400: 6cda 1069 735f 7769 6e64 6f77 5f61 6374  l..is_window_act
-00001410: 696f 6e72 9800 0000 7212 0000 00da 0c62  ionr....r......b
-00001420: 6f75 6e64 5f61 6374 696f 6e72 6c00 0000  ound_actionrl...
-00001430: 7246 0000 0072 9900 0000 729a 0000 0072  rF...r....r....r
-00001440: 9b00 0000 729c 0000 0072 9d00 0000 729e  ....r....r....r.
-00001450: 0000 0072 9f00 0000 da0f 6765 745f 6163  ...r......get_ac
-00001460: 7469 6f6e 5f69 636f 6e29 0472 4000 0000  tion_icon).r@...
-00001470: da01 76da 0672 6573 756c 7472 a000 0000  ..v..resultr....
-00001480: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
-00001490: 4f00 0000 a100 0000 7324 0000 000e 0206  O.......s$......
-000014a0: 0406 0106 0104 0106 fd0a 060e 0110 0110  ................
-000014b0: 0210 020e 0110 010e 010e 010a 020c 0104  ................
-000014c0: 027a 1452 656e 6465 7265 722e 6163 7469  .z.Renderer.acti
-000014d0: 6f6e 326a 736f 6e63 0200 0000 0000 0000  on2jsonc........
-000014e0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-000014f0: 732e 0000 0074 007c 0174 0183 0273 074a  s....t.|.t...s.J
-00001500: 0082 017c 01a0 02a1 007d 0274 037c 00a0  ...|.....}.t.|..
-00001510: 047c 026a 05a1 017c 026a 066a 0764 018d  .|.j...|.j.j.d..
-00001520: 0253 0029 024e 2902 da04 6d61 696e da0b  .S.).N)...main..
-00001530: 7769 6e64 6f77 5f73 697a 6529 0872 a100  window_size).r..
-00001540: 0000 721d 0000 00da 1167 6574 5f6c 6179  ..r......get_lay
-00001550: 6f75 745f 6861 6e64 6c65 7271 0000 00da  out_handlerq....
-00001560: 0965 6c65 6d32 6a73 6f6e 72a8 0000 00da  .elem2jsonr.....
-00001570: 066c 6179 6f75 7472 a900 0000 2903 7240  .layoutr....).r@
-00001580: 0000 0072 9200 0000 72a6 0000 0072 3700  ...r....r....r7.
-00001590: 0000 7237 0000 0072 3800 0000 7287 0000  ..r7...r8...r...
-000015a0: 00be 0000 0073 0a00 0000 0e01 0803 0c01  .....s..........
-000015b0: 0601 06ff 7a13 5265 6e64 6572 6572 2e70  ....z.Renderer.p
-000015c0: 616e 656c 326a 736f 6e63 0200 0000 0000  anel2jsonc......
-000015d0: 0000 0000 0000 0400 0000 0500 0000 0300  ................
-000015e0: 0000 73da 0000 0074 007c 0174 0183 0273  ..s....t.|.t...s
-000015f0: 074a 0082 0174 027c 01a0 03a1 007c 016a  .J...t.|.....|.j
-00001600: 047c 016a 056a 0664 018d 037d 0274 077c  .|.j.j.d...}.t.|
-00001610: 0164 0283 0272 2487 0066 0164 0364 0484  .d...r$..f.d.d..
-00001620: 087c 016a 0844 0083 017c 0264 053c 007c  .|.j.D...|.d.<.|
-00001630: 02a0 0974 0a7c 0164 0683 02a1 0101 0074  ...t.|.d.......t
-00001640: 077c 0164 0783 0272 557c 02a0 0974 0a7c  .|.d...rU|...t.|
-00001650: 016a 0b64 0883 02a1 0101 0074 077c 0164  .j.d.......t.|.d
-00001660: 0983 0272 557c 016a 0c64 0075 0172 557c  ...rU|.j.d.u.rU|
-00001670: 016a 0ca0 0da1 0044 005d 0b5c 027d 037d  .j.....D.].\.}.}
-00001680: 0188 00a0 0e7c 01a1 017c 027c 033c 0071  .....|...|.|.<.q
-00001690: 4974 0f7c 016a 0574 1083 0272 6b7c 026a  It.|.j.t...rk|.j
-000016a0: 097c 01a0 11a1 0064 0a8d 0101 007c 026a  .|.....d.....|.j
-000016b0: 097c 016a 126a 1364 0b8d 0101 007c 0253  .|.j.j.d.....|.S
-000016c0: 0029 0c4e 2903 7296 0000 00da 0873 6f72  .).N).r......sor
-000016d0: 7461 626c 65da 0a72 6561 6374 5f6e 616d  table..react_nam
-000016e0: 65da 0865 6c65 6d65 6e74 7363 0100 0000  e..elementsc....
-000016f0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00001700: 1300 0000 731e 0000 0067 007c 005d 0b7d  ....s....g.|.].}
-00001710: 017c 01a0 00a1 0072 0288 00a0 017c 01a1  .|.....r.....|..
-00001720: 0191 0271 0253 0072 3700 0000 2902 da0a  ...q.S.r7...)...
-00001730: 6973 5f76 6973 6962 6c65 72ab 0000 0029  is_visibler....)
-00001740: 0272 4700 0000 da01 6572 5100 0000 7237  .rG.....erQ...r7
-00001750: 0000 0072 3800 0000 7249 0000 00ce 0000  ...r8...rI......
-00001760: 0073 0200 0000 1e00 7a26 5265 6e64 6572  .s......z&Render
-00001770: 6572 2e65 6c65 6d32 6a73 6f6e 2e3c 6c6f  er.elem2json.<lo
-00001780: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001790: 7268 0000 007a 9866 6965 6c64 735f 696e  rh...z.fields_in
-000017a0: 6465 7820 6669 656c 6473 5f69 6e64 6578  dex fields_index
-000017b0: 5f68 6964 6465 6e20 6564 6974 6162 6c65  _hidden editable
-000017c0: 2076 6572 7469 6361 6c20 6870 6164 2069   vertical hpad i
-000017d0: 735f 6669 656c 6473 6574 206e 616d 6520  s_fieldset name 
-000017e0: 7769 6474 6820 7072 6566 6572 7265 645f  width preferred_
-000017f0: 7769 6474 6820 2020 2020 2020 2020 2020  width           
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 2020 2020 2020 2068 6964 6465 6e20 7661         hidden va
-00001820: 6c75 6520 6866 6c65 7820 7666 6c65 7872  lue hflex vflexr
-00001830: 9900 0000 7a15 6163 746f 725f 6964 2064  ....z.actor_id d
-00001840: 6973 706c 6179 5f6d 6f64 65da 0673 6c61  isplay_mode..sla
-00001850: 7665 7329 01da 0d66 6965 6c64 5f6f 7074  ves)...field_opt
-00001860: 696f 6e73 2901 da09 6865 6c70 5f74 6578  ions)...help_tex
-00001870: 7429 1472 a100 0000 721e 0000 0072 7100  t).r....r....rq.
-00001880: 0000 72a2 0000 0072 ad00 0000 7243 0000  ..r....r....rC..
-00001890: 00da 085f 5f6e 616d 655f 5f72 8300 0000  ...__name__r....
-000018a0: 72af 0000 0072 7700 0000 7228 0000 0072  r....rw...r(...r
-000018b0: 9900 0000 72b2 0000 0072 6800 0000 72ab  ....r....rh...r.
-000018c0: 0000 00da 0a69 7373 7562 636c 6173 7372  .....issubclassr
-000018d0: 2100 0000 da11 6765 745f 6669 656c 645f  !.....get_field_
-000018e0: 6f70 7469 6f6e 73da 0566 6965 6c64 72b4  options..fieldr.
-000018f0: 0000 0029 0472 4000 0000 72a6 0000 0072  ...).r@...r....r
-00001900: a700 0000 da01 6b72 3700 0000 7251 0000  ......kr7...rQ..
-00001910: 0072 3800 0000 72ab 0000 00c6 0000 0073  .r8...r........s
-00001920: 2200 0000 0e01 0802 0401 0602 06fd 0a04  "...............
-00001930: 1801 1002 0a04 1202 1403 1201 1001 0c03  ................
-00001940: 1001 1001 0402 7a12 5265 6e64 6572 6572  ......z.Renderer
-00001950: 2e65 6c65 6d32 6a73 6f6e 6301 0000 0000  .elem2jsonc.....
-00001960: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001970: 0000 0073 0400 0000 6401 5300 2902 4e7a  ...s....d.S.).Nz
-00001980: 1e77 696e 646f 772e 4170 702e 6461 7368  .window.App.dash
-00001990: 626f 6172 642e 7265 6c6f 6164 2829 3b72  board.reload();r
-000019a0: 3700 0000 7251 0000 0072 3700 0000 7237  7...rQ...r7...r7
-000019b0: 0000 0072 3800 0000 da09 7265 6c6f 6164  ...r8.....reload
-000019c0: 5f6a 73e6 0000 0073 0200 0000 0401 7a12  _js....s......z.
-000019d0: 5265 6e64 6572 6572 2e72 656c 6f61 645f  Renderer.reload_
-000019e0: 6a73 6302 0000 0000 0000 0000 0000 0006  jsc.............
-000019f0: 0000 0004 0000 004f 0000 0073 dc00 0000  .......O...s....
-00001a00: 7c01 6a00 6a01 6401 6b02 720f 7c00 6a02  |.j.j.d.k.r.|.j.
-00001a10: 6a03 7c02 6900 7c03 a401 8e01 5300 7c01  j.|.i.|.....S.|.
-00001a20: a004 a100 7d04 7c03 a005 7c04 6402 1900  ....}.|...|.d...
-00001a30: a101 0100 7406 7c03 7c01 8302 0100 7c01  ....t.|.|.....|.
-00001a40: 6a07 6403 7501 722c 7c03 a008 7409 6a0a  j.d.u.r,|...t.j.
-00001a50: 7c01 6a07 a102 0100 7c01 6a0b 6403 7501  |.j.....|.j.d.u.
-00001a60: 7239 7c03 a008 7409 6a0c 7c01 6a0b a102  r9|...t.j.|.j...
-00001a70: 0100 7c01 6a0d 6403 7501 725c 7c01 6a0d  ..|.j.d.u.r\|.j.
-00001a80: 6404 1900 7d05 7c05 a00e 6405 a101 7255  d...}.|...d...rU
-00001a90: 7c05 6406 6403 8502 1900 7d05 7c03 a008  |.d.d.....}.|...
-00001aa0: 7409 6a0f 6407 a102 0100 7c03 a008 7409  t.j.d.....|...t.
-00001ab0: 6a10 7c05 a102 0100 7c00 6a02 6a03 7c01  j.|.....|.j.j.|.
-00001ac0: 6a00 6a11 7c01 6a00 6a01 6702 7c02 a201  j.j.|.j.j.g.|...
-00001ad0: 5200 6900 7c03 a401 8e01 5300 2908 7a20  R.i.|.....S.).z 
-00001ae0: 5573 6564 2066 6f72 2074 7572 6e20 7265  Used for turn re
-00001af0: 7175 6573 7473 2069 6e74 6f20 7572 6c73  quests into urls
-00001b00: da04 4d61 696e da0b 6261 7365 5f70 6172  ..Main..base_par
-00001b10: 616d 734e 7201 0000 00fa 012d 722d 0000  amsNr......-r-..
-00001b20: 00da 0444 4553 4329 1272 9900 0000 72b5  ...DESC).r....r.
-00001b30: 0000 0072 4100 0000 da0f 6275 696c 645f  ...rA.....build_
-00001b40: 706c 6169 6e5f 7572 6cda 0a67 6574 5f73  plain_url..get_s
-00001b50: 7461 7475 7372 7700 0000 7208 0000 00da  tatusrw...r.....
-00001b60: 066f 6666 7365 74da 0a73 6574 6465 6661  .offset..setdefa
-00001b70: 756c 7472 0c00 0000 da0f 5552 4c5f 5041  ultr......URL_PA
-00001b80: 5241 4d5f 5354 4152 54da 056c 696d 6974  RAM_START..limit
-00001b90: da0f 5552 4c5f 5041 5241 4d5f 4c49 4d49  ..URL_PARAM_LIMI
-00001ba0: 54da 086f 7264 6572 5f62 79da 0a73 7461  T..order_by..sta
-00001bb0: 7274 7377 6974 68da 1155 524c 5f50 4152  rtswith..URL_PAR
-00001bc0: 414d 5f53 4f52 5444 4952 da0e 5552 4c5f  AM_SORTDIR..URL_
-00001bd0: 5041 5241 4d5f 534f 5254 da09 6170 705f  PARAM_SORT..app_
-00001be0: 6c61 6265 6c29 0672 4000 0000 da02 6172  label).r@.....ar
-00001bf0: da04 6172 6773 da02 6b77 da02 7374 da02  ..args..kw..st..
-00001c00: 7363 7237 0000 0072 3700 0000 7238 0000  scr7...r7...r8..
-00001c10: 00da 0f67 6574 5f72 6571 7565 7374 5f75  ...get_request_u
-00001c20: 726c e900 0000 732c 0000 000c 0212 0108  rl....s,........
-00001c30: 020e 010a 010a 0110 010a 0110 010a 010a  ................
-00001c40: 010a 010c 010e 010e 0106 030c 0102 ff02  ................
-00001c50: 0106 ff02 0106 ff7a 1852 656e 6465 7265  .......z.Rendere
-00001c60: 722e 6765 745f 7265 7175 6573 745f 7572  r.get_request_ur
-00001c70: 6c4e 6305 0000 0000 0000 0000 0000 0007  lNc.............
-00001c80: 0000 0005 0000 004b 0000 0073 ae00 0000  .......K...s....
-00001c90: 7c04 7005 7c03 a000 a100 7d04 7401 7c04  |.p.|.....}.t.|.
-00001ca0: 8301 6401 6b02 7211 6402 a002 7c04 a101  ..d.k.r.d...|...
-00001cb0: 7d04 7c03 6a03 6a04 722c 7c03 6a03 6a05  }.|.j.j.r,|.j.j.
-00001cc0: 732c 7c00 a006 7c02 7c03 7c01 a103 7d06  s,|...|.|.|...}.
-00001cd0: 7c00 6a07 7c02 7c03 7c06 7c04 6604 6900  |.j.|.|.|.|.f.i.
-00001ce0: 7c05 a401 8e01 5300 7c03 6a03 6a08 724b  |.....S.|.j.j.rK
-00001cf0: 7c02 a009 a100 7d06 7c01 6400 7501 723f  |.....}.|.d.u.r?
-00001d00: 7c06 6a0a 7c01 6a0b 6403 8d01 0100 7c00  |.j.|.j.d.....|.
-00001d10: 6a07 7c02 7c03 7c06 7c04 6604 6900 7c05  j.|.|.|.|.f.i.|.
-00001d20: a401 8e01 5300 7c00 6a0c 7c01 7c02 7c03  ....S.|.j.|.|.|.
-00001d30: 7c04 6604 6900 7c05 a401 8e01 5300 2904  |.f.i.|.....S.).
-00001d40: 4e72 2d00 0000 7506 0000 00c2 a07b 7dc2  Nr-...u......{}.
-00001d50: a029 01da 0972 6563 6f72 645f 6964 290d  .)...record_id).
-00001d60: da10 6765 745f 6275 7474 6f6e 5f6c 6162  ..get_button_lab
-00001d70: 656c da03 6c65 6eda 0666 6f72 6d61 7472  el..len..formatr
-00001d80: 6c00 0000 da0a 7061 7261 6d65 7465 7273  l.....parameters
-00001d90: da10 6e6f 5f70 6172 616d 735f 7769 6e64  ..no_params_wind
-00001da0: 6f77 da11 6765 745f 6163 7469 6f6e 5f73  ow..get_action_s
-00001db0: 7461 7475 73da 1477 696e 646f 775f 6163  tatus..window_ac
-00001dc0: 7469 6f6e 5f62 7574 746f 6eda 0e6f 7065  tion_button..ope
-00001dd0: 6e73 5f61 5f77 696e 646f 7772 c000 0000  ns_a_windowr....
-00001de0: 7277 0000 00da 0270 6bda 1172 6f77 5f61  rw.....pk..row_a
-00001df0: 6374 696f 6e5f 6275 7474 6f6e 2907 7240  ction_button).r@
-00001e00: 0000 00da 036f 626a 72cb 0000 0072 9000  .....objr....r..
-00001e10: 0000 7296 0000 0072 cd00 0000 72ce 0000  ..r....r....r...
-00001e20: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
-00001e30: da0d 6163 7469 6f6e 5f62 7574 746f 6e01  ..action_button.
-00001e40: 0100 0073 2000 0000 0c01 0c01 0a01 1002  ...s ...........
-00001e50: 0e01 0401 0801 04ff 0201 06ff 0802 0801  ................
-00001e60: 0801 0e01 1801 1801 7a16 5265 6e64 6572  ........z.Render
-00001e70: 6572 2e61 6374 696f 6e5f 6275 7474 6f6e  er.action_button
-00001e80: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
-00001e90: 0004 0000 004b 0000 0073 4000 0000 7c02  .....K...s@...|.
-00001ea0: 6401 7500 720d 7c03 6a00 6402 6900 7c04  d.u.r.|.j.d.i.|.
-00001eb0: a401 8e01 7d06 6e09 7c02 6a01 7c03 6601  ....}.n.|.j.|.f.
-00001ec0: 6900 7c04 a401 8e01 7d06 7c00 6a02 7c06  i.|.....}.|.j.|.
-00001ed0: 7c01 6602 6900 7c05 a401 8e01 5300 2903  |.f.i.|.....S.).
-00001ee0: 61cf 0100 004e 6f74 6520 7468 6174 2060  a....Note that `
-00001ef0: 6261 2e61 6374 6f72 6020 6d61 7920 6469  ba.actor` may di
-00001f00: 6666 6572 2066 726f 6d20 6061 722e 6163  ffer from `ar.ac
-00001f10: 746f 7260 2077 6865 6e20 6465 6669 6e65  tor` when define
-00001f20: 6420 6f6e 2061 0a20 2020 2020 2020 2064  d on a.        d
-00001f30: 6966 6665 7265 6e74 2061 6374 6f72 2e20  ifferent actor. 
-00001f40: 5265 6d65 6d62 6572 2065 2e67 2e20 7468  Remember e.g. th
-00001f50: 6520 224d 7573 7420 7265 6164 2065 4944  e "Must read eID
-00001f60: 2063 6172 6422 2061 6374 696f 6e0a 2020   card" action.  
-00001f70: 2020 2020 2020 6275 7474 6f6e 2069 6e20        button in 
-00001f80: 6569 645f 696e 666f 206f 6620 6e65 7763  eid_info of newc
-00001f90: 6f6d 6572 732e 4e65 7743 6c69 656e 7473  omers.NewClients
-00001fa0: 2028 3230 3134 3034 3232 292e 0a0a 2020   (20140422)...  
-00001fb0: 2020 2020 2020 3a6f 626a 3a20 2054 6865        :obj:  The
-00001fc0: 2064 6174 6162 6173 6520 6f62 6a65 6374   database object
-00001fd0: 0a20 2020 2020 2020 203a 6172 3a20 2020  .        :ar:   
-00001fe0: 5468 6520 6163 7469 6f6e 2072 6571 7565  The action reque
-00001ff0: 7374 0a20 2020 2020 2020 203a 6261 3a20  st.        :ba: 
-00002000: 2054 6865 2062 6f75 6e64 2061 6374 696f   The bound actio
-00002010: 6e0a 2020 2020 2020 2020 3a72 6571 7565  n.        :reque
-00002020: 7374 5f6b 7761 7267 733a 206b 6579 776f  st_kwargs: keywo
-00002030: 7264 2061 7267 756d 656e 7473 2074 6f20  rd arguments to 
-00002040: 666f 7277 6172 6465 6420 746f 2074 6865  forwarded to the
-00002050: 2063 6869 6c64 2061 6374 696f 6e20 7265   child action re
-00002060: 7175 6573 740a 0a20 2020 2020 2020 2041  quest..        A
-00002070: 6e79 206b 6579 776f 7264 206f 7468 6572  ny keyword other
-00002080: 2061 7267 756d 656e 7473 2061 7265 2066   arguments are f
-00002090: 6f72 7761 7264 6564 2074 6f20 3a6d 6574  orwarded to :met
-000020a0: 683a 6061 7232 6a73 602e 0a0a 2020 2020  h:`ar2js`...    
-000020b0: 2020 2020 4e72 3700 0000 2903 da07 7265      Nr7...)...re
-000020c0: 7175 6573 74da 0573 7061 776e da05 6172  quest..spawn..ar
-000020d0: 326a 7329 0772 4000 0000 72dc 0000 0072  2js).r@...r....r
-000020e0: cb00 0000 7290 0000 00da 0e72 6571 7565  ....r......reque
-000020f0: 7374 5f6b 7761 7267 73da 0673 7461 7475  st_kwargs..statu
-00002100: 73da 0373 6172 7237 0000 0072 3700 0000  s..sarr7...r7...
-00002110: 7238 0000 00da 1761 6374 696f 6e5f 6361  r8.....action_ca
-00002120: 6c6c 5f6f 6e5f 696e 7374 616e 6365 1201  ll_on_instance..
-00002130: 0000 7308 0000 0008 0e12 0112 0314 017a  ..s............z
-00002140: 2052 656e 6465 7265 722e 6163 7469 6f6e   Renderer.action
-00002150: 5f63 616c 6c5f 6f6e 5f69 6e73 7461 6e63  _call_on_instanc
-00002160: 6563 0200 0000 0000 0000 0000 0000 0400  ec..............
-00002170: 0000 0400 0000 4300 0000 732c 0000 007c  ......C...s,...|
-00002180: 016a 0070 057c 016a 017d 0274 02a0 037c  .j.p.|.j.}.t...|
-00002190: 0264 01a1 027d 037c 0364 0175 0072 1264  .d...}.|.d.u.r.d
-000021a0: 0153 0064 027c 0316 0053 0029 037a bf0a  .S.d.|...S.).z..
-000021b0: 2020 2020 2020 2020 5573 6573 2061 6e20          Uses an 
-000021c0: 696e 7465 726e 616c 206d 6170 7069 6e67  internal mapping
-000021d0: 2066 6f72 2069 636f 6e20 6e61 6d65 7320   for icon names 
-000021e0: 746f 2063 6f6e 7665 7274 2065 7869 7374  to convert exist
-000021f0: 696e 6720 6963 6f6e 7320 696e 746f 2072  ing icons into r
-00002200: 6561 6374 2d75 7361 626c 652e 0a20 2020  eact-usable..   
-00002210: 2020 2020 203a 7061 7261 6d20 6163 7469       :param acti
-00002220: 6f6e 3a0a 2020 2020 2020 2020 3a72 6574  on:.        :ret
-00002230: 7572 6e3a 2073 7472 3a20 6120 6963 6f6e  urn: str: a icon
-00002240: 206e 616d 6520 666f 7220 6569 7468 6572   name for either
-00002250: 2070 7269 6d65 2d72 6561 6374 206f 7220   prime-react or 
-00002260: 6963 6f6e 380a 2020 2020 2020 2020 4e7a  icon8.        Nz
-00002270: 0570 6920 2573 2904 da0f 7265 6163 745f  .pi %s)...react_
-00002280: 6963 6f6e 5f6e 616d 65da 0969 636f 6e5f  icon_name..icon_
-00002290: 6e61 6d65 722e 0000 00da 0367 6574 2904  namer......get).
-000022a0: 7240 0000 0072 6c00 0000 72a0 0000 00da  r@...rl...r.....
-000022b0: 0a72 6561 6374 5f69 636f 6e72 3700 0000  .react_iconr7...
-000022c0: 7237 0000 0072 3800 0000 72a5 0000 0027  r7...r8...r....'
-000022d0: 0100 0073 0a00 0000 0c07 0c01 0801 0401  ...s............
-000022e0: 0802 7a18 5265 6e64 6572 6572 2e67 6574  ..z.Renderer.get
-000022f0: 5f61 6374 696f 6e5f 6963 6f6e 6303 0000  _action_iconc...
-00002300: 0000 0000 0000 0000 0008 0000 0007 0000  ................
-00002310: 004b 0000 0073 a400 0000 7c01 6a00 7d04  .K...s....|.j.}.
-00002320: 7c01 6a01 7d05 6900 7d06 7c05 6a02 a003  |.j.}.i.}.|.j...
-00002330: a100 721c 7c03 a004 7c00 a005 7c01 7c05  ..r.|...|...|.|.
-00002340: 7c02 a103 a101 0100 7c06 a004 7c03 a101  |.......|...|...
-00002350: 0100 7c06 a004 7c00 a006 7c01 7c05 7c02  ..|...|...|.|.|.
-00002360: a103 a101 0100 7c06 a004 7c03 a101 0100  ......|...|.....
-00002370: 7c04 7c05 6a02 6a07 7c01 6a08 7c05 6a09  |.|.j.j.|.j.|.j.
-00002380: 6a0a 7c06 6401 9c05 7d07 740b 7c02 6402  j.|.d...}.t.|.d.
-00002390: 8302 7243 7c02 6a0c 7c07 6403 3c00 6e09  ..rC|.j.|.d.<.n.
-000023a0: 740d 7c02 740e 8302 724c 7c02 7c07 6403  t.|.t...rL|.|.d.
-000023b0: 3c00 6404 740f 7c07 8301 1600 5300 2905  <.d.t.|.....S.).
-000023c0: 7a43 496d 706c 656d 656e 7473 203a 6d65  zCImplements :me
-000023d0: 7468 3a60 6c69 6e6f 2e63 6f72 652e 7265  th:`lino.core.re
-000023e0: 6e64 6572 6572 2e48 746d 6c52 656e 6465  nderer.HtmlRende
-000023f0: 7265 722e 6172 326a 7360 2e0a 0a20 2020  rer.ar2js`...   
-00002400: 2020 2020 2029 05da 0272 7072 9500 0000       )...rpr....
-00002410: da06 6f6e 4d61 696e da07 6163 746f 7249  ..onMain..actorI
-00002420: 6472 e200 0000 72da 0000 00da 0273 72fa  dr....r......sr.
-00002430: 1877 696e 646f 772e 4170 702e 7275 6e41  .window.App.runA
-00002440: 6374 696f 6e28 2573 2929 10da 1072 6571  ction(%s))...req
-00002450: 7565 7374 696e 675f 7061 6e65 6c72 a400  uesting_panelr..
-00002460: 0000 726c 0000 0072 a300 0000 7277 0000  ..rl...r....rw..
-00002470: 0072 d700 0000 da11 6765 745f 6163 7469  .r......get_acti
-00002480: 6f6e 5f70 6172 616d 7372 4e00 0000 da10  on_paramsrN.....
-00002490: 6973 5f6f 6e5f 6d61 696e 5f61 6374 6f72  is_on_main_actor
-000024a0: 7299 0000 00da 0861 6374 6f72 5f69 6472  r......actor_idr
-000024b0: 8300 0000 72da 0000 0072 a100 0000 7278  ....r....r....rx
-000024c0: 0000 0072 2600 0000 2908 7240 0000 0072  ...r&...).r@...r
-000024d0: cb00 0000 72dc 0000 0072 e200 0000 72e9  ....r....r....r.
-000024e0: 0000 0072 9000 0000 da06 7061 7261 6d73  ...r......params
-000024f0: da06 6a73 5f6f 626a 7237 0000 0072 3700  ..js_objr7...r7.
-00002500: 0000 7238 0000 0072 e000 0000 3501 0000  ..r8...r....5...
-00002510: 732a 0000 0006 0406 0104 010a 0114 040a  s*..............
-00002520: 0114 010a 0102 0306 0104 0106 0102 0106  ................
-00002530: fb0a 070c 010a 0208 0102 0206 0104 ff7a  ...............z
-00002540: 0e52 656e 6465 7265 722e 6172 326a 7363  .Renderer.ar2jsc
-00002550: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00002560: 0600 0000 4300 0000 73bc 0100 007c 0174  ....C...s....|.t
-00002570: 006a 016a 0275 0072 0a74 0364 0183 0153  .j.j.u.r.t.d...S
-00002580: 0074 047c 0174 0583 0272 1674 0664 02a0  .t.|.t...r.t.d..
-00002590: 077c 01a1 0183 0182 0174 047c 0174 086a  .|.......t.|.t.j
-000025a0: 0983 0272 2009 007c 016a 0a53 0074 047c  ...r ..|.j.S.t.|
-000025b0: 0174 0b6a 0c83 0272 297c 016a 0d53 0074  .t.j...r)|.j.S.t
-000025c0: 047c 0174 0683 0272 3274 0e7c 0183 0153  .|.t...r2t.|...S
-000025d0: 0074 047c 0174 0f83 0272 4a7c 016a 1064  .t.|.t...rJ|.j.d
-000025e0: 0375 0072 3f7c 016a 1153 0074 127c 016a  .u.r?|.j.S.t.|.j
-000025f0: 1374 127c 016a 1164 048d 0164 058d 0253  .t.|.j.d...d...S
-00002600: 0074 047c 0174 1483 0272 cc7c 016a 1564  .t.|.t...r.|.j.d
-00002610: 0375 0172 6d7c 00a0 1664 037c 016a 1564  .u.rm|...d.|.j.d
-00002620: 03a1 037d 027c 0264 0375 0173 624a 0082  ...}.|.d.u.sbJ..
-00002630: 0164 067c 0216 007d 037c 00a0 177c 017c  .d.|...}.|...|.|
-00002640: 0264 03a1 0353 007c 016a 1864 0375 0172  .d...S.|.j.d.u.r
-00002650: 957c 016a 1972 857c 016a 186a 1a64 0d69  .|.j.r.|.j.j.d.i
-00002660: 007c 016a 19a4 018e 017d 047c 00a0 1b7c  .|.j.....}.|...|
-00002670: 04a1 017d 036e 087c 00a0 1c64 037c 016a  ...}.n.|...d.|.j
-00002680: 1869 00a1 037d 037c 00a0 177c 017c 037c  .i...}.|...|.|.|
-00002690: 016a 1da1 0353 007c 016a 1e64 0375 0172  .j...S.|.j.d.u.r
-000026a0: a764 067c 016a 1e16 007d 037c 00a0 177c  .d.|.j...}.|...|
-000026b0: 017c 037c 016a 1da1 0353 007c 016a 1f64  .|.|.j...S.|.j.d
-000026c0: 0375 0172 b07c 016a 1f7d 056e 037c 016a  .u.r.|.j.}.n.|.j
-000026d0: 1353 007c 016a 106a 1064 0375 0072 c574  .S.|.j.j.d.u.r.t
-000026e0: 1264 077c 016a 1374 0364 087c 0516 0083  .d.|.j.t.d.|....
-000026f0: 0164 098d 0353 0074 127c 016a 137c 0564  .d...S.t.|.j.|.d
-00002700: 0a8d 0253 0074 047c 0174 0383 0272 dc74  ...S.t.|.t...r.t
-00002710: 207c 0064 0b64 0c83 0372 dc74 0e7c 016a   |.d.d...r.t.|.j
-00002720: 2183 0153 007c 0153 0029 0e7a 540a 2020  !..S.|.S.).zT.  
-00002730: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
-00002740: 2063 6f6e 7665 7274 696e 6720 6c6f 6769   converting logi
-00002750: 6320 666f 7220 7365 7269 616c 697a 696e  c for serializin
-00002760: 6720 5079 7468 6f6e 2076 616c 7565 7320  g Python values 
-00002770: 746f 206a 736f 6e2e 0a20 2020 2020 2020  to json..       
-00002780: 20da 104c 414e 4755 4147 455f 4348 4f49   ..LANGUAGE_CHOI
-00002790: 4345 537a 0b32 3032 3130 3531 3720 7b7d  CESz.20210517 {}
-000027a0: 4e29 0172 6800 0000 2902 7245 0000 0072  N).rh...).rE...r
-000027b0: 5600 0000 7a02 2573 da06 6275 7474 6f6e  V...z.%s..button
-000027c0: 7a23 6675 6e63 7469 6f6e 2829 207b 204c  z#function() { L
-000027d0: 696e 6f2e 6c6f 6164 5f75 726c 2827 2573  ino.load_url('%s
-000027e0: 2729 3b20 7d29 03da 0578 7479 7065 7245  '); })...xtyperE
-000027f0: 0000 00da 0768 616e 646c 6572 2902 7245  .....handler).rE
-00002800: 0000 00da 0468 7265 6672 6e00 0000 4672  .....hrefrn...Fr
-00002810: 3700 0000 2922 7204 0000 0072 6f00 0000  7...)"r....ro...
-00002820: 72f4 0000 0072 2700 0000 72a1 0000 0072  r....r'...r....r
-00002830: 1c00 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
-00002840: d400 0000 720d 0000 00da 0643 686f 6963  ....r......Choic
-00002850: 6572 4400 0000 7205 0000 00da 054d 6f64  erD...r......Mod
-00002860: 656c 72da 0000 0072 4600 0000 720a 0000  elr....rF...r...
-00002870: 00da 0670 6172 656e 7472 6800 0000 7271  ...parentrh...rq
-00002880: 0000 0072 9600 0000 720b 0000 00da 0869  ...r....r......i
-00002890: 6e73 7461 6e63 65da 1069 6e73 7461 6e63  nstance..instanc
-000028a0: 655f 6861 6e64 6c65 72da 0c68 616e 646c  e_handler..handl
-000028b0: 6572 5f69 7465 6d72 a400 0000 72f2 0000  er_itemr....r...
-000028c0: 0072 de00 0000 da0f 7265 7175 6573 745f  .r......request_
-000028d0: 6861 6e64 6c65 72da 0b61 6374 696f 6e5f  handler..action_
-000028e0: 6361 6c6c 72b4 0000 00da 0a6a 6176 6173  callr......javas
-000028f0: 6372 6970 7472 f800 0000 da07 6765 7461  criptr......geta
-00002900: 7474 72da 0173 2906 7240 0000 0072 a600  ttr..s).r@...r..
-00002910: 0000 da01 68da 026a 7372 cb00 0000 da03  ....h..jsr......
-00002920: 7572 6c72 3700 0000 7237 0000 0072 3800  urlr7...r7...r8.
-00002930: 0000 723f 0000 0056 0100 0073 5400 0000  ..r?...V...sT...
-00002940: 0c04 0801 0a01 0e01 0c01 0201 0603 0c01  ................
-00002950: 0601 0a01 0801 0a01 0a01 0601 1603 0a02  ................
-00002960: 0a01 1001 0c01 0801 0e01 0a01 0601 1401  ................
-00002970: 0c01 1002 1001 0a02 0a01 1001 0a01 0801  ................
-00002980: 0607 0c02 0202 0601 0a02 06fd 0e04 1602  ................
-00002990: 0a02 0402 7a18 5265 6e64 6572 6572 2e70  ....z.Renderer.p
-000029a0: 7932 6a73 5f63 6f6e 7665 7274 6572 6304  y2js_converterc.
-000029b0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-000029c0: 0000 0043 0000 0073 5000 0000 7400 7c01  ...C...sP...t.|.
-000029d0: 6a01 7c02 6401 8d02 7d04 7c01 6a02 721a  j.|.d...}.|.j.r.
-000029e0: 7c01 6a02 6a03 6a04 721a 7c04 6a05 6402  |.j.j.j.r.|.j.d.
-000029f0: 7c01 6a02 6a03 6a04 1700 6403 8d01 0100  |.j.j.j...d.....
-00002a00: 7406 6a07 6a08 7226 7c03 7226 7c04 6a05  t.j.j.r&|.r&|.j.
-00002a10: 7c03 6404 8d01 0100 7c04 5300 2905 da00  |.d.....|.S.)...
-00002a20: 2902 7245 0000 0072 f700 0000 7a07 782d  ).rE...r....z.x-
-00002a30: 7462 6172 2d29 01da 0769 636f 6e43 6c73  tbar-)...iconCls
-00002a40: 2901 da07 746f 6f6c 5469 7029 0972 7100  )...toolTip).rq.
-00002a50: 0000 7296 0000 0072 a400 0000 726c 0000  ..r....r....rl..
-00002a60: 0072 e600 0000 7277 0000 0072 0400 0000  .r....rw...r....
-00002a70: 726f 0000 00da 0d75 7365 5f71 7569 636b  ro.....use_quick
-00002a80: 7469 7073 2905 7240 0000 00da 026d 6972  tips).r@.....mir
-00002a90: f700 0000 72b4 0000 00da 0164 7237 0000  ....r......dr7..
-00002aa0: 0072 3700 0000 7238 0000 0072 ff00 0000  .r7...r8...r....
-00002ab0: a401 0000 730c 0000 000e 0410 0116 010c  ....s...........
-00002ac0: 010c 0304 017a 1552 656e 6465 7265 722e  .....z.Renderer.
-00002ad0: 6861 6e64 6c65 725f 6974 656d 6302 0000  handler_itemc...
-00002ae0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-00002af0: 004f 0000 0073 2000 0000 7c01 6a00 6402  .O...s ...|.j.d.
-00002b00: 6900 7c03 a401 8e01 7d04 7c00 a001 7c01  i.|.....}.|...|.
-00002b10: 7c01 6a02 7c04 a103 5300 2903 7a36 2047  |.j.|...S.).z6 G
-00002b20: 656e 6572 6174 6573 206a 7320 7374 7269  enerates js stri
-00002b30: 6e67 2066 6f72 2061 6374 696f 6e20 6275  ng for action bu
-00002b40: 7474 6f6e 2063 616c 6c73 2e0a 2020 2020  tton calls..    
-00002b50: 2020 2020 4e72 3700 0000 2903 72c0 0000      Nr7...).r...
-00002b60: 0072 0101 0000 72a4 0000 0029 0572 4000  .r....r....).r@.
-00002b70: 0000 72cb 0000 0072 cc00 0000 72cd 0000  ..r....r....r...
-00002b80: 0072 ce00 0000 7237 0000 0072 3700 0000  .r....r7...r7...
-00002b90: 7238 0000 0072 0001 0000 b201 0000 7304  r8...r........s.
-00002ba0: 0000 0010 0410 017a 1852 656e 6465 7265  .......z.Rendere
-00002bb0: 722e 7265 7175 6573 745f 6861 6e64 6c65  r.request_handle
-00002bc0: 7263 0400 0000 0000 0000 0000 0000 0800  rc..............
-00002bd0: 0000 0800 0000 4300 0000 739c 0000 007c  ......C...s....|
-00002be0: 026a 007d 047c 02a0 01a1 00a0 0264 0164  .j.}.|.......d.d
-00002bf0: 02a1 025c 027d 057d 067c 0373 1169 007d  ...\.}.}.|.s.i.}
-00002c00: 037c 0164 0075 0172 2274 037c 0164 0383  .|.d.u.r"t.|.d..
-00002c10: 0272 227c 016a 0464 0869 007c 03a4 018e  .r"|.j.d.i.|....
-00002c20: 017d 037c 0172 2d7c 016a 0572 2d7c 016a  .}.|.r-|.j.r-|.j
-00002c30: 057c 0374 066a 073c 007c 0664 046b 0272  .|.t.j.<.|.d.k.r
-00002c40: 3974 037c 0364 0583 0272 397c 0364 053d  9t.|.d...r9|.d.=
-00002c50: 007c 0164 0075 0072 3f64 006e 027c 016a  .|.d.u.r?d.n.|.j
-00002c60: 087d 0764 0674 0974 0a7c 067c 057c 037c  .}.d.t.t.|.|.|.|
-00002c70: 0764 078d 0483 0116 0053 0029 094e da01  .d.......S.).N..
-00002c80: 2e72 2d00 0000 72c0 0000 00da 0467 7269  .r-...r......gri
-00002c90: 6472 d100 0000 72ed 0000 0029 0472 9500  dr....r....).r..
-00002ca0: 0000 72eb 0000 0072 e200 0000 72e9 0000  ..r....r....r...
-00002cb0: 0072 3700 0000 290b 726c 0000 00da 0966  .r7...).rl.....f
-00002cc0: 756c 6c5f 6e61 6d65 da06 7273 706c 6974  ull_name..rsplit
-00002cd0: 7283 0000 0072 c000 0000 da0a 7375 6273  r....r......subs
-00002ce0: 745f 7573 6572 720c 0000 00da 1455 524c  t_userr......URL
-00002cf0: 5f50 4152 414d 5f53 5542 5354 5f55 5345  _PARAM_SUBST_USE
-00002d00: 5272 ee00 0000 7226 0000 0072 7100 0000  Rr....r&...rq...
-00002d10: 2908 7240 0000 0072 cb00 0000 72a4 0000  ).r@...r....r...
-00002d20: 0072 e200 0000 7250 0000 0072 eb00 0000  .r....rP...r....
-00002d30: 7295 0000 0072 e900 0000 7237 0000 0072  r....r....r7...r
-00002d40: 3700 0000 7238 0000 0072 0101 0000 bc01  7...r8...r......
-00002d50: 0000 7322 0000 0006 0214 0204 0204 0112  ..s"............
-00002d60: 0210 010a 020c 0112 1106 0112 0206 0202  ................
-00002d70: 0102 0102 0102 010a fc7a 1452 656e 6465  .........z.Rende
-00002d80: 7265 722e 6163 7469 6f6e 5f63 616c 6c63  rer.action_callc
-00002d90: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002da0: 0400 0000 4300 0000 732e 0000 007c 0173  ....C...s....|.s
-00002db0: 0464 0053 0074 007c 0174 0183 0273 0d74  .d.S.t.|.t...s.t
-00002dc0: 017c 0183 017d 0174 027c 0164 0164 028d  .|...}.t.|.d.d..
-00002dd0: 027d 0164 037c 0117 0053 0029 044e 4629  .}.d.|...S.).NF)
-00002de0: 01da 0571 756f 7465 7a0b 6a61 7661 7363  ...quotez.javasc
-00002df0: 7269 7074 3a29 0372 a100 0000 7246 0000  ript:).r....rF..
-00002e00: 0072 0300 0000 2902 7240 0000 0072 0601  .r....).r@...r..
-00002e10: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-00002e20: 00da 066a 7332 7572 6ce6 0100 0073 0c00  ...js2url....s..
-00002e30: 0000 0401 0401 0a02 0801 0c01 0801 7a0f  ..............z.
-00002e40: 5265 6e64 6572 6572 2e6a 7332 7572 6c63  Renderer.js2urlc
-00002e50: 0600 0000 0000 0000 0000 0000 0700 0000  ................
-00002e60: 0400 0000 4300 0000 7356 0000 0074 006a  ....C...sV...t.j
-00002e70: 016a 0272 2774 006a 016a 0372 0f64 017c  .j.r't.j.j.r.d.|
-00002e80: 047c 0566 0216 007d 066e 0264 027d 067c  .|.f...}.n.d.}.|
-00002e90: 0272 1974 0464 037c 067c 0283 037d 067c  .r.t.d.|.|...}.|
-00002ea0: 0672 297c 016a 0564 047c 037c 0666 0216  .r)|.j.d.|.|.f..
-00002eb0: 0064 058d 0101 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
-00002ec0: 0053 0029 064e 7a08 2825 732e 2573 2920  .S.).Nz.(%s.%s) 
-00002ed0: 7208 0100 007a 047b 7d7b 7d7a 0728 2573  r....z.{}{}z.(%s
-00002ee0: 2c25 7329 2901 da08 7175 6963 6b74 6970  ,%s))...quicktip
-00002ef0: 2906 7204 0000 0072 6f00 0000 720b 0100  ).r....ro...r...
-00002f00: 00da 1973 686f 775f 696e 7465 726e 616c  ...show_internal
-00002f10: 5f66 6965 6c64 5f6e 616d 6573 7206 0000  _field_namesr...
-00002f20: 0072 7700 0000 2907 7240 0000 0072 cd00  .rw...).r@...r..
-00002f30: 0000 72b4 0000 0072 7400 0000 da0a 6461  ..r....rt.....da
-00002f40: 7461 736f 7572 6365 da09 6669 656c 646e  tasource..fieldn
-00002f50: 616d 65da 0374 7474 7237 0000 0072 3700  ame..tttr7...r7.
-00002f60: 0000 7238 0000 00da 0d61 6464 5f68 656c  ..r8.....add_hel
-00002f70: 705f 7465 7874 ef01 0000 7318 0000 0008  p_text....s.....
-00002f80: 0108 010e 0104 0204 010c 0104 0108 0402  ................
-00002f90: 010e ff04 f504 077a 1652 656e 6465 7265  .......z.Rendere
-00002fa0: 722e 6164 645f 6865 6c70 5f74 6578 7463  r.add_help_textc
-00002fb0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00002fc0: 0300 0000 4300 0000 7356 0000 0074 0083  ....C...sV...t..
-00002fd0: 007d 0264 017c 0117 0064 0217 007d 037c  .}.d.|...d...}.|
-00002fe0: 006a 01a0 0264 03a1 0164 0419 007d 047c  .j...d...d...}.|
-00002ff0: 0264 0575 0172 1c7c 037c 026a 0364 0217  .d.u.r.|.|.j.d..
-00003000: 0037 007d 037c 0374 04a0 05a1 0064 0317  .7.}.|.t.....d..
-00003010: 007c 0417 0037 007d 0364 067c 047c 0366  .|...7.}.d.|.|.f
-00003020: 0353 0029 077a 2c4c 696b 6520 6c69 6e6f  .S.).z,Like lino
-00003030: 5f6a 735f 7061 7274 732c 2062 7574 2066  _js_parts, but f
-00003040: 6f72 2061 6374 6f72 5f6c 6576 656c 2064  or actor_level d
-00003050: 6174 61da 054c 696e 6f5f da01 5f72 0e01  ata..Lino_.._r..
-00003060: 0000 722f 0000 004e da05 6361 6368 6529  ..r/...N..cache)
-00003070: 0672 2900 0000 da11 6c69 6e6f 5f77 6562  .r).....lino_web
-00003080: 5f74 656d 706c 6174 6572 1101 0000 7244  _templater....rD
-00003090: 0000 0072 0700 0000 da0c 6765 745f 6c61  ...r......get_la
-000030a0: 6e67 7561 6765 2905 7240 0000 0072 eb00  nguage).r@...r..
-000030b0: 0000 da09 7573 6572 5f74 7970 65da 0866  ....user_type..f
-000030c0: 696c 656e 616d 65da 0966 696c 655f 7479  ilename..file_ty
-000030d0: 7065 7237 0000 0072 3700 0000 7238 0000  per7...r7...r8..
-000030e0: 00da 156c 696e 6f5f 6a73 5f70 6172 7473  ...lino_js_parts
-000030f0: 5f63 6875 6e6b 6564 fe01 0000 730e 0000  _chunked....s...
-00003100: 0006 020c 0110 0108 010e 0114 010a 017a  ...............z
-00003110: 1e52 656e 6465 7265 722e 6c69 6e6f 5f6a  .Renderer.lino_j
-00003120: 735f 7061 7274 735f 6368 756e 6b65 6463  s_parts_chunkedc
-00003130: 0200 0000 0000 0000 0000 0000 1100 0000  ................
-00003140: 0600 0000 4300 0000 73de 0100 0067 007d  ....C...s....g.}
-00003150: 0267 007d 037c 0144 005d e47d 047c 04a0  .g.}.|.D.].}.|..
-00003160: 00a1 007d 057c 0573 127c 046a 016a 0272  ...}.|.s.|.j.j.r
-00003170: cc74 036a 047c 046a 016a 0569 017d 067c  .t.j.|.j.j.i.}.|
-00003180: 0572 237c 066a 067c 056a 076a 0864 018d  .r#|.j.|.j.j.d..
-00003190: 0101 007c 046a 016a 0272 c767 007d 0774  ...|.j.j.r.g.}.t
-000031a0: 0983 007d 087c 046a 0aa0 0b7c 046a 0174  ...}.|.j...|.j.t
-000031b0: 0c83 00a1 0244 005d 727d 0974 097c 096a  .....D.]r}.t.|.j
-000031c0: 016a 0564 028d 017d 0a7c 096a 016a 0d7d  .j.d...}.|.j.j.}
-000031d0: 0b7c 0b72 487c 0b7c 0a64 033c 007c 096a  .|.rH|.|.d.<.|.j
-000031e0: 016a 0e7d 0c7c 0c72 5e74 0f7c 0c83 0172  .j.}.|.r^t.|...r
-000031f0: 5a7c 0c7c 096a 0a83 017c 0a64 043c 006e  Z|.|.j...|.d.<.n
-00003200: 047c 0c7c 0a64 043c 007c 096a 016a 1064  .|.|.d.<.|.j.j.d
-00003210: 0575 0172 847c 096a 016a 107d 0d7c 0d7c  .u.r.|.j.j.}.|.|
-00003220: 0876 0072 747c 087c 0d19 00a0 117c 0aa1  .v.rt|.|.....|..
-00003230: 0101 006e 1574 097c 0d64 068d 017d 0e7c  ...n.t.|.d...}.|
-00003240: 0a67 017c 087c 0d3c 007c 07a0 117c 0ea1  .g.|.|.<.|...|..
-00003250: 0101 006e 057c 07a0 117c 0aa1 0101 007c  ...n.|...|.....|
-00003260: 096a 016a 1272 a774 137c 096a 016a 1283  .j.j.r.t.|.j.j..
-00003270: 017d 0f74 147c 0f64 0783 0273 9e7c 096a  .}.t.|.d...s.|.j
-00003280: 016a 057c 0f64 073c 007c 0f7c 0376 0172  .j.|.d.<.|.|.v.r
-00003290: a77c 03a0 117c 0fa1 0101 0071 357c 0872  .|...|.....q5|.r
-000032a0: c374 157c 0783 0144 005d 145c 027d 107d  .t.|...D.].\.}.}
-000032b0: 0a7c 0aa0 1664 0864 09a1 0272 c27c 087c  .|...d.d...r.|.|
-000032c0: 0a64 0819 0019 007c 077c 1019 0064 0a3c  .d.....|.|...d.<
-000032d0: 0071 ae7c 077c 0664 0b3c 007c 02a0 117c  .q.|.|.d.<.|...|
-000032e0: 06a1 0101 007c 046a 016a 1272 ea74 137c  .....|.j.j.r.t.|
-000032f0: 046a 016a 1283 017d 0f74 147c 0f64 0783  .j.j...}.t.|.d..
-00003300: 0273 e17c 046a 016a 057c 0f64 073c 007c  .s.|.j.j.|.d.<.|
-00003310: 0f7c 0376 0172 ea7c 03a0 117c 0fa1 0101  .|.v.r.|...|....
-00003320: 0071 067c 027c 0366 0253 0029 0c7a 4543  .q.|.|.f.S.).zEC
-00003330: 6f6e 7665 7274 7320 6f66 2061 6c6c 2074  onverts of all t
-00003340: 6865 2062 6f75 6e64 6163 7469 6f6e 7320  he boundactions 
-00003350: 6f66 2061 6e20 6163 746f 7220 746f 206a  of an actor to j
-00003360: 736f 6e20 666f 726d 6174 2e0a 2020 2020  son format..    
-00003370: 2020 2020 a901 7265 0000 0029 0172 9500      ..re...).r..
-00003380: 0000 72b4 0000 00da 0a6a 735f 6861 6e64  ..r......js_hand
-00003390: 6c65 724e 2901 da05 636f 6d62 6f72 9000  lerN)...combor..
-000033a0: 0000 7227 0100 0046 7256 0000 00da 0e74  ..r'...FrV.....t
-000033b0: 6f6f 6c62 6172 4163 7469 6f6e 7329 17da  oolbarActions)..
-000033c0: 1167 6574 5f6c 6179 6f75 745f 6861 6e64  .get_layout_hand
-000033d0: 656c 726c 0000 00da 0b77 696e 646f 775f  elrl.....window_
-000033e0: 7479 7065 720c 0000 00da 1555 524c 5f50  typer......URL_P
-000033f0: 4152 414d 5f41 4354 494f 4e5f 4e41 4d45  ARAM_ACTION_NAME
-00003400: 724e 0000 0072 7700 0000 72ac 0000 0072  rN...rw...r....r
-00003410: 8800 0000 7271 0000 0072 9900 0000 da13  ....rq...r......
-00003420: 6765 745f 746f 6f6c 6261 725f 6163 7469  get_toolbar_acti
-00003430: 6f6e 7372 2900 0000 72b4 0000 0072 2601  onsr)...r....r&.
-00003440: 0000 7230 0000 00da 0b63 6f6d 626f 5f67  ..r0.....combo_g
-00003450: 726f 7570 da06 6170 7065 6e64 da06 686f  roup..append..ho
-00003460: 746b 6579 da04 7661 7273 7283 0000 0072  tkey..varsr....r
-00003470: 3100 0000 72e7 0000 0029 1172 4000 0000  1...r....).r@...
-00003480: da0c 6163 7469 6f6e 735f 6c69 7374 72a7  ..actions_listr.
-00003490: 0000 00da 0768 6f74 6b65 7973 7290 0000  .....hotkeysr...
-000034a0: 00da 026c 68da 1161 6374 696f 6e5f 6465  ...lh..action_de
-000034b0: 7363 7269 7074 6f72 da04 7462 6173 da09  scriptor..tbas..
-000034c0: 636f 6d62 6f5f 6d61 7072 5000 0000 da03  combo_maprP.....
-000034d0: 7462 6172 b400 0000 7226 0100 0072 2d01  tbar....r&...r-.
-000034e0: 0000 7227 0100 0072 2f01 0000 7235 0000  ..r'...r/...r5..
-000034f0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
-00003500: da0c 6163 7469 6f6e 7332 6a73 6f6e 0802  ..actions2json..
-00003510: 0000 7368 0000 0004 0404 0108 0208 010c  ..sh............
-00003520: 010e 0204 0110 0108 0104 0106 0106 0208  ................
-00003530: 0108 ff0e 0308 010c 0108 0104 0108 0110  ................
-00003540: 0108 020c 0208 0108 0210 010a 020a 010c  ................
-00003550: 010a 0208 020c 010a 010c 0108 010a 0102  ................
-00003560: 8004 0210 010c 0114 0102 8008 020a 0208  ................
-00003570: 020c 010a 010c 0108 010a 0102 8008 027a  ...............z
-00003580: 1552 656e 6465 7265 722e 6163 7469 6f6e  .Renderer.action
-00003590: 7332 6a73 6f6e 6302 0000 0000 0000 0000  s2jsonc.........
-000035a0: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-000035b0: 5800 0000 6700 7d02 6400 7d03 7c01 4400  X...g.}.d.}.|.D.
-000035c0: 5d14 7d04 7c04 6401 1900 6400 7500 7213  ].}.|.d...d.u.r.
-000035d0: 7c04 6402 1900 7d03 7106 7c02 a000 7401  |.d...}.q.|...t.
-000035e0: 7c04 8301 a101 0100 7106 7402 7c02 6403  |.......q.t.|.d.
-000035f0: 6404 8400 6405 8d02 7d02 7c02 a000 6400  d...d...}.|...d.
-00003600: 7c03 6702 a101 0100 7c02 5300 2906 4e72  |.g.....|.S.).Nr
-00003610: 0100 0000 722d 0000 0063 0100 0000 0000  ....r-...c......
-00003620: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
-00003630: 0000 7308 0000 007c 0064 0119 0053 0029  ..s....|.d...S.)
-00003640: 024e 7201 0000 0072 3700 0000 2901 7236  .Nr....r7...).r6
-00003650: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-00003660: 0000 da08 3c6c 616d 6264 613e 5402 0000  ....<lambda>T...
-00003670: 7302 0000 0008 007a 2c52 656e 6465 7265  s......z,Rendere
-00003680: 722e 6469 7370 6c61 795f 6d6f 6465 326a  r.display_mode2j
-00003690: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c61  son.<locals>.<la
-000036a0: 6d62 6461 3ea9 0172 3400 0000 2903 722e  mbda>..r4...).r.
-000036b0: 0100 0072 7800 0000 da06 736f 7274 6564  ...rx.....sorted
-000036c0: 2905 7240 0000 00da 0c64 6973 706c 6179  ).r@.....display
-000036d0: 5f6d 6f64 65da 0364 6d73 da03 646d 6472  _mode..dms..dmdr
-000036e0: 9300 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
-000036f0: 0000 00da 1164 6973 706c 6179 5f6d 6f64  .....display_mod
-00003700: 6532 6a73 6f6e 4c02 0000 7312 0000 0004  e2jsonL...s.....
-00003710: 0104 0108 010c 010a 0110 0210 010e 0104  ................
-00003720: 017a 1a52 656e 6465 7265 722e 6469 7370  .z.Renderer.disp
-00003730: 6c61 795f 6d6f 6465 326a 736f 6e63 0200  lay_mode2jsonc..
-00003740: 0000 0000 0000 0000 0000 1100 0000 0800  ................
-00003750: 0000 4300 0000 7322 0300 0074 007c 0183  ..C...s"...t.|..
-00003760: 0172 0974 017c 0174 0283 0273 0b4a 0082  .r.t.|.t...s.J..
-00003770: 017c 00a0 037c 016a 04a1 015c 027d 027d  .|...|.j...\.}.}
-00003780: 0374 057c 016a 067c 027c 01a0 07a1 0074  .t.|.j.|.|.....t
-00003790: 087c 016a 0983 017c 01a0 0a74 0b83 00a1  .|.j...|...t....
-000037a0: 010c 0064 018d 057d 0474 0c7c 0383 0172  ...d...}.t.|...r
-000037b0: 317c 046a 0d7c 0364 028d 0101 007c 01a0  1|.j.|.d.....|..
-000037c0: 0ea1 007d 057c 056a 0f64 0075 0072 4374  ...}.|.j.d.u.rCt
-000037d0: 106a 116a 12a0 1364 037c 01a1 0201 006e  .j.j...d.|.....n
-000037e0: 5d74 147c 0564 0483 0272 9767 007d 0664  ]t.|.d...r.g.}.d
-000037f0: 057d 077c 05a0 15a1 007d 087c 0844 005d  .}.|.....}.|.D.]
-00003800: 407d 097c 00a0 167c 09a1 017d 0a7c 0a6a  @}.|...|...}.|.j
-00003810: 0d74 177c 056a 0f6a 187c 096a 196a 1a64  .t.|.j.j.|.j.j.d
-00003820: 0664 0784 0064 088d 037c 0717 0064 098d  .d...d...|...d..
-00003830: 0101 0074 1b7c 0974 1c83 0272 8474 1b7c  ...t.|.t...r.t.|
-00003840: 0974 1d83 0273 847c 0a6a 0d7c 0a64 0a19  .t...s.|.j.|.d..
-00003850: 0064 0b17 0064 0c8d 0101 007c 0764 0b37  .d...d.....|.d.7
-00003860: 007d 0774 1b7c 0974 1e83 0272 8d7c 0764  .}.t.|.t...r.|.d
-00003870: 0d37 007d 077c 06a0 1f7c 0aa1 0101 0071  .7.}.|...|.....q
-00003880: 527c 067c 0464 0e3c 007c 04a0 0d74 207c  R|.|.d.<.|...t |
-00003890: 056a 0f64 0f83 02a1 0101 007c 04a0 0d74  .j.d.......|...t
-000038a0: 207c 0164 1083 02a1 0101 0074 147c 016a   |.d.......t.|.j
-000038b0: 2164 1183 0272 b47c 046a 0d64 1264 138d  !d...r.|.j.d.d..
-000038c0: 0101 0074 007c 016a 2183 0172 c574 017c  ...t.|.j!..r.t.|
-000038d0: 016a 2174 2283 0272 c57c 046a 0d64 1264  .j!t"..r.|.j.d.d
-000038e0: 148d 0101 007c 016a 2364 0075 0172 d27c  .....|.j#d.u.r.|
-000038f0: 00a0 247c 016a 23a1 017c 0464 153c 007c  ..$|.j#..|.d.<.|
-00003900: 016a 2564 0075 0172 e77c 016a 25a0 26a1  .j%d.u.r.|.j%.&.
-00003910: 007d 0b7c 0b64 0075 0172 e77c 046a 0d7c  .}.|.d.u.r.|.j.|
-00003920: 0b6a 2764 168d 0101 007c 016a 2872 f37c  .j'd.....|.j(r.|
-00003930: 046a 0d74 297c 016a 2883 0164 178d 0101  .j.t)|.j(..d....
-00003940: 0074 2a7c 0164 1864 0083 037d 0c7c 0c64  .t*|.d.d...}.|.d
-00003950: 0075 0190 0172 057c 046a 0d7c 0c6a 2764  .u...r.|.j.|.j'd
-00003960: 198d 0101 0074 2a7c 0164 1a64 0083 037d  .....t*|.d.d...}
-00003970: 0d7c 0d64 0075 0190 0172 177c 046a 0d7c  .|.d.u...r.|.j.|
-00003980: 0d6a 2764 1b8d 0101 0074 2a7c 016a 2164  .j'd.....t*|.j!d
-00003990: 1c69 0083 037d 0e7c 0e90 0172 2e7c 046a  .i...}.|...r.|.j
-000039a0: 0d64 1d64 1e84 007c 0ea0 2ba1 0044 0083  .d.d...|..+..D..
-000039b0: 0164 1f8d 0101 0074 106a 11a0 2c64 20a1  .d.....t.j..,d .
-000039c0: 0190 0172 5174 2a7c 0164 2164 0083 0364  ...rQt*|.d!d...d
-000039d0: 0075 0190 0172 5174 147c 016a 2164 2283  .u...rQt.|.j!d".
-000039e0: 0290 0172 517c 046a 0d74 2d6a 2ea0 2f7c  ...rQ|.j.t-j../|
-000039f0: 016a 21a1 016a 3064 238d 0101 0064 2444  .j!..j0d#....d$D
-00003a00: 005d 177d 0f74 2a7c 017c 0f64 0083 037d  .].}.t*|.|.d...}
-00003a10: 107c 1064 0075 0190 0172 697c 04a0 0d7c  .|.d.u...ri|...|
-00003a20: 0f7c 106a 316a 3269 01a1 0101 0090 0171  .|.j1j2i.......q
-00003a30: 537c 016a 3364 0075 0190 0172 8f7c 046a  S|.j3d.u...r.|.j
-00003a40: 0d7c 016a 336a 2764 2564 2684 007c 016a  .|.j3j'd%d&..|.j
-00003a50: 336a 346a 3544 0083 0164 278d 0201 0074  3j4j5D...d'....t
-00003a60: 147c 0164 2883 0290 0172 8f7c 046a 0d7c  .|.d(....r.|.j.|
-00003a70: 016a 3664 298d 0101 007c 0453 0029 2a4e  .j6d)....|.S.)*N
-00003a80: 2905 da02 6964 7231 0100 0072 9600 0000  )...idr1...r....
-00003a90: da05 736c 6176 65da 0865 6469 7461 626c  ..slave..editabl
-00003aa0: 6529 0172 3201 0000 7a0f 2573 2068 6173  e).r2...z.%s has
-00003ab0: 206e 6f20 7374 6f72 65da 0b67 6574 5f63   no store..get_c
-00003ac0: 6f6c 756d 6e73 7201 0000 0063 0100 0000  olumnsr....c....
-00003ad0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00003ae0: 5300 0000 7306 0000 007c 006a 0053 0072  S...s....|.j.S.r
-00003af0: 3b00 0000 a901 7253 0000 00a9 0172 8d00  ;.....rS.....r..
-00003b00: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-00003b10: 0072 3901 0000 7102 0000 7302 0000 0006  .r9...q...s.....
-00003b20: 007a 2552 656e 6465 7265 722e 6163 746f  .z%Renderer.acto
-00003b30: 7232 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  r2json.<locals>.
-00003b40: 3c6c 616d 6264 613e 723a 0100 0029 01da  <lambda>r:...)..
-00003b50: 0c66 6965 6c64 735f 696e 6465 7872 4601  .fields_indexrF.
-00003b60: 0000 722d 0000 0029 01da 1366 6965 6c64  ..r-...)...field
-00003b70: 735f 696e 6465 785f 6869 6464 656e e902  s_index_hidden..
-00003b80: 0000 00da 0363 6f6c da08 706b 5f69 6e64  .....col..pk_ind
-00003b90: 6578 7ad0 7072 6576 6965 775f 6c69 6d69  exz.preview_limi
-00003ba0: 7420 7573 655f 6465 7461 696c 5f70 6172  t use_detail_par
-00003bb0: 616d 5f70 616e 656c 2075 7365 5f64 6574  am_panel use_det
-00003bc0: 6169 6c5f 7061 7261 6d73 5f76 616c 7565  ail_params_value
-00003bd0: 2068 6964 655f 6e61 7669 6761 746f 7220   hide_navigator 
-00003be0: 7573 655f 6465 7461 696c 5f70 6172 616d  use_detail_param
-00003bf0: 735f 7661 6c75 6520 7265 6163 745f 7265  s_value react_re
-00003c00: 7370 6f6e 7369 7665 206d 6178 5f72 656e  sponsive max_ren
-00003c10: 6465 725f 6465 7074 6820 7369 6d70 6c65  der_depth simple
-00003c20: 5f73 6c61 7665 6772 6964 5f68 6561 6465  _slavegrid_heade
-00003c30: 7220 7061 6769 6e61 746f 725f 7465 6d70  r paginator_temp
-00003c40: 6c61 7465 2068 6964 655f 746f 705f 746f  late hide_top_to
-00003c50: 6f6c 6261 7220 6869 6465 5f69 665f 656d  olbar hide_if_em
-00003c60: 7074 7920 da04 6669 6c65 5429 01da 0d63  pty ..fileT)...c
-00003c70: 6f6e 7461 696e 5f6d 6564 6961 2901 da09  ontain_media)...
-00003c80: 6564 6974 5f73 6166 6572 3c01 0000 7225  edit_safer<...r%
-00003c90: 0100 0029 01da 0d61 6374 6976 655f 6669  ...)...active_fi
-00003ca0: 656c 6473 da0b 6361 7264 5f6c 6179 6f75  elds..card_layou
-00003cb0: 7429 0172 4f01 0000 da0b 6c69 7374 5f6c  t).rO.....list_l
-00003cc0: 6179 6f75 7429 0172 5001 0000 da0e 5f63  ayout).rP....._c
-00003cd0: 686f 6f73 6572 735f 6469 6374 6301 0000  hoosers_dictc...
-00003ce0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-00003cf0: 0053 0000 0073 2200 0000 6900 7c00 5d0d  .S...s"...i.|.].
-00003d00: 5c02 7d01 7d02 7c01 6400 6401 8400 7c02  \.}.}.|.d.d...|.
-00003d10: 6a00 4400 8301 9302 7102 5300 2902 6301  j.D.....q.S.).c.
-00003d20: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00003d30: 0000 0053 0000 00f3 1200 0000 6700 7c00  ...S........g.|.
-00003d40: 5d05 7d01 7c01 6a00 9102 7102 5300 7237  ].}.|.j...q.S.r7
-00003d50: 0000 0072 4401 0000 2902 7247 0000 00da  ...rD...).rG....
-00003d60: 0263 6672 3700 0000 7237 0000 0072 3800  .cfr7...r7...r8.
-00003d70: 0000 7249 0000 00aa 0200 00f3 0200 0000  ..rI............
-00003d80: 1200 7a32 5265 6e64 6572 6572 2e61 6374  ..z2Renderer.act
-00003d90: 6f72 326a 736f 6e2e 3c6c 6f63 616c 733e  or2json.<locals>
-00003da0: 2e3c 6469 6374 636f 6d70 3e2e 3c6c 6973  .<dictcomp>.<lis
-00003db0: 7463 6f6d 703e 2901 da0e 636f 6e74 6578  tcomp>)...contex
-00003dc0: 745f 6669 656c 6473 2903 7247 0000 00da  t_fields).rG....
-00003dd0: 0266 6e72 4800 0000 7237 0000 0072 3700  .fnrH...r7...r7.
-00003de0: 0000 7238 0000 0072 4d00 0000 aa02 0000  ..r8...rM.......
-00003df0: 7306 0000 0006 0006 0116 ff7a 2752 656e  s..........z'Ren
-00003e00: 6465 7265 722e 6163 746f 7232 6a73 6f6e  derer.actor2json
-00003e10: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00003e20: 6f6d 703e 2901 da0c 6368 6f6f 7365 725f  omp>)...chooser_
-00003e30: 6469 6374 da0c 636f 6e74 656e 7474 7970  dict..contenttyp
-00003e40: 6573 da05 6d6f 6465 6cda 055f 6d65 7461  es..model.._meta
-00003e50: 2901 da0c 636f 6e74 656e 745f 7479 7065  )...content_type
-00003e60: 2903 da0d 6465 7461 696c 5f61 6374 696f  )...detail_actio
-00003e70: 6eda 0d69 6e73 6572 745f 6163 7469 6f6e  n..insert_action
-00003e80: da0e 6465 6661 756c 745f 6163 7469 6f6e  ..default_action
-00003e90: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00003ea0: 0003 0000 0053 0000 0072 5201 0000 7237  .....S...rR...r7
-00003eb0: 0000 0072 4401 0000 2902 7247 0000 0072  ...rD...).rG...r
-00003ec0: 8d00 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
-00003ed0: 0000 0072 4900 0000 ba02 0000 7254 0100  ...rI.......rT..
-00003ee0: 007a 2752 656e 6465 7265 722e 6163 746f  .z'Renderer.acto
-00003ef0: 7232 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  r2json.<locals>.
-00003f00: 3c6c 6973 7463 6f6d 703e 2902 da0d 7061  <listcomp>)...pa
-00003f10: 7261 6d73 5f6c 6179 6f75 74da 0d70 6172  rams_layout..par
-00003f20: 616d 735f 6669 656c 6473 da10 7061 7261  ams_fields..para
-00003f30: 6d73 5f70 616e 656c 5f70 6f73 2901 7261  ms_panel_pos).ra
-00003f40: 0100 0029 3772 2c00 0000 72b6 0000 0072  ...)7r,...r....r
-00003f50: 1b00 0000 7238 0100 00da 0d5f 6163 7469  ....r8....._acti
-00003f60: 6f6e 735f 6c69 7374 7271 0000 0072 f100  ons_listrq...r..
-00003f70: 0000 da0f 6765 745f 6163 746f 725f 6c61  ....get_actor_la
-00003f80: 6265 6cda 0462 6f6f 6cda 066d 6173 7465  bel..bool..maste
-00003f90: 72da 0c68 6964 655f 6564 6974 696e 6772  r..hide_editingr
-00003fa0: 2900 0000 72d3 0000 0072 7700 0000 da0a  )...r....rw.....
-00003fb0: 6765 745f 6861 6e64 6c65 da05 7374 6f72  get_handle..stor
-00003fc0: 6572 0400 0000 726f 0000 00da 066c 6f67  er....ro.....log
-00003fd0: 6765 72da 0777 6172 6e69 6e67 7283 0000  ger..warningr...
-00003fe0: 0072 4301 0000 72ab 0000 0072 3900 0000  .rC...r....r9...
-00003ff0: da0b 6c69 7374 5f66 6965 6c64 7372 b800  ..list_fieldsr..
-00004000: 0000 7253 0000 0072 a100 0000 721f 0000  ..rS...r....r...
-00004010: 0072 2000 0000 7222 0000 0072 2e01 0000  .r ...r"...r....
-00004020: 7228 0000 0072 5901 0000 722b 0000 0072  r(...rY...r+...r
-00004030: 3c01 0000 723f 0100 0072 5c01 0000 da11  <...r?...r\.....
-00004040: 6765 745f 7769 6e64 6f77 5f6c 6179 6f75  get_window_layou
-00004050: 7472 8800 0000 724e 0100 0072 7800 0000  tr....rN...rx...
-00004060: 7203 0100 0072 6800 0000 7276 0000 0072  r....rh...rv...r
-00004070: 0e00 0000 da07 6f62 6a65 6374 73da 0d67  ......objects..g
-00004080: 6574 5f66 6f72 5f6d 6f64 656c 72da 0000  et_for_modelr...
-00004090: 0072 6c00 0000 724e 0000 0072 5f01 0000  .rl...rN...r_...
-000040a0: da0c 7061 7261 6d73 5f73 746f 7265 da0c  ..params_store..
-000040b0: 7061 7261 6d5f 6669 656c 6473 7261 0100  param_fieldsra..
-000040c0: 0029 1172 4000 0000 72a6 0000 00da 0261  .).r@...r......a
-000040d0: 6cda 0268 6b72 a700 0000 da02 6168 da07  l..hkr......ah..
-000040e0: 636f 6c75 6d6e 73da 0969 6e64 6578 5f6d  columns..index_m
-000040f0: 6f64 da09 636f 6c5f 656c 656d 7372 4901  od..col_elemsrI.
-00004100: 0000 720d 0100 00da 0277 6c72 4f01 0000  ..r......wlrO...
-00004110: 7250 0100 0072 5701 0000 72b9 0000 0072  rP...rW...r....r
-00004120: 9000 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
-00004130: 0000 00da 0a61 6374 6f72 326a 736f 6e58  .....actor2jsonX
-00004140: 0200 0073 9200 0000 1601 1001 0601 0201  ...s............
-00004150: 0601 0801 0c01 06fc 0807 0c01 0802 0a01  ................
-00004160: 1201 0a03 0401 0401 0801 0801 0a01 1201  ................
-00004170: 0601 04ff 0201 08ff 1402 1403 0801 0a01  ................
-00004180: 0801 0c01 0801 1205 1001 0c0d 0c01 1602  ................
-00004190: 0c01 0a02 1001 0a02 0a01 0801 0e01 0602  ................
-000041a0: 1201 0c02 0a01 0e01 0c02 0a01 0e02 0e03  ................
-000041b0: 0601 0a01 0601 0aff 2603 0201 06ff 1803  ........&.......
-000041c0: 0801 0c01 0a01 1201 0480 0c02 0402 0601  ................
-000041d0: 1201 06fe 0c04 0e01 0401 7a13 5265 6e64  ..........z.Rend
-000041e0: 6572 6572 2e61 6374 6f72 326a 736f 6e63  erer.actor2jsonc
-000041f0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00004200: 0600 0000 0300 0000 7364 0000 0064 0188  ........sd...d..
-00004210: 015f 0088 016a 0144 005d 2289 0088 006a  ._...j.D.]"....j
-00004220: 0264 0075 0172 0e71 0674 036a 046a 0588  .d.u.r.q.t.j.j..
-00004230: 01a0 0688 006a 07a1 018e 007d 0287 0087  .....j.....}....
-00004240: 0166 0264 0264 0384 087d 0374 086a 096a  .f.d.d...}.t.j.j
-00004250: 0aa0 0b7c 027c 037c 01a1 0301 0071 0664  ...|.|.|.....q.d
-00004260: 0488 015f 0074 0c83 00a0 0d7c 01a1 0153  ..._.t.....|...S
-00004270: 0029 054e 5463 0100 0000 0000 0000 0000  .).NTc..........
-00004280: 0000 0100 0000 0600 0000 1300 0000 7318  ..............s.
-00004290: 0000 007c 00a0 0074 0188 01a0 0288 00a1  ...|...t........
-000042a0: 0183 01a1 0101 0064 0053 0072 3b00 0000  .......d.S.r;...
-000042b0: 2903 728c 0000 0072 2600 0000 7278 0100  ).r....r&...rx..
-000042c0: 0072 4501 0000 a902 7299 0000 0072 4000  .rE.....r....r@.
-000042d0: 0000 7237 0000 0072 3800 0000 728c 0000  ..r7...r8...r...
-000042e0: 00c9 0200 0073 0200 0000 1801 7a26 5265  .....s......z&Re
-000042f0: 6e64 6572 6572 2e62 7569 6c64 5f6a 735f  nderer.build_js_
-00004300: 6361 6368 652e 3c6c 6f63 616c 733e 2e77  cache.<locals>.w
-00004310: 7269 7465 4629 0e72 6e00 0000 726a 0000  riteF).rn...rj..
-00004320: 00da 0f67 6574 5f68 616e 646c 655f 6e61  ...get_handle_na
-00004330: 6d65 727d 0000 00da 0470 6174 68da 046a  mer}.....path..j
-00004340: 6f69 6e72 2401 0000 72f1 0000 0072 0400  oinr$...r....r..
-00004350: 0000 726f 0000 0072 2300 0000 da0f 6d61  ..ro...r#.....ma
-00004360: 6b65 5f63 6163 6865 5f66 696c 6572 3c00  ke_cache_filer<.
-00004370: 0000 da0e 6275 696c 645f 6a73 5f63 6163  ....build_js_cac
-00004380: 6865 2904 7240 0000 00da 0566 6f72 6365  he).r@.....force
-00004390: 7256 0100 0072 8c00 0000 7242 0000 0072  rV...r....rB...r
-000043a0: 7901 0000 7238 0000 0072 7e01 0000 c002  y...r8...r~.....
-000043b0: 0000 7312 0000 0006 020a 020a 0102 0114  ..s.............
-000043c0: 010e 0214 0306 020c 017a 1752 656e 6465  .........z.Rende
-000043d0: 7265 722e 6275 696c 645f 6a73 5f63 6163  rer.build_js_cac
-000043e0: 6865 723b 0000 0029 2072 b500 0000 da0a  her;...) r......
-000043f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00004400: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00004410: 5fda 0e69 735f 696e 7465 7261 6374 6976  _..is_interactiv
-00004420: 65da 0863 616e 5f61 7574 6872 1f01 0000  e..can_authr....
-00004430: 7223 0100 00da 1873 7570 706f 7274 5f64  r#.....support_d
-00004440: 6173 6862 6f61 7264 5f6c 6179 6f75 7472  ashboard_layoutr
-00004450: 3d00 0000 7294 0000 0072 4f00 0000 7287  =...r....rO...r.
-00004460: 0000 0072 ab00 0000 72ba 0000 0072 d000  ...r....r....r..
-00004470: 0000 72dd 0000 0072 e400 0000 72a5 0000  ..r....r....r...
-00004480: 0072 e000 0000 723f 0000 0072 ff00 0000  .r....r?...r....
-00004490: 7200 0100 0072 0101 0000 7215 0100 0072  r....r....r....r
-000044a0: 1b01 0000 7224 0100 0072 3801 0000 723f  ....r$...r8...r?
-000044b0: 0100 0072 7801 0000 727e 0100 00da 0d5f  ...rx...r~....._
-000044c0: 5f63 6c61 7373 6365 6c6c 5f5f 7237 0000  _classcell__r7..
-000044d0: 0072 3700 0000 7242 0000 0072 3800 0000  .r7...rB...r8...
-000044e0: 723a 0000 003b 0000 0073 3c00 0000 0800  r:...;...s<.....
-000044f0: 0401 0403 0401 0402 0401 0401 0c02 0804  ................
-00004500: 0857 081d 0808 0820 0803 0a18 0212 0aff  .W..... ........
-00004510: 0815 080e 0821 084e 080e 080a 082a 0809  .....!.N.....*..
-00004520: 080f 080a 0844 080c 1468 723a 0000 0072  .....D...hr:...r
-00004530: 3b00 0000 2948 727d 0000 00da 0770 6174  ;...)Hr}.....pat
-00004540: 686c 6962 7202 0000 00da 0468 746d 6c72  hlibr......htmlr
-00004550: 0300 0000 da0b 646a 616e 676f 2e63 6f6e  ......django.con
-00004560: 6672 0400 0000 da09 646a 616e 676f 2e64  fr......django.d
-00004570: 6272 0500 0000 da11 646a 616e 676f 2e75  br......django.u
-00004580: 7469 6c73 2e74 6578 7472 0600 0000 da0c  tils.textr......
-00004590: 646a 616e 676f 2e75 7469 6c73 7207 0000  django.utilsr...
-000045a0: 00da 126c 696e 6f2e 636f 7265 2e72 656e  ...lino.core.ren
-000045b0: 6465 7265 7272 0800 0000 7209 0000 00da  dererr....r.....
-000045c0: 0f6c 696e 6f2e 636f 7265 2e6d 656e 7573  .lino.core.menus
-000045d0: 720a 0000 0072 0b00 0000 da09 6c69 6e6f  r....r......lino
-000045e0: 2e63 6f72 6572 0c00 0000 720d 0000 00da  .corer....r.....
-000045f0: 0e6c 696e 6f2e 636f 7265 2e67 666b 7372  .lino.core.gfksr
-00004600: 0e00 0000 da1e 6c69 6e6f 2e6d 6f64 6c69  ......lino.modli
-00004610: 622e 6578 746a 732e 6578 745f 7265 6e64  b.extjs.ext_rend
-00004620: 6572 6572 720f 0000 00da 116c 696e 6f2e  ererr......lino.
-00004630: 636f 7265 2e61 6374 696f 6e73 7210 0000  core.actionsr...
-00004640: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00004650: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00004660: 1700 0000 da15 6c69 6e6f 2e63 6f72 652e  ......lino.core.
-00004670: 626f 756e 6461 6374 696f 6e72 1800 0000  boundactionr....
-00004680: da15 6c69 6e6f 2e63 6f72 652e 6368 6f69  ..lino.core.choi
-00004690: 6365 6c69 7374 7372 1900 0000 da1e 6c69  celistsr......li
-000046a0: 6e6f 2e6d 6f64 6c69 622e 7379 7374 656d  no.modlib.system
-000046b0: 2e63 686f 6963 656c 6973 7473 721a 0000  .choicelistsr...
-000046c0: 00da 106c 696e 6f2e 636f 7265 2e61 6374  ...lino.core.act
-000046d0: 6f72 7372 1b00 0000 da11 6c69 6e6f 2e63  orsr......lino.c
-000046e0: 6f72 652e 6c61 796f 7574 7372 1c00 0000  ore.layoutsr....
-000046f0: 721d 0000 00da 0f6c 696e 6f2e 636f 7265  r......lino.core
-00004700: 2e65 6c65 6d73 721e 0000 0072 1f00 0000  .elemsr....r....
-00004710: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00004720: 2300 0000 da0a 6574 6765 6e2e 6874 6d6c  #.....etgen.html
-00004730: 7224 0000 00da 0a6c 696e 6f2e 7574 696c  r$.....lino.util
-00004740: 7372 2500 0000 da10 6c69 6e6f 2e75 7469  sr%.....lino.uti
-00004750: 6c73 2e6a 7367 656e 7226 0000 0072 2700  ls.jsgenr&...r'.
-00004760: 0000 7228 0000 00da 176c 696e 6f2e 6d6f  ..r(.....lino.mo
-00004770: 646c 6962 2e75 7365 7273 2e75 7469 6c73  dlib.users.utils
-00004780: 7229 0000 0072 2a00 0000 da19 6c69 6e6f  r)...r*.....lino
-00004790: 2e6d 6f64 6c69 622e 7379 7374 656d 2e6d  .modlib.system.m
-000047a0: 6978 696e 7372 2b00 0000 da07 696e 7370  ixinsr+.....insp
-000047b0: 6563 7472 2c00 0000 da05 6963 6f6e 7372  ectr,.....iconsr
-000047c0: 2e00 0000 7239 0000 0072 3a00 0000 7237  ....r9...r:...r7
-000047d0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-000047e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000047f0: 733c 0000 0008 040c 010c 010c 010c 010c  s<..............
-00004800: 010c 0110 0210 020c 010c 010c 010c 0128  ...............(
-00004810: 020c 030c 010c 010c 0110 011c 010c 020c  ................
-00004820: 020c 0214 0110 020c 010c 020c 020a 0314  ................
-00004830: 0d                                       .
+00000020: 0004 0000 0040 0000 0073 b601 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 0100 6400 6408 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000090: 6d10 5a10 0100 6400 6409 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+000000a0: 6d13 5a13 0100 6400 640a 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 640b 6c14 6d16 5a16 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 640c 6c17 6d18 5a18 0100 6400 640d 6c19  d.l.m.Z...d.d.l.
+000000d0: 6d1a 5a1a 0100 6400 640e 6c1b 6d1c 5a1c  m.Z...d.d.l.m.Z.
+000000e0: 6d1d 5a1d 6d1e 5a1e 6d1f 5a1f 6d20 5a20  m.Z.m.Z.m.Z.m Z 
+000000f0: 6d21 5a21 6d22 5a22 6d23 5a23 0100 6400  m!Z!m"Z"m#Z#..d.
+00000100: 640f 6c24 6d25 5a25 0100 6400 6410 6c26  d.l$m%Z%..d.d.l&
+00000110: 6d27 5a27 0100 6400 6411 6c28 6d29 5a29  m'Z'..d.d.l(m)Z)
+00000120: 0100 6400 6412 6c2a 6d2b 5a2b 0100 6400  ..d.d.l*m+Z+..d.
+00000130: 6413 6c2c 6d2d 5a2d 6d2e 5a2e 0100 6400  d.l,m-Z-m.Z...d.
+00000140: 6414 6c2f 6d30 5a30 6d31 5a31 6d32 5a32  d.l/m0Z0m1Z1m2Z2
+00000150: 6d33 5a33 6d34 5a34 0100 6400 6415 6c14  m3Z3m4Z4..d.d.l.
+00000160: 6d35 5a35 0100 6400 6416 6c36 6d37 5a37  m5Z5..d.d.l6m7Z7
+00000170: 0100 6400 6417 6c38 6d39 5a39 0100 6400  ..d.d.l8m9Z9..d.
+00000180: 6418 6c3a 6d3b 5a3b 6d3c 5a3c 6d3d 5a3d  d.l:m;Z;m<Z<m=Z=
+00000190: 0100 6400 6419 6c3e 6d3f 5a3f 6d40 5a40  ..d.d.l>m?Z?m@Z@
+000001a0: 0100 6400 641a 6c41 6d42 5a42 0100 6400  ..d.d.lAmBZB..d.
+000001b0: 641b 6c43 6d44 5a44 0100 641c 641d 6c45  d.lCmDZD..d.d.lE
+000001c0: 6d46 5a46 0100 6422 641e 641f 8401 5a47  mFZF..d"d.d...ZG
+000001d0: 4700 6420 6421 8400 6421 6510 8303 5a48  G.d d!..d!e...ZH
+000001e0: 6401 5300 2923 e900 0000 004e 2901 da04  d.S.)#.....N)...
+000001f0: 5061 7468 2901 da06 6573 6361 7065 2901  Path)...escape).
+00000200: da08 7365 7474 696e 6773 2901 da06 6d6f  ..settings)...mo
+00000210: 6465 6c73 2901 da0b 666f 726d 6174 5f6c  dels)...format_l
+00000220: 617a 7929 01da 0b74 7261 6e73 6c61 7469  azy)...translati
+00000230: 6f6e 2902 da11 6164 645f 7573 6572 5f6c  on)...add_user_l
+00000240: 616e 6775 6167 65da 0f4a 7343 6163 6865  anguage..JsCache
+00000250: 5265 6e64 6572 6572 2902 da04 4d65 6e75  Renderer)...Menu
+00000260: da08 4d65 6e75 4974 656d 2901 da09 636f  ..MenuItem)...co
+00000270: 6e73 7461 6e74 7329 01da 0b63 686f 6963  nstants)...choic
+00000280: 656c 6973 7473 2901 da0b 436f 6e74 656e  elists)...Conten
+00000290: 7454 7970 6529 01da 0b45 7874 5265 6e64  tType)...ExtRend
+000002a0: 6572 6572 2908 da0e 5368 6f77 456d 7074  erer)...ShowEmpt
+000002b0: 7954 6162 6c65 da0a 5368 6f77 4465 7461  yTable..ShowDeta
+000002c0: 696c da0d 5772 6170 7065 6441 6374 696f  il..WrappedActio
+000002d0: 6eda 0a53 686f 7749 6e73 6572 74da 0953  n..ShowInsert..S
+000002e0: 686f 7754 6162 6c65 da0c 5375 626d 6974  howTable..Submit
+000002f0: 4465 7461 696c da0c 5375 626d 6974 496e  Detail..SubmitIn
+00000300: 7365 7274 da06 4163 7469 6f6e 2901 da0b  sert..Action)...
+00000310: 426f 756e 6441 6374 696f 6e29 01da 0e43  BoundAction)...C
+00000320: 686f 6963 654c 6973 744d 6574 6129 01da  hoiceListMeta)..
+00000330: 1044 6173 6862 6f61 7264 4c61 796f 7574  .DashboardLayout
+00000340: 7329 01da 0541 6374 6f72 2902 da0c 4c61  s)...Actor)...La
+00000350: 796f 7574 4861 6e64 6c65 da0a 4261 7365  youtHandle..Base
+00000360: 4c61 796f 7574 2905 da0d 4c61 796f 7574  Layout)...Layout
+00000370: 456c 656d 656e 74da 1143 6f6d 626f 4669  Element..ComboFi
+00000380: 656c 6445 6c65 6d65 6e74 da1d 5369 6d70  eldElement..Simp
+00000390: 6c65 5265 6d6f 7465 436f 6d62 6f46 6965  leRemoteComboFie
+000003a0: 6c64 456c 656d 656e 74da 0c46 6965 6c64  ldElement..Field
+000003b0: 456c 656d 656e 74da 1750 7265 7669 6577  Element..Preview
+000003c0: 5465 7874 4669 656c 6445 6c65 6d65 6e74  TextFieldElement
+000003d0: 2901 da06 6b65 726e 656c 2901 da01 4529  )...kernel)...E)
+000003e0: 01da 056a 7367 656e 2903 da05 7079 326a  ...jsgen)...py2j
+000003f0: 73da 076a 735f 636f 6465 da08 6f62 6a32  s..js_code..obj2
+00000400: 6469 6374 2902 da10 6765 745f 7573 6572  dict)...get_user
+00000410: 5f70 726f 6669 6c65 da11 7769 7468 5f75  _profile..with_u
+00000420: 7365 725f 7072 6f66 696c 6529 01da 0845  ser_profile)...E
+00000430: 6469 7453 6166 6529 01da 0769 7363 6c61  ditSafe)...iscla
+00000440: 7373 e901 0000 0029 01da 1252 4541 4354  ss.....)...REACT
+00000450: 5f49 434f 4e5f 4d41 5050 494e 4763 0300  _ICON_MAPPINGc..
+00000460: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+00000470: 0000 4300 0000 734a 0000 007c 0264 016b  ..C...sJ...|.d.k
+00000480: 0273 0c74 007c 0283 0173 0c4a 0064 0283  .s.t.|...s.J.d..
+00000490: 0182 0174 017c 0083 0144 005d 125c 027d  ...t.|...D.].\.}
+000004a0: 037d 047c 0272 1a7c 027c 0483 017d 047c  .}.|.r.|.|...}.|
+000004b0: 047c 016b 0272 227c 0302 0001 0053 0071  .|.k.r"|.....S.q
+000004c0: 1064 0353 0029 047a 4d52 6574 7572 6e73  .d.S.).zMReturns
+000004d0: 2074 6865 2069 6e64 6578 206f 6620 616e   the index of an
+000004e0: 2065 6c65 6d65 6e74 2069 6e20 6120 6361   element in a ca
+000004f0: 6c6c 6162 6c65 2077 6869 6368 2063 616e  llable which can
+00000500: 2062 6520 7573 6520 6120 6b65 7920 6675   be use a key fu
+00000510: 6e63 7469 6f6e 4e7a 586b 6579 2073 686f  nctionNzXkey sho
+00000520: 6c64 2062 6520 6120 6675 6e63 7469 6f6e  ld be a function
+00000530: 2074 6861 7420 7461 6b65 7320 7468 6520   that takes the 
+00000540: 6974 7465 7227 7320 6974 656d 2061 6e64  itter's item and
+00000550: 2072 6574 7572 6e73 2074 6861 7420 7761   returns that wa
+00000560: 6e74 6564 206d 6174 6368 6564 2069 7465  nted matched ite
+00000570: 6de9 ffff ffff 2902 da08 6361 6c6c 6162  m.....)...callab
+00000580: 6c65 da09 656e 756d 6572 6174 6529 05da  le..enumerate)..
+00000590: 0569 7474 6572 da06 7461 7267 6574 da03  .itter..target..
+000005a0: 6b65 79da 0169 da01 78a9 0072 3700 0000  key..i..x..r7...
+000005b0: fa45 2f68 6f6d 652f 626c 7572 7279 2f6c  .E/home/blurry/l
+000005c0: 696e 6f2f 656e 762f 7265 706f 7369 746f  ino/env/reposito
+000005d0: 7269 6573 2f72 6561 6374 2f6c 696e 6f5f  ries/react/lino_
+000005e0: 7265 6163 742f 7265 6163 742f 7265 6e64  react/react/rend
+000005f0: 6572 6572 2e70 79da 0466 696e 642f 0000  erer.py..find/..
+00000600: 0073 1000 0000 1802 1002 0401 0801 0801  .s..............
+00000610: 0801 02ff 0403 7239 0000 0063 0000 0000  ......r9...c....
+00000620: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000630: 0000 0000 73e6 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000640: 0264 015a 0364 025a 0464 025a 0564 035a  .d.Z.d.Z.d.Z.d.Z
+00000650: 0664 045a 0764 025a 0887 0066 0164 0564  .d.Z.d.Z...f.d.d
+00000660: 0684 085a 0964 0764 0884 005a 0a64 0964  ...Z.d.d...Z.d.d
+00000670: 0a84 005a 0b64 0b64 0c84 005a 0c64 0d64  ...Z.d.d...Z.d.d
+00000680: 0e84 005a 0d64 0f64 1084 005a 0e64 1164  ...Z.d.d...Z.d.d
+00000690: 1284 005a 0f64 3264 1464 1584 015a 1069  ...Z.d2d.d...Z.i
+000006a0: 0066 0164 1664 1784 015a 1164 1864 1984  .f.d.d...Z.d.d..
+000006b0: 005a 1264 1a64 1b84 005a 1364 1c64 1d84  .Z.d.d...Z.d.d..
+000006c0: 005a 1464 1e64 1f84 005a 1564 2064 2184  .Z.d.d...Z.d d!.
+000006d0: 005a 1664 2264 2384 005a 1764 2464 2584  .Z.d"d#..Z.d$d%.
+000006e0: 005a 1864 2664 2784 005a 1964 2864 2984  .Z.d&d'..Z.d(d).
+000006f0: 005a 1a64 2a64 2b84 005a 1b64 2c64 2d84  .Z.d*d+..Z.d,d-.
+00000700: 005a 1c64 2e64 2f84 005a 1d87 0066 0164  .Z.d.d/..Z...f.d
+00000710: 3064 3184 085a 1e87 0004 005a 1f53 0029  0d1..Z.....Z.S.)
+00000720: 33da 0852 656e 6465 7265 727a 480a 2020  3..RendererzH.  
+00000730: 2020 4120 6672 6f6e 742d 656e 6420 7265    A front-end re
+00000740: 6e64 6572 6572 2074 6861 7420 7573 6573  nderer that uses
+00000750: 2074 6865 2052 6561 6374 204a 6176 6173   the React Javas
+00000760: 6372 6970 7420 6672 616d 6577 6f72 6b2e  cript framework.
+00000770: 0a20 2020 2054 7a12 7265 6163 742f 6c69  .    Tz.react/li
+00000780: 6e6f 7765 622e 6a73 6f6e 7a05 2e6a 736f  noweb.jsonz..jso
+00000790: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
+000007a0: 0000 0300 0000 0300 0000 731c 0000 0074  ..........s....t
+000007b0: 0083 00a0 017c 01a1 0101 0074 02a0 037c  .....|.....t...|
+000007c0: 006a 04a1 0101 0064 0053 00a9 014e 2905  .j.....d.S...N).
+000007d0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+000007e0: 5f72 2500 0000 da12 7265 6769 7374 6572  _r%.....register
+000007f0: 5f63 6f6e 7665 7274 6572 da0f 7079 326a  _converter..py2j
+00000800: 735f 636f 6e76 6572 7465 7229 02da 0473  s_converter)...s
+00000810: 656c 66da 0966 726f 6e74 5f65 6e64 a901  elf..front_end..
+00000820: da09 5f5f 636c 6173 735f 5f72 3700 0000  ..__class__r7...
+00000830: 7238 0000 0072 3d00 0000 4700 0000 7304  r8...r=...G...s.
+00000840: 0000 000c 0110 017a 1152 656e 6465 7265  .......z.Rendere
+00000850: 722e 5f5f 696e 6974 5f5f 6302 0000 0000  r.__init__c.....
+00000860: 0000 0000 0000 000c 0000 0008 0000 0003  ................
+00000870: 0000 0073 7c02 0000 6401 6402 8400 7400  ...s|...d.d...t.
+00000880: 6a01 a002 a100 4400 8301 7d02 7403 8300  j.....D...}.t...
+00000890: 7d03 8800 6a04 4400 5d14 7d04 7c04 a005  }...j.D.].}.|...
+000008a0: a100 4400 5d0d 7d05 7c05 6a06 7c03 7601  ..D.].}.|.j.|.v.
+000008b0: 7223 7c03 a007 7c05 6a06 a101 0100 7116  r#|...|.j.....q.
+000008c0: 7110 6403 8800 5f08 7409 6a0a 6a0b 7d06  q.d..._.t.j.j.}.
+000008d0: 740c 8700 6601 6404 6402 8408 7c03 4400  t...f.d.d...|.D.
+000008e0: 8301 7409 6a0a a00d 740e 8300 a101 7c06  ..t.j...t.....|.
+000008f0: 6a0f 6a10 7409 6a0a 6a11 8800 6a12 6a13  j.j.t.j.j...j.j.
+00000900: 6405 7501 6406 6402 8400 7409 6a0a 6a14  d.u.d.d...t.j.j.
+00000910: 4400 8301 6407 8d06 7d07 7409 6a0a a015  D...d...}.t.j...
+00000920: 6408 a101 7264 7c07 6a16 7417 7c06 6a18  d...rd|.j.t.|.j.
+00000930: 6a19 6a1a a01b a100 8301 6409 8d01 0100  j.j.......d.....
+00000940: 7c07 6a16 7409 6a0a 6a00 6a1c 640a 8d01  |.j.t.j.j.j.d...
+00000950: 0100 7a12 741d a01e 741f 7409 6a20 8301  ..z.t...t.t.j ..
+00000960: 640b 1b00 640c 1b00 a101 6a21 7c07 7422  d...d.....j!|.t"
+00000970: 6a23 3c00 5700 6e09 0400 7424 7988 0100  j#<.W.n...t$y...
+00000980: 0100 0100 5900 6e01 7700 7425 7409 6a0a  ....Y.n.w.t%t.j.
+00000990: 640d 8302 7297 7c07 6a16 7409 6a0a 6a26  d...r.|.j.t.j.j&
+000009a0: 640e 8d01 0100 7409 6a0a 6a27 6405 6b02  d.....t.j.j'd.k.
+000009b0: 72a4 7c07 6a16 6403 640f 8d01 0100 6e0e  r.|.j.d.d.....n.
+000009c0: 7425 7c06 6a28 6410 8302 72b2 7c07 6a16  t%|.j(d...r.|.j.
+000009d0: 7c06 6a28 6a29 6411 8d01 0100 7409 6a0a  |.j(j)d.....t.j.
+000009e0: a015 6412 a101 72c4 7c07 6a16 7c06 6a2a  ..d...r.|.j.|.j*
+000009f0: 6a2b 6fc1 7409 6a0a 6a2c 6413 8d01 0100  j+o.t.j.j,d.....
+00000a00: 6900 7d08 8800 6a2d 4400 5d2f 7d09 8800  i.}...j-D.]/}...
+00000a10: a02e 7c09 a101 7c08 7c09 6a2f 3c00 7425  ..|...|.|.j/<.t%
+00000a20: 7c09 6414 8302 72f8 6415 7c09 6a2f 7600  |.d...r.d.|.j/v.
+00000a30: 72f8 7430 7c02 6416 1900 8301 4400 5d14  r.t0|.d.....D.].
+00000a40: 5c02 7d0a 7d0b 7c0b 6417 1900 7c09 6a31  \.}.}.|.d...|.j1
+00000a50: 6b02 72f7 7c09 6a2f 7c02 6416 1900 7c0a  k.r.|.j/|.d...|.
+00000a60: 1900 6418 3c00 71e3 71c9 8800 6a32 4400  ..d.<.q.q...j2D.
+00000a70: 5d0a 7d09 8800 a02e 7c09 a101 7c08 7c09  ].}.....|...|.|.
+00000a80: 6a2f 3c00 71fc 8800 6a33 4400 5d0b 7d09  j/<.q...j3D.].}.
+00000a90: 8800 a02e 7c09 a101 7c08 7c09 6a2f 3c00  ....|...|.|.j/<.
+00000aa0: 9001 710a 8800 6a34 4400 5d0b 7d09 8800  ..q...j4D.].}...
+00000ab0: a02e 7c09 a101 7c08 7c09 6a2f 3c00 9001  ..|...|.|.j/<...
+00000ac0: 7119 7c07 6a16 7c08 7c02 6419 8d02 0100  q.|.j.|.|.d.....
+00000ad0: 7435 6a36 7435 a037 7438 7c07 8301 a101  t5j6t5.7t8|.....
+00000ae0: 7c01 641a 641b 8d03 0100 641c 8800 5f08  |.d.d.....d..._.
+00000af0: 641d 5300 291e 7a86 0a20 2020 2020 2020  d.S.).z..       
+00000b00: 2043 7265 6174 6573 2077 6861 7420 6973   Creates what is
+00000b10: 206b 6e6f 776e 2061 7320 7769 6e64 6f77   known as window
+00000b20: 2e41 7070 2e73 7461 7465 2e73 6974 655f  .App.state.site_
+00000b30: 6461 7461 2069 6e20 5265 6163 7420 636f  data in React co
+00000b40: 6465 2e0a 0a20 2020 2020 2020 203a 7061  de...        :pa
+00000b50: 7261 6d20 663a 2046 696c 6520 6f62 6a65  ram f: File obje
+00000b60: 6374 0a20 2020 2020 2020 203a 7265 7475  ct.        :retu
+00000b70: 726e 3a20 310a 2020 2020 2020 2020 6301  rn: 1.        c.
+00000b80: 0000 0000 0000 0000 0000 0003 0000 0006  ................
+00000b90: 0000 0053 0000 0073 2400 0000 6900 7c00  ...S...s$...i.|.
+00000ba0: 5d0e 5c02 7d01 7d02 7c01 6400 6401 8400  ].\.}.}.|.d.d...
+00000bb0: 7c02 a000 a100 4400 8301 9302 7102 5300  |.....D.....q.S.
+00000bc0: 2902 6301 0000 0000 0000 0000 0000 0002  ).c.............
+00000bd0: 0000 0006 0000 0053 0000 0073 2400 0000  .......S...s$...
+00000be0: 6700 7c00 5d0e 7d01 7c01 6400 1900 6a00  g.|.].}.|.d...j.
+00000bf0: 7401 7c01 6401 1900 8301 6402 9c02 9102  t.|.d.....d.....
+00000c00: 7102 5300 2903 7201 0000 0072 2d00 0000  q.S.).r....r-...
+00000c10: 2902 da05 7661 6c75 65da 0474 6578 7429  )...value..text)
+00000c20: 0272 4400 0000 da03 7374 7229 02da 022e  .rD.....str)....
+00000c30: 30da 0163 7237 0000 0072 3700 0000 7238  0..cr7...r7...r8
+00000c40: 0000 00da 0a3c 6c69 7374 636f 6d70 3e54  .....<listcomp>T
+00000c50: 0000 0073 0200 0000 2400 7a35 5265 6e64  ...s....$.z5Rend
+00000c60: 6572 6572 2e77 7269 7465 5f6c 696e 6f5f  erer.write_lino_
+00000c70: 6a73 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  js.<locals>.<dic
+00000c80: 7463 6f6d 703e 2e3c 6c69 7374 636f 6d70  tcomp>.<listcomp
+00000c90: 3e29 01da 0b67 6574 5f63 686f 6963 6573  >)...get_choices
+00000ca0: 2903 7247 0000 00da 0249 44da 0263 6c72  ).rG.....ID..clr
+00000cb0: 3700 0000 7237 0000 0072 3800 0000 da0a  7...r7...r8.....
+00000cc0: 3c64 6963 7463 6f6d 703e 5200 0000 7308  <dictcomp>R...s.
+00000cd0: 0000 0006 0006 0312 ff06 fe7a 2a52 656e  ...........z*Ren
+00000ce0: 6465 7265 722e 7772 6974 655f 6c69 6e6f  derer.write_lino
+00000cf0: 5f6a 732e 3c6c 6f63 616c 733e 2e3c 6469  _js.<locals>.<di
+00000d00: 6374 636f 6d70 3e54 6301 0000 0000 0000  ctcomp>Tc.......
+00000d10: 0000 0000 0002 0000 0006 0000 0013 0000  ................
+00000d20: 0073 1a00 0000 6900 7c00 5d09 7d01 7c01  .s....i.|.].}.|.
+00000d30: 6a00 8800 a001 7c01 a101 9302 7102 5300  j.....|.....q.S.
+00000d40: 7237 0000 0029 02da 0b61 6374 696f 6e5f  r7...)...action_
+00000d50: 6e61 6d65 da0b 6163 7469 6f6e 326a 736f  name..action2jso
+00000d60: 6e29 0272 4700 0000 da01 61a9 0172 4000  n).rG.....a..r@.
+00000d70: 0000 7237 0000 0072 3800 0000 724d 0000  ..r7...r8...rM..
+00000d80: 0061 0000 0073 0200 0000 1a00 4e63 0100  .a...s......Nc..
+00000d90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000da0: 0000 5300 0000 7316 0000 0069 007c 005d  ..S...s....i.|.]
+00000db0: 077d 017c 016a 007c 016a 0193 0271 0253  .}.|.j.|.j...q.S
+00000dc0: 0072 3700 0000 2902 da0b 646a 616e 676f  .r7...)...django
+00000dd0: 5f63 6f64 65da 046e 616d 6529 0272 4700  _code..name).rG.
+00000de0: 0000 da04 6c61 6e67 7237 0000 0072 3700  ....langr7...r7.
+00000df0: 0000 7238 0000 0072 4d00 0000 6700 0000  ..r8...rM...g...
+00000e00: 7302 0000 0016 0029 06da 0761 6374 696f  s......)...actio
+00000e10: 6e73 da04 6d65 6e75 da15 7573 655f 6461  ns..menu..use_da
+00000e20: 7368 626f 6172 645f 6c61 796f 7574 73da  shboard_layouts.
+00000e30: 0a73 6974 655f 7469 746c 65da 1065 6469  .site_title..edi
+00000e40: 7469 6e67 5f66 726f 6e74 656e 64da 096c  ting_frontend..l
+00000e50: 616e 6775 6167 6573 da04 6d65 6d6f 2901  anguages..memo).
+00000e60: da0a 7375 6767 6573 746f 7273 2901 da0f  ..suggestors)...
+00000e70: 7265 7669 7369 6f6e 5f6e 756d 6265 72da  revision_number.
+00000e80: 0572 6561 6374 7a07 6d61 696e 2e6a 73da  .reactz.main.js.
+00000e90: 0a74 6865 6d65 5f6e 616d 6529 0172 5f00  .theme_name).r_.
+00000ea0: 0000 2901 da0d 6e6f 5f75 7365 725f 6d6f  ..)...no_user_mo
+00000eb0: 6465 6cda 1961 6c6c 6f77 5f6f 6e6c 696e  del..allow_onlin
+00000ec0: 655f 7265 6769 7374 7261 7469 6f6e 2901  e_registration).
+00000ed0: 7261 0000 00da 066e 6f74 6966 7929 01da  ra.....notify)..
+00000ee0: 0c75 7365 5f70 7573 685f 6170 69da 0b63  .use_push_api..c
+00000ef0: 686f 6963 655f 6e61 6d65 7a10 7379 7374  hoice_namez.syst
+00000f00: 656d 2e44 6173 6862 6f61 7264 7a17 7379  em.Dashboardz.sy
+00000f10: 7374 656d 2e44 6173 6862 6f61 7264 4c61  stem.DashboardLa
+00000f20: 796f 7574 7372 4400 0000 da0d 7769 6e64  youtsrD.....wind
+00000f30: 6f77 5f6c 6179 6f75 7429 02da 0b66 6f72  ow_layout)...for
+00000f40: 6d5f 7061 6e65 6c73 720d 0000 00e9 0400  m_panelsr.......
+00000f50: 0000 a901 da06 696e 6465 6e74 4672 2d00  ......indentFr-.
+00000f60: 0000 2939 7223 0000 00da 0b43 484f 4943  ..)9r#.....CHOIC
+00000f70: 454c 4953 5453 da05 6974 656d 73da 0373  ELISTS..items..s
+00000f80: 6574 da0b 6163 746f 7273 5f6c 6973 74da  et..actors_list.
+00000f90: 0b67 6574 5f61 6374 696f 6e73 da06 6163  .get_actions..ac
+00000fa0: 7469 6f6e da03 6164 64da 1173 6572 6961  tion..add..seria
+00000fb0: 6c69 7365 5f6a 735f 636f 6465 7204 0000  lise_js_coder...
+00000fc0: 00da 0453 4954 45da 0770 6c75 6769 6e73  ...SITE..plugins
+00000fd0: da04 6469 6374 da0d 6765 745f 7369 7465  ..dict..get_site
+00000fe0: 5f6d 656e 7572 2900 0000 da06 7379 7374  _menur).....syst
+00000ff0: 656d 7257 0000 00da 0574 6974 6c65 7241  emrW.....titlerA
+00001000: 0000 00da 0a75 726c 5f70 7265 6669 7872  .....url_prefixr
+00001010: 5a00 0000 da0c 6973 5f69 6e73 7461 6c6c  Z.....is_install
+00001020: 6564 da06 7570 6461 7465 da04 6c69 7374  ed..update..list
+00001030: 725b 0000 00da 0670 6172 7365 72da 0a73  r[.....parser..s
+00001040: 7567 6765 7374 6572 73da 046b 6579 73da  uggesters..keys.
+00001050: 0a63 6f64 655f 6d74 696d 65da 026f 73da  .code_mtime..os.
+00001060: 0473 7461 7472 0200 0000 da0b 5354 4154  .statr......STAT
+00001070: 4943 5f52 4f4f 54da 0873 745f 6d74 696d  IC_ROOT..st_mtim
+00001080: 6572 0c00 0000 da1b 5552 4c5f 5041 5241  er......URL_PARA
+00001090: 4d5f 4d41 494e 5f4a 535f 5449 4d45 5354  M_MAIN_JS_TIMEST
+000010a0: 414d 50da 1146 696c 654e 6f74 466f 756e  AMP..FileNotFoun
+000010b0: 6445 7272 6f72 da07 6861 7361 7474 7272  dError..hasattrr
+000010c0: 5f00 0000 da0a 7573 6572 5f6d 6f64 656c  _.....user_model
+000010d0: da05 7573 6572 7372 6100 0000 7262 0000  ..usersra...rb..
+000010e0: 0072 6300 0000 da09 7573 655f 6c69 6e6f  .rc.....use_lino
+000010f0: 6472 6600 0000 da0a 7061 6e65 6c32 6a73  drf.....panel2js
+00001100: 6f6e da0f 5f66 6f72 6d70 616e 656c 5f6e  on.._formpanel_n
+00001110: 616d 6572 3100 0000 7264 0000 00da 0c70  amer1...rd.....p
+00001120: 6172 616d 5f70 616e 656c 73da 1361 6374  aram_panels..act
+00001130: 696f 6e5f 7061 7261 6d5f 7061 6e65 6c73  ion_param_panels
+00001140: da0c 6f74 6865 725f 7061 6e65 6c73 da04  ..other_panels..
+00001150: 6a73 6f6e da04 6475 6d70 da05 6c6f 6164  json..dump..load
+00001160: 7372 2600 0000 290c 7240 0000 00da 0166  sr&...).r@.....f
+00001170: da10 6368 6f69 6365 6c69 7374 735f 6461  ..choicelists_da
+00001180: 7461 7255 0000 00da 0372 7074 da02 6261  tarU.....rpt..ba
+00001190: 7273 0000 00da 0464 6174 6172 6600 0000  rs.....datarf...
+000011a0: da01 7072 3500 0000 da04 6974 656d 7237  ..pr5.....itemr7
+000011b0: 0000 0072 5100 0000 7238 0000 00da 0d77  ...rQ...r8.....w
+000011c0: 7269 7465 5f6c 696e 6f5f 6a73 4b00 0000  rite_lino_jsK...
+000011d0: 7378 0000 0006 0708 0306 fd06 050a 010c  sx..............
+000011e0: 020a 010c 0102 8002 fe06 0408 0102 0110  ................
+000011f0: 010c 0206 0106 010a 0110 0106 f90c 0904  ................
+00001200: 0210 0106 ff12 0602 0104 0110 0102 ff02  ................
+00001210: 020c fe0c 0304 0102 ff0c 0310 010c 020e  ................
+00001220: 010c 0110 010c 0218 0104 090a 0110 0114  ................
+00001230: 0114 010e 0112 0104 800a 0112 010a 0114  ................
+00001240: 010a 0114 010e 011a 0506 0304 017a 1652  .............z.R
+00001250: 656e 6465 7265 722e 7772 6974 655f 6c69  enderer.write_li
+00001260: 6e6f 5f6a 7363 0200 0000 0000 0000 0000  no_jsc..........
+00001270: 0000 0400 0000 0600 0000 4300 0000 73c6  ..........C...s.
+00001280: 0000 0074 007c 0174 0183 0273 074a 0082  ...t.|.t...s.J..
+00001290: 0174 027c 016a 037c 01a0 04a1 007c 01a0  .t.|.j.|.....|..
+000012a0: 05a1 007c 016a 0664 018d 047d 0274 007c  ...|.j.d...}.t.|
+000012b0: 0174 0783 0272 297c 016a 086a 096a 037c  .t...r)|.j.j.j.|
+000012c0: 0264 023c 0074 0a7c 016a 086a 0b83 017c  .d.<.t.|.j.j...|
+000012d0: 0264 033c 007c 016a 0c72 317c 016a 0c7c  .d.<.|.j.r1|.j.|
+000012e0: 0264 043c 007c 016a 0d72 397c 016a 0d7c  .d.<.|.j.r9|.j.|
+000012f0: 0264 053c 007c 016a 0e72 4064 067c 0264  .d.<.|.j.r@d.|.d
+00001300: 073c 007c 016a 0f72 487c 016a 0f7c 0264  .<.|.j.rH|.j.|.d
+00001310: 083c 007c 016a 1072 4f64 067c 0264 093c  .<.|.j.rOd.|.d.<
+00001320: 007c 016a 1172 5664 067c 0264 0a3c 007c  .|.j.rVd.|.d.<.|
+00001330: 00a0 127c 01a1 017d 037c 0372 617c 037c  ...|...}.|.ra|.|
+00001340: 0264 0b3c 007c 0253 0029 0c7a 3343 6f6e  .d.<.|.S.).z3Con
+00001350: 7665 7274 7320 676c 6f62 616c 206c 6973  verts global lis
+00001360: 7420 6f66 2061 6c6c 2061 6374 696f 6e73  t of all actions
+00001370: 2074 6f20 6a73 6f6e 2066 6f72 6d61 742e   to json format.
+00001380: 2904 da02 616e da05 6c61 6265 6cda 0d77  )...an..label..w
+00001390: 696e 646f 775f 6163 7469 6f6e da0b 6874  indow_action..ht
+000013a0: 7470 5f6d 6574 686f 6472 9a00 0000 da05  tp_methodr......
+000013b0: 6163 746f 72da 0c70 7265 7072 6f63 6573  actor..preproces
+000013c0: 736f 72da 0b73 656c 6563 745f 726f 7773  sor..select_rows
+000013d0: 54da 1073 7562 6d69 745f 666f 726d 5f64  T..submit_form_d
+000013e0: 6174 61da 0b62 7574 746f 6e5f 7465 7874  ata..button_text
+000013f0: da14 7368 6f77 5f69 6e5f 7369 6465 5f74  ..show_in_side_t
+00001400: 6f6f 6c62 6172 da0e 6e65 7665 725f 636f  oolbar..never_co
+00001410: 6c6c 6170 7365 da04 6963 6f6e 2913 da0a  llapse..icon)...
+00001420: 6973 696e 7374 616e 6365 7217 0000 0072  isinstancer....r
+00001430: 7400 0000 724e 0000 00da 0967 6574 5f6c  t...rN.....get_l
+00001440: 6162 656c da10 6973 5f77 696e 646f 775f  abel..is_window_
+00001450: 6163 7469 6f6e 729d 0000 0072 1200 0000  actionr....r....
+00001460: da0c 626f 756e 645f 6163 7469 6f6e 726f  ..bound_actionro
+00001470: 0000 0072 4600 0000 729e 0000 0072 9f00  ...rF...r....r..
+00001480: 0000 72a0 0000 0072 a100 0000 72a2 0000  ..r....r....r...
+00001490: 0072 a300 0000 72a4 0000 00da 0f67 6574  .r....r......get
+000014a0: 5f61 6374 696f 6e5f 6963 6f6e 2904 7240  _action_icon).r@
+000014b0: 0000 00da 0176 da06 7265 7375 6c74 72a5  .....v..resultr.
+000014c0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+000014d0: 0000 724f 0000 00a3 0000 0073 2400 0000  ..rO.......s$...
+000014e0: 0e02 0604 0601 0601 0401 06fd 0a06 0e01  ................
+000014f0: 1001 1002 1002 0e01 1001 0e01 0e01 0a02  ................
+00001500: 0c01 0402 7a14 5265 6e64 6572 6572 2e61  ....z.Renderer.a
+00001510: 6374 696f 6e32 6a73 6f6e 6302 0000 0000  ction2jsonc.....
+00001520: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00001530: 0000 0073 2e00 0000 7400 7c01 7401 8302  ...s....t.|.t...
+00001540: 7307 4a00 8201 7c01 a002 a100 7d02 7403  s.J...|.....}.t.
+00001550: 7c00 a004 7c02 6a05 a101 7c02 6a06 6a07  |...|.j...|.j.j.
+00001560: 6401 8d02 5300 2902 4e29 02da 046d 6169  d...S.).N)...mai
+00001570: 6eda 0b77 696e 646f 775f 7369 7a65 2908  n..window_size).
+00001580: 72a6 0000 0072 1d00 0000 da11 6765 745f  r....r......get_
+00001590: 6c61 796f 7574 5f68 616e 646c 6572 7400  layout_handlert.
+000015a0: 0000 da09 656c 656d 326a 736f 6e72 ad00  ....elem2jsonr..
+000015b0: 0000 da06 6c61 796f 7574 72ae 0000 0029  ....layoutr....)
+000015c0: 0372 4000 0000 7297 0000 0072 ab00 0000  .r@...r....r....
+000015d0: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+000015e0: 8a00 0000 c000 0000 730a 0000 000e 0108  ........s.......
+000015f0: 030c 0106 0106 ff7a 1352 656e 6465 7265  .......z.Rendere
+00001600: 722e 7061 6e65 6c32 6a73 6f6e 6302 0000  r.panel2jsonc...
+00001610: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00001620: 0003 0000 0073 da00 0000 7400 7c01 7401  .....s....t.|.t.
+00001630: 8302 7307 4a00 8201 7402 7c01 a003 a100  ..s.J...t.|.....
+00001640: 7c01 6a04 7c01 6a05 6a06 6401 8d03 7d02  |.j.|.j.j.d...}.
+00001650: 7407 7c01 6402 8302 7224 8700 6601 6403  t.|.d...r$..f.d.
+00001660: 6404 8408 7c01 6a08 4400 8301 7c02 6405  d...|.j.D...|.d.
+00001670: 3c00 7c02 a009 740a 7c01 6406 8302 a101  <.|...t.|.d.....
+00001680: 0100 7407 7c01 6407 8302 7255 7c02 a009  ..t.|.d...rU|...
+00001690: 740a 7c01 6a0b 6408 8302 a101 0100 7407  t.|.j.d.......t.
+000016a0: 7c01 6409 8302 7255 7c01 6a0c 6400 7501  |.d...rU|.j.d.u.
+000016b0: 7255 7c01 6a0c a00d a100 4400 5d0b 5c02  rU|.j.....D.].\.
+000016c0: 7d03 7d01 8800 a00e 7c01 a101 7c02 7c03  }.}.....|...|.|.
+000016d0: 3c00 7149 740f 7c01 6a05 7410 8302 726b  <.qIt.|.j.t...rk
+000016e0: 7c02 6a09 7c01 a011 a100 640a 8d01 0100  |.j.|.....d.....
+000016f0: 7c02 6a09 7c01 6a12 6a13 640b 8d01 0100  |.j.|.j.j.d.....
+00001700: 7c02 5300 290c 4e29 0372 9b00 0000 da08  |.S.).N).r......
+00001710: 736f 7274 6162 6c65 da0a 7265 6163 745f  sortable..react_
+00001720: 6e61 6d65 da08 656c 656d 656e 7473 6301  name..elementsc.
+00001730: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00001740: 0000 0013 0000 0073 1e00 0000 6700 7c00  .......s....g.|.
+00001750: 5d0b 7d01 7c01 a000 a100 7202 8800 a001  ].}.|.....r.....
+00001760: 7c01 a101 9102 7102 5300 7237 0000 0029  |.....q.S.r7...)
+00001770: 02da 0a69 735f 7669 7369 626c 6572 b000  ...is_visibler..
+00001780: 0000 2902 7247 0000 00da 0165 7251 0000  ..).rG.....erQ..
+00001790: 0072 3700 0000 7238 0000 0072 4900 0000  .r7...r8...rI...
+000017a0: d000 0000 7302 0000 001e 007a 2652 656e  ....s......z&Ren
+000017b0: 6465 7265 722e 656c 656d 326a 736f 6e2e  derer.elem2json.
+000017c0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000017d0: 6d70 3e72 6b00 0000 7a98 6669 656c 6473  mp>rk...z.fields
+000017e0: 5f69 6e64 6578 2066 6965 6c64 735f 696e  _index fields_in
+000017f0: 6465 785f 6869 6464 656e 2065 6469 7461  dex_hidden edita
+00001800: 626c 6520 7665 7274 6963 616c 2068 7061  ble vertical hpa
+00001810: 6420 6973 5f66 6965 6c64 7365 7420 6e61  d is_fieldset na
+00001820: 6d65 2077 6964 7468 2070 7265 6665 7272  me width preferr
+00001830: 6564 5f77 6964 7468 2020 2020 2020 2020  ed_width        
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
+00001860: 2076 616c 7565 2068 666c 6578 2076 666c   value hflex vfl
+00001870: 6578 729e 0000 007a 1561 6374 6f72 5f69  exr....z.actor_i
+00001880: 6420 6469 7370 6c61 795f 6d6f 6465 da06  d display_mode..
+00001890: 736c 6176 6573 2901 da0d 6669 656c 645f  slaves)...field_
+000018a0: 6f70 7469 6f6e 7329 01da 0968 656c 705f  options)...help_
+000018b0: 7465 7874 2914 72a6 0000 0072 1e00 0000  text).r....r....
+000018c0: 7274 0000 0072 a700 0000 72b2 0000 0072  rt...r....r....r
+000018d0: 4300 0000 da08 5f5f 6e61 6d65 5f5f 7286  C.....__name__r.
+000018e0: 0000 0072 b400 0000 727a 0000 0072 2800  ...r....rz...r(.
+000018f0: 0000 729e 0000 0072 b700 0000 726b 0000  ..r....r....rk..
+00001900: 0072 b000 0000 da0a 6973 7375 6263 6c61  .r......issubcla
+00001910: 7373 7221 0000 00da 1167 6574 5f66 6965  ssr!.....get_fie
+00001920: 6c64 5f6f 7074 696f 6e73 da05 6669 656c  ld_options..fiel
+00001930: 6472 b900 0000 2904 7240 0000 0072 ab00  dr....).r@...r..
+00001940: 0000 72ac 0000 00da 016b 7237 0000 0072  ..r......kr7...r
+00001950: 5100 0000 7238 0000 0072 b000 0000 c800  Q...r8...r......
+00001960: 0000 7322 0000 000e 0108 0204 0106 0206  ..s"............
+00001970: fd0a 0418 0110 020a 0412 0214 0312 0110  ................
+00001980: 010c 0310 0110 0104 027a 1252 656e 6465  .........z.Rende
+00001990: 7265 722e 656c 656d 326a 736f 6e63 0100  rer.elem2jsonc..
+000019a0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000019b0: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
+000019c0: 024e 7a1e 7769 6e64 6f77 2e41 7070 2e64  .Nz.window.App.d
+000019d0: 6173 6862 6f61 7264 2e72 656c 6f61 6428  ashboard.reload(
+000019e0: 293b 7237 0000 0072 5100 0000 7237 0000  );r7...rQ...r7..
+000019f0: 0072 3700 0000 7238 0000 00da 0972 656c  .r7...r8.....rel
+00001a00: 6f61 645f 6a73 e800 0000 7302 0000 0004  oad_js....s.....
+00001a10: 017a 1252 656e 6465 7265 722e 7265 6c6f  .z.Renderer.relo
+00001a20: 6164 5f6a 7363 0200 0000 0000 0000 0000  ad_jsc..........
+00001a30: 0000 0600 0000 0400 0000 4f00 0000 73dc  ..........O...s.
+00001a40: 0000 007c 016a 006a 0164 016b 0272 0f7c  ...|.j.j.d.k.r.|
+00001a50: 006a 026a 037c 0269 007c 03a4 018e 0153  .j.j.|.i.|.....S
+00001a60: 007c 01a0 04a1 007d 047c 03a0 057c 0464  .|.....}.|...|.d
+00001a70: 0219 00a1 0101 0074 067c 037c 0183 0201  .......t.|.|....
+00001a80: 007c 016a 0764 0375 0172 2c7c 03a0 0874  .|.j.d.u.r,|...t
+00001a90: 096a 0a7c 016a 07a1 0201 007c 016a 0b64  .j.|.j.....|.j.d
+00001aa0: 0375 0172 397c 03a0 0874 096a 0c7c 016a  .u.r9|...t.j.|.j
+00001ab0: 0ba1 0201 007c 016a 0d64 0375 0172 5c7c  .....|.j.d.u.r\|
+00001ac0: 016a 0d64 0419 007d 057c 05a0 0e64 05a1  .j.d...}.|...d..
+00001ad0: 0172 557c 0564 0664 0385 0219 007d 057c  .rU|.d.d.....}.|
+00001ae0: 03a0 0874 096a 0f64 07a1 0201 007c 03a0  ...t.j.d.....|..
+00001af0: 0874 096a 107c 05a1 0201 007c 006a 026a  .t.j.|.....|.j.j
+00001b00: 037c 016a 006a 117c 016a 006a 0167 027c  .|.j.j.|.j.j.g.|
+00001b10: 02a2 0152 0069 007c 03a4 018e 0153 0029  ...R.i.|.....S.)
+00001b20: 087a 2055 7365 6420 666f 7220 7475 726e  .z Used for turn
+00001b30: 2072 6571 7565 7374 7320 696e 746f 2075   requests into u
+00001b40: 726c 73da 044d 6169 6eda 0b62 6173 655f  rls..Main..base_
+00001b50: 7061 7261 6d73 4e72 0100 0000 da01 2d72  paramsNr......-r
+00001b60: 2d00 0000 da04 4445 5343 2912 729e 0000  -.....DESC).r...
+00001b70: 0072 ba00 0000 7241 0000 00da 0f62 7569  .r....rA.....bui
+00001b80: 6c64 5f70 6c61 696e 5f75 726c da0a 6765  ld_plain_url..ge
+00001b90: 745f 7374 6174 7573 727a 0000 0072 0800  t_statusrz...r..
+00001ba0: 0000 da06 6f66 6673 6574 da0a 7365 7464  ....offset..setd
+00001bb0: 6566 6175 6c74 720c 0000 00da 0f55 524c  efaultr......URL
+00001bc0: 5f50 4152 414d 5f53 5441 5254 da05 6c69  _PARAM_START..li
+00001bd0: 6d69 74da 0f55 524c 5f50 4152 414d 5f4c  mit..URL_PARAM_L
+00001be0: 494d 4954 da08 6f72 6465 725f 6279 da0a  IMIT..order_by..
+00001bf0: 7374 6172 7473 7769 7468 da11 5552 4c5f  startswith..URL_
+00001c00: 5041 5241 4d5f 534f 5254 4449 52da 0e55  PARAM_SORTDIR..U
+00001c10: 524c 5f50 4152 414d 5f53 4f52 54da 0961  RL_PARAM_SORT..a
+00001c20: 7070 5f6c 6162 656c 2906 7240 0000 00da  pp_label).r@....
+00001c30: 0261 72da 0461 7267 73da 026b 77da 0273  .ar..args..kw..s
+00001c40: 74da 0273 6372 3700 0000 7237 0000 0072  t..scr7...r7...r
+00001c50: 3800 0000 da0f 6765 745f 7265 7175 6573  8.....get_reques
+00001c60: 745f 7572 6ceb 0000 0073 2c00 0000 0c02  t_url....s,.....
+00001c70: 1201 0802 0e01 0a01 0a01 1001 0a01 1001  ................
+00001c80: 0a01 0a01 0a01 0c01 0e01 0e01 0603 0c01  ................
+00001c90: 02ff 0201 06ff 0201 06ff 7a18 5265 6e64  ..........z.Rend
+00001ca0: 6572 6572 2e67 6574 5f72 6571 7565 7374  erer.get_request
+00001cb0: 5f75 726c 4e63 0500 0000 0000 0000 0000  _urlNc..........
+00001cc0: 0000 0700 0000 0500 0000 4b00 0000 73ae  ..........K...s.
+00001cd0: 0000 007c 0470 057c 03a0 00a1 007d 0474  ...|.p.|.....}.t
+00001ce0: 017c 0483 0164 016b 0272 1164 02a0 027c  .|...d.k.r.d...|
+00001cf0: 04a1 017d 047c 036a 036a 0472 2c7c 036a  ...}.|.j.j.r,|.j
+00001d00: 036a 0573 2c7c 00a0 067c 027c 037c 01a1  .j.s,|...|.|.|..
+00001d10: 037d 067c 006a 077c 027c 037c 067c 0466  .}.|.j.|.|.|.|.f
+00001d20: 0469 007c 05a4 018e 0153 007c 036a 036a  .i.|.....S.|.j.j
+00001d30: 0872 4b7c 02a0 09a1 007d 067c 0164 0075  .rK|.....}.|.d.u
+00001d40: 0172 3f7c 066a 0a7c 016a 0b64 038d 0101  .r?|.j.|.j.d....
+00001d50: 007c 006a 077c 027c 037c 067c 0466 0469  .|.j.|.|.|.|.f.i
+00001d60: 007c 05a4 018e 0153 007c 006a 0c7c 017c  .|.....S.|.j.|.|
+00001d70: 027c 037c 0466 0469 007c 05a4 018e 0153  .|.|.f.i.|.....S
+00001d80: 0029 044e 722d 0000 0075 0600 0000 c2a0  .).Nr-...u......
+00001d90: 7b7d c2a0 2901 da09 7265 636f 7264 5f69  {}..)...record_i
+00001da0: 6429 0dda 1067 6574 5f62 7574 746f 6e5f  d)...get_button_
+00001db0: 6c61 6265 6cda 036c 656e da06 666f 726d  label..len..form
+00001dc0: 6174 726f 0000 00da 0a70 6172 616d 6574  atro.....paramet
+00001dd0: 6572 73da 106e 6f5f 7061 7261 6d73 5f77  ers..no_params_w
+00001de0: 696e 646f 77da 1167 6574 5f61 6374 696f  indow..get_actio
+00001df0: 6e5f 7374 6174 7573 da14 7769 6e64 6f77  n_status..window
+00001e00: 5f61 6374 696f 6e5f 6275 7474 6f6e da0e  _action_button..
+00001e10: 6f70 656e 735f 615f 7769 6e64 6f77 72c5  opens_a_windowr.
+00001e20: 0000 0072 7a00 0000 da02 706b da11 726f  ...rz.....pk..ro
+00001e30: 775f 6163 7469 6f6e 5f62 7574 746f 6e29  w_action_button)
+00001e40: 0772 4000 0000 da03 6f62 6a72 d000 0000  .r@.....objr....
+00001e50: 7295 0000 0072 9b00 0000 72d2 0000 0072  r....r....r....r
+00001e60: d300 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
+00001e70: 0000 00da 0d61 6374 696f 6e5f 6275 7474  .....action_butt
+00001e80: 6f6e 0301 0000 7320 0000 000c 010c 010a  on....s ........
+00001e90: 0110 020e 0104 0108 0104 ff02 0106 ff08  ................
+00001ea0: 0208 0108 010e 0118 0118 017a 1652 656e  ...........z.Ren
+00001eb0: 6465 7265 722e 6163 7469 6f6e 5f62 7574  derer.action_but
+00001ec0: 746f 6e63 0500 0000 0000 0000 0000 0000  tonc............
+00001ed0: 0700 0000 0400 0000 4b00 0000 7340 0000  ........K...s@..
+00001ee0: 007c 0264 0175 0072 0d7c 036a 0064 0269  .|.d.u.r.|.j.d.i
+00001ef0: 007c 04a4 018e 017d 066e 097c 026a 017c  .|.....}.n.|.j.|
+00001f00: 0366 0169 007c 04a4 018e 017d 067c 006a  .f.i.|.....}.|.j
+00001f10: 027c 067c 0166 0269 007c 05a4 018e 0153  .|.|.f.i.|.....S
+00001f20: 0029 0361 cf01 0000 4e6f 7465 2074 6861  .).a....Note tha
+00001f30: 7420 6062 612e 6163 746f 7260 206d 6179  t `ba.actor` may
+00001f40: 2064 6966 6665 7220 6672 6f6d 2060 6172   differ from `ar
+00001f50: 2e61 6374 6f72 6020 7768 656e 2064 6566  .actor` when def
+00001f60: 696e 6564 206f 6e20 610a 2020 2020 2020  ined on a.      
+00001f70: 2020 6469 6666 6572 656e 7420 6163 746f    different acto
+00001f80: 722e 2052 656d 656d 6265 7220 652e 672e  r. Remember e.g.
+00001f90: 2074 6865 2022 4d75 7374 2072 6561 6420   the "Must read 
+00001fa0: 6549 4420 6361 7264 2220 6163 7469 6f6e  eID card" action
+00001fb0: 0a20 2020 2020 2020 2062 7574 746f 6e20  .        button 
+00001fc0: 696e 2065 6964 5f69 6e66 6f20 6f66 206e  in eid_info of n
+00001fd0: 6577 636f 6d65 7273 2e4e 6577 436c 6965  ewcomers.NewClie
+00001fe0: 6e74 7320 2832 3031 3430 3432 3229 2e0a  nts (20140422)..
+00001ff0: 0a20 2020 2020 2020 203a 6f62 6a3a 2020  .        :obj:  
+00002000: 5468 6520 6461 7461 6261 7365 206f 626a  The database obj
+00002010: 6563 740a 2020 2020 2020 2020 3a61 723a  ect.        :ar:
+00002020: 2020 2054 6865 2061 6374 696f 6e20 7265     The action re
+00002030: 7175 6573 740a 2020 2020 2020 2020 3a62  quest.        :b
+00002040: 613a 2020 5468 6520 626f 756e 6420 6163  a:  The bound ac
+00002050: 7469 6f6e 0a20 2020 2020 2020 203a 7265  tion.        :re
+00002060: 7175 6573 745f 6b77 6172 6773 3a20 6b65  quest_kwargs: ke
+00002070: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00002080: 746f 2066 6f72 7761 7264 6564 2074 6f20  to forwarded to 
+00002090: 7468 6520 6368 696c 6420 6163 7469 6f6e  the child action
+000020a0: 2072 6571 7565 7374 0a0a 2020 2020 2020   request..      
+000020b0: 2020 416e 7920 6b65 7977 6f72 6420 6f74    Any keyword ot
+000020c0: 6865 7220 6172 6775 6d65 6e74 7320 6172  her arguments ar
+000020d0: 6520 666f 7277 6172 6465 6420 746f 203a  e forwarded to :
+000020e0: 6d65 7468 3a60 6172 326a 7360 2e0a 0a20  meth:`ar2js`... 
+000020f0: 2020 2020 2020 204e 7237 0000 0029 03da         Nr7...)..
+00002100: 0772 6571 7565 7374 da05 7370 6177 6eda  .request..spawn.
+00002110: 0561 7232 6a73 2907 7240 0000 0072 e100  .ar2js).r@...r..
+00002120: 0000 72d0 0000 0072 9500 0000 da0e 7265  ..r....r......re
+00002130: 7175 6573 745f 6b77 6172 6773 da06 7374  quest_kwargs..st
+00002140: 6174 7573 da03 7361 7272 3700 0000 7237  atus..sarr7...r7
+00002150: 0000 0072 3800 0000 da17 6163 7469 6f6e  ...r8.....action
+00002160: 5f63 616c 6c5f 6f6e 5f69 6e73 7461 6e63  _call_on_instanc
+00002170: 6514 0100 0073 0800 0000 080e 1201 1203  e....s..........
+00002180: 1401 7a20 5265 6e64 6572 6572 2e61 6374  ..z Renderer.act
+00002190: 696f 6e5f 6361 6c6c 5f6f 6e5f 696e 7374  ion_call_on_inst
+000021a0: 616e 6365 6302 0000 0000 0000 0000 0000  ancec...........
+000021b0: 0004 0000 0004 0000 0043 0000 0073 2c00  .........C...s,.
+000021c0: 0000 7c01 6a00 7005 7c01 6a01 7d02 7402  ..|.j.p.|.j.}.t.
+000021d0: a003 7c02 6401 a102 7d03 7c03 6401 7500  ..|.d...}.|.d.u.
+000021e0: 7212 6401 5300 6402 7c03 1600 5300 2903  r.d.S.d.|...S.).
+000021f0: 7abf 0a20 2020 2020 2020 2055 7365 7320  z..        Uses 
+00002200: 616e 2069 6e74 6572 6e61 6c20 6d61 7070  an internal mapp
+00002210: 696e 6720 666f 7220 6963 6f6e 206e 616d  ing for icon nam
+00002220: 6573 2074 6f20 636f 6e76 6572 7420 6578  es to convert ex
+00002230: 6973 7469 6e67 2069 636f 6e73 2069 6e74  isting icons int
+00002240: 6f20 7265 6163 742d 7573 6162 6c65 2e0a  o react-usable..
+00002250: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+00002260: 6374 696f 6e3a 0a20 2020 2020 2020 203a  ction:.        :
+00002270: 7265 7475 726e 3a20 7374 723a 2061 2069  return: str: a i
+00002280: 636f 6e20 6e61 6d65 2066 6f72 2065 6974  con name for eit
+00002290: 6865 7220 7072 696d 652d 7265 6163 7420  her prime-react 
+000022a0: 6f72 2069 636f 6e38 0a20 2020 2020 2020  or icon8.       
+000022b0: 204e 7a05 7069 2025 7329 04da 0f72 6561   Nz.pi %s)...rea
+000022c0: 6374 5f69 636f 6e5f 6e61 6d65 da09 6963  ct_icon_name..ic
+000022d0: 6f6e 5f6e 616d 6572 2e00 0000 da03 6765  on_namer......ge
+000022e0: 7429 0472 4000 0000 726f 0000 0072 a500  t).r@...ro...r..
+000022f0: 0000 da0a 7265 6163 745f 6963 6f6e 7237  ....react_iconr7
+00002300: 0000 0072 3700 0000 7238 0000 0072 aa00  ...r7...r8...r..
+00002310: 0000 2901 0000 730a 0000 000c 070c 0108  ..)...s.........
+00002320: 0104 0108 027a 1852 656e 6465 7265 722e  .....z.Renderer.
+00002330: 6765 745f 6163 7469 6f6e 5f69 636f 6e63  get_action_iconc
+00002340: 0300 0000 0000 0000 0000 0000 0800 0000  ................
+00002350: 0700 0000 4b00 0000 73a4 0000 007c 016a  ....K...s....|.j
+00002360: 007d 047c 016a 017d 0569 007d 067c 056a  .}.|.j.}.i.}.|.j
+00002370: 02a0 03a1 0072 1c7c 03a0 047c 00a0 057c  .....r.|...|...|
+00002380: 017c 057c 02a1 03a1 0101 007c 06a0 047c  .|.|.......|...|
+00002390: 03a1 0101 007c 06a0 047c 00a0 067c 017c  .....|...|...|.|
+000023a0: 057c 02a1 03a1 0101 007c 06a0 047c 03a1  .|.......|...|..
+000023b0: 0101 007c 047c 056a 026a 077c 016a 087c  ...|.|.j.j.|.j.|
+000023c0: 056a 096a 0a7c 0664 019c 057d 0774 0b7c  .j.j.|.d...}.t.|
+000023d0: 0264 0283 0272 437c 026a 0c7c 0764 033c  .d...rC|.j.|.d.<
+000023e0: 006e 0974 0d7c 0274 0e83 0272 4c7c 027c  .n.t.|.t...rL|.|
+000023f0: 0764 033c 0064 0474 0f7c 0783 0116 0053  .d.<.d.t.|.....S
+00002400: 0029 057a 4349 6d70 6c65 6d65 6e74 7320  .).zCImplements 
+00002410: 3a6d 6574 683a 606c 696e 6f2e 636f 7265  :meth:`lino.core
+00002420: 2e72 656e 6465 7265 722e 4874 6d6c 5265  .renderer.HtmlRe
+00002430: 6e64 6572 6572 2e61 7232 6a73 602e 0a0a  nderer.ar2js`...
+00002440: 2020 2020 2020 2020 2905 da02 7270 729a          )...rpr.
+00002450: 0000 00da 066f 6e4d 6169 6eda 0761 6374  .....onMain..act
+00002460: 6f72 4964 72e7 0000 0072 df00 0000 da02  orIdr....r......
+00002470: 7372 fa18 7769 6e64 6f77 2e41 7070 2e72  sr..window.App.r
+00002480: 756e 4163 7469 6f6e 2825 7329 2910 da10  unAction(%s))...
+00002490: 7265 7175 6573 7469 6e67 5f70 616e 656c  requesting_panel
+000024a0: 72a9 0000 0072 6f00 0000 72a8 0000 0072  r....ro...r....r
+000024b0: 7a00 0000 72dc 0000 00da 1167 6574 5f61  z...r......get_a
+000024c0: 6374 696f 6e5f 7061 7261 6d73 724e 0000  ction_paramsrN..
+000024d0: 00da 1069 735f 6f6e 5f6d 6169 6e5f 6163  ...is_on_main_ac
+000024e0: 746f 7272 9e00 0000 da08 6163 746f 725f  torr......actor_
+000024f0: 6964 7286 0000 0072 df00 0000 72a6 0000  idr....r....r...
+00002500: 0072 7b00 0000 7226 0000 0029 0872 4000  .r{...r&...).r@.
+00002510: 0000 72d0 0000 0072 e100 0000 72e7 0000  ..r....r....r...
+00002520: 0072 ee00 0000 7295 0000 00da 0670 6172  .r....r......par
+00002530: 616d 73da 066a 735f 6f62 6a72 3700 0000  ams..js_objr7...
+00002540: 7237 0000 0072 3800 0000 72e5 0000 0037  r7...r8...r....7
+00002550: 0100 0073 2a00 0000 0604 0601 0401 0a01  ...s*...........
+00002560: 1404 0a01 1401 0a01 0203 0601 0401 0601  ................
+00002570: 0201 06fb 0a07 0c01 0a02 0801 0202 0601  ................
+00002580: 04ff 7a0e 5265 6e64 6572 6572 2e61 7232  ..z.Renderer.ar2
+00002590: 6a73 6302 0000 0000 0000 0000 0000 0006  jsc.............
+000025a0: 0000 0006 0000 0043 0000 0073 bc01 0000  .......C...s....
+000025b0: 7c01 7400 6a01 6a02 7500 720a 7403 6401  |.t.j.j.u.r.t.d.
+000025c0: 8301 5300 7404 7c01 7405 8302 7216 7406  ..S.t.|.t...r.t.
+000025d0: 6402 a007 7c01 a101 8301 8201 7404 7c01  d...|.......t.|.
+000025e0: 7408 6a09 8302 7220 0900 7c01 6a0a 5300  t.j...r ..|.j.S.
+000025f0: 7404 7c01 740b 6a0c 8302 7229 7c01 6a0d  t.|.t.j...r)|.j.
+00002600: 5300 7404 7c01 7406 8302 7232 740e 7c01  S.t.|.t...r2t.|.
+00002610: 8301 5300 7404 7c01 740f 8302 724a 7c01  ..S.t.|.t...rJ|.
+00002620: 6a10 6403 7500 723f 7c01 6a11 5300 7412  j.d.u.r?|.j.S.t.
+00002630: 7c01 6a13 7412 7c01 6a11 6404 8d01 6405  |.j.t.|.j.d...d.
+00002640: 8d02 5300 7404 7c01 7414 8302 72cc 7c01  ..S.t.|.t...r.|.
+00002650: 6a15 6403 7501 726d 7c00 a016 6403 7c01  j.d.u.rm|...d.|.
+00002660: 6a15 6403 a103 7d02 7c02 6403 7501 7362  j.d...}.|.d.u.sb
+00002670: 4a00 8201 6406 7c02 1600 7d03 7c00 a017  J...d.|...}.|...
+00002680: 7c01 7c02 6403 a103 5300 7c01 6a18 6403  |.|.d...S.|.j.d.
+00002690: 7501 7295 7c01 6a19 7285 7c01 6a18 6a1a  u.r.|.j.r.|.j.j.
+000026a0: 640d 6900 7c01 6a19 a401 8e01 7d04 7c00  d.i.|.j.....}.|.
+000026b0: a01b 7c04 a101 7d03 6e08 7c00 a01c 6403  ..|...}.n.|...d.
+000026c0: 7c01 6a18 6900 a103 7d03 7c00 a017 7c01  |.j.i...}.|...|.
+000026d0: 7c03 7c01 6a1d a103 5300 7c01 6a1e 6403  |.|.j...S.|.j.d.
+000026e0: 7501 72a7 6406 7c01 6a1e 1600 7d03 7c00  u.r.d.|.j...}.|.
+000026f0: a017 7c01 7c03 7c01 6a1d a103 5300 7c01  ..|.|.|.j...S.|.
+00002700: 6a1f 6403 7501 72b0 7c01 6a1f 7d05 6e03  j.d.u.r.|.j.}.n.
+00002710: 7c01 6a13 5300 7c01 6a10 6a10 6403 7500  |.j.S.|.j.j.d.u.
+00002720: 72c5 7412 6407 7c01 6a13 7403 6408 7c05  r.t.d.|.j.t.d.|.
+00002730: 1600 8301 6409 8d03 5300 7412 7c01 6a13  ....d...S.t.|.j.
+00002740: 7c05 640a 8d02 5300 7404 7c01 7403 8302  |.d...S.t.|.t...
+00002750: 72dc 7420 7c00 640b 640c 8303 72dc 740e  r.t |.d.d...r.t.
+00002760: 7c01 6a21 8301 5300 7c01 5300 290e 7a54  |.j!..S.|.S.).zT
+00002770: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
+00002780: 6e61 6c20 636f 6e76 6572 7469 6e67 206c  nal converting l
+00002790: 6f67 6963 2066 6f72 2073 6572 6961 6c69  ogic for seriali
+000027a0: 7a69 6e67 2050 7974 686f 6e20 7661 6c75  zing Python valu
+000027b0: 6573 2074 6f20 6a73 6f6e 2e0a 2020 2020  es to json..    
+000027c0: 2020 2020 da10 4c41 4e47 5541 4745 5f43      ..LANGUAGE_C
+000027d0: 484f 4943 4553 7a0b 3230 3231 3035 3137  HOICESz.20210517
+000027e0: 207b 7d4e 2901 726b 0000 0029 0272 4500   {}N).rk...).rE.
+000027f0: 0000 7256 0000 007a 0225 73da 0662 7574  ..rV...z.%s..but
+00002800: 746f 6e7a 2366 756e 6374 696f 6e28 2920  tonz#function() 
+00002810: 7b20 4c69 6e6f 2e6c 6f61 645f 7572 6c28  { Lino.load_url(
+00002820: 2725 7327 293b 207d 2903 da05 7874 7970  '%s'); })...xtyp
+00002830: 6572 4500 0000 da07 6861 6e64 6c65 7229  erE.....handler)
+00002840: 0272 4500 0000 da04 6872 6566 7271 0000  .rE.....hrefrq..
+00002850: 0046 7237 0000 0029 2272 0400 0000 7272  .Fr7...)"r....rr
+00002860: 0000 0072 f900 0000 7227 0000 0072 a600  ...r....r'...r..
+00002870: 0000 721c 0000 00da 0945 7863 6570 7469  ..r......Excepti
+00002880: 6f6e 72d9 0000 0072 0d00 0000 da06 4368  onr....r......Ch
+00002890: 6f69 6365 7244 0000 0072 0500 0000 da05  oicerD...r......
+000028a0: 4d6f 6465 6c72 df00 0000 7246 0000 0072  Modelr....rF...r
+000028b0: 0a00 0000 da06 7061 7265 6e74 726b 0000  ......parentrk..
+000028c0: 0072 7400 0000 729b 0000 0072 0b00 0000  .rt...r....r....
+000028d0: da08 696e 7374 616e 6365 da10 696e 7374  ..instance..inst
+000028e0: 616e 6365 5f68 616e 646c 6572 da0c 6861  ance_handler..ha
+000028f0: 6e64 6c65 725f 6974 656d 72a9 0000 0072  ndler_itemr....r
+00002900: f700 0000 72e3 0000 00da 0f72 6571 7565  ....r......reque
+00002910: 7374 5f68 616e 646c 6572 da0b 6163 7469  st_handler..acti
+00002920: 6f6e 5f63 616c 6c72 b900 0000 da0a 6a61  on_callr......ja
+00002930: 7661 7363 7269 7074 72fd 0000 00da 0767  vascriptr......g
+00002940: 6574 6174 7472 da01 7329 0672 4000 0000  etattr..s).r@...
+00002950: 72ab 0000 00da 0168 da02 6a73 72d0 0000  r......h..jsr...
+00002960: 00da 0375 726c 7237 0000 0072 3700 0000  ...urlr7...r7...
+00002970: 7238 0000 0072 3f00 0000 5801 0000 7354  r8...r?...X...sT
+00002980: 0000 000c 0408 010a 010e 010c 0102 0106  ................
+00002990: 030c 0106 010a 0108 010a 010a 0106 0116  ................
+000029a0: 030a 020a 0110 010c 0108 010e 010a 0106  ................
+000029b0: 0114 010c 0110 0210 010a 020a 0110 010a  ................
+000029c0: 0108 0106 070c 0202 0206 010a 0206 fd0e  ................
+000029d0: 0416 020a 0204 027a 1852 656e 6465 7265  .......z.Rendere
+000029e0: 722e 7079 326a 735f 636f 6e76 6572 7465  r.py2js_converte
+000029f0: 7263 0400 0000 0000 0000 0000 0000 0500  rc..............
+00002a00: 0000 0400 0000 4300 0000 7350 0000 0074  ......C...sP...t
+00002a10: 007c 016a 017c 0264 018d 027d 047c 016a  .|.j.|.d...}.|.j
+00002a20: 0272 1a7c 016a 026a 036a 0472 1a7c 046a  .r.|.j.j.j.r.|.j
+00002a30: 0564 027c 016a 026a 036a 0417 0064 038d  .d.|.j.j.j...d..
+00002a40: 0101 0074 066a 076a 0872 267c 0372 267c  ...t.j.j.r&|.r&|
+00002a50: 046a 057c 0364 048d 0101 007c 0453 0029  .j.|.d.....|.S.)
+00002a60: 05da 0029 0272 4500 0000 72fc 0000 007a  ...).rE...r....z
+00002a70: 0778 2d74 6261 722d 2901 da07 6963 6f6e  .x-tbar-)...icon
+00002a80: 436c 7329 01da 0774 6f6f 6c54 6970 2909  Cls)...toolTip).
+00002a90: 7274 0000 0072 9b00 0000 72a9 0000 0072  rt...r....r....r
+00002aa0: 6f00 0000 72eb 0000 0072 7a00 0000 7204  o...r....rz...r.
+00002ab0: 0000 0072 7200 0000 da0d 7573 655f 7175  ...rr.....use_qu
+00002ac0: 6963 6b74 6970 7329 0572 4000 0000 da02  icktips).r@.....
+00002ad0: 6d69 72fc 0000 0072 b900 0000 da01 6472  mir....r......dr
+00002ae0: 3700 0000 7237 0000 0072 3800 0000 7204  7...r7...r8...r.
+00002af0: 0100 00a6 0100 0073 0c00 0000 0e04 1001  .......s........
+00002b00: 1601 0c01 0c03 0401 7a15 5265 6e64 6572  ........z.Render
+00002b10: 6572 2e68 616e 646c 6572 5f69 7465 6d63  er.handler_itemc
+00002b20: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00002b30: 0500 0000 4f00 0000 7320 0000 007c 016a  ....O...s ...|.j
+00002b40: 0064 0269 007c 03a4 018e 017d 047c 00a0  .d.i.|.....}.|..
+00002b50: 017c 017c 016a 027c 04a1 0353 0029 037a  .|.|.j.|...S.).z
+00002b60: 3620 4765 6e65 7261 7465 7320 6a73 2073  6 Generates js s
+00002b70: 7472 696e 6720 666f 7220 6163 7469 6f6e  tring for action
+00002b80: 2062 7574 746f 6e20 6361 6c6c 732e 0a20   button calls.. 
+00002b90: 2020 2020 2020 204e 7237 0000 0029 0372         Nr7...).r
+00002ba0: c500 0000 7206 0100 0072 a900 0000 2905  ....r....r....).
+00002bb0: 7240 0000 0072 d000 0000 72d1 0000 0072  r@...r....r....r
+00002bc0: d200 0000 72d3 0000 0072 3700 0000 7237  ....r....r7...r7
+00002bd0: 0000 0072 3800 0000 7205 0100 00b4 0100  ...r8...r.......
+00002be0: 0073 0400 0000 1004 1001 7a18 5265 6e64  .s........z.Rend
+00002bf0: 6572 6572 2e72 6571 7565 7374 5f68 616e  erer.request_han
+00002c00: 646c 6572 6304 0000 0000 0000 0000 0000  dlerc...........
+00002c10: 0008 0000 0008 0000 0043 0000 0073 9c00  .........C...s..
+00002c20: 0000 7c02 6a00 7d04 7c02 a001 a100 a002  ..|.j.}.|.......
+00002c30: 6401 6402 a102 5c02 7d05 7d06 7c03 7311  d.d...\.}.}.|.s.
+00002c40: 6900 7d03 7c01 6400 7501 7222 7403 7c01  i.}.|.d.u.r"t.|.
+00002c50: 6403 8302 7222 7c01 6a04 6408 6900 7c03  d...r"|.j.d.i.|.
+00002c60: a401 8e01 7d03 7c01 722d 7c01 6a05 722d  ....}.|.r-|.j.r-
+00002c70: 7c01 6a05 7c03 7406 6a07 3c00 7c06 6404  |.j.|.t.j.<.|.d.
+00002c80: 6b02 7239 7403 7c03 6405 8302 7239 7c03  k.r9t.|.d...r9|.
+00002c90: 6405 3d00 7c01 6400 7500 723f 6400 6e02  d.=.|.d.u.r?d.n.
+00002ca0: 7c01 6a08 7d07 6406 7409 740a 7c06 7c05  |.j.}.d.t.t.|.|.
+00002cb0: 7c03 7c07 6407 8d04 8301 1600 5300 2909  |.|.d.......S.).
+00002cc0: 4eda 012e 722d 0000 0072 c500 0000 da04  N...r-...r......
+00002cd0: 6772 6964 72d6 0000 0072 f200 0000 2904  gridr....r....).
+00002ce0: 729a 0000 0072 f000 0000 72e7 0000 0072  r....r....r....r
+00002cf0: ee00 0000 7237 0000 0029 0b72 6f00 0000  ....r7...).ro...
+00002d00: da09 6675 6c6c 5f6e 616d 65da 0672 7370  ..full_name..rsp
+00002d10: 6c69 7472 8600 0000 72c5 0000 00da 0a73  litr....r......s
+00002d20: 7562 7374 5f75 7365 7272 0c00 0000 da14  ubst_userr......
+00002d30: 5552 4c5f 5041 5241 4d5f 5355 4253 545f  URL_PARAM_SUBST_
+00002d40: 5553 4552 72f3 0000 0072 2600 0000 7274  USERr....r&...rt
+00002d50: 0000 0029 0872 4000 0000 72d0 0000 0072  ...).r@...r....r
+00002d60: a900 0000 72e7 0000 0072 5000 0000 72f0  ....r....rP...r.
+00002d70: 0000 0072 9a00 0000 72ee 0000 0072 3700  ...r....r....r7.
+00002d80: 0000 7237 0000 0072 3800 0000 7206 0100  ..r7...r8...r...
+00002d90: 00be 0100 0073 2200 0000 0602 1402 0402  .....s".........
+00002da0: 0401 1202 1001 0a02 0c01 1211 0601 1202  ................
+00002db0: 0602 0201 0201 0201 0201 0afc 7a14 5265  ............z.Re
+00002dc0: 6e64 6572 6572 2e61 6374 696f 6e5f 6361  nderer.action_ca
+00002dd0: 6c6c 6302 0000 0000 0000 0000 0000 0002  llc.............
+00002de0: 0000 0004 0000 0043 0000 0073 2e00 0000  .......C...s....
+00002df0: 7c01 7304 6400 5300 7400 7c01 7401 8302  |.s.d.S.t.|.t...
+00002e00: 730d 7401 7c01 8301 7d01 7402 7c01 6401  s.t.|...}.t.|.d.
+00002e10: 6402 8d02 7d01 6403 7c01 1700 5300 2904  d...}.d.|...S.).
+00002e20: 4e46 2901 da05 7175 6f74 657a 0b6a 6176  NF)...quotez.jav
+00002e30: 6173 6372 6970 743a 2903 72a6 0000 0072  ascript:).r....r
+00002e40: 4600 0000 7203 0000 0029 0272 4000 0000  F...r....).r@...
+00002e50: 720b 0100 0072 3700 0000 7237 0000 0072  r....r7...r7...r
+00002e60: 3800 0000 da06 6a73 3275 726c e801 0000  8.....js2url....
+00002e70: 730c 0000 0004 0104 010a 0208 010c 0108  s...............
+00002e80: 017a 0f52 656e 6465 7265 722e 6a73 3275  .z.Renderer.js2u
+00002e90: 726c 6306 0000 0000 0000 0000 0000 0007  rlc.............
+00002ea0: 0000 0004 0000 0043 0000 0073 5600 0000  .......C...sV...
+00002eb0: 7400 6a01 6a02 7227 7400 6a01 6a03 720f  t.j.j.r't.j.j.r.
+00002ec0: 6401 7c04 7c05 6602 1600 7d06 6e02 6402  d.|.|.f...}.n.d.
+00002ed0: 7d06 7c02 7219 7404 6403 7c06 7c02 8303  }.|.r.t.d.|.|...
+00002ee0: 7d06 7c06 7229 7c01 6a05 6404 7c03 7c06  }.|.r)|.j.d.|.|.
+00002ef0: 6602 1600 6405 8d01 0100 6400 5300 6400  f...d.....d.S.d.
+00002f00: 5300 6400 5300 2906 4e7a 0828 2573 2e25  S.d.S.).Nz.(%s.%
+00002f10: 7329 2072 0d01 0000 7a04 7b7d 7b7d 7a07  s) r....z.{}{}z.
+00002f20: 2825 732c 2573 2929 01da 0871 7569 636b  (%s,%s))...quick
+00002f30: 7469 7029 0672 0400 0000 7272 0000 0072  tip).r....rr...r
+00002f40: 1001 0000 da19 7368 6f77 5f69 6e74 6572  ......show_inter
+00002f50: 6e61 6c5f 6669 656c 645f 6e61 6d65 7372  nal_field_namesr
+00002f60: 0600 0000 727a 0000 0029 0772 4000 0000  ....rz...).r@...
+00002f70: 72d2 0000 0072 b900 0000 7277 0000 00da  r....r....rw....
+00002f80: 0a64 6174 6173 6f75 7263 65da 0966 6965  .datasource..fie
+00002f90: 6c64 6e61 6d65 da03 7474 7472 3700 0000  ldname..tttr7...
+00002fa0: 7237 0000 0072 3800 0000 da0d 6164 645f  r7...r8.....add_
+00002fb0: 6865 6c70 5f74 6578 74f1 0100 0073 1800  help_text....s..
+00002fc0: 0000 0801 0801 0e01 0402 0401 0c01 0401  ................
+00002fd0: 0804 0201 0eff 04f5 0407 7a16 5265 6e64  ..........z.Rend
+00002fe0: 6572 6572 2e61 6464 5f68 656c 705f 7465  erer.add_help_te
+00002ff0: 7874 6302 0000 0000 0000 0000 0000 0005  xtc.............
+00003000: 0000 0003 0000 0043 0000 0073 5600 0000  .......C...sV...
+00003010: 7400 8300 7d02 6401 7c01 1700 6402 1700  t...}.d.|...d...
+00003020: 7d03 7c00 6a01 a002 6403 a101 6404 1900  }.|.j...d...d...
+00003030: 7d04 7c02 6405 7501 721c 7c03 7c02 6a03  }.|.d.u.r.|.|.j.
+00003040: 6402 1700 3700 7d03 7c03 7404 a005 a100  d...7.}.|.t.....
+00003050: 6403 1700 7c04 1700 3700 7d03 6406 7c04  d...|...7.}.d.|.
+00003060: 7c03 6603 5300 2907 7a2c 4c69 6b65 206c  |.f.S.).z,Like l
+00003070: 696e 6f5f 6a73 5f70 6172 7473 2c20 6275  ino_js_parts, bu
+00003080: 7420 666f 7220 6163 746f 725f 6c65 7665  t for actor_leve
+00003090: 6c20 6461 7461 da05 4c69 6e6f 5fda 015f  l data..Lino_.._
+000030a0: 7213 0100 0072 2f00 0000 4eda 0563 6163  r....r/...N..cac
+000030b0: 6865 2906 7229 0000 00da 116c 696e 6f5f  he).r).....lino_
+000030c0: 7765 625f 7465 6d70 6c61 7465 7216 0100  web_templater...
+000030d0: 0072 4400 0000 7207 0000 00da 0c67 6574  .rD...r......get
+000030e0: 5f6c 616e 6775 6167 6529 0572 4000 0000  _language).r@...
+000030f0: 72f0 0000 00da 0975 7365 725f 7479 7065  r......user_type
+00003100: da08 6669 6c65 6e61 6d65 da09 6669 6c65  ..filename..file
+00003110: 5f74 7970 6572 3700 0000 7237 0000 0072  _typer7...r7...r
+00003120: 3800 0000 da15 6c69 6e6f 5f6a 735f 7061  8.....lino_js_pa
+00003130: 7274 735f 6368 756e 6b65 6400 0200 0073  rts_chunked....s
+00003140: 0e00 0000 0602 0c01 1001 0801 0e01 1401  ................
+00003150: 0a01 7a1e 5265 6e64 6572 6572 2e6c 696e  ..z.Renderer.lin
+00003160: 6f5f 6a73 5f70 6172 7473 5f63 6875 6e6b  o_js_parts_chunk
+00003170: 6564 6302 0000 0000 0000 0000 0000 0011  edc.............
+00003180: 0000 0006 0000 0043 0000 0073 de01 0000  .......C...s....
+00003190: 6700 7d02 6700 7d03 7c01 4400 5de4 7d04  g.}.g.}.|.D.].}.
+000031a0: 7c04 a000 a100 7d05 7c05 7312 7c04 6a01  |.....}.|.s.|.j.
+000031b0: 6a02 72cc 7403 6a04 7c04 6a01 6a05 6901  j.r.t.j.|.j.j.i.
+000031c0: 7d06 7c05 7223 7c06 6a06 7c05 6a07 6a08  }.|.r#|.j.|.j.j.
+000031d0: 6401 8d01 0100 7c04 6a01 6a02 72c7 6700  d.....|.j.j.r.g.
+000031e0: 7d07 7409 8300 7d08 7c04 6a0a a00b 7c04  }.t...}.|.j...|.
+000031f0: 6a01 740c 8300 a102 4400 5d72 7d09 7409  j.t.....D.]r}.t.
+00003200: 7c09 6a01 6a05 6402 8d01 7d0a 7c09 6a01  |.j.j.d...}.|.j.
+00003210: 6a0d 7d0b 7c0b 7248 7c0b 7c0a 6403 3c00  j.}.|.rH|.|.d.<.
+00003220: 7c09 6a01 6a0e 7d0c 7c0c 725e 740f 7c0c  |.j.j.}.|.r^t.|.
+00003230: 8301 725a 7c0c 7c09 6a0a 8301 7c0a 6404  ..rZ|.|.j...|.d.
+00003240: 3c00 6e04 7c0c 7c0a 6404 3c00 7c09 6a01  <.n.|.|.d.<.|.j.
+00003250: 6a10 6405 7501 7284 7c09 6a01 6a10 7d0d  j.d.u.r.|.j.j.}.
+00003260: 7c0d 7c08 7600 7274 7c08 7c0d 1900 a011  |.|.v.rt|.|.....
+00003270: 7c0a a101 0100 6e15 7409 7c0d 6406 8d01  |.....n.t.|.d...
+00003280: 7d0e 7c0a 6701 7c08 7c0d 3c00 7c07 a011  }.|.g.|.|.<.|...
+00003290: 7c0e a101 0100 6e05 7c07 a011 7c0a a101  |.....n.|...|...
+000032a0: 0100 7c09 6a01 6a12 72a7 7413 7c09 6a01  ..|.j.j.r.t.|.j.
+000032b0: 6a12 8301 7d0f 7414 7c0f 6407 8302 739e  j...}.t.|.d...s.
+000032c0: 7c09 6a01 6a05 7c0f 6407 3c00 7c0f 7c03  |.j.j.|.d.<.|.|.
+000032d0: 7601 72a7 7c03 a011 7c0f a101 0100 7135  v.r.|...|.....q5
+000032e0: 7c08 72c3 7415 7c07 8301 4400 5d14 5c02  |.r.t.|...D.].\.
+000032f0: 7d10 7d0a 7c0a a016 6408 6409 a102 72c2  }.}.|...d.d...r.
+00003300: 7c08 7c0a 6408 1900 1900 7c07 7c10 1900  |.|.d.....|.|...
+00003310: 640a 3c00 71ae 7c07 7c06 640b 3c00 7c02  d.<.q.|.|.d.<.|.
+00003320: a011 7c06 a101 0100 7c04 6a01 6a12 72ea  ..|.....|.j.j.r.
+00003330: 7413 7c04 6a01 6a12 8301 7d0f 7414 7c0f  t.|.j.j...}.t.|.
+00003340: 6407 8302 73e1 7c04 6a01 6a05 7c0f 6407  d...s.|.j.j.|.d.
+00003350: 3c00 7c0f 7c03 7601 72ea 7c03 a011 7c0f  <.|.|.v.r.|...|.
+00003360: a101 0100 7106 7c02 7c03 6602 5300 290c  ....q.|.|.f.S.).
+00003370: 7a45 436f 6e76 6572 7473 206f 6620 616c  zEConverts of al
+00003380: 6c20 7468 6520 626f 756e 6461 6374 696f  l the boundactio
+00003390: 6e73 206f 6620 616e 2061 6374 6f72 2074  ns of an actor t
+000033a0: 6f20 6a73 6f6e 2066 6f72 6d61 742e 0a20  o json format.. 
+000033b0: 2020 2020 2020 20a9 0172 6500 0000 2901         ..re...).
+000033c0: 729a 0000 0072 b900 0000 da0a 6a73 5f68  r....r......js_h
+000033d0: 616e 646c 6572 4e29 01da 0563 6f6d 626f  andlerN)...combo
+000033e0: 7295 0000 0072 2c01 0000 4672 5600 0000  r....r,...FrV...
+000033f0: da0e 746f 6f6c 6261 7241 6374 696f 6e73  ..toolbarActions
+00003400: 2917 da11 6765 745f 6c61 796f 7574 5f68  )...get_layout_h
+00003410: 616e 6465 6c72 6f00 0000 da0b 7769 6e64  andelro.....wind
+00003420: 6f77 5f74 7970 6572 0c00 0000 da15 5552  ow_typer......UR
+00003430: 4c5f 5041 5241 4d5f 4143 5449 4f4e 5f4e  L_PARAM_ACTION_N
+00003440: 414d 4572 4e00 0000 727a 0000 0072 b100  AMErN...rz...r..
+00003450: 0000 728b 0000 0072 7400 0000 729e 0000  ..r....rt...r...
+00003460: 00da 1367 6574 5f74 6f6f 6c62 6172 5f61  ...get_toolbar_a
+00003470: 6374 696f 6e73 7229 0000 0072 b900 0000  ctionsr)...r....
+00003480: 722b 0100 0072 3000 0000 da0b 636f 6d62  r+...r0.....comb
+00003490: 6f5f 6772 6f75 70da 0661 7070 656e 64da  o_group..append.
+000034a0: 0668 6f74 6b65 79da 0476 6172 7372 8600  .hotkey..varsr..
+000034b0: 0000 7231 0000 0072 ec00 0000 2911 7240  ..r1...r....).r@
+000034c0: 0000 00da 0c61 6374 696f 6e73 5f6c 6973  .....actions_lis
+000034d0: 7472 ac00 0000 da07 686f 746b 6579 7372  tr......hotkeysr
+000034e0: 9500 0000 da02 6c68 da11 6163 7469 6f6e  ......lh..action
+000034f0: 5f64 6573 6372 6970 746f 72da 0474 6261  _descriptor..tba
+00003500: 73da 0963 6f6d 626f 5f6d 6170 7250 0000  s..combo_maprP..
+00003510: 00da 0374 6261 72b9 0000 0072 2b01 0000  ...tbar....r+...
+00003520: 7232 0100 0072 2c01 0000 7234 0100 0072  r2...r,...r4...r
+00003530: 3500 0000 7237 0000 0072 3700 0000 7238  5...r7...r7...r8
+00003540: 0000 00da 0c61 6374 696f 6e73 326a 736f  .....actions2jso
+00003550: 6e0a 0200 0073 6800 0000 0404 0401 0802  n....sh.........
+00003560: 0801 0c01 0e02 0401 1001 0801 0401 0601  ................
+00003570: 0602 0801 08ff 0e03 0801 0c01 0801 0401  ................
+00003580: 0801 1001 0802 0c02 0801 0802 1001 0a02  ................
+00003590: 0a01 0c01 0a02 0802 0c01 0a01 0c01 0801  ................
+000035a0: 0a01 0280 0402 1001 0c01 1401 0280 0802  ................
+000035b0: 0a02 0802 0c01 0a01 0c01 0801 0a01 0280  ................
+000035c0: 0802 7a15 5265 6e64 6572 6572 2e61 6374  ..z.Renderer.act
+000035d0: 696f 6e73 326a 736f 6e63 0200 0000 0000  ions2jsonc......
+000035e0: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+000035f0: 0000 7358 0000 0067 007d 0264 007d 037c  ..sX...g.}.d.}.|
+00003600: 0144 005d 147d 047c 0464 0119 0064 0075  .D.].}.|.d...d.u
+00003610: 0072 137c 0464 0219 007d 0371 067c 02a0  .r.|.d...}.q.|..
+00003620: 0074 017c 0483 01a1 0101 0071 0674 027c  .t.|.......q.t.|
+00003630: 0264 0364 0484 0064 058d 027d 027c 02a0  .d.d...d...}.|..
+00003640: 0064 007c 0367 02a1 0101 007c 0253 0029  .d.|.g.....|.S.)
+00003650: 064e 7201 0000 0072 2d00 0000 6301 0000  .Nr....r-...c...
+00003660: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003670: 0053 0000 0073 0800 0000 7c00 6401 1900  .S...s....|.d...
+00003680: 5300 2902 4e72 0100 0000 7237 0000 0029  S.).Nr....r7...)
+00003690: 0172 3600 0000 7237 0000 0072 3700 0000  .r6...r7...r7...
+000036a0: 7238 0000 00da 083c 6c61 6d62 6461 3e56  r8.....<lambda>V
+000036b0: 0200 0073 0200 0000 0800 7a2c 5265 6e64  ...s......z,Rend
+000036c0: 6572 6572 2e64 6973 706c 6179 5f6d 6f64  erer.display_mod
+000036d0: 6532 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  e2json.<locals>.
+000036e0: 3c6c 616d 6264 613e a901 7234 0000 0029  <lambda>..r4...)
+000036f0: 0372 3301 0000 727b 0000 00da 0673 6f72  .r3...r{.....sor
+00003700: 7465 6429 0572 4000 0000 da0c 6469 7370  ted).r@.....disp
+00003710: 6c61 795f 6d6f 6465 da03 646d 73da 0364  lay_mode..dms..d
+00003720: 6d64 7298 0000 0072 3700 0000 7237 0000  mdr....r7...r7..
+00003730: 0072 3800 0000 da11 6469 7370 6c61 795f  .r8.....display_
+00003740: 6d6f 6465 326a 736f 6e4e 0200 0073 1200  mode2jsonN...s..
+00003750: 0000 0401 0401 0801 0c01 0a01 1002 1001  ................
+00003760: 0e01 0401 7a1a 5265 6e64 6572 6572 2e64  ....z.Renderer.d
+00003770: 6973 706c 6179 5f6d 6f64 6532 6a73 6f6e  isplay_mode2json
+00003780: 6302 0000 0000 0000 0000 0000 0011 0000  c...............
+00003790: 0008 0000 0043 0000 0073 2203 0000 7400  .....C...s"...t.
+000037a0: 7c01 8301 7209 7401 7c01 7402 8302 730b  |...r.t.|.t...s.
+000037b0: 4a00 8201 7c00 a003 7c01 6a04 a101 5c02  J...|...|.j...\.
+000037c0: 7d02 7d03 7405 7c01 6a06 7c02 7c01 a007  }.}.t.|.j.|.|...
+000037d0: a100 7408 7c01 6a09 8301 7c01 a00a 740b  ..t.|.j...|...t.
+000037e0: 8300 a101 0c00 6401 8d05 7d04 740c 7c03  ......d...}.t.|.
+000037f0: 8301 7231 7c04 6a0d 7c03 6402 8d01 0100  ..r1|.j.|.d.....
+00003800: 7c01 a00e a100 7d05 7c05 6a0f 6400 7500  |.....}.|.j.d.u.
+00003810: 7243 7410 6a11 6a12 a013 6403 7c01 a102  rCt.j.j...d.|...
+00003820: 0100 6e5d 7414 7c05 6404 8302 7297 6700  ..n]t.|.d...r.g.
+00003830: 7d06 6405 7d07 7c05 a015 a100 7d08 7c08  }.d.}.|.....}.|.
+00003840: 4400 5d40 7d09 7c00 a016 7c09 a101 7d0a  D.]@}.|...|...}.
+00003850: 7c0a 6a0d 7417 7c05 6a0f 6a18 7c09 6a19  |.j.t.|.j.j.|.j.
+00003860: 6a1a 6406 6407 8400 6408 8d03 7c07 1700  j.d.d...d...|...
+00003870: 6409 8d01 0100 741b 7c09 741c 8302 7284  d.....t.|.t...r.
+00003880: 741b 7c09 741d 8302 7384 7c0a 6a0d 7c0a  t.|.t...s.|.j.|.
+00003890: 640a 1900 640b 1700 640c 8d01 0100 7c07  d...d...d.....|.
+000038a0: 640b 3700 7d07 741b 7c09 741e 8302 728d  d.7.}.t.|.t...r.
+000038b0: 7c07 640d 3700 7d07 7c06 a01f 7c0a a101  |.d.7.}.|...|...
+000038c0: 0100 7152 7c06 7c04 640e 3c00 7c04 a00d  ..qR|.|.d.<.|...
+000038d0: 7420 7c05 6a0f 640f 8302 a101 0100 7c04  t |.j.d.......|.
+000038e0: a00d 7420 7c01 6410 8302 a101 0100 7414  ..t |.d.......t.
+000038f0: 7c01 6a21 6411 8302 72b4 7c04 6a0d 6412  |.j!d...r.|.j.d.
+00003900: 6413 8d01 0100 7400 7c01 6a21 8301 72c5  d.....t.|.j!..r.
+00003910: 7401 7c01 6a21 7422 8302 72c5 7c04 6a0d  t.|.j!t"..r.|.j.
+00003920: 6412 6414 8d01 0100 7c01 6a23 6400 7501  d.d.....|.j#d.u.
+00003930: 72d2 7c00 a024 7c01 6a23 a101 7c04 6415  r.|..$|.j#..|.d.
+00003940: 3c00 7c01 6a25 6400 7501 72e7 7c01 6a25  <.|.j%d.u.r.|.j%
+00003950: a026 a100 7d0b 7c0b 6400 7501 72e7 7c04  .&..}.|.d.u.r.|.
+00003960: 6a0d 7c0b 6a27 6416 8d01 0100 7c01 6a28  j.|.j'd.....|.j(
+00003970: 72f3 7c04 6a0d 7429 7c01 6a28 8301 6417  r.|.j.t)|.j(..d.
+00003980: 8d01 0100 742a 7c01 6418 6400 8303 7d0c  ....t*|.d.d...}.
+00003990: 7c0c 6400 7501 9001 7205 7c04 6a0d 7c0c  |.d.u...r.|.j.|.
+000039a0: 6a27 6419 8d01 0100 742a 7c01 641a 6400  j'd.....t*|.d.d.
+000039b0: 8303 7d0d 7c0d 6400 7501 9001 7217 7c04  ..}.|.d.u...r.|.
+000039c0: 6a0d 7c0d 6a27 641b 8d01 0100 742a 7c01  j.|.j'd.....t*|.
+000039d0: 6a21 641c 6900 8303 7d0e 7c0e 9001 722e  j!d.i...}.|...r.
+000039e0: 7c04 6a0d 641d 641e 8400 7c0e a02b a100  |.j.d.d...|..+..
+000039f0: 4400 8301 641f 8d01 0100 7410 6a11 a02c  D...d.....t.j..,
+00003a00: 6420 a101 9001 7251 742a 7c01 6421 6400  d ....rQt*|.d!d.
+00003a10: 8303 6400 7501 9001 7251 7414 7c01 6a21  ..d.u...rQt.|.j!
+00003a20: 6422 8302 9001 7251 7c04 6a0d 742d 6a2e  d"....rQ|.j.t-j.
+00003a30: a02f 7c01 6a21 a101 6a30 6423 8d01 0100  ./|.j!..j0d#....
+00003a40: 6424 4400 5d17 7d0f 742a 7c01 7c0f 6400  d$D.].}.t*|.|.d.
+00003a50: 8303 7d10 7c10 6400 7501 9001 7269 7c04  ..}.|.d.u...ri|.
+00003a60: a00d 7c0f 7c10 6a31 6a32 6901 a101 0100  ..|.|.j1j2i.....
+00003a70: 9001 7153 7c01 6a33 6400 7501 9001 728f  ..qS|.j3d.u...r.
+00003a80: 7c04 6a0d 7c01 6a33 6a27 6425 6426 8400  |.j.|.j3j'd%d&..
+00003a90: 7c01 6a33 6a34 6a35 4400 8301 6427 8d02  |.j3j4j5D...d'..
+00003aa0: 0100 7414 7c01 6428 8302 9001 728f 7c04  ..t.|.d(....r.|.
+00003ab0: 6a0d 7c01 6a36 6429 8d01 0100 7c04 5300  j.|.j6d)....|.S.
+00003ac0: 292a 4e29 05da 0269 6472 3601 0000 729b  )*N)...idr6...r.
+00003ad0: 0000 00da 0573 6c61 7665 da08 6564 6974  .....slave..edit
+00003ae0: 6162 6c65 2901 7237 0100 007a 0f25 7320  able).r7...z.%s 
+00003af0: 6861 7320 6e6f 2073 746f 7265 da0b 6765  has no store..ge
+00003b00: 745f 636f 6c75 6d6e 7372 0100 0000 6301  t_columnsr....c.
+00003b10: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00003b20: 0000 0053 0000 0073 0600 0000 7c00 6a00  ...S...s....|.j.
+00003b30: 5300 723b 0000 00a9 0172 5300 0000 a901  S.r;.....rS.....
+00003b40: 7292 0000 0072 3700 0000 7237 0000 0072  r....r7...r7...r
+00003b50: 3800 0000 723e 0100 0073 0200 0073 0200  8...r>...s...s..
+00003b60: 0000 0600 7a25 5265 6e64 6572 6572 2e61  ....z%Renderer.a
+00003b70: 6374 6f72 326a 736f 6e2e 3c6c 6f63 616c  ctor2json.<local
+00003b80: 733e 2e3c 6c61 6d62 6461 3e72 3f01 0000  s>.<lambda>r?...
+00003b90: 2901 da0c 6669 656c 6473 5f69 6e64 6578  )...fields_index
+00003ba0: 724b 0100 0072 2d00 0000 2901 da13 6669  rK...r-...)...fi
+00003bb0: 656c 6473 5f69 6e64 6578 5f68 6964 6465  elds_index_hidde
+00003bc0: 6ee9 0200 0000 da03 636f 6cda 0870 6b5f  n.......col..pk_
+00003bd0: 696e 6465 787a d070 7265 7669 6577 5f6c  indexz.preview_l
+00003be0: 696d 6974 2075 7365 5f64 6574 6169 6c5f  imit use_detail_
+00003bf0: 7061 7261 6d5f 7061 6e65 6c20 7573 655f  param_panel use_
+00003c00: 6465 7461 696c 5f70 6172 616d 735f 7661  detail_params_va
+00003c10: 6c75 6520 6869 6465 5f6e 6176 6967 6174  lue hide_navigat
+00003c20: 6f72 2075 7365 5f64 6574 6169 6c5f 7061  or use_detail_pa
+00003c30: 7261 6d73 5f76 616c 7565 2072 6561 6374  rams_value react
+00003c40: 5f72 6573 706f 6e73 6976 6520 6d61 785f  _responsive max_
+00003c50: 7265 6e64 6572 5f64 6570 7468 2073 696d  render_depth sim
+00003c60: 706c 655f 736c 6176 6567 7269 645f 6865  ple_slavegrid_he
+00003c70: 6164 6572 2070 6167 696e 6174 6f72 5f74  ader paginator_t
+00003c80: 656d 706c 6174 6520 6869 6465 5f74 6f70  emplate hide_top
+00003c90: 5f74 6f6f 6c62 6172 2068 6964 655f 6966  _toolbar hide_if
+00003ca0: 5f65 6d70 7479 20da 0466 696c 6554 2901  _empty ..fileT).
+00003cb0: da0d 636f 6e74 6169 6e5f 6d65 6469 6129  ..contain_media)
+00003cc0: 01da 0965 6469 745f 7361 6665 7241 0100  ...edit_saferA..
+00003cd0: 0072 2a01 0000 2901 da0d 6163 7469 7665  .r*...)...active
+00003ce0: 5f66 6965 6c64 73da 0b63 6172 645f 6c61  _fields..card_la
+00003cf0: 796f 7574 2901 7254 0100 00da 0b6c 6973  yout).rT.....lis
+00003d00: 745f 6c61 796f 7574 2901 7255 0100 00da  t_layout).rU....
+00003d10: 0e5f 6368 6f6f 7365 7273 5f64 6963 7463  ._choosers_dictc
+00003d20: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00003d30: 0500 0000 5300 0000 7322 0000 0069 007c  ....S...s"...i.|
+00003d40: 005d 0d5c 027d 017d 027c 0164 0064 0184  .].\.}.}.|.d.d..
+00003d50: 007c 026a 0044 0083 0193 0271 0253 0029  .|.j.D.....q.S.)
+00003d60: 0263 0100 0000 0000 0000 0000 0000 0200  .c..............
+00003d70: 0000 0300 0000 5300 0000 f312 0000 0067  ......S........g
+00003d80: 007c 005d 057d 017c 016a 0091 0271 0253  .|.].}.|.j...q.S
+00003d90: 0072 3700 0000 7249 0100 0029 0272 4700  .r7...rI...).rG.
+00003da0: 0000 da02 6366 7237 0000 0072 3700 0000  ....cfr7...r7...
+00003db0: 7238 0000 0072 4900 0000 ac02 0000 f302  r8...rI.........
+00003dc0: 0000 0012 007a 3252 656e 6465 7265 722e  .....z2Renderer.
+00003dd0: 6163 746f 7232 6a73 6f6e 2e3c 6c6f 6361  actor2json.<loca
+00003de0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2e3c  ls>.<dictcomp>.<
+00003df0: 6c69 7374 636f 6d70 3e29 01da 0e63 6f6e  listcomp>)...con
+00003e00: 7465 7874 5f66 6965 6c64 7329 0372 4700  text_fields).rG.
+00003e10: 0000 da02 666e 7248 0000 0072 3700 0000  ....fnrH...r7...
+00003e20: 7237 0000 0072 3800 0000 724d 0000 00ac  r7...r8...rM....
+00003e30: 0200 0073 0600 0000 0600 0601 16ff 7a27  ...s..........z'
+00003e40: 5265 6e64 6572 6572 2e61 6374 6f72 326a  Renderer.actor2j
+00003e50: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6469  son.<locals>.<di
+00003e60: 6374 636f 6d70 3e29 01da 0c63 686f 6f73  ctcomp>)...choos
+00003e70: 6572 5f64 6963 74da 0c63 6f6e 7465 6e74  er_dict..content
+00003e80: 7479 7065 73da 056d 6f64 656c da05 5f6d  types..model.._m
+00003e90: 6574 6129 01da 0c63 6f6e 7465 6e74 5f74  eta)...content_t
+00003ea0: 7970 6529 03da 0d64 6574 6169 6c5f 6163  ype)...detail_ac
+00003eb0: 7469 6f6e da0d 696e 7365 7274 5f61 6374  tion..insert_act
+00003ec0: 696f 6eda 0e64 6566 6175 6c74 5f61 6374  ion..default_act
+00003ed0: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
+00003ee0: 0200 0000 0300 0000 5300 0000 7257 0100  ........S...rW..
+00003ef0: 0072 3700 0000 7249 0100 0029 0272 4700  .r7...rI...).rG.
+00003f00: 0000 7292 0000 0072 3700 0000 7237 0000  ..r....r7...r7..
+00003f10: 0072 3800 0000 7249 0000 00bc 0200 0072  .r8...rI.......r
+00003f20: 5901 0000 7a27 5265 6e64 6572 6572 2e61  Y...z'Renderer.a
+00003f30: 6374 6f72 326a 736f 6e2e 3c6c 6f63 616c  ctor2json.<local
+00003f40: 733e 2e3c 6c69 7374 636f 6d70 3e29 02da  s>.<listcomp>)..
+00003f50: 0d70 6172 616d 735f 6c61 796f 7574 da0d  .params_layout..
+00003f60: 7061 7261 6d73 5f66 6965 6c64 73da 1070  params_fields..p
+00003f70: 6172 616d 735f 7061 6e65 6c5f 706f 7329  arams_panel_pos)
+00003f80: 0172 6601 0000 2937 722c 0000 0072 bb00  .rf...)7r,...r..
+00003f90: 0000 721b 0000 0072 3d01 0000 da0d 5f61  ..r....r=....._a
+00003fa0: 6374 696f 6e73 5f6c 6973 7472 7400 0000  ctions_listrt...
+00003fb0: 72f6 0000 00da 0f67 6574 5f61 6374 6f72  r......get_actor
+00003fc0: 5f6c 6162 656c da04 626f 6f6c da06 6d61  _label..bool..ma
+00003fd0: 7374 6572 da0c 6869 6465 5f65 6469 7469  ster..hide_editi
+00003fe0: 6e67 7229 0000 0072 d800 0000 727a 0000  ngr)...r....rz..
+00003ff0: 00da 0a67 6574 5f68 616e 646c 65da 0573  ...get_handle..s
+00004000: 746f 7265 7204 0000 0072 7200 0000 da06  torer....rr.....
+00004010: 6c6f 6767 6572 da07 7761 726e 696e 6772  logger..warningr
+00004020: 8600 0000 7248 0100 0072 b000 0000 7239  ....rH...r....r9
+00004030: 0000 00da 0b6c 6973 745f 6669 656c 6473  .....list_fields
+00004040: 72bd 0000 0072 5300 0000 72a6 0000 0072  r....rS...r....r
+00004050: 1f00 0000 7220 0000 0072 2200 0000 7233  ....r ...r"...r3
+00004060: 0100 0072 2800 0000 725e 0100 0072 2b00  ...r(...r^...r+.
+00004070: 0000 7241 0100 0072 4401 0000 7261 0100  ..rA...rD...ra..
+00004080: 00da 1167 6574 5f77 696e 646f 775f 6c61  ...get_window_la
+00004090: 796f 7574 728b 0000 0072 5301 0000 727b  youtr....rS...r{
+000040a0: 0000 0072 0801 0000 726b 0000 0072 7900  ...r....rk...ry.
+000040b0: 0000 720e 0000 00da 076f 626a 6563 7473  ..r......objects
+000040c0: da0d 6765 745f 666f 725f 6d6f 6465 6c72  ..get_for_modelr
+000040d0: df00 0000 726f 0000 0072 4e00 0000 7264  ....ro...rN...rd
+000040e0: 0100 00da 0c70 6172 616d 735f 7374 6f72  .....params_stor
+000040f0: 65da 0c70 6172 616d 5f66 6965 6c64 7372  e..param_fieldsr
+00004100: 6601 0000 2911 7240 0000 0072 ab00 0000  f...).r@...r....
+00004110: da02 616c da02 686b 72ac 0000 00da 0261  ..al..hkr......a
+00004120: 68da 0763 6f6c 756d 6e73 da09 696e 6465  h..columns..inde
+00004130: 785f 6d6f 64da 0963 6f6c 5f65 6c65 6d73  x_mod..col_elems
+00004140: 724e 0100 0072 1201 0000 da02 776c 7254  rN...r......wlrT
+00004150: 0100 0072 5501 0000 725c 0100 0072 be00  ...rU...r\...r..
+00004160: 0000 7295 0000 0072 3700 0000 7237 0000  ..r....r7...r7..
+00004170: 0072 3800 0000 da0a 6163 746f 7232 6a73  .r8.....actor2js
+00004180: 6f6e 5a02 0000 7392 0000 0016 0110 0106  onZ...s.........
+00004190: 0102 0106 0108 010c 0106 fc08 070c 0108  ................
+000041a0: 020a 0112 010a 0304 0104 0108 0108 010a  ................
+000041b0: 0112 0106 0104 ff02 0108 ff14 0214 0308  ................
+000041c0: 010a 0108 010c 0108 0112 0510 010c 0d0c  ................
+000041d0: 0116 020c 010a 0210 010a 020a 0108 010e  ................
+000041e0: 0106 0212 010c 020a 010e 010c 020a 010e  ................
+000041f0: 020e 0306 010a 0106 010a ff26 0302 0106  ...........&....
+00004200: ff18 0308 010c 010a 0112 0104 800c 0204  ................
+00004210: 0206 0112 0106 fe0c 040e 0104 017a 1352  .............z.R
+00004220: 656e 6465 7265 722e 6163 746f 7232 6a73  enderer.actor2js
+00004230: 6f6e 6302 0000 0000 0000 0000 0000 0004  onc.............
+00004240: 0000 0006 0000 0003 0000 0073 6400 0000  ...........sd...
+00004250: 6401 8801 5f00 8801 6a01 4400 5d22 8900  d..._...j.D.]"..
+00004260: 8800 6a02 6400 7501 720e 7106 7403 6a04  ..j.d.u.r.q.t.j.
+00004270: 6a05 8801 a006 8800 6a07 a101 8e00 7d02  j.......j.....}.
+00004280: 8700 8701 6602 6402 6403 8408 7d03 7408  ....f.d.d...}.t.
+00004290: 6a09 6a0a a00b 7c02 7c03 7c01 a103 0100  j.j...|.|.|.....
+000042a0: 7106 6404 8801 5f00 740c 8300 a00d 7c01  q.d..._.t.....|.
+000042b0: a101 5300 2905 4e54 6301 0000 0000 0000  ..S.).NTc.......
+000042c0: 0000 0000 0001 0000 0007 0000 0013 0000  ................
+000042d0: 0073 2400 0000 7400 6a01 7400 a002 7403  .s$...t.j.t...t.
+000042e0: 8801 a004 8800 a101 8301 a101 7c00 6401  ............|.d.
+000042f0: 6402 8d03 0100 6400 5300 2903 4e72 6700  d.....d.S.).Nrg.
+00004300: 0000 7268 0000 0029 0572 8f00 0000 7290  ..rh...).r....r.
+00004310: 0000 0072 9100 0000 7226 0000 0072 7d01  ...r....r&...r}.
+00004320: 0000 724a 0100 00a9 0272 9e00 0000 7240  ..rJ.....r....r@
+00004330: 0000 0072 3700 0000 7238 0000 00da 0577  ...r7...r8.....w
+00004340: 7269 7465 cb02 0000 7302 0000 0024 027a  rite....s....$.z
+00004350: 2652 656e 6465 7265 722e 6275 696c 645f  &Renderer.build_
+00004360: 6a73 5f63 6163 6865 2e3c 6c6f 6361 6c73  js_cache.<locals
+00004370: 3e2e 7772 6974 6546 290e 7271 0000 0072  >.writeF).rq...r
+00004380: 6d00 0000 da0f 6765 745f 6861 6e64 6c65  m.....get_handle
+00004390: 5f6e 616d 6572 8000 0000 da04 7061 7468  _namer......path
+000043a0: da04 6a6f 696e 7229 0100 0072 f600 0000  ..joinr)...r....
+000043b0: 7204 0000 0072 7200 0000 7223 0000 00da  r....rr...r#....
+000043c0: 0f6d 616b 655f 6361 6368 655f 6669 6c65  .make_cache_file
+000043d0: 723c 0000 00da 0e62 7569 6c64 5f6a 735f  r<.....build_js_
+000043e0: 6361 6368 6529 0472 4000 0000 da05 666f  cache).r@.....fo
+000043f0: 7263 6572 5b01 0000 727f 0100 0072 4200  rcer[...r....rB.
+00004400: 0000 727e 0100 0072 3800 0000 7284 0100  ..r~...r8...r...
+00004410: 00c2 0200 0073 1200 0000 0602 0a02 0a01  .....s..........
+00004420: 0201 1401 0e02 1404 0602 0c01 7a17 5265  ............z.Re
+00004430: 6e64 6572 6572 2e62 7569 6c64 5f6a 735f  nderer.build_js_
+00004440: 6361 6368 6572 3b00 0000 2920 72ba 0000  cacher;...) r...
+00004450: 00da 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  ...__module__.._
+00004460: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00004470: 6f63 5f5f da0e 6973 5f69 6e74 6572 6163  oc__..is_interac
+00004480: 7469 7665 da08 6361 6e5f 6175 7468 7224  tive..can_authr$
+00004490: 0100 0072 2801 0000 da18 7375 7070 6f72  ...r(.....suppor
+000044a0: 745f 6461 7368 626f 6172 645f 6c61 796f  t_dashboard_layo
+000044b0: 7574 723d 0000 0072 9900 0000 724f 0000  utr=...r....rO..
+000044c0: 0072 8a00 0000 72b0 0000 0072 bf00 0000  .r....r....r....
+000044d0: 72d5 0000 0072 e200 0000 72e9 0000 0072  r....r....r....r
+000044e0: aa00 0000 72e5 0000 0072 3f00 0000 7204  ....r....r?...r.
+000044f0: 0100 0072 0501 0000 7206 0100 0072 1a01  ...r....r....r..
+00004500: 0000 7220 0100 0072 2901 0000 723d 0100  ..r ...r)...r=..
+00004510: 0072 4401 0000 727d 0100 0072 8401 0000  .rD...r}...r....
+00004520: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00004530: 3700 0000 7237 0000 0072 4200 0000 7238  7...r7...rB...r8
+00004540: 0000 0072 3a00 0000 3c00 0000 733c 0000  ...r:...<...s<..
+00004550: 0008 0004 0104 0304 0104 0204 0104 010c  ................
+00004560: 0208 0408 5808 1d08 0808 2008 030a 1802  ....X..... .....
+00004570: 120a ff08 1508 0e08 2108 4e08 0e08 0a08  ........!.N.....
+00004580: 2a08 0908 0f08 0a08 4408 0c14 6872 3a00  *.......D...hr:.
+00004590: 0000 723b 0000 0029 4972 8f00 0000 7280  ..r;...)Ir....r.
+000045a0: 0000 00da 0770 6174 686c 6962 7202 0000  .....pathlibr...
+000045b0: 00da 0468 746d 6c72 0300 0000 da0b 646a  ...htmlr......dj
+000045c0: 616e 676f 2e63 6f6e 6672 0400 0000 da09  ango.confr......
+000045d0: 646a 616e 676f 2e64 6272 0500 0000 da11  django.dbr......
+000045e0: 646a 616e 676f 2e75 7469 6c73 2e74 6578  django.utils.tex
+000045f0: 7472 0600 0000 da0c 646a 616e 676f 2e75  tr......django.u
+00004600: 7469 6c73 7207 0000 00da 126c 696e 6f2e  tilsr......lino.
+00004610: 636f 7265 2e72 656e 6465 7265 7272 0800  core.rendererr..
+00004620: 0000 7209 0000 00da 0f6c 696e 6f2e 636f  ..r......lino.co
+00004630: 7265 2e6d 656e 7573 720a 0000 0072 0b00  re.menusr....r..
+00004640: 0000 da09 6c69 6e6f 2e63 6f72 6572 0c00  ....lino.corer..
+00004650: 0000 720d 0000 00da 0e6c 696e 6f2e 636f  ..r......lino.co
+00004660: 7265 2e67 666b 7372 0e00 0000 da1e 6c69  re.gfksr......li
+00004670: 6e6f 2e6d 6f64 6c69 622e 6578 746a 732e  no.modlib.extjs.
+00004680: 6578 745f 7265 6e64 6572 6572 720f 0000  ext_rendererr...
+00004690: 00da 116c 696e 6f2e 636f 7265 2e61 6374  ...lino.core.act
+000046a0: 696f 6e73 7210 0000 0072 1100 0000 7212  ionsr....r....r.
+000046b0: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+000046c0: 0000 7216 0000 0072 1700 0000 da15 6c69  ..r....r......li
+000046d0: 6e6f 2e63 6f72 652e 626f 756e 6461 6374  no.core.boundact
+000046e0: 696f 6e72 1800 0000 da15 6c69 6e6f 2e63  ionr......lino.c
+000046f0: 6f72 652e 6368 6f69 6365 6c69 7374 7372  ore.choicelistsr
+00004700: 1900 0000 da1e 6c69 6e6f 2e6d 6f64 6c69  ......lino.modli
+00004710: 622e 7379 7374 656d 2e63 686f 6963 656c  b.system.choicel
+00004720: 6973 7473 721a 0000 00da 106c 696e 6f2e  istsr......lino.
+00004730: 636f 7265 2e61 6374 6f72 7372 1b00 0000  core.actorsr....
+00004740: da11 6c69 6e6f 2e63 6f72 652e 6c61 796f  ..lino.core.layo
+00004750: 7574 7372 1c00 0000 721d 0000 00da 0f6c  utsr....r......l
+00004760: 696e 6f2e 636f 7265 2e65 6c65 6d73 721e  ino.core.elemsr.
+00004770: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+00004780: 0000 7222 0000 0072 2300 0000 da0a 6574  ..r"...r#.....et
+00004790: 6765 6e2e 6874 6d6c 7224 0000 00da 0a6c  gen.htmlr$.....l
+000047a0: 696e 6f2e 7574 696c 7372 2500 0000 da10  ino.utilsr%.....
+000047b0: 6c69 6e6f 2e75 7469 6c73 2e6a 7367 656e  lino.utils.jsgen
+000047c0: 7226 0000 0072 2700 0000 7228 0000 00da  r&...r'...r(....
+000047d0: 176c 696e 6f2e 6d6f 646c 6962 2e75 7365  .lino.modlib.use
+000047e0: 7273 2e75 7469 6c73 7229 0000 0072 2a00  rs.utilsr)...r*.
+000047f0: 0000 da19 6c69 6e6f 2e6d 6f64 6c69 622e  ....lino.modlib.
+00004800: 7379 7374 656d 2e6d 6978 696e 7372 2b00  system.mixinsr+.
+00004810: 0000 da07 696e 7370 6563 7472 2c00 0000  ....inspectr,...
+00004820: da05 6963 6f6e 7372 2e00 0000 7239 0000  ..iconsr....r9..
+00004830: 0072 3a00 0000 7237 0000 0072 3700 0000  .r:...r7...r7...
+00004840: 7237 0000 0072 3800 0000 da08 3c6d 6f64  r7...r8.....<mod
+00004850: 756c 653e 0100 0000 733e 0000 0008 0408  ule>....s>......
+00004860: 010c 010c 010c 010c 010c 010c 0110 0210  ................
+00004870: 020c 010c 010c 010c 0128 020c 030c 010c  .........(......
+00004880: 010c 0110 011c 010c 020c 020c 0214 0110  ................
+00004890: 020c 010c 020c 020a 0314 0d              ...........
```

### Comparing `lino_react-23.7.4/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 24 10:38:37 2023 UTC, .py size: 28705 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ad7d 1d64 2170 0000  o........}.d!p..
+00000000: 6f0d 0d0a 0000 0000 6be5 8564 2170 0000  o.......k..d!p..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0e03 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6401 6404 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
@@ -106,1183 +106,1184 @@
 00000690: 7461 6b65 7320 7468 6520 6974 7465 7227  takes the itter'
 000006a0: 7320 6974 656d 2061 6e64 2072 6574 7572  s item and retur
 000006b0: 6e73 2074 6861 7420 7761 6e74 6564 206d  ns that wanted m
 000006c0: 6174 6368 6564 2069 7465 6de9 ffff ffff  atched item.....
 000006d0: 2902 da08 6361 6c6c 6162 6c65 da09 656e  )...callable..en
 000006e0: 756d 6572 6174 6529 05da 0569 7474 6572  umerate)...itter
 000006f0: da06 7461 7267 6574 da03 6b65 79da 0169  ..target..key..i
-00000700: da01 78a9 0072 3600 0000 fa2e 2f68 6f6d  ..x..r6...../hom
-00000710: 652f 6c75 632f 776f 726b 2f72 6561 6374  e/luc/work/react
-00000720: 2f6c 696e 6f5f 7265 6163 742f 7265 6163  /lino_react/reac
-00000730: 742f 7669 6577 732e 7079 da04 6669 6e64  t/views.py..find
-00000740: 3800 0000 7310 0000 0018 0210 0204 0108  8...s...........
-00000750: 0108 0108 0102 ff04 0372 3800 0000 7a21  .........r8...z!
-00000760: 2573 2068 6173 206e 6f20 726f 7720 7769  %s has no row wi
-00000770: 7468 2070 7269 6d61 7279 206b 6579 2025  th primary key %
-00000780: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-00000790: 0000 0300 0000 4000 0000 732a 0000 0065  ......@...s*...e
-000007a0: 005a 0164 005a 0264 0864 0264 0384 015a  .Z.d.Z.d.d.d...Z
-000007b0: 0364 0864 0464 0584 015a 0464 0864 0664  .d.d.d...Z.d.d.d
-000007c0: 0784 015a 0564 0153 0029 0972 2b00 0000  ...Z.d.S.).r+...
-000007d0: 4e63 0500 0000 0000 0000 0000 0000 0800  Nc..............
-000007e0: 0000 0800 0000 4300 0000 7354 0000 007c  ......C...sT...|
-000007f0: 016a 007d 0574 017c 027c 037c 017c 0564  .j.}.t.|.|.|.|.d
-00000800: 0174 026a 036a 046a 056a 0664 028d 067d  .t.j.j.j.j.d...}
-00000810: 067c 0464 036b 0272 1e7c 06a0 07a1 007d  .|.d.k.r.|.....}
-00000820: 077c 0767 017c 065f 086e 057c 06a0 097c  .|.g.|._.n.|...|
-00000830: 04a1 0101 0074 026a 036a 0aa0 0b7c 06a1  .....t.j.j...|..
-00000840: 0153 0029 044e 54a9 01da 0872 656e 6465  .S.).NT....rende
-00000850: 7265 72fa 062d 3939 3939 3829 0cda 0450  rer..-99998)...P
-00000860: 4f53 5472 2000 0000 720b 0000 00da 0453  OSTr ...r......S
-00000870: 4954 45da 0770 6c75 6769 6e73 da05 7265  ITE..plugins..re
-00000880: 6163 7472 3a00 0000 da0f 6372 6561 7465  actr:.....create
-00000890: 5f69 6e73 7461 6e63 65da 0d73 656c 6563  _instance..selec
-000008a0: 7465 645f 726f 7773 da10 7365 745f 7365  ted_rows..set_se
-000008b0: 6c65 6374 6564 5f70 6b73 7226 0000 00da  lected_pksr&....
-000008c0: 0a72 756e 5f61 6374 696f 6e29 08da 0473  .run_action)...s
-000008d0: 656c 66da 0772 6571 7565 7374 da09 6170  elf..request..ap
-000008e0: 705f 6c61 6265 6cda 0561 6374 6f72 da02  p_label..actor..
-000008f0: 706b da04 6461 7461 da02 6172 da04 656c  pk..data..ar..el
-00000900: 656d 7236 0000 0072 3600 0000 7237 0000  emr6...r6...r7..
-00000910: 00da 0470 6f73 744f 0000 0073 1400 0000  ...postO...s....
-00000920: 0602 0201 0a01 0a01 06fe 0803 0801 0a01  ................
-00000930: 0a02 0e01 7a0f 4170 6945 6c65 6d65 6e74  ....z.ApiElement
-00000940: 2e70 6f73 7463 0500 0000 0000 0000 0000  .postc..........
-00000950: 0000 0700 0000 0800 0000 4300 0000 f340  ..........C....@
-00000960: 0000 0074 00a0 017c 016a 02a1 017d 0574  ...t...|.j...}.t
-00000970: 037c 027c 037c 017c 0564 0174 046a 056a  .|.|.|.|.d.t.j.j
-00000980: 066a 076a 0864 028d 067d 067c 06a0 097c  .j.j.d...}.|...|
-00000990: 04a1 0101 0074 046a 056a 0aa0 0b7c 06a1  .....t.j.j...|..
-000009a0: 0153 00a9 034e 4672 3900 0000 a90c 7209  .S...NFr9.....r.
-000009b0: 0000 00da 0951 7565 7279 4469 6374 da04  .....QueryDict..
-000009c0: 626f 6479 7220 0000 0072 0b00 0000 723d  bodyr ...r....r=
-000009d0: 0000 0072 3e00 0000 723f 0000 0072 3a00  ...r>...r?...r:.
-000009e0: 0000 7242 0000 0072 2600 0000 7243 0000  ..rB...r&...rC..
-000009f0: 00a9 0772 4400 0000 7245 0000 0072 4600  ...rD...rE...rF.
-00000a00: 0000 7247 0000 0072 4800 0000 7249 0000  ..rG...rH...rI..
-00000a10: 0072 4a00 0000 7236 0000 0072 3600 0000  .rJ...r6...r6...
-00000a20: 7237 0000 00da 0370 7574 5c00 0000 730e  r7.....put\...s.
-00000a30: 0000 000c 0102 030a 010a 0106 fe0a 030e  ................
-00000a40: 017a 0e41 7069 456c 656d 656e 742e 7075  .z.ApiElement.pu
-00000a50: 7463 0500 0000 0000 0000 0000 0000 0700  tc..............
-00000a60: 0000 0800 0000 4300 0000 724d 0000 0072  ......C...rM...r
-00000a70: 4e00 0000 724f 0000 0072 5200 0000 7236  N...rO...rR...r6
-00000a80: 0000 0072 3600 0000 7237 0000 00da 0664  ...r6...r7.....d
-00000a90: 656c 6574 6566 0000 0073 0e00 0000 0c01  eletef...s......
-00000aa0: 0201 0a01 0a01 06fe 0a03 0e01 7a11 4170  ............z.Ap
-00000ab0: 6945 6c65 6d65 6e74 2e64 656c 6574 65a9  iElement.delete.
-00000ac0: 034e 4e4e 2906 da08 5f5f 6e61 6d65 5f5f  .NNN)...__name__
-00000ad0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000ae0: 7175 616c 6e61 6d65 5f5f 724c 0000 0072  qualname__rL...r
-00000af0: 5300 0000 7254 0000 0072 3600 0000 7236  S...rT...r6...r6
-00000b00: 0000 0072 3600 0000 7237 0000 0072 2b00  ...r6...r7...r+.
-00000b10: 0000 4d00 0000 7308 0000 0008 000a 020a  ..M...s.........
-00000b20: 0d0e 0a72 2b00 0000 6300 0000 0000 0000  ...r+...c.......
-00000b30: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000b40: 0073 2000 0000 6500 5a01 6400 5a02 6406  .s ...e.Z.d.Z.d.
-00000b50: 6402 6403 8401 5a03 6406 6404 6405 8401  d.d...Z.d.d.d...
-00000b60: 5a04 6401 5300 2907 da07 4170 694c 6973  Z.d.S.)...ApiLis
-00000b70: 744e 6304 0000 0000 0000 0000 0000 0005  tNc.............
-00000b80: 0000 0006 0000 0043 0000 0073 3400 0000  .......C...s4...
-00000b90: 7400 7c02 7c03 7c01 7c01 6a01 6401 8305  t.|.|.|.|.j.d...
-00000ba0: 7d04 7c04 a002 a100 0100 7403 6a04 6a05  }.|.......t.j.j.
-00000bb0: 6a06 7c04 5f07 7403 6a04 6a05 a008 7c04  j.|._.t.j.j...|.
-00000bc0: a101 5300 2902 4e54 2909 7220 0000 0072  ..S.).NT).r ...r
-00000bd0: 3c00 0000 da0a 6765 745f 7374 6174 7573  <.....get_status
-00000be0: 720b 0000 0072 3d00 0000 7226 0000 00da  r....r=...r&....
-00000bf0: 1064 6566 6175 6c74 5f72 656e 6465 7265  .default_rendere
-00000c00: 7272 3a00 0000 7243 0000 0029 0572 4400  rr:...rC...).rD.
-00000c10: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00000c20: 0072 4a00 0000 7236 0000 0072 3600 0000  .rJ...r6...r6...
-00000c30: 7237 0000 0072 4c00 0000 7000 0000 7308  r7...rL...p...s.
-00000c40: 0000 0012 0108 010c 010e 017a 0c41 7069  ...........z.Api
-00000c50: 4c69 7374 2e70 6f73 7463 0400 0000 0000  List.postc......
-00000c60: 0000 0000 0000 1300 0000 0800 0000 0300  ................
-00000c70: 0000 7376 0200 0074 007c 0183 017d 047c  ..sv...t.|...}.|
-00000c80: 0472 0a74 017c 0483 0153 0074 027c 027c  .r.t.|...S.t.|.|
-00000c90: 037c 017c 016a 0364 0183 0589 0088 00a0  .|.|.j.d........
-00000ca0: 04a1 0073 2064 02a0 0588 00a1 017d 0574  ...s d.......}.t
-00000cb0: 067c 0583 0182 0174 076a 086a 096a 0a88  .|.....t.j.j.j..
-00000cc0: 005f 0b88 006a 0c89 027c 016a 03a0 0d74  ._...j...|.j...t
-00000cd0: 0e6a 0f88 006a 106a 116a 12a1 027d 067c  .j...j.j.j...}.|
-00000ce0: 016a 03a0 0d74 0e6a 13a1 017d 077c 0772  .j...t.j...}.|.r
-00000cf0: 4474 076a 086a 09a0 1488 00a1 0153 007c  Dt.j.j.......S.|
-00000d00: 0674 0e6a 156b 0290 0172 3474 1688 006a  .t.j.k...r4t...j
-00000d10: 106a 1174 1783 0272 6088 00a0 18a1 007d  .j.t...r`......}
-00000d20: 0874 1988 0088 006a 0c7c 0883 037d 0974  .t.....j.|...}.t
-00000d30: 017c 0983 0153 007c 016a 03a0 0d74 0e6a  .|...S.|.j...t.j
-00000d40: 1a74 0e6a 1ba1 0289 0188 0174 0e6a 1c6b  .t.j.......t.j.k
-00000d50: 0272 8864 037d 0a67 007d 0b88 006a 1d44  .r.d.}.g.}...j.D
-00000d60: 005d 117d 0c7c 0a7c 0ca0 1e88 00a1 0137  .].}.|.|.......7
-00000d70: 007d 0a7c 0ba0 1f64 047c 0c6a 2069 01a1  .}.|...d.|.j i..
-00000d80: 0101 0071 756e 4088 0174 0e6a 216b 0272  ...qun@..t.j!k.r
-00000d90: b464 037d 0a67 007d 0b88 006a 1d44 005d  .d.}.g.}...j.D.]
-00000da0: 1e7d 0c88 00a0 227c 0ca1 017d 0d88 00a0  .}...."|...}....
-00000db0: 237c 0c7c 0da1 027d 0d64 05a0 057c 0da1  #|.|...}.d...|..
-00000dc0: 017d 0d7c 0a7c 0d37 007d 0a7c 0ba0 1f64  .}.|.|.7.}.|...d
-00000dd0: 047c 0c6a 2069 01a1 0101 0071 946e 1464  .|.j i.....q.n.d
-00000de0: 007d 0a87 0187 0266 0264 0664 0784 0889  .}.....f.d.d....
-00000df0: 0387 0087 0366 0264 0864 0984 0888 006a  .....f.d.d.....j
-00000e00: 1d44 0083 017d 0b88 00a0 24a1 007d 0e88  .D...}....$..}..
-00000e10: 0174 0e6a 1b6b 0272 fb88 00a0 25a1 0044  .t.j.k.r....%..D
-00000e20: 005d 257d 0f88 006a 2664 0075 0073 ec74  .]%}...j&d.u.s.t
-00000e30: 277c 0b83 0164 0a17 0088 006a 266b 0073  '|...d.....j&k.s
-00000e40: ec88 006a 267c 0e64 0a17 006b 0272 f688  ...j&|.d...k.r..
-00000e50: 0388 007c 0f83 027d 107c 0ba0 1f7c 10a1  ...|...}.|...|..
-00000e60: 0101 007c 0e64 0a37 007d 0e71 d574 287c  ...|.d.7.}.q.t(|
-00000e70: 0e7c 0b7c 0a64 0188 006a 2988 00a0 2aa1  .|.|.d...j)...*.
-00000e80: 0064 0b8d 067d 1188 0174 0e6a 1b6b 0390  .d...}...t.j.k..
-00000e90: 0172 1d88 00a0 2ba1 007d 127c 1264 0075  .r....+..}.|.d.u
-00000ea0: 0190 0172 1d7c 0ba0 2c64 0c7c 12a1 0201  ...r.|..,d.|....
-00000eb0: 0088 006a 2d6a 2e90 0172 307c 116a 2f88  ...j-j...r0|.j/.
-00000ec0: 006a 2d6a 306a 31a0 3288 0088 006a 33a1  .j-j0j1.2....j3.
-00000ed0: 0264 0d8d 0101 0074 017c 1183 0153 0074  .d.....t.|...S.t
-00000ee0: 076a 086a 09a0 1488 00a1 0153 0029 0e4e  .j.j.......S.).N
-00000ef0: 547a 174e 6f20 7065 726d 6973 7369 6f6e  Tz.No permission
-00000f00: 2074 6f20 7275 6e20 7b7d da00 da02 6964   to run {}....id
-00000f10: 7a09 3c70 3e7b 7d3c 2f70 3e63 0200 0000  z.<p>{}</p>c....
-00000f20: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-00000f30: 1300 0000 7362 0000 0088 0074 006a 016b  ....sb.....t.j.k
-00000f40: 0272 0c88 016a 02a0 037c 007c 01a1 0253  .r...j...|.|...S
-00000f50: 0088 0074 006a 046b 0272 167c 01a0 057c  ...t.j.k.r.|...|
-00000f60: 00a1 0153 0088 0074 006a 066b 0272 2088  ...S...t.j.k.r .
-00000f70: 016a 026a 077d 026e 0488 016a 026a 087d  .j.j.}.n...j.j.}
-00000f80: 0288 016a 026a 097c 007c 017c 027c 00a0  ...j.j.|.|.|.|..
-00000f90: 0a7c 01a1 0164 018d 0453 0029 027a 4f55  .|...d...S.).zOU
-00000fa0: 7365 2064 6973 706c 6179 5f6d 6f64 6520  se display_mode 
-00000fb0: 746f 2064 6574 6572 6d69 6e65 2077 6869  to determine whi
-00000fc0: 6368 2073 6572 696c 6973 6174 696f 6e20  ch serilisation 
-00000fd0: 7374 6f72 6520 6d65 7468 6f64 2061 6e64  store method and
-00000fe0: 2066 6965 6c64 7320 746f 2075 7365 2902   fields to use).
-00000ff0: 7216 0000 00da 0a63 6172 645f 7469 746c  r......card_titl
-00001000: 6529 0b72 1b00 0000 da12 4449 5350 4c41  e).r......DISPLA
-00001010: 595f 4d4f 4445 5f54 4142 4c45 da05 7374  Y_MODE_TABLE..st
-00001020: 6f72 65da 0872 6f77 326c 6973 74da 1444  ore..row2list..D
-00001030: 4953 504c 4159 5f4d 4f44 455f 4741 4c4c  ISPLAY_MODE_GALL
-00001040: 4552 59da 1067 6574 5f67 616c 6c65 7279  ERY..get_gallery
-00001050: 5f69 7465 6dda 1244 4953 504c 4159 5f4d  _item..DISPLAY_M
-00001060: 4f44 455f 4341 5244 53da 0b63 6172 645f  ODE_CARDS..card_
-00001070: 6669 656c 6473 da0d 6465 7461 696c 5f66  fields..detail_f
-00001080: 6965 6c64 73da 0872 6f77 3264 6963 74da  ields..row2dict.
-00001090: 0e67 6574 5f63 6172 645f 7469 746c 6529  .get_card_title)
-000010a0: 0372 4a00 0000 da03 726f 7772 1600 0000  .rJ.....rowr....
-000010b0: 2902 da0c 6469 7370 6c61 795f 6d6f 6465  )...display_mode
-000010c0: da02 7268 7236 0000 0072 3700 0000 da09  ..rhr6...r7.....
-000010d0: 7365 7269 616c 697a 65b3 0000 0073 1400  serialize....s..
-000010e0: 0000 0a02 0e01 0a01 0a02 0a02 0a01 0802  ................
-000010f0: 0801 0c01 06ff 7a1e 4170 694c 6973 742e  ......z.ApiList.
-00001100: 6765 742e 3c6c 6f63 616c 733e 2e73 6572  get.<locals>.ser
-00001110: 6961 6c69 7a65 6301 0000 0000 0000 0000  ializec.........
-00001120: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-00001130: 1600 0000 6700 7c00 5d07 7d01 8801 8800  ....g.|.].}.....
-00001140: 7c01 8302 9102 7102 5300 7236 0000 0072  |.....q.S.r6...r
-00001150: 3600 0000 a902 da02 2e30 7269 0000 0029  6........0ri...)
-00001160: 0272 4a00 0000 726c 0000 0072 3600 0000  .rJ...rl...r6...
-00001170: 7237 0000 00da 0a3c 6c69 7374 636f 6d70  r7.....<listcomp
-00001180: 3ec2 0000 0073 0600 0000 0600 0201 0eff  >....s..........
-00001190: 7a1f 4170 694c 6973 742e 6765 742e 3c6c  z.ApiList.get.<l
-000011a0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000011b0: 3ee9 0100 0000 2906 da05 636f 756e 74da  >.....)...count.
-000011c0: 0472 6f77 73da 0968 746d 6c5f 7465 7874  .rows..html_text
-000011d0: da07 7375 6363 6573 73da 0c6e 6f5f 6461  ..success..no_da
-000011e0: 7461 5f74 6578 74da 0574 6974 6c65 7201  ta_text..titler.
-000011f0: 0000 0029 01da 0c70 6172 616d 5f76 616c  ...)...param_val
-00001200: 7565 7329 3472 2c00 0000 7221 0000 0072  ues)4r,...r!...r
-00001210: 2000 0000 da03 4745 54da 0e67 6574 5f70   .....GET..get_p
-00001220: 6572 6d69 7373 696f 6eda 0666 6f72 6d61  ermission..forma
-00001230: 7472 1200 0000 720b 0000 0072 3d00 0000  tr....r....r=...
-00001240: 7226 0000 0072 5b00 0000 723a 0000 00da  r&...r[...r:....
-00001250: 0261 68da 0367 6574 721b 0000 00da 1055  .ah..getr......U
-00001260: 524c 5f50 4152 414d 5f46 4f52 4d41 54da  RL_PARAM_FORMAT.
-00001270: 0c62 6f75 6e64 5f61 6374 696f 6eda 0661  .bound_action..a
-00001280: 6374 696f 6eda 0e64 6566 6175 6c74 5f66  ction..default_f
-00001290: 6f72 6d61 74da 1555 524c 5f50 4152 414d  ormat..URL_PARAM
-000012a0: 5f41 4354 494f 4e5f 4e41 4d45 7243 0000  _ACTION_NAMErC..
-000012b0: 00da 0f55 524c 5f46 4f52 4d41 545f 4a53  ...URL_FORMAT_JS
-000012c0: 4f4e da0a 6973 696e 7374 616e 6365 7225  ON..isinstancer%
-000012d0: 0000 0072 4000 0000 722d 0000 00da 1655  ...r@...r-.....U
-000012e0: 524c 5f50 4152 414d 5f44 4953 504c 4159  RL_PARAM_DISPLAY
-000012f0: 5f4d 4f44 4572 5f00 0000 da12 4449 5350  _MODEr_.....DISP
-00001300: 4c41 595f 4d4f 4445 5f53 544f 5259 da14  LAY_MODE_STORY..
-00001310: 736c 6963 6564 5f64 6174 615f 6974 6572  sliced_data_iter
-00001320: 6174 6f72 da0d 6173 5f73 746f 7279 5f69  ator..as_story_i
-00001330: 7465 6dda 0661 7070 656e 6472 4800 0000  tem..appendrH...
-00001340: da11 4449 5350 4c41 595f 4d4f 4445 5f4c  ..DISPLAY_MODE_L
-00001350: 4953 54da 1072 6f77 5f61 735f 7061 7261  IST..row_as_para
-00001360: 6772 6170 68da 0f61 6464 5f64 6574 6169  graph..add_detai
-00001370: 6c5f 6c69 6e6b da0f 6765 745f 746f 7461  l_link..get_tota
-00001380: 6c5f 636f 756e 74da 1363 7265 6174 655f  l_count..create_
-00001390: 7068 616e 746f 6d5f 726f 7773 da05 6c69  phantom_rows..li
-000013a0: 6d69 74da 036c 656e da04 6469 6374 7275  mit..len..dictru
-000013b0: 0000 00da 0967 6574 5f74 6974 6c65 da0d  .....get_title..
-000013c0: 6765 745f 6d61 696e 5f63 6172 64da 0669  get_main_card..i
-000013d0: 6e73 6572 7472 4700 0000 da0a 7061 7261  nsertrG.....para
-000013e0: 6d65 7465 7273 da06 7570 6461 7465 da0d  meters..update..
-000013f0: 7061 7261 6d73 5f6c 6179 6f75 74da 0c70  params_layout..p
-00001400: 6172 616d 735f 7374 6f72 65da 0770 7632  arams_store..pv2
-00001410: 6469 6374 7277 0000 0029 1372 4400 0000  dictrw...).rD...
-00001420: 7245 0000 0072 4600 0000 7247 0000 00da  rE...rF...rG....
-00001430: 0276 6dda 036d 7367 da03 666d 74da 0b61  .vm..msg..fmt..a
-00001440: 6374 696f 6e5f 6e61 6d65 724b 0000 00da  ction_namerK....
-00001450: 0764 6174 6172 6563 7273 0000 0072 7200  .datarecrs...rr.
-00001460: 0000 da03 6f62 6ada 0370 6172 da0b 746f  ....obj..par..to
-00001470: 7461 6c5f 636f 756e 7472 6900 0000 da01  tal_countri.....
-00001480: 64da 026b 77da 026d 6372 3600 0000 2904  d..kw..mcr6...).
-00001490: 724a 0000 0072 6a00 0000 726b 0000 0072  rJ...rj...rk...r
-000014a0: 6c00 0000 7237 0000 0072 7c00 0000 7600  l...r7...r|...v.
-000014b0: 0000 7390 0000 0008 0104 0108 0112 0108  ..s.............
-000014c0: 080a 0108 020c 0206 0106 0204 0108 0104  ................
-000014d0: fe0e 0404 020e 010c 020e 0108 010e 0108  ................
-000014e0: 0106 0208 0104 ff0a 0304 0104 010a 010e  ................
-000014f0: 0112 0102 fe0a 0304 0104 010a 010a 010c  ................
-00001500: 010a 0208 0612 0102 f504 0d0e 010c 0f04  ................
-00001510: 0106 ff08 030a 010c 012a 010a 010a 010a  .........*......
-00001520: 0104 0202 0102 0102 0104 0106 0106 fb0c  ................
-00001530: 0608 010a 010c 010a 0104 010a 0106 0102  ................
-00001540: ff06 ff08 030e 027a 0b41 7069 4c69 7374  .......z.ApiList
-00001550: 2e67 6574 2902 4e4e 2905 7256 0000 0072  .get).NN).rV...r
-00001560: 5700 0000 7258 0000 0072 4c00 0000 727c  W...rX...rL...r|
-00001570: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
-00001580: 0000 7237 0000 0072 5900 0000 6f00 0000  ..r7...rY...o...
-00001590: 7306 0000 0008 000a 010e 0672 5900 0000  s..........rY...
-000015a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000015b0: 0002 0000 0040 0000 00f3 1800 0000 6500  .....@........e.
-000015c0: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
-000015d0: 5a04 6404 5300 2905 da0f 4368 6f69 6365  Z.d.S.)...Choice
-000015e0: 4c69 7374 4d6f 6465 6c7a a20a 2020 2020  ListModelz..    
-000015f0: 4372 6561 7465 7320 6120 6c61 7267 6520  Creates a large 
-00001600: 4a53 4f4e 206d 6f64 656c 2074 6861 7420  JSON model that 
-00001610: 636f 6e74 6169 6e73 2061 6c6c 2074 6865  contains all the
-00001620: 2063 686f 6963 656c 6973 7473 202b 2063   choicelists + c
-00001630: 686f 6963 6573 0a0a 2020 2020 4e6f 7465  hoices..    Note
-00001640: 3a20 5468 6973 2063 6f75 6c64 2062 6520  : This could be 
-00001650: 696d 7072 6f76 6564 2c20 6f72 206d 6967  improved, or mig
-00001660: 6874 2063 6175 7365 2069 7373 7565 7320  ht cause issues 
-00001670: 6475 6520 746f 2063 6861 6e67 696e 6720  due to changing 
-00001680: 6c61 6e67 7561 6765 0a20 2020 2063 0200  language.    c..
-00001690: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-000016a0: 0000 4300 0000 731c 0000 0064 0164 0284  ..C...s....d.d..
-000016b0: 0074 006a 01a0 02a1 0044 0083 017d 0274  .t.j.....D...}.t
-000016c0: 037c 0283 0153 0029 034e 6301 0000 0000  .|...S.).Nc.....
-000016d0: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
-000016e0: 0000 0073 2400 0000 6900 7c00 5d0e 7d01  ...s$...i.|.].}.
-000016f0: 7400 7c01 8301 6400 6401 8400 7c01 a001  t.|...d.d...|...
-00001700: a100 4400 8301 9302 7102 5300 2902 6301  ..D.....q.S.).c.
-00001710: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00001720: 0000 0053 0000 0073 3200 0000 6700 7c00  ...S...s2...g.|.
-00001730: 5d15 7d01 7400 7c01 6400 1900 8301 a001  ].}.t.|.d.......
-00001740: 6401 a101 7400 7c01 6402 1900 8301 a001  d...t.|.d.......
-00001750: 6401 a101 6403 9c02 9102 7102 5300 2904  d...d.....q.S.).
-00001760: 7201 0000 00fa 0122 7270 0000 0029 0272  r......"rp...).r
-00001770: 3300 0000 da04 7465 7874 2902 7215 0000  3.....text).r...
-00001780: 00da 0573 7472 6970 2902 726e 0000 00da  ...strip).rn....
-00001790: 0163 7236 0000 0072 3600 0000 7237 0000  .cr6...r6...r7..
-000017a0: 0072 6f00 0000 e800 0000 7302 0000 0032  .ro.......s....2
-000017b0: 007a 3243 686f 6963 654c 6973 744d 6f64  .z2ChoiceListMod
-000017c0: 656c 2e67 6574 2e3c 6c6f 6361 6c73 3e2e  el.get.<locals>.
-000017d0: 3c64 6963 7463 6f6d 703e 2e3c 6c69 7374  <dictcomp>.<list
-000017e0: 636f 6d70 3e29 02da 0373 7472 da0b 6765  comp>)...str..ge
-000017f0: 745f 6368 6f69 6365 7329 0272 6e00 0000  t_choices).rn...
-00001800: da02 636c 7236 0000 0072 3600 0000 7237  ..clr6...r6...r7
-00001810: 0000 00da 0a3c 6469 6374 636f 6d70 3ee8  .....<dictcomp>.
-00001820: 0000 0073 0600 0000 0600 0201 1cff 7a27  ...s..........z'
-00001830: 4368 6f69 6365 4c69 7374 4d6f 6465 6c2e  ChoiceListModel.
-00001840: 6765 742e 3c6c 6f63 616c 733e 2e3c 6469  get.<locals>.<di
-00001850: 6374 636f 6d70 3e29 0472 2600 0000 da0b  ctcomp>).r&.....
-00001860: 4348 4f49 4345 4c49 5354 53da 0676 616c  CHOICELISTS..val
-00001870: 7565 7372 2100 0000 2903 7244 0000 0072  uesr!...).rD...r
-00001880: 4500 0000 7249 0000 0072 3600 0000 7236  E...rI...r6...r6
-00001890: 0000 0072 3700 0000 727c 0000 00e7 0000  ...r7...r|......
-000018a0: 0073 0800 0000 0601 0802 06fe 0803 7a13  .s............z.
-000018b0: 4368 6f69 6365 4c69 7374 4d6f 6465 6c2e  ChoiceListModel.
-000018c0: 6765 744e a905 7256 0000 0072 5700 0000  getN..rV...rW...
-000018d0: 7258 0000 00da 075f 5f64 6f63 5f5f 727c  rX.....__doc__r|
-000018e0: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
-000018f0: 0000 7237 0000 0072 a500 0000 e000 0000  ..r7...r........
-00001900: f306 0000 0008 0004 010c 0672 a500 0000  ...........r....
-00001910: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001920: 0003 0000 0040 0000 00f3 1600 0000 6500  .....@........e.
-00001930: 5a01 6400 5a02 6404 6402 6403 8401 5a03  Z.d.Z.d.d.d...Z.
-00001940: 6401 5300 2905 da07 4368 6f69 6365 734e  d.S.)...ChoicesN
-00001950: 6305 0000 0000 0000 0000 0000 000b 0000  c...............
-00001960: 0008 0000 004b 0000 0073 7c00 0000 7400  .....K...s|...t.
-00001970: 7c02 7c03 8302 7d06 6401 7d07 7c04 6401  |.|...}.d.}.|.d.
-00001980: 7500 7219 7c06 6a01 7c01 6402 8d01 7d08  u.r.|.j.|.d...}.
-00001990: 7c08 6a02 7d09 6403 6404 8400 7d0a 6e1b  |.j.}.d.d...}.n.
-000019a0: 7c06 a003 7c04 a101 7022 7c06 a004 7c04  |...|...p"|...|.
-000019b0: a101 7d04 7c04 6a05 7228 6405 7d07 7406  ..}.|.j.r(d.}.t.
-000019c0: 7c06 6a01 7c01 6402 8d01 7c06 7c04 8303  |.j.|.d...|.|...
-000019d0: 5c02 7d09 7d0a 7407 7c06 7c01 7c09 7c0a  \.}.}.t.|.|.|.|.
-000019e0: 7c07 7c04 6406 8d06 5300 2907 6141 0100  |.|.d...S.).aA..
-000019f0: 0049 6620 6066 6c64 6e61 6d65 6020 6973  .If `fldname` is
-00001a00: 2073 7065 6369 6669 6564 2c20 7265 7475   specified, retu
-00001a10: 726e 2061 204a 534f 4e20 6f62 6a65 6374  rn a JSON object
-00001a20: 2077 6974 6820 7477 6f0a 2020 2020 2020   with two.      
-00001a30: 2020 6174 7472 6962 7574 6573 2060 636f    attributes `co
-00001a40: 756e 7460 2061 6e64 2060 726f 7773 602c  unt` and `rows`,
-00001a50: 2077 6865 7265 2060 726f 7773 6020 6973   where `rows` is
-00001a60: 2061 206c 6973 7420 6f66 0a20 2020 2020   a list of.     
-00001a70: 2020 2060 2864 6973 706c 6179 5f74 6578     `(display_tex
-00001a80: 742c 2076 616c 7565 2960 2074 7570 6c65  t, value)` tuple
-00001a90: 732e 2020 5573 6564 2062 7920 436f 6d62  s.  Used by Comb
-00001aa0: 6f42 6f78 6573 206f 7220 7369 6d69 6c61  oBoxes or simila
-00001ab0: 720a 2020 2020 2020 2020 7769 6467 6574  r.        widget
-00001ac0: 732e 0a0a 2020 2020 2020 2020 4966 2060  s...        If `
-00001ad0: 666c 646e 616d 6560 2069 7320 6e6f 7420  fldname` is not 
-00001ae0: 7370 6563 6966 6965 642c 2072 6574 7572  specified, retur
-00001af0: 6e73 2074 6865 2063 686f 6963 6573 2066  ns the choices f
-00001b00: 6f72 2074 6865 0a20 2020 2020 2020 2060  or the.        `
-00001b10: 7265 636f 7264 5f73 656c 6563 746f 7260  record_selector`
-00001b20: 2077 6964 6765 742e 0a0a 2020 2020 2020   widget...      
-00001b30: 2020 4ea9 0172 4500 0000 6302 0000 0000    N..rE...c.....
-00001b40: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001b50: 0000 0073 1e00 0000 7400 7c00 8301 7c01  ...s....t.|...|.
-00001b60: 7401 6a02 3c00 7c00 6a03 7c01 7401 6a04  t.j.<.|.j.|.t.j.
-00001b70: 3c00 7c01 5300 a901 4e29 0572 aa00 0000  <.|.S...N).r....
-00001b80: 721b 0000 00da 1243 484f 4943 4553 5f54  r......CHOICES_T
-00001b90: 4558 545f 4649 454c 4472 4800 0000 da13  EXT_FIELDrH.....
-00001ba0: 4348 4f49 4345 535f 5641 4c55 455f 4649  CHOICES_VALUE_FI
-00001bb0: 454c 4429 0272 9e00 0000 72a1 0000 0072  ELD).r....r....r
-00001bc0: 3600 0000 7236 0000 0072 3700 0000 7267  6...r6...r7...rg
-00001bd0: 0000 0007 0100 0073 0600 0000 0e01 0c02  .......s........
-00001be0: 0401 7a1d 4368 6f69 6365 732e 6765 742e  ..z.Choices.get.
-00001bf0: 3c6c 6f63 616c 733e 2e72 6f77 3264 6963  <locals>.row2dic
-00001c00: 7472 5c00 0000 a901 da05 6669 656c 6429  tr\.......field)
-00001c10: 0872 1f00 0000 7245 0000 00da 0d64 6174  .r....rE.....dat
-00001c20: 615f 6974 6572 6174 6f72 da0e 6765 745f  a_iterator..get_
-00001c30: 7061 7261 6d5f 656c 656d da0d 6765 745f  param_elem..get_
-00001c40: 6461 7461 5f65 6c65 6dda 0562 6c61 6e6b  data_elem..blank
-00001c50: 7218 0000 0072 2300 0000 290b 7244 0000  r....r#...).rD..
-00001c60: 0072 4500 0000 7246 0000 0072 4700 0000  .rE...rF...rG...
-00001c70: 72ba 0000 0072 a200 0000 da03 7270 74da  r....r......rpt.
-00001c80: 0a65 6d70 7479 5661 6c75 6572 4a00 0000  .emptyValuerJ...
-00001c90: da02 7173 7267 0000 0072 3600 0000 7236  ..qsrg...r6...r6
-00001ca0: 0000 0072 3700 0000 727c 0000 00f0 0000  ...r7...r|......
-00001cb0: 0073 1600 0000 0a0a 0401 0801 0c01 0606  .s..............
-00001cc0: 0a04 1409 0601 0402 1801 1402 7a0b 4368  ............z.Ch
-00001cd0: 6f69 6365 732e 6765 7472 5500 0000 a904  oices.getrU.....
-00001ce0: 7256 0000 0072 5700 0000 7258 0000 0072  rV...rW...rX...r
-00001cf0: 7c00 0000 7236 0000 0072 3600 0000 7236  |...r6...r6...r6
-00001d00: 0000 0072 3700 0000 72b4 0000 00ef 0000  ...r7...r.......
-00001d10: 00f3 0400 0000 0800 0e01 72b4 0000 0063  ..........r....c
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 0300 0000 4000 0000 72b3 0000 0029 05da  ....@...r....)..
-00001d40: 0c44 656c 6179 6564 5661 6c75 654e 6306  .DelayedValueNc.
-00001d50: 0000 0000 0000 0000 0000 000d 0000 0005  ................
-00001d60: 0000 004b 0000 0073 9e00 0000 7400 7c02  ...K...s....t.|.
-00001d70: 7c03 8302 7d07 7c07 a001 7c05 a101 7d08  |...}.|...|...}.
-00001d80: 7c08 6400 7500 7215 6401 a002 7c07 7c05  |.d.u.r.d...|.|.
-00001d90: a102 7d09 6e34 7c07 6a03 7c01 7404 6a05  ..}.n4|.j.|.t.j.
-00001da0: 6a06 6a07 6a08 6402 8d02 7d0a 7c04 6403  j.j.j.d...}.|.d.
-00001db0: 6b02 7227 6400 7d0b 6e0a 7c0a a009 7c04  k.r'd.}.n.|...|.
-00001dc0: a101 0100 7c0a 6a0a 6404 1900 7d0b 740b  ....|.j.d...}.t.
-00001dd0: 7c07 7c08 7c05 8303 7d0c 7c0c 6400 7500  |.|.|...}.|.d.u.
-00001de0: 7243 6405 a002 7c07 7c08 7c05 a103 7d09  rCd...|.|.|...}.
-00001df0: 6e06 7c0c a00c 7c0b 7c0a a102 7d09 740d  n.|...|.|...}.t.
-00001e00: 6406 7c09 6901 8301 5300 2907 4e7a 197b  d.|.i...S.).Nz.{
-00001e10: 7d20 6861 7320 6e6f 2064 6174 6120 656c  } has no data el
-00001e20: 656d 656e 7420 7b7d a902 7245 0000 0072  ement {}..rE...r
-00001e30: 3a00 0000 723b 0000 0072 0100 0000 7a2c  :...r;...r....z,
-00001e40: 4f6f 7073 2c20 6765 745f 6174 6f6d 697a  Oops, get_atomiz
-00001e50: 6572 287b 7d2c 207b 7d2c 207b 7d29 2072  er({}, {}, {}) r
-00001e60: 6574 7572 6e65 6420 4e6f 6e65 7249 0000  eturned NonerI..
-00001e70: 0029 0e72 1f00 0000 72bd 0000 0072 7a00  .).r....r....rz.
-00001e80: 0000 7245 0000 0072 0b00 0000 723d 0000  ..rE...r....r=..
-00001e90: 0072 3e00 0000 723f 0000 0072 3a00 0000  .r>...r?...r:...
-00001ea0: 7242 0000 0072 4100 0000 7227 0000 00da  rB...rA...r'....
-00001eb0: 1666 756c 6c5f 7661 6c75 655f 6672 6f6d  .full_value_from
-00001ec0: 5f6f 626a 6563 7472 2100 0000 290d 7244  _objectr!...).rD
-00001ed0: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
-00001ee0: 0000 7248 0000 0072 ba00 0000 72a2 0000  ..rH...r....r...
-00001ef0: 0072 bf00 0000 da02 6465 da01 7672 4a00  .r......de..vrJ.
-00001f00: 0000 7269 0000 00da 0273 6672 3600 0000  ..ri.....sfr6...
-00001f10: 7236 0000 0072 3700 0000 727c 0000 001a  r6...r7...r|....
-00001f20: 0100 0073 1c00 0000 0a01 0a07 0801 0e01  ...s............
-00001f30: 1602 0801 0601 0a02 0a01 0c02 0801 1001  ................
-00001f40: 0c02 0c03 7a10 4465 6c61 7965 6456 616c  ....z.DelayedVal
-00001f50: 7565 2e67 6574 a904 4e4e 4e4e 72c2 0000  ue.get..NNNNr...
-00001f60: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-00001f70: 7237 0000 0072 c400 0000 1901 0000 72c3  r7...r........r.
-00001f80: 0000 0072 c400 0000 6300 0000 0000 0000  ...r....c.......
-00001f90: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00001fa0: 0072 b300 0000 2905 da12 4163 7469 6f6e  .r....)...Action
-00001fb0: 5061 7261 6d43 686f 6963 6573 4e63 0600  ParamChoicesNc..
-00001fc0: 0000 0000 0000 0000 0000 0b00 0000 0800  ................
-00001fd0: 0000 4b00 0000 7376 0000 0074 007c 027c  ..K...sv...t.|.|
-00001fe0: 0383 027d 037c 03a0 017c 04a1 017d 077c  ...}.|...|...}.|
-00001ff0: 0764 0075 0072 1674 0264 017c 047c 0366  .d.u.r.t.d.|.|.f
-00002000: 0216 0083 0182 017c 076a 03a0 047c 05a1  .......|.j...|..
-00002010: 017d 0574 057c 076a 067c 0164 028d 017c  .}.t.|.j.|.d...|
-00002020: 076a 037c 0583 035c 027d 087d 097c 056a  .j.|...\.}.}.|.j
-00002030: 0772 2f64 037d 0a6e 0264 007d 0a74 087c  .r/d.}.n.d.}.t.|
-00002040: 037c 017c 087c 097c 0a7c 0564 048d 0653  .|.|.|.|.|.d...S
-00002050: 0029 054e 7a18 556e 6b6e 6f77 6e20 6163  .).Nz.Unknown ac
-00002060: 7469 6f6e 2025 7220 666f 7220 2573 72b5  tion %r for %sr.
-00002070: 0000 007a 053c 6272 2f3e 72b9 0000 0029  ...z.<br/>r....)
-00002080: 0972 1f00 0000 da0e 6765 745f 7572 6c5f  .r......get_url_
-00002090: 6163 7469 6f6e da09 4578 6365 7074 696f  action..Exceptio
-000020a0: 6e72 7f00 0000 72bc 0000 0072 1800 0000  nr....r....r....
-000020b0: 7245 0000 0072 be00 0000 7223 0000 0029  rE...r....r#...)
-000020c0: 0b72 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
-000020d0: 7247 0000 00da 0261 6e72 ba00 0000 72a2  rG.....anr....r.
-000020e0: 0000 00da 0262 6172 c100 0000 7267 0000  .....bar....rg..
-000020f0: 0072 c000 0000 7236 0000 0072 3600 0000  .r....r6...r6...
-00002100: 7237 0000 0072 7c00 0000 3a01 0000 7314  r7...r|...:...s.
-00002110: 0000 000a 010a 0108 0110 010c 011a 0106  ................
-00002120: 0106 0104 0214 017a 1641 6374 696f 6e50  .......z.ActionP
-00002130: 6172 616d 4368 6f69 6365 732e 6765 7472  aramChoices.getr
-00002140: ca00 0000 72c2 0000 0072 3600 0000 7236  ....r....r6...r6
-00002150: 0000 0072 3600 0000 7237 0000 0072 cb00  ...r6...r7...r..
-00002160: 0000 3801 0000 7304 0000 0008 000e 0272  ..8...s........r
-00002170: cb00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00002180: 0000 0000 0003 0000 0040 0000 0073 2e00  .........@...s..
-00002190: 0000 6500 5a01 6400 5a02 6401 5a03 6409  ..e.Z.d.Z.d.Z.d.
-000021a0: 6403 6404 8401 5a04 6409 6405 6406 8401  d.d...Z.d.d.d...
-000021b0: 5a05 6409 6407 6408 8401 5a06 6402 5300  Z.d.d.d...Z.d.S.
-000021c0: 290a da07 5265 7374 6675 6c7a 3c0a 2020  )...Restfulz<.  
-000021d0: 2020 5573 6564 2074 6f20 636f 6c6c 6162    Used to collab
-000021e0: 6f72 6174 6520 7769 7468 2061 2072 6573  orate with a res
-000021f0: 7466 756c 2045 7874 2e64 6174 612e 5374  tful Ext.data.St
-00002200: 6f72 652e 0a20 2020 204e 6305 0000 0000  ore..    Nc.....
-00002210: 0000 0000 0000 0009 0000 0006 0000 0043  ...............C
-00002220: 0000 0073 8800 0000 7400 7c02 7c03 8302  ...s....t.|.|...
-00002230: 7d05 7c05 6a01 7c01 6401 8d01 7d06 7c06  }.|.j.|.d...}.|.
-00002240: a002 a100 7d07 7c06 6a03 6a04 6400 7501  ....}.|.j.j.d.u.
-00002250: 721c 7c06 6a03 a004 7c07 7c01 a102 0100  r.|.j...|.|.....
-00002260: 7c01 6a05 a006 6402 a101 7d08 7407 a008  |.j...d...}.t...
-00002270: 7c08 a101 7d08 7c06 a009 7c08 7c07 6403  |...}.|...|.|.d.
-00002280: a103 0100 7c06 6a0a 7c06 6a0b 6a0c a00d  ....|.j.|.j.j...
-00002290: 7c06 7c07 7c06 6a0b 6a0c 6a0e a103 6701  |.|.|.j.j.j...g.
-000022a0: 6404 8d01 0100 740f 7c06 6a10 8301 5300  d.....t.|.j...S.
-000022b0: 2905 4e72 b500 0000 7272 0000 0054 a901  ).Nr....rr...T..
-000022c0: 7272 0000 0029 1172 1f00 0000 7245 0000  rr...).r....rE..
-000022d0: 0072 4000 0000 7247 0000 00da 1568 616e  .r@...rG.....han
-000022e0: 646c 655f 7570 6c6f 6164 6564 5f66 696c  dle_uploaded_fil
-000022f0: 6573 723c 0000 0072 7c00 0000 da04 6a73  esr<...r|.....js
-00002300: 6f6e da05 6c6f 6164 73da 1166 6f72 6d32  on..loads..form2
-00002310: 6f62 6a5f 616e 645f 7361 7665 da0c 7365  obj_and_save..se
-00002320: 745f 7265 7370 6f6e 7365 727b 0000 0072  t_responser{...r
-00002330: 6000 0000 7267 0000 00da 0b6c 6973 745f  `...rg.....list_
-00002340: 6669 656c 6473 7221 0000 00da 0872 6573  fieldsr!.....res
-00002350: 706f 6e73 6529 0972 4400 0000 7245 0000  ponse).rD...rE..
-00002360: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
-00002370: 72bf 0000 0072 4a00 0000 da08 696e 7374  r....rJ.....inst
-00002380: 616e 6365 7249 0000 0072 3600 0000 7236  ancerI...r6...r6
-00002390: 0000 0072 3700 0000 724c 0000 004d 0100  ...r7...rL...M..
-000023a0: 0073 1c00 0000 0a01 0c01 0802 0c03 0e01  .s..............
-000023b0: 0c02 0a01 0e01 0403 0801 0c01 04ff 06ff  ................
-000023c0: 0a03 7a0c 5265 7374 6675 6c2e 706f 7374  ..z.Restful.post
-000023d0: 6305 0000 0000 0000 0000 0000 000f 0000  c...............
-000023e0: 0005 0000 0003 0000 0073 6201 0000 7400  .........sb...t.
-000023f0: 7c02 7c03 8302 7d05 7c01 6a01 a002 7403  |.|...}.|.j...t.
-00002400: 6a04 6401 a102 7d06 7c01 6a01 a002 7403  j.d...}.|.j...t.
-00002410: 6a05 7403 6a06 a102 7d07 7c01 6a01 a007  j.t.j...}.|.j...
-00002420: 7403 6a08 a101 7d08 7c08 7322 7c04 6701  t.j...}.|.s"|.g.
-00002430: 7d08 7c05 6a09 7c01 7c08 6402 8d02 8900  }.|.j.|.|.d.....
-00002440: 7c04 6401 7500 7251 8800 6a0a 8901 8700  |.d.u.rQ..j.....
-00002450: 8701 6602 6403 6404 8408 8800 6a0b 4400  ..f.d.d.....j.D.
-00002460: 8301 7d09 740c 8800 a00d a100 7c09 6405  ..}.t.......|.d.
-00002470: 8d02 7d0a 7c0a 6a0e 740f 8800 a010 a100  ..}.|.j.t.......
-00002480: 8301 6406 8d01 0100 7411 7c0a 8301 5300  ..d.....t.|...S.
-00002490: 7c06 7259 7c05 a012 7c06 a101 7d0b 6e03  |.rY|...|...}.n.
-000024a0: 7c05 6a13 7d0b 8800 6a0a 7d0c 7c0b 6a09  |.j.}...j.}.|.j.
-000024b0: 7c01 7c08 6402 8d02 8900 8800 6a14 6407  |.|.d.......j.d.
-000024c0: 1900 7d0d 7c07 7403 6a06 6b02 72af 7c04  ..}.|.t.j.k.r.|.
-000024d0: 6408 6b02 7282 8800 a015 a100 7d0d 8800  d.k.r.......}...
-000024e0: a016 7c0c 7c0d a102 7d0e 7411 7c0e 8301  ..|.|...}.t.|...
-000024f0: 5300 7c04 6409 6b02 7294 8800 a015 a100  S.|.d.k.r.......
-00002500: 7d0d 7417 8800 7c0c 7c0d 8303 7d0e 7411  }.t...|.|...}.t.
-00002510: 7c0e 8301 5300 7c0d 6401 7500 72a6 740c  |...S.|.d.u.r.t.
-00002520: 640a 7418 7c05 7c04 6602 1600 640b 8d02  d.t.|.|.f...d...
-00002530: 7d0e 7411 7c0e 8301 5300 8800 a019 7c0d  }.t.|...S.....|.
-00002540: a101 7d0e 7411 7c0e 8301 5300 6401 5300  ..}.t.|...S.d.S.
-00002550: 290c 7a3b 0a20 2020 2020 2020 2057 6f72  ).z;.        Wor
-00002560: 6b73 2c20 6275 7420 6973 2075 676c 7920  ks, but is ugly 
-00002570: 746f 2067 6574 206c 6973 7420 616e 6420  to get list and 
-00002580: 6465 7461 696c 0a20 2020 2020 2020 204e  detail.        N
-00002590: 2902 7245 0000 00da 0c73 656c 6563 7465  ).rE.....selecte
-000025a0: 645f 706b 7363 0100 0000 0000 0000 0000  d_pksc..........
-000025b0: 0000 0200 0000 0700 0000 1300 0000 7320  ..............s 
-000025c0: 0000 0067 007c 005d 0c7d 0188 016a 00a0  ...g.|.].}...j..
-000025d0: 0188 007c 0188 016a 006a 02a1 0391 0271  ...|...j.j.....q
-000025e0: 0253 0072 3600 0000 2903 7260 0000 0072  .S.r6...).r`...r
-000025f0: 6700 0000 da0a 616c 6c5f 6669 656c 6473  g.....all_fields
-00002600: 726d 0000 00a9 0272 4a00 0000 726b 0000  rm.....rJ...rk..
-00002610: 0072 3600 0000 7237 0000 0072 6f00 0000  .r6...r7...ro...
-00002620: 7601 0000 7308 0000 0006 0002 0212 ff06  v...s...........
-00002630: ff7a 1f52 6573 7466 756c 2e67 6574 2e3c  .z.Restful.get.<
-00002640: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002650: 703e 2902 7271 0000 0072 7200 0000 2901  p>).rq...rr...).
-00002660: 7276 0000 0072 0100 0000 7a06 2d39 3939  rv...r....z.-999
-00002670: 3939 723b 0000 0046 2902 7274 0000 00da  99r;...F).rt....
-00002680: 076d 6573 7361 6765 291a 721f 0000 0072  .message).r....r
-00002690: 7800 0000 727c 0000 0072 1b00 0000 7281  x...r|...r....r.
-000026a0: 0000 0072 7d00 0000 7282 0000 00da 0767  ...r}...r......g
-000026b0: 6574 6c69 7374 da12 5552 4c5f 5041 5241  etlist..URL_PARA
-000026c0: 4d5f 5345 4c45 4354 4544 7245 0000 0072  M_SELECTEDrE...r
-000026d0: 7b00 0000 7286 0000 0072 9000 0000 728c  {...r....r....r.
-000026e0: 0000 0072 9500 0000 72aa 0000 0072 9100  ...r....r....r..
-000026f0: 0000 7221 0000 0072 cc00 0000 da0d 6465  ..r!...r......de
-00002700: 7461 696c 5f61 6374 696f 6e72 4100 0000  tail_actionrA...
-00002710: 7240 0000 00da 0f65 6c65 6d32 7265 635f  r@.....elem2rec_
-00002720: 696e 7365 7274 722d 0000 00da 094e 4f54  insertr-.....NOT
-00002730: 5f46 4f55 4e44 da11 656c 656d 3272 6563  _FOUND..elem2rec
-00002740: 5f64 6574 6169 6c65 6429 0f72 4400 0000  _detailed).rD...
-00002750: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
-00002760: 4800 0000 72bf 0000 0072 9c00 0000 729b  H...r....r....r.
-00002770: 0000 00da 0273 7272 7200 0000 72a2 0000  .....srrr...r...
-00002780: 0072 cf00 0000 727b 0000 0072 4b00 0000  .r....r{...rK...
-00002790: 729d 0000 0072 3600 0000 72dc 0000 0072  r....r6...r....r
-000027a0: 3700 0000 727c 0000 0067 0100 0073 5000  7...r|...g...sP.
-000027b0: 0000 0a04 1002 0601 0801 04ff 0e02 0401  ................
-000027c0: 0601 0e01 0801 0601 0c01 0402 06fe 1003  ................
-000027d0: 1401 0801 0403 0c01 0602 0601 0e01 0a01  ................
-000027e0: 0a01 0801 0801 0c01 0809 08f8 0801 0c01  ................
-000027f0: 0806 08fb 0201 0c01 06ff 0804 0aff 0801  ................
-00002800: 04f4 7a0b 5265 7374 6675 6c2e 6765 7463  ..z.Restful.getc
-00002810: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
-00002820: 0600 0000 4300 0000 73a8 0000 0074 007c  ....C...s....t.|
-00002830: 027c 0383 027d 057c 056a 017c 0164 018d  .|...}.|.j.|.d..
-00002840: 017d 067c 06a0 027c 04a1 0101 007c 066a  .}.|...|.....|.j
-00002850: 0364 0219 007d 077c 066a 047d 0874 05a0  .d...}.|.j.}.t..
-00002860: 067c 016a 07a1 01a0 0864 03a1 017d 0974  .|.j.....d...}.t
-00002870: 09a0 0a7c 09a1 017d 097c 05a0 0b7c 056a  ...|...}.|...|.j
-00002880: 0ca1 017d 0a7c 056a 017c 017c 0a64 048d  ...}.|.j.|.|.d..
-00002890: 027d 0674 0d6a 0e6a 0f6a 107c 065f 117c  .}.t.j.j.j.|._.|
-000028a0: 06a0 127c 097c 0764 05a1 0301 007c 066a  ...|.|.d.....|.j
-000028b0: 137c 086a 14a0 157c 067c 077c 086a 146a  .|.j...|.|.|.j.j
-000028c0: 16a1 0367 0164 068d 0101 0074 177c 066a  ...g.d.....t.|.j
-000028d0: 1883 0153 0029 074e 72b5 0000 0072 0100  ...S.).Nr....r..
-000028e0: 0000 7272 0000 0029 0272 4500 0000 727f  ..rr...).rE...r.
-000028f0: 0000 0046 72d1 0000 0029 1972 1f00 0000  ...Fr....).r....
-00002900: 7245 0000 0072 4200 0000 7241 0000 0072  rE...rB...rA...r
-00002910: 7b00 0000 7209 0000 0072 5000 0000 7251  {...r....rP...rQ
-00002920: 0000 0072 7c00 0000 72d3 0000 0072 d400  ...r|...r....r..
-00002930: 0000 72cc 0000 00da 1864 6566 6175 6c74  ..r......default
-00002940: 5f6c 6973 745f 6163 7469 6f6e 5f6e 616d  _list_action_nam
-00002950: 6572 0b00 0000 723d 0000 0072 2600 0000  er....r=...r&...
-00002960: da0e 6578 746a 735f 7265 6e64 6572 6572  ..extjs_renderer
-00002970: 723a 0000 0072 d500 0000 72d6 0000 0072  r:...r....r....r
-00002980: 6000 0000 7267 0000 0072 d700 0000 7221  `...rg...r....r!
-00002990: 0000 0072 d800 0000 290b 7244 0000 0072  ...r....).rD...r
-000029a0: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
-000029b0: 0000 0072 bf00 0000 724a 0000 0072 4b00  ...r....rJ...rK.
-000029c0: 0000 726b 0000 0072 4900 0000 da01 6172  ..rk...rI.....ar
-000029d0: 3600 0000 7236 0000 0072 3700 0000 7253  6...r6...r7...rS
-000029e0: 0000 0093 0100 0073 1e00 0000 0a01 0c01  .......s........
-000029f0: 0a01 0a01 0601 1202 0a01 0c01 0e01 0c01  ................
-00002a00: 0e01 0402 1401 06ff 0a02 7a0b 5265 7374  ..........z.Rest
-00002a10: 6675 6c2e 7075 7472 5500 0000 2907 7256  ful.putrU...).rV
-00002a20: 0000 0072 5700 0000 7258 0000 0072 b100  ...rW...rX...r..
-00002a30: 0000 724c 0000 0072 7c00 0000 7253 0000  ..rL...r|...rS..
-00002a40: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-00002a50: 7237 0000 0072 d000 0000 4801 0000 730a  r7...r....H...s.
-00002a60: 0000 0008 0004 010a 040a 1a0e 2c72 d000  ............,r..
-00002a70: 0000 6303 0000 0000 0000 0000 0000 0009  ..c.............
-00002a80: 0000 0005 0000 0043 0000 0073 7000 0000  .......C...sp...
-00002a90: 7c00 a000 a100 7d03 7401 8300 7d04 7c03  |.....}.t...}.|.
-00002aa0: 6a02 7c04 6602 7d05 7c00 6a03 6406 6900  j.|.f.}.|.j.d.i.
-00002ab0: 7c02 a401 8e01 7d02 7c00 7c02 6401 3c00  |.....}.|.|.d.<.
-00002ac0: 7c00 6a04 7c02 6402 3c00 7405 6a06 6a07  |.j.|.d.<.t.j.j.
-00002ad0: 6a08 6a09 6a0a 7d06 7c06 a00b 7c01 a101  j.j.j.}.|...|...
-00002ae0: 7d07 740c 6a0d 7c07 6a0e 6406 6900 7c02  }.t.j.|.j.d.i.|.
-00002af0: a401 8e01 6403 6404 8d02 7d08 7c08 5300  ....d.d...}.|.S.
-00002b00: 2907 7a14 4465 7365 7276 6573 2061 2064  ).z.Deserves a d
-00002b10: 6f63 7374 7269 6e67 724a 0000 00da 046d  ocstringrJ.....m
-00002b20: 656d 6ffa 1974 6578 742f 6874 6d6c 3b63  emo..text/html;c
-00002b30: 6861 7273 6574 3d22 7574 662d 3822 a901  harset="utf-8"..
-00002b40: da0c 636f 6e74 656e 745f 7479 7065 4e72  ..content_typeNr
-00002b50: 3600 0000 290f da08 6765 745f 7573 6572  6...)...get_user
-00002b60: 7211 0000 00da 0975 7365 725f 7479 7065  r......user_type
-00002b70: da15 6765 745f 7072 696e 7461 626c 655f  ..get_printable_
-00002b80: 636f 6e74 6578 74da 0a70 6172 7365 5f6d  context..parse_m
-00002b90: 656d 6f72 0b00 0000 723d 0000 0072 3e00  emor....r=...r>.
-00002ba0: 0000 da05 6a69 6e6a 6172 3a00 0000 da09  ....jinjar:.....
-00002bb0: 6a69 6e6a 615f 656e 76da 0c67 6574 5f74  jinja_env..get_t
-00002bc0: 656d 706c 6174 6572 0900 0000 da0c 4874  emplater......Ht
-00002bd0: 7470 5265 7370 6f6e 7365 da06 7265 6e64  tpResponse..rend
-00002be0: 6572 2909 724a 0000 00da 0774 706c 6e61  er).rJ.....tplna
-00002bf0: 6d65 da07 636f 6e74 6578 74da 0175 da04  me..context..u..
-00002c00: 6c61 6e67 da01 6bda 0365 6e76 da08 7465  lang..k..env..te
-00002c10: 6d70 6c61 7465 72d8 0000 0072 3600 0000  mplater....r6...
-00002c20: 7236 0000 0072 3700 0000 da0d 6874 7470  r6...r7.....http
-00002c30: 5f72 6573 706f 6e73 65a6 0100 0073 1a00  _response....s..
-00002c40: 0000 0802 0601 0a01 1001 0801 0a01 0e01  ................
-00002c50: 0a01 0402 0e01 0201 06fe 0404 72fc 0000  ............r...
-00002c60: 0063 0300 0000 0000 0000 0000 0000 0c00  .c..............
-00002c70: 0000 0a00 0000 4300 0000 73ea 0000 007c  ......C...s....|
-00002c80: 006a 0064 1469 007c 02a4 018e 017d 027c  .j.d.i.|.....}.|
-00002c90: 026a 0174 0264 018d 0101 0074 036a 046a  .j.t.d.....t.j.j
-00002ca0: 056a 066a 076a 087d 037a 077c 03a0 097c  .j.j.j.}.z.|...|
-00002cb0: 01a1 017d 0457 006e 1604 0074 0a79 3201  ...}.W.n...t.y2.
-00002cc0: 007d 0501 007a 0a74 0ba0 0ca1 0057 0006  .}...z.t.....W..
-00002cd0: 0059 0064 027d 057e 0553 0064 027d 057e  .Y.d.}.~.S.d.}.~
-00002ce0: 0577 0177 0064 0364 0484 007d 067c 026a  .w.w.d.d...}.|.j
-00002cf0: 017c 0664 058d 0101 0064 0664 0784 007d  .|.d.....d.d...}
-00002d00: 0764 0864 0984 007d 0864 0a64 0b84 007d  .d.d...}.d.d...}
-00002d10: 097c 036a 0da0 0174 0e7c 077c 087c 0964  .|.j...t.|.|.|.d
-00002d20: 0c8d 03a1 0101 007c 01a0 0f64 0da1 0172  .......|...d...r
-00002d30: 5b64 0e6e 087c 01a0 0f64 0fa1 0172 6264  [d.n.|...d...rbd
-00002d40: 106e 0164 117d 0a74 0b6a 107c 046a 1164  .n.d.}.t.j.|.j.d
-00002d50: 1469 007c 02a4 018e 017c 0a64 1217 0064  .i.|.....|.d...d
-00002d60: 138d 027d 0b7c 0b53 0029 157a 6a0a 2020  ...}.|.S.).zj.  
-00002d70: 2020 5265 7370 6f6e 6520 7573 6564 2066    Respone used f
-00002d80: 6f72 2072 656e 6465 7269 6e67 2058 4d4c  or rendering XML
-00002d90: 2076 6965 7773 2069 6e20 7265 6163 742e   views in react.
-00002da0: 0a20 2020 2049 6e63 6c75 6465 7320 736f  .    Includes so
-00002db0: 6d65 2068 656c 7065 7220 6675 6e63 7469  me helper functi
-00002dc0: 6f6e 7320 666f 7220 7265 6e64 6572 696e  ons for renderin
-00002dd0: 672e 0a20 2020 2072 1a00 0000 4e63 0000  g..    r....Nc..
-00002de0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00002df0: 0000 5700 0000 7320 0000 0064 0164 0284  ..W...s ...d.d..
-00002e00: 007c 0044 0083 017d 0064 0364 04a0 007c  .|.D...}.d.d...|
-00002e10: 00a1 0117 0064 0517 0053 0029 067a 2748  .....d...S.).z'H
-00002e20: 656c 7065 7220 6675 6e63 7469 6f6e 2074  elper function t
-00002e30: 6f20 7772 6170 2061 2073 7472 696e 6720  o wrap a string 
-00002e40: 696e 207b 7d73 6301 0000 0000 0000 0000  in {}sc.........
-00002e50: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00002e60: 1400 0000 6700 7c00 5d06 7d01 7400 7c01  ....g.|.].}.t.|.
-00002e70: 8301 9102 7102 5300 7236 0000 0029 0172  ....q.S.r6...).r
-00002e80: aa00 0000 2902 726e 0000 0072 e700 0000  ....).rn...r....
-00002e90: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00002ea0: 6f00 0000 cd01 0000 7302 0000 0014 007a  o.......s......z
-00002eb0: 2e58 4d4c 5f72 6573 706f 6e73 652e 3c6c  .XML_response.<l
-00002ec0: 6f63 616c 733e 2e62 696e 642e 3c6c 6f63  ocals>.bind.<loc
-00002ed0: 616c 733e 2e3c 6c69 7374 636f 6d70 3eda  als>.<listcomp>.
-00002ee0: 017b 725c 0000 00da 017d 2901 da04 6a6f  .{r\.....})...jo
-00002ef0: 696e a901 da04 6172 6773 7236 0000 0072  in....argsr6...r
-00002f00: 3600 0000 7237 0000 00da 0462 696e 64cb  6...r7.....bind.
-00002f10: 0100 0073 0400 0000 0e02 1201 7a1a 584d  ...s........z.XM
-00002f20: 4c5f 7265 7370 6f6e 7365 2e3c 6c6f 6361  L_response.<loca
-00002f30: 6c73 3e2e 6269 6e64 2901 7202 0100 0063  ls>.bind).r....c
-00002f40: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00002f50: 0200 0000 5700 0000 730c 0000 0074 007c  ....W...s....t.|
-00002f60: 0083 0101 0064 0153 0029 027a 8844 6562  .....d.S.).z.Deb
-00002f70: 7567 6765 7220 6865 6c70 6572 3b20 7072  ugger helper; pr
-00002f80: 696e 7473 206f 7574 2061 6c6c 2061 7267  ints out all arg
-00002f90: 7320 7075 7420 696e 746f 2074 6865 2066  s put into the f
-00002fa0: 696c 7465 7220 6275 7420 646f 6573 6e27  ilter but doesn'
-00002fb0: 7420 696e 636c 7564 6520 7468 656d 2069  t include them i
-00002fc0: 6e20 7468 6520 7465 6d70 6c61 7465 2e0a  n the template..
-00002fd0: 2020 2020 2020 2020 7573 6167 653a 207b          usage: {
-00002fe0: 7b64 6562 7567 207c 2070 7d7d 0a20 2020  {debug | p}}.   
-00002ff0: 2020 2020 2072 5c00 0000 2901 da05 7072       r\...)...pr
-00003000: 696e 7472 0001 0000 7236 0000 0072 3600  intr....r6...r6.
-00003010: 0000 7237 0000 00da 0170 d201 0000 7304  ..r7.....p....s.
-00003020: 0000 0008 0404 017a 1758 4d4c 5f72 6573  .......z.XML_res
-00003030: 706f 6e73 652e 3c6c 6f63 616c 733e 2e70  ponse.<locals>.p
-00003040: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00003050: 0004 0000 0053 0000 0073 2000 0000 6401  .....S...s ...d.
-00003060: 6402 6c00 7d01 7c01 a001 7402 7c00 8301  d.l.}.|...t.|...
-00003070: a101 7d02 7c02 a003 6403 a101 5300 2904  ..}.|...d...S.).
-00003080: 7ab0 0a20 2020 2020 2020 2043 6f6d 7072  z..        Compr
-00003090: 6573 7320 6120 636f 6d70 6c65 7820 7661  ess a complex va
-000030a0: 6c75 6520 696e 206f 7264 6572 2074 6f20  lue in order to 
-000030b0: 6765 7420 6465 636f 6d70 7265 7373 2062  get decompress b
-000030c0: 7920 7468 6520 636f 6e74 726f 6c6c 6572  y the controller
-000030d0: 2061 6674 6572 7761 7264 730a 2020 2020   afterwards.    
-000030e0: 2020 2020 3a70 6172 616d 2073 3a20 7661      :param s: va
-000030f0: 6c75 6520 746f 2067 6574 2063 6f6d 7072  lue to get compr
-00003100: 6573 7365 642e 0a20 2020 2020 2020 203a  essed..        :
-00003110: 7265 7475 726e 3a20 436f 6d70 7265 7373  return: Compress
-00003120: 6564 2076 616c 7565 2e0a 2020 2020 2020  ed value..      
-00003130: 2020 7201 0000 004e da06 6261 7365 3634    r....N..base64
-00003140: 2904 da04 7a6c 6962 da08 636f 6d70 7265  )...zlib..compre
-00003150: 7373 72aa 0000 00da 0665 6e63 6f64 6529  ssr......encode)
-00003160: 03da 0173 7206 0100 00da 0a63 6f6d 7072  ...sr......compr
-00003170: 6573 7365 6472 3600 0000 7236 0000 0072  essedr6...r6...r
-00003180: 3700 0000 da0d 7a6c 6962 5f63 6f6d 7072  7.....zlib_compr
-00003190: 6573 73d9 0100 0073 0600 0000 0806 0e01  ess....s........
-000031a0: 0a01 7a23 584d 4c5f 7265 7370 6f6e 7365  ..z#XML_response
-000031b0: 2e3c 6c6f 6361 6c73 3e2e 7a6c 6962 5f63  .<locals>.zlib_c
-000031c0: 6f6d 7072 6573 7363 0200 0000 0000 0000  ompressc........
-000031d0: 0000 0000 0300 0000 0300 0000 5300 0000  ............S...
-000031e0: 7320 0000 007c 0072 0e7c 0144 005d 097d  s ...|.r.|.D.].}
-000031f0: 027c 007c 026b 0272 0d01 0064 0153 0071  .|.|.k.r...d.S.q
-00003200: 0464 0253 0029 037a f60a 2020 2020 2020  .d.S.).z..      
-00003210: 2020 6368 6563 6b20 6966 2074 6865 2066    check if the f
-00003220: 6965 6c64 7320 6973 2061 7661 696c 6162  ields is availab
-00003230: 6c65 2069 6e20 7468 6520 7365 7420 6f66  le in the set of
-00003240: 2063 6f6c 6c65 6374 696f 6e73 0a20 2020   collections.   
-00003250: 2020 2020 203a 7061 7261 6d20 7365 6172       :param sear
-00003260: 6368 6564 5f66 6965 6c64 3a20 7365 6172  ched_field: sear
-00003270: 6368 6564 2066 6965 6c64 0a20 2020 2020  ched field.     
-00003280: 2020 203a 7061 7261 6d20 636f 6c6c 6563     :param collec
-00003290: 7469 6f6e 733a 2073 6574 206f 6620 6669  tions: set of fi
-000032a0: 656c 6473 0a20 2020 2020 2020 203a 7265  elds.        :re
-000032b0: 7475 726e 3a20 5472 7565 2069 6620 7468  turn: True if th
-000032c0: 6520 6669 656c 6420 6973 2070 7265 7365  e field is prese
-000032d0: 6e74 2069 6e20 7468 6520 636f 6c6c 6563  nt in the collec
-000032e0: 7469 6f6e 732c 4661 6c73 6520 6f74 6865  tions,False othe
-000032f0: 7277 6973 652e 0a20 2020 2020 2020 2054  rwise..        T
-00003300: 4672 3600 0000 2903 da0e 7365 6172 6368  Fr6...)...search
-00003310: 6564 5f66 6965 6c64 da0b 636f 6c6c 6563  ed_field..collec
-00003320: 7469 6f6e 7372 ba00 0000 7236 0000 0072  tionsr....r6...r
-00003330: 3600 0000 7237 0000 00da 0d66 6965 6c64  6...r7.....field
-00003340: 735f 7365 6172 6368 e401 0000 730c 0000  s_search....s...
-00003350: 0004 0708 0108 0106 0102 ff04 027a 2358  .............z#X
-00003360: 4d4c 5f72 6573 706f 6e73 652e 3c6c 6f63  ML_response.<loc
-00003370: 616c 733e 2e66 6965 6c64 735f 7365 6172  als>.fields_sear
-00003380: 6368 2903 7204 0100 0072 0b01 0000 720e  ch).r....r....r.
-00003390: 0100 007a 042e 786d 6c7a 0874 6578 742f  ...z..xmlz.text/
-000033a0: 786d 6c7a 032e 6a73 fa16 6170 706c 6963  xmlz..js..applic
-000033b0: 6174 696f 6e2f 6a61 7661 7363 7269 7074  ation/javascript
-000033c0: 7a10 6170 706c 6963 6174 696f 6e2f 6a73  z.application/js
-000033d0: 6f6e 7a10 3b63 6861 7273 6574 3d22 7574  onz.;charset="ut
-000033e0: 662d 3822 72ea 0000 0072 3600 0000 2912  f-8"r....r6...).
-000033f0: 72ee 0000 0072 9500 0000 721b 0000 0072  r....r....r....r
-00003400: 0b00 0000 723d 0000 0072 3e00 0000 72f0  ....r=...r>...r.
-00003410: 0000 0072 3a00 0000 72f1 0000 0072 f200  ...r:...r....r..
-00003420: 0000 7204 0000 0072 0900 0000 da14 4874  ..r....r......Ht
-00003430: 7470 5265 7370 6f6e 7365 4e6f 7446 6f75  tpResponseNotFou
-00003440: 6e64 da07 6669 6c74 6572 7372 9000 0000  nd..filtersr....
-00003450: da08 656e 6473 7769 7468 72f3 0000 0072  ..endswithr....r
-00003460: f400 0000 290c 724a 0000 0072 f500 0000  ....).rJ...r....
-00003470: 72f6 0000 0072 fa00 0000 72fb 0000 00da  r....r....r.....
-00003480: 0165 7202 0100 0072 0401 0000 720b 0100  .er....r....r...
-00003490: 0072 0e01 0000 72eb 0000 0072 d800 0000  .r....r....r....
-000034a0: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
-000034b0: 0c58 4d4c 5f72 6573 706f 6e73 65b9 0100  .XML_response...
-000034c0: 0073 3000 0000 1008 0c01 0e03 0201 0e01  .s0.............
-000034d0: 0e01 1401 0880 02ff 0803 0c05 0802 0807  ................
-000034e0: 080b 160d 0e01 0e01 0201 02fe 0403 0e01  ................
-000034f0: 0601 06fe 0404 7214 0100 0063 0000 0000  ......r....c....
-00003500: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00003510: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00003520: 0264 015a 0364 025a 0464 0353 0029 04da  .d.Z.d.Z.d.S.)..
-00003530: 0653 5756 6965 777a 1772 6561 6374 2f73  .SWViewz.react/s
-00003540: 6572 7669 6365 2d77 6f72 6b65 722e 6a73  ervice-worker.js
-00003550: 720f 0100 004e 2905 7256 0000 0072 5700  r....N).rV...rW.
-00003560: 0000 7258 0000 00da 0d74 656d 706c 6174  ..rX.....templat
-00003570: 655f 6e61 6d65 72eb 0000 0072 3600 0000  e_namer....r6...
-00003580: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00003590: 1501 0000 fc01 0000 7306 0000 0008 0004  ........s.......
-000035a0: 0108 0172 1501 0000 6300 0000 0000 0000  ...r....c.......
-000035b0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-000035c0: 0073 2000 0000 6500 5a01 6400 5a02 6401  .s ...e.Z.d.Z.d.
-000035d0: 5a03 8700 6601 6402 6403 8408 5a04 8700  Z...f.d.d...Z...
-000035e0: 0400 5a05 5300 2904 da06 5742 5669 6577  ..Z.S.)...WBView
-000035f0: 720f 0100 0063 0200 0000 0000 0000 0000  r....c..........
-00003600: 0000 0400 0000 0400 0000 0f00 0000 732c  ..............s,
-00003610: 0000 0074 0083 006a 017c 0167 017c 02a2  ...t...j.|.g.|..
-00003620: 0152 0069 007c 03a4 018e 0101 0064 017c  .R.i.|.......d.|
-00003630: 0364 0219 0017 007c 005f 0264 0053 0029  .d.....|._.d.S.)
-00003640: 034e 7a06 7265 6163 742f da07 776f 726b  .Nz.react/..work
-00003650: 626f 7829 03da 0573 7570 6572 da05 7365  box)...super..se
-00003660: 7475 7072 1601 0000 2904 7244 0000 0072  tupr....).rD...r
-00003670: 4500 0000 7201 0100 00da 066b 7761 7267  E...r......kwarg
-00003680: 73a9 01da 095f 5f63 6c61 7373 5f5f 7236  s....__class__r6
-00003690: 0000 0072 3700 0000 721a 0100 0003 0200  ...r7...r.......
-000036a0: 0073 0400 0000 1a01 1201 7a0c 5742 5669  .s........z.WBVi
-000036b0: 6577 2e73 6574 7570 2906 7256 0000 0072  ew.setup).rV...r
-000036c0: 5700 0000 7258 0000 0072 eb00 0000 721a  W...rX...r....r.
-000036d0: 0100 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-000036e0: 5f5f 7236 0000 0072 3600 0000 721c 0100  __r6...r6...r...
-000036f0: 0072 3700 0000 7217 0100 0000 0200 0073  .r7...r........s
-00003700: 0600 0000 0800 0401 1402 7217 0100 0063  ..........r....c
-00003710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003720: 0200 0000 4000 0000 f314 0000 0065 005a  ....@........e.Z
-00003730: 0164 005a 0264 0164 0284 005a 0364 0353  .d.Z.d.d...Z.d.S
-00003740: 0029 04da 084d 6169 6e48 746d 6c63 0200  .)...MainHtmlc..
-00003750: 0000 0000 0000 0000 0000 0700 0000 0400  ................
-00003760: 0000 4f00 0000 7358 0000 0074 006a 01a0  ..O...sX...t.j..
-00003770: 02a1 0001 0074 006a 016a 036a 046a 057d  .....t.j.j.j.j.}
-00003780: 0474 067c 017c 0464 018d 027d 0564 027c  .t.|.|.d...}.d.|
-00003790: 015f 0774 006a 01a0 087c 05a1 017d 067c  ._.t.j...|...}.|
-000037a0: 04a0 097c 06a1 017d 067c 056a 0a7c 0664  ...|...}.|.j.|.d
-000037b0: 038d 0101 0074 0b7c 056a 0c7c 056a 0d83  .....t.|.j.|.j..
-000037c0: 0253 0029 047a 3252 6574 7572 6e73 2061  .S.).z2Returns a
-000037d0: 206a 736f 6e20 7374 7275 6374 2066 6f72   json struct for
-000037e0: 2074 6865 206d 6169 6e20 7573 6572 2064   the main user d
-000037f0: 6173 6862 6f61 7264 2e72 3900 0000 7a0e  ashboard.r9...z.
-00003800: 6461 7368 626f 6172 642d 6d61 696e 7207  dashboard-mainr.
-00003810: 0000 0029 0e72 0b00 0000 723d 0000 00da  ...).r....r=....
-00003820: 0773 7461 7274 7570 723e 0000 0072 3f00  .startupr>...r?.
-00003830: 0000 723a 0000 0072 1c00 0000 da10 7265  ..r:...r......re
-00003840: 7175 6573 7469 6e67 5f70 616e 656c da0d  questing_panel..
-00003850: 6765 745f 6d61 696e 5f68 746d 6c72 7300  get_main_htmlrs.
-00003860: 0000 7274 0000 0072 2100 0000 72d8 0000  ..rt...r!...r...
-00003870: 0072 eb00 0000 2907 7244 0000 0072 4500  .r....).rD...rE.
-00003880: 0000 7201 0100 0072 a200 0000 da03 726e  ..r....r......rn
-00003890: 6472 4a00 0000 7208 0000 0072 3600 0000  drJ...r....r6...
-000038a0: 7236 0000 0072 3700 0000 727c 0000 0009  r6...r7...r|....
-000038b0: 0200 0073 1000 0000 0a03 0c02 0c01 0602  ...s............
-000038c0: 0c01 0a01 0c01 0e01 7a0c 4d61 696e 4874  ........z.MainHt
-000038d0: 6d6c 2e67 6574 4e72 c200 0000 7236 0000  ml.getNr....r6..
-000038e0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-000038f0: 7220 0100 0008 0200 00f3 0400 0000 0800  r ..............
-00003900: 0c01 7220 0100 0063 0000 0000 0000 0000  ..r ...c........
-00003910: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00003920: 721f 0100 0029 04da 0d44 6173 6862 6f61  r....)...Dashboa
-00003930: 7264 4974 656d 6303 0000 0000 0000 0000  rdItemc.........
-00003940: 0000 000a 0000 0005 0000 004f 0000 0073  ...........O...s
-00003950: 9800 0000 7400 7c01 8301 7d05 7401 6a02  ....t.|...}.t.j.
-00003960: 6a03 6a04 6a05 7c05 5f05 6401 7c02 9b00  j.j.j.|._.d.|...
-00003970: 9d02 7c05 5f06 7c05 a007 a100 a008 a100  ..|._.|.........
-00003980: 6a09 7d06 740a 7c06 8301 7c02 6b04 722b  j.}.t.|...|.k.r+
-00003990: 7c06 7c02 1900 7d07 6402 a00b 7c07 a00c  |.|...}.d...|...
-000039a0: 7c05 a101 a101 7d08 6e02 6402 7d08 740d  |.....}.n.d.}.t.
-000039b0: 7c08 6403 8d01 7d04 740e 7c01 8301 7d09  |.d...}.t.|...}.
-000039c0: 7c09 723d 7c04 a00f 7c09 a101 0100 7c05  |.r=|...|.....|.
-000039d0: 6a10 6405 6900 7c04 a401 8e01 0100 7411  j.d.i.|.......t.
-000039e0: 7c05 6a12 7c05 6a13 8302 5300 2906 7a3d  |.j.|.j...S.).z=
-000039f0: 5265 7475 726e 7320 6120 7265 6e64 6572  Returns a render
-00003a00: 6564 2048 544d 4c20 7665 7273 696f 6e20  ed HTML version 
-00003a10: 7468 6520 7265 7175 6573 7465 6420 7573  the requested us
-00003a20: 6572 2064 6173 6862 6f61 7264 2e7a 0a64  er dashboard.z.d
-00003a30: 6173 6862 6f61 7264 2d72 5c00 0000 7207  ashboard-r\...r.
-00003a40: 0000 004e 7236 0000 0029 1472 1c00 0000  ...Nr6...).r....
-00003a50: 720b 0000 0072 3d00 0000 723e 0000 0072  r....r=...r>...r
-00003a60: 3f00 0000 723a 0000 0072 2201 0000 72ec  ?...r:...r"...r.
-00003a70: 0000 00da 0f67 6574 5f70 7265 6665 7265  .....get_prefere
-00003a80: 6e63 6573 da0f 6461 7368 626f 6172 645f  nces..dashboard_
-00003a90: 6974 656d 7372 8f00 0000 72ff 0000 0072  itemsr....r....r
-00003aa0: f400 0000 7290 0000 0072 2c00 0000 7295  ....r....r,...r.
-00003ab0: 0000 0072 7400 0000 7221 0000 0072 d800  ...rt...r!...r..
-00003ac0: 0000 72eb 0000 0029 0a72 4400 0000 7245  ..r....).rD...rE
-00003ad0: 0000 00da 0569 6e64 6578 7201 0100 0072  .....indexr....r
-00003ae0: a200 0000 724a 0000 00da 0464 6173 68da  ....rJ.....dash.
-00003af0: 0469 7465 6d72 0800 0000 7299 0000 0072  .itemr....r....r
-00003b00: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
-00003b10: 0000 0019 0200 0073 1c00 0000 0802 0e01  .......s........
-00003b20: 0c01 0e01 0c01 0801 1203 0402 0a01 0801  ................
-00003b30: 0401 0a01 1001 0e01 7a11 4461 7368 626f  ........z.Dashbo
-00003b40: 6172 6449 7465 6d2e 6765 744e 72c2 0000  ardItem.getNr...
-00003b50: 0072 3600 0000 7236 0000 0072 3600 0000  .r6...r6...r6...
-00003b60: 7237 0000 0072 2601 0000 1802 0000 7225  r7...r&.......r%
-00003b70: 0100 0072 2601 0000 6300 0000 0000 0000  ...r&...c.......
-00003b80: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00003b90: 0073 2000 0000 6500 5a01 6400 5a02 6401  .s ...e.Z.d.Z.d.
-00003ba0: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
-00003bb0: 5a05 6406 5300 2907 da04 4e75 6c6c 7a6c  Z.d.S.)...Nullzl
-00003bc0: 4a75 7374 2072 6574 7572 6e73 2032 3030  Just returns 200
-00003bd0: 2c20 7573 6564 2069 6e20 616e 2069 6672  , used in an ifr
-00003be0: 616d 6520 746f 2063 6175 7365 2074 6865  ame to cause the
-00003bf0: 2062 726f 7773 6572 2074 6f20 7472 6967   browser to trig
-00003c00: 6765 7220 2244 6f20 796f 7520 7761 6e74  ger "Do you want
-00003c10: 2074 6f20 7265 6d65 6d62 6572 2074 6869   to remember thi
-00003c20: 7320 7077 2220 6469 616c 6f67 6302 0000  s pw" dialogc...
-00003c30: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00003c40: 0043 0000 00f3 0800 0000 7400 a001 a100  .C........t.....
-00003c50: 5300 72b6 0000 00a9 0272 0900 0000 72f3  S.r......r....r.
-00003c60: 0000 00a9 0272 4400 0000 7245 0000 0072  .....rD...rE...r
-00003c70: 3600 0000 7236 0000 0072 3700 0000 724c  6...r6...r7...rL
-00003c80: 0000 0031 0200 00f3 0200 0000 0801 7a09  ...1..........z.
-00003c90: 4e75 6c6c 2e70 6f73 7463 0200 0000 0000  Null.postc......
-00003ca0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00003cb0: 0000 722d 0100 0072 b600 0000 722e 0100  ..r-...r....r...
-00003cc0: 0072 2f01 0000 7236 0000 0072 3600 0000  .r/...r6...r6...
-00003cd0: 7237 0000 0072 7c00 0000 3402 0000 7230  r7...r|...4...r0
-00003ce0: 0100 007a 084e 756c 6c2e 6765 744e 2906  ...z.Null.getN).
-00003cf0: 7256 0000 0072 5700 0000 7258 0000 0072  rV...rW...rX...r
-00003d00: b100 0000 724c 0000 0072 7c00 0000 7236  ....rL...r|...r6
-00003d10: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003d20: 0000 722c 0100 002e 0200 0073 0800 0000  ..r,.......s....
-00003d30: 0800 0401 0802 0c03 722c 0100 0063 0000  ........r,...c..
-00003d40: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00003d50: 0000 4000 0000 731c 0000 0065 005a 0164  ..@...s....e.Z.d
-00003d60: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00003d70: 005a 0464 0553 0029 06da 0c41 7574 6865  .Z.d.S.)...Authe
-00003d80: 6e74 6963 6174 6563 0200 0000 0000 0000  nticatec........
-00003d90: 0000 0000 0700 0000 0400 0000 4f00 0000  ............O...
-00003da0: 7336 0000 007c 016a 00a0 0174 026a 03a1  s6...|.j...t.j..
-00003db0: 017d 0409 007c 016a 04a0 0564 0364 00a1  .}...|.j...d.d..
-00003dc0: 027d 0574 06a0 077c 01a1 0101 0064 047d  .}.t...|.....d.}
-00003dd0: 0674 08a0 097c 06a1 0153 0029 054e 54da  .t...|...S.).NT.
-00003de0: 066c 6f67 6f75 74da 0875 7365 726e 616d  .logout..usernam
-00003df0: 65fa 012f 290b 7278 0000 0072 7c00 0000  e../).rx...r|...
-00003e00: 721b 0000 0072 8100 0000 da07 7365 7373  r....r......sess
-00003e10: 696f 6eda 0370 6f70 7213 0000 0072 3201  ion..popr....r2.
-00003e20: 0000 7209 0000 00da 1448 7474 7052 6573  ..r......HttpRes
-00003e30: 706f 6e73 6552 6564 6972 6563 74da 0748  ponseRedirect..H
-00003e40: 7474 7034 3034 2907 7244 0000 0072 4500  ttp404).rD...rE.
-00003e50: 0000 7201 0100 0072 a200 0000 729c 0000  ..r....r....r...
-00003e60: 0072 3301 0000 7232 0000 0072 3600 0000  .r3...r2...r6...
-00003e70: 7236 0000 0072 3700 0000 727c 0000 0039  r6...r7...r|...9
-00003e80: 0200 0073 0c00 0000 0e01 0201 0e01 0a01  ...s............
-00003e90: 0405 0a01 7a10 4175 7468 656e 7469 6361  ....z.Authentica
-00003ea0: 7465 2e67 6574 6302 0000 0000 0000 0000  te.getc.........
-00003eb0: 0000 0008 0000 0005 0000 004f 0000 0073  ...........O...s
-00003ec0: 4c00 0000 7c01 6a00 a001 6401 a101 7d04  L...|.j...d...}.
-00003ed0: 7c01 6a00 a001 6402 a101 7d05 7402 6a03  |.j...d...}.t.j.
-00003ee0: 7c01 7c04 7c05 6403 8d03 7d06 7402 6a04  |.|.|.d...}.t.j.
-00003ef0: 7c01 7c06 6404 6405 8d03 0100 6406 6407  |.|.d.d.....d.d.
-00003f00: 8400 7d07 7405 7c06 6a06 7c07 8302 5300  ..}.t.|.j.|...S.
-00003f10: 2908 7a46 6c6f 6773 2074 6865 2075 7365  ).zFlogs the use
-00003f20: 7220 696e 2061 6e64 2062 7569 6c64 7320  r in and builds 
-00003f30: 7468 6520 6c69 6e6f 7765 622e 6a73 2066  the linoweb.js f
-00003f40: 696c 6520 666f 7220 7468 6520 6c6f 6767  ile for the logg
-00003f50: 6564 2069 6e20 7573 6572 7233 0100 00da  ed in userr3....
-00003f60: 0870 6173 7377 6f72 6429 0272 3301 0000  .password).r3...
-00003f70: 7239 0100 007a 246c 696e 6f2e 636f 7265  r9...z$lino.core
-00003f80: 2e61 7574 682e 6261 636b 656e 6473 2e4d  .auth.backends.M
-00003f90: 6f64 656c 4261 636b 656e 6429 01da 0762  odelBackend)...b
-00003fa0: 6163 6b65 6e64 6300 0000 0000 0000 0000  ackendc.........
-00003fb0: 0000 0000 0000 0003 0000 0053 0000 0073  ...........S...s
-00003fc0: 2600 0000 7400 6a01 6a02 720d 7400 6a01  &...t.j.j.r.t.j.
-00003fd0: 6a03 6a04 6a05 a006 6401 a101 0100 7407  j.j.j...d.....t.
-00003fe0: 6402 6403 6901 8301 5300 2904 4e46 7274  d.d.i...S.).NFrt
-00003ff0: 0000 0054 2908 720b 0000 0072 3d00 0000  ...T).r....r=...
-00004000: da14 6465 7665 6c6f 7065 725f 7369 7465  ..developer_site
-00004010: 5f63 6163 6865 723e 0000 0072 3f00 0000  _cacher>...r?...
-00004020: 723a 0000 00da 0e62 7569 6c64 5f6a 735f  r:.....build_js_
-00004030: 6361 6368 6572 2100 0000 7236 0000 0072  cacher!...r6...r
-00004040: 3600 0000 7236 0000 0072 3700 0000 da06  6...r6...r7.....
-00004050: 7265 7375 6c74 5402 0000 7306 0000 0008  resultT...s.....
-00004060: 0112 010c 027a 2141 7574 6865 6e74 6963  .....z!Authentic
-00004070: 6174 652e 706f 7374 2e3c 6c6f 6361 6c73  ate.post.<locals
-00004080: 3e2e 7265 7375 6c74 2907 723c 0000 0072  >.result).r<...r
-00004090: 7c00 0000 7213 0000 00da 0c61 7574 6865  |...r......authe
-000040a0: 6e74 6963 6174 65da 056c 6f67 696e 7229  nticate..loginr)
-000040b0: 0000 0072 ed00 0000 2908 7244 0000 0072  ...r....).rD...r
-000040c0: 4500 0000 7201 0100 0072 a200 0000 7233  E...r....r....r3
-000040d0: 0100 0072 3901 0000 da04 7573 6572 723d  ...r9.....userr=
-000040e0: 0100 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-000040f0: 0000 724c 0000 004a 0200 0073 1000 0000  ..rL...J...s....
-00004100: 0c02 0c01 0402 0601 06ff 1002 0803 0c06  ................
-00004110: 7a11 4175 7468 656e 7469 6361 7465 2e70  z.Authenticate.p
-00004120: 6f73 744e 2905 7256 0000 0072 5700 0000  ostN).rV...rW...
-00004130: 7258 0000 0072 7c00 0000 724c 0000 0072  rX...r|...rL...r
-00004140: 3600 0000 7236 0000 0072 3600 0000 7237  6...r6...r6...r7
-00004150: 0000 0072 3101 0000 3802 0000 7306 0000  ...r1...8...s...
-00004160: 0008 0008 010c 1172 3101 0000 6300 0000  .......r1...c...
-00004170: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00004180: 0040 0000 0072 a400 0000 2905 da05 496e  .@...r....)...In
-00004190: 6465 787a 930a 2020 2020 4d61 696e 2061  dexz..    Main a
-000041a0: 7070 2065 6e74 7279 2070 6f69 6e74 2c0a  pp entry point,.
-000041b0: 2020 2020 416c 736f 2062 7569 6c64 7320      Also builds 
-000041c0: 6c69 6e6f 7765 6220 6669 6c65 2066 6f72  linoweb file for
-000041d0: 2063 7572 7265 6e74 2075 7365 7220 7479   current user ty
-000041e0: 7065 2e0a 2020 2020 436f 6e74 656e 7420  pe..    Content 
-000041f0: 6973 206d 6f73 746c 7920 696e 2074 6865  is mostly in the
-00004200: 203a 7866 696c 653a 6072 6561 6374 2f6d   :xfile:`react/m
-00004210: 6169 6e2e 6874 6d6c 6020 7465 6d70 6c61  ain.html` templa
-00004220: 7465 2e0a 2020 2020 6302 0000 0000 0000  te..    c.......
-00004230: 0000 0000 0003 0000 0003 0000 0003 0000  ................
-00004240: 0073 2e00 0000 8800 6a00 8901 0900 8800  .s......j.......
-00004250: 6a01 720a 8800 6a01 8901 8700 8701 6602  j.r...j.......f.
-00004260: 6402 6403 8408 7d02 7402 8801 6a03 7c02  d.d...}.t...j.|.
-00004270: 8302 5300 2904 4e54 6300 0000 0000 0000  ..S.).NTc.......
-00004280: 0000 0000 0007 0000 0006 0000 0013 0000  ................
-00004290: 0073 b600 0000 7400 6a01 6a02 6a03 7d00  .s....t.j.j.j.}.
-000042a0: 7404 8800 7c00 6a05 6401 8d02 7d01 7406  t...|.j.d...}.t.
-000042b0: 7c00 8800 8801 6402 8d03 7d02 7c02 6a07  |.....d...}.|.j.
-000042c0: 7c01 6403 8d01 0100 6404 7d03 6405 8800  |.d.....d.}.d...
-000042d0: 6a08 7600 7229 6406 a009 740a a00b 6407  j.v.r)d...t...d.
-000042e0: 6408 a102 a101 7d03 7c02 6a07 7c03 6409  d.....}.|.j.|.d.
-000042f0: 8d01 0100 7c01 6a0c 640f 6900 7c02 a401  ....|.j.d.i.|...
-00004300: 8e01 7d02 7400 6a01 6a02 6a0d 6a05 6a0e  ..}.t.j.j.j.j.j.
-00004310: 7d04 7c04 a00f 640a a101 7d05 7410 6a11  }.|...d...}.t.j.
-00004320: 7c05 6a12 640f 6900 7c02 a401 8e01 640b  |.j.d.i.|.....d.
-00004330: 640c 8d02 7d06 6405 8800 6a08 7600 7259  d...}.d...j.v.rY
-00004340: 640d 7c06 640e 3c00 7c06 5300 2910 4e72  d.|.d.<.|.S.).Nr
-00004350: c500 0000 2903 da09 6672 6f6e 745f 656e  ....)...front_en
-00004360: 6472 4500 0000 7240 0100 0029 0172 4a00  drE...r@...).rJ.
-00004370: 0000 725c 0000 00da 0c75 7064 6174 655f  ..r\.....update_
-00004380: 666f 756e 647a 093f 6d74 696d 653d 7b7d  foundz.?mtime={}
-00004390: 6907 b201 0069 3f42 0f00 2901 da08 6e6f  i....i?B..)...no
-000043a0: 5f63 6163 6865 7a0f 7265 6163 742f 6d61  _cachez.react/ma
-000043b0: 696e 2e68 746d 6c72 e900 0000 72ea 0000  in.htmlr....r...
-000043c0: 007a 1222 6361 6368 6522 2c20 2273 746f  .z."cache", "sto
-000043d0: 7261 6765 227a 0f43 6c65 6172 2d53 6974  rage"z.Clear-Sit
-000043e0: 652d 4461 7461 7236 0000 0029 1372 0b00  e-Datar6...).r..
-000043f0: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
-00004400: 0072 1c00 0000 723a 0000 0072 9000 0000  .r....r:...r....
-00004410: 7295 0000 0072 7800 0000 727a 0000 00da  r....rx...rz....
-00004420: 0672 616e 646f 6dda 0772 616e 6469 6e74  .random..randint
-00004430: 72ee 0000 0072 f000 0000 72f1 0000 0072  r....r....r....r
-00004440: f200 0000 7209 0000 0072 f300 0000 72f4  ....r....r....r.
-00004450: 0000 0029 07da 0275 6972 4a00 0000 72f6  ...)...uirJ...r.
-00004460: 0000 0072 4401 0000 72fa 0000 0072 fb00  ...rD...r....r..
-00004470: 0000 da04 7265 7370 a902 7245 0000 0072  ....resp..rE...r
-00004480: 4001 0000 7236 0000 0072 3700 0000 da05  @...r6...r7.....
-00004490: 6765 7469 7478 0200 0073 3200 0000 0a01  getitx...s2.....
-000044a0: 0203 0202 0401 06fd 0204 0204 0201 0201  ................
-000044b0: 06fa 0c08 0402 0a01 1201 0c01 1001 0e01  ................
-000044c0: 0a01 0401 0e01 0201 06fe 0a04 0801 0402  ................
-000044d0: 7a18 496e 6465 782e 6765 742e 3c6c 6f63  z.Index.get.<loc
-000044e0: 616c 733e 2e67 6574 6974 2904 7240 0100  als>.getit).r@..
-000044f0: 00da 0a73 7562 7374 5f75 7365 7272 2900  ...subst_userr).
-00004500: 0000 72ed 0000 00a9 0372 4400 0000 7245  ..r......rD...rE
-00004510: 0000 0072 4a01 0000 7236 0000 0072 4901  ...rJ...r6...rI.
-00004520: 0000 7237 0000 0072 7c00 0000 7102 0000  ..r7...r|...q...
-00004530: 730c 0000 0006 0202 0106 0106 010e 020c  s...............
-00004540: 227a 0949 6e64 6578 2e67 6574 4e72 b000  "z.Index.getNr..
-00004550: 0000 7236 0000 0072 3600 0000 7236 0000  ..r6...r6...r6..
-00004560: 0072 3700 0000 7241 0100 006a 0200 0072  .r7...rA...j...r
-00004570: b200 0000 7241 0100 0063 0000 0000 0000  ....rA...c......
-00004580: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00004590: 0000 72a4 0000 0029 05da 0c55 7365 7253  ..r....)...UserS
-000045a0: 6574 7469 6e67 737a 420a 2020 2020 416a  ettingszB.    Aj
-000045b0: 6178 2069 6e74 6572 6661 6365 2066 6f72  ax interface for
-000045c0: 2067 6574 7469 6e67 2074 6865 2063 7572   getting the cur
-000045d0: 7265 6e74 2073 6573 7369 6f6e 2f75 7365  rent session/use
-000045e0: 7220 7365 7474 696e 6773 2e63 0200 0000  r settings.c....
-000045f0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00004600: 0300 0000 734e 0000 0074 007c 0183 017d  ....sN...t.|...}
-00004610: 017c 016a 0189 037c 016a 0289 0188 0172  .|.j...|.j.....r
-00004620: 117c 016a 02a0 03a1 006e 0164 0189 0288  .|.j.....n.d....
-00004630: 036a 0489 0087 0087 0187 0287 0366 0464  .j...........f.d
-00004640: 0264 0384 087d 0274 0588 0170 2388 036a  .d...}.t...p#..j
-00004650: 067c 0283 0253 0029 044e 725c 0000 0063  .|...S.).Nr\...c
-00004660: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00004670: 1100 0000 1300 0000 737c 0100 0074 006a  ........s|...t.j
-00004680: 016a 0272 1174 006a 016a 0373 1174 006a  .j.r.t.j.j.s.t.j
-00004690: 016a 046a 056a 06a0 0764 01a1 0101 0074  .j.j.j...d.....t
-000046a0: 0888 036a 0974 0a88 03a0 0ba1 006a 0c83  ...j.t.......j..
-000046b0: 0188 036a 0d74 0e83 0074 006a 016a 0f74  ...j.t...t.j.j.t
-000046c0: 006a 016a 046a 056a 06a0 10a1 008e 0074  .j.j.j.j.......t
-000046d0: 006a 016a 116a 1288 0088 0072 3488 03a0  .j.j.j.....r4...
-000046e0: 13a1 006e 0374 1464 0283 0188 0274 1464  ...n.t.d.....t.d
-000046f0: 0383 0174 1464 0483 0174 1464 0483 0174  ...t.d...t.d...t
-00004700: 1464 0583 0174 006a 01a0 1564 06a1 0172  .d...t.j...d...r
-00004710: 5074 006a 016a 046a 166a 1770 5374 1464  Pt.j.j.j.j.pSt.d
-00004720: 0783 0188 036a 1864 088d 0f7d 0088 0272  .....j.d...}...r
-00004730: 6888 016a 1904 007c 0064 093c 007c 0064  h..j...|.d.<.|.d
-00004740: 0a3c 0088 016a 097c 0064 0b3c 0088 0072  .<...j.|.d.<...r
-00004750: ba88 03a0 1aa1 007c 0064 0c3c 0088 036a  .......|.d.<...j
-00004760: 1b7c 0064 0d3c 0074 006a 016a 046a 166a  .|.d.<.t.j.j.j.j
-00004770: 1c72 ba88 03a0 1da1 000c 007d 017c 0172  .r.........}.|.r
-00004780: ba88 036a 1e64 0075 0172 ba64 0e7c 0064  ...j.d.u.r.d.|.d
-00004790: 0f3c 0088 036a 1e74 1f6a 2074 006a 016a  .<...j.t.j t.j.j
-000047a0: 046a 166a 2164 108d 0117 007d 0274 22a0  .j.j!d.....}.t".
-000047b0: 2364 11a1 018f 1101 0074 1f6a 1fa0 2474  #d.......t.j..$t
-000047c0: 22a0 257c 02a1 01a1 017d 0357 0064 0004  ".%|.....}.W.d..
-000047d0: 0004 0083 0301 006e 0831 0073 b177 0101  .......n.1.s.w..
-000047e0: 0001 0001 0059 0001 007c 037c 0064 123c  .....Y...|.|.d.<
-000047f0: 0074 267c 0083 0153 0029 134e 46da 0941  .t&|...S.).NF..A
-00004800: 6e6f 6e79 6d6f 7573 7a31 596f 7520 6172  nonymousz1You ar
-00004810: 6520 6175 7468 6f72 6973 6564 2074 6f20  e authorised to 
-00004820: 6163 7420 6173 2074 6865 2066 6f6c 6c6f  act as the follo
-00004830: 7769 6e67 2075 7365 7273 2e7a 1341 6374  wing users.z.Act
-00004840: 2061 7320 616e 6f74 6865 7220 7573 6572   as another user
-00004850: 7a1b 5374 6f70 2061 6374 696e 6720 6173  z.Stop acting as
-00004860: 2061 6e6f 7468 6572 2075 7365 72da 0575   another user..u
-00004870: 7365 7273 7a0b 4d79 2073 6574 7469 6e67  sersz.My setting
-00004880: 7329 0f72 ed00 0000 7228 0100 00da 0565  s).r....r(.....e
-00004890: 6d61 696c 72f8 0000 00da 0973 6974 655f  mailr......site_
-000048a0: 6461 7461 da09 7369 7465 5f6e 616d 65da  data..site_name.
-000048b0: 096c 6f67 6765 645f 696e 7233 0100 00da  .logged_inr3....
-000048c0: 0773 755f 6e61 6d65 da0e 6163 745f 6173  .su_name..act_as
-000048d0: 5f73 7562 7465 7874 da11 6163 745f 6173  _subtext..act_as
-000048e0: 5f74 6974 6c65 5f74 6578 74da 1261 6374  _title_text..act
-000048f0: 5f61 735f 6275 7474 6f6e 5f74 6578 74da  _as_button_text.
-00004900: 1061 6374 5f61 735f 7365 6c66 5f74 6578  .act_as_self_tex
-00004910: 74da 0f6d 795f 7365 7474 696e 675f 7465  t..my_setting_te
-00004920: 7874 da07 7573 6572 5f69 6472 5a01 0000  xt..user_idrZ...
-00004930: da05 7375 5f69 64da 0c73 755f 7573 6572  ..su_id..su_user
-00004940: 5f74 7970 65da 0b61 7574 686f 7269 7469  _type..authoriti
-00004950: 6573 da10 6461 7368 626f 6172 645f 6c61  es..dashboard_la
-00004960: 796f 7574 54da 1472 6571 7569 7265 5f76  youtT..require_v
-00004970: 6572 6966 6963 6174 696f 6e29 01da 076d  erification)...m
-00004980: 696e 7574 6573 da03 5554 43da 0b63 6f64  inutes..UTC..cod
-00004990: 655f 6578 7069 7279 2927 720b 0000 0072  e_expiry)'r....r
-000049a0: 3d00 0000 723b 0100 00da 166e 6576 6572  =...r;.....never
-000049b0: 5f62 7569 6c64 5f73 6974 655f 6361 6368  _build_site_cach
-000049c0: 6572 3e00 0000 723f 0000 0072 3a00 0000  er>...r?...r:...
-000049d0: 723c 0100 0072 9000 0000 72ed 0000 0072  r<...r....r....r
-000049e0: 8f00 0000 7227 0100 0072 2801 0000 7250  ....r'...r(...rP
-000049f0: 0100 0072 1100 0000 da14 6275 696c 645f  ...r......build_
-00004a00: 7369 7465 5f63 6163 6865 5f75 726c da0d  site_cache_url..
-00004a10: 6c69 6e6f 5f6a 735f 7061 7274 73da 0b70  lino_js_parts..p
-00004a20: 726f 6a65 6374 5f64 6972 da04 6e61 6d65  roject_dir..name
-00004a30: da0d 6765 745f 6675 6c6c 5f6e 616d 65da  ..get_full_name.
-00004a40: 015f da0c 6973 5f69 6e73 7461 6c6c 6564  ._..is_installed
-00004a50: 724f 0100 0072 5901 0000 7248 0000 0072  rO...rY...rH...r
-00004a60: 5d00 0000 da0f 6765 745f 6175 7468 6f72  ].....get_author
-00004a70: 6974 6965 7372 5e01 0000 da19 616c 6c6f  itiesr^.....allo
-00004a80: 775f 6f6e 6c69 6e65 5f72 6567 6973 7472  w_online_registr
-00004a90: 6174 696f 6eda 0b69 735f 7665 7269 6669  ation..is_verifi
-00004aa0: 6564 da19 7665 7269 6669 6361 7469 6f6e  ed..verification
-00004ab0: 5f63 6f64 655f 7365 6e74 5f6f 6eda 0864  _code_sent_on..d
-00004ac0: 6174 6574 696d 65da 0974 696d 6564 656c  atetime..timedel
-00004ad0: 7461 da19 7665 7269 6669 6361 7469 6f6e  ta..verification
-00004ae0: 5f63 6f64 655f 6578 7069 7265 7372 0f00  _code_expiresr..
-00004af0: 0000 da08 6f76 6572 7269 6465 da09 7469  ....override..ti
-00004b00: 6d65 7374 616d 70da 0a6d 616b 655f 6e61  mestamp..make_na
-00004b10: 6976 6572 2100 0000 2904 da0d 7573 6572  iver!...)...user
-00004b20: 5f73 6574 7469 6e67 7372 5f01 0000 da0b  _settingsr_.....
-00004b30: 6578 7069 7279 5f74 696d 65da 0c65 7870  expiry_time..exp
-00004b40: 6972 795f 7374 616d 70a9 04da 086e 6f74  iry_stamp....not
-00004b50: 5f61 6e6f 6eda 0273 7572 5401 0000 72f7  _anon..surT...r.
-00004b60: 0000 0072 3600 0000 7237 0000 0072 4a01  ...r6...r7...rJ.
-00004b70: 0000 aa02 0000 7352 0000 0008 0206 0102  ......sR........
-00004b80: ff12 0202 0204 010c 0104 0104 0216 0108  ................
-00004b90: 0102 0112 0102 0106 0106 0106 0106 011e  ................
-00004ba0: 0204 0106 ef04 1412 010a 0104 020c 010a  ................
-00004bb0: 010c 020a 010e 0108 0108 010a 0108 ff0c  ................
-00004bc0: 0306 0108 0106 ff1c ff08 0308 027a 1f55  .............z.U
-00004bd0: 7365 7253 6574 7469 6e67 732e 6765 742e  serSettings.get.
-00004be0: 3c6c 6f63 616c 733e 2e67 6574 6974 2907  <locals>.getit).
-00004bf0: 721c 0000 0072 4001 0000 724b 0100 0072  r....r@...rK...r
-00004c00: 6801 0000 da10 6973 5f61 7574 6865 6e74  h.....is_authent
-00004c10: 6963 6174 6564 7229 0000 0072 ed00 0000  icatedr)...r....
-00004c20: 724c 0100 0072 3600 0000 7278 0100 0072  rL...r6...rx...r
-00004c30: 3700 0000 727c 0000 00a1 0200 0073 0e00  7...r|.......s..
-00004c40: 0000 0801 0601 0601 1201 0603 1202 1032  ...............2
-00004c50: 7a10 5573 6572 5365 7474 696e 6773 2e67  z.UserSettings.g
-00004c60: 6574 4e72 b000 0000 7236 0000 0072 3600  etNr....r6...r6.
-00004c70: 0000 7236 0000 0072 3700 0000 724d 0100  ..r6...r7...rM..
-00004c80: 009d 0200 0073 0600 0000 0800 0401 0c03  .....s..........
-00004c90: 724d 0100 0072 b600 0000 2962 72b1 0000  rM...r....)br...
-00004ca0: 00da 026f 7372 0200 0000 726f 0100 00da  ...osr....ro....
-00004cb0: 0272 65da 0363 6769 da03 6173 7472 d300  .re..cgi..astr..
-00004cc0: 0000 7245 0100 0072 0800 0000 da05 7479  ..rE...r......ty
-00004cd0: 7065 7372 0300 0000 da11 6a69 6e6a 6132  pesr......jinja2
-00004ce0: 2e65 7863 6570 7469 6f6e 7372 0400 0000  .exceptionsr....
-00004cf0: da0a 6574 6765 6e2e 6874 6d6c 7205 0000  ..etgen.htmlr...
-00004d00: 0072 0600 0000 da05 6574 6765 6eda 0678  .r......etgen..x
-00004d10: 6768 746d 6cda 0664 6a61 6e67 6f72 0900  ghtml..djangor..
-00004d20: 0000 da09 646a 616e 676f 2e64 6272 0a00  ....django.dbr..
-00004d30: 0000 da0b 646a 616e 676f 2e63 6f6e 6672  ....django.confr
-00004d40: 0b00 0000 da14 646a 616e 676f 2e76 6965  ......django.vie
-00004d50: 7773 2e67 656e 6572 6963 720c 0000 00da  ws.genericr.....
-00004d60: 1964 6a61 6e67 6f2e 7669 6577 732e 6765  .django.views.ge
-00004d70: 6e65 7269 632e 6261 7365 720d 0000 00da  neric.baser.....
-00004d80: 0b64 6a61 6e67 6f2e 636f 7265 720e 0000  .django.corer...
-00004d90: 00da 0c64 6a61 6e67 6f2e 7574 696c 7372  ...django.utilsr
-00004da0: 0f00 0000 da18 646a 616e 676f 2e75 7469  ......django.uti
-00004db0: 6c73 2e74 7261 6e73 6c61 7469 6f6e 7210  ls.translationr.
-00004dc0: 0000 0072 6901 0000 7211 0000 00da 1664  ...ri...r......d
-00004dd0: 6a61 6e67 6f2e 636f 7265 2e65 7863 6570  jango.core.excep
-00004de0: 7469 6f6e 7372 1200 0000 da09 6c69 6e6f  tionsr......lino
-00004df0: 2e63 6f72 6572 1300 0000 da0a 6c69 6e6f  .corer......lino
-00004e00: 2e75 7469 6c73 7214 0000 00da 106c 696e  .utilsr......lin
-00004e10: 6f2e 7574 696c 732e 6a73 6765 6e72 1500  o.utils.jsgenr..
-00004e20: 0000 7216 0000 00da 0f6c 696e 6f2e 636f  ..r......lino.co
-00004e30: 7265 2e65 6c65 6d73 7217 0000 00da 106c  re.elemsr......l
-00004e40: 696e 6f2e 636f 7265 2e66 6965 6c64 7372  ino.core.fieldsr
-00004e50: 1800 0000 da0e 6c69 6e6f 2e63 6f72 652e  ......lino.core.
-00004e60: 6766 6b73 7219 0000 0072 1b00 0000 da12  gfksr....r......
-00004e70: 6c69 6e6f 2e63 6f72 652e 7265 7175 6573  lino.core.reques
-00004e80: 7473 721c 0000 0072 1d00 0000 da16 6c69  tsr....r......li
-00004e90: 6e6f 2e63 6f72 652e 7461 626c 6572 6571  no.core.tablereq
-00004ea0: 7565 7374 721e 0000 00da 0f6c 696e 6f2e  uestr......lino.
-00004eb0: 636f 7265 2e76 6965 7773 721f 0000 0072  core.viewsr....r
-00004ec0: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00004ed0: 0000 00da 0f6c 696e 6f2e 636f 7265 2e75  .....lino.core.u
-00004ee0: 7469 6c73 7224 0000 00da 116c 696e 6f2e  tilsr$.....lino.
-00004ef0: 636f 7265 2e61 6374 696f 6e73 7225 0000  core.actionsr%..
-00004f00: 0072 2600 0000 da0f 6c69 6e6f 2e63 6f72  .r&.....lino.cor
-00004f10: 652e 7374 6f72 6572 2700 0000 da17 6c69  e.storer'.....li
-00004f20: 6e6f 2e6d 6f64 6c69 622e 7573 6572 732e  no.modlib.users.
-00004f30: 7574 696c 7372 2800 0000 7229 0000 00da  utilsr(...r)....
-00004f40: 086c 696e 6f2e 6170 6972 2a00 0000 da17  .lino.apir*.....
-00004f50: 6c69 6e6f 2e6d 6f64 6c69 622e 6578 746a  lino.modlib.extj
-00004f60: 732e 7669 6577 7372 2b00 0000 722c 0000  s.viewsr+...r,..
-00004f70: 0072 2d00 0000 7238 0000 0072 e200 0000  .r-...r8...r....
-00004f80: 7259 0000 0072 a500 0000 72b4 0000 0072  rY...r....r....r
-00004f90: c400 0000 72cb 0000 0072 d000 0000 72fc  ....r....r....r.
-00004fa0: 0000 0072 1401 0000 7215 0100 0072 1701  ...r....r....r..
-00004fb0: 0000 7220 0100 0072 2601 0000 722c 0100  ..r ...r&...r,..
-00004fc0: 0072 3101 0000 7241 0100 0072 4d01 0000  .r1...rA...rM...
-00004fd0: 7236 0000 0072 3600 0000 7236 0000 0072  r6...r6...r6...r
-00004fe0: 3700 0000 da08 3c6d 6f64 756c 653e 0100  7.....<module>..
-00004ff0: 0000 737c 0000 0004 040c 0308 0108 0108  ..s|............
-00005000: 0108 0108 0108 0108 010c 010c 0110 010c  ................
-00005010: 010c 020c 010c 010c 010c 010c 010c 010c  ................
-00005020: 010c 010c 010c 030c 010c 010c 010c 010c  ................
-00005030: 010c 010c 0110 010c 0110 0110 010c 010c  ................
-00005040: 010c 010c 010c 0110 020c 0114 010a 0304  ................
-00005050: 0e10 0710 2210 7110 0f10 2a10 1f10 1008  ....".q...*.....
-00005060: 5e08 1310 4310 0410 0810 1010 1610 0a10  ^...C...........
-00005070: 3214 33                                  2.3
+00000700: da01 78a9 0072 3600 0000 fa42 2f68 6f6d  ..x..r6....B/hom
+00000710: 652f 626c 7572 7279 2f6c 696e 6f2f 656e  e/blurry/lino/en
+00000720: 762f 7265 706f 7369 746f 7269 6573 2f72  v/repositories/r
+00000730: 6561 6374 2f6c 696e 6f5f 7265 6163 742f  eact/lino_react/
+00000740: 7265 6163 742f 7669 6577 732e 7079 da04  react/views.py..
+00000750: 6669 6e64 3800 0000 7310 0000 0018 0210  find8...s.......
+00000760: 0204 0108 0108 0108 0102 ff04 0372 3800  .............r8.
+00000770: 0000 7a21 2573 2068 6173 206e 6f20 726f  ..z!%s has no ro
+00000780: 7720 7769 7468 2070 7269 6d61 7279 206b  w with primary k
+00000790: 6579 2025 7263 0000 0000 0000 0000 0000  ey %rc..........
+000007a0: 0000 0000 0000 0300 0000 4000 0000 732a  ..........@...s*
+000007b0: 0000 0065 005a 0164 005a 0264 0864 0264  ...e.Z.d.Z.d.d.d
+000007c0: 0384 015a 0364 0864 0464 0584 015a 0464  ...Z.d.d.d...Z.d
+000007d0: 0864 0664 0784 015a 0564 0153 0029 0972  .d.d...Z.d.S.).r
+000007e0: 2b00 0000 4e63 0500 0000 0000 0000 0000  +...Nc..........
+000007f0: 0000 0800 0000 0800 0000 4300 0000 7354  ..........C...sT
+00000800: 0000 007c 016a 007d 0574 017c 027c 037c  ...|.j.}.t.|.|.|
+00000810: 017c 0564 0174 026a 036a 046a 056a 0664  .|.d.t.j.j.j.j.d
+00000820: 028d 067d 067c 0464 036b 0272 1e7c 06a0  ...}.|.d.k.r.|..
+00000830: 07a1 007d 077c 0767 017c 065f 086e 057c  ...}.|.g.|._.n.|
+00000840: 06a0 097c 04a1 0101 0074 026a 036a 0aa0  ...|.....t.j.j..
+00000850: 0b7c 06a1 0153 0029 044e 54a9 01da 0872  .|...S.).NT....r
+00000860: 656e 6465 7265 72fa 062d 3939 3939 3829  enderer..-99998)
+00000870: 0cda 0450 4f53 5472 2000 0000 720b 0000  ...POSTr ...r...
+00000880: 00da 0453 4954 45da 0770 6c75 6769 6e73  ...SITE..plugins
+00000890: da05 7265 6163 7472 3a00 0000 da0f 6372  ..reactr:.....cr
+000008a0: 6561 7465 5f69 6e73 7461 6e63 65da 0d73  eate_instance..s
+000008b0: 656c 6563 7465 645f 726f 7773 da10 7365  elected_rows..se
+000008c0: 745f 7365 6c65 6374 6564 5f70 6b73 7226  t_selected_pksr&
+000008d0: 0000 00da 0a72 756e 5f61 6374 696f 6e29  .....run_action)
+000008e0: 08da 0473 656c 66da 0772 6571 7565 7374  ...self..request
+000008f0: da09 6170 705f 6c61 6265 6cda 0561 6374  ..app_label..act
+00000900: 6f72 da02 706b da04 6461 7461 da02 6172  or..pk..data..ar
+00000910: da04 656c 656d 7236 0000 0072 3600 0000  ..elemr6...r6...
+00000920: 7237 0000 00da 0470 6f73 744f 0000 0073  r7.....postO...s
+00000930: 1400 0000 0602 0201 0a01 0a01 06fe 0803  ................
+00000940: 0801 0a01 0a02 0e01 7a0f 4170 6945 6c65  ........z.ApiEle
+00000950: 6d65 6e74 2e70 6f73 7463 0500 0000 0000  ment.postc......
+00000960: 0000 0000 0000 0700 0000 0800 0000 4300  ..............C.
+00000970: 0000 f340 0000 0074 00a0 017c 016a 02a1  ...@...t...|.j..
+00000980: 017d 0574 037c 027c 037c 017c 0564 0174  .}.t.|.|.|.|.d.t
+00000990: 046a 056a 066a 076a 0864 028d 067d 067c  .j.j.j.j.d...}.|
+000009a0: 06a0 097c 04a1 0101 0074 046a 056a 0aa0  ...|.....t.j.j..
+000009b0: 0b7c 06a1 0153 00a9 034e 4672 3900 0000  .|...S...NFr9...
+000009c0: a90c 7209 0000 00da 0951 7565 7279 4469  ..r......QueryDi
+000009d0: 6374 da04 626f 6479 7220 0000 0072 0b00  ct..bodyr ...r..
+000009e0: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
+000009f0: 0072 3a00 0000 7242 0000 0072 2600 0000  .r:...rB...r&...
+00000a00: 7243 0000 00a9 0772 4400 0000 7245 0000  rC.....rD...rE..
+00000a10: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
+00000a20: 7249 0000 0072 4a00 0000 7236 0000 0072  rI...rJ...r6...r
+00000a30: 3600 0000 7237 0000 00da 0370 7574 5c00  6...r7.....put\.
+00000a40: 0000 730e 0000 000c 0102 030a 010a 0106  ..s.............
+00000a50: fe0a 030e 017a 0e41 7069 456c 656d 656e  .....z.ApiElemen
+00000a60: 742e 7075 7463 0500 0000 0000 0000 0000  t.putc..........
+00000a70: 0000 0700 0000 0800 0000 4300 0000 724d  ..........C...rM
+00000a80: 0000 0072 4e00 0000 724f 0000 0072 5200  ...rN...rO...rR.
+00000a90: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00000aa0: 00da 0664 656c 6574 6566 0000 0073 0e00  ...deletef...s..
+00000ab0: 0000 0c01 0201 0a01 0a01 06fe 0a03 0e01  ................
+00000ac0: 7a11 4170 6945 6c65 6d65 6e74 2e64 656c  z.ApiElement.del
+00000ad0: 6574 65a9 034e 4e4e 2906 da08 5f5f 6e61  ete..NNN)...__na
+00000ae0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000af0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 724c  ..__qualname__rL
+00000b00: 0000 0072 5300 0000 7254 0000 0072 3600  ...rS...rT...r6.
+00000b10: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00000b20: 0072 2b00 0000 4d00 0000 7308 0000 0008  .r+...M...s.....
+00000b30: 000a 020a 0d0e 0a72 2b00 0000 6300 0000  .......r+...c...
+00000b40: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000b50: 0040 0000 0073 2000 0000 6500 5a01 6400  .@...s ...e.Z.d.
+00000b60: 5a02 6406 6402 6403 8401 5a03 6406 6404  Z.d.d.d...Z.d.d.
+00000b70: 6405 8401 5a04 6401 5300 2907 da07 4170  d...Z.d.S.)...Ap
+00000b80: 694c 6973 744e 6304 0000 0000 0000 0000  iListNc.........
+00000b90: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00000ba0: 3400 0000 7400 7c02 7c03 7c01 7c01 6a01  4...t.|.|.|.|.j.
+00000bb0: 6401 8305 7d04 7c04 a002 a100 0100 7403  d...}.|.......t.
+00000bc0: 6a04 6a05 6a06 7c04 5f07 7403 6a04 6a05  j.j.j.|._.t.j.j.
+00000bd0: a008 7c04 a101 5300 2902 4e54 2909 7220  ..|...S.).NT).r 
+00000be0: 0000 0072 3c00 0000 da0a 6765 745f 7374  ...r<.....get_st
+00000bf0: 6174 7573 720b 0000 0072 3d00 0000 7226  atusr....r=...r&
+00000c00: 0000 00da 1064 6566 6175 6c74 5f72 656e  .....default_ren
+00000c10: 6465 7265 7272 3a00 0000 7243 0000 0029  dererr:...rC...)
+00000c20: 0572 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
+00000c30: 7247 0000 0072 4a00 0000 7236 0000 0072  rG...rJ...r6...r
+00000c40: 3600 0000 7237 0000 0072 4c00 0000 7000  6...r7...rL...p.
+00000c50: 0000 7308 0000 0012 0108 010c 010e 017a  ..s............z
+00000c60: 0c41 7069 4c69 7374 2e70 6f73 7463 0400  .ApiList.postc..
+00000c70: 0000 0000 0000 0000 0000 1300 0000 0800  ................
+00000c80: 0000 0300 0000 7376 0200 0074 007c 0183  ......sv...t.|..
+00000c90: 017d 047c 0472 0a74 017c 0483 0153 0074  .}.|.r.t.|...S.t
+00000ca0: 027c 027c 037c 017c 016a 0364 0183 0589  .|.|.|.|.j.d....
+00000cb0: 0088 00a0 04a1 0073 2064 02a0 0588 00a1  .......s d......
+00000cc0: 017d 0574 067c 0583 0182 0174 076a 086a  .}.t.|.....t.j.j
+00000cd0: 096a 0a88 005f 0b88 006a 0c89 027c 016a  .j..._...j...|.j
+00000ce0: 03a0 0d74 0e6a 0f88 006a 106a 116a 12a1  ...t.j...j.j.j..
+00000cf0: 027d 067c 016a 03a0 0d74 0e6a 13a1 017d  .}.|.j...t.j...}
+00000d00: 077c 0772 4474 076a 086a 09a0 1488 00a1  .|.rDt.j.j......
+00000d10: 0153 007c 0674 0e6a 156b 0290 0172 3474  .S.|.t.j.k...r4t
+00000d20: 1688 006a 106a 1174 1783 0272 6088 00a0  ...j.j.t...r`...
+00000d30: 18a1 007d 0874 1988 0088 006a 0c7c 0883  ...}.t.....j.|..
+00000d40: 037d 0974 017c 0983 0153 007c 016a 03a0  .}.t.|...S.|.j..
+00000d50: 0d74 0e6a 1a74 0e6a 1ba1 0289 0188 0174  .t.j.t.j.......t
+00000d60: 0e6a 1c6b 0272 8864 037d 0a67 007d 0b88  .j.k.r.d.}.g.}..
+00000d70: 006a 1d44 005d 117d 0c7c 0a7c 0ca0 1e88  .j.D.].}.|.|....
+00000d80: 00a1 0137 007d 0a7c 0ba0 1f64 047c 0c6a  ...7.}.|...d.|.j
+00000d90: 2069 01a1 0101 0071 756e 4088 0174 0e6a   i.....qun@..t.j
+00000da0: 216b 0272 b464 037d 0a67 007d 0b88 006a  !k.r.d.}.g.}...j
+00000db0: 1d44 005d 1e7d 0c88 00a0 227c 0ca1 017d  .D.].}...."|...}
+00000dc0: 0d88 00a0 237c 0c7c 0da1 027d 0d64 05a0  ....#|.|...}.d..
+00000dd0: 057c 0da1 017d 0d7c 0a7c 0d37 007d 0a7c  .|...}.|.|.7.}.|
+00000de0: 0ba0 1f64 047c 0c6a 2069 01a1 0101 0071  ...d.|.j i.....q
+00000df0: 946e 1464 007d 0a87 0187 0266 0264 0664  .n.d.}.....f.d.d
+00000e00: 0784 0889 0387 0087 0366 0264 0864 0984  .........f.d.d..
+00000e10: 0888 006a 1d44 0083 017d 0b88 00a0 24a1  ...j.D...}....$.
+00000e20: 007d 0e88 0174 0e6a 1b6b 0272 fb88 00a0  .}...t.j.k.r....
+00000e30: 25a1 0044 005d 257d 0f88 006a 2664 0075  %..D.]%}...j&d.u
+00000e40: 0073 ec74 277c 0b83 0164 0a17 0088 006a  .s.t'|...d.....j
+00000e50: 266b 0073 ec88 006a 267c 0e64 0a17 006b  &k.s...j&|.d...k
+00000e60: 0272 f688 0388 007c 0f83 027d 107c 0ba0  .r.....|...}.|..
+00000e70: 1f7c 10a1 0101 007c 0e64 0a37 007d 0e71  .|.....|.d.7.}.q
+00000e80: d574 287c 0e7c 0b7c 0a64 0188 006a 2988  .t(|.|.|.d...j).
+00000e90: 00a0 2aa1 0064 0b8d 067d 1188 0174 0e6a  ..*..d...}...t.j
+00000ea0: 1b6b 0390 0172 1d88 00a0 2ba1 007d 127c  .k...r....+..}.|
+00000eb0: 1264 0075 0190 0172 1d7c 0ba0 2c64 0c7c  .d.u...r.|..,d.|
+00000ec0: 12a1 0201 0088 006a 2d6a 2e90 0172 307c  .......j-j...r0|
+00000ed0: 116a 2f88 006a 2d6a 306a 31a0 3288 0088  .j/..j-j0j1.2...
+00000ee0: 006a 33a1 0264 0d8d 0101 0074 017c 1183  .j3..d.....t.|..
+00000ef0: 0153 0074 076a 086a 09a0 1488 00a1 0153  .S.t.j.j.......S
+00000f00: 0029 0e4e 547a 174e 6f20 7065 726d 6973  .).NTz.No permis
+00000f10: 7369 6f6e 2074 6f20 7275 6e20 7b7d da00  sion to run {}..
+00000f20: da02 6964 7a09 3c70 3e7b 7d3c 2f70 3e63  ..idz.<p>{}</p>c
+00000f30: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000f40: 0700 0000 1300 0000 7362 0000 0088 0074  ........sb.....t
+00000f50: 006a 016b 0272 0c88 016a 02a0 037c 007c  .j.k.r...j...|.|
+00000f60: 01a1 0253 0088 0074 006a 046b 0272 167c  ...S...t.j.k.r.|
+00000f70: 01a0 057c 00a1 0153 0088 0074 006a 066b  ...|...S...t.j.k
+00000f80: 0272 2088 016a 026a 077d 026e 0488 016a  .r ..j.j.}.n...j
+00000f90: 026a 087d 0288 016a 026a 097c 007c 017c  .j.}...j.j.|.|.|
+00000fa0: 027c 00a0 0a7c 01a1 0164 018d 0453 0029  .|...|...d...S.)
+00000fb0: 027a 4f55 7365 2064 6973 706c 6179 5f6d  .zOUse display_m
+00000fc0: 6f64 6520 746f 2064 6574 6572 6d69 6e65  ode to determine
+00000fd0: 2077 6869 6368 2073 6572 696c 6973 6174   which serilisat
+00000fe0: 696f 6e20 7374 6f72 6520 6d65 7468 6f64  ion store method
+00000ff0: 2061 6e64 2066 6965 6c64 7320 746f 2075   and fields to u
+00001000: 7365 2902 7216 0000 00da 0a63 6172 645f  se).r......card_
+00001010: 7469 746c 6529 0b72 1b00 0000 da12 4449  title).r......DI
+00001020: 5350 4c41 595f 4d4f 4445 5f54 4142 4c45  SPLAY_MODE_TABLE
+00001030: da05 7374 6f72 65da 0872 6f77 326c 6973  ..store..row2lis
+00001040: 74da 1444 4953 504c 4159 5f4d 4f44 455f  t..DISPLAY_MODE_
+00001050: 4741 4c4c 4552 59da 1067 6574 5f67 616c  GALLERY..get_gal
+00001060: 6c65 7279 5f69 7465 6dda 1244 4953 504c  lery_item..DISPL
+00001070: 4159 5f4d 4f44 455f 4341 5244 53da 0b63  AY_MODE_CARDS..c
+00001080: 6172 645f 6669 656c 6473 da0d 6465 7461  ard_fields..deta
+00001090: 696c 5f66 6965 6c64 73da 0872 6f77 3264  il_fields..row2d
+000010a0: 6963 74da 0e67 6574 5f63 6172 645f 7469  ict..get_card_ti
+000010b0: 746c 6529 0372 4a00 0000 da03 726f 7772  tle).rJ.....rowr
+000010c0: 1600 0000 2902 da0c 6469 7370 6c61 795f  ....)...display_
+000010d0: 6d6f 6465 da02 7268 7236 0000 0072 3700  mode..rhr6...r7.
+000010e0: 0000 da09 7365 7269 616c 697a 65b3 0000  ....serialize...
+000010f0: 0073 1400 0000 0a02 0e01 0a01 0a02 0a02  .s..............
+00001100: 0a01 0802 0801 0c01 06ff 7a1e 4170 694c  ..........z.ApiL
+00001110: 6973 742e 6765 742e 3c6c 6f63 616c 733e  ist.get.<locals>
+00001120: 2e73 6572 6961 6c69 7a65 6301 0000 0000  .serializec.....
+00001130: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00001140: 0000 0073 1600 0000 6700 7c00 5d07 7d01  ...s....g.|.].}.
+00001150: 8801 8800 7c01 8302 9102 7102 5300 7236  ....|.....q.S.r6
+00001160: 0000 0072 3600 0000 a902 da02 2e30 7269  ...r6........0ri
+00001170: 0000 0029 0272 4a00 0000 726c 0000 0072  ...).rJ...rl...r
+00001180: 3600 0000 7237 0000 00da 0a3c 6c69 7374  6...r7.....<list
+00001190: 636f 6d70 3ec2 0000 0073 0600 0000 0600  comp>....s......
+000011a0: 0201 0eff 7a1f 4170 694c 6973 742e 6765  ....z.ApiList.ge
+000011b0: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
+000011c0: 636f 6d70 3ee9 0100 0000 2906 da05 636f  comp>.....)...co
+000011d0: 756e 74da 0472 6f77 73da 0968 746d 6c5f  unt..rows..html_
+000011e0: 7465 7874 da07 7375 6363 6573 73da 0c6e  text..success..n
+000011f0: 6f5f 6461 7461 5f74 6578 74da 0574 6974  o_data_text..tit
+00001200: 6c65 7201 0000 0029 01da 0c70 6172 616d  ler....)...param
+00001210: 5f76 616c 7565 7329 3472 2c00 0000 7221  _values)4r,...r!
+00001220: 0000 0072 2000 0000 da03 4745 54da 0e67  ...r .....GET..g
+00001230: 6574 5f70 6572 6d69 7373 696f 6eda 0666  et_permission..f
+00001240: 6f72 6d61 7472 1200 0000 720b 0000 0072  ormatr....r....r
+00001250: 3d00 0000 7226 0000 0072 5b00 0000 723a  =...r&...r[...r:
+00001260: 0000 00da 0261 68da 0367 6574 721b 0000  .....ah..getr...
+00001270: 00da 1055 524c 5f50 4152 414d 5f46 4f52  ...URL_PARAM_FOR
+00001280: 4d41 54da 0c62 6f75 6e64 5f61 6374 696f  MAT..bound_actio
+00001290: 6eda 0661 6374 696f 6eda 0e64 6566 6175  n..action..defau
+000012a0: 6c74 5f66 6f72 6d61 74da 1555 524c 5f50  lt_format..URL_P
+000012b0: 4152 414d 5f41 4354 494f 4e5f 4e41 4d45  ARAM_ACTION_NAME
+000012c0: 7243 0000 00da 0f55 524c 5f46 4f52 4d41  rC.....URL_FORMA
+000012d0: 545f 4a53 4f4e da0a 6973 696e 7374 616e  T_JSON..isinstan
+000012e0: 6365 7225 0000 0072 4000 0000 722d 0000  cer%...r@...r-..
+000012f0: 00da 1655 524c 5f50 4152 414d 5f44 4953  ...URL_PARAM_DIS
+00001300: 504c 4159 5f4d 4f44 4572 5f00 0000 da12  PLAY_MODEr_.....
+00001310: 4449 5350 4c41 595f 4d4f 4445 5f53 544f  DISPLAY_MODE_STO
+00001320: 5259 da14 736c 6963 6564 5f64 6174 615f  RY..sliced_data_
+00001330: 6974 6572 6174 6f72 da0d 6173 5f73 746f  iterator..as_sto
+00001340: 7279 5f69 7465 6dda 0661 7070 656e 6472  ry_item..appendr
+00001350: 4800 0000 da11 4449 5350 4c41 595f 4d4f  H.....DISPLAY_MO
+00001360: 4445 5f4c 4953 54da 1072 6f77 5f61 735f  DE_LIST..row_as_
+00001370: 7061 7261 6772 6170 68da 0f61 6464 5f64  paragraph..add_d
+00001380: 6574 6169 6c5f 6c69 6e6b da0f 6765 745f  etail_link..get_
+00001390: 746f 7461 6c5f 636f 756e 74da 1363 7265  total_count..cre
+000013a0: 6174 655f 7068 616e 746f 6d5f 726f 7773  ate_phantom_rows
+000013b0: da05 6c69 6d69 74da 036c 656e da04 6469  ..limit..len..di
+000013c0: 6374 7275 0000 00da 0967 6574 5f74 6974  ctru.....get_tit
+000013d0: 6c65 da0d 6765 745f 6d61 696e 5f63 6172  le..get_main_car
+000013e0: 64da 0669 6e73 6572 7472 4700 0000 da0a  d..insertrG.....
+000013f0: 7061 7261 6d65 7465 7273 da06 7570 6461  parameters..upda
+00001400: 7465 da0d 7061 7261 6d73 5f6c 6179 6f75  te..params_layou
+00001410: 74da 0c70 6172 616d 735f 7374 6f72 65da  t..params_store.
+00001420: 0770 7632 6469 6374 7277 0000 0029 1372  .pv2dictrw...).r
+00001430: 4400 0000 7245 0000 0072 4600 0000 7247  D...rE...rF...rG
+00001440: 0000 00da 0276 6dda 036d 7367 da03 666d  .....vm..msg..fm
+00001450: 74da 0b61 6374 696f 6e5f 6e61 6d65 724b  t..action_namerK
+00001460: 0000 00da 0764 6174 6172 6563 7273 0000  .....datarecrs..
+00001470: 0072 7200 0000 da03 6f62 6ada 0370 6172  .rr.....obj..par
+00001480: da0b 746f 7461 6c5f 636f 756e 7472 6900  ..total_countri.
+00001490: 0000 da01 64da 026b 77da 026d 6372 3600  ....d..kw..mcr6.
+000014a0: 0000 2904 724a 0000 0072 6a00 0000 726b  ..).rJ...rj...rk
+000014b0: 0000 0072 6c00 0000 7237 0000 0072 7c00  ...rl...r7...r|.
+000014c0: 0000 7600 0000 7390 0000 0008 0104 0108  ..v...s.........
+000014d0: 0112 0108 080a 0108 020c 0206 0106 0204  ................
+000014e0: 0108 0104 fe0e 0404 020e 010c 020e 0108  ................
+000014f0: 010e 0108 0106 0208 0104 ff0a 0304 0104  ................
+00001500: 010a 010e 0112 0102 fe0a 0304 0104 010a  ................
+00001510: 010a 010c 010a 0208 0612 0102 f504 0d0e  ................
+00001520: 010c 0f04 0106 ff08 030a 010c 012a 010a  .............*..
+00001530: 010a 010a 0104 0202 0102 0102 0104 0106  ................
+00001540: 0106 fb0c 0608 010a 010c 010a 0104 010a  ................
+00001550: 0106 0102 ff06 ff08 030e 027a 0b41 7069  ...........z.Api
+00001560: 4c69 7374 2e67 6574 2902 4e4e 2905 7256  List.get).NN).rV
+00001570: 0000 0072 5700 0000 7258 0000 0072 4c00  ...rW...rX...rL.
+00001580: 0000 727c 0000 0072 3600 0000 7236 0000  ..r|...r6...r6..
+00001590: 0072 3600 0000 7237 0000 0072 5900 0000  .r6...r7...rY...
+000015a0: 6f00 0000 7306 0000 0008 000a 010e 0672  o...s..........r
+000015b0: 5900 0000 6300 0000 0000 0000 0000 0000  Y...c...........
+000015c0: 0000 0000 0002 0000 0040 0000 00f3 1800  .........@......
+000015d0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000015e0: 6403 8400 5a04 6404 5300 2905 da0f 4368  d...Z.d.S.)...Ch
+000015f0: 6f69 6365 4c69 7374 4d6f 6465 6c7a a20a  oiceListModelz..
+00001600: 2020 2020 4372 6561 7465 7320 6120 6c61      Creates a la
+00001610: 7267 6520 4a53 4f4e 206d 6f64 656c 2074  rge JSON model t
+00001620: 6861 7420 636f 6e74 6169 6e73 2061 6c6c  hat contains all
+00001630: 2074 6865 2063 686f 6963 656c 6973 7473   the choicelists
+00001640: 202b 2063 686f 6963 6573 0a0a 2020 2020   + choices..    
+00001650: 4e6f 7465 3a20 5468 6973 2063 6f75 6c64  Note: This could
+00001660: 2062 6520 696d 7072 6f76 6564 2c20 6f72   be improved, or
+00001670: 206d 6967 6874 2063 6175 7365 2069 7373   might cause iss
+00001680: 7565 7320 6475 6520 746f 2063 6861 6e67  ues due to chang
+00001690: 696e 6720 6c61 6e67 7561 6765 0a20 2020  ing language.   
+000016a0: 2063 0200 0000 0000 0000 0000 0000 0300   c..............
+000016b0: 0000 0300 0000 4300 0000 731c 0000 0064  ......C...s....d
+000016c0: 0164 0284 0074 006a 01a0 02a1 0044 0083  .d...t.j.....D..
+000016d0: 017d 0274 037c 0283 0153 0029 034e 6301  .}.t.|...S.).Nc.
+000016e0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+000016f0: 0000 0053 0000 0073 2400 0000 6900 7c00  ...S...s$...i.|.
+00001700: 5d0e 7d01 7400 7c01 8301 6400 6401 8400  ].}.t.|...d.d...
+00001710: 7c01 a001 a100 4400 8301 9302 7102 5300  |.....D.....q.S.
+00001720: 2902 6301 0000 0000 0000 0000 0000 0002  ).c.............
+00001730: 0000 0006 0000 0053 0000 0073 3200 0000  .......S...s2...
+00001740: 6700 7c00 5d15 7d01 7400 7c01 6400 1900  g.|.].}.t.|.d...
+00001750: 8301 a001 6401 a101 7400 7c01 6402 1900  ....d...t.|.d...
+00001760: 8301 a001 6401 a101 6403 9c02 9102 7102  ....d...d.....q.
+00001770: 5300 2904 7201 0000 00fa 0122 7270 0000  S.).r......"rp..
+00001780: 0029 0272 3300 0000 da04 7465 7874 2902  .).r3.....text).
+00001790: 7215 0000 00da 0573 7472 6970 2902 726e  r......strip).rn
+000017a0: 0000 00da 0163 7236 0000 0072 3600 0000  .....cr6...r6...
+000017b0: 7237 0000 0072 6f00 0000 e800 0000 7302  r7...ro.......s.
+000017c0: 0000 0032 007a 3243 686f 6963 654c 6973  ...2.z2ChoiceLis
+000017d0: 744d 6f64 656c 2e67 6574 2e3c 6c6f 6361  tModel.get.<loca
+000017e0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2e3c  ls>.<dictcomp>.<
+000017f0: 6c69 7374 636f 6d70 3e29 02da 0373 7472  listcomp>)...str
+00001800: da0b 6765 745f 6368 6f69 6365 7329 0272  ..get_choices).r
+00001810: 6e00 0000 da02 636c 7236 0000 0072 3600  n.....clr6...r6.
+00001820: 0000 7237 0000 00da 0a3c 6469 6374 636f  ..r7.....<dictco
+00001830: 6d70 3ee8 0000 0073 0600 0000 0600 0201  mp>....s........
+00001840: 1cff 7a27 4368 6f69 6365 4c69 7374 4d6f  ..z'ChoiceListMo
+00001850: 6465 6c2e 6765 742e 3c6c 6f63 616c 733e  del.get.<locals>
+00001860: 2e3c 6469 6374 636f 6d70 3e29 0472 2600  .<dictcomp>).r&.
+00001870: 0000 da0b 4348 4f49 4345 4c49 5354 53da  ....CHOICELISTS.
+00001880: 0676 616c 7565 7372 2100 0000 2903 7244  .valuesr!...).rD
+00001890: 0000 0072 4500 0000 7249 0000 0072 3600  ...rE...rI...r6.
+000018a0: 0000 7236 0000 0072 3700 0000 727c 0000  ..r6...r7...r|..
+000018b0: 00e7 0000 0073 0800 0000 0601 0802 06fe  .....s..........
+000018c0: 0803 7a13 4368 6f69 6365 4c69 7374 4d6f  ..z.ChoiceListMo
+000018d0: 6465 6c2e 6765 744e a905 7256 0000 0072  del.getN..rV...r
+000018e0: 5700 0000 7258 0000 00da 075f 5f64 6f63  W...rX.....__doc
+000018f0: 5f5f 727c 0000 0072 3600 0000 7236 0000  __r|...r6...r6..
+00001900: 0072 3600 0000 7237 0000 0072 a500 0000  .r6...r7...r....
+00001910: e000 0000 f306 0000 0008 0004 010c 0672  ...............r
+00001920: a500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001930: 0000 0000 0003 0000 0040 0000 00f3 1600  .........@......
+00001940: 0000 6500 5a01 6400 5a02 6404 6402 6403  ..e.Z.d.Z.d.d.d.
+00001950: 8401 5a03 6401 5300 2905 da07 4368 6f69  ..Z.d.S.)...Choi
+00001960: 6365 734e 6305 0000 0000 0000 0000 0000  cesNc...........
+00001970: 000b 0000 0008 0000 004b 0000 0073 7c00  .........K...s|.
+00001980: 0000 7400 7c02 7c03 8302 7d06 6401 7d07  ..t.|.|...}.d.}.
+00001990: 7c04 6401 7500 7219 7c06 6a01 7c01 6402  |.d.u.r.|.j.|.d.
+000019a0: 8d01 7d08 7c08 6a02 7d09 6403 6404 8400  ..}.|.j.}.d.d...
+000019b0: 7d0a 6e1b 7c06 a003 7c04 a101 7022 7c06  }.n.|...|...p"|.
+000019c0: a004 7c04 a101 7d04 7c04 6a05 7228 6405  ..|...}.|.j.r(d.
+000019d0: 7d07 7406 7c06 6a01 7c01 6402 8d01 7c06  }.t.|.j.|.d...|.
+000019e0: 7c04 8303 5c02 7d09 7d0a 7407 7c06 7c01  |...\.}.}.t.|.|.
+000019f0: 7c09 7c0a 7c07 7c04 6406 8d06 5300 2907  |.|.|.|.d...S.).
+00001a00: 6141 0100 0049 6620 6066 6c64 6e61 6d65  aA...If `fldname
+00001a10: 6020 6973 2073 7065 6369 6669 6564 2c20  ` is specified, 
+00001a20: 7265 7475 726e 2061 204a 534f 4e20 6f62  return a JSON ob
+00001a30: 6a65 6374 2077 6974 6820 7477 6f0a 2020  ject with two.  
+00001a40: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
+00001a50: 2060 636f 756e 7460 2061 6e64 2060 726f   `count` and `ro
+00001a60: 7773 602c 2077 6865 7265 2060 726f 7773  ws`, where `rows
+00001a70: 6020 6973 2061 206c 6973 7420 6f66 0a20  ` is a list of. 
+00001a80: 2020 2020 2020 2060 2864 6973 706c 6179         `(display
+00001a90: 5f74 6578 742c 2076 616c 7565 2960 2074  _text, value)` t
+00001aa0: 7570 6c65 732e 2020 5573 6564 2062 7920  uples.  Used by 
+00001ab0: 436f 6d62 6f42 6f78 6573 206f 7220 7369  ComboBoxes or si
+00001ac0: 6d69 6c61 720a 2020 2020 2020 2020 7769  milar.        wi
+00001ad0: 6467 6574 732e 0a0a 2020 2020 2020 2020  dgets...        
+00001ae0: 4966 2060 666c 646e 616d 6560 2069 7320  If `fldname` is 
+00001af0: 6e6f 7420 7370 6563 6966 6965 642c 2072  not specified, r
+00001b00: 6574 7572 6e73 2074 6865 2063 686f 6963  eturns the choic
+00001b10: 6573 2066 6f72 2074 6865 0a20 2020 2020  es for the.     
+00001b20: 2020 2060 7265 636f 7264 5f73 656c 6563     `record_selec
+00001b30: 746f 7260 2077 6964 6765 742e 0a0a 2020  tor` widget...  
+00001b40: 2020 2020 2020 4ea9 0172 4500 0000 6302        N..rE...c.
+00001b50: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001b60: 0000 0053 0000 0073 1e00 0000 7400 7c00  ...S...s....t.|.
+00001b70: 8301 7c01 7401 6a02 3c00 7c00 6a03 7c01  ..|.t.j.<.|.j.|.
+00001b80: 7401 6a04 3c00 7c01 5300 a901 4e29 0572  t.j.<.|.S...N).r
+00001b90: aa00 0000 721b 0000 00da 1243 484f 4943  ....r......CHOIC
+00001ba0: 4553 5f54 4558 545f 4649 454c 4472 4800  ES_TEXT_FIELDrH.
+00001bb0: 0000 da13 4348 4f49 4345 535f 5641 4c55  ....CHOICES_VALU
+00001bc0: 455f 4649 454c 4429 0272 9e00 0000 72a1  E_FIELD).r....r.
+00001bd0: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00001be0: 0000 7267 0000 0007 0100 0073 0600 0000  ..rg.......s....
+00001bf0: 0e01 0c02 0401 7a1d 4368 6f69 6365 732e  ......z.Choices.
+00001c00: 6765 742e 3c6c 6f63 616c 733e 2e72 6f77  get.<locals>.row
+00001c10: 3264 6963 7472 5c00 0000 a901 da05 6669  2dictr\.......fi
+00001c20: 656c 6429 0872 1f00 0000 7245 0000 00da  eld).r....rE....
+00001c30: 0d64 6174 615f 6974 6572 6174 6f72 da0e  .data_iterator..
+00001c40: 6765 745f 7061 7261 6d5f 656c 656d da0d  get_param_elem..
+00001c50: 6765 745f 6461 7461 5f65 6c65 6dda 0562  get_data_elem..b
+00001c60: 6c61 6e6b 7218 0000 0072 2300 0000 290b  lankr....r#...).
+00001c70: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
+00001c80: 4700 0000 72ba 0000 0072 a200 0000 da03  G...r....r......
+00001c90: 7270 74da 0a65 6d70 7479 5661 6c75 6572  rpt..emptyValuer
+00001ca0: 4a00 0000 da02 7173 7267 0000 0072 3600  J.....qsrg...r6.
+00001cb0: 0000 7236 0000 0072 3700 0000 727c 0000  ..r6...r7...r|..
+00001cc0: 00f0 0000 0073 1600 0000 0a0a 0401 0801  .....s..........
+00001cd0: 0c01 0606 0a04 1409 0601 0402 1801 1402  ................
+00001ce0: 7a0b 4368 6f69 6365 732e 6765 7472 5500  z.Choices.getrU.
+00001cf0: 0000 a904 7256 0000 0072 5700 0000 7258  ....rV...rW...rX
+00001d00: 0000 0072 7c00 0000 7236 0000 0072 3600  ...r|...r6...r6.
+00001d10: 0000 7236 0000 0072 3700 0000 72b4 0000  ..r6...r7...r...
+00001d20: 00ef 0000 00f3 0400 0000 0800 0e01 72b4  ..............r.
+00001d30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001d40: 0000 0000 0300 0000 4000 0000 72b3 0000  ........@...r...
+00001d50: 0029 05da 0c44 656c 6179 6564 5661 6c75  .)...DelayedValu
+00001d60: 654e 6306 0000 0000 0000 0000 0000 000d  eNc.............
+00001d70: 0000 0005 0000 004b 0000 0073 9e00 0000  .......K...s....
+00001d80: 7400 7c02 7c03 8302 7d07 7c07 a001 7c05  t.|.|...}.|...|.
+00001d90: a101 7d08 7c08 6400 7500 7215 6401 a002  ..}.|.d.u.r.d...
+00001da0: 7c07 7c05 a102 7d09 6e34 7c07 6a03 7c01  |.|...}.n4|.j.|.
+00001db0: 7404 6a05 6a06 6a07 6a08 6402 8d02 7d0a  t.j.j.j.j.d...}.
+00001dc0: 7c04 6403 6b02 7227 6400 7d0b 6e0a 7c0a  |.d.k.r'd.}.n.|.
+00001dd0: a009 7c04 a101 0100 7c0a 6a0a 6404 1900  ..|.....|.j.d...
+00001de0: 7d0b 740b 7c07 7c08 7c05 8303 7d0c 7c0c  }.t.|.|.|...}.|.
+00001df0: 6400 7500 7243 6405 a002 7c07 7c08 7c05  d.u.rCd...|.|.|.
+00001e00: a103 7d09 6e06 7c0c a00c 7c0b 7c0a a102  ..}.n.|...|.|...
+00001e10: 7d09 740d 6406 7c09 6901 8301 5300 2907  }.t.d.|.i...S.).
+00001e20: 4e7a 197b 7d20 6861 7320 6e6f 2064 6174  Nz.{} has no dat
+00001e30: 6120 656c 656d 656e 7420 7b7d a902 7245  a element {}..rE
+00001e40: 0000 0072 3a00 0000 723b 0000 0072 0100  ...r:...r;...r..
+00001e50: 0000 7a2c 4f6f 7073 2c20 6765 745f 6174  ..z,Oops, get_at
+00001e60: 6f6d 697a 6572 287b 7d2c 207b 7d2c 207b  omizer({}, {}, {
+00001e70: 7d29 2072 6574 7572 6e65 6420 4e6f 6e65  }) returned None
+00001e80: 7249 0000 0029 0e72 1f00 0000 72bd 0000  rI...).r....r...
+00001e90: 0072 7a00 0000 7245 0000 0072 0b00 0000  .rz...rE...r....
+00001ea0: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
+00001eb0: 3a00 0000 7242 0000 0072 4100 0000 7227  :...rB...rA...r'
+00001ec0: 0000 00da 1666 756c 6c5f 7661 6c75 655f  .....full_value_
+00001ed0: 6672 6f6d 5f6f 626a 6563 7472 2100 0000  from_objectr!...
+00001ee0: 290d 7244 0000 0072 4500 0000 7246 0000  ).rD...rE...rF..
+00001ef0: 0072 4700 0000 7248 0000 0072 ba00 0000  .rG...rH...r....
+00001f00: 72a2 0000 0072 bf00 0000 da02 6465 da01  r....r......de..
+00001f10: 7672 4a00 0000 7269 0000 00da 0273 6672  vrJ...ri.....sfr
+00001f20: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
+00001f30: 0000 001a 0100 0073 1c00 0000 0a01 0a07  .......s........
+00001f40: 0801 0e01 1602 0801 0601 0a02 0a01 0c02  ................
+00001f50: 0801 1001 0c02 0c03 7a10 4465 6c61 7965  ........z.Delaye
+00001f60: 6456 616c 7565 2e67 6574 a904 4e4e 4e4e  dValue.get..NNNN
+00001f70: 72c2 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00001f80: 3600 0000 7237 0000 0072 c400 0000 1901  6...r7...r......
+00001f90: 0000 72c3 0000 0072 c400 0000 6300 0000  ..r....r....c...
+00001fa0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00001fb0: 0040 0000 0072 b300 0000 2905 da12 4163  .@...r....)...Ac
+00001fc0: 7469 6f6e 5061 7261 6d43 686f 6963 6573  tionParamChoices
+00001fd0: 4e63 0600 0000 0000 0000 0000 0000 0b00  Nc..............
+00001fe0: 0000 0800 0000 4b00 0000 7376 0000 0074  ......K...sv...t
+00001ff0: 007c 027c 0383 027d 037c 03a0 017c 04a1  .|.|...}.|...|..
+00002000: 017d 077c 0764 0075 0072 1674 0264 017c  .}.|.d.u.r.t.d.|
+00002010: 047c 0366 0216 0083 0182 017c 076a 03a0  .|.f.......|.j..
+00002020: 047c 05a1 017d 0574 057c 076a 067c 0164  .|...}.t.|.j.|.d
+00002030: 028d 017c 076a 037c 0583 035c 027d 087d  ...|.j.|...\.}.}
+00002040: 097c 056a 0772 2f64 037d 0a6e 0264 007d  .|.j.r/d.}.n.d.}
+00002050: 0a74 087c 037c 017c 087c 097c 0a7c 0564  .t.|.|.|.|.|.|.d
+00002060: 048d 0653 0029 054e 7a18 556e 6b6e 6f77  ...S.).Nz.Unknow
+00002070: 6e20 6163 7469 6f6e 2025 7220 666f 7220  n action %r for 
+00002080: 2573 72b5 0000 007a 053c 6272 2f3e 72b9  %sr....z.<br/>r.
+00002090: 0000 0029 0972 1f00 0000 da0e 6765 745f  ...).r......get_
+000020a0: 7572 6c5f 6163 7469 6f6e da09 4578 6365  url_action..Exce
+000020b0: 7074 696f 6e72 7f00 0000 72bc 0000 0072  ptionr....r....r
+000020c0: 1800 0000 7245 0000 0072 be00 0000 7223  ....rE...r....r#
+000020d0: 0000 0029 0b72 4400 0000 7245 0000 0072  ...).rD...rE...r
+000020e0: 4600 0000 7247 0000 00da 0261 6e72 ba00  F...rG.....anr..
+000020f0: 0000 72a2 0000 00da 0262 6172 c100 0000  ..r......bar....
+00002100: 7267 0000 0072 c000 0000 7236 0000 0072  rg...r....r6...r
+00002110: 3600 0000 7237 0000 0072 7c00 0000 3a01  6...r7...r|...:.
+00002120: 0000 7314 0000 000a 010a 0108 0110 010c  ..s.............
+00002130: 011a 0106 0106 0104 0214 017a 1641 6374  ...........z.Act
+00002140: 696f 6e50 6172 616d 4368 6f69 6365 732e  ionParamChoices.
+00002150: 6765 7472 ca00 0000 72c2 0000 0072 3600  getr....r....r6.
+00002160: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00002170: 0072 cb00 0000 3801 0000 7304 0000 0008  .r....8...s.....
+00002180: 000e 0272 cb00 0000 6300 0000 0000 0000  ...r....c.......
+00002190: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000021a0: 0073 2e00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000021b0: 5a03 6409 6403 6404 8401 5a04 6409 6405  Z.d.d.d...Z.d.d.
+000021c0: 6406 8401 5a05 6409 6407 6408 8401 5a06  d...Z.d.d.d...Z.
+000021d0: 6402 5300 290a da07 5265 7374 6675 6c7a  d.S.)...Restfulz
+000021e0: 3c0a 2020 2020 5573 6564 2074 6f20 636f  <.    Used to co
+000021f0: 6c6c 6162 6f72 6174 6520 7769 7468 2061  llaborate with a
+00002200: 2072 6573 7466 756c 2045 7874 2e64 6174   restful Ext.dat
+00002210: 612e 5374 6f72 652e 0a20 2020 204e 6305  a.Store..    Nc.
+00002220: 0000 0000 0000 0000 0000 0009 0000 0006  ................
+00002230: 0000 0043 0000 0073 8800 0000 7400 7c02  ...C...s....t.|.
+00002240: 7c03 8302 7d05 7c05 6a01 7c01 6401 8d01  |...}.|.j.|.d...
+00002250: 7d06 7c06 a002 a100 7d07 7c06 6a03 6a04  }.|.....}.|.j.j.
+00002260: 6400 7501 721c 7c06 6a03 a004 7c07 7c01  d.u.r.|.j...|.|.
+00002270: a102 0100 7c01 6a05 a006 6402 a101 7d08  ....|.j...d...}.
+00002280: 7407 a008 7c08 a101 7d08 7c06 a009 7c08  t...|...}.|...|.
+00002290: 7c07 6403 a103 0100 7c06 6a0a 7c06 6a0b  |.d.....|.j.|.j.
+000022a0: 6a0c a00d 7c06 7c07 7c06 6a0b 6a0c 6a0e  j...|.|.|.j.j.j.
+000022b0: a103 6701 6404 8d01 0100 740f 7c06 6a10  ..g.d.....t.|.j.
+000022c0: 8301 5300 2905 4e72 b500 0000 7272 0000  ..S.).Nr....rr..
+000022d0: 0054 a901 7272 0000 0029 1172 1f00 0000  .T..rr...).r....
+000022e0: 7245 0000 0072 4000 0000 7247 0000 00da  rE...r@...rG....
+000022f0: 1568 616e 646c 655f 7570 6c6f 6164 6564  .handle_uploaded
+00002300: 5f66 696c 6573 723c 0000 0072 7c00 0000  _filesr<...r|...
+00002310: da04 6a73 6f6e da05 6c6f 6164 73da 1166  ..json..loads..f
+00002320: 6f72 6d32 6f62 6a5f 616e 645f 7361 7665  orm2obj_and_save
+00002330: da0c 7365 745f 7265 7370 6f6e 7365 727b  ..set_responser{
+00002340: 0000 0072 6000 0000 7267 0000 00da 0b6c  ...r`...rg.....l
+00002350: 6973 745f 6669 656c 6473 7221 0000 00da  ist_fieldsr!....
+00002360: 0872 6573 706f 6e73 6529 0972 4400 0000  .response).rD...
+00002370: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
+00002380: 4800 0000 72bf 0000 0072 4a00 0000 da08  H...r....rJ.....
+00002390: 696e 7374 616e 6365 7249 0000 0072 3600  instancerI...r6.
+000023a0: 0000 7236 0000 0072 3700 0000 724c 0000  ..r6...r7...rL..
+000023b0: 004d 0100 0073 1c00 0000 0a01 0c01 0802  .M...s..........
+000023c0: 0c03 0e01 0c02 0a01 0e01 0403 0801 0c01  ................
+000023d0: 04ff 06ff 0a03 7a0c 5265 7374 6675 6c2e  ......z.Restful.
+000023e0: 706f 7374 6305 0000 0000 0000 0000 0000  postc...........
+000023f0: 000f 0000 0005 0000 0003 0000 0073 6201  .............sb.
+00002400: 0000 7400 7c02 7c03 8302 7d05 7c01 6a01  ..t.|.|...}.|.j.
+00002410: a002 7403 6a04 6401 a102 7d06 7c01 6a01  ..t.j.d...}.|.j.
+00002420: a002 7403 6a05 7403 6a06 a102 7d07 7c01  ..t.j.t.j...}.|.
+00002430: 6a01 a007 7403 6a08 a101 7d08 7c08 7322  j...t.j...}.|.s"
+00002440: 7c04 6701 7d08 7c05 6a09 7c01 7c08 6402  |.g.}.|.j.|.|.d.
+00002450: 8d02 8900 7c04 6401 7500 7251 8800 6a0a  ....|.d.u.rQ..j.
+00002460: 8901 8700 8701 6602 6403 6404 8408 8800  ......f.d.d.....
+00002470: 6a0b 4400 8301 7d09 740c 8800 a00d a100  j.D...}.t.......
+00002480: 7c09 6405 8d02 7d0a 7c0a 6a0e 740f 8800  |.d...}.|.j.t...
+00002490: a010 a100 8301 6406 8d01 0100 7411 7c0a  ......d.....t.|.
+000024a0: 8301 5300 7c06 7259 7c05 a012 7c06 a101  ..S.|.rY|...|...
+000024b0: 7d0b 6e03 7c05 6a13 7d0b 8800 6a0a 7d0c  }.n.|.j.}...j.}.
+000024c0: 7c0b 6a09 7c01 7c08 6402 8d02 8900 8800  |.j.|.|.d.......
+000024d0: 6a14 6407 1900 7d0d 7c07 7403 6a06 6b02  j.d...}.|.t.j.k.
+000024e0: 72af 7c04 6408 6b02 7282 8800 a015 a100  r.|.d.k.r.......
+000024f0: 7d0d 8800 a016 7c0c 7c0d a102 7d0e 7411  }.....|.|...}.t.
+00002500: 7c0e 8301 5300 7c04 6409 6b02 7294 8800  |...S.|.d.k.r...
+00002510: a015 a100 7d0d 7417 8800 7c0c 7c0d 8303  ....}.t...|.|...
+00002520: 7d0e 7411 7c0e 8301 5300 7c0d 6401 7500  }.t.|...S.|.d.u.
+00002530: 72a6 740c 640a 7418 7c05 7c04 6602 1600  r.t.d.t.|.|.f...
+00002540: 640b 8d02 7d0e 7411 7c0e 8301 5300 8800  d...}.t.|...S...
+00002550: a019 7c0d a101 7d0e 7411 7c0e 8301 5300  ..|...}.t.|...S.
+00002560: 6401 5300 290c 7a3b 0a20 2020 2020 2020  d.S.).z;.       
+00002570: 2057 6f72 6b73 2c20 6275 7420 6973 2075   Works, but is u
+00002580: 676c 7920 746f 2067 6574 206c 6973 7420  gly to get list 
+00002590: 616e 6420 6465 7461 696c 0a20 2020 2020  and detail.     
+000025a0: 2020 204e 2902 7245 0000 00da 0c73 656c     N).rE.....sel
+000025b0: 6563 7465 645f 706b 7363 0100 0000 0000  ected_pksc......
+000025c0: 0000 0000 0000 0200 0000 0700 0000 1300  ................
+000025d0: 0000 7320 0000 0067 007c 005d 0c7d 0188  ..s ...g.|.].}..
+000025e0: 016a 00a0 0188 007c 0188 016a 006a 02a1  .j.....|...j.j..
+000025f0: 0391 0271 0253 0072 3600 0000 2903 7260  ...q.S.r6...).r`
+00002600: 0000 0072 6700 0000 da0a 616c 6c5f 6669  ...rg.....all_fi
+00002610: 656c 6473 726d 0000 00a9 0272 4a00 0000  eldsrm.....rJ...
+00002620: 726b 0000 0072 3600 0000 7237 0000 0072  rk...r6...r7...r
+00002630: 6f00 0000 7601 0000 7308 0000 0006 0002  o...v...s.......
+00002640: 0212 ff06 ff7a 1f52 6573 7466 756c 2e67  .....z.Restful.g
+00002650: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  et.<locals>.<lis
+00002660: 7463 6f6d 703e 2902 7271 0000 0072 7200  tcomp>).rq...rr.
+00002670: 0000 2901 7276 0000 0072 0100 0000 7a06  ..).rv...r....z.
+00002680: 2d39 3939 3939 723b 0000 0046 2902 7274  -99999r;...F).rt
+00002690: 0000 00da 076d 6573 7361 6765 291a 721f  .....message).r.
+000026a0: 0000 0072 7800 0000 727c 0000 0072 1b00  ...rx...r|...r..
+000026b0: 0000 7281 0000 0072 7d00 0000 7282 0000  ..r....r}...r...
+000026c0: 00da 0767 6574 6c69 7374 da12 5552 4c5f  ...getlist..URL_
+000026d0: 5041 5241 4d5f 5345 4c45 4354 4544 7245  PARAM_SELECTEDrE
+000026e0: 0000 0072 7b00 0000 7286 0000 0072 9000  ...r{...r....r..
+000026f0: 0000 728c 0000 0072 9500 0000 72aa 0000  ..r....r....r...
+00002700: 0072 9100 0000 7221 0000 0072 cc00 0000  .r....r!...r....
+00002710: da0d 6465 7461 696c 5f61 6374 696f 6e72  ..detail_actionr
+00002720: 4100 0000 7240 0000 00da 0f65 6c65 6d32  A...r@.....elem2
+00002730: 7265 635f 696e 7365 7274 722d 0000 00da  rec_insertr-....
+00002740: 094e 4f54 5f46 4f55 4e44 da11 656c 656d  .NOT_FOUND..elem
+00002750: 3272 6563 5f64 6574 6169 6c65 6429 0f72  2rec_detailed).r
+00002760: 4400 0000 7245 0000 0072 4600 0000 7247  D...rE...rF...rG
+00002770: 0000 0072 4800 0000 72bf 0000 0072 9c00  ...rH...r....r..
+00002780: 0000 729b 0000 00da 0273 7272 7200 0000  ..r......srrr...
+00002790: 72a2 0000 0072 cf00 0000 727b 0000 0072  r....r....r{...r
+000027a0: 4b00 0000 729d 0000 0072 3600 0000 72dc  K...r....r6...r.
+000027b0: 0000 0072 3700 0000 727c 0000 0067 0100  ...r7...r|...g..
+000027c0: 0073 5000 0000 0a04 1002 0601 0801 04ff  .sP.............
+000027d0: 0e02 0401 0601 0e01 0801 0601 0c01 0402  ................
+000027e0: 06fe 1003 1401 0801 0403 0c01 0602 0601  ................
+000027f0: 0e01 0a01 0a01 0801 0801 0c01 0809 08f8  ................
+00002800: 0801 0c01 0806 08fb 0201 0c01 06ff 0804  ................
+00002810: 0aff 0801 04f4 7a0b 5265 7374 6675 6c2e  ......z.Restful.
+00002820: 6765 7463 0500 0000 0000 0000 0000 0000  getc............
+00002830: 0b00 0000 0600 0000 4300 0000 73a8 0000  ........C...s...
+00002840: 0074 007c 027c 0383 027d 057c 056a 017c  .t.|.|...}.|.j.|
+00002850: 0164 018d 017d 067c 06a0 027c 04a1 0101  .d...}.|...|....
+00002860: 007c 066a 0364 0219 007d 077c 066a 047d  .|.j.d...}.|.j.}
+00002870: 0874 05a0 067c 016a 07a1 01a0 0864 03a1  .t...|.j.....d..
+00002880: 017d 0974 09a0 0a7c 09a1 017d 097c 05a0  .}.t...|...}.|..
+00002890: 0b7c 056a 0ca1 017d 0a7c 056a 017c 017c  .|.j...}.|.j.|.|
+000028a0: 0a64 048d 027d 0674 0d6a 0e6a 0f6a 107c  .d...}.t.j.j.j.|
+000028b0: 065f 117c 06a0 127c 097c 0764 05a1 0301  ._.|...|.|.d....
+000028c0: 007c 066a 137c 086a 14a0 157c 067c 077c  .|.j.|.j...|.|.|
+000028d0: 086a 146a 16a1 0367 0164 068d 0101 0074  .j.j...g.d.....t
+000028e0: 177c 066a 1883 0153 0029 074e 72b5 0000  .|.j...S.).Nr...
+000028f0: 0072 0100 0000 7272 0000 0029 0272 4500  .r....rr...).rE.
+00002900: 0000 727f 0000 0046 72d1 0000 0029 1972  ..r....Fr....).r
+00002910: 1f00 0000 7245 0000 0072 4200 0000 7241  ....rE...rB...rA
+00002920: 0000 0072 7b00 0000 7209 0000 0072 5000  ...r{...r....rP.
+00002930: 0000 7251 0000 0072 7c00 0000 72d3 0000  ..rQ...r|...r...
+00002940: 0072 d400 0000 72cc 0000 00da 1864 6566  .r....r......def
+00002950: 6175 6c74 5f6c 6973 745f 6163 7469 6f6e  ault_list_action
+00002960: 5f6e 616d 6572 0b00 0000 723d 0000 0072  _namer....r=...r
+00002970: 2600 0000 da0e 6578 746a 735f 7265 6e64  &.....extjs_rend
+00002980: 6572 6572 723a 0000 0072 d500 0000 72d6  ererr:...r....r.
+00002990: 0000 0072 6000 0000 7267 0000 0072 d700  ...r`...rg...r..
+000029a0: 0000 7221 0000 0072 d800 0000 290b 7244  ..r!...r....).rD
+000029b0: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
+000029c0: 0000 7248 0000 0072 bf00 0000 724a 0000  ..rH...r....rJ..
+000029d0: 0072 4b00 0000 726b 0000 0072 4900 0000  .rK...rk...rI...
+000029e0: da01 6172 3600 0000 7236 0000 0072 3700  ..ar6...r6...r7.
+000029f0: 0000 7253 0000 0093 0100 0073 1e00 0000  ..rS.......s....
+00002a00: 0a01 0c01 0a01 0a01 0601 1202 0a01 0c01  ................
+00002a10: 0e01 0c01 0e01 0402 1401 06ff 0a02 7a0b  ..............z.
+00002a20: 5265 7374 6675 6c2e 7075 7472 5500 0000  Restful.putrU...
+00002a30: 2907 7256 0000 0072 5700 0000 7258 0000  ).rV...rW...rX..
+00002a40: 0072 b100 0000 724c 0000 0072 7c00 0000  .r....rL...r|...
+00002a50: 7253 0000 0072 3600 0000 7236 0000 0072  rS...r6...r6...r
+00002a60: 3600 0000 7237 0000 0072 d000 0000 4801  6...r7...r....H.
+00002a70: 0000 730a 0000 0008 0004 010a 040a 1a0e  ..s.............
+00002a80: 2c72 d000 0000 6303 0000 0000 0000 0000  ,r....c.........
+00002a90: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
+00002aa0: 7000 0000 7c00 a000 a100 7d03 7401 8300  p...|.....}.t...
+00002ab0: 7d04 7c03 6a02 7c04 6602 7d05 7c00 6a03  }.|.j.|.f.}.|.j.
+00002ac0: 6406 6900 7c02 a401 8e01 7d02 7c00 7c02  d.i.|.....}.|.|.
+00002ad0: 6401 3c00 7c00 6a04 7c02 6402 3c00 7405  d.<.|.j.|.d.<.t.
+00002ae0: 6a06 6a07 6a08 6a09 6a0a 7d06 7c06 a00b  j.j.j.j.j.}.|...
+00002af0: 7c01 a101 7d07 740c 6a0d 7c07 6a0e 6406  |...}.t.j.|.j.d.
+00002b00: 6900 7c02 a401 8e01 6403 6404 8d02 7d08  i.|.....d.d...}.
+00002b10: 7c08 5300 2907 7a14 4465 7365 7276 6573  |.S.).z.Deserves
+00002b20: 2061 2064 6f63 7374 7269 6e67 724a 0000   a docstringrJ..
+00002b30: 00da 046d 656d 6ffa 1974 6578 742f 6874  ...memo..text/ht
+00002b40: 6d6c 3b63 6861 7273 6574 3d22 7574 662d  ml;charset="utf-
+00002b50: 3822 a901 da0c 636f 6e74 656e 745f 7479  8"....content_ty
+00002b60: 7065 4e72 3600 0000 290f da08 6765 745f  peNr6...)...get_
+00002b70: 7573 6572 7211 0000 00da 0975 7365 725f  userr......user_
+00002b80: 7479 7065 da15 6765 745f 7072 696e 7461  type..get_printa
+00002b90: 626c 655f 636f 6e74 6578 74da 0a70 6172  ble_context..par
+00002ba0: 7365 5f6d 656d 6f72 0b00 0000 723d 0000  se_memor....r=..
+00002bb0: 0072 3e00 0000 da05 6a69 6e6a 6172 3a00  .r>.....jinjar:.
+00002bc0: 0000 da09 6a69 6e6a 615f 656e 76da 0c67  ....jinja_env..g
+00002bd0: 6574 5f74 656d 706c 6174 6572 0900 0000  et_templater....
+00002be0: da0c 4874 7470 5265 7370 6f6e 7365 da06  ..HttpResponse..
+00002bf0: 7265 6e64 6572 2909 724a 0000 00da 0774  render).rJ.....t
+00002c00: 706c 6e61 6d65 da07 636f 6e74 6578 74da  plname..context.
+00002c10: 0175 da04 6c61 6e67 da01 6bda 0365 6e76  .u..lang..k..env
+00002c20: da08 7465 6d70 6c61 7465 72d8 0000 0072  ..templater....r
+00002c30: 3600 0000 7236 0000 0072 3700 0000 da0d  6...r6...r7.....
+00002c40: 6874 7470 5f72 6573 706f 6e73 65a6 0100  http_response...
+00002c50: 0073 1a00 0000 0802 0601 0a01 1001 0801  .s..............
+00002c60: 0a01 0e01 0a01 0402 0e01 0201 06fe 0404  ................
+00002c70: 72fc 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00002c80: 0000 0c00 0000 0a00 0000 4300 0000 73ea  ..........C...s.
+00002c90: 0000 007c 006a 0064 1469 007c 02a4 018e  ...|.j.d.i.|....
+00002ca0: 017d 027c 026a 0174 0264 018d 0101 0074  .}.|.j.t.d.....t
+00002cb0: 036a 046a 056a 066a 076a 087d 037a 077c  .j.j.j.j.j.}.z.|
+00002cc0: 03a0 097c 01a1 017d 0457 006e 1604 0074  ...|...}.W.n...t
+00002cd0: 0a79 3201 007d 0501 007a 0a74 0ba0 0ca1  .y2..}...z.t....
+00002ce0: 0057 0006 0059 0064 027d 057e 0553 0064  .W...Y.d.}.~.S.d
+00002cf0: 027d 057e 0577 0177 0064 0364 0484 007d  .}.~.w.w.d.d...}
+00002d00: 067c 026a 017c 0664 058d 0101 0064 0664  .|.j.|.d.....d.d
+00002d10: 0784 007d 0764 0864 0984 007d 0864 0a64  ...}.d.d...}.d.d
+00002d20: 0b84 007d 097c 036a 0da0 0174 0e7c 077c  ...}.|.j...t.|.|
+00002d30: 087c 0964 0c8d 03a1 0101 007c 01a0 0f64  .|.d.......|...d
+00002d40: 0da1 0172 5b64 0e6e 087c 01a0 0f64 0fa1  ...r[d.n.|...d..
+00002d50: 0172 6264 106e 0164 117d 0a74 0b6a 107c  .rbd.n.d.}.t.j.|
+00002d60: 046a 1164 1469 007c 02a4 018e 017c 0a64  .j.d.i.|.....|.d
+00002d70: 1217 0064 138d 027d 0b7c 0b53 0029 157a  ...d...}.|.S.).z
+00002d80: 6a0a 2020 2020 5265 7370 6f6e 6520 7573  j.    Respone us
+00002d90: 6564 2066 6f72 2072 656e 6465 7269 6e67  ed for rendering
+00002da0: 2058 4d4c 2076 6965 7773 2069 6e20 7265   XML views in re
+00002db0: 6163 742e 0a20 2020 2049 6e63 6c75 6465  act..    Include
+00002dc0: 7320 736f 6d65 2068 656c 7065 7220 6675  s some helper fu
+00002dd0: 6e63 7469 6f6e 7320 666f 7220 7265 6e64  nctions for rend
+00002de0: 6572 696e 672e 0a20 2020 2072 1a00 0000  ering..    r....
+00002df0: 4e63 0000 0000 0000 0000 0000 0000 0100  Nc..............
+00002e00: 0000 0400 0000 5700 0000 7320 0000 0064  ......W...s ...d
+00002e10: 0164 0284 007c 0044 0083 017d 0064 0364  .d...|.D...}.d.d
+00002e20: 04a0 007c 00a1 0117 0064 0517 0053 0029  ...|.....d...S.)
+00002e30: 067a 2748 656c 7065 7220 6675 6e63 7469  .z'Helper functi
+00002e40: 6f6e 2074 6f20 7772 6170 2061 2073 7472  on to wrap a str
+00002e50: 696e 6720 696e 207b 7d73 6301 0000 0000  ing in {}sc.....
+00002e60: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00002e70: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
+00002e80: 7400 7c01 8301 9102 7102 5300 7236 0000  t.|.....q.S.r6..
+00002e90: 0029 0172 aa00 0000 2902 726e 0000 0072  .).r....).rn...r
+00002ea0: e700 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00002eb0: 0000 0072 6f00 0000 cd01 0000 7302 0000  ...ro.......s...
+00002ec0: 0014 007a 2e58 4d4c 5f72 6573 706f 6e73  ...z.XML_respons
+00002ed0: 652e 3c6c 6f63 616c 733e 2e62 696e 642e  e.<locals>.bind.
+00002ee0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00002ef0: 6d70 3eda 017b 725c 0000 00da 017d 2901  mp>..{r\.....}).
+00002f00: da04 6a6f 696e a901 da04 6172 6773 7236  ..join....argsr6
+00002f10: 0000 0072 3600 0000 7237 0000 00da 0462  ...r6...r7.....b
+00002f20: 696e 64cb 0100 0073 0400 0000 0e02 1201  ind....s........
+00002f30: 7a1a 584d 4c5f 7265 7370 6f6e 7365 2e3c  z.XML_response.<
+00002f40: 6c6f 6361 6c73 3e2e 6269 6e64 2901 7202  locals>.bind).r.
+00002f50: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002f60: 0100 0000 0200 0000 5700 0000 730c 0000  ........W...s...
+00002f70: 0074 007c 0083 0101 0064 0153 0029 027a  .t.|.....d.S.).z
+00002f80: 8844 6562 7567 6765 7220 6865 6c70 6572  .Debugger helper
+00002f90: 3b20 7072 696e 7473 206f 7574 2061 6c6c  ; prints out all
+00002fa0: 2061 7267 7320 7075 7420 696e 746f 2074   args put into t
+00002fb0: 6865 2066 696c 7465 7220 6275 7420 646f  he filter but do
+00002fc0: 6573 6e27 7420 696e 636c 7564 6520 7468  esn't include th
+00002fd0: 656d 2069 6e20 7468 6520 7465 6d70 6c61  em in the templa
+00002fe0: 7465 2e0a 2020 2020 2020 2020 7573 6167  te..        usag
+00002ff0: 653a 207b 7b64 6562 7567 207c 2070 7d7d  e: {{debug | p}}
+00003000: 0a20 2020 2020 2020 2072 5c00 0000 2901  .        r\...).
+00003010: da05 7072 696e 7472 0001 0000 7236 0000  ..printr....r6..
+00003020: 0072 3600 0000 7237 0000 00da 0170 d201  .r6...r7.....p..
+00003030: 0000 7304 0000 0008 0404 017a 1758 4d4c  ..s........z.XML
+00003040: 5f72 6573 706f 6e73 652e 3c6c 6f63 616c  _response.<local
+00003050: 733e 2e70 6301 0000 0000 0000 0000 0000  s>.pc...........
+00003060: 0003 0000 0004 0000 0053 0000 0073 2000  .........S...s .
+00003070: 0000 6401 6402 6c00 7d01 7c01 a001 7402  ..d.d.l.}.|...t.
+00003080: 7c00 8301 a101 7d02 7c02 a003 6403 a101  |.....}.|...d...
+00003090: 5300 2904 7ab0 0a20 2020 2020 2020 2043  S.).z..        C
+000030a0: 6f6d 7072 6573 7320 6120 636f 6d70 6c65  ompress a comple
+000030b0: 7820 7661 6c75 6520 696e 206f 7264 6572  x value in order
+000030c0: 2074 6f20 6765 7420 6465 636f 6d70 7265   to get decompre
+000030d0: 7373 2062 7920 7468 6520 636f 6e74 726f  ss by the contro
+000030e0: 6c6c 6572 2061 6674 6572 7761 7264 730a  ller afterwards.
+000030f0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+00003100: 3a20 7661 6c75 6520 746f 2067 6574 2063  : value to get c
+00003110: 6f6d 7072 6573 7365 642e 0a20 2020 2020  ompressed..     
+00003120: 2020 203a 7265 7475 726e 3a20 436f 6d70     :return: Comp
+00003130: 7265 7373 6564 2076 616c 7565 2e0a 2020  ressed value..  
+00003140: 2020 2020 2020 7201 0000 004e da06 6261        r....N..ba
+00003150: 7365 3634 2904 da04 7a6c 6962 da08 636f  se64)...zlib..co
+00003160: 6d70 7265 7373 72aa 0000 00da 0665 6e63  mpressr......enc
+00003170: 6f64 6529 03da 0173 7206 0100 00da 0a63  ode)...sr......c
+00003180: 6f6d 7072 6573 7365 6472 3600 0000 7236  ompressedr6...r6
+00003190: 0000 0072 3700 0000 da0d 7a6c 6962 5f63  ...r7.....zlib_c
+000031a0: 6f6d 7072 6573 73d9 0100 0073 0600 0000  ompress....s....
+000031b0: 0806 0e01 0a01 7a23 584d 4c5f 7265 7370  ......z#XML_resp
+000031c0: 6f6e 7365 2e3c 6c6f 6361 6c73 3e2e 7a6c  onse.<locals>.zl
+000031d0: 6962 5f63 6f6d 7072 6573 7363 0200 0000  ib_compressc....
+000031e0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000031f0: 5300 0000 7320 0000 007c 0072 0e7c 0144  S...s ...|.r.|.D
+00003200: 005d 097d 027c 007c 026b 0272 0d01 0064  .].}.|.|.k.r...d
+00003210: 0153 0071 0464 0253 0029 037a f60a 2020  .S.q.d.S.).z..  
+00003220: 2020 2020 2020 6368 6563 6b20 6966 2074        check if t
+00003230: 6865 2066 6965 6c64 7320 6973 2061 7661  he fields is ava
+00003240: 696c 6162 6c65 2069 6e20 7468 6520 7365  ilable in the se
+00003250: 7420 6f66 2063 6f6c 6c65 6374 696f 6e73  t of collections
+00003260: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003270: 7365 6172 6368 6564 5f66 6965 6c64 3a20  searched_field: 
+00003280: 7365 6172 6368 6564 2066 6965 6c64 0a20  searched field. 
+00003290: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+000032a0: 6c6c 6563 7469 6f6e 733a 2073 6574 206f  llections: set o
+000032b0: 6620 6669 656c 6473 0a20 2020 2020 2020  f fields.       
+000032c0: 203a 7265 7475 726e 3a20 5472 7565 2069   :return: True i
+000032d0: 6620 7468 6520 6669 656c 6420 6973 2070  f the field is p
+000032e0: 7265 7365 6e74 2069 6e20 7468 6520 636f  resent in the co
+000032f0: 6c6c 6563 7469 6f6e 732c 4661 6c73 6520  llections,False 
+00003300: 6f74 6865 7277 6973 652e 0a20 2020 2020  otherwise..     
+00003310: 2020 2054 4672 3600 0000 2903 da0e 7365     TFr6...)...se
+00003320: 6172 6368 6564 5f66 6965 6c64 da0b 636f  arched_field..co
+00003330: 6c6c 6563 7469 6f6e 7372 ba00 0000 7236  llectionsr....r6
+00003340: 0000 0072 3600 0000 7237 0000 00da 0d66  ...r6...r7.....f
+00003350: 6965 6c64 735f 7365 6172 6368 e401 0000  ields_search....
+00003360: 730c 0000 0004 0708 0108 0106 0102 ff04  s...............
+00003370: 027a 2358 4d4c 5f72 6573 706f 6e73 652e  .z#XML_response.
+00003380: 3c6c 6f63 616c 733e 2e66 6965 6c64 735f  <locals>.fields_
+00003390: 7365 6172 6368 2903 7204 0100 0072 0b01  search).r....r..
+000033a0: 0000 720e 0100 007a 042e 786d 6c7a 0874  ..r....z..xmlz.t
+000033b0: 6578 742f 786d 6c7a 032e 6a73 fa16 6170  ext/xmlz..js..ap
+000033c0: 706c 6963 6174 696f 6e2f 6a61 7661 7363  plication/javasc
+000033d0: 7269 7074 7a10 6170 706c 6963 6174 696f  riptz.applicatio
+000033e0: 6e2f 6a73 6f6e 7a10 3b63 6861 7273 6574  n/jsonz.;charset
+000033f0: 3d22 7574 662d 3822 72ea 0000 0072 3600  ="utf-8"r....r6.
+00003400: 0000 2912 72ee 0000 0072 9500 0000 721b  ..).r....r....r.
+00003410: 0000 0072 0b00 0000 723d 0000 0072 3e00  ...r....r=...r>.
+00003420: 0000 72f0 0000 0072 3a00 0000 72f1 0000  ..r....r:...r...
+00003430: 0072 f200 0000 7204 0000 0072 0900 0000  .r....r....r....
+00003440: da14 4874 7470 5265 7370 6f6e 7365 4e6f  ..HttpResponseNo
+00003450: 7446 6f75 6e64 da07 6669 6c74 6572 7372  tFound..filtersr
+00003460: 9000 0000 da08 656e 6473 7769 7468 72f3  ......endswithr.
+00003470: 0000 0072 f400 0000 290c 724a 0000 0072  ...r....).rJ...r
+00003480: f500 0000 72f6 0000 0072 fa00 0000 72fb  ....r....r....r.
+00003490: 0000 00da 0165 7202 0100 0072 0401 0000  .....er....r....
+000034a0: 720b 0100 0072 0e01 0000 72eb 0000 0072  r....r....r....r
+000034b0: d800 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+000034c0: 0000 00da 0c58 4d4c 5f72 6573 706f 6e73  .....XML_respons
+000034d0: 65b9 0100 0073 3000 0000 1008 0c01 0e03  e....s0.........
+000034e0: 0201 0e01 0e01 1401 0880 02ff 0803 0c05  ................
+000034f0: 0802 0807 080b 160d 0e01 0e01 0201 02fe  ................
+00003500: 0403 0e01 0601 06fe 0404 7214 0100 0063  ..........r....c
+00003510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003520: 0100 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
+00003530: 0164 005a 0264 015a 0364 025a 0464 0353  .d.Z.d.Z.d.Z.d.S
+00003540: 0029 04da 0653 5756 6965 777a 1772 6561  .)...SWViewz.rea
+00003550: 6374 2f73 6572 7669 6365 2d77 6f72 6b65  ct/service-worke
+00003560: 722e 6a73 720f 0100 004e 2905 7256 0000  r.jsr....N).rV..
+00003570: 0072 5700 0000 7258 0000 00da 0d74 656d  .rW...rX.....tem
+00003580: 706c 6174 655f 6e61 6d65 72eb 0000 0072  plate_namer....r
+00003590: 3600 0000 7236 0000 0072 3600 0000 7237  6...r6...r6...r7
+000035a0: 0000 0072 1501 0000 fc01 0000 7306 0000  ...r........s...
+000035b0: 0008 0004 0108 0172 1501 0000 6300 0000  .......r....c...
+000035c0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000035d0: 0000 0000 0073 2000 0000 6500 5a01 6400  .....s ...e.Z.d.
+000035e0: 5a02 6401 5a03 8700 6601 6402 6403 8408  Z.d.Z...f.d.d...
+000035f0: 5a04 8700 0400 5a05 5300 2904 da06 5742  Z.....Z.S.)...WB
+00003600: 5669 6577 720f 0100 0063 0200 0000 0000  Viewr....c......
+00003610: 0000 0000 0000 0400 0000 0400 0000 0f00  ................
+00003620: 0000 732c 0000 0074 0083 006a 017c 0167  ..s,...t...j.|.g
+00003630: 017c 02a2 0152 0069 007c 03a4 018e 0101  .|...R.i.|......
+00003640: 0064 017c 0364 0219 0017 007c 005f 0264  .d.|.d.....|._.d
+00003650: 0053 0029 034e 7a06 7265 6163 742f da07  .S.).Nz.react/..
+00003660: 776f 726b 626f 7829 03da 0573 7570 6572  workbox)...super
+00003670: da05 7365 7475 7072 1601 0000 2904 7244  ..setupr....).rD
+00003680: 0000 0072 4500 0000 7201 0100 00da 066b  ...rE...r......k
+00003690: 7761 7267 73a9 01da 095f 5f63 6c61 7373  wargs....__class
+000036a0: 5f5f 7236 0000 0072 3700 0000 721a 0100  __r6...r7...r...
+000036b0: 0003 0200 0073 0400 0000 1a01 1201 7a0c  .....s........z.
+000036c0: 5742 5669 6577 2e73 6574 7570 2906 7256  WBView.setup).rV
+000036d0: 0000 0072 5700 0000 7258 0000 0072 eb00  ...rW...rX...r..
+000036e0: 0000 721a 0100 00da 0d5f 5f63 6c61 7373  ..r......__class
+000036f0: 6365 6c6c 5f5f 7236 0000 0072 3600 0000  cell__r6...r6...
+00003700: 721c 0100 0072 3700 0000 7217 0100 0000  r....r7...r.....
+00003710: 0200 0073 0600 0000 0800 0401 1402 7217  ...s..........r.
+00003720: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00003730: 0000 0000 0200 0000 4000 0000 f314 0000  ........@.......
+00003740: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00003750: 0364 0353 0029 04da 084d 6169 6e48 746d  .d.S.)...MainHtm
+00003760: 6c63 0200 0000 0000 0000 0000 0000 0700  lc..............
+00003770: 0000 0400 0000 4f00 0000 7358 0000 0074  ......O...sX...t
+00003780: 006a 01a0 02a1 0001 0074 006a 016a 036a  .j.......t.j.j.j
+00003790: 046a 057d 0474 067c 017c 0464 018d 027d  .j.}.t.|.|.d...}
+000037a0: 0564 027c 015f 0774 006a 01a0 087c 05a1  .d.|._.t.j...|..
+000037b0: 017d 067c 04a0 097c 06a1 017d 067c 056a  .}.|...|...}.|.j
+000037c0: 0a7c 0664 038d 0101 0074 0b7c 056a 0c7c  .|.d.....t.|.j.|
+000037d0: 056a 0d83 0253 0029 047a 3252 6574 7572  .j...S.).z2Retur
+000037e0: 6e73 2061 206a 736f 6e20 7374 7275 6374  ns a json struct
+000037f0: 2066 6f72 2074 6865 206d 6169 6e20 7573   for the main us
+00003800: 6572 2064 6173 6862 6f61 7264 2e72 3900  er dashboard.r9.
+00003810: 0000 7a0e 6461 7368 626f 6172 642d 6d61  ..z.dashboard-ma
+00003820: 696e 7207 0000 0029 0e72 0b00 0000 723d  inr....).r....r=
+00003830: 0000 00da 0773 7461 7274 7570 723e 0000  .....startupr>..
+00003840: 0072 3f00 0000 723a 0000 0072 1c00 0000  .r?...r:...r....
+00003850: da10 7265 7175 6573 7469 6e67 5f70 616e  ..requesting_pan
+00003860: 656c da0d 6765 745f 6d61 696e 5f68 746d  el..get_main_htm
+00003870: 6c72 7300 0000 7274 0000 0072 2100 0000  lrs...rt...r!...
+00003880: 72d8 0000 0072 eb00 0000 2907 7244 0000  r....r....).rD..
+00003890: 0072 4500 0000 7201 0100 0072 a200 0000  .rE...r....r....
+000038a0: da03 726e 6472 4a00 0000 7208 0000 0072  ..rndrJ...r....r
+000038b0: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
+000038c0: 0000 0009 0200 0073 1000 0000 0a03 0c02  .......s........
+000038d0: 0c01 0602 0c01 0a01 0c01 0e01 7a0c 4d61  ............z.Ma
+000038e0: 696e 4874 6d6c 2e67 6574 4e72 c200 0000  inHtml.getNr....
+000038f0: 7236 0000 0072 3600 0000 7236 0000 0072  r6...r6...r6...r
+00003900: 3700 0000 7220 0100 0008 0200 00f3 0400  7...r ..........
+00003910: 0000 0800 0c01 7220 0100 0063 0000 0000  ......r ...c....
+00003920: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00003930: 4000 0000 721f 0100 0029 04da 0d44 6173  @...r....)...Das
+00003940: 6862 6f61 7264 4974 656d 6303 0000 0000  hboardItemc.....
+00003950: 0000 0000 0000 000a 0000 0005 0000 004f  ...............O
+00003960: 0000 0073 9800 0000 7400 7c01 8301 7d05  ...s....t.|...}.
+00003970: 7401 6a02 6a03 6a04 6a05 7c05 5f05 6401  t.j.j.j.j.|._.d.
+00003980: 7c02 9b00 9d02 7c05 5f06 7c05 a007 a100  |.....|._.|.....
+00003990: a008 a100 6a09 7d06 740a 7c06 8301 7c02  ....j.}.t.|...|.
+000039a0: 6b04 722b 7c06 7c02 1900 7d07 6402 a00b  k.r+|.|...}.d...
+000039b0: 7c07 a00c 7c05 a101 a101 7d08 6e02 6402  |...|.....}.n.d.
+000039c0: 7d08 740d 7c08 6403 8d01 7d04 740e 7c01  }.t.|.d...}.t.|.
+000039d0: 8301 7d09 7c09 723d 7c04 a00f 7c09 a101  ..}.|.r=|...|...
+000039e0: 0100 7c05 6a10 6405 6900 7c04 a401 8e01  ..|.j.d.i.|.....
+000039f0: 0100 7411 7c05 6a12 7c05 6a13 8302 5300  ..t.|.j.|.j...S.
+00003a00: 2906 7a3d 5265 7475 726e 7320 6120 7265  ).z=Returns a re
+00003a10: 6e64 6572 6564 2048 544d 4c20 7665 7273  ndered HTML vers
+00003a20: 696f 6e20 7468 6520 7265 7175 6573 7465  ion the requeste
+00003a30: 6420 7573 6572 2064 6173 6862 6f61 7264  d user dashboard
+00003a40: 2e7a 0a64 6173 6862 6f61 7264 2d72 5c00  .z.dashboard-r\.
+00003a50: 0000 7207 0000 004e 7236 0000 0029 1472  ..r....Nr6...).r
+00003a60: 1c00 0000 720b 0000 0072 3d00 0000 723e  ....r....r=...r>
+00003a70: 0000 0072 3f00 0000 723a 0000 0072 2201  ...r?...r:...r".
+00003a80: 0000 72ec 0000 00da 0f67 6574 5f70 7265  ..r......get_pre
+00003a90: 6665 7265 6e63 6573 da0f 6461 7368 626f  ferences..dashbo
+00003aa0: 6172 645f 6974 656d 7372 8f00 0000 72ff  ard_itemsr....r.
+00003ab0: 0000 0072 f400 0000 7290 0000 0072 2c00  ...r....r....r,.
+00003ac0: 0000 7295 0000 0072 7400 0000 7221 0000  ..r....rt...r!..
+00003ad0: 0072 d800 0000 72eb 0000 0029 0a72 4400  .r....r....).rD.
+00003ae0: 0000 7245 0000 00da 0569 6e64 6578 7201  ..rE.....indexr.
+00003af0: 0100 0072 a200 0000 724a 0000 00da 0464  ...r....rJ.....d
+00003b00: 6173 68da 0469 7465 6d72 0800 0000 7299  ash..itemr....r.
+00003b10: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003b20: 0000 727c 0000 0019 0200 0073 1c00 0000  ..r|.......s....
+00003b30: 0802 0e01 0c01 0e01 0c01 0801 1203 0402  ................
+00003b40: 0a01 0801 0401 0a01 1001 0e01 7a11 4461  ............z.Da
+00003b50: 7368 626f 6172 6449 7465 6d2e 6765 744e  shboardItem.getN
+00003b60: 72c2 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00003b70: 3600 0000 7237 0000 0072 2601 0000 1802  6...r7...r&.....
+00003b80: 0000 7225 0100 0072 2601 0000 6300 0000  ..r%...r&...c...
+00003b90: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00003ba0: 0040 0000 0073 2000 0000 6500 5a01 6400  .@...s ...e.Z.d.
+00003bb0: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
+00003bc0: 6405 8400 5a05 6406 5300 2907 da04 4e75  d...Z.d.S.)...Nu
+00003bd0: 6c6c 7a6c 4a75 7374 2072 6574 7572 6e73  llzlJust returns
+00003be0: 2032 3030 2c20 7573 6564 2069 6e20 616e   200, used in an
+00003bf0: 2069 6672 616d 6520 746f 2063 6175 7365   iframe to cause
+00003c00: 2074 6865 2062 726f 7773 6572 2074 6f20   the browser to 
+00003c10: 7472 6967 6765 7220 2244 6f20 796f 7520  trigger "Do you 
+00003c20: 7761 6e74 2074 6f20 7265 6d65 6d62 6572  want to remember
+00003c30: 2074 6869 7320 7077 2220 6469 616c 6f67   this pw" dialog
+00003c40: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00003c50: 0002 0000 0043 0000 00f3 0800 0000 7400  .....C........t.
+00003c60: a001 a100 5300 72b6 0000 00a9 0272 0900  ....S.r......r..
+00003c70: 0000 72f3 0000 00a9 0272 4400 0000 7245  ..r......rD...rE
+00003c80: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003c90: 0000 724c 0000 0031 0200 00f3 0200 0000  ..rL...1........
+00003ca0: 0801 7a09 4e75 6c6c 2e70 6f73 7463 0200  ..z.Null.postc..
+00003cb0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00003cc0: 0000 4300 0000 722d 0100 0072 b600 0000  ..C...r-...r....
+00003cd0: 722e 0100 0072 2f01 0000 7236 0000 0072  r....r/...r6...r
+00003ce0: 3600 0000 7237 0000 0072 7c00 0000 3402  6...r7...r|...4.
+00003cf0: 0000 7230 0100 007a 084e 756c 6c2e 6765  ..r0...z.Null.ge
+00003d00: 744e 2906 7256 0000 0072 5700 0000 7258  tN).rV...rW...rX
+00003d10: 0000 0072 b100 0000 724c 0000 0072 7c00  ...r....rL...r|.
+00003d20: 0000 7236 0000 0072 3600 0000 7236 0000  ..r6...r6...r6..
+00003d30: 0072 3700 0000 722c 0100 002e 0200 0073  .r7...r,.......s
+00003d40: 0800 0000 0800 0401 0802 0c03 722c 0100  ............r,..
+00003d50: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003d60: 0000 0200 0000 4000 0000 731c 0000 0065  ......@...s....e
+00003d70: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00003d80: 0364 0484 005a 0464 0553 0029 06da 0c41  .d...Z.d.S.)...A
+00003d90: 7574 6865 6e74 6963 6174 6563 0200 0000  uthenticatec....
+00003da0: 0000 0000 0000 0000 0700 0000 0400 0000  ................
+00003db0: 4f00 0000 7336 0000 007c 016a 00a0 0174  O...s6...|.j...t
+00003dc0: 026a 03a1 017d 0409 007c 016a 04a0 0564  .j...}...|.j...d
+00003dd0: 0364 00a1 027d 0574 06a0 077c 01a1 0101  .d...}.t...|....
+00003de0: 0064 047d 0674 08a0 097c 06a1 0153 0029  .d.}.t...|...S.)
+00003df0: 054e 54da 066c 6f67 6f75 74da 0875 7365  .NT..logout..use
+00003e00: 726e 616d 65fa 012f 290b 7278 0000 0072  rname../).rx...r
+00003e10: 7c00 0000 721b 0000 0072 8100 0000 da07  |...r....r......
+00003e20: 7365 7373 696f 6eda 0370 6f70 7213 0000  session..popr...
+00003e30: 0072 3201 0000 7209 0000 00da 1448 7474  .r2...r......Htt
+00003e40: 7052 6573 706f 6e73 6552 6564 6972 6563  pResponseRedirec
+00003e50: 74da 0748 7474 7034 3034 2907 7244 0000  t..Http404).rD..
+00003e60: 0072 4500 0000 7201 0100 0072 a200 0000  .rE...r....r....
+00003e70: 729c 0000 0072 3301 0000 7232 0000 0072  r....r3...r2...r
+00003e80: 3600 0000 7236 0000 0072 3700 0000 727c  6...r6...r7...r|
+00003e90: 0000 0039 0200 0073 0c00 0000 0e01 0201  ...9...s........
+00003ea0: 0e01 0a01 0405 0a01 7a10 4175 7468 656e  ........z.Authen
+00003eb0: 7469 6361 7465 2e67 6574 6302 0000 0000  ticate.getc.....
+00003ec0: 0000 0000 0000 0008 0000 0005 0000 004f  ...............O
+00003ed0: 0000 0073 4c00 0000 7c01 6a00 a001 6401  ...sL...|.j...d.
+00003ee0: a101 7d04 7c01 6a00 a001 6402 a101 7d05  ..}.|.j...d...}.
+00003ef0: 7402 6a03 7c01 7c04 7c05 6403 8d03 7d06  t.j.|.|.|.d...}.
+00003f00: 7402 6a04 7c01 7c06 6404 6405 8d03 0100  t.j.|.|.d.d.....
+00003f10: 6406 6407 8400 7d07 7405 7c06 6a06 7c07  d.d...}.t.|.j.|.
+00003f20: 8302 5300 2908 7a46 6c6f 6773 2074 6865  ..S.).zFlogs the
+00003f30: 2075 7365 7220 696e 2061 6e64 2062 7569   user in and bui
+00003f40: 6c64 7320 7468 6520 6c69 6e6f 7765 622e  lds the linoweb.
+00003f50: 6a73 2066 696c 6520 666f 7220 7468 6520  js file for the 
+00003f60: 6c6f 6767 6564 2069 6e20 7573 6572 7233  logged in userr3
+00003f70: 0100 00da 0870 6173 7377 6f72 6429 0272  .....password).r
+00003f80: 3301 0000 7239 0100 007a 246c 696e 6f2e  3...r9...z$lino.
+00003f90: 636f 7265 2e61 7574 682e 6261 636b 656e  core.auth.backen
+00003fa0: 6473 2e4d 6f64 656c 4261 636b 656e 6429  ds.ModelBackend)
+00003fb0: 01da 0762 6163 6b65 6e64 6300 0000 0000  ...backendc.....
+00003fc0: 0000 0000 0000 0000 0000 0003 0000 0053  ...............S
+00003fd0: 0000 0073 2600 0000 7400 6a01 6a02 720d  ...s&...t.j.j.r.
+00003fe0: 7400 6a01 6a03 6a04 6a05 a006 6401 a101  t.j.j.j.j...d...
+00003ff0: 0100 7407 6402 6403 6901 8301 5300 2904  ..t.d.d.i...S.).
+00004000: 4e46 7274 0000 0054 2908 720b 0000 0072  NFrt...T).r....r
+00004010: 3d00 0000 da14 6465 7665 6c6f 7065 725f  =.....developer_
+00004020: 7369 7465 5f63 6163 6865 723e 0000 0072  site_cacher>...r
+00004030: 3f00 0000 723a 0000 00da 0e62 7569 6c64  ?...r:.....build
+00004040: 5f6a 735f 6361 6368 6572 2100 0000 7236  _js_cacher!...r6
+00004050: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00004060: 0000 da06 7265 7375 6c74 5402 0000 7306  ....resultT...s.
+00004070: 0000 0008 0112 010c 027a 2141 7574 6865  .........z!Authe
+00004080: 6e74 6963 6174 652e 706f 7374 2e3c 6c6f  nticate.post.<lo
+00004090: 6361 6c73 3e2e 7265 7375 6c74 2907 723c  cals>.result).r<
+000040a0: 0000 0072 7c00 0000 7213 0000 00da 0c61  ...r|...r......a
+000040b0: 7574 6865 6e74 6963 6174 65da 056c 6f67  uthenticate..log
+000040c0: 696e 7229 0000 0072 ed00 0000 2908 7244  inr)...r....).rD
+000040d0: 0000 0072 4500 0000 7201 0100 0072 a200  ...rE...r....r..
+000040e0: 0000 7233 0100 0072 3901 0000 da04 7573  ..r3...r9.....us
+000040f0: 6572 723d 0100 0072 3600 0000 7236 0000  err=...r6...r6..
+00004100: 0072 3700 0000 724c 0000 004a 0200 0073  .r7...rL...J...s
+00004110: 1000 0000 0c02 0c01 0402 0601 06ff 1002  ................
+00004120: 0803 0c06 7a11 4175 7468 656e 7469 6361  ....z.Authentica
+00004130: 7465 2e70 6f73 744e 2905 7256 0000 0072  te.postN).rV...r
+00004140: 5700 0000 7258 0000 0072 7c00 0000 724c  W...rX...r|...rL
+00004150: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
+00004160: 0000 7237 0000 0072 3101 0000 3802 0000  ..r7...r1...8...
+00004170: 7306 0000 0008 0008 010c 1172 3101 0000  s..........r1...
+00004180: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004190: 0002 0000 0040 0000 0072 a400 0000 2905  .....@...r....).
+000041a0: da05 496e 6465 787a 930a 2020 2020 4d61  ..Indexz..    Ma
+000041b0: 696e 2061 7070 2065 6e74 7279 2070 6f69  in app entry poi
+000041c0: 6e74 2c0a 2020 2020 416c 736f 2062 7569  nt,.    Also bui
+000041d0: 6c64 7320 6c69 6e6f 7765 6220 6669 6c65  lds linoweb file
+000041e0: 2066 6f72 2063 7572 7265 6e74 2075 7365   for current use
+000041f0: 7220 7479 7065 2e0a 2020 2020 436f 6e74  r type..    Cont
+00004200: 656e 7420 6973 206d 6f73 746c 7920 696e  ent is mostly in
+00004210: 2074 6865 203a 7866 696c 653a 6072 6561   the :xfile:`rea
+00004220: 6374 2f6d 6169 6e2e 6874 6d6c 6020 7465  ct/main.html` te
+00004230: 6d70 6c61 7465 2e0a 2020 2020 6302 0000  mplate..    c...
+00004240: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00004250: 0003 0000 0073 2e00 0000 8800 6a00 8901  .....s......j...
+00004260: 0900 8800 6a01 720a 8800 6a01 8901 8700  ....j.r...j.....
+00004270: 8701 6602 6402 6403 8408 7d02 7402 8801  ..f.d.d...}.t...
+00004280: 6a03 7c02 8302 5300 2904 4e54 6300 0000  j.|...S.).NTc...
+00004290: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+000042a0: 0013 0000 0073 b600 0000 7400 6a01 6a02  .....s....t.j.j.
+000042b0: 6a03 7d00 7404 8800 7c00 6a05 6401 8d02  j.}.t...|.j.d...
+000042c0: 7d01 7406 7c00 8800 8801 6402 8d03 7d02  }.t.|.....d...}.
+000042d0: 7c02 6a07 7c01 6403 8d01 0100 6404 7d03  |.j.|.d.....d.}.
+000042e0: 6405 8800 6a08 7600 7229 6406 a009 740a  d...j.v.r)d...t.
+000042f0: a00b 6407 6408 a102 a101 7d03 7c02 6a07  ..d.d.....}.|.j.
+00004300: 7c03 6409 8d01 0100 7c01 6a0c 640f 6900  |.d.....|.j.d.i.
+00004310: 7c02 a401 8e01 7d02 7400 6a01 6a02 6a0d  |.....}.t.j.j.j.
+00004320: 6a05 6a0e 7d04 7c04 a00f 640a a101 7d05  j.j.}.|...d...}.
+00004330: 7410 6a11 7c05 6a12 640f 6900 7c02 a401  t.j.|.j.d.i.|...
+00004340: 8e01 640b 640c 8d02 7d06 6405 8800 6a08  ..d.d...}.d...j.
+00004350: 7600 7259 640d 7c06 640e 3c00 7c06 5300  v.rYd.|.d.<.|.S.
+00004360: 2910 4e72 c500 0000 2903 da09 6672 6f6e  ).Nr....)...fron
+00004370: 745f 656e 6472 4500 0000 7240 0100 0029  t_endrE...r@...)
+00004380: 0172 4a00 0000 725c 0000 00da 0c75 7064  .rJ...r\.....upd
+00004390: 6174 655f 666f 756e 647a 093f 6d74 696d  ate_foundz.?mtim
+000043a0: 653d 7b7d 6907 b201 0069 3f42 0f00 2901  e={}i....i?B..).
+000043b0: da08 6e6f 5f63 6163 6865 7a0f 7265 6163  ..no_cachez.reac
+000043c0: 742f 6d61 696e 2e68 746d 6c72 e900 0000  t/main.htmlr....
+000043d0: 72ea 0000 007a 1222 6361 6368 6522 2c20  r....z."cache", 
+000043e0: 2273 746f 7261 6765 227a 0f43 6c65 6172  "storage"z.Clear
+000043f0: 2d53 6974 652d 4461 7461 7236 0000 0029  -Site-Datar6...)
+00004400: 1372 0b00 0000 723d 0000 0072 3e00 0000  .r....r=...r>...
+00004410: 723f 0000 0072 1c00 0000 723a 0000 0072  r?...r....r:...r
+00004420: 9000 0000 7295 0000 0072 7800 0000 727a  ....r....rx...rz
+00004430: 0000 00da 0672 616e 646f 6dda 0772 616e  .....random..ran
+00004440: 6469 6e74 72ee 0000 0072 f000 0000 72f1  dintr....r....r.
+00004450: 0000 0072 f200 0000 7209 0000 0072 f300  ...r....r....r..
+00004460: 0000 72f4 0000 0029 07da 0275 6972 4a00  ..r....)...uirJ.
+00004470: 0000 72f6 0000 0072 4401 0000 72fa 0000  ..r....rD...r...
+00004480: 0072 fb00 0000 da04 7265 7370 a902 7245  .r......resp..rE
+00004490: 0000 0072 4001 0000 7236 0000 0072 3700  ...r@...r6...r7.
+000044a0: 0000 da05 6765 7469 7478 0200 0073 3200  ....getitx...s2.
+000044b0: 0000 0a01 0203 0202 0401 06fd 0204 0204  ................
+000044c0: 0201 0201 06fa 0c08 0402 0a01 1201 0c01  ................
+000044d0: 1001 0e01 0a01 0401 0e01 0201 06fe 0a04  ................
+000044e0: 0801 0402 7a18 496e 6465 782e 6765 742e  ....z.Index.get.
+000044f0: 3c6c 6f63 616c 733e 2e67 6574 6974 2904  <locals>.getit).
+00004500: 7240 0100 00da 0a73 7562 7374 5f75 7365  r@.....subst_use
+00004510: 7272 2900 0000 72ed 0000 00a9 0372 4400  rr)...r......rD.
+00004520: 0000 7245 0000 0072 4a01 0000 7236 0000  ..rE...rJ...r6..
+00004530: 0072 4901 0000 7237 0000 0072 7c00 0000  .rI...r7...r|...
+00004540: 7102 0000 730c 0000 0006 0202 0106 0106  q...s...........
+00004550: 010e 020c 227a 0949 6e64 6578 2e67 6574  ...."z.Index.get
+00004560: 4e72 b000 0000 7236 0000 0072 3600 0000  Nr....r6...r6...
+00004570: 7236 0000 0072 3700 0000 7241 0100 006a  r6...r7...rA...j
+00004580: 0200 0072 b200 0000 7241 0100 0063 0000  ...r....rA...c..
+00004590: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000045a0: 0000 4000 0000 72a4 0000 0029 05da 0c55  ..@...r....)...U
+000045b0: 7365 7253 6574 7469 6e67 737a 420a 2020  serSettingszB.  
+000045c0: 2020 416a 6178 2069 6e74 6572 6661 6365    Ajax interface
+000045d0: 2066 6f72 2067 6574 7469 6e67 2074 6865   for getting the
+000045e0: 2063 7572 7265 6e74 2073 6573 7369 6f6e   current session
+000045f0: 2f75 7365 7220 7365 7474 696e 6773 2e63  /user settings.c
+00004600: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00004610: 0400 0000 0300 0000 734e 0000 0074 007c  ........sN...t.|
+00004620: 0183 017d 017c 016a 0189 037c 016a 0289  ...}.|.j...|.j..
+00004630: 0188 0172 117c 016a 02a0 03a1 006e 0164  ...r.|.j.....n.d
+00004640: 0189 0288 036a 0489 0087 0087 0187 0287  .....j..........
+00004650: 0366 0464 0264 0384 087d 0274 0588 0170  .f.d.d...}.t...p
+00004660: 2388 036a 067c 0283 0253 0029 044e 725c  #..j.|...S.).Nr\
+00004670: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00004680: 0400 0000 1100 0000 1300 0000 737c 0100  ............s|..
+00004690: 0074 006a 016a 0272 1174 006a 016a 0373  .t.j.j.r.t.j.j.s
+000046a0: 1174 006a 016a 046a 056a 06a0 0764 01a1  .t.j.j.j.j...d..
+000046b0: 0101 0074 0888 036a 0974 0a88 03a0 0ba1  ...t...j.t......
+000046c0: 006a 0c83 0188 036a 0d74 0e83 0074 006a  .j.....j.t...t.j
+000046d0: 016a 0f74 006a 016a 046a 056a 06a0 10a1  .j.t.j.j.j.j....
+000046e0: 008e 0074 006a 016a 116a 1288 0088 0072  ...t.j.j.j.....r
+000046f0: 3488 03a0 13a1 006e 0374 1464 0283 0188  4......n.t.d....
+00004700: 0274 1464 0383 0174 1464 0483 0174 1464  .t.d...t.d...t.d
+00004710: 0483 0174 1464 0583 0174 006a 01a0 1564  ...t.d...t.j...d
+00004720: 06a1 0172 5074 006a 016a 046a 166a 1770  ...rPt.j.j.j.j.p
+00004730: 5374 1464 0783 0188 036a 1864 088d 0f7d  St.d.....j.d...}
+00004740: 0088 0272 6888 016a 1904 007c 0064 093c  ...rh..j...|.d.<
+00004750: 007c 0064 0a3c 0088 016a 097c 0064 0b3c  .|.d.<...j.|.d.<
+00004760: 0088 0072 ba88 03a0 1aa1 007c 0064 0c3c  ...r.......|.d.<
+00004770: 0088 036a 1b7c 0064 0d3c 0074 006a 016a  ...j.|.d.<.t.j.j
+00004780: 046a 166a 1c72 ba88 03a0 1da1 000c 007d  .j.j.r.........}
+00004790: 017c 0172 ba88 036a 1e64 0075 0172 ba64  .|.r...j.d.u.r.d
+000047a0: 0e7c 0064 0f3c 0088 036a 1e74 1f6a 2074  .|.d.<...j.t.j t
+000047b0: 006a 016a 046a 166a 2164 108d 0117 007d  .j.j.j.j!d.....}
+000047c0: 0274 22a0 2364 11a1 018f 1101 0074 1f6a  .t".#d.......t.j
+000047d0: 1fa0 2474 22a0 257c 02a1 01a1 017d 0357  ..$t".%|.....}.W
+000047e0: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+000047f0: b177 0101 0001 0001 0059 0001 007c 037c  .w.......Y...|.|
+00004800: 0064 123c 0074 267c 0083 0153 0029 134e  .d.<.t&|...S.).N
+00004810: 46da 0941 6e6f 6e79 6d6f 7573 7a31 596f  F..Anonymousz1Yo
+00004820: 7520 6172 6520 6175 7468 6f72 6973 6564  u are authorised
+00004830: 2074 6f20 6163 7420 6173 2074 6865 2066   to act as the f
+00004840: 6f6c 6c6f 7769 6e67 2075 7365 7273 2e7a  ollowing users.z
+00004850: 1341 6374 2061 7320 616e 6f74 6865 7220  .Act as another 
+00004860: 7573 6572 7a1b 5374 6f70 2061 6374 696e  userz.Stop actin
+00004870: 6720 6173 2061 6e6f 7468 6572 2075 7365  g as another use
+00004880: 72da 0575 7365 7273 7a0b 4d79 2073 6574  r..usersz.My set
+00004890: 7469 6e67 7329 0f72 ed00 0000 7228 0100  tings).r....r(..
+000048a0: 00da 0565 6d61 696c 72f8 0000 00da 0973  ...emailr......s
+000048b0: 6974 655f 6461 7461 da09 7369 7465 5f6e  ite_data..site_n
+000048c0: 616d 65da 096c 6f67 6765 645f 696e 7233  ame..logged_inr3
+000048d0: 0100 00da 0773 755f 6e61 6d65 da0e 6163  .....su_name..ac
+000048e0: 745f 6173 5f73 7562 7465 7874 da11 6163  t_as_subtext..ac
+000048f0: 745f 6173 5f74 6974 6c65 5f74 6578 74da  t_as_title_text.
+00004900: 1261 6374 5f61 735f 6275 7474 6f6e 5f74  .act_as_button_t
+00004910: 6578 74da 1061 6374 5f61 735f 7365 6c66  ext..act_as_self
+00004920: 5f74 6578 74da 0f6d 795f 7365 7474 696e  _text..my_settin
+00004930: 675f 7465 7874 da07 7573 6572 5f69 6472  g_text..user_idr
+00004940: 5a01 0000 da05 7375 5f69 64da 0c73 755f  Z.....su_id..su_
+00004950: 7573 6572 5f74 7970 65da 0b61 7574 686f  user_type..autho
+00004960: 7269 7469 6573 da10 6461 7368 626f 6172  rities..dashboar
+00004970: 645f 6c61 796f 7574 54da 1472 6571 7569  d_layoutT..requi
+00004980: 7265 5f76 6572 6966 6963 6174 696f 6e29  re_verification)
+00004990: 01da 076d 696e 7574 6573 da03 5554 43da  ...minutes..UTC.
+000049a0: 0b63 6f64 655f 6578 7069 7279 2927 720b  .code_expiry)'r.
+000049b0: 0000 0072 3d00 0000 723b 0100 00da 166e  ...r=...r;.....n
+000049c0: 6576 6572 5f62 7569 6c64 5f73 6974 655f  ever_build_site_
+000049d0: 6361 6368 6572 3e00 0000 723f 0000 0072  cacher>...r?...r
+000049e0: 3a00 0000 723c 0100 0072 9000 0000 72ed  :...r<...r....r.
+000049f0: 0000 0072 8f00 0000 7227 0100 0072 2801  ...r....r'...r(.
+00004a00: 0000 7250 0100 0072 1100 0000 da14 6275  ..rP...r......bu
+00004a10: 696c 645f 7369 7465 5f63 6163 6865 5f75  ild_site_cache_u
+00004a20: 726c da0d 6c69 6e6f 5f6a 735f 7061 7274  rl..lino_js_part
+00004a30: 73da 0b70 726f 6a65 6374 5f64 6972 da04  s..project_dir..
+00004a40: 6e61 6d65 da0d 6765 745f 6675 6c6c 5f6e  name..get_full_n
+00004a50: 616d 65da 015f da0c 6973 5f69 6e73 7461  ame.._..is_insta
+00004a60: 6c6c 6564 724f 0100 0072 5901 0000 7248  lledrO...rY...rH
+00004a70: 0000 0072 5d00 0000 da0f 6765 745f 6175  ...r].....get_au
+00004a80: 7468 6f72 6974 6965 7372 5e01 0000 da19  thoritiesr^.....
+00004a90: 616c 6c6f 775f 6f6e 6c69 6e65 5f72 6567  allow_online_reg
+00004aa0: 6973 7472 6174 696f 6eda 0b69 735f 7665  istration..is_ve
+00004ab0: 7269 6669 6564 da19 7665 7269 6669 6361  rified..verifica
+00004ac0: 7469 6f6e 5f63 6f64 655f 7365 6e74 5f6f  tion_code_sent_o
+00004ad0: 6eda 0864 6174 6574 696d 65da 0974 696d  n..datetime..tim
+00004ae0: 6564 656c 7461 da19 7665 7269 6669 6361  edelta..verifica
+00004af0: 7469 6f6e 5f63 6f64 655f 6578 7069 7265  tion_code_expire
+00004b00: 7372 0f00 0000 da08 6f76 6572 7269 6465  sr......override
+00004b10: da09 7469 6d65 7374 616d 70da 0a6d 616b  ..timestamp..mak
+00004b20: 655f 6e61 6976 6572 2100 0000 2904 da0d  e_naiver!...)...
+00004b30: 7573 6572 5f73 6574 7469 6e67 7372 5f01  user_settingsr_.
+00004b40: 0000 da0b 6578 7069 7279 5f74 696d 65da  ....expiry_time.
+00004b50: 0c65 7870 6972 795f 7374 616d 70a9 04da  .expiry_stamp...
+00004b60: 086e 6f74 5f61 6e6f 6eda 0273 7572 5401  .not_anon..surT.
+00004b70: 0000 72f7 0000 0072 3600 0000 7237 0000  ..r....r6...r7..
+00004b80: 0072 4a01 0000 aa02 0000 7352 0000 0008  .rJ.......sR....
+00004b90: 0206 0102 ff12 0202 0204 010c 0104 0104  ................
+00004ba0: 0216 0108 0102 0112 0102 0106 0106 0106  ................
+00004bb0: 0106 011e 0204 0106 ef04 1412 010a 0104  ................
+00004bc0: 020c 010a 010c 020a 010e 0108 0108 010a  ................
+00004bd0: 0108 ff0c 0306 0108 0106 ff1c ff08 0308  ................
+00004be0: 027a 1f55 7365 7253 6574 7469 6e67 732e  .z.UserSettings.
+00004bf0: 6765 742e 3c6c 6f63 616c 733e 2e67 6574  get.<locals>.get
+00004c00: 6974 2907 721c 0000 0072 4001 0000 724b  it).r....r@...rK
+00004c10: 0100 0072 6801 0000 da10 6973 5f61 7574  ...rh.....is_aut
+00004c20: 6865 6e74 6963 6174 6564 7229 0000 0072  henticatedr)...r
+00004c30: ed00 0000 724c 0100 0072 3600 0000 7278  ....rL...r6...rx
+00004c40: 0100 0072 3700 0000 727c 0000 00a1 0200  ...r7...r|......
+00004c50: 0073 0e00 0000 0801 0601 0601 1201 0603  .s..............
+00004c60: 1202 1032 7a10 5573 6572 5365 7474 696e  ...2z.UserSettin
+00004c70: 6773 2e67 6574 4e72 b000 0000 7236 0000  gs.getNr....r6..
+00004c80: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+00004c90: 724d 0100 009d 0200 0073 0600 0000 0800  rM.......s......
+00004ca0: 0401 0c03 724d 0100 0072 b600 0000 2962  ....rM...r....)b
+00004cb0: 72b1 0000 00da 026f 7372 0200 0000 726f  r......osr....ro
+00004cc0: 0100 00da 0272 65da 0363 6769 da03 6173  .....re..cgi..as
+00004cd0: 7472 d300 0000 7245 0100 0072 0800 0000  tr....rE...r....
+00004ce0: da05 7479 7065 7372 0300 0000 da11 6a69  ..typesr......ji
+00004cf0: 6e6a 6132 2e65 7863 6570 7469 6f6e 7372  nja2.exceptionsr
+00004d00: 0400 0000 da0a 6574 6765 6e2e 6874 6d6c  ......etgen.html
+00004d10: 7205 0000 0072 0600 0000 da05 6574 6765  r....r......etge
+00004d20: 6eda 0678 6768 746d 6cda 0664 6a61 6e67  n..xghtml..djang
+00004d30: 6f72 0900 0000 da09 646a 616e 676f 2e64  or......django.d
+00004d40: 6272 0a00 0000 da0b 646a 616e 676f 2e63  br......django.c
+00004d50: 6f6e 6672 0b00 0000 da14 646a 616e 676f  onfr......django
+00004d60: 2e76 6965 7773 2e67 656e 6572 6963 720c  .views.genericr.
+00004d70: 0000 00da 1964 6a61 6e67 6f2e 7669 6577  .....django.view
+00004d80: 732e 6765 6e65 7269 632e 6261 7365 720d  s.generic.baser.
+00004d90: 0000 00da 0b64 6a61 6e67 6f2e 636f 7265  .....django.core
+00004da0: 720e 0000 00da 0c64 6a61 6e67 6f2e 7574  r......django.ut
+00004db0: 696c 7372 0f00 0000 da18 646a 616e 676f  ilsr......django
+00004dc0: 2e75 7469 6c73 2e74 7261 6e73 6c61 7469  .utils.translati
+00004dd0: 6f6e 7210 0000 0072 6901 0000 7211 0000  onr....ri...r...
+00004de0: 00da 1664 6a61 6e67 6f2e 636f 7265 2e65  ...django.core.e
+00004df0: 7863 6570 7469 6f6e 7372 1200 0000 da09  xceptionsr......
+00004e00: 6c69 6e6f 2e63 6f72 6572 1300 0000 da0a  lino.corer......
+00004e10: 6c69 6e6f 2e75 7469 6c73 7214 0000 00da  lino.utilsr.....
+00004e20: 106c 696e 6f2e 7574 696c 732e 6a73 6765  .lino.utils.jsge
+00004e30: 6e72 1500 0000 7216 0000 00da 0f6c 696e  nr....r......lin
+00004e40: 6f2e 636f 7265 2e65 6c65 6d73 7217 0000  o.core.elemsr...
+00004e50: 00da 106c 696e 6f2e 636f 7265 2e66 6965  ...lino.core.fie
+00004e60: 6c64 7372 1800 0000 da0e 6c69 6e6f 2e63  ldsr......lino.c
+00004e70: 6f72 652e 6766 6b73 7219 0000 0072 1b00  ore.gfksr....r..
+00004e80: 0000 da12 6c69 6e6f 2e63 6f72 652e 7265  ....lino.core.re
+00004e90: 7175 6573 7473 721c 0000 0072 1d00 0000  questsr....r....
+00004ea0: da16 6c69 6e6f 2e63 6f72 652e 7461 626c  ..lino.core.tabl
+00004eb0: 6572 6571 7565 7374 721e 0000 00da 0f6c  erequestr......l
+00004ec0: 696e 6f2e 636f 7265 2e76 6965 7773 721f  ino.core.viewsr.
+00004ed0: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00004ee0: 0000 7223 0000 00da 0f6c 696e 6f2e 636f  ..r#.....lino.co
+00004ef0: 7265 2e75 7469 6c73 7224 0000 00da 116c  re.utilsr$.....l
+00004f00: 696e 6f2e 636f 7265 2e61 6374 696f 6e73  ino.core.actions
+00004f10: 7225 0000 0072 2600 0000 da0f 6c69 6e6f  r%...r&.....lino
+00004f20: 2e63 6f72 652e 7374 6f72 6572 2700 0000  .core.storer'...
+00004f30: da17 6c69 6e6f 2e6d 6f64 6c69 622e 7573  ..lino.modlib.us
+00004f40: 6572 732e 7574 696c 7372 2800 0000 7229  ers.utilsr(...r)
+00004f50: 0000 00da 086c 696e 6f2e 6170 6972 2a00  .....lino.apir*.
+00004f60: 0000 da17 6c69 6e6f 2e6d 6f64 6c69 622e  ....lino.modlib.
+00004f70: 6578 746a 732e 7669 6577 7372 2b00 0000  extjs.viewsr+...
+00004f80: 722c 0000 0072 2d00 0000 7238 0000 0072  r,...r-...r8...r
+00004f90: e200 0000 7259 0000 0072 a500 0000 72b4  ....rY...r....r.
+00004fa0: 0000 0072 c400 0000 72cb 0000 0072 d000  ...r....r....r..
+00004fb0: 0000 72fc 0000 0072 1401 0000 7215 0100  ..r....r....r...
+00004fc0: 0072 1701 0000 7220 0100 0072 2601 0000  .r....r ...r&...
+00004fd0: 722c 0100 0072 3101 0000 7241 0100 0072  r,...r1...rA...r
+00004fe0: 4d01 0000 7236 0000 0072 3600 0000 7236  M...r6...r6...r6
+00004ff0: 0000 0072 3700 0000 da08 3c6d 6f64 756c  ...r7.....<modul
+00005000: 653e 0100 0000 737c 0000 0004 040c 0308  e>....s|........
+00005010: 0108 0108 0108 0108 0108 0108 010c 010c  ................
+00005020: 0110 010c 010c 020c 010c 010c 010c 010c  ................
+00005030: 010c 010c 010c 010c 010c 030c 010c 010c  ................
+00005040: 010c 010c 010c 010c 0110 010c 0110 0110  ................
+00005050: 010c 010c 010c 010c 010c 0110 020c 0114  ................
+00005060: 010a 0304 0e10 0710 2210 7110 0f10 2a10  ........".q...*.
+00005070: 1f10 1008 5e08 1310 4310 0410 0810 1010  ....^...C.......
+00005080: 1610 0a10 3214 33                        ....2.3
```

### Comparing `lino_react-23.7.4/lino_react/react/config/react/main.html` & `lino_react-23.7.5/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/config/react/service-worker.js` & `lino_react-23.7.5/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/icons.py` & `lino_react-23.7.5/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/renderer.py` & `lino_react-23.7.5/lino_react/react/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2012-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
+import json
 import os
 from pathlib import Path
 from html import escape
 from django.conf import settings
 from django.db import models
 from django.utils.text import format_lazy
 from django.utils import translation
@@ -149,15 +150,16 @@
         for p in self.other_panels:
             form_panels[p._formpanel_name] = self.panel2json(p)
         data.update(form_panels=form_panels, choicelists=choicelists_data)
 
 
         # print("20210417", data)
 
-        f.write(py2js(data))
+        json.dump(json.loads(py2js(data)), f, indent=4)
+        # f.write(py2js(data))
         # f.write(py2js(data, compact=not settings.SITE.is_demo_site))
         self.serialise_js_code = False
         return 1
 
     def action2json(self, v):
         """Converts global list of all actions to json format."""
         assert isinstance(v, Action)
@@ -707,13 +709,14 @@
 
         for actor in self.actors_list:
             if actor.get_handle_name is not None:
                 continue
             fn = os.path.join(*self.lino_js_parts_chunked(actor.actor_id))
 
             def write(f):
-                f.write(py2js(self.actor2json(actor)))
+                # f.write(py2js(self.actor2json(actor)))
+                json.dump(json.loads(py2js(self.actor2json(actor))), f, indent=4)
 
             settings.SITE.kernel.make_cache_file(fn, write, force)
 
         self.serialise_js_code = False
         return super().build_js_cache(force)
```

### Comparing `lino_react-23.7.4/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.7.5/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.7.5/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.7.5/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.7.5/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/static/react/main.js` & `lino_react-23.7.5/lino_react/react/static/react/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2645,15 +2645,17 @@
                             if ("string" == typeof e.value) {
                                 a[n ? o.fields_index : o.name] = e.value;
                                 var l = this.state.rows.filter((function(t) {
                                     return t.text.toLowerCase().includes(e.value.toLowerCase())
                                 }));
                                 1 === l.length ? a[n ? o.fields_index + 1 : o.name + "Hidden"] = l[0].value : 0 === l.length && "" === e.value && this.props.elem.field_options.allowBlank ? a[n ? o.fields_index + 1 : o.name + "Hidden"] = null : a[n ? o.fields_index + 1 : o.name + "Hidden"] = e.value
                             } else a[n ? o.fields_index : o.name] = e.value.text, a[n ? o.fields_index + 1 : o.name + "Hidden"] = e.value.value;
-                            r(a, o, i)
+                            r(a, o, i), n && "click" === e.originalEvent.type && this.props.column.onEditorSubmit({
+                                columnProps: this.props.column
+                            }, !0, !0)
                         }
                     }, {
                         key: "clear",
                         value: function() {
                             var e, t = this.props,
                                 n = t.in_grid,
                                 o = t.elem,
@@ -3043,15 +3045,19 @@
                                 }
                             }
                         }, {
                             key: "render",
                             value: function() {
                                 return react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, this.state.loadMask && react__WEBPACK_IMPORTED_MODULE_0__.createElement(LinoLoadMask, null), this.props.reload && !this.props.nonCollapsibles && !this.props.onSide && react__WEBPACK_IMPORTED_MODULE_0__.createElement(primereact_button__WEBPACK_IMPORTED_MODULE_3__.z, {
                                     icon: "pi pi-refresh",
-                                    onClick: this.props.reload
+                                    onClick: this.props.reload,
+                                    tooltip: "Reload this view from the underlying database",
+                                    tooltipOptions: {
+                                        position: "bottom"
+                                    }
                                 }), this.render_buttons())
                             }
                         }]), LinoBbar
                     }(react__WEBPACK_IMPORTED_MODULE_0__.Component);
                 LinoBbar.propTypes = {
                     actorData: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
                     an: prop_types__WEBPACK_IMPORTED_MODULE_1___default().string,
@@ -5449,15 +5455,15 @@
                             d.page = void 0 !== n ? n : this.data.page, d.sortFieldName = void 0 !== a ? a.name : this.data.sortFieldName, d.sortOrder = void 0 !== s ? s : this.data.sortOrder, d.displayMode = void 0 !== u ? u : this.state.layout, Object.assign(this.data, {
                                 page: d.page,
                                 sortFieldName: d.sortFieldName,
                                 sortOrder: d.sortOrder,
                                 topRow: d.page * this.data.rowsPerPage
                             });
                             var f = {};
-                            return f[me.Vk] = void 0 !== r ? "" === r ? void 0 : r : this.data.urlParams.query, f[me.i5] = me.oi, f[me.qg] = d.page * this.data.rowsPerPage, f[me.EL] = this.data.rowsPerPage, f[me.mQ] = this.rp || c()(this), f[me.Vp] = d.displayMode, f[me.$S] = me.zf, f[me.xX] = window.App.state.site_data.revision_number, f[me.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, f[me.jT] = window.App.state.site_data[me.jT], void 0 !== d.sortFieldName && (f.sort = d.sortFieldName), 0 !== d.sortOrder && (f.dir = 1 === d.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv ? f[me.ks] = (0, x.ku)(this.props.parent_pv, this.props.actorData.params_fields) : this.props.actorData.params_layout && (f[me.ks] = this.data.urlParams.pv), void 0 !== this.props.mk && null !== this.props.mt && (f.mk = this.props.mk), void 0 !== this.props.mt && null !== this.props.mt && (f.mt = this.props.mt), window.App.add_su(f), f
+                            return f[me.Vk] = void 0 !== r ? "" === r ? void 0 : r : this.data.urlParams.query, f[me.i5] = me.oi, f[me.qg] = d.page * this.data.rowsPerPage, f[me.EL] = this.data.rowsPerPage, f[me.mQ] = this.rp || c()(this), f[me.Vp] = d.displayMode, f[me.$S] = me.zf, f[me.xX] = window.App.state.site_data.revision_number, f[me.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, f[me.jT] = window.App.state.site_data[me.jT], void 0 !== d.sortFieldName && (f.sort = d.sortFieldName), 0 !== d.sortOrder && (f.dir = 1 === d.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv ? f[me.ks] = (0, x.ku)(this.props.parent_pv, this.props.actorData.params_fields) : this.props.actorData.params_layout && !this.props.inDetail && (f[me.ks] = this.data.urlParams.pv), void 0 !== this.props.mk && null !== this.props.mt && (f.mk = this.props.mk), void 0 !== this.props.mt && null !== this.props.mt && (f.mt = this.props.mt), window.App.add_su(f), f
                         }
                     }, {
                         key: "getUri",
                         value: function(e) {
                             var t = "api/".concat(this.props.packId, "/").concat(this.props.actorId);
                             return void 0 !== e && (t += "?".concat(g.stringify(e))), t
                         }
@@ -7521,15 +7527,15 @@
                 }
                 var Labeled = function(e) {
                     var t = e.label || e.elem.label;
                     return react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, !e.hide_label && e.elem.label && react__WEBPACK_IMPORTED_MODULE_0__.createElement(react__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, react__WEBPACK_IMPORTED_MODULE_0__.createElement("label", {
                         className: classnames__WEBPACK_IMPORTED_MODULE_18___default()("l-label", {
                             "l-label--unfilled": !e.isFilled
                         }),
-                        title: e.elem.help_text
+                        title: Object.assign({}, e.elem.value || {}).quicktip || e.elem.help_text
                     }, t, ":"), e.helpText && react__WEBPACK_IMPORTED_MODULE_0__.createElement("span", {
                         style: {
                             float: "right",
                             cursor: "pointer"
                         },
                         title: e.helpText
                     }, "?"), react__WEBPACK_IMPORTED_MODULE_0__.createElement("br", null)), e.children)
@@ -7848,15 +7854,15 @@
                                             background: "transparent",
                                             color: "black"
                                         },
                                         onClick: function(t) {
                                             var n = {
                                                     base_params: {
                                                         mk: e.props.pk,
-                                                        mt: e.props.mt
+                                                        mt: e.props.actorData.slave ? e.props.actorData.content_type : e.props.mt
                                                     }
                                                 },
                                                 o = e.props.elem.name.replace("_", ".");
                                             o.includes(".") || "HtmlBoxElement" != e.props.elem.react_name || (o = e.props.actorId.split(".")[0] + "." + o), window.App.runAction({
                                                 an: "grid",
                                                 actorId: o,
                                                 rp: null,
@@ -8624,15 +8630,15 @@
                                     return react__WEBPACK_IMPORTED_MODULE_0__.createElement(_LinoBody__WEBPACK_IMPORTED_MODULE_16__.Z, {
                                         depth: t.depth,
                                         reload_timestamp: t.reload_timestamp,
                                         ref: window.App.setRpRef,
                                         inDetail: !0,
                                         router: t.router,
                                         mk: t.pk,
-                                        mt: t.mt,
+                                        mt: t.actorData.slave ? t.actorData.content_type : t.mt,
                                         parent_pv: t.parent_pv,
                                         actorId: r,
                                         packId: o,
                                         actorData: n,
                                         widthInCh: e.container.offsetWidth / e.chInPx.offsetWidth
                                     })
                                 }))), react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
@@ -9372,141 +9378,153 @@
                         return !0
                     }
                 }
             },
             5783: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    ec: () => D,
-                    MB: () => P,
-                    ZP: () => R
+                    ec: () => I,
+                    MB: () => T,
+                    ZP: () => q
                 });
                 var o = n(2437),
                     r = (n(4159), n(6318), n(6959)),
                     i = n.n(r),
-                    a = n(3374),
-                    l = (n(9898), n(3723)),
-                    s = n(9694),
-                    p = n(2494),
-                    u = n(2280),
-                    c = n(3215),
-                    d = (n(8330), n(4439)),
-                    f = n(9502),
-                    h = n(1008),
-                    m = n(3379),
-                    b = n.n(m),
-                    g = n(5699);
+                    a = n(9281),
+                    l = n(3374),
+                    s = (n(9898), n(3723)),
+                    p = n(9694),
+                    u = n(2494),
+                    c = n(2280),
+                    d = n(3215),
+                    f = (n(8330), n(7705)),
+                    h = n(4439),
+                    m = n(9502),
+                    b = n(1008),
+                    g = n(3379),
+                    v = n.n(g),
+                    y = n(5699);
 
-                function v(e) {
-                    return v = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function w() {
+                    return w = Object.assign || function(e) {
+                        for (var t = 1; t < arguments.length; t++) {
+                            var n = arguments[t];
+                            for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
+                        }
+                        return e
+                    }, w.apply(this, arguments)
+                }
+
+                function _(e) {
+                    return _ = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, v(e)
+                    }, _(e)
                 }
 
-                function y(e, t) {
+                function k(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }
 
-                function w(e, t) {
+                function x(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function _(e, t, n) {
-                    return t && w(e.prototype, t), n && w(e, n), Object.defineProperty(e, "prototype", {
+                function E(e, t, n) {
+                    return t && x(e.prototype, t), n && x(e, n), Object.defineProperty(e, "prototype", {
                         writable: !1
                     }), e
                 }
 
-                function k(e, t) {
+                function O(e, t) {
                     if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                     Object.defineProperty(e, "prototype", {
                         value: Object.create(t && t.prototype, {
                             constructor: {
                                 value: e,
                                 writable: !0,
                                 configurable: !0
                             }
                         }),
                         writable: !1
-                    }), t && x(e, t)
+                    }), t && C(e, t)
                 }
 
-                function x(e, t) {
-                    return x = Object.setPrototypeOf || function(e, t) {
+                function C(e, t) {
+                    return C = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, x(e, t)
+                    }, C(e, t)
                 }
 
-                function E(e) {
+                function S(e) {
                     var t = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }();
                     return function() {
-                        var n, o = S(e);
+                        var n, o = R(e);
                         if (t) {
-                            var r = S(this).constructor;
+                            var r = R(this).constructor;
                             n = Reflect.construct(o, arguments, r)
                         } else n = o.apply(this, arguments);
-                        return O(this, n)
+                        return D(this, n)
                     }
                 }
 
-                function O(e, t) {
-                    if (t && ("object" === v(t) || "function" == typeof t)) return t;
+                function D(e, t) {
+                    if (t && ("object" === _(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return C(e)
+                    return P(e)
                 }
 
-                function C(e) {
+                function P(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function S(e) {
-                    return S = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function R(e) {
+                    return R = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, S(e)
+                    }, R(e)
                 }
-                b()(g.Z, {
+                v()(y.Z, {
                     insert: "head",
                     singleton: !1
-                }), g.Z.locals;
-                var D = function(e) {
-                    k(n, e);
-                    var t = E(n);
+                }), y.Z.locals;
+                var I = function(e) {
+                    O(n, e);
+                    var t = S(n);
 
                     function n(e) {
                         var o;
-                        return y(this, n), (o = t.call(this, e)).state = {}, o.parent = e.parent, o.onLayoutButtonClick = o.onLayoutButtonClick.bind(C(o)), o.reload = o.reload.bind(C(o)), o.wrappedOnLayoutButtonClick = o.wrappedOnLayoutButtonClick.bind(C(o)), o
+                        return k(this, n), (o = t.call(this, e)).state = {}, o.parent = e.parent, o.onLayoutButtonClick = o.onLayoutButtonClick.bind(P(o)), o.reload = o.reload.bind(P(o)), o.wrappedOnLayoutButtonClick = o.wrappedOnLayoutButtonClick.bind(P(o)), o
                     }
-                    return _(n, [{
+                    return E(n, [{
                         key: "onLayoutButtonClick",
                         value: function(e, t) {
-                            (0, f.rX)(null) ? window.Detail.onDirtyLeave({}, "INAPP", this.wrappedOnLayoutButtonClick, [e, t]): this.wrappedOnLayoutButtonClick(e, t)
+                            (0, m.rX)(null) ? window.Detail.onDirtyLeave({}, "INAPP", this.wrappedOnLayoutButtonClick, [e, t]): this.wrappedOnLayoutButtonClick(e, t)
                         }
                     }, {
                         key: "wrappedOnLayoutButtonClick",
                         value: function(e, t) {
                             switch (e) {
-                                case h.dJ:
+                                case b.dJ:
                                     if (0 === this.parent.data.sr.length) {
                                         var n, o = this.parent.data.rows[0];
-                                        o && (n = o.hasOwnProperty("id") ? o.id : "object" === v(o) ? o[this.parent.props.actorData.pk_index] : null), null === n ? this.setState({
+                                        o && (n = o.hasOwnProperty("id") ? o.id : "object" === _(o) ? o[this.parent.props.actorData.pk_index] : null), null === n ? this.setState({
                                             noData: !0
                                         }) : this.parent.onRowDoubleClick(t, n)
                                     } else {
                                         this.parent.setState({
                                             layout: ""
                                         });
                                         var r = this.parent.data.sr[0];
@@ -9515,15 +9533,15 @@
                                     break;
                                 case "external":
                                     this.parent.multiRowView();
                                     break;
                                 default:
                                     this.parent.setState({
                                         layout: e,
-                                        data_view: [h.dI, h.OW].includes(e)
+                                        data_view: [b.dI, b.OW].includes(e)
                                     }), this.reload({
                                         displayMode: e
                                     })
                             }
                         }
                     }, {
                         key: "reload",
@@ -9536,99 +9554,99 @@
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this;
                             return o.createElement(o.Fragment, null, this.parent.props.actorData.card_layout || this.parent.props.actorData.list_layout || this.parent.props.actorData.contain_media ? o.createElement("span", {
                                 className: "p-buttonset"
-                            }, !this.state.noData && !this.parent.props.inDetail && o.createElement(c.C, {
+                            }, !this.state.noData && !this.parent.props.inDetail && o.createElement(d.C, {
                                 checked: this.parent.data.detail_window,
                                 offIcon: "pi pi-file-o",
                                 offLabel: "",
                                 onChange: function(t) {
-                                    return e.onLayoutButtonClick(h.dJ, t)
+                                    return e.onLayoutButtonClick(b.dJ, t)
                                 },
                                 onIcon: "pi pi-file-o",
                                 onLabel: "",
                                 tooltip: "Detail view",
                                 tooltipOptions: {
                                     position: "left",
                                     showDelay: 50
                                 }
-                            }), this.parent.props.actorData.contain_media && o.createElement(c.C, {
-                                checked: !this.parent.data.detail_window && this.parent.state.layout === h.dI,
+                            }), this.parent.props.actorData.contain_media && o.createElement(d.C, {
+                                checked: !this.parent.data.detail_window && this.parent.state.layout === b.dI,
                                 offIcon: "pi pi-clone",
                                 offLabel: "",
                                 onChange: function(t) {
-                                    return e.onLayoutButtonClick(h.dI)
+                                    return e.onLayoutButtonClick(b.dI)
                                 },
                                 onIcon: "pi pi-clone",
                                 onLabel: "",
                                 tooltip: "Gallery view",
                                 tooltipOptions: {
                                     position: "left",
                                     showDelay: 50
                                 }
-                            }), o.createElement(c.C, {
-                                checked: !this.parent.data.detail_window && this.parent.state.layout === h.UZ,
+                            }), o.createElement(d.C, {
+                                checked: !this.parent.data.detail_window && this.parent.state.layout === b.UZ,
                                 offIcon: "pi pi-map",
                                 offLabel: "",
                                 onChange: function(t) {
-                                    return e.onLayoutButtonClick(h.UZ)
+                                    return e.onLayoutButtonClick(b.UZ)
                                 },
                                 onIcon: "pi pi-map",
                                 onLabel: "",
                                 tooltip: "Story view",
                                 tooltipOptions: {
                                     position: "left",
                                     showDelay: 50
                                 }
-                            }), o.createElement(c.C, {
-                                checked: !this.parent.data.detail_window && this.parent.state.layout === h.do,
+                            }), o.createElement(d.C, {
+                                checked: !this.parent.data.detail_window && this.parent.state.layout === b.do,
                                 offIcon: "pi pi-bars",
                                 offLabel: "",
                                 onChange: function(t) {
-                                    return e.onLayoutButtonClick(h.do)
+                                    return e.onLayoutButtonClick(b.do)
                                 },
                                 onIcon: "pi pi-bars",
                                 onLabel: "",
                                 tooltip: "List view",
                                 tooltipOptions: {
                                     position: "left",
                                     showDelay: 50
                                 }
-                            }), this.parent.props.actorData.card_layout && o.createElement(c.C, {
-                                checked: !this.parent.data.detail_window && this.parent.state.layout === h.OW,
+                            }), this.parent.props.actorData.card_layout && o.createElement(d.C, {
+                                checked: !this.parent.data.detail_window && this.parent.state.layout === b.OW,
                                 offIcon: "pi pi-th-large",
                                 offLabel: "",
                                 onChange: function(t) {
-                                    return e.onLayoutButtonClick(h.OW)
+                                    return e.onLayoutButtonClick(b.OW)
                                 },
                                 onIcon: "pi pi-th-large",
                                 onLabel: "",
                                 tooltip: "Card view",
                                 tooltipOptions: {
                                     position: "left",
                                     showDelay: 50
                                 }
-                            }), o.createElement(c.C, {
-                                checked: !this.parent.data.detail_window && this.parent.state.layout === h.C2,
+                            }), o.createElement(d.C, {
+                                checked: !this.parent.data.detail_window && this.parent.state.layout === b.C2,
                                 offIcon: "pi pi-table",
                                 offLabel: "",
                                 onChange: function(t) {
-                                    return e.onLayoutButtonClick(h.C2)
+                                    return e.onLayoutButtonClick(b.C2)
                                 },
                                 onIcon: "pi pi-table",
                                 onLabel: "",
                                 tooltip: "Table view",
                                 tooltipOptions: {
                                     position: "left",
                                     showDelay: 50
                                 }
-                            })) : null, this.parent.props.inDetail && this.parent.props.actorData.editable && o.createElement(a.z, {
+                            })) : null, this.parent.props.inDetail && this.parent.props.actorData.editable && o.createElement(l.z, {
                                 className: "p-transparent-button",
                                 style: {
                                     border: "0px",
                                     background: "transparent",
                                     color: "black"
                                 },
                                 onClick: function(t) {
@@ -9637,43 +9655,43 @@
                                 icon: "pi pi-external-link",
                                 label: ""
                             }))
                         }
                     }]), n
                 }(o.Component);
 
-                function P(e) {
+                function T(e) {
                     var t = e.parent.state.loading || e.parent.state.refresh || e.parent.state.site_loading;
-                    return o.createElement(p.k, {
+                    return o.createElement(u.k, {
                         mode: "indeterminate",
                         className: t ? "" : "lino-transparent",
                         style: {
                             height: "5px"
                         }
                     })
                 }
-                var R = function(e) {
-                    k(n, e);
-                    var t = E(n);
+                var q = function(e) {
+                    O(n, e);
+                    var t = S(n);
 
                     function n(e) {
                         var o;
-                        return y(this, n), (o = t.call(this, e)).state = {
+                        return k(this, n), (o = t.call(this, e)).state = {
                             query: e.parent.data.urlParams.query || ""
-                        }, o.parent = e.parent, o.controller = new(i()), o.renderActionBar = o.renderActionBar.bind(C(o)), o.renderDataViewSortButton = o.renderDataViewSortButton.bind(C(o)), o.renderDetailNavigator = o.renderDetailNavigator.bind(C(o)), o.renderEditorButton = o.renderEditorButton.bind(C(o)), o.renderParamValueControls = o.renderParamValueControls.bind(C(o)), o.renderQuickFilter = o.renderQuickFilter.bind(C(o)), o.renderToggle_colControls = o.renderToggle_colControls.bind(C(o)), o
+                        }, o.parent = e.parent, o.controller = new(i()), o.renderActionBar = o.renderActionBar.bind(P(o)), o.renderDataViewSortButton = o.renderDataViewSortButton.bind(P(o)), o.renderDetailNavigator = o.renderDetailNavigator.bind(P(o)), o.renderEditorButton = o.renderEditorButton.bind(P(o)), o.renderParamValueControls = o.renderParamValueControls.bind(P(o)), o.renderQuickFilter = o.renderQuickFilter.bind(P(o)), o.renderToggle_colControls = o.renderToggle_colControls.bind(P(o)), o
                     }
-                    return _(n, [{
+                    return E(n, [{
                         key: "componentDidUpdate",
                         value: function(e, t, n) {
-                            window.App.isMobile || this.parent.data.editing_mode || window.App.data.dialogs.length || "calview" === this.parent.props.packId || this.parent.state.showPVDialog || this.inputEl && this.inputEl.focus()
+                            window.App.isMobile || this.parent.data.editing_mode || window.App.data.dialogs.length || "calview" === this.parent.props.packId || this.parent.state.showPVDialog || this.inputEl && (this.inputEl.hasOwnProperty("inputRef") ? this.inputEl.inputRef.current.focus() : this.inputEl.focus())
                         }
                     }, {
                         key: "renderActionBar",
                         value: function(e, t) {
-                            return o.createElement(d.Z, {
+                            return o.createElement(h.Z, {
                                 actorData: this.parent.props.actorData,
                                 disabledFields: this.parent.data.disabled_fields,
                                 editing_mode: this.parent.data.editing_mode,
                                 mk: this.parent.props.mk,
                                 mt: this.parent.props.mt,
                                 sr: this.parent.data.detail_window ? [this.parent.data.id] : this.parent.data.sr,
                                 reload: this.parent.reload,
@@ -9697,15 +9715,15 @@
                                         label: t.name,
                                         value: String(t.fields_index),
                                         command: function(t) {
                                             e.parent.data.sortField = t.item.value, e.parent.data.sortFieldName = t.item.label, e.parent.refresh()
                                         }
                                     }
                                 }));
-                                return o.createElement(u.a, {
+                                return o.createElement(c.a, {
                                     icon: 0 === this.parent.data.sortOrder ? "pi pi-sort-alt" : 1 === this.parent.data.sortOrder ? "pi pi-sort-amount-up" : "pi pi-sort-amount-down",
                                     label: "Sort By: " + (this.parent.data.sortFieldName || ""),
                                     model: t,
                                     onClick: function(t) {
                                         var n = 1 === e.parent.data.sortOrder ? -1 : 1;
                                         e.parent.onSort({
                                             sortOrder: n,
@@ -9718,136 +9736,206 @@
                                 })
                             }
                         }
                     }, {
                         key: "renderDetailNavigator",
                         value: function() {
                             var e = this;
-                            return this.parent.data.detail_window ? this.parent.data.navinfo && o.createElement(o.Fragment, null, o.createElement(a.z, {
+                            return this.parent.data.detail_window ? this.parent.data.navinfo && o.createElement(o.Fragment, null, o.createElement(l.z, {
                                 disabled: this.parent.state.loading || null === this.parent.data.navinfo.first || this.parent.data.navinfo.first === this.parent.data.id,
                                 className: "l-nav-first",
                                 icon: "pi pi-angle-double-left",
                                 onClick: function(t) {
                                     e.parent.onRowDoubleClick(t, e.parent.data.navinfo.first)
                                 }
-                            }), o.createElement(a.z, {
+                            }), o.createElement(l.z, {
                                 disabled: this.parent.state.loading || null === this.parent.data.navinfo.first || this.parent.data.navinfo.first === this.parent.data.id,
                                 className: "l-nav-prev",
                                 icon: "pi pi-angle-left",
                                 onClick: function(t) {
                                     e.parent.onRowDoubleClick(t, e.parent.data.navinfo.prev)
                                 }
-                            }), o.createElement(a.z, {
+                            }), o.createElement(l.z, {
                                 disabled: this.parent.state.loading || null === this.parent.data.navinfo.last || this.parent.data.navinfo.last === this.parent.data.id,
                                 className: "l-nav-next",
                                 icon: "pi pi-angle-right",
                                 onClick: function(t) {
                                     e.parent.onRowDoubleClick(t, e.parent.data.navinfo.next)
                                 }
-                            }), o.createElement(a.z, {
+                            }), o.createElement(l.z, {
                                 disabled: this.parent.state.loading || null === this.parent.data.navinfo.last || this.parent.data.navinfo.last === this.parent.data.id,
                                 className: "l-nav-last",
                                 icon: "pi pi-angle-double-right",
                                 onClick: function(t) {
                                     e.parent.onRowDoubleClick(t, e.parent.data.navinfo.last)
                                 }
                             })) : null
                         }
                     }, {
                         key: "renderEditorButton",
                         value: function() {
                             var e = this;
                             return this.parent.data.detail_window && this.parent.props.actorData.editable && !this.parent.props.actorData.edit_safe ? o.createElement("span", {
                                 hidden: this.parent.data.data.disable_editing
-                            }, o.createElement(c.C, {
+                            }, o.createElement(d.C, {
                                 checked: !this.parent.data.editing_mode,
                                 className: "l-bbar-editor-button",
                                 onChange: function(t) {
                                     e.parent.data.editing_mode = !e.parent.data.editing_mode, e.parent.setState({
                                         loading: !1
                                     })
                                 },
                                 onLabel: "",
                                 offLabel: "",
                                 offIcon: "pi pi-times",
                                 onIcon: "pi pi-pencil",
-                                tooltip: this.parent.data.editing_mode ? "Cancel" : "Edit"
+                                tooltip: this.parent.data.editing_mode ? "Cancel" : "Edit",
+                                tooltipOptions: {
+                                    position: "bottom"
+                                }
                             })) : null
                         }
                     }, {
                         key: "renderParamValueControls",
                         value: function() {
                             var e = this;
-                            return this.parent.props.actorData.params_layout && o.createElement(o.Fragment, null, o.createElement(a.z, {
+                            return this.parent.props.actorData.params_layout && o.createElement(o.Fragment, null, o.createElement(l.z, {
                                 icon: "pi pi-sliders-h",
                                 onClick: function(t) {
                                     e.parent.setState({
                                         showPVDialog: !e.parent.state.showPVDialog
                                     })
+                                },
+                                tooltip: this.parent.state.showPVDialog ? "Hide parameters panel" : "Show parameters panel",
+                                tooltipOptions: {
+                                    position: "bottom"
                                 }
-                            }), 0 !== Object.keys(this.parent.data.pv || {}).length && o.createElement(a.z, {
+                            }), 0 !== Object.keys(this.parent.data.pv || {}).length && o.createElement(l.z, {
                                 icon: "pi pi-times-circle",
                                 onClick: function() {
                                     e.parent.data.params_values = {}, e.parent.data.pv = [], e.parent.reload()
+                                },
+                                tooltip: "Clear and set the parameter values to default",
+                                tooltipOptions: {
+                                    position: "bottom"
                                 }
                             }))
                         }
                     }, {
                         key: "renderQuickFilter",
                         value: function(e) {
-                            var t = this;
-                            return this.parent.props.actorData.id, o.createElement("span", {
+                            var t = this,
+                                n = {
+                                    className: "l-grid-quickfilter",
+                                    placeholder: "QuickSearch",
+                                    style: {
+                                        width: e ? "100%" : void 0,
+                                        marginRight: e ? "1ch" : void 0,
+                                        marginLeft: e ? "1ch" : void 0
+                                    },
+                                    ref: function(e) {
+                                        return t.inputEl = e
+                                    },
+                                    value: this.state.query
+                                };
+                            return this.parent.data.detail_window ? o.createElement("span", {
                                 onKeyDown: function(e) {
                                     46 === e.keyCode && e.stopPropagation()
                                 }
-                            }, o.createElement(l.o, {
-                                className: "l-grid-quickfilter",
-                                style: {
-                                    width: e ? "100%" : void 0,
-                                    marginRight: e ? "1ch" : void 0,
-                                    marginLeft: e ? "1ch" : void 0
+                            }, o.createElement(a.Q, w({}, n, {
+                                completeMethod: function(e) {
+                                    return n = e.query, r = (o = t.parent.props).mk, i = o.mt, a = {
+                                        query: n,
+                                        start: 0,
+                                        wt: b.zf
+                                    }, void 0 !== r && (a.mk = r), void 0 !== i && (a.mt = i), t.parent.props.actorData.slave && (a.mt = t.parent.props.actorData.content_type), window.App.add_su(a), void fetch("/choices/".concat(t.parent.props.packId, "/").concat(t.parent.props.actorId, "?").concat(f.stringify(a))).then((function(e) {
+                                        return e.json()
+                                    })).then((function(e) {
+                                        return t.setState((function() {
+                                            return {
+                                                rows: e.rows.slice()
+                                            }
+                                        }))
+                                    })).catch((function(e) {
+                                        return window.App.handleAjaxException(e)
+                                    }));
+                                    var n, o, r, i, a
+                                },
+                                dropdown: !0,
+                                field: "text",
+                                itemTemplate: function(e) {
+                                    var t = "object" === _(e) ? e.text : e;
+                                    return o.createElement("div", {
+                                        dangerouslySetInnerHTML: {
+                                            __html: t || " "
+                                        }
+                                    })
+                                },
+                                onChange: function(e) {
+                                    return t.setState({
+                                        query: e.value
+                                    })
+                                },
+                                onSelect: function(e) {
+                                    var n = t.parent.props,
+                                        o = n.mk,
+                                        r = n.mt,
+                                        i = {
+                                            wt: b.zf
+                                        },
+                                        a = e.value.value;
+                                    if (a && !(0, m.i2)(a)) {
+                                        void 0 !== o && (i.mk = o), void 0 !== r && (i.mt = r), window.App.add_su(i);
+                                        var l = "/api/".concat(t.parent.props.packId, "/").concat(t.parent.props.actorId, "/").concat(a, "?").concat(f.stringify(i));
+                                        t.parent.props.router.history.push(l)
+                                    } else console.log(e)
                                 },
-                                placeholder: "QuickSearch",
-                                value: this.state.query,
+                                suggestions: this.state.rows
+                            }))) : o.createElement("span", {
+                                onKeyDown: function(e) {
+                                    46 === e.keyCode && e.stopPropagation()
+                                }
+                            }, o.createElement(s.o, w({}, n, {
                                 onChange: function(e) {
                                     t.controller.abort(), t.controller = new(i());
                                     var n = e.target.value;
                                     t.setState({
                                         query: n
                                     }), t.parent.quickFilter({
                                         query: n,
                                         signal: t.controller.signal
                                     })
-                                },
-                                ref: function(e) {
-                                    return t.inputEl = e
                                 }
-                            }))
+                            })))
                         }
                     }, {
                         key: "renderToggle_colControls",
                         value: function() {
                             var e = this;
                             return this.parent.data.detail_window ? null : o.createElement(o.Fragment, null, o.createElement("span", {
                                 style: {
                                     position: "relative"
                                 },
                                 ref: function(t) {
                                     return e.toggleCol = t
                                 }
-                            }, o.createElement(a.z, {
+                            }, o.createElement(l.z, {
                                 icon: "pi pi-list",
                                 onClick: function() {
                                     e.parent.setState({
                                         toggle_col: !0
                                     }), e.show_col_selector.show()
+                                },
+                                tooltip: "Configure visibility of the grid columns",
+                                tooltipOptions: {
+                                    position: "bottom"
                                 }
                             }), o.createElement("span", {
                                 hidden: !0
-                            }, o.createElement(s.N, {
+                            }, o.createElement(p.N, {
                                 appendTo: this.toggleCol,
                                 panelStyle: {
                                     zIndex: "99999",
                                     height: "auto",
                                     width: "auto",
                                     position: "absolute"
                                 },
@@ -9883,36 +9971,37 @@
                             return o.createElement(o.Fragment, null, this.parent.state.show_top_toolbar ? o.createElement(o.Fragment, null, o.createElement("div", {
                                 className: "table-header"
                             }, o.createElement("div", {
                                 className: "l-bbar-left",
                                 style: {
                                     background: "transparent"
                                 }
-                            }, !this.parent.props.actorData.hide_navigator && o.createElement(o.Fragment, null, this.renderQuickFilter(), this.renderParamValueControls(), this.parent.state.layout !== h.C2 ? this.renderDataViewSortButton() : this.renderToggle_colControls(), this.renderDetailNavigator()), this.renderActionBar(!1), this.renderEditorButton()), o.createElement(D, {
+                            }, !this.parent.props.actorData.hide_navigator && o.createElement(o.Fragment, null, this.renderQuickFilter(), this.renderParamValueControls(), this.parent.state.layout !== b.C2 ? this.renderDataViewSortButton() : this.renderToggle_colControls(), this.renderDetailNavigator()), this.renderActionBar(!1), this.renderEditorButton()), o.createElement(I, {
                                 parent: this.props.parent
-                            }))) : this.props.side ? o.createElement(o.Fragment, null, !this.parent.props.actorData.hide_navigator && o.createElement(o.Fragment, null, this.renderDetailNavigator(), this.parent.state.layout === h.C2 && this.renderToggle_colControls()), this.renderActionBar(!0), this.renderEditorButton()) : !this.parent.props.actorData.hide_top_toolbar && o.createElement(o.Fragment, null, o.createElement("div", {
+                            }))) : this.props.side ? o.createElement(o.Fragment, null, !this.parent.props.actorData.hide_navigator && o.createElement(o.Fragment, null, this.renderDetailNavigator(), this.parent.state.layout === b.C2 && this.renderToggle_colControls()), this.renderActionBar(!0), this.renderEditorButton()) : !this.parent.props.actorData.hide_top_toolbar && o.createElement(o.Fragment, null, o.createElement("div", {
                                 className: "table-header"
                             }, o.createElement("div", {
                                 className: "l-bbar-left",
                                 style: {
                                     background: "transparent"
                                 }
-                            }, !this.parent.props.actorData.hide_navigator && o.createElement(o.Fragment, null, this.renderQuickFilter(), this.renderParamValueControls(), this.parent.state.layout !== h.C2 && this.renderDataViewSortButton()), this.renderActionBar(!1, !0)), o.createElement(D, {
+                            }, !this.parent.props.actorData.hide_navigator && o.createElement(o.Fragment, null, this.renderQuickFilter(), this.renderParamValueControls(), this.parent.state.layout !== b.C2 && this.renderDataViewSortButton()), this.renderActionBar(!1, !0)), o.createElement(I, {
                                 parent: this.props.parent
-                            }))), !this.props.side && o.createElement(o.Fragment, null, o.createElement(P, {
+                            }))), !this.props.side && o.createElement(o.Fragment, null, o.createElement(T, {
                                 parent: this.parent
                             })))
                         }
                     }]), n
                 }(o.Component)
             },
             9502: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     eJ: () => s,
+                    i2: () => p,
                     tq: () => u,
                     k_: () => c,
                     VW: () => d,
                     ol: () => f,
                     rX: () => h,
                     Ds: () => m,
                     a_: () => b,
```

### Comparing `lino_react-23.7.4/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.7.5/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/react/views.py` & `lino_react-23.7.5/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.4/lino_react/setup_info.py` & `lino_react-23.7.5/lino_react/setup_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.7.4',
+    version='23.7.5',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.7.4/lino_react.egg-info/PKG-INFO` & `lino_react-23.7.5/lino_react.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-react
-Version: 23.7.4
+Version: 23.7.5
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
 Classifier:   Environment :: Web Environment
 Classifier:   Framework :: Django
 Classifier:   Intended Audience :: Developers
 Classifier:   Intended Audience :: System Administrators
@@ -25,9 +23,7 @@
 
 
 The React front end for Lino
 
 Project homepage is https://gitlab.com/lino-framework/react
 
 
-
-
```

