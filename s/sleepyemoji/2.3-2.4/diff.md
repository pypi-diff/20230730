# Comparing `tmp/sleepyemoji-2.3.tar.gz` & `tmp/sleepyemoji-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-2.3.tar", max compression
+gzip compressed data, was "sleepyemoji-2.4.tar", max compression
```

## Comparing `sleepyemoji-2.3.tar` & `sleepyemoji-2.4.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.3/README.md
--rw-r--r--   0        0        0      821 2023-07-30 09:03:10.287107 sleepyemoji-2.3/pyproject.toml
--rwxr-xr-x   0        0        0     1655 2023-07-30 08:48:52.465412 sleepyemoji-2.3/sleepyemoji.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.3/PKG-INFO
+-rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.4/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 09:06:08.500527 sleepyemoji-2.4/pyproject.toml
+-rwxr-xr-x   0        0        0     1657 2023-07-30 09:03:39.624836 sleepyemoji-2.4/sleepyemoji.py
+-rw-r--r--   0        0        0     1268 2023-07-30 09:00:33.922101 sleepyemoji-2.4/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.4/toolchain/emojis.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.4/PKG-INFO
```

### Comparing `sleepyemoji-2.3/README.md` & `sleepyemoji-2.4/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.3/sleepyemoji.py` & `sleepyemoji-2.4/sleepyemoji.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Adding Emojis:
   1. Append lists in toolchain/emojis.py
   2. Update pypi package:
     - poetry config http-basic.pypi sleepyboy <password>
     - poetry version <next-version>
     - poetry build
     - poetry publish
-    - pip install <package> --upgrade # pull down update
+    - pip install sleepyemoji --upgrade # pull down update
   3. Update repository
 '''
 
 # stdlib
 from typing import List, Dict, Union
 from sys import argv, exit, getsizeof
 from subprocess import call, check_output
```

### Comparing `sleepyemoji-2.3/PKG-INFO` & `sleepyemoji-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 2.3
+Version: 2.4
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

