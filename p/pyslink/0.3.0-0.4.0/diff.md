# Comparing `tmp/pyslink-0.3.0.tar.gz` & `tmp/pyslink-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslink-0.3.0.tar", last modified: Sat Jan  2 11:16:43 2021, max compression
+gzip compressed data, was "pyslink-0.4.0.tar", max compression
```

## Comparing `pyslink-0.3.0.tar` & `pyslink-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 11:16:43.138886 pyslink-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1461 2021-01-02 11:16:20.000000 pyslink-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-02 11:16:20.000000 pyslink-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2021-01-02 11:16:43.138886 pyslink-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      477 2021-01-02 11:16:20.000000 pyslink-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 11:16:43.134886 pyslink-0.3.0/pyslink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2021-01-02 11:16:43.000000 pyslink-0.3.0/pyslink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      252 2021-01-02 11:16:43.000000 pyslink-0.3.0/pyslink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-02 11:16:43.000000 pyslink-0.3.0/pyslink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       42 2021-01-02 11:16:43.000000 pyslink-0.3.0/pyslink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-02 11:16:43.000000 pyslink-0.3.0/pyslink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-02 11:16:43.000000 pyslink-0.3.0/pyslink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1496 2021-01-02 11:16:20.000000 pyslink-0.3.0/pyslink.py
--rw-r--r--   0 runner    (1001) docker     (116)      138 2021-01-02 11:16:43.138886 pyslink-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1273 2021-01-02 11:16:20.000000 pyslink-0.3.0/setup.py
+-rw-r--r--   0        0        0     1461 2023-07-30 09:13:42.753132 pyslink-0.4.0/LICENSE
+-rw-r--r--   0        0        0      707 2023-07-30 09:13:42.757132 pyslink-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1453 2023-07-30 09:13:42.757132 pyslink-0.4.0/pyslink.py
+-rw-r--r--   0        0        0      670 2023-07-30 09:13:42.757132 pyslink-0.4.0/readme.md
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 pyslink-0.4.0/PKG-INFO
```

### Comparing `pyslink-0.3.0/LICENSE.txt` & `pyslink-0.4.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 Quantmind
+Copyright (c) 2023 Quantmind
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `pyslink-0.3.0/pyslink.py` & `pyslink-0.4.0/pyslink.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Soft link a file/directory with python site-packages directory"""
 import os
 import subprocess
 import sys
 from distutils.sysconfig import get_python_lib
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 
-def sh(command, cwd=None):
+def sh(command: str) -> str:
     return subprocess.Popen(
         command,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         shell=True,
-        cwd=cwd,
         universal_newlines=True,
     ).communicate()[0]
 
 
-def main(argv=None):
-    argv = sys.argv if argv is None else argv
+def main() -> int:
+    argv = sys.argv
     if len(argv) > 1 and len(argv) < 3:
         path = argv[1]
     else:
         print("requires one positional parameters")
         return 1
 
     pylib = get_python_lib()
```

