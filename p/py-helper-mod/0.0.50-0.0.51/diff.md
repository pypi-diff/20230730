# Comparing `tmp/py-helper-mod-0.0.50.tar.gz` & `tmp/py-helper-mod-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.50.tar", last modified: Sat Jul 29 18:58:42 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.51.tar", last modified: Sun Jul 30 03:47:26 2023, max compression
```

## Comparing `py-helper-mod-0.0.50.tar` & `py-helper-mod-0.0.51.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.50/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.50/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91802 2023-07-29 18:56:58.000000 py-helper-mod-0.0.50/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.50/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.50/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-30 03:47:26.161456 py-helper-mod-0.0.51/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.51/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-30 03:47:26.161456 py-helper-mod-0.0.51/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.51/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    92078 2023-07-30 03:46:23.000000 py-helper-mod-0.0.51/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-30 03:47:26.161456 py-helper-mod-0.0.51/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.51/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-30 03:47:26.165456 py-helper-mod-0.0.51/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.51/setup.py
```

### Comparing `py-helper-mod-0.0.50/LICENSE` & `py-helper-mod-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.50/PKG-INFO` & `py-helper-mod-0.0.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.50
+Version: 0.0.51
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.50/py_helper.py` & `py-helper-mod-0.0.51/py_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1184,15 +1184,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,50)
+VERSION=(0,0,51)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1646,14 +1646,30 @@
 
 		td = datetime.now() - startTime
 
 		return td
 
 	return Stop
 
+# Running Time Decorator
+def TimeMe(func):
+	"""Time a function call"""
+
+	@functools.wraps(func)
+	def wrapper(*args,**kwargs):
+		startTime = datetime.now()
+
+		results = func(*args,**kwargs)
+
+		endTime = datetime.now()
+
+		return (endTime - startTime), results
+
+	return wrapper
+
 #
 # Generic Helper Functions
 #
 
 # Parse Delimited Strings
 def ParseDelimitedString(input_str,delimiters="'\"",separator=" "):
 	"""Parse An Input String that May have delimited text into an array"""
```

### Comparing `py-helper-mod-0.0.50/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.51/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.50
+Version: 0.0.51
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.50/setup.cfg` & `py-helper-mod-0.0.51/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.50
+version = 0.0.51
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

