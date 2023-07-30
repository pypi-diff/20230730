# Comparing `tmp/adafruit-circuitpython-scd4x-1.3.9.tar.gz` & `tmp/adafruit-circuitpython-scd4x-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-scd4x-1.3.9.tar", last modified: Fri May 26 15:56:53 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-scd4x-1.4.0.tar", last modified: Sun Jul 30 19:30:41 2023, max compression
```

## Comparing `adafruit-circuitpython-scd4x-1.3.9.tar` & `adafruit-circuitpython-scd4x-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.906529 adafruit-circuitpython-scd4x-1.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_scd4x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_tuning_knobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.576898 adafruit-circuitpython-scd4x-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.568898 adafruit-circuitpython-scd4x-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.572898 adafruit-circuitpython-scd4x-1.4.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.572898 adafruit-circuitpython-scd4x-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.572898 adafruit-circuitpython-scd4x-1.4.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-30 19:30:41.576898 adafruit-circuitpython-scd4x-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.572898 adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-30 19:30:41.000000 adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-30 19:30:41.000000 adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:30:41.000000 adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-30 19:30:41.000000 adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 19:30:41.000000 adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-30 19:30:34.000000 adafruit-circuitpython-scd4x-1.4.0/adafruit_scd4x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.576898 adafruit-circuitpython-scd4x-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.576898 adafruit-circuitpython-scd4x-1.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:30:41.576898 adafruit-circuitpython-scd4x-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-30 19:30:34.000000 adafruit-circuitpython-scd4x-1.4.0/examples/scd41_single_shot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-30 19:30:34.000000 adafruit-circuitpython-scd4x-1.4.0/examples/scd4x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-30 19:30:34.000000 adafruit-circuitpython-scd4x-1.4.0/examples/scd4x_tuning_knobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-30 19:30:34.000000 adafruit-circuitpython-scd4x-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-30 19:30:25.000000 adafruit-circuitpython-scd4x-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 19:30:41.576898 adafruit-circuitpython-scd4x-1.4.0/setup.cfg
```

### Comparing `adafruit-circuitpython-scd4x-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-scd4x-1.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/.gitignore` & `adafruit-circuitpython-scd4x-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/.pre-commit-config.yaml` & `adafruit-circuitpython-scd4x-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/.pylintrc` & `adafruit-circuitpython-scd4x-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-scd4x-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/LICENSE` & `adafruit-circuitpython-scd4x-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-scd4x-1.4.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/LICENSES/MIT.txt` & `adafruit-circuitpython-scd4x-1.4.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-scd4x-1.4.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/PKG-INFO` & `adafruit-circuitpython-scd4x-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-scd4x
-Version: 1.3.9
+Version: 1.4.0
 Summary: Driver for Sensirion SCD4X CO2 sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git
 Keywords: adafruit,blinka,circuitpython,micropython,scd4x,CO2,humidity,temperature,sensor,SCD40,SCD41
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-scd4x-1.3.9/README.rst` & `adafruit-circuitpython-scd4x-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/PKG-INFO` & `adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-scd4x
-Version: 1.3.9
+Version: 1.4.0
 Summary: Driver for Sensirion SCD4X CO2 sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git
 Keywords: adafruit,blinka,circuitpython,micropython,scd4x,CO2,humidity,temperature,sensor,SCD40,SCD41
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt` & `adafruit-circuitpython-scd4x-1.4.0/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/scd41_single_shot_example.py
 examples/scd4x_simpletest.py
 examples/scd4x_tuning_knobs.py
```

### Comparing `adafruit-circuitpython-scd4x-1.3.9/adafruit_scd4x.py` & `adafruit-circuitpython-scd4x-1.4.0/adafruit_scd4x.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Tuple, Union
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.3.9"
+__version__ = "1.4.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git"
 
 SCD4X_DEFAULT_ADDR = 0x62
 _SCD4X_REINIT = const(0x3646)
 _SCD4X_FACTORYRESET = const(0x3632)
 _SCD4X_FORCEDRECAL = const(0x362F)
 _SCD4X_SELFTEST = const(0x3639)
@@ -55,14 +55,16 @@
 _SCD4X_SETTEMPOFFSET = const(0x241D)
 _SCD4X_GETALTITUDE = const(0x2322)
 _SCD4X_SETALTITUDE = const(0x2427)
 _SCD4X_SETPRESSURE = const(0xE000)
 _SCD4X_PERSISTSETTINGS = const(0x3615)
 _SCD4X_GETASCE = const(0x2313)
 _SCD4X_SETASCE = const(0x2416)
+_SCD4X_MEASURESINGLESHOT = const(0x219D)
+_SCD4X_MEASURESINGLESHOTRHTONLY = const(0x2196)
 
 
 class SCD4X:
     """
     CircuitPython helper class for using the SCD4X CO2 sensor
 
     :param ~busio.I2C i2c_bus: The I2C bus the SCD4X is connected to.
@@ -143,14 +145,24 @@
             Between measurements, the most recent reading will be cached and returned.
 
         """
         if self.data_ready:
             self._read_data()
         return self._relative_humidity
 
+    def measure_single_shot(self) -> None:
+        """On-demand measurement of CO2 concentration, relative humidity, and
+        temperature for SCD41 only"""
+        self._send_command(_SCD4X_MEASURESINGLESHOT, cmd_delay=5)
+
+    def measure_single_shot_rht_only(self) -> None:
+        """On-demand measurement of relative humidity and temperature for
+        SCD41 only"""
+        self._send_command(_SCD4X_MEASURESINGLESHOTRHTONLY, cmd_delay=0.05)
+
     def reinit(self) -> None:
         """Reinitializes the sensor by reloading user settings from EEPROM."""
         self.stop_periodic_measurement()
         self._send_command(_SCD4X_REINIT, cmd_delay=0.02)
 
     def factory_reset(self) -> None:
         """Resets all configuration settings stored in the EEPROM and erases the
```

### Comparing `adafruit-circuitpython-scd4x-1.3.9/docs/_static/favicon.ico` & `adafruit-circuitpython-scd4x-1.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/docs/conf.py` & `adafruit-circuitpython-scd4x-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/docs/index.rst` & `adafruit-circuitpython-scd4x-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_simpletest.py` & `adafruit-circuitpython-scd4x-1.4.0/examples/scd4x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_tuning_knobs.py` & `adafruit-circuitpython-scd4x-1.4.0/examples/scd4x_tuning_knobs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.9/pyproject.toml` & `adafruit-circuitpython-scd4x-1.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-scd4x"
 description = "Driver for Sensirion SCD4X CO2 sensor"
-version = "1.3.9"
+version = "1.4.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git"}
 keywords = [
     "adafruit",
```

