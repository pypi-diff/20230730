# Comparing `tmp/DsToDc-0.5.1a0.tar.gz` & `tmp/DsToDc-0.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DsToDc-0.5.1a0.tar", last modified: Sat Jul 29 12:03:46 2023, max compression
+gzip compressed data, was "DsToDc-0.5.1b0.tar", last modified: Sun Jul 30 09:41:47 2023, max compression
```

## Comparing `DsToDc-0.5.1a0.tar` & `DsToDc-0.5.1b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 12:03:46.321160 DsToDc-0.5.1a0/
-drwxrwxrwx   0        0        0        0 2023-07-29 12:03:46.320161 DsToDc-0.5.1a0/DsToDc.egg-info/
--rw-rw-rw-   0        0        0      496 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      128 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      496 2023-07-29 12:03:46.321160 DsToDc-0.5.1a0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-29 12:03:46.322162 DsToDc-0.5.1a0/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-07-29 12:03:43.000000 DsToDc-0.5.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:41:47.613531 DsToDc-0.5.1b0/
+drwxrwxrwx   0        0        0        0 2023-07-30 09:41:47.610531 DsToDc-0.5.1b0/DsToDc.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-07-30 09:41:47.000000 DsToDc-0.5.1b0/DsToDc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2023-07-30 09:41:47.000000 DsToDc-0.5.1b0/DsToDc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:41:47.000000 DsToDc-0.5.1b0/DsToDc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:41:47.000000 DsToDc-0.5.1b0/DsToDc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      417 2023-07-30 09:41:47.612533 DsToDc-0.5.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-30 09:41:47.613531 DsToDc-0.5.1b0/setup.cfg
+-rw-rw-rw-   0        0        0      820 2023-07-30 09:41:37.000000 DsToDc-0.5.1b0/setup.py
```

