# Comparing `tmp/pyboko-0.1.0.tar.gz` & `tmp/pyboko-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboko-0.1.0.tar", last modified: Thu Jul 27 23:33:12 2023, max compression
+gzip compressed data, was "pyboko-0.1.0.post1.tar", last modified: Sun Jul 30 03:58:17 2023, max compression
```

## Comparing `pyboko-0.1.0.tar` & `pyboko-0.1.0.post1.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 23:33:12.912776 pyboko-0.1.0/
--rw-rw-rw-   0        0        0    35057 2023-07-27 23:32:13.000000 pyboko-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      218 2023-07-27 23:33:12.911773 pyboko-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-07-27 23:28:49.000000 pyboko-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 23:33:12.911773 pyboko-0.1.0/pyboko.egg-info/
--rw-rw-rw-   0        0        0      218 2023-07-27 23:33:12.000000 pyboko-0.1.0/pyboko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-07-27 23:33:12.000000 pyboko-0.1.0/pyboko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 23:33:12.000000 pyboko-0.1.0/pyboko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 23:33:12.000000 pyboko-0.1.0/pyboko.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 23:33:12.000000 pyboko-0.1.0/pyboko.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 23:33:12.912776 pyboko-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      317 2023-07-27 23:33:03.000000 pyboko-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 03:58:17.924344 pyboko-0.1.0.post1/
+-rw-rw-rw-   0        0        0    35057 2023-07-27 23:32:13.000000 pyboko-0.1.0.post1/LICENSE
+-rw-rw-rw-   0        0        0      224 2023-07-30 03:58:17.922840 pyboko-0.1.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-07-27 23:28:49.000000 pyboko-0.1.0.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 03:58:17.904614 pyboko-0.1.0.post1/pyboko/
+-rw-rw-rw-   0        0        0        0 2023-07-30 03:55:12.000000 pyboko-0.1.0.post1/pyboko/__init__.py
+-rw-rw-rw-   0        0        0     1918 2023-07-27 22:04:50.000000 pyboko-0.1.0.post1/pyboko/client.py
+drwxrwxrwx   0        0        0        0 2023-07-30 03:58:17.922840 pyboko-0.1.0.post1/pyboko/models/
+-rw-rw-rw-   0        0        0      133 2023-07-26 04:49:35.000000 pyboko-0.1.0.post1/pyboko/models/__init__.py
+-rw-rw-rw-   0        0        0     6297 2023-07-27 23:20:15.000000 pyboko-0.1.0.post1/pyboko/models/models.py
+-rw-rw-rw-   0        0        0      533 2023-07-26 05:17:19.000000 pyboko-0.1.0.post1/pyboko/models/sounds.py
+drwxrwxrwx   0        0        0        0 2023-07-30 03:58:17.920841 pyboko-0.1.0.post1/pyboko.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-07-30 03:58:17.000000 pyboko-0.1.0.post1/pyboko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-30 03:58:17.000000 pyboko-0.1.0.post1/pyboko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 03:58:17.000000 pyboko-0.1.0.post1/pyboko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 03:58:17.000000 pyboko-0.1.0.post1/pyboko.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 03:58:17.000000 pyboko-0.1.0.post1/pyboko.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 03:58:17.924344 pyboko-0.1.0.post1/setup.cfg
+-rw-rw-rw-   0        0        0      323 2023-07-30 03:57:51.000000 pyboko-0.1.0.post1/setup.py
```

### Comparing `pyboko-0.1.0/LICENSE` & `pyboko-0.1.0.post1/LICENSE`

 * *Files identical despite different names*

