# Comparing `tmp/poetry-githooks-2.0.0.tar.gz` & `tmp/poetry_githooks-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-githooks-2.0.0.tar", max compression
+gzip compressed data, was "poetry_githooks-2.0.1.tar", max compression
```

## Comparing `poetry-githooks-2.0.0.tar` & `poetry_githooks-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1072 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/LICENSE
--rw-r--r--   0        0        0      571 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/README.md
--rw-r--r--   0        0        0     1183 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/poetry_githooks/__init__.py
--rw-r--r--   0        0        0      999 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/poetry_githooks/helpers.py
--rw-r--r--   0        0        0     1860 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/poetry_githooks/hooks.py
--rw-r--r--   0        0        0     1181 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/poetry_githooks/settings.py
--rw-r--r--   0        0        0     1353 2022-02-06 18:36:16.740360 poetry-githooks-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1411 2022-02-06 18:36:37.068453 poetry-githooks-2.0.0/setup.py
--rw-r--r--   0        0        0     1710 2022-02-06 18:36:37.068748 poetry-githooks-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/LICENSE
+-rw-r--r--   0        0        0      571 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/README.md
+-rw-r--r--   0        0        0     1183 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/poetry_githooks/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/poetry_githooks/helpers.py
+-rw-r--r--   0        0        0     1860 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/poetry_githooks/hooks.py
+-rw-r--r--   0        0        0     1181 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/poetry_githooks/settings.py
+-rw-r--r--   0        0        0     1253 2023-07-30 18:39:52.405484 poetry_githooks-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 poetry_githooks-2.0.1/PKG-INFO
```

### Comparing `poetry-githooks-2.0.0/LICENSE` & `poetry_githooks-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-githooks-2.0.0/README.md` & `poetry_githooks-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry-githooks-2.0.0/poetry_githooks/__init__.py` & `poetry_githooks-2.0.1/poetry_githooks/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-githooks-2.0.0/poetry_githooks/helpers.py` & `poetry_githooks-2.0.1/poetry_githooks/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-githooks-2.0.0/poetry_githooks/hooks.py` & `poetry_githooks-2.0.1/poetry_githooks/hooks.py`

 * *Files identical despite different names*

### Comparing `poetry-githooks-2.0.0/poetry_githooks/settings.py` & `poetry_githooks-2.0.1/poetry_githooks/settings.py`

 * *Files identical despite different names*

### Comparing `poetry-githooks-2.0.0/pyproject.toml` & `poetry_githooks-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-githooks"
-version = "2.0.0"
+version = "2.0.1"
 description = "Simple git hooks with poetry"
 authors = ["Thomas Thiebaud <thiebaud.tom@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thomasthiebaud/poetry-githooks"
 repository = "https://github.com/thomasthiebaud/poetry-githooks"
 documentation = "https://github.com/thomasthiebaud/poetry-githooks"
@@ -19,30 +19,26 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.6.2"
 toml = "^0.10.2"
 click = "^8.0.3"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
-mamba = "^0.11.2"
-taskipy = "^1.9.0"
 
 [tool.poetry.scripts]
 githooks = "poetry_githooks:cli"
 
-[tool.taskipy.tasks]
-lint = "black ."
-"lint:check" = "black . --check"
-test = "mamba --format=documentation tests/*"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.0.0"
 
 [tool.githooks]
 pre-commit = "black . --check"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `poetry-githooks-2.0.0/PKG-INFO` & `poetry_githooks-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: poetry-githooks
-Version: 2.0.0
+Version: 2.0.1
 Summary: Simple git hooks with poetry
 Home-page: https://github.com/thomasthiebaud/poetry-githooks
 License: MIT
 Keywords: git,hook,githooks,poetry
 Author: Thomas Thiebaud
 Author-email: thiebaud.tom@gmail.com
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.6.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://github.com/thomasthiebaud/poetry-githooks
 Project-URL: Repository, https://github.com/thomasthiebaud/poetry-githooks
 Description-Content-Type: text/markdown
```

