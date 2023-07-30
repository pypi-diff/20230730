# Comparing `tmp/slack-logger-python-0.2.8.tar.gz` & `tmp/slack-logger-python-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-logger-python-0.2.8.tar", last modified: Mon Jul 24 15:20:20 2023, max compression
+gzip compressed data, was "slack-logger-python-0.2.9.tar", last modified: Sun Jul 30 15:36:39 2023, max compression
```

## Comparing `slack-logger-python-0.2.8.tar` & `slack-logger-python-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.584969 slack-logger-python-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.576969 slack-logger-python-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.github/workflows/tagging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-24 15:20:20.584969 slack-logger-python-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 15:20:09.000000 slack-logger-python-0.2.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:20:20.584969 slack-logger-python-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/slack_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/slack_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/slack_logger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/slack_logger_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 15:20:20.000000 slack-logger-python-0.2.8/slack_logger_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:20:20.580969 slack-logger-python-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-24 15:19:59.000000 slack-logger-python-0.2.8/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.821392 slack-logger-python-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.github/workflows/tagging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 15:36:31.000000 slack-logger-python-0.2.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/slack_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/slack_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/slack_logger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/slack_logger_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/tests/test_basic.py
```

### Comparing `slack-logger-python-0.2.8/.github/workflows/deploy.yml` & `slack-logger-python-0.2.9/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/.github/workflows/format.yml` & `slack-logger-python-0.2.9/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/.github/workflows/tagging.yml` & `slack-logger-python-0.2.9/.github/workflows/tagging.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/.gitignore` & `slack-logger-python-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/LICENSE` & `slack-logger-python-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/pyproject.toml` & `slack-logger-python-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/shell.nix` & `slack-logger-python-0.2.9/shell.nix`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/slack_logger/__init__.py` & `slack-logger-python-0.2.9/slack_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/slack_logger_python.egg-info/SOURCES.txt` & `slack-logger-python-0.2.9/slack_logger_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.8/tests/test_basic.py` & `slack-logger-python-0.2.9/tests/test_basic.py`

 * *Files identical despite different names*

