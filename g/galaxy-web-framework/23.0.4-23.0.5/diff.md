# Comparing `tmp/galaxy-web-framework-23.0.4.tar.gz` & `tmp/galaxy-web-framework-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_framework/dist/.tmp-o415zbd0/galaxy-web-framework-23.0.4.tar", last modified: Fri Jun 30 22:08:06 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_framework/dist/.tmp-iq036dt0/galaxy-web-framework-23.0.5.tar", last modified: Sun Jul 30 10:54:30 2023, max compression
```

## Comparing `galaxy-web-framework-23.0.4.tar` & `galaxy-web-framework-23.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-web-framework-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/form_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/remoteuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/sqldebug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/translogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/xforwardedhost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/legacy_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/legacy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38893 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/legacy_framework/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/mapper.js
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/proxy/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy/web/short_term_storage/
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/short_term_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/galaxy/web/statsd_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-30 22:08:06.000000 galaxy-web-framework-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:00:50.000000 galaxy-web-framework-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-web-framework-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/form_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/remoteuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/sqldebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/translogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/xforwardedhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/legacy_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/legacy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38893 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/legacy_framework/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/mapper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/proxy/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy/web/short_term_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/short_term_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/galaxy/web/statsd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-30 10:54:30.000000 galaxy-web-framework-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:47:08.000000 galaxy-web-framework-23.0.5/test-requirements.txt
```

### Comparing `galaxy-web-framework-23.0.4/LICENSE` & `galaxy-web-framework-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/PKG-INFO` & `galaxy-web-framework-23.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,26 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Media player fix issue 16415 by `@bdwheele <https://github.com/bdwheele>`_ in `#16443 <https://github.com/galaxyproject/galaxy/pull/16443>`_
+* Fix static file serving for ``robots.txt`` and ``favicon.ico`` when using per_host settings by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#16459 <https://github.com/galaxyproject/galaxy/pull/16459>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/__init__.py` & `galaxy-web-framework-23.0.5/galaxy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/__init__.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/base.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,17 +535,17 @@
         body = [b""]
     # Fall back on sending the file in chunks
     else:
         trans.response.headers["accept-ranges"] = "bytes"
         start = None
         end = None
         if trans.request.range:
-            start = trans.request.range.start
-            end = trans.request.range.end
-            file_size = trans.response.headers["content-length"]
+            start = int(trans.request.range.start)
+            file_size = int(trans.response.headers["content-length"])
+            end = int(file_size if end is None else trans.request.range.end)
             trans.response.headers["content-length"] = str(end - start)
             trans.response.headers["content-range"] = f"bytes {start}-{end - 1}/{file_size}"
             trans.response.status = 206
         body = iterate_file(body, start, end)
     start_response(trans.response.wsgi_status(), trans.response.wsgi_headeritems())
     return body
```

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/decorators.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/__init__.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/grids.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/helpers/tags.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/error.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/error.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/profile.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/remoteuser.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/remoteuser.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/sqldebug.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/sqldebug.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/static.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/static.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,33 +14,36 @@
     def __init__(self, directory, cache_seconds=None, directory_per_host=None):
         StaticURLParser.__init__(self, directory)
         self.cache_seconds = cache_seconds
         self.directory_per_host = directory_per_host
 
     def __call__(self, environ, start_response):
         path_info = environ.get("PATH_INFO", "")
-        if not path_info:
+        script_name = environ.get("SCRIPT_NAME", "")
+        if script_name == "/robots.txt" or script_name == "/favicon.ico":
+            filename = script_name.replace("/", "")
+        elif not path_info:
             # See if this is a static file hackishly mapped.
             if os.path.exists(self.directory) and os.path.isfile(self.directory):
                 app = FileApp(self.directory)
                 if self.cache_seconds:
                     app.cache_control(max_age=int(self.cache_seconds))
                 return app(environ, start_response)
             return self.add_slash(environ, start_response)
-        if path_info == "/":
+        elif path_info == "/":
             # @@: This should obviously be configurable
             filename = "index.html"
         else:
             filename = request.path_info_pop(environ)
 
         directory = self.directory
         host = environ.get("HTTP_HOST")
         if self.directory_per_host and host:
             for host_key, host_val in self.directory_per_host.items():
-                if host_key in host:
+                if host_key == host:
                     directory = host_val
                     break
 
         full = self.normpath(os.path.join(directory, filename))
         if not full.startswith(directory):
             # Out of bounds
             return self.not_found(environ, start_response)
```

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/statsd.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/statsd.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/translogger.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/translogger.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/framework/middleware/xforwardedhost.py` & `galaxy-web-framework-23.0.5/galaxy/web/framework/middleware/xforwardedhost.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/legacy_framework/grids.py` & `galaxy-web-framework-23.0.5/galaxy/web/legacy_framework/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/proxy/__init__.py` & `galaxy-web-framework-23.0.5/galaxy/web/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/proxy/js/Dockerfile` & `galaxy-web-framework-23.0.5/galaxy/web/proxy/js/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/main.js` & `galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/main.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/mapper.js` & `galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/mapper.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/proxy/js/lib/proxy.js` & `galaxy-web-framework-23.0.5/galaxy/web/proxy/js/lib/proxy.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/short_term_storage/__init__.py` & `galaxy-web-framework-23.0.5/galaxy/web/short_term_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy/web/statsd_client.py` & `galaxy-web-framework-23.0.5/galaxy/web/statsd_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/PKG-INFO` & `galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,26 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Media player fix issue 16415 by `@bdwheele <https://github.com/bdwheele>`_ in `#16443 <https://github.com/galaxyproject/galaxy/pull/16443>`_
+* Fix static file serving for ``robots.txt`` and ``favicon.ico`` when using per_host settings by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#16459 <https://github.com/galaxyproject/galaxy/pull/16459>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-web-framework-23.0.4/galaxy_web_framework.egg-info/SOURCES.txt` & `galaxy-web-framework-23.0.5/galaxy_web_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.4/setup.cfg` & `galaxy-web-framework-23.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-framework
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	galaxy-web-stack
```

