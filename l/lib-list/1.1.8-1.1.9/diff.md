# Comparing `tmp/lib_list-1.1.8.tar.gz` & `tmp/lib_list-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_list-1.1.8.tar", last modified: Fri Jul 14 12:38:42 2023, max compression
+gzip compressed data, was "lib_list-1.1.9.tar", last modified: Sun Jul 30 07:18:51 2023, max compression
```

## Comparing `lib_list-1.1.8.tar` & `lib_list-1.1.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.867275 lib_list-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/.3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 12:37:55.000000 lib_list-1.1.8/.3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-14 12:37:55.000000 lib_list-1.1.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 12:37:55.000000 lib_list-1.1.8/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 12:37:55.000000 lib_list-1.1.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.851275 lib_list-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 12:37:55.000000 lib_list-1.1.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-14 12:37:55.000000 lib_list-1.1.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 12:37:55.000000 lib_list-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-14 12:37:55.000000 lib_list-1.1.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-14 12:37:55.000000 lib_list-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-14 12:37:55.000000 lib_list-1.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 12:37:55.000000 lib_list-1.1.8/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 12:37:55.000000 lib_list-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 12:37:55.000000 lib_list-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 12:37:55.000000 lib_list-1.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-14 12:38:42.867275 lib_list-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 12:37:55.000000 lib_list-1.1.8/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-14 12:37:55.000000 lib_list-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 12:37:55.000000 lib_list-1.1.8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/lib_list/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/lib_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/lib_list_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/lib_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 12:38:42.000000 lib_list-1.1.8/lib_list.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-14 12:37:55.000000 lib_list-1.1.8/lib_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 12:37:55.000000 lib_list-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 12:37:55.000000 lib_list-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 12:37:55.000000 lib_list-1.1.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:38:42.867275 lib_list-1.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.863275 lib_list-1.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:38:42.867275 lib_list-1.1.8/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-14 12:37:55.000000 lib_list-1.1.8/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.327052 lib_list-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.323052 lib_list-1.1.9/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-30 07:18:08.000000 lib_list-1.1.9/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-30 07:18:08.000000 lib_list-1.1.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.323052 lib_list-1.1.9/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-30 07:18:08.000000 lib_list-1.1.9/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-30 07:18:08.000000 lib_list-1.1.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.319052 lib_list-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.323052 lib_list-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-30 07:18:08.000000 lib_list-1.1.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-30 07:18:08.000000 lib_list-1.1.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-30 07:18:08.000000 lib_list-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-30 07:18:08.000000 lib_list-1.1.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-30 07:18:08.000000 lib_list-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-30 07:18:08.000000 lib_list-1.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-30 07:18:08.000000 lib_list-1.1.9/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-30 07:18:08.000000 lib_list-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 07:18:08.000000 lib_list-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-30 07:18:08.000000 lib_list-1.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-30 07:18:51.327052 lib_list-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 07:18:08.000000 lib_list-1.1.9/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-30 07:18:08.000000 lib_list-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-30 07:18:08.000000 lib_list-1.1.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.327052 lib_list-1.1.9/lib_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-30 07:18:08.000000 lib_list-1.1.9/lib_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-30 07:18:08.000000 lib_list-1.1.9/lib_list/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-07-30 07:18:08.000000 lib_list-1.1.9/lib_list/lib_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-30 07:18:08.000000 lib_list-1.1.9/lib_list/lib_list_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:08.000000 lib_list-1.1.9/lib_list/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.327052 lib_list-1.1.9/lib_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-30 07:18:51.000000 lib_list-1.1.9/lib_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-30 07:18:51.000000 lib_list-1.1.9/lib_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 07:18:51.000000 lib_list-1.1.9/lib_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 07:18:51.000000 lib_list-1.1.9/lib_list.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 07:18:51.000000 lib_list-1.1.9/lib_list.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 07:18:51.000000 lib_list-1.1.9/lib_list.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-30 07:18:08.000000 lib_list-1.1.9/lib_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-30 07:18:08.000000 lib_list-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-30 07:18:08.000000 lib_list-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-30 07:18:08.000000 lib_list-1.1.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 07:18:51.327052 lib_list-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.327052 lib_list-1.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:18:51.327052 lib_list-1.1.9/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-30 07:18:08.000000 lib_list-1.1.9/tests/test_cli.py
```

### Comparing `lib_list-1.1.8/.3rd_party_stubs/readme.txt` & `lib_list-1.1.9/.3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/.coveragerc` & `lib_list-1.1.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/.docs/README_template.rst` & `lib_list-1.1.9/.docs/README_template.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_list
 ========
 
 
-Version v1.1.8 as of 2023-07-14 see `Changelog`_
+Version v1.1.9 as of 2023-07-30 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_list-1.1.8/.docs/badges.rst` & `lib_list-1.1.9/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/.docs/installation.rst` & `lib_list-1.1.9/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/.github/workflows/codeql-analysis.yml` & `lib_list-1.1.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/.github/workflows/python-package.yml` & `lib_list-1.1.9/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -145,26 +145,26 @@
 
           - os: ubuntu-latest
             python-version: "pypy-3.9"
             env:
               BUILD_DOCS: "False"
               BUILD: "True"  
               BUILD_TEST: "True"
-              MYPY_DO_TESTS: "False"
+              MYPY_DO_TESTS: "True"
               DO_SETUP_INSTALL: "True"
               DO_SETUP_INSTALL_TEST: "True"
               DO_CLI_TEST: "True"
 
           - os: ubuntu-latest
             python-version: "pypy-3.10"
             env:
               BUILD_DOCS: "False"
               BUILD: "True"  
               BUILD_TEST: "True"
