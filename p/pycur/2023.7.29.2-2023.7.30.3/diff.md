# Comparing `tmp/pycur-2023.7.29.2.tar.gz` & `tmp/pycur-2023.7.30.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycur-2023.7.29.2.tar", last modified: Sat Jul 29 11:40:31 2023, max compression
+gzip compressed data, was "dist/pycur-2023.7.30.3.tar", last modified: Sun Jul 30 09:26:24 2023, max compression
```

## Comparing `pycur-2023.7.29.2.tar` & `pycur-2023.7.30.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:40:31.614230 pycur-2023.7.29.2/
--rw-rw-rw-   0        0        0      408 2023-07-29 11:40:31.612223 pycur-2023.7.29.2/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-29 11:40:14.000000 pycur-2023.7.29.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 11:40:31.578323 pycur-2023.7.29.2/pycur/
--rw-rw-rw-   0        0        0      704 2023-07-29 11:40:26.000000 pycur-2023.7.29.2/pycur/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:40:31.607944 pycur-2023.7.29.2/pycur.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-29 11:40:31.000000 pycur-2023.7.29.2/pycur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-07-29 11:40:31.000000 pycur-2023.7.29.2/pycur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:40:31.000000 pycur-2023.7.29.2/pycur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-29 11:40:31.000000 pycur-2023.7.29.2/pycur.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:40:31.614230 pycur-2023.7.29.2/setup.cfg
--rw-rw-rw-   0        0        0      366 2023-07-29 11:33:42.000000 pycur-2023.7.29.2/setup.py
+drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/
+-rw-rw-r--   0 app       (1000) app       (1000)      681 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/PKG-INFO
+drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur/
+-rw-r--r--   0 app       (1000) app       (1000)     1431 2023-07-30 09:26:19.000000 pycur-2023.7.30.3/pycur/__init__.py
+drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/
+-rw-rw-r--   0 app       (1000) app       (1000)      681 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/PKG-INFO
+-rw-rw-r--   0 app       (1000) app       (1000)      142 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/SOURCES.txt
+-rw-rw-r--   0 app       (1000) app       (1000)        1 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/dependency_links.txt
+-rw-rw-r--   0 app       (1000) app       (1000)        6 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/top_level.txt
+-rw-rw-r--   0 app       (1000) app       (1000)       38 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/setup.cfg
+-rw-r--r--   0 app       (1000) app       (1000)      356 2023-07-30 09:19:47.000000 pycur-2023.7.30.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

