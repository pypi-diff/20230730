# Comparing `tmp/thematos-0.2.1.tar.gz` & `tmp/thematos-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thematos-0.2.1.tar", max compression
+gzip compressed data, was "thematos-0.2.2.tar", max compression
```

## Comparing `thematos-0.2.1.tar` & `thematos-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-07-28 06:55:54.395306 thematos-0.2.1/LICENSE
--rw-r--r--   0        0        0     2112 2023-07-28 06:55:54.395306 thematos-0.2.1/README.md
--rw-r--r--   0        0        0     3118 2023-07-28 06:56:20.383753 thematos-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/__init__.py
--rw-r--r--   0        0        0       21 2023-07-28 06:56:20.339752 thematos-0.2.1/src/thematos/_version.py
--rw-r--r--   0        0        0        0 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/conf/__init__.py
--rw-r--r--   0        0        0      179 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/conf/about/thematos.yaml
--rw-r--r--   0        0        0        0 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/conf/topic/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/py.typed
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 thematos-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-30 11:22:41.525165 thematos-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2112 2023-07-30 11:22:41.525165 thematos-0.2.2/README.md
+-rw-r--r--   0        0        0     3118 2023-07-30 11:23:11.381886 thematos-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-30 11:22:41.529165 thematos-0.2.2/src/thematos/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-30 11:22:41.529165 thematos-0.2.2/src/thematos/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-30 11:23:11.333885 thematos-0.2.2/src/thematos/_version.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:22:41.529165 thematos-0.2.2/src/thematos/conf/__init__.py
+-rw-r--r--   0        0        0      179 2023-07-30 11:22:41.529165 thematos-0.2.2/src/thematos/conf/about/thematos.yaml
+-rw-r--r--   0        0        0        0 2023-07-30 11:22:41.529165 thematos-0.2.2/src/thematos/conf/topic/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-30 11:22:41.529165 thematos-0.2.2/src/thematos/py.typed
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 thematos-0.2.2/PKG-INFO
```

### Comparing `thematos-0.2.1/LICENSE` & `thematos-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thematos-0.2.1/README.md` & `thematos-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `thematos-0.2.1/pyproject.toml` & `thematos-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "thematos"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python Library for Topic Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://thematos.entelecheia.ai"
 repository = "https://github.com/entelecheia/thematos"
 readme = "README.md"
 packages = [{ include = "thematos", from = "src" }]
 
 [tool.poetry.scripts]
 thematos = 'thematos.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.12.0"
+hyfi = "^1.12.5"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `thematos-0.2.1/PKG-INFO` & `thematos-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thematos
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python Library for Topic Modeling
 Home-page: https://thematos.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.12.0,<2.0.0)
+Requires-Dist: hyfi (>=1.12.5,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/thematos
 Description-Content-Type: text/markdown
 
 # ThematOS
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

