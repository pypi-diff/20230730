# Comparing `tmp/adafruit-circuitpython-servokit-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-servokit-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-servokit-1.3.8.tar", last modified: Wed Feb 23 16:19:10 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-servokit-1.3.9.tar", last modified: Tue Jun  7 17:18:36 2022, max compression
```

## Comparing `adafruit-circuitpython-servokit-1.3.8.tar` & `adafruit-circuitpython-servokit-1.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.102001 adafruit-circuitpython-servokit-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.102001 adafruit-circuitpython-servokit-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.102001 adafruit-circuitpython-servokit-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.102001 adafruit-circuitpython-servokit-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-02-23 16:19:09.000000 adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-02-23 16:19:09.000000 adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-23 16:19:09.000000 adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-02-23 16:19:09.000000 adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-23 16:19:09.000000 adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6995 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/adafruit_servokit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)      549 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/examples/servokit_all_servos_sequential.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      596 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/examples/servokit_all_servos_synchronised.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/examples/servokit_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-23 16:19:10.106001 adafruit-circuitpython-servokit-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-02-23 16:18:56.000000 adafruit-circuitpython-servokit-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.137269 adafruit-circuitpython-servokit-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.129268 adafruit-circuitpython-servokit-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.133268 adafruit-circuitpython-servokit-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.133268 adafruit-circuitpython-servokit-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.133268 adafruit-circuitpython-servokit-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-06-07 17:18:36.137269 adafruit-circuitpython-servokit-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.133268 adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-06-07 17:18:36.000000 adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-06-07 17:18:36.000000 adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:18:36.000000 adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-07 17:18:36.000000 adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-07 17:18:36.000000 adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6995 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/adafruit_servokit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.133268 adafruit-circuitpython-servokit-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.133268 adafruit-circuitpython-servokit-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5776 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:18:36.137269 adafruit-circuitpython-servokit-1.3.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      549 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/examples/servokit_all_servos_sequential.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      596 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/examples/servokit_all_servos_synchronised.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/examples/servokit_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:18:36.137269 adafruit-circuitpython-servokit-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-06-07 17:18:18.000000 adafruit-circuitpython-servokit-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-servokit-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-servokit-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-servokit-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-servokit-1.3.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
     rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/.pylintrc` & `adafruit-circuitpython-servokit-1.3.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-servokit-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/LICENSE` & `adafruit-circuitpython-servokit-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-servokit-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-servokit-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-servokit-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/PKG-INFO` & `adafruit-circuitpython-servokit-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-servokit
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython helper library for PWM/Servo FeatherWing, Shield, and Pi HAT and Bonnet kits.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit servo motor pwm pca9685 featherwing pi shield bonnet servokit kit i2c hardware micropython circuitpython
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-servokit/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/servokit/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/README.rst` & `adafruit-circuitpython-servokit-1.3.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-servokit/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/servokit/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/PKG-INFO` & `adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-servokit
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython helper library for PWM/Servo FeatherWing, Shield, and Pi HAT and Bonnet kits.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit servo motor pwm pca9685 featherwing pi shield bonnet servokit kit i2c hardware micropython circuitpython
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-servokit/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/servokit/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_ServoKit/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/adafruit_circuitpython_servokit.egg-info/SOURCES.txt` & `adafruit-circuitpython-servokit-1.3.9/adafruit_circuitpython_servokit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/adafruit_servokit.py` & `adafruit-circuitpython-servokit-1.3.9/adafruit_servokit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-servokit-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/docs/conf.py` & `adafruit-circuitpython-servokit-1.3.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-servokit-1.3.8/docs/index.rst` & `adafruit-circuitpython-servokit-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/examples/servokit_all_servos_sequential.py` & `adafruit-circuitpython-servokit-1.3.9/examples/servokit_all_servos_sequential.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/examples/servokit_all_servos_synchronised.py` & `adafruit-circuitpython-servokit-1.3.9/examples/servokit_all_servos_synchronised.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/examples/servokit_simpletest.py` & `adafruit-circuitpython-servokit-1.3.9/examples/servokit_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-servokit-1.3.8/setup.py` & `adafruit-circuitpython-servokit-1.3.9/setup.py`

 * *Files identical despite different names*

