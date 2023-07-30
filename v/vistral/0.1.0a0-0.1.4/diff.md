# Comparing `tmp/vistral-0.1.0a0.tar.gz` & `tmp/vistral-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vistral-0.1.0a0.tar", max compression
+gzip compressed data, was "vistral-0.1.4.tar", max compression
```

## Comparing `vistral-0.1.0a0.tar` & `vistral-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0       61 2023-03-31 15:23:09.812323 vistral-0.1.0a0/README.md
--rw-r--r--   0        0        0     1643 2023-04-07 07:31:03.558155 vistral-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 10:31:25.445651 vistral-0.1.0a0/src/vistral/__init__.py
--rw-r--r--   0        0        0       20 2023-04-07 07:27:43.950826 vistral-0.1.0a0/src/vistral/__version__.py
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 vistral-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      411 2023-07-30 16:06:46.185463 vistral-0.1.4/README.md
+-rw-r--r--   0        0        0     1781 2023-07-30 16:06:46.185463 vistral-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-30 16:06:46.185463 vistral-0.1.4/src/vistral/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-30 16:06:46.185463 vistral-0.1.4/src/vistral/__version__.py
+-rw-r--r--   0        0        0     1106 2023-07-30 16:06:46.185463 vistral-0.1.4/src/vistral/command_bus/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-30 16:06:46.185463 vistral-0.1.4/src/vistral/command_bus/command.py
+-rw-r--r--   0        0        0      423 2023-07-30 16:06:46.189463 vistral-0.1.4/src/vistral/command_bus/exceptions.py
+-rw-r--r--   0        0        0      446 2023-07-30 16:06:46.189463 vistral-0.1.4/src/vistral/command_bus/resolver.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:06:46.189463 vistral-0.1.4/src/vistral/contrib/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-30 16:06:46.189463 vistral-0.1.4/src/vistral/contrib/lagom.py
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 vistral-0.1.4/PKG-INFO
```

### Comparing `vistral-0.1.0a0/pyproject.toml` & `vistral-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
-version = "0.1.0a0"
+version = "0.1.4"
 version_files = ["pyproject.toml:version", "src/vistral/__version__.py"]
 
 [tool.coverage.report]
 exclude_lines = [
   "def __repr__",
   "def __str__",
   "if TYPE_CHECKING:",
@@ -43,41 +43,47 @@
 check_untyped_defs = true
 disallow_any_unimported = true
 disallow_untyped_defs = true
 exclude = [
   "(^|/)tests/"
 ]
 no_implicit_optional = true
-plugins = [
-  "vistral.contrib.mypy"
-]
 show_error_codes = true
 warn_return_any = true
 warn_unused_ignores = true
 
 [tool.poetry]
 authors = ["Łukasz Wolak"]
 description = ""
+exclude = ["**/conftest.py", "**/tests/**/*"]
 name = "vistral"
 packages = [{from = "src", include = "vistral"}]
 readme = "README.md"
-version = "0.1.0a0"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+lagom = {optional = true, version = "^2.4.1"}
 
-[tool.poetry.group.contrib-lagom]
-optional = true
-
-[tool.poetry.group.contrib-lagom.dependencies]
-lagom = "^2.4.1"
+[tool.poetry.extras]
+lagom = ["lagom"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 commitizen = "^2.42.1"
 import-linter = "^1.8.0"
 isort = "^5.12.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pyupgrade = "^3.3.1"
+ruff = ">=0.0.262, <0.1.0"
 toml-sort = "^0.23.0"
+
+[tool.ruff]
+line-length = 120
+src = ["src"]
+
+[tool.tomlsort]
+all = true
+in_place = true
+sort_first = ["tool.poetry.dependencies.python"]
```

