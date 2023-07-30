# Comparing `tmp/FSRS-Optimizer-4.5.2.tar.gz` & `tmp/FSRS-Optimizer-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.5.2.tar", last modified: Sun Jul 30 02:55:23 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.5.3.tar", last modified: Sun Jul 30 03:06:24 2023, max compression
```

## Comparing `FSRS-Optimizer-4.5.2.tar` & `FSRS-Optimizer-4.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52297 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52297 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.5.2/LICENSE` & `FSRS-Optimizer-4.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.2/PKG-INFO` & `FSRS-Optimizer-4.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.2
+Version: 4.5.3
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.2/README.md` & `FSRS-Optimizer-4.5.3/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.2
+Version: 4.5.3
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.2/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.5.3/src/fsrs_optimizer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import fsrs_optimizer
 import argparse
 import json
 import pytz
 import os
 from pathlib import Path
 
+import matplotlib.pyplot as plt
+
 def prompt(msg: str, fallback):
     default = ""
     if fallback:
         default = f"(default: {fallback})"
 
     response = input(f"{msg} {default}: ")
     if response == "":
@@ -130,25 +132,25 @@
                         action=argparse.BooleanOptionalAction,
                         help="If set automatically defaults on all stdin settings."
                         )
     parser.add_argument("-o","--out",
                         help="File to APPEND the automatically generated profile to."
                         )
     args = parser.parse_args()
-
+    curdir = os.getcwd()
     for filename in args.filenames:
         if os.path.isdir(filename):
             files = [f for f in os.listdir(filename) if f.lower().endswith('.apkg')]
             files = [os.path.join(filename, f) for f in files]
             for file_path in files:
                 try:
-                    curdir = os.getcwd()
                     process(file_path)
-                    os.chdir(curdir)
                 except Exception as e:
                     print(e)
                     print(f"Failed to process {file_path}")
+                finally:
+                    plt.close('all')
                     os.chdir(curdir)
                     continue
         else:
             process(filename)
```

### Comparing `FSRS-Optimizer-4.5.2/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.5.3/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files identical despite different names*