-              MYPY_DO_TESTS: "False"
+              MYPY_DO_TESTS: "True"
               DO_SETUP_INSTALL: "True"
               DO_SETUP_INSTALL_TEST: "True"
               DO_CLI_TEST: "True"
 
           - os: macos-latest
             python-version: "3.11"
             env:
```

### Comparing `lib_list-1.1.8/.gitignore` & `lib_list-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/CHANGES.rst` & `lib_list-1.1.9/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+---------
+2023-07-30:
+    -   flake 8 E721 do not compare types, for instance checks use `isinstance()`
+
 v1.1.8
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `lib_list-1.1.8/CODE_OF_CONDUCT.md` & `lib_list-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/CONTRIBUTING.md` & `lib_list-1.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/ISSUE_TEMPLATE.md` & `lib_list-1.1.9/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/LICENSE` & `lib_list-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/Makefile` & `lib_list-1.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/PKG-INFO` & `lib_list-1.1.9/lib_list.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib_list
-Version: 1.1.8
+Name: lib-list
+Version: 1.1.9
 Summary: some convenience functions for lists
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_list
 Project-URL: Documentation, https://github.com/bitranox/lib_list/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_list.git
 Project-URL: Changelog, https://github.com/bitranox/lib_list/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_list
 ========
 
 
-Version v1.1.8 as of 2023-07-14 see `Changelog`_
+Version v1.1.9 as of 2023-07-30 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
@@ -243,14 +243,19 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+---------
+2023-07-30:
+    -   flake 8 E721 do not compare types, for instance checks use `isinstance()`
+
 v1.1.8
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `lib_list-1.1.8/PULL_REQUEST_TEMPLATE.md` & `lib_list-1.1.9/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/README.rst` & `lib_list-1.1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_list
 ========
 
 
-Version v1.1.8 as of 2023-07-14 see `Changelog`_
+Version v1.1.9 as of 2023-07-30 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
@@ -221,14 +221,19 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+---------
+2023-07-30:
+    -   flake 8 E721 do not compare types, for instance checks use `isinstance()`
+
 v1.1.8
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `lib_list-1.1.8/lib_list/lib_list.py` & `lib_list-1.1.9/lib_list/lib_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     """
 
     if not ls_elements:
         return ls_elements
 
     ls_results = []
     for s_element in ls_elements:
-        if type(s_element) == str:
+        if isinstance(s_element, str):
             s_element = s_element.replace(s_old, s_new)
         ls_results.append(s_element)
     return ls_results
 
 
 def ls_lstrip_list(list_of_strings: List[str], chars: str = "") -> List[str]:
     """
```

### Comparing `lib_list-1.1.8/lib_list/lib_list_cli.py` & `lib_list-1.1.9/lib_list/lib_list_cli.py`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/lib_list.egg-info/PKG-INFO` & `lib_list-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib-list
-Version: 1.1.8
+Name: lib_list
+Version: 1.1.9
 Summary: some convenience functions for lists
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_list
 Project-URL: Documentation, https://github.com/bitranox/lib_list/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_list.git
 Project-URL: Changelog, https://github.com/bitranox/lib_list/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_list
 ========
 
 
-Version v1.1.8 as of 2023-07-14 see `Changelog`_
+Version v1.1.9 as of 2023-07-30 see `Changelog`_
 
 |build_badge| |codeql| |license| |jupyter| |pypi|
 |pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_list/actions/workflows/python-package.yml/badge.svg
@@ -243,14 +243,19 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+---------
+2023-07-30:
+    -   flake 8 E721 do not compare types, for instance checks use `isinstance()`
+
 v1.1.8
 ---------
 2023-07-14:
     - add codeql badge
     - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
     - add pypy 3.10 tests
     - add python 3.12-dev tests
```

### Comparing `lib_list-1.1.8/lib_list.egg-info/SOURCES.txt` & `lib_list-1.1.9/lib_list.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/lib_list.ipynb` & `lib_list-1.1.9/lib_list.ipynb`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/pyproject.toml` & `lib_list-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
-    "click",
     "cli_exit_tools",
+    "click",
 ]
-version = "v1.1.8"
+version = "v1.1.9"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_list"
 Documentation = "https://github.com/bitranox/lib_list/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_list.git"
@@ -42,29 +42,29 @@
 [project.optional-dependencies]
 test = [
     "black",
     "codecov",
     "coloredlogs",
     "coverage",
     "flake8",
-    "mypy ; platform_python_implementation != 'PyPy'",
+    "mypy",
     "pytest",
     "pytest-cov",
     "pytest-runner",
     "readme_renderer",
 ]
 
 [project.scripts]
     lib_list = "lib_list.lib_list_cli:cli_main"
 
 [tool.setuptools.package-data]
 lib_list = [
-    "py.typed",
     "*.pyi",
     "__init__.pyi",
+    "py.typed",
 ]
 
 [tool.black]
 line-length = 160
 #You should include all Python versions that you want your code to run under
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 # Note that you have to use single-quoted strings in TOML for regular expressions
```

### Comparing `lib_list-1.1.8/tests/local_testscripts/lib_bash_functions.sh` & `lib_list-1.1.9/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/local_testscripts/run_pytest.sh` & `lib_list-1.1.9/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/local_testscripts/run_testloop.sh` & `lib_list-1.1.9/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_list-1.1.9/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/local_testscripts/run_testloop_windows.cmd` & `lib_list-1.1.9/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/local_testscripts/shellcheck.sh` & `lib_list-1.1.9/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/local_testscripts/testing_tools.py` & `lib_list-1.1.9/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*

### Comparing `lib_list-1.1.8/tests/test_cli.py` & `lib_list-1.1.9/tests/test_cli.py`

 * *Files identical despite different names*

