# Comparing `tmp/sleepyemoji-3.1.tar.gz` & `tmp/sleepyemoji-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-3.1.tar", max compression
+gzip compressed data, was "sleepyemoji-3.2.tar", max compression
```

## Comparing `sleepyemoji-3.1.tar` & `sleepyemoji-3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-3.1/README.md
--rw-r--r--   0        0        0      568 2023-07-30 09:47:13.232415 sleepyemoji-3.1/pyproject.toml
--rwxr-xr-x   0        0        0     1599 2023-07-30 09:46:58.063835 sleepyemoji-3.1/sleepyemoji.py
--rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.1/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.1/toolchain/emojis.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-3.1/PKG-INFO
+-rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-3.2/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 09:48:04.283096 sleepyemoji-3.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1581 2023-07-30 09:47:44.632323 sleepyemoji-3.2/sleepyemoji.py
+-rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.2/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.2/toolchain/emojis.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-3.2/PKG-INFO
```

### Comparing `sleepyemoji-3.1/README.md` & `sleepyemoji-3.2/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.1/pyproject.toml` & `sleepyemoji-3.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "3.1"
+version = "3.2"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-3.1/sleepyemoji.py` & `sleepyemoji-3.2/sleepyemoji.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,13 @@
     str :: prettytable string
     '''
     if not categories:
       os.environ['PAGER'] = 'cat'
       help(sleepyemoji)
       exit(1)
     return run_logic(categories)
-  print(__name__)
   if (__name__ == "sleepyemoji") or (__name__ == '__main__'):
     app()
 
 
 #───Local Testing────────────
 # sleepyemoji(argv)
```

### Comparing `sleepyemoji-3.1/toolchain/commands.py` & `sleepyemoji-3.2/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.1/toolchain/emojis.py` & `sleepyemoji-3.2/toolchain/emojis.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.1/PKG-INFO` & `sleepyemoji-3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 3.1
+Version: 3.2
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

