# Comparing `tmp/aibasics-0.2.2.tar.gz` & `tmp/aibasics-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibasics-0.2.2.tar", max compression
+gzip compressed data, was "aibasics-0.2.3.tar", max compression
```

## Comparing `aibasics-0.2.2.tar` & `aibasics-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,10 @@
--rw-r--r--   0        0        0    18656 2023-04-26 08:37:55.616187 aibasics-0.2.2/LICENSE
--rw-r--r--   0        0        0     2049 2023-04-26 08:37:55.616187 aibasics-0.2.2/README.md
--rw-r--r--   0        0        0     3236 2023-04-26 08:38:24.428229 aibasics-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      176 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/__cli__.py
--rw-r--r--   0        0        0      889 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/__init__.py
--rw-r--r--   0        0        0       22 2023-04-26 08:38:24.376229 aibasics-0.2.2/src/aibasics/_version.py
--rw-r--r--   0        0        0        0 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/__init__.py
--rw-r--r--   0        0        0      326 2023-04-26 08:38:24.376229 aibasics-0.2.2/src/aibasics/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/conf/task/__init__.yaml
--rw-r--r--   0        0        0        0 2023-04-26 08:37:55.620187 aibasics-0.2.2/src/aibasics/py.typed
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 aibasics-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    18656 2023-07-30 04:34:44.630255 aibasics-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2245 2023-07-30 04:34:44.630255 aibasics-0.2.3/README.md
+-rw-r--r--   0        0        0     2904 2023-07-30 04:35:13.527998 aibasics-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-30 04:34:44.634255 aibasics-0.2.3/src/aibasics/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-30 04:34:44.634255 aibasics-0.2.3/src/aibasics/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 04:35:13.467995 aibasics-0.2.3/src/aibasics/_version.py
+-rw-r--r--   0        0        0        0 2023-07-30 04:34:44.634255 aibasics-0.2.3/src/aibasics/conf/__init__.py
+-rw-r--r--   0        0        0      212 2023-07-30 04:34:44.634255 aibasics-0.2.3/src/aibasics/conf/about/aibasics.yaml
+-rw-r--r--   0        0        0        0 2023-07-30 04:34:44.634255 aibasics-0.2.3/src/aibasics/py.typed
+-rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 aibasics-0.2.3/PKG-INFO
```

### Comparing `aibasics-0.2.2/LICENSE` & `aibasics-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aibasics-0.2.2/README.md` & `aibasics-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # AI Uncovered
 
 [![pypi-image]][pypi-url]
-[![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
+[![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/chu-aie/aibasics/branch/main/graph/badge.svg?token=dzfp4tGZ87
+[codecov-url]: https://codecov.io/gh/chu-aie/aibasics
 [pypi-image]: https://img.shields.io/pypi/v/aibasics
 [license-image]: https://img.shields.io/github/license/chu-aie/aibasics
 [license-url]: https://github.com/chu-aie/aibasics/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/chu-aie/aibasics?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/chu-aie/aibasics
 [release-url]: https://github.com/chu-aie/aibasics/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

### Comparing `aibasics-0.2.2/pyproject.toml` & `aibasics-0.2.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,57 @@
 [tool.poetry]
 name = "aibasics"
-version = "0.2.2"
+version = "0.2.3"
 description = "AI Uncovered: A Comprehensive Guide to AI Basics and Applications"
-authors = [
-    "Yongjun Chang <yongnjin@chu.ac.kr>",
-    "Sungjin Kim <r3dzon3@chu.ac.kr>",
-    "Young Joon Lee <yj.lee@chu.ac.kr>",
-]
+authors = ["Young Joon Lee <yj.lee@chu.ac.kr>"]
 license = "CC-BY-4.0"
 homepage = "https://aibasics.entelecheia.ai"
 repository = "https://github.com/chu-aie/aibasics"
 readme = "README.md"
 packages = [{ include = "aibasics", from = "src" }]
 
 [tool.poetry.scripts]
 aibasics = 'aibasics.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.20"
+click = "^8.1.3"
+hyfi = "^1.12.5"
+
+[tool.poetry.group.dev]
+optional = true
 
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
-ipykernel = "^6.22.0"
+
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
 
 [tool.black]
-exclude = [
-    '_version.py',
-    'node_modules',
-    '_build',
-    'docs',
-    'tests',
-    'venv',
-    '.copier-template',
-    '.refs',
-]
+exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
-skip = [
-    '_version.py',
-    'node_modules',
-    '_build',
-    'docs',
-    'tests',
-    'venv',
-    '.copier-template',
-    '.refs',
-]
+skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.flake8]
 ignore = ['F401', 'E501', 'W503']
-exclude = [
-    "node_modules",
-    "_build",
-    "docs",
-    "tests",
-    "venv",
-    ".copier-template",
-    ".refs",
-]
+exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
-exclude = [
-    "node_modules",
-    "build",
-    "_build",
-    "dist",
-    "docs",
-    "tests",
-    "venv",
-    ".copier-template",
-    ".refs",
-]
+exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = true
 disallow_any_expr = false
 disallow_any_decorated = false
 disallow_any_explicit = true
@@ -111,30 +77,29 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/aibasics/_version.py:__version__"
-version_pattern = 'src/aibasics/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
-commit_version_number = true                                                   # required for version_source = "tag"
+commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
+hvcs = "github" # hosting version control system, gitlab is also supported
 build_command = "poetry build --no-cache"
-hvcs = "github"                                                                # hosting version control system, gitlab is also supported
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `aibasics-0.2.2/PKG-INFO` & `aibasics-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: aibasics
-Version: 0.2.2
+Version: 0.2.3
 Summary: AI Uncovered: A Comprehensive Guide to AI Basics and Applications
 Home-page: https://aibasics.entelecheia.ai
 License: CC-BY-4.0
-Author: Yongjun Chang
-Author-email: yongnjin@chu.ac.kr
+Author: Young Joon Lee
+Author-email: yj.lee@chu.ac.kr
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.20,<0.3.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: hyfi (>=1.12.5,<2.0.0)
 Project-URL: Repository, https://github.com/chu-aie/aibasics
 Description-Content-Type: text/markdown
 
 # AI Uncovered
 
 [![pypi-image]][pypi-url]
-[![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
+[![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/chu-aie/aibasics/branch/main/graph/badge.svg?token=dzfp4tGZ87
+[codecov-url]: https://codecov.io/gh/chu-aie/aibasics
 [pypi-image]: https://img.shields.io/pypi/v/aibasics
 [license-image]: https://img.shields.io/github/license/chu-aie/aibasics
 [license-url]: https://github.com/chu-aie/aibasics/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/chu-aie/aibasics?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/chu-aie/aibasics
 [release-url]: https://github.com/chu-aie/aibasics/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

