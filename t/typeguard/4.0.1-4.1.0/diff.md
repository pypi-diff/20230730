# Comparing `tmp/typeguard-4.0.1.tar.gz` & `tmp/typeguard-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.0.1.tar", last modified: Thu Jul 27 13:37:36 2023, max compression
+gzip compressed data, was "typeguard-4.1.0.tar", last modified: Sat Jul 29 22:19:47 2023, max compression
```

## Comparing `typeguard-4.0.1.tar` & `typeguard-4.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.232788 typeguard-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 13:37:26.000000 typeguard-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-27 13:37:26.000000 typeguard-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 13:37:26.000000 typeguard-4.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-27 13:37:26.000000 typeguard-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-27 13:37:36.232788 typeguard-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-27 13:37:26.000000 typeguard-4.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.228788 typeguard-4.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-27 13:37:26.000000 typeguard-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:37:36.232788 typeguard-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.228788 typeguard-4.0.1/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27389 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    43580 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.228788 typeguard-4.0.1/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.232788 typeguard-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.232788 typeguard-4.0.1/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32870 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    44319 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.612262 typeguard-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.604262 typeguard-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.604262 typeguard-4.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-29 22:19:38.000000 typeguard-4.1.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 22:19:38.000000 typeguard-4.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-29 22:19:38.000000 typeguard-4.1.0/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.604262 typeguard-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 22:19:38.000000 typeguard-4.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-29 22:19:38.000000 typeguard-4.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-29 22:19:38.000000 typeguard-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-29 22:19:38.000000 typeguard-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-29 22:19:38.000000 typeguard-4.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-29 22:19:38.000000 typeguard-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-29 22:19:47.612262 typeguard-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-29 22:19:38.000000 typeguard-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.604262 typeguard-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20205 2023-07-29 22:19:38.000000 typeguard-4.1.0/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-29 22:19:38.000000 typeguard-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:19:47.612262 typeguard-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.604262 typeguard-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.608262 typeguard-4.1.0/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27389 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43721 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:38.000000 typeguard-4.1.0/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.608262 typeguard-4.1.0/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-29 22:19:47.000000 typeguard-4.1.0/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-29 22:19:47.000000 typeguard-4.1.0/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:19:47.000000 typeguard-4.1.0/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 22:19:47.000000 typeguard-4.1.0/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-29 22:19:47.000000 typeguard-4.1.0/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 22:19:47.000000 typeguard-4.1.0/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.608262 typeguard-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:19:47.608262 typeguard-4.1.0/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33064 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44319 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 22:19:38.000000 typeguard-4.1.0/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.1.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.1.0/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/.github/workflows/publish.yml` & `typeguard-4.1.0/.github/workflows/publish.yml`

 * *Files 26% similar despite different names*

```diff
@@ -5,24 +5,37 @@
     tags:
       - "[0-9]+.[0-9]+.[0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+.post[0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+[a-b][0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+rc[0-9]+"
 
 jobs:
-  publish:
+  build:
     runs-on: ubuntu-latest
     environment: release
-    permissions:
-      id-token: write
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
       run: python -m build
