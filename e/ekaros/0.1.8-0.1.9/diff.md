# Comparing `tmp/ekaros-0.1.8.tar.gz` & `tmp/ekaros-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekaros-0.1.8.tar", max compression
+gzip compressed data, was "ekaros-0.1.9.tar", max compression
```

## Comparing `ekaros-0.1.8.tar` & `ekaros-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-08 04:33:55.195780 ekaros-0.1.8/LICENSE
--rw-r--r--   0        0        0     1798 2023-05-08 04:33:55.195780 ekaros-0.1.8/README.md
--rw-r--r--   0        0        0     2917 2023-05-08 04:34:18.899757 ekaros-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      287 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/__cli__.py
--rw-r--r--   0        0        0      379 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/__init__.py
--rw-r--r--   0        0        0       22 2023-05-08 04:34:18.851757 ekaros-0.1.8/src/ekaros/_version.py
--rw-r--r--   0        0        0        0 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/__init__.py
--rw-r--r--   0        0        0      222 2023-05-08 04:34:18.851757 ekaros-0.1.8/src/ekaros/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/copier/conf.yaml
--rw-r--r--   0        0        0      807 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/project/__init__.yaml
--rw-r--r--   0        0        0      196 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/project.toml
--rw-r--r--   0        0        0        0 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/py.typed
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 ekaros-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 23:11:04.334300 ekaros-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1998 2023-07-29 23:11:04.334300 ekaros-0.1.9/README.md
+-rw-r--r--   0        0        0     3073 2023-07-29 23:11:40.347582 ekaros-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-07-29 23:11:04.338300 ekaros-0.1.9/src/ekaros/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-29 23:11:04.338300 ekaros-0.1.9/src/ekaros/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-29 23:11:40.283580 ekaros-0.1.9/src/ekaros/_version.py
+-rw-r--r--   0        0        0        0 2023-07-29 23:11:04.338300 ekaros-0.1.9/src/ekaros/conf/__init__.py
+-rw-r--r--   0        0        0      178 2023-07-29 23:11:04.338300 ekaros-0.1.9/src/ekaros/conf/about/ekaros.yaml
+-rw-r--r--   0        0        0      196 2023-07-29 23:11:04.338300 ekaros-0.1.9/src/ekaros/project.toml
+-rw-r--r--   0        0        0        0 2023-07-29 23:11:04.338300 ekaros-0.1.9/src/ekaros/py.typed
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 ekaros-0.1.9/PKG-INFO
```

### Comparing `ekaros-0.1.8/LICENSE` & `ekaros-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.8/README.md` & `ekaros-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Ekaros
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/entelecheia/ekaros/branch/main/graph/badge.svg?token=PTZWYZT2X9
+[codecov-url]: https://codecov.io/gh/entelecheia/ekaros
 [pypi-image]: https://img.shields.io/pypi/v/ekaros
 [license-image]: https://img.shields.io/github/license/entelecheia/ekaros
 [license-url]: https://github.com/entelecheia/ekaros/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/ekaros?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/ekaros
 [release-url]: https://github.com/entelecheia/ekaros/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

### Comparing `ekaros-0.1.8/pyproject.toml` & `ekaros-0.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,92 @@
 [tool.poetry]
 name = "ekaros"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Python Library for Generative AI Art"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://ekaros.entelecheia.ai"
 repository = "https://github.com/entelecheia/ekaros"
 readme = "README.md"
 packages = [{ include = "ekaros", from = "src" }]
 
 [tool.poetry.scripts]
 ekaros = 'ekaros.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.4.0"
+hyfi = "^1.12.5"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
-black = "^23.1.0"
+black = ">=23.0.0,<=23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe]
 include = [".tasks.toml", ".tasks-extra.toml"]
 
 [tool.black]
-exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+exclude = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.isort]
 profile = "black"
-skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+skip = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.flake8]
 ignore = ['F401', 'E501', 'W503']
-exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "_build",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
-exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "build",
+    "_build",
+    "dist",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = true
 disallow_any_expr = false
 disallow_any_decorated = false
 disallow_any_explicit = true
@@ -82,24 +118,22 @@
 name = "cz_conventional_commits"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/ekaros/_version.py:__version__"
-version_pattern = 'src/ekaros/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
-commit_version_number = true # required for version_source = "tag"
+commit_version_number = true                                    # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-hvcs = "github" # hosting version control system, gitlab is also supported
+hvcs = "github"                                                 # hosting version control system, gitlab is also supported
 build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `ekaros-0.1.8/PKG-INFO` & `ekaros-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: ekaros
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python Library for Generative AI Art
 Home-page: https://ekaros.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.4.0,<0.5.0)
+Requires-Dist: hyfi (>=1.12.5,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/ekaros
 Description-Content-Type: text/markdown
 
 # Ekaros
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/entelecheia/ekaros/branch/main/graph/badge.svg?token=PTZWYZT2X9
+[codecov-url]: https://codecov.io/gh/entelecheia/ekaros
 [pypi-image]: https://img.shields.io/pypi/v/ekaros
 [license-image]: https://img.shields.io/github/license/entelecheia/ekaros
 [license-url]: https://github.com/entelecheia/ekaros/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/ekaros?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/ekaros
 [release-url]: https://github.com/entelecheia/ekaros/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

