# Comparing `tmp/shz_geo-0.0.4.tar.gz` & `tmp/shz_geo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shz_geo-0.0.4.tar", last modified: Thu Jul 27 16:52:23 2023, max compression
+gzip compressed data, was "shz_geo-0.1.1.tar", last modified: Sat Jul 29 22:20:58 2023, max compression
```

## Comparing `shz_geo-0.0.4.tar` & `shz_geo-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:52:23.345669 shz_geo-0.0.4/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-25 13:56:48.000000 shz_geo-0.0.4/LICENSE
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:52:23.345351 shz_geo-0.0.4/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-25 13:57:15.000000 shz_geo-0.0.4/README.md
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-27 16:52:23.345774 shz_geo-0.0.4/setup.cfg
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      537 2023-07-27 16:52:19.000000 shz_geo-0.0.4/setup.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:52:23.342578 shz_geo-0.0.4/shz_geo/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       39 2023-07-27 16:52:15.000000 shz_geo-0.0.4/shz_geo/__init__.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:52:23.344855 shz_geo-0.0.4/shz_geo.egg-info/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      200 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/SOURCES.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/dependency_links.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       19 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/requires.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        8 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/top_level.txt
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:20:58.030527 shz_geo-0.1.1/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-29 17:02:27.000000 shz_geo-0.1.1/LICENSE
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      267 2023-07-29 22:20:58.030139 shz_geo-0.1.1/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 17:02:27.000000 shz_geo-0.1.1/README.md
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-29 22:20:58.030666 shz_geo-0.1.1/setup.cfg
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      562 2023-07-29 22:20:50.000000 shz_geo-0.1.1/setup.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:20:58.023115 shz_geo-0.1.1/shz_geo/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:05:58.000000 shz_geo-0.1.1/shz_geo/__init__.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:20:58.027284 shz_geo-0.1.1/shz_geo/modis/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       71 2023-07-29 17:10:58.000000 shz_geo-0.1.1/shz_geo/modis/__init__.py
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1077 2023-07-29 17:10:58.000000 shz_geo-0.1.1/shz_geo/modis/download_data.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:20:58.029301 shz_geo-0.1.1/shz_geo/tools/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       62 2023-07-29 17:11:09.000000 shz_geo-0.1.1/shz_geo/tools/__init__.py
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      356 2023-07-29 22:18:38.000000 shz_geo-0.1.1/shz_geo/tools/normalizeWithScaleFactor.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:20:58.025983 shz_geo-0.1.1/shz_geo.egg-info/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      267 2023-07-29 22:20:57.000000 shz_geo-0.1.1/shz_geo.egg-info/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      325 2023-07-29 22:20:57.000000 shz_geo-0.1.1/shz_geo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-29 22:20:57.000000 shz_geo-0.1.1/shz_geo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       34 2023-07-29 22:20:57.000000 shz_geo-0.1.1/shz_geo.egg-info/requires.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        8 2023-07-29 22:20:57.000000 shz_geo-0.1.1/shz_geo.egg-info/top_level.txt
```

### Comparing `shz_geo-0.0.4/LICENSE` & `shz_geo-0.1.1/LICENSE`

 * *Files identical despite different names*

