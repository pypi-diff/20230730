# Comparing `tmp/sleepyemoji-2.5.tar.gz` & `tmp/sleepyemoji-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-2.5.tar", max compression
+gzip compressed data, was "sleepyemoji-2.6.tar", max compression
```

## Comparing `sleepyemoji-2.5.tar` & `sleepyemoji-2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.5/README.md
--rw-r--r--   0        0        0      568 2023-07-30 09:14:06.860328 sleepyemoji-2.5/pyproject.toml
--rwxr-xr-x   0        0        0     1676 2023-07-30 09:13:37.679690 sleepyemoji-2.5/sleepyemoji.py
--rw-r--r--   0        0        0     1268 2023-07-30 09:00:33.922101 sleepyemoji-2.5/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.5/toolchain/emojis.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.5/PKG-INFO
+-rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.6/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 09:16:16.159971 sleepyemoji-2.6/pyproject.toml
+-rwxr-xr-x   0        0        0     1718 2023-07-30 09:16:00.703855 sleepyemoji-2.6/sleepyemoji.py
+-rw-r--r--   0        0        0     1268 2023-07-30 09:00:33.922101 sleepyemoji-2.6/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.6/toolchain/emojis.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.6/PKG-INFO
```

### Comparing `sleepyemoji-2.5/README.md` & `sleepyemoji-2.6/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.5/pyproject.toml` & `sleepyemoji-2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "2.5"
+version = "2.6"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-2.5/sleepyemoji.py` & `sleepyemoji-2.6/sleepyemoji.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     - poetry build
     - poetry publish
     - pip install sleepyemoji --upgrade # pull down update
   3. Update repository
 '''
 
 # stdlib
+import os
 from typing import List, Dict, Union
 from sys import argv, exit, getsizeof
 from subprocess import call, check_output
 # custom modules
 from toolchain.commands import sleepyemoji_logic
 # 3rd party
 try:
@@ -62,14 +63,15 @@
   ───Example
     ./sleepyemoji.py a f h
 
   ───Return
   str :: prettytable string
   '''
   if not categories:
+    os.environ['PAGER'] = 'cat'
     help(sleepyemoji)
   return sleepyemoji_logic(categories)
 
 
 #───Entry────────────────────
 if __name__ == "__main__":
   app()
```

### Comparing `sleepyemoji-2.5/toolchain/commands.py` & `sleepyemoji-2.6/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.5/toolchain/emojis.py` & `sleepyemoji-2.6/toolchain/emojis.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.5/PKG-INFO` & `sleepyemoji-2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 2.5
+Version: 2.6
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

