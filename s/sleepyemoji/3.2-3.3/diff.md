# Comparing `tmp/sleepyemoji-3.2.tar.gz` & `tmp/sleepyemoji-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-3.2.tar", max compression
+gzip compressed data, was "sleepyemoji-3.3.tar", max compression
```

## Comparing `sleepyemoji-3.2.tar` & `sleepyemoji-3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-3.2/README.md
--rw-r--r--   0        0        0      568 2023-07-30 09:48:04.283096 sleepyemoji-3.2/pyproject.toml
--rwxr-xr-x   0        0        0     1581 2023-07-30 09:47:44.632323 sleepyemoji-3.2/sleepyemoji.py
--rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.2/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.2/toolchain/emojis.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-3.2/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.3/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 09:58:40.929674 sleepyemoji-3.3/pyproject.toml
+-rwxr-xr-x   0        0        0     1580 2023-07-30 09:48:18.187624 sleepyemoji-3.3/sleepyemoji.py
+-rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.3/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.3/toolchain/emojis.py
+-rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 sleepyemoji-3.3/PKG-INFO
```

### Comparing `sleepyemoji-3.2/pyproject.toml` & `sleepyemoji-3.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "3.2"
+version = "3.3"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-3.2/sleepyemoji.py` & `sleepyemoji-3.3/sleepyemoji.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
   sleepyemoji(argv[1:])
   exit(0)
 
 Adding Emojis:
   1. New category? Update toolchain/commands.py
   2. Append lists in toolchain/emojis.py
-  3. Update pypi package:
+  3. Update pypi package
   4. Update repository
 '''
 
 # stdlib
 import os
 from typing import List
 from sys import exit, argv
```

### Comparing `sleepyemoji-3.2/toolchain/commands.py` & `sleepyemoji-3.3/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.2/toolchain/emojis.py` & `sleepyemoji-3.3/toolchain/emojis.py`

 * *Files identical despite different names*