+    - name: Archive packages
+      uses: actions/upload-artifact@v3
+      with:
+        name: dist
+        path: dist
+
+  publish:
+    needs: build
+    runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
+    steps:
+    - name: Retrieve packages
+      uses: actions/download-artifact@v3
     - name: Upload packages
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `typeguard-4.0.1/.github/workflows/test.yml` & `typeguard-4.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/.pre-commit-config.yaml` & `typeguard-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/LICENSE` & `typeguard-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/PKG-INFO` & `typeguard-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.1
+Version: 4.1.0
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.1/README.rst` & `typeguard-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/api.rst` & `typeguard-4.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/conf.py` & `typeguard-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/contributing.rst` & `typeguard-4.1.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/extending.rst` & `typeguard-4.1.0/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/features.rst` & `typeguard-4.1.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/userguide.rst` & `typeguard-4.1.0/docs/userguide.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/docs/versionhistory.rst` & `typeguard-4.1.0/docs/versionhistory.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.1.0** (2023-07-30)
+
+- Added support for passing a tuple as ``expected_type`` to ``check_type()``, making it
+  more of a drop-in replacement for ``isinstance()``
+  (`#371 <https://github.com/agronholm/typeguard/issues/371>`_
+- Fixed regression where ``Literal`` inside a ``Union`` had quotes stripped from its
+  contents, thus typically causing ``NameError`` to be raised when run
+  (`#372 <https://github.com/agronholm/typeguard/issues/372>`_)
+
 **4.0.1** (2023-07-27)
 
 - Fixed handling of ``typing_extensions.Literal`` on Python 3.8 and 3.9 when
   ``typing_extensions>=4.6.0`` is installed
   (`#363 <https://github.com/agronholm/typeguard/issues/363>`_; PR by Alex Waygood)
 - Fixed ``NameError`` when generated type checking code references an imported name from
   a method (`#362 <https://github.com/agronholm/typeguard/issues/362>`_)
```

### Comparing `typeguard-4.0.1/pyproject.toml` & `typeguard-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/__init__.py` & `typeguard-4.1.0/src/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_checkers.py` & `typeguard-4.1.0/src/typeguard/_checkers.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_config.py` & `typeguard-4.1.0/src/typeguard/_config.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_decorators.py` & `typeguard-4.1.0/src/typeguard/_decorators.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_exceptions.py` & `typeguard-4.1.0/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_functions.py` & `typeguard-4.1.0/src/typeguard/_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sys
 import warnings
