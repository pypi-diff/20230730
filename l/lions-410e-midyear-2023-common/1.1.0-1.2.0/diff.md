# Comparing `tmp/lions_410e_midyear_2023_common-1.1.0.tar.gz` & `tmp/lions_410e_midyear_2023_common-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions_410e_midyear_2023_common-1.1.0.tar", max compression
+gzip compressed data, was "lions_410e_midyear_2023_common-1.2.0.tar", max compression
```

## Comparing `lions_410e_midyear_2023_common-1.1.0.tar` & `lions_410e_midyear_2023_common-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2021-11-21 15:16:13.135043 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/__init__.py
--rw-r--r--   0        0        0     1590 2022-06-22 13:09:03.440647 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/build_pdf.py
--rw-r--r--   0        0        0       44 2023-07-30 14:20:03.676267 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/constants.py
--rw-r--r--   0        0        0      375 2023-07-27 18:25:20.428828 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/data.json
--rw-r--r--   0        0        0     1750 2022-07-05 15:11:28.452005 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/emailer.py
--rw-r--r--   0        0        0     1042 2022-08-21 15:45:01.177687 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/models.py
--rw-r--r--   0        0        0      933 2022-06-21 17:50:18.027424 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/sqs.py
--rw-r--r--   0        0        0   916941 2022-06-24 18:59:51.866568 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/test.pdf
--rw-r--r--   0        0        0      359 2021-11-21 15:06:03.434257 lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/test.py
--rw-r--r--   0        0        0      643 2023-07-30 14:20:57.998404 lions_410e_midyear_2023_common-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      229 2022-06-19 12:19:59.092856 lions_410e_midyear_2023_common-1.1.0/readme.md
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 lions_410e_midyear_2023_common-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2021-11-21 15:16:13.135043 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/__init__.py
+-rw-r--r--   0        0        0     1590 2023-07-30 18:20:28.805939 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/build_pdf.py
+-rw-r--r--   0        0        0       44 2023-07-30 14:20:03.676267 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/constants.py
+-rw-r--r--   0        0        0      375 2023-07-27 18:25:20.428828 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/data.json
+-rw-r--r--   0        0        0     1750 2022-07-05 15:11:28.452005 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/emailer.py
+-rw-r--r--   0        0        0     1042 2022-08-21 15:45:01.177687 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/models.py
+-rw-r--r--   0        0        0      933 2022-06-21 17:50:18.027424 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/sqs.py
+-rw-r--r--   0        0        0   916941 2022-06-24 18:59:51.866568 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/test.pdf
+-rw-r--r--   0        0        0      359 2021-11-21 15:06:03.434257 lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/test.py
+-rw-r--r--   0        0        0      643 2023-07-30 18:20:44.045413 lions_410e_midyear_2023_common-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      229 2022-06-19 12:19:59.092856 lions_410e_midyear_2023_common-1.2.0/readme.md
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 lions_410e_midyear_2023_common-1.2.0/PKG-INFO
```

### Comparing `lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/build_pdf.py` & `lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/build_pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __version__ = "0.0.1"
 import os.path
 
 import click
 import docker
 from rich import print
 
-IMAGE = "registry.gitlab.com/lions-410e-midyear-2022/pdf-creator:main"
+IMAGE = "registry.gitlab.com/lions-410e-midyear-2023/pdf-creator:main"
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 def build_pdf(source_dir, source_file, pull=False, debug=False):
     """Read SOURCE_FILE from SOURCE_DIR and write an equivalently named PDF file to SOURCE_DIR"""
     client = docker.from_env()
```

### Comparing `lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/emailer.py` & `lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/emailer.py`

 * *Files identical despite different names*

### Comparing `lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/models.py` & `lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/models.py`

 * *Files identical despite different names*

### Comparing `lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/sqs.py` & `lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/sqs.py`

 * *Files identical despite different names*

### Comparing `lions_410e_midyear_2023_common-1.1.0/lions_410e_midyear_2023_common/test.pdf` & `lions_410e_midyear_2023_common-1.2.0/lions_410e_midyear_2023_common/test.pdf`

 * *Files identical despite different names*

### Comparing `lions_410e_midyear_2023_common-1.1.0/pyproject.toml` & `lions_410e_midyear_2023_common-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lions_410e_midyear_2023_common"
-version = "1.1.0"
+version = "1.2.0"
 description = "Common libraries for applications related to the 2023 Lions District 410E Midyear Conference"
 authors = ["Kim van Wyk <vanwykk@gmail.com>"]
 repository = "https://gitlab.com/410e-midyear-2023/common"
 readme = "readme.md" 
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `lions_410e_midyear_2023_common-1.1.0/PKG-INFO` & `lions_410e_midyear_2023_common-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions-410e-midyear-2023-common
-Version: 1.1.0
+Version: 1.2.0
 Summary: Common libraries for applications related to the 2023 Lions District 410E Midyear Conference
 Home-page: https://gitlab.com/410e-midyear-2023/common
 Author: Kim van Wyk
 Author-email: vanwykk@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

