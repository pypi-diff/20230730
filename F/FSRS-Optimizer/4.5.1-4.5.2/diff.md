# Comparing `tmp/FSRS-Optimizer-4.5.1.tar.gz` & `tmp/FSRS-Optimizer-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.5.1.tar", last modified: Sat Jul 29 15:58:44 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.5.2.tar", last modified: Sun Jul 30 02:55:23 2023, max compression
```

## Comparing `FSRS-Optimizer-4.5.1.tar` & `FSRS-Optimizer-4.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52297 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 02:55:23.000000 FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:55:23.081514 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52297 2023-07-30 02:55:11.000000 FSRS-Optimizer-4.5.2/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.5.1/LICENSE` & `FSRS-Optimizer-4.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.1/PKG-INFO` & `FSRS-Optimizer-4.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.1
+Version: 4.5.2
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.1/README.md` & `FSRS-Optimizer-4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.5.2/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.1
+Version: 4.5.2
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.1/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.5.2/src/fsrs_optimizer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import fsrs_optimizer
 import argparse
 import json
 import pytz
 import os
+from pathlib import Path
 
 def prompt(msg: str, fallback):
     default = ""
     if fallback:
         default = f"(default: {fallback})"
 
     response = input(f"{msg} {default}: ")
     if response == "":
         if fallback is not None:
             return fallback
         else: # If there is no fallback
             raise Exception("You failed to enter a required parameter")
     return response
 
-def process(filename):
+def process(filepath):
+    suffix = filepath.split('/')[-1].replace(".", "_").replace("@", "_")
+    proj_dir = Path(f'{suffix}')
+    proj_dir.mkdir(parents=True, exist_ok=True)
+    os.chdir(proj_dir)
+
     try: # Try and remember the last values inputted.
         with open(config_save, "r") as f:
             remembered_fallbacks = json.load(f)
     except FileNotFoundError:
         remembered_fallbacks = { # Defaults to this if not there
             "timezone": None, # Timezone starts with no default
             "next_day": 4,
@@ -58,24 +64,26 @@
     with open(config_save, "w+") as f: # Save the settings to load next time the program is run
         json.dump(remembered_fallbacks, f)
 
     save_graphs = graphs_input != "n"
 
     optimizer = fsrs_optimizer.Optimizer()
     optimizer.anki_extract(
-        filename,
+        f"../{filepath}",
         remembered_fallbacks["filter_out_suspended_cards"] == "y"
     )
     analysis = optimizer.create_time_series(
         remembered_fallbacks["timezone"],
         remembered_fallbacks["revlog_start_date"],
         remembered_fallbacks["next_day"]
     )
     print(analysis)
 
+    filename = os.path.splitext(os.path.basename(filepath))[0]
+
     optimizer.define_model()
     figures = optimizer.pretrain(verbose=save_graphs)
     for i, f in enumerate(figures):
         f.savefig(f"pretrain_{i}.png")
     figures = optimizer.train(verbose=save_graphs)
     for i, f in enumerate(figures):
         f.savefig(f"train_{i}.png")
@@ -87,15 +95,15 @@
             f.savefig(f"find_optimal_retention_{i}.png")
 
     optimizer.preview(optimizer.optimal_retention)
 
     profile = \
     f"""{{
     // Generated, Optimized anki deck settings
-    "deckName": "{os.path.splitext(os.path.basename(filename))[0]}",// PLEASE CHANGE THIS TO THE DECKS PROPER NAME
+    "deckName": "{filename}",// PLEASE CHANGE THIS TO THE DECKS PROPER NAME
     "w": {optimizer.w},
     "requestRetention": {optimizer.optimal_retention},
     "maximumInterval": 36500,
 }},
 """
 
     print("Paste this into your scheduling code")
@@ -129,14 +137,18 @@
 
     for filename in args.filenames:
         if os.path.isdir(filename):
             files = [f for f in os.listdir(filename) if f.lower().endswith('.apkg')]
             files = [os.path.join(filename, f) for f in files]
             for file_path in files:
                 try:
+                    curdir = os.getcwd()
                     process(file_path)
+                    os.chdir(curdir)
                 except Exception as e:
+                    print(e)
                     print(f"Failed to process {file_path}")
+                    os.chdir(curdir)
                     continue
         else:
             process(filename)
```

### Comparing `FSRS-Optimizer-4.5.1/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.5.2/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files identical despite different names*