-from typing import Any, Callable, NoReturn, TypeVar, overload
+from typing import Any, Callable, NoReturn, TypeVar, Union, overload
 
 from . import _suppression
 from ._checkers import BINARY_MAGIC_METHODS, check_type_internal
 from ._config import (
     CollectionCheckStrategy,
     ForwardRefPolicy,
     TypeCheckConfiguration,
@@ -76,24 +76,27 @@
     Note that this function is independent of the globally shared configuration in
     :data:`typeguard.config`. This means that usage within libraries is safe from being
     affected configuration changes made by other libraries or by the integrating
     application. Instead, configuration options have the same default values as their
     corresponding fields in :class:`TypeCheckConfiguration`.
 
     :param value: value to be checked against ``expected_type``
-    :param expected_type: a class or generic type instance
+    :param expected_type: a class or generic type instance, or a tuple of such things
     :param forward_ref_policy: see :attr:`TypeCheckConfiguration.forward_ref_policy`
     :param typecheck_fail_callback:
         see :attr`TypeCheckConfiguration.typecheck_fail_callback`
     :param collection_check_strategy:
         see :attr:`TypeCheckConfiguration.collection_check_strategy`
     :return: ``value``, unmodified
     :raises TypeCheckError: if there is a type mismatch
 
     """
+    if type(expected_type) is tuple:
+        expected_type = Union[expected_type]
+
     config = TypeCheckConfiguration(
         forward_ref_policy=forward_ref_policy,
         typecheck_fail_callback=typecheck_fail_callback,
         collection_check_strategy=collection_check_strategy,
     )
 
     if _suppression.type_checks_suppressed or expected_type is Any:
```

### Comparing `typeguard-4.0.1/src/typeguard/_importhook.py` & `typeguard-4.1.0/src/typeguard/_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_memo.py` & `typeguard-4.1.0/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_pytest_plugin.py` & `typeguard-4.1.0/src/typeguard/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_suppression.py` & `typeguard-4.1.0/src/typeguard/_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_transformer.py` & `typeguard-4.1.0/src/typeguard/_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,14 +359,20 @@
         if isinstance(new_node, expr) and self._memo.name_matches(
             new_node, *anytype_names
         ):
             return None
 
         return new_node
 
+    def generic_visit(self, node: AST) -> AST:
+        if isinstance(node, expr) and self._memo.name_matches(node, *literal_names):
+            return node
+
+        return super().generic_visit(node)
+
     def visit_BinOp(self, node: BinOp) -> Any:
         self.generic_visit(node)
 
         if isinstance(node.op, BitOr):
             # If either side of the operation resolved to None, return None
             if not hasattr(node, "left") or not hasattr(node, "right"):
                 return None
@@ -391,15 +397,15 @@
 
     def visit_Subscript(self, node: Subscript) -> Any:
         if self._memo.is_ignored_name(node.value):
             return None
 
         # The subscript of typing(_extensions).Literal can be any arbitrary string, so
         # don't try to evaluate it as code
-        if not self._memo.name_matches(node.value, *literal_names) and node.slice:
+        if node.slice:
             if isinstance(node.slice, Index):
                 # Python 3.7 and 3.8
                 slice_value = node.slice.value  # type: ignore[attr-defined]
             else:
                 slice_value = node.slice
 
             if isinstance(slice_value, Tuple):
```

### Comparing `typeguard-4.0.1/src/typeguard/_union_transformer.py` & `typeguard-4.1.0/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard/_utils.py` & `typeguard-4.1.0/src/typeguard/_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.1.0/src/typeguard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.1
+Version: 4.1.0
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.1/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.1.0/src/typeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/__init__.py` & `typeguard-4.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/conftest.py` & `typeguard-4.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/dummymodule.py` & `typeguard-4.1.0/tests/dummymodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -330,14 +330,20 @@
 @typechecked
 def literal(x: Literal["foo"]) -> Literal["foo"]:
     y: Literal["foo"] = x
     return y
 
 
 @typechecked
+def literal_in_union(x: Union[Literal["foo"],]) -> Literal["foo"]:
+    y: Literal["foo"] = x
+    return y
+
+
+@typechecked
 def typevar_forwardref(x: Type[T]) -> T:
     return x()
 
 
 def never_called(x: List["NonExistentType"]) -> List["NonExistentType"]:  # noqa: F821
     """Regression test for #335."""
     return x
```

### Comparing `typeguard-4.0.1/tests/mypy/negative.py` & `typeguard-4.1.0/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/mypy/positive.py` & `typeguard-4.1.0/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/mypy/test_type_annotations.py` & `typeguard-4.1.0/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_checkers.py` & `typeguard-4.1.0/tests/test_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1076,7 +1076,15 @@
 
 def test_imported_str_forward_ref():
     value = {"foo": 1}
     memo = TypeCheckMemo(globals(), locals())
     pattern = r"Skipping type check against 'Dict\[str, int\]'"
     with pytest.warns(TypeHintWarning, match=pattern):
         check_type_internal(value, "Dict[str, int]", memo)
+
+
+def test_check_against_tuple_success():
+    check_type(1, (float, Union[str, int]))
+
+
+def test_check_against_tuple_failure():
+    pytest.raises(TypeCheckError, check_type, "aa", (int, bytes))
```

### Comparing `typeguard-4.0.1/tests/test_importhook.py` & `typeguard-4.1.0/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_instrumentation.py` & `typeguard-4.1.0/tests/test_instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,10 +320,15 @@
         assert dummymodule.guarded_type_hint_subscript_nested(["foo"]) == ["foo"]
 
 
 def test_literal(dummymodule):
     assert dummymodule.literal("foo") == "foo"
 
 
+def test_literal_in_union(dummymodule):
+    """Regression test for #372."""
+    assert dummymodule.literal_in_union("foo") == "foo"
+
+
 def test_typevar_forwardref(dummymodule):
     instance = dummymodule.typevar_forwardref(dummymodule.DummyClass)
     assert isinstance(instance, dummymodule.DummyClass)
```

### Comparing `typeguard-4.0.1/tests/test_plugins.py` & `typeguard-4.1.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_suppression.py` & `typeguard-4.1.0/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_transformer.py` & `typeguard-4.1.0/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_typechecked.py` & `typeguard-4.1.0/tests/test_typechecked.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_union_transformer.py` & `typeguard-4.1.0/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_utils.py` & `typeguard-4.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.1/tests/test_warn_on_error.py` & `typeguard-4.1.0/tests/test_warn_on_error.py`

 * *Files identical despite different names*

