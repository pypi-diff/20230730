# Comparing `tmp/ozer-0.1.0.tar.gz` & `tmp/ozer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozer-0.1.0.tar", last modified: Sun Jul 30 10:08:56 2023, max compression
+gzip compressed data, was "ozer-0.1.1.tar", last modified: Sun Jul 30 10:43:38 2023, max compression
```

## Comparing `ozer-0.1.0.tar` & `ozer-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-30 10:08:56.766064 ozer-0.1.0/
--rw-rw-r--   0 oem      (29999) oem      (29999)      160 2023-07-30 10:08:56.766064 ozer-0.1.0/PKG-INFO
--rw-r--r--   0 oem      (29999) oem      (29999)      935 2023-07-22 08:14:26.000000 ozer-0.1.0/README.md
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-30 10:08:56.766064 ozer-0.1.0/ozer.egg-info/
--rw-rw-r--   0 oem      (29999) oem      (29999)      160 2023-07-30 10:08:56.000000 ozer-0.1.0/ozer.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      157 2023-07-30 10:08:56.000000 ozer-0.1.0/ozer.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-30 10:08:56.000000 ozer-0.1.0/ozer.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        5 2023-07-30 10:08:56.000000 ozer-0.1.0/ozer.egg-info/requires.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-30 10:08:56.000000 ozer-0.1.0/ozer.egg-info/top_level.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-07-30 10:08:56.766064 ozer-0.1.0/setup.cfg
--rw-rw-r--   0 oem      (29999) oem      (29999)      282 2023-07-30 10:06:15.000000 ozer-0.1.0/setup.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-30 10:43:38.214801 ozer-0.1.1/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      160 2023-07-30 10:43:38.210801 ozer-0.1.1/PKG-INFO
+-rw-r--r--   0 oem      (29999) oem      (29999)      935 2023-07-22 08:14:26.000000 ozer-0.1.1/README.md
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-30 10:43:38.210801 ozer-0.1.1/ozer.egg-info/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      160 2023-07-30 10:43:38.000000 ozer-0.1.1/ozer.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      157 2023-07-30 10:43:38.000000 ozer-0.1.1/ozer.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-30 10:43:38.000000 ozer-0.1.1/ozer.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        7 2023-07-30 10:43:38.000000 ozer-0.1.1/ozer.egg-info/requires.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-30 10:43:38.000000 ozer-0.1.1/ozer.egg-info/top_level.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-07-30 10:43:38.214801 ozer-0.1.1/setup.cfg
+-rw-rw-r--   0 oem      (29999) oem      (29999)      743 2023-07-30 10:43:07.000000 ozer-0.1.1/setup.py
```

### Comparing `ozer-0.1.0/README.md` & `ozer-0.1.1/README.md`

 * *Files identical despite different names*

