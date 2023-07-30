# Comparing `tmp/sleepyemoji-3.3.tar.gz` & `tmp/sleepyemoji-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-3.3.tar", max compression
+gzip compressed data, was "sleepyemoji-3.4.tar", max compression
```

## Comparing `sleepyemoji-3.3.tar` & `sleepyemoji-3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.3/README.md
--rw-r--r--   0        0        0      568 2023-07-30 09:58:40.929674 sleepyemoji-3.3/pyproject.toml
--rwxr-xr-x   0        0        0     1580 2023-07-30 09:48:18.187624 sleepyemoji-3.3/sleepyemoji.py
--rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.3/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.3/toolchain/emojis.py
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 sleepyemoji-3.3/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.4/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 10:34:52.646069 sleepyemoji-3.4/pyproject.toml
+-rwxr-xr-x   0        0        0     1372 2023-07-30 10:27:04.209058 sleepyemoji-3.4/sleepyemoji.py
+-rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.4/toolchain/commands.py
+-rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.4/toolchain/emojis.py
+-rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 sleepyemoji-3.4/PKG-INFO
```

### Comparing `sleepyemoji-3.3/README.md` & `sleepyemoji-3.4/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.3/pyproject.toml` & `sleepyemoji-3.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "3.3"
+version = "3.4"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-3.3/sleepyemoji.py` & `sleepyemoji-3.4/sleepyemoji.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 try:
   import typer
 except ModuleNotFoundError as e:
   print("Error: Missing one or more 3rd-party packages (pip install).")
   exit(1)
 
 
-#───Commands─────────────────
 def sleepyemoji(categories:List[str]) -> str:
   app = typer.Typer()
   @app.command()
   def run(categories:List[str]) -> str:
     '''Another example command
 
     Prints emojis with some metadata, organized by category.
@@ -55,18 +54,14 @@
 
     ───Example\n
       ./sleepyemoji.py a f h
 
     ───Return\n
     str :: prettytable string
     '''
-    if not categories:
-      os.environ['PAGER'] = 'cat'
-      help(sleepyemoji)
-      exit(1)
     return run_logic(categories)
   if (__name__ == "sleepyemoji") or (__name__ == '__main__'):
     app()
 
 
-#───Local Testing────────────
+## Local Testing
 # sleepyemoji(argv)
```

### Comparing `sleepyemoji-3.3/toolchain/commands.py` & `sleepyemoji-3.4/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.3/toolchain/emojis.py` & `sleepyemoji-3.4/toolchain/emojis.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.3/PKG-INFO` & `sleepyemoji-3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 3.3
+Version: 3.4
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

