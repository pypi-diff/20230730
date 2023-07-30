# Comparing `tmp/sleepyemoji-2.6.tar.gz` & `tmp/sleepyemoji-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-2.6.tar", max compression
+gzip compressed data, was "sleepyemoji-2.7.tar", max compression
```

## Comparing `sleepyemoji-2.6.tar` & `sleepyemoji-2.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.6/README.md
--rw-r--r--   0        0        0      568 2023-07-30 09:16:16.159971 sleepyemoji-2.6/pyproject.toml
--rwxr-xr-x   0        0        0     1718 2023-07-30 09:16:00.703855 sleepyemoji-2.6/sleepyemoji.py
--rw-r--r--   0        0        0     1268 2023-07-30 09:00:33.922101 sleepyemoji-2.6/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.6/toolchain/emojis.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.6/PKG-INFO
+-rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.7/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 09:31:50.687904 sleepyemoji-2.7/pyproject.toml
+-rwxr-xr-x   0        0        0     1593 2023-07-30 09:30:13.000312 sleepyemoji-2.7/sleepyemoji.py
+-rw-r--r--   0        0        0     1140 2023-07-30 09:27:48.658286 sleepyemoji-2.7/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.7/toolchain/emojis.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.7/PKG-INFO
```

### Comparing `sleepyemoji-2.6/README.md` & `sleepyemoji-2.7/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.6/pyproject.toml` & `sleepyemoji-2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "2.6"
+version = "2.7"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-2.6/toolchain/commands.py` & `sleepyemoji-2.7/toolchain/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # stdlib
-from os import path
-from pathlib import Path
-from typing import List, Dict, Union
-from sys import argv, exit, getsizeof
-from subprocess import call, check_output
+from typing import List
+from sys import exit
 # custom modules
 from toolchain.emojis import *
 # 3rd party
 try:
   from prettytable import PrettyTable
 except ModuleNotFoundError as e:
   print("Error: Missing one or more 3rd-party packages (pip install).")
   exit(1)
 
 
 #───Commands─────────────────
-def sleepyemoji_logic(categories:List[str]) -> str:
+def run_logic(categories:List[str]) -> str:
   '''adds categories to output table provided in input array'''
 
   cats = [i.lower() for i in categories]
   res  = PrettyTable()
 
   res.field_names = [
     "Emoji", "Discord Value", "iOS Descriptor"
@@ -35,8 +32,8 @@
     res.add_rows(icons)
   if ('people' in cats) or ('p' in cats) or ('all' in cats):
     res.add_rows(people)
   if ('combos' in cats) or ('combinations' in cats) or ('all' in cats):
     res.add_rows(combos)
 
   print(res)
-  return res
+  exit(0)
```

### Comparing `sleepyemoji-2.6/toolchain/emojis.py` & `sleepyemoji-2.7/toolchain/emojis.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.6/PKG-INFO` & `sleepyemoji-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 2.6
+Version: 2.7
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

