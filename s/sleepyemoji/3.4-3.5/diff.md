# Comparing `tmp/sleepyemoji-3.4.tar.gz` & `tmp/sleepyemoji-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-3.4.tar", max compression
+gzip compressed data, was "sleepyemoji-3.5.tar", max compression
```

## Comparing `sleepyemoji-3.4.tar` & `sleepyemoji-3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.4/README.md
--rw-r--r--   0        0        0      568 2023-07-30 10:34:52.646069 sleepyemoji-3.4/pyproject.toml
--rwxr-xr-x   0        0        0     1372 2023-07-30 10:27:04.209058 sleepyemoji-3.4/sleepyemoji.py
--rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.4/toolchain/commands.py
--rw-r--r--   0        0        0     3190 2023-07-30 08:39:13.313344 sleepyemoji-3.4/toolchain/emojis.py
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 sleepyemoji-3.4/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.5/README.md
+-rw-r--r--   0        0        0      568 2023-07-30 10:41:36.876291 sleepyemoji-3.5/pyproject.toml
+-rwxr-xr-x   0        0        0     1372 2023-07-30 10:27:04.209058 sleepyemoji-3.5/sleepyemoji.py
+-rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.5/toolchain/commands.py
+-rw-r--r--   0        0        0     3186 2023-07-30 10:40:43.525787 sleepyemoji-3.5/toolchain/emojis.py
+-rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 sleepyemoji-3.5/PKG-INFO
```

### Comparing `sleepyemoji-3.4/README.md` & `sleepyemoji-3.5/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.4/pyproject.toml` & `sleepyemoji-3.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "3.4"
+version = "3.5"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-3.4/sleepyemoji.py` & `sleepyemoji-3.5/sleepyemoji.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.4/toolchain/commands.py` & `sleepyemoji-3.5/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.4/toolchain/emojis.py` & `sleepyemoji-3.5/toolchain/emojis.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,18 +63,16 @@
   ["❗", ":exclamation:", "red exclamation mark"],
   ["❓", ":question:", "red question mark"],
   ["™️", ":tm:", "trade mark sign"],
   ["📁", ":file_folder:", "closed file folder"],
   ["🎉", ":tada:", "party popper"],
 ]
 people = [
-  "🤷",
-  [":person_shrugging", "person shrugging"],
-  "💃",
-  [":dancer:", "woman dancing"],
+  ["🤷", ":person_shrugging", "person shrugging"],
+  ["💃", ":dancer:", "woman dancing"],
 ]
 
 
 '''
 combos = [
   ['<emojis>', '', ''],
 ]
```

### Comparing `sleepyemoji-3.4/PKG-INFO` & `sleepyemoji-3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 3.4
+Version: 3.5
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

