# Comparing `tmp/todotree-0.1.3.tar.gz` & `tmp/todotree-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todotree-0.1.3.tar", last modified: Sun Jun  5 15:31:16 2022, max compression
+gzip compressed data, was "todotree-1.0.2.tar", max compression
```

## Comparing `todotree-0.1.3.tar` & `todotree-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 chim1aap  (1000) chim1aap  (1001)        0 2022-06-05 15:31:16.594037 todotree-0.1.3/
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)     1211 2021-04-21 17:59:25.000000 todotree-0.1.3/LICENSE
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)     1964 2022-06-05 15:31:16.594037 todotree-0.1.3/PKG-INFO
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)     1431 2022-06-05 13:15:10.000000 todotree-0.1.3/README.md
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)       87 2022-06-05 14:56:51.000000 todotree-0.1.3/pyproject.toml
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)       38 2022-06-05 15:31:16.594037 todotree-0.1.3/setup.cfg
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)      847 2022-06-05 14:53:42.000000 todotree-0.1.3/setup.py
-drwxr-xr-x   0 chim1aap  (1000) chim1aap  (1001)        0 2022-06-05 15:31:16.590704 todotree-0.1.3/src/
-drwxr-xr-x   0 chim1aap  (1000) chim1aap  (1001)        0 2022-06-05 15:31:16.594037 todotree-0.1.3/src/todotree.egg-info/
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)     1964 2022-06-05 15:31:15.000000 todotree-0.1.3/src/todotree.egg-info/PKG-INFO
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)      185 2022-06-05 15:31:16.000000 todotree-0.1.3/src/todotree.egg-info/SOURCES.txt
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)        1 2022-06-05 15:31:16.000000 todotree-0.1.3/src/todotree.egg-info/dependency_links.txt
--rw-r--r--   0 chim1aap  (1000) chim1aap  (1001)        1 2022-06-05 15:31:16.000000 todotree-0.1.3/src/todotree.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1211 2023-07-30 08:50:14.009923 todotree-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1855 2023-07-30 08:50:14.009923 todotree-1.0.2/README.md
+-rw-r--r--   0        0        0     2169 2023-07-30 08:50:34.122963 todotree-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Errors/ProjectFolderError.py
+-rw-r--r--   0        0        0      180 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Errors/TaskParseError.py
+-rw-r--r--   0        0        0      198 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Errors/WishListFolderError.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:50:14.044904 todotree-1.0.2/todotree/Errors/__init__.py
+-rw-r--r--   0        0        0    12425 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Task.py
+-rw-r--r--   0        0        0    11122 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Taskmanager.py
+-rw-r--r--   0        0        0     4493 2023-07-30 08:50:14.014920 todotree-1.0.2/todotree/Tree.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:50:14.044904 todotree-1.0.2/todotree/__init__.py
+-rw-r--r--   0        0        0     5960 2023-07-30 08:50:14.015920 todotree-1.0.2/todotree/config.py
+-rwxr-xr-x   0        0        0    10611 2023-07-30 08:50:14.015920 todotree-1.0.2/todotree/main.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 todotree-1.0.2/PKG-INFO
```

### Comparing `todotree-0.1.3/LICENSE` & `todotree-1.0.2/LICENSE`

 * *Files identical despite different names*

