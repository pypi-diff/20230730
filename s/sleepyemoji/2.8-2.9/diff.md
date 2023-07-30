# Comparing `tmp/sleepyemoji-2.8.tar.gz` & `tmp/sleepyemoji-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-2.8.tar", max compression
+gzip compressed data, was "sleepyemoji-2.9.tar", max compression
```

## Comparing `sleepyemoji-2.8.tar` & `sleepyemoji-2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.8/README.md
--rw-r--r--   0        0        0      568 2023-07-30 09:35:50.752113 sleepyemoji-2.8/pyproject.toml
--rwxr-xr-x   0        0        0     1592 2023-07-30 09:35:32.765454 sleepyemoji-2.8/sleepyemoji.py
--rw-r--r--   0        0        0     1140 2023-07-30 09:27:48.658286 sleepyemoji-2.8/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.8/toolchain/emojis.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.8/PKG-INFO
+-rw-r--r--   0        0        0     2448 2023-07-30 04:08:53.877468 sleepyemoji-2.9/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 09:37:20.997337 sleepyemoji-2.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1600 2023-07-30 09:37:06.615021 sleepyemoji-2.9/sleepyemoji.py
+-rw-r--r--   0        0        0     1140 2023-07-30 09:27:48.658286 sleepyemoji-2.9/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-2.9/toolchain/emojis.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.9/PKG-INFO
```

### Comparing `sleepyemoji-2.8/README.md` & `sleepyemoji-2.9/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.8/pyproject.toml` & `sleepyemoji-2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "2.8"
+version = "2.9"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-2.8/sleepyemoji.py` & `sleepyemoji-2.9/sleepyemoji.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,12 +64,12 @@
     '''
     if not categories:
       os.environ['PAGER'] = 'cat'
       help(sleepyemoji)
       exit(1)
     return run_logic(categories)
   
-  if __name__ == "__run__":
+  if __name__ == "__sleepyemoji__":
     app()
 
 
 #───Entry────────────────────
```

### Comparing `sleepyemoji-2.8/toolchain/commands.py` & `sleepyemoji-2.9/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.8/toolchain/emojis.py` & `sleepyemoji-2.9/toolchain/emojis.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.8/PKG-INFO` & `sleepyemoji-2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 2.8
+Version: 2.9
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

