# Comparing `tmp/whool-0.2.1.tar.gz` & `tmp/whool-0.2.2.tar.gz`

## Comparing `whool-0.2.1.tar` & `whool-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 whool-0.2.1/.flake8
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 whool-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 whool-0.2.1/TODO
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 whool-0.2.1/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/__main__.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/buildapi.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/cli.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/compat.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/dependencies.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/py.typed
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/version.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 whool-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whool-0.2.1/tests/test_build_sdist.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 whool-0.2.1/tests/test_build_wheel.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 whool-0.2.1/tests/test_init.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 whool-0.2.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 whool-0.2.1/LICENSE
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 whool-0.2.1/README.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 whool-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 whool-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 whool-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 whool-0.2.2/TODO
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 whool-0.2.2/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/__main__.py
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/buildapi.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/cli.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/compat.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/dependencies.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/py.typed
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 whool-0.2.2/src/whool/version.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 whool-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whool-0.2.2/tests/test_build_sdist.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 whool-0.2.2/tests/test_build_wheel.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 whool-0.2.2/tests/test_init.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 whool-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 whool-0.2.2/LICENSE
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 whool-0.2.2/README.md
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 whool-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whool-0.2.2/PKG-INFO
```

### Comparing `whool-0.2.1/.pre-commit-config.yaml` & `whool-0.2.2/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 exclude: ^tests/data/
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
       - id: fix-encoding-pragma
         args: ["--remove"]
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-xml
       - id: mixed-line-ending
         args: ["--fix=lf"]
-  - repo: https://github.com/pycqa/flake8
-    rev: "5.0.4"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.272
     hooks:
-      - id: flake8
-        additional_dependencies: ["flake8-bugbear==22.9.23 "]
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.1
-    hooks:
-      - id: pyupgrade
-        args: [--py36-plus]
-  - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
+      - id: ruff
```

### Comparing `whool-0.2.1/tox.ini` & `whool-0.2.2/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [gh-actions]
 python =
-    3.6: py36
     3.7: py37
     3.8: py38, typing
     3.9: py39, typing
     3.10: py310, typing
     3.11: py311, typing, pypi-description
     pypy3: pypy3
 
 [tox]
 isolated_build = True
 envlist =
-    py36
     py37
     py38
     py39
     py310
     py311
     pypy3
     lint
```

### Comparing `whool-0.2.1/src/whool/buildapi.py` & `whool-0.2.2/src/whool/buildapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         return (
             subprocess.check_output(
                 ["git", "ls-files"], universal_newlines=True, cwd=addon_dir
             )
             .strip()
             .split("\n")
         )
-    except subprocess.CalledProcessError:
-        raise NoScmFound()
+    except subprocess.CalledProcessError as e:
+        raise NoScmFound() from e
 
 
 def _copy_to(addon_dir: Path, dst: Path) -> None:
     if _get_pkg_info_metadata(addon_dir):
         # if PKG-INFO is present, assume we are in an sdist, copy everything
         shutil.copytree(addon_dir, dst)
         return
```

### Comparing `whool-0.2.1/src/whool/cli.py` & `whool-0.2.2/src/whool/cli.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/src/whool/dependencies.py` & `whool-0.2.2/src/whool/dependencies.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/src/whool/init.py` & `whool-0.2.2/src/whool/init.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/tests/conftest.py` & `whool-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/tests/test_build_sdist.py` & `whool-0.2.2/tests/test_build_sdist.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/tests/test_build_wheel.py` & `whool-0.2.2/tests/test_build_wheel.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/tests/test_init.py` & `whool-0.2.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/.gitignore` & `whool-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/LICENSE` & `whool-0.2.2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 The MIT License (MIT)
 
+Copyright (c) 2019 Stéphane Bidoul
 Copyright (c) 2019 ACSONE SA/NV
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `whool-0.2.1/README.md` & `whool-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `whool-0.2.1/pyproject.toml` & `whool-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 name = "whool"
 description = "whool - build backend for Odoo addons"
 readme = "README.md"
 authors = [
   {name = "Stéphane Bidoul", email = "stephane.bidoul@acsone.eu"}
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Framework :: Odoo",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 dependencies = [
     "manifestoo-core[metadata]>=0.8",
+    "wheel<0.42",  # pin because we use an undocumented feature
     "tomli; python_version<'3.11'",
-    "wheel<0.41",  # pin because we use an undocumented feature
     "importlib_metadata; python_version<'3.8'",
 ]
 scripts = {whool = "whool.cli:main"}
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
@@ -40,42 +40,61 @@
 
 [project.urls]
 Homepage = "https://github.com/acsone/whool"
 Documentation = "https://whool.readthedocs.io/en/stable/"
 Changelog = "https://whool.readthedocs.io/en/stable/changelog.html"
 Source = "https://github.com/acsone/whool"
 
+
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build]
 exclude = [
     "/.github",
 ]
 
 
-[tool.isort]
-profile = 'black'
-
 [tool.mypy]
 strict = true
+show_error_codes = true
+
 
 [tool.coverage.run]
 branch = true
 source_pkgs = ["whool"]
 
 [tool.coverage.paths]
 source = ["src", ".tox/*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
     "pragma: no cover",
 ]
 
+
 [tool.towncrier]
 package = "manifestoo_core"
 package_dir = "src"
 filename = "HISTORY.rst"
 directory = "news"
 issue_format = "`#{issue} <https://github.com/sbidoul/manifestoo-core/issues/{issue}>`_"
 title_format = "{version} ({project_date})"
+
+
+[tool.ruff]
+fix = true
+select = [
+    "E", "F", "W", "C90", "B", "I", "UP", "RUF", "TCH"
+]
+target-version = "py37"
+
+[tool.ruff.per-file-ignores]
+"__main__.py" = ["B008"]
+
+[tool.ruff.mccabe]
+max-complexity = 13
+
+[tool.ruff.isort]
+known-first-party = ["whool"]
+combine-as-imports = true
```

### Comparing `whool-0.2.1/PKG-INFO` & `whool-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: whool
-Version: 0.2.1
+Version: 0.2.2
 Summary: whool - build backend for Odoo addons
 Project-URL: Homepage, https://github.com/acsone/whool
 Project-URL: Documentation, https://whool.readthedocs.io/en/stable/
 Project-URL: Changelog, https://whool.readthedocs.io/en/stable/changelog.html
 Project-URL: Source, https://github.com/acsone/whool
 Author-email: Stéphane Bidoul <stephane.bidoul@acsone.eu>
 License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Odoo
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: manifestoo-core[metadata]>=0.8
 Requires-Dist: tomli; python_version < '3.11'
-Requires-Dist: wheel<0.41
+Requires-Dist: wheel<0.42
 Provides-Extra: doc
 Requires-Dist: furo; extra == 'doc'
 Requires-Dist: myst-parser; extra == 'doc'
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinxcontrib-towncrier; extra == 'doc'
 Requires-Dist: towncrier; extra == 'doc'
 Provides-Extra: test
```

