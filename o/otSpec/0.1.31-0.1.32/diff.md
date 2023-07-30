# Comparing `tmp/otSpec-0.1.31.tar.gz` & `tmp/otSpec-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otSpec-0.1.31.tar", last modified: Sun Jan  1 15:35:33 2023, max compression
+gzip compressed data, was "otSpec-0.1.32.tar", last modified: Sun Jul 30 12:58:52 2023, max compression
```

## Comparing `otSpec-0.1.31.tar` & `otSpec-0.1.32.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.770860 otSpec-0.1.31/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-01-01 15:35:32.000000 otSpec-0.1.31/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.762860 otSpec-0.1.31/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.764860 otSpec-0.1.31/Lib/otSpec/
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.766860 otSpec-0.1.31/Lib/otSpec/cpg/
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/cpg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   194505 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/cpg/data.txt
--rw-rw-rw-   0 root         (0) root         (0)     4219 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/cpg/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.769860 otSpec-0.1.31/Lib/otSpec/table/
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/GPOS.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/GSUB.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/MVAR.py
--rw-rw-rw-   0 root         (0) root         (0)    29194 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/OS2.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/STAT.py
--rw-rw-rw-   0 root         (0) root         (0)     4004 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/gasp.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/head.py
--rw-rw-rw-   0 root         (0) root         (0)    12172 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/table/name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.770860 otSpec-0.1.31/Lib/otSpec/tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28084 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/tag/feature.py
--rw-rw-rw-   0 root         (0) root         (0)    13260 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/tag/language.py
--rw-rw-rw-   0 root         (0) root         (0)     4294 2023-01-01 15:35:32.000000 otSpec-0.1.31/Lib/otSpec/tag/script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-01 15:35:33.765860 otSpec-0.1.31/Lib/otSpec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1434 2023-01-01 15:35:33.000000 otSpec-0.1.31/Lib/otSpec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      594 2023-01-01 15:35:33.000000 otSpec-0.1.31/Lib/otSpec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-01 15:35:33.000000 otSpec-0.1.31/Lib/otSpec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-01 15:35:33.000000 otSpec-0.1.31/Lib/otSpec.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1434 2023-01-01 15:35:33.770860 otSpec-0.1.31/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-01-01 15:35:33.771860 otSpec-0.1.31/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-01-01 15:35:32.000000 otSpec-0.1.31/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.463755 otSpec-0.1.32/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-30 12:58:51.000000 otSpec-0.1.32/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.458754 otSpec-0.1.32/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.459755 otSpec-0.1.32/Lib/otSpec/
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.460754 otSpec-0.1.32/Lib/otSpec/cpg/
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/cpg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   194505 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/cpg/data.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4219 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/cpg/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.462754 otSpec-0.1.32/Lib/otSpec/table/
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/GPOS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/GSUB.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/MVAR.py
+-rw-rw-rw-   0 root         (0) root         (0)    29247 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/OS2.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/STAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     4004 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/gasp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/head.py
+-rw-rw-rw-   0 root         (0) root         (0)    12172 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/table/name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.462754 otSpec-0.1.32/Lib/otSpec/tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28084 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/tag/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)    13260 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/tag/language.py
+-rw-rw-rw-   0 root         (0) root         (0)     4294 2023-07-30 12:58:51.000000 otSpec-0.1.32/Lib/otSpec/tag/script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:58:52.459755 otSpec-0.1.32/Lib/otSpec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-30 12:58:52.000000 otSpec-0.1.32/Lib/otSpec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-30 12:58:52.000000 otSpec-0.1.32/Lib/otSpec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 12:58:52.000000 otSpec-0.1.32/Lib/otSpec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-30 12:58:52.000000 otSpec-0.1.32/Lib/otSpec.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-30 12:58:52.463755 otSpec-0.1.32/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-30 12:58:52.463755 otSpec-0.1.32/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-07-30 12:58:51.000000 otSpec-0.1.32/setup.py
```

### Comparing `otSpec-0.1.31/LICENSE` & `otSpec-0.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/cpg/data.txt` & `otSpec-0.1.32/Lib/otSpec/cpg/data.txt`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/cpg/update.py` & `otSpec-0.1.32/Lib/otSpec/cpg/update.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/table/GPOS.py` & `otSpec-0.1.32/Lib/otSpec/table/GPOS.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/table/GSUB.py` & `otSpec-0.1.32/Lib/otSpec/table/GSUB.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/table/MVAR.py` & `otSpec-0.1.32/Lib/otSpec/table/MVAR.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/table/OS2.py` & `otSpec-0.1.32/Lib/otSpec/table/OS2.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     | fsSelection_USE_TYPO_METRICS
     | fsSelection_WWS
     | fsSelection_OBLIQUE
 )
 
 
 def get_fsSelection_mask(OS2table):
+    """
+    Mask for valid fsSelection bits.
+    """
     if 0 <= OS2table.version <= 3:
         return fsSelection_OS2_v3_mask
     if 4 <= OS2table.version <= 5:
         return fsSelection_OS2_v4_mask
 
 
 fsSelectionToStyleNameMap = {
```

