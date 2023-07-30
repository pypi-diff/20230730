# Comparing `tmp/unidata-blocks-0.0.3.tar.gz` & `tmp/unidata-blocks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidata-blocks-0.0.3.tar", last modified: Thu Jun  1 03:30:11 2023, max compression
+gzip compressed data, was "unidata-blocks-0.0.4.tar", last modified: Sun Jul 30 11:31:01 2023, max compression
```

## Comparing `unidata-blocks-0.0.3.tar` & `unidata-blocks-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/src/unidata_blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks/unidata/
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/src/unidata_blocks/unidata/Blocks.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks/unidata/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/src/unidata_blocks/unidata/i18n/zh-cn.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 03:30:11.000000 unidata-blocks-0.0.3/src/unidata_blocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:30:11.085544 unidata-blocks-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-01 03:30:01.000000 unidata-blocks-0.0.3/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.009579 unidata-blocks-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:31:01.009579 unidata-blocks-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/unidata_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/src/unidata_blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/unidata_blocks/unidata/
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/src/unidata_blocks/unidata/Blocks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/src/unidata_blocks/unidata/lang-codes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-30 11:31:01.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 11:31:00.000000 unidata-blocks-0.0.4/src/unidata_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:31:01.005579 unidata-blocks-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-30 11:30:45.000000 unidata-blocks-0.0.4/tests/test_.py
```

### Comparing `unidata-blocks-0.0.3/LICENSE` & `unidata-blocks-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.3/PKG-INFO` & `unidata-blocks-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
@@ -21,25 +21,29 @@
 [![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/unidata-blocks)](https://pypi.org/project/unidata-blocks/)
 
 A library that helps query unicode blocks by [Blocks.txt](https://www.unicode.org/Public/UNIDATA/Blocks.txt).
 
 ## Installation
 
-```commandline
+```shell
 pip install unidata-blocks
 ```
 
 ## Usage
 
 ```python
 import unidata_blocks
 
 block = unidata_blocks.get_block_by_chr('A')
 assert block.code_start == 0x0000
 assert block.code_end == 0x007F
 assert block.name == 'Basic Latin'
 ```
 
+## Dependencies
+
+- [Langcodes](https://github.com/rspeer/langcodes)
+
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `unidata-blocks-0.0.3/README.md` & `unidata-blocks-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 [![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/unidata-blocks)](https://pypi.org/project/unidata-blocks/)
 
 A library that helps query unicode blocks by [Blocks.txt](https://www.unicode.org/Public/UNIDATA/Blocks.txt).
 
 ## Installation
 
-```commandline
+```shell
 pip install unidata-blocks
 ```
 
 ## Usage
 
 ```python
 import unidata_blocks
 
 block = unidata_blocks.get_block_by_chr('A')
 assert block.code_start == 0x0000
 assert block.code_end == 0x007F
 assert block.name == 'Basic Latin'
 ```
 
+## Dependencies
+
+- [Langcodes](https://github.com/rspeer/langcodes)
+
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `unidata-blocks-0.0.3/pyproject.toml` & `unidata-blocks-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "unidata-blocks"
-version = "0.0.3"
+version = "0.0.4"
 description = "A library that helps query unicode blocks by Blocks.txt."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
@@ -14,14 +14,18 @@
 keywords = ["unicode"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "langcodes>=3.3.0",
+]
+
 [project.urls]
 homepage = "https://github.com/TakWolf/unidata-blocks"
 source = "https://github.com/TakWolf/unidata-blocks"
 issues = "https://github.com/TakWolf/unidata-blocks/issues"
 
 [tool.setuptools]
 package-data = { "unidata_blocks" = ["unidata/*.txt", "unidata/i18n/*.txt"] }
```

### Comparing `unidata-blocks-0.0.3/src/unidata_blocks/unidata/Blocks.txt` & `unidata-blocks-0.0.4/src/unidata_blocks/unidata/Blocks.txt`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.3/src/unidata_blocks.egg-info/PKG-INFO` & `unidata-blocks-0.0.4/src/unidata_blocks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
@@ -21,25 +21,29 @@
 [![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/unidata-blocks)](https://pypi.org/project/unidata-blocks/)
 
 A library that helps query unicode blocks by [Blocks.txt](https://www.unicode.org/Public/UNIDATA/Blocks.txt).
 
 ## Installation
 
-```commandline
+```shell
 pip install unidata-blocks
 ```
 
 ## Usage
 
 ```python
 import unidata_blocks
 
 block = unidata_blocks.get_block_by_chr('A')
 assert block.code_start == 0x0000
 assert block.code_end == 0x007F
 assert block.name == 'Basic Latin'
 ```
 
+## Dependencies
+
+- [Langcodes](https://github.com/rspeer/langcodes)
+
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `unidata-blocks-0.0.3/tests/test_query.py` & `unidata-blocks-0.0.4/tests/test_.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,14 @@
     assert str(block) == '100000..10FFFF; Supplementary Private Use Area-B'
 
 
 def test_i18n():
     block = unidata_blocks.get_block_by_code_point(0x0000)
     assert block.name_localized('en') == 'Basic Latin'
     assert block.name_localized('EN') == 'Basic Latin'
+    assert block.name_localized('zh') == '基本拉丁'
+    assert block.name_localized('ZH') == '基本拉丁'
+    assert block.name_localized('zh-hans') == '基本拉丁'
+    assert block.name_localized('zh-chs') == '基本拉丁'
     assert block.name_localized('zh-cn') == '基本拉丁'
-    assert block.name_localized('ZH_CN') == '基本拉丁'
-    assert block.name_localized('no-locale') is None
-
-    block = unidata_blocks.get_block_by_code_point(0x4E00)
-    assert block.name_localized('en') == 'CJK Unified Ideographs'
-    assert block.name_localized('EN') == 'CJK Unified Ideographs'
-    assert block.name_localized('zh-cn') == '中日韩统一表意文字'
-    assert block.name_localized('ZH_CN') == '中日韩统一表意文字'
-    assert block.name_localized('no-locale') is None
+    assert block.name_localized('no-language') is None
+    assert block.name_localized('no-language', 'abc') == 'abc'
```

