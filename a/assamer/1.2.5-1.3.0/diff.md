# Comparing `tmp/assamer-1.2.5.tar.gz` & `tmp/assamer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assamer-1.2.5.tar", last modified: Sun Jul 30 13:41:06 2023, max compression
+gzip compressed data, was "assamer-1.3.0.tar", last modified: Sun Jul 30 13:54:53 2023, max compression
```

## Comparing `assamer-1.2.5.tar` & `assamer-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 13:41:06.071381 assamer-1.2.5/
--rw-rw-rw-   0        0        0      229 2023-07-30 13:41:06.071381 assamer-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2822 2023-07-09 02:17:04.000000 assamer-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 13:41:06.070410 assamer-1.2.5/assamer.egg-info/
--rw-rw-rw-   0        0        0      229 2023-07-30 13:41:06.000000 assamer-1.2.5/assamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-07-30 13:41:06.000000 assamer-1.2.5/assamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 13:41:06.000000 assamer-1.2.5/assamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 13:41:06.000000 assamer-1.2.5/assamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 13:41:06.000000 assamer-1.2.5/assamer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 13:41:06.071381 assamer-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      330 2023-07-30 13:41:02.000000 assamer-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 13:54:53.843746 assamer-1.3.0/
+-rw-rw-rw-   0        0        0     8586 2023-07-10 19:24:19.000000 assamer-1.3.0/A2L.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 13:49:48.000000 assamer-1.3.0/ASSAM.py
+-rw-rw-rw-   0        0        0      229 2023-07-30 13:54:53.842757 assamer-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2822 2023-07-09 02:17:04.000000 assamer-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 13:54:53.840817 assamer-1.3.0/assamer.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-30 13:54:53.000000 assamer-1.3.0/assamer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3719 2023-07-09 02:22:57.000000 assamer-1.3.0/hexa2l.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 13:54:53.843746 assamer-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      374 2023-07-30 13:54:45.000000 assamer-1.3.0/setup.py
```

### Comparing `assamer-1.2.5/README.md` & `assamer-1.3.0/README.md`

 * *Files identical despite different names*

