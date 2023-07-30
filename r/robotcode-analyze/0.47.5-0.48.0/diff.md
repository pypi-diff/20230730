# Comparing `tmp/robotcode_analyze-0.47.5.tar.gz` & `tmp/robotcode_analyze-0.48.0.tar.gz`

## Comparing `robotcode_analyze-0.47.5.tar` & `robotcode_analyze-0.48.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/src/robotcode/analyze/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/src/robotcode/analyze/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/src/robotcode/analyze/__version__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/src/robotcode/analyze/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/src/robotcode/analyze/py.typed
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/src/robotcode/analyze/cli/__init__.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/LICENSE.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/README.md
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/pyproject.toml
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 robotcode_analyze-0.47.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/src/robotcode/analyze/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/src/robotcode/analyze/__version__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/src/robotcode/analyze/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/src/robotcode/analyze/py.typed
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/src/robotcode/analyze/cli/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/LICENSE.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/README.md
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/pyproject.toml
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 robotcode_analyze-0.48.0/PKG-INFO
```

### Comparing `robotcode_analyze-0.47.5/src/robotcode/analyze/cli/__init__.py` & `robotcode_analyze-0.48.0/src/robotcode/analyze/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.47.5/.gitignore` & `robotcode_analyze-0.48.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.47.5/LICENSE.txt` & `robotcode_analyze-0.48.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.47.5/README.md` & `robotcode_analyze-0.48.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_analyze-0.47.5/pyproject.toml` & `robotcode_analyze-0.48.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,17 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-plugin==0.47.5",
-  "robotcode-robot==0.47.5",
+  "robotcode-plugin==0.48.0",
+  "robotcode-robot==0.48.0",
+  "robotcode==0.48.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 analyze = "robotcode.analyze.hooks"
 
 [project.urls]
```

### Comparing `robotcode_analyze-0.47.5/PKG-INFO` & `robotcode_analyze-0.48.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-analyze
-Version: 0.47.5
+Version: 0.48.0
 Summary: RobotCode analyze plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-plugin==0.47.5
-Requires-Dist: robotcode-robot==0.47.5
+Requires-Dist: robotcode-plugin==0.48.0
+Requires-Dist: robotcode-robot==0.48.0
+Requires-Dist: robotcode==0.48.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-analyze
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-analyze.svg)](https://pypi.org/project/robotcode-analyze)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-analyze.svg)](https://pypi.org/project/robotcode-analyze)
```

