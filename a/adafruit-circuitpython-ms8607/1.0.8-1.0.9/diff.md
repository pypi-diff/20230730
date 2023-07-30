# Comparing `tmp/adafruit-circuitpython-ms8607-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-ms8607-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ms8607-1.0.8.tar", last modified: Mon Nov 15 18:58:50 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ms8607-1.0.9.tar", last modified: Fri Feb  4 20:18:31 2022, max compression
```

## Comparing `adafruit-circuitpython-ms8607-1.0.8.tar` & `adafruit-circuitpython-ms8607-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.785488 adafruit-circuitpython-ms8607-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.781489 adafruit-circuitpython-ms8607-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.781489 adafruit-circuitpython-ms8607-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.781489 adafruit-circuitpython-ms8607-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16260 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.781489 adafruit-circuitpython-ms8607-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2021-11-15 18:58:50.785488 adafruit-circuitpython-ms8607-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.781489 adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2021-11-15 18:58:50.000000 adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      902 2021-11-15 18:58:50.000000 adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:58:50.000000 adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 18:58:50.000000 adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-15 18:58:50.000000 adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14398 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/adafruit_ms8607.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.785488 adafruit-circuitpython-ms8607-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.785488 adafruit-circuitpython-ms8607-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:58:50.785488 adafruit-circuitpython-ms8607-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/examples/ms8607_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:58:50.785488 adafruit-circuitpython-ms8607-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-11-15 18:58:37.000000 adafruit-circuitpython-ms8607-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:30.997249 adafruit-circuitpython-ms8607-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:30.997249 adafruit-circuitpython-ms8607-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16260 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-02-04 20:18:30.000000 adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-02-04 20:18:30.000000 adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:18:30.000000 adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 20:18:30.000000 adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:18:30.000000 adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14398 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/adafruit_ms8607.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5440 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/examples/ms8607_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:18:31.001249 adafruit-circuitpython-ms8607-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-02-04 20:18:14.000000 adafruit-circuitpython-ms8607-1.0.9/setup.py
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ms8607-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 Thank you for contributing! Before you submit a pull request, please read the following.
 
-Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://circuitpython.readthedocs.io/en/latest/docs/design_guide.html
+Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://docs.circuitpython.org/en/latest/docs/design_guide.html
 
 If your changes are to documentation, please verify that the documentation builds locally by following the steps found here: https://adafru.it/build-docs
 
 Before submitting the pull request, make sure you've run Pylint and Black locally on your code. You can do this manually or using pre-commit. Instructions are available here: https://adafru.it/check-your-code
 
 Please remove all of this text before submitting. Include an explanation or list of changes included in your PR, as well as, if applicable, a link to any related issues.
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-ms8607-1.0.9/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.7
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-ms8607-1.0.9/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.6
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
@@ -63,15 +63,15 @@
     - uses: actions/checkout@v1
     - name: Check For setup.py
       id: need-pypi
       run: |
         echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
     - name: Set up Python
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ms8607-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/.pylintrc` & `adafruit-circuitpython-ms8607-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ms8607-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/LICENSE` & `adafruit-circuitpython-ms8607-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ms8607-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ms8607-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ms8607-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/PKG-INFO` & `adafruit-circuitpython-ms8607-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ms8607
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for the MS8607 PTH sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MS8607
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ms8607 pressure humidity temperature sensor
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ms8607/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ms8607/en/latest/
+    :target: https://docs.circuitpython.org/projects/ms8607/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MS8607/workflows/Build%20CI/badge.svg
@@ -96,15 +94,15 @@
         sleep(1)
 
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ms8607/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ms8607/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_MS8607/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/README.rst` & `adafruit-circuitpython-ms8607-1.0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ms8607/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ms8607/en/latest/
+    :target: https://docs.circuitpython.org/projects/ms8607/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MS8607/workflows/Build%20CI/badge.svg
@@ -75,15 +75,15 @@
         sleep(1)
 
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ms8607/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ms8607/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_MS8607/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/PKG-INFO` & `adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ms8607
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for the MS8607 PTH sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MS8607
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ms8607 pressure humidity temperature sensor
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ms8607/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ms8607/en/latest/
+    :target: https://docs.circuitpython.org/projects/ms8607/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MS8607/workflows/Build%20CI/badge.svg
@@ -96,15 +94,15 @@
         sleep(1)
 
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ms8607/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ms8607/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_MS8607/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/adafruit_circuitpython_ms8607.egg-info/SOURCES.txt` & `adafruit-circuitpython-ms8607-1.0.9/adafruit_circuitpython_ms8607.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/adafruit_ms8607.py` & `adafruit-circuitpython-ms8607-1.0.9/adafruit_ms8607.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ms8607-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ms8607-1.0.8/docs/conf.py` & `adafruit-circuitpython-ms8607-1.0.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 
 autodoc_mock_imports = ["adafruit_bus_device"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "python": ("https://docs.python.org/3", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/docs/index.rst` & `adafruit-circuitpython-ms8607-1.0.9/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     Adafruit MS8607 Breakout <https://www.adafruit.com/products/4716>
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/adafruit/Adafruit_CircuitPython_MS8607/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ms8607-1.0.8/setup.py` & `adafruit-circuitpython-ms8607-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Hardware",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
     ],
     # What does your project relate to?
     keywords="adafruit blinka circuitpython micropython ms8607 pressure humidity temperature "
     "sensor",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     # TODO: IF LIBRARY FILES ARE A PACKAGE FOLDER,
```

