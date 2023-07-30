# Comparing `tmp/unidata-blocks-0.0.4.tar.gz` & `tmp/unidata-blocks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidata-blocks-0.0.4.tar", last modified: Sun Jul 30 11:31:01 2023, max compression
+gzip compressed data, was "unidata-blocks-0.0.5.tar", last modified: Sun Jul 30 17:52:06 2023, max compression
```

## Comparing `unidata-blocks-0.0.4.tar` & `unidata-blocks-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.009579 unidata-blocks-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:31:01.009579 unidata-blocks-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/unidata_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/src/unidata_blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/unidata_blocks/unidata/
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/src/unidata_blocks/unidata/Blocks.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/src/unidata_blocks/unidata/lang-codes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-30 11:31:01.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.841655 unidata-blocks-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 17:52:06.841655 unidata-blocks-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:52:06.841655 unidata-blocks-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.837655 unidata-blocks-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.837655 unidata-blocks-0.0.5/src/unidata_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/src/unidata_blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.841655 unidata-blocks-0.0.5/src/unidata_blocks/unidata/
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/src/unidata_blocks/unidata/Blocks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/src/unidata_blocks/unidata/lang-codes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.841655 unidata-blocks-0.0.5/src/unidata_blocks/unidata/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/src/unidata_blocks/unidata/translations/zh-hans.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.837655 unidata-blocks-0.0.5/src/unidata_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 17:52:06.000000 unidata-blocks-0.0.5/src/unidata_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-30 17:52:06.000000 unidata-blocks-0.0.5/src/unidata_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:52:06.000000 unidata-blocks-0.0.5/src/unidata_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 17:52:06.000000 unidata-blocks-0.0.5/src/unidata_blocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 17:52:06.000000 unidata-blocks-0.0.5/src/unidata_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:52:06.841655 unidata-blocks-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-30 17:51:56.000000 unidata-blocks-0.0.5/tests/test_.py
```

### Comparing `unidata-blocks-0.0.4/LICENSE` & `unidata-blocks-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.4/PKG-INFO` & `unidata-blocks-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
```

### Comparing `unidata-blocks-0.0.4/README.md` & `unidata-blocks-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.4/pyproject.toml` & `unidata-blocks-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "unidata-blocks"
-version = "0.0.4"
+version = "0.0.5"
 description = "A library that helps query unicode blocks by Blocks.txt."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
@@ -24,13 +24,13 @@
 
 [project.urls]
 homepage = "https://github.com/TakWolf/unidata-blocks"
 source = "https://github.com/TakWolf/unidata-blocks"
 issues = "https://github.com/TakWolf/unidata-blocks/issues"
 
 [tool.setuptools]
-package-data = { "unidata_blocks" = ["unidata/*.txt", "unidata/i18n/*.txt"] }
+package-data = { "unidata_blocks" = ["unidata/*.txt", "unidata/translations/*.txt"] }
 
 [tool.pytest.ini_options]
 pythonpath = [
     "src",
 ]
```

### Comparing `unidata-blocks-0.0.4/src/unidata_blocks/__init__.py` & `unidata-blocks-0.0.5/src/unidata_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.4/src/unidata_blocks/unidata/Blocks.txt` & `unidata-blocks-0.0.5/src/unidata_blocks/unidata/Blocks.txt`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.4/src/unidata_blocks.egg-info/PKG-INFO` & `unidata-blocks-0.0.5/src/unidata_blocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
```

### Comparing `unidata-blocks-0.0.4/tests/test_.py` & `unidata-blocks-0.0.5/tests/test_.py`

 * *Files identical despite different names*

