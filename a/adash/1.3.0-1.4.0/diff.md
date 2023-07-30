# Comparing `tmp/adash-1.3.0.tar.gz` & `tmp/adash-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adash-1.3.0.tar", last modified: Tue Jan  4 07:44:42 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `adash-1.3.0.tar` & `adash-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,52 @@
--rw-r--r--   0        0        0     1064 2021-12-20 01:46:48.541789 adash-1.3.0/LICENSE
--rw-r--r--   0        0        0      573 2021-12-20 01:46:48.543662 adash-1.3.0/README.md
--rw-r--r--   0        0        0      476 2022-01-04 07:44:39.395987 adash-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      359 2022-01-04 07:15:11.145733 adash-1.3.0/src/adash/__init__.py
--rw-r--r--   0        0        0      608 2022-01-03 03:11:32.289275 adash-1.3.0/src/adash/collection_util.py
--rw-r--r--   0        0        0     1163 2021-12-26 11:40:38.116573 adash-1.3.0/src/adash/date_util.py
--rw-r--r--   0        0        0     2381 2022-01-04 07:36:46.638623 adash-1.3.0/src/adash/file_util.py
--rw-r--r--   0        0        0     1610 2021-12-26 11:40:38.117467 adash-1.3.0/src/adash/proportion.py
--rw-r--r--   0        0        0     3701 2021-12-26 11:40:38.118180 adash-1.3.0/src/adash/string_util.py
--rw-r--r--   0        0        0     1194 2022-01-04 07:44:42.150676 adash-1.3.0/setup.py
--rw-r--r--   0        0        0     1025 2022-01-04 07:44:42.150961 adash-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 adash-1.4.0/.python-version
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 adash-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    18820 2020-02-02 00:00:00.000000 adash-1.4.0/poetry.lock
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 adash-1.4.0/pyproject.poetry.toml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 adash-1.4.0/pytest.ini
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 adash-1.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 adash-1.4.0/requirements.lock
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 adash-1.4.0/ruff.toml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 adash-1.4.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 adash-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/.gitignore
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/rye-venv.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/activate
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/coverage
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/coverage-3.8
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/coverage3
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/ptw
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/py.test
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/pytest
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/pytest-watch
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/python -> /Users/atu/.rye/py/cpython@3.8.16/install/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/python3.8 -> python
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 adash-1.4.0/.venv/bin/watchmedo
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 adash-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 adash-1.4.0/docs/adash/download.html
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 adash-1.4.0/docs/adash/index.html
+-rw-r--r--   0        0        0    10824 2020-02-02 00:00:00.000000 adash-1.4.0/docs/adash/proportion.html
+-rw-r--r--   0        0        0    18298 2020-02-02 00:00:00.000000 adash-1.4.0/docs/adash/string_util.html
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 adash-1.4.0/src/adash/__init__.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 adash-1.4.0/src/adash/collection_util.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 adash-1.4.0/src/adash/date_util.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 adash-1.4.0/src/adash/file_util.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 adash-1.4.0/src/adash/proportion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 adash-1.4.0/src/adash/string_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adash-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 adash-1.4.0/tests/test_collection_util.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 adash-1.4.0/tests/test_date_list.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 adash-1.4.0/tests/test_file_util.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 adash-1.4.0/tests/test_proportion.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 adash-1.4.0/tests/test_string_util.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 adash-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 adash-1.4.0/LICENSE
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 adash-1.4.0/README.md
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 adash-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 adash-1.4.0/PKG-INFO
```

### Comparing `adash-1.3.0/LICENSE` & `adash-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adash-1.3.0/README.md` & `adash-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `adash-1.3.0/src/adash/date_util.py` & `adash-1.4.0/src/adash/date_util.py`

 * *Files identical despite different names*

### Comparing `adash-1.3.0/src/adash/file_util.py` & `adash-1.4.0/src/adash/file_util.py`

 * *Files identical despite different names*

### Comparing `adash-1.3.0/src/adash/proportion.py` & `adash-1.4.0/src/adash/proportion.py`

 * *Files identical despite different names*

### Comparing `adash-1.3.0/src/adash/string_util.py` & `adash-1.4.0/src/adash/string_util.py`

 * *Files identical despite different names*