### Comparing `otSpec-0.1.31/Lib/otSpec/table/__init__.py` & `otSpec-0.1.32/Lib/otSpec/table/__init__.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/table/head.py` & `otSpec-0.1.32/Lib/otSpec/table/head.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/table/name.py` & `otSpec-0.1.32/Lib/otSpec/table/name.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/tag/feature.py` & `otSpec-0.1.32/Lib/otSpec/tag/feature.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/tag/language.py` & `otSpec-0.1.32/Lib/otSpec/tag/language.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec/tag/script.py` & `otSpec-0.1.32/Lib/otSpec/tag/script.py`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/Lib/otSpec.egg-info/PKG-INFO` & `otSpec-0.1.32/Lib/otSpec.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: otSpec
-Version: 0.1.31
+Version: 0.1.32
 Summary: Useful constants for OpenType.
-Home-page: https://gitlab.com/fontstuff/ot
+Home-page: https://gitlab.com/fontstuff/otSpec
 Author: Andreas Eigendorf
+License: MIT
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `otSpec-0.1.31/Lib/otSpec.egg-info/SOURCES.txt` & `otSpec-0.1.32/Lib/otSpec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otSpec-0.1.31/PKG-INFO` & `otSpec-0.1.32/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: otSpec
-Version: 0.1.31
+Version: 0.1.32
 Summary: Useful constants for OpenType.
-Home-page: https://gitlab.com/fontstuff/ot
+Home-page: https://gitlab.com/fontstuff/otSpec
 Author: Andreas Eigendorf
+License: MIT
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `otSpec-0.1.31/setup.cfg` & `otSpec-0.1.32/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [bumpversion]
-current_version = 0.1.31
+current_version = 0.1.32
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
 [metadata]
 name = otSpec
 author = Andreas Eigendorf
 description = Useful constants for OpenType.
-url = https://gitlab.com/fontstuff/ot
+url = https://gitlab.com/fontstuff/otSpec
 long_description = file: readme.md
 long_description_content_type = text/markdown
+license = MIT
+license_files = LICENSE
 platforms = Any
 classifiers = 
 	Development Status :: 3 - Alpha
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
@@ -32,11 +34,16 @@
 [options]
 python_requires = >=3.7
 
 [bumpversion:file:Lib/otSpec/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
+[tool:pytest]
+junit_family = legacy
+testpaths = 
+	tests
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `otSpec-0.1.31/setup.py` & `otSpec-0.1.32/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,13 @@
     with open("Lib/otSpec/__init__.py", "r", encoding="utf-8") as f:
         for line in f:
             if line.startswith("__version__"):
                 return ast.parse(line).body[0].value.s
         raise RuntimeError("No __version__ string found!")
 
 
-with open("readme.md", "r") as f:
-    long_description = f.read()
-
 setup(
     version=_get_version(),
     package_dir={"": "Lib"},
     packages=find_packages("Lib"),
     package_data={"": ["cpg/data.txt"]},
 )
```

