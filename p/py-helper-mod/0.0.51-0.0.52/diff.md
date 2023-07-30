# Comparing `tmp/py-helper-mod-0.0.51.tar.gz` & `tmp/py-helper-mod-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.51.tar", last modified: Sun Jul 30 03:47:26 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.52.tar", last modified: Sun Jul 30 05:31:22 2023, max compression
```

## Comparing `py-helper-mod-0.0.51.tar` & `py-helper-mod-0.0.52.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-30 03:47:26.161456 py-helper-mod-0.0.51/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.51/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-30 03:47:26.161456 py-helper-mod-0.0.51/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.51/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    92078 2023-07-30 03:46:23.000000 py-helper-mod-0.0.51/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-30 03:47:26.161456 py-helper-mod-0.0.51/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-30 03:47:26.000000 py-helper-mod-0.0.51/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.51/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-30 03:47:26.165456 py-helper-mod-0.0.51/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.51/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-30 05:31:22.674417 py-helper-mod-0.0.52/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.52/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-30 05:31:22.674417 py-helper-mod-0.0.52/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.52/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    92173 2023-07-30 05:30:43.000000 py-helper-mod-0.0.52/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-30 05:31:22.674417 py-helper-mod-0.0.52/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-30 05:31:22.000000 py-helper-mod-0.0.52/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-30 05:31:22.000000 py-helper-mod-0.0.52/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-30 05:31:22.000000 py-helper-mod-0.0.52/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-30 05:31:22.000000 py-helper-mod-0.0.52/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.52/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-30 05:31:22.674417 py-helper-mod-0.0.52/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.52/setup.py
```

### Comparing `py-helper-mod-0.0.51/LICENSE` & `py-helper-mod-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.51/PKG-INFO` & `py-helper-mod-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.51
+Version: 0.0.52
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.51/py_helper.py` & `py-helper-mod-0.0.52/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1184,15 +1184,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,51)
+VERSION=(0,0,52)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1545,46 +1545,48 @@
 	message = f"Entering {msg}"
 
 	if callerframe == None:
 		callerframe = inspect.currentframe().f_back
 
 	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
 
+# Block Exit Debug Messages
+def DbgExit(msg,dbglabel=None,func=None,prefix="<--",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None):
+	"""DbgMsg Helper Function Output a message when exitting a code block"""
+
+	message = f"Exitting {msg}"
+
+	if callerframe == None:
+		callerframe = inspect.currentframe().f_back
+
+	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
+
 # Get Debug Names (Block, Label) Lambda
 DbgNames = lambda object: [ object.__qualname__, object.__name__ ]
 
 # DebugMe Decorator
 def DebugMe(func):
 	"""Debug Decorator For Enter/Exit Messages"""
 
 	@functools.wraps(func)
 	def wrapper(*args,**kwargs):
 		dbgblk, dbglb = DbgNames(func)
 
-		DbgEnter(dbgblk,dbglb)
+		callerframe = inspect.currentframe().f_back
+
+		DbgEnter(dbgblk,dbglb,callerframe=callerframe)
 
 		results = func(*args,**kwargs)
 
-		DbgExit(dbgblk,dbglb)
+		DbgExit(dbgblk,dbglb,callerframe=callerframe)
 
 		return results
 
 	return wrapper
 
-# Block Exit Debug Messages
-def DbgExit(msg,dbglabel=None,func=None,prefix="<--",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None):
-	"""DbgMsg Helper Function Output a message when exitting a code block"""
-
-	message = f"Exitting {msg}"
-
-	if callerframe == None:
-		callerframe = inspect.currentframe().f_back
-
-	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
-
 # DbgAuto Messages
 def DbgAuto(msg="Auto Dbg",prefix="[* DbgAuto *]",callerframe=None,timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,dbglabel=None):
 	"""
 	Generate an Automated DbgMsg With File-Line number and optional msg
 
 	Generally the purpose here is generate temporary debug scaffolding messages for
 	fast debugging. It is INTENDED that they will be removed once the debugging sequence
```

### Comparing `py-helper-mod-0.0.51/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.52/py_helper_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.51
+Version: 0.0.52
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.51/setup.cfg` & `py-helper-mod-0.0.52/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.51
+version = 0.0.52
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

