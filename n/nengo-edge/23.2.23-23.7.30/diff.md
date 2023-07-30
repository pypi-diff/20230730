# Comparing `tmp/nengo-edge-23.2.23.tar.gz` & `tmp/nengo-edge-23.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nengo-edge-23.2.23.tar", last modified: Thu Feb 23 17:16:10 2023, max compression
+gzip compressed data, was "nengo-edge-23.7.30.tar", last modified: Sun Jul 30 16:44:01 2023, max compression
```

## Comparing `nengo-edge-23.2.23.tar` & `nengo-edge-23.7.30.tar`

### file list

```diff
@@ -1,42 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/.nengobones.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   127465 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/_static/demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/docs/examples/microphone-demo/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/examples/microphone-demo/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/examples/microphone-demo/microphone-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/examples/microphone-demo/saved_model.pb.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/examples/microphone-demo/variables.dvc
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/nengo_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/saved_model_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/nengo_edge/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/tests/test_saved_model_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/tests/test_tflite_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/tflite_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/nengo_edge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:16:10.354166 nengo-edge-23.2.23/nengo_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-23 17:16:10.000000 nengo-edge-23.2.23/nengo_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-23 17:16:10.000000 nengo-edge-23.2.23/nengo_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:16:10.000000 nengo-edge-23.2.23/nengo_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:15:25.000000 nengo-edge-23.2.23/nengo_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-23 17:16:10.000000 nengo-edge-23.2.23/nengo_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 17:16:10.000000 nengo-edge-23.2.23/nengo_edge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-23 17:16:10.358166 nengo-edge-23.2.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-02-23 17:14:31.000000 nengo-edge-23.2.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/.nengobones.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.939337 nengo-edge-23.7.30/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.939337 nengo-edge-23.7.30/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   127465 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/_static/demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.939337 nengo-edge-23.7.30/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/examples/coral_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/examples/micro_device_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.939337 nengo-edge-23.7.30/docs/examples/microphone-demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/examples/microphone-demo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/examples/microphone-demo/microphone-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/examples/microphone-demo/saved_model.pb.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/examples/microphone-demo/variables.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/nengo_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/nengo_edge/device_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/device_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/device_modules/coral_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/device_modules/np_mfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/nengo_edge/device_modules/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/device_modules/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/device_modules/tests/test_coral_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/device_modules/tests/test_np_mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/micro_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/network_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/saved_model_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/nengo_edge/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/test_micro_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/test_network_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/test_saved_model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/test_tflite_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/tflite_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/nengo_edge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:44:01.943337 nengo-edge-23.7.30/nengo_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-30 16:44:01.000000 nengo-edge-23.7.30/nengo_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-30 16:44:01.000000 nengo-edge-23.7.30/nengo_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:44:01.000000 nengo-edge-23.7.30/nengo_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:43:09.000000 nengo-edge-23.7.30/nengo_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-30 16:44:01.000000 nengo-edge-23.7.30/nengo_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 16:44:01.000000 nengo-edge-23.7.30/nengo_edge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-30 16:44:01.947337 nengo-edge-23.7.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-30 16:41:34.000000 nengo-edge-23.7.30/setup.py
```

### Comparing `nengo-edge-23.2.23/.nengobones.yml` & `nengo-edge-23.7.30/.nengobones.yml`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 description: Tools for working with NengoEdge
 copyright_start: 2022
 license: mit
 
 setup_cfg:
   mypy:
     ignore_missing_imports:
+      - serial
       - tensorflow
+      - tflite_runtime
+      - rich
 
 ci_scripts:
   - template: static
     pip_install:
       - -e
       - .[tests]
   - template: test
@@ -28,26 +31,28 @@
 
 manifest_in: {}
 
 setup_py:
   author_email: edge-info@appliedbrainresearch.com
   include_package_data: True
   install_req:
+    - pyserial>=3.5
     - tensorflow>=2.10.0 # TODO: support earlier versions?
   tests_req:
     - mypy>=0.901
     - pytest>=7.1.1
     - pytest-rng>=1.0.0
   docs_req:
     - jupyter>=1.0.0
     - nbsphinx>=0.8.11
     - nengo-sphinx-theme>=20.9
     - numpydoc>=1.4.0
+    - rich>=13.3.1
     - sounddevice>=0.4.5
-    - sphinx-tabs~=3.2.0  # more recent versions are incompatible with sphinx 3
+    - sphinx-tabs~=3.2.0 # more recent versions are incompatible with sphinx 3
   url: https://github.com/nengo/nengo-edge
   classifiers:
     - "Development Status :: 4 - Beta"
     - "Framework :: Nengo"
     - "Operating System :: Microsoft :: Windows"
     - "Operating System :: POSIX :: Linux"
     - "Programming Language :: Python"
```

### Comparing `nengo-edge-23.2.23/LICENSE.rst` & `nengo-edge-23.7.30/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nengo-edge-23.2.23/MANIFEST.in` & `nengo-edge-23.7.30/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nengo-edge-23.2.23/PKG-INFO` & `nengo-edge-23.7.30/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nengo-edge
-Version: 23.2.23
+Version: 23.7.30
 Summary: Tools for working with NengoEdge
 Home-page: https://github.com/nengo/nengo-edge
 Author: Applied Brain Research
 Author-email: edge-info@appliedbrainresearch.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Nengo
@@ -76,14 +76,37 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+23.7.30 (July 30, 2023)
+=======================
+
+**Added**
+
+- Added ``CoralRunner`` for running models exported for the Coral board. (`#4`_)
+- Added ``DiscoRunner`` for running models exported for the Disco board. (`#4`_)
+- Added ``NordicRunner`` for running models exported for the Nordic board. (`#4`_)
+- Added on-device MFCC extraction code
+  (``device_modules.np_mfcc.LogMelFeatureExtractor``). (`#4`_)
+- Added two new examples demonstrating how to run models exported for the
+  Coral/Disco/Nordic devices. (`#4`_)
+
+**Changed**
+
+- Renamed ``tflite_runner.Runner`` to ``TFLiteRunner``. (`#4`_)
+- Renamed ``saved_model_runner.Runner`` to ``SavedModelRunner``. (`#4`_)
+- ``TFLiteRunner.reset_state`` now takes a ``batch_size`` argument, which can be used
+  to prepare the model to run with different batch sizes. (`#5`_)
+
+.. _#4: https://github.com/nengo/nengo-edge/pull/4
+.. _#5: https://github.com/nengo/nengo-edge/pull/5
+
 23.2.23 (February 23, 2023)
 ===========================
 
 **Fixed**
 
 - Fixed an issue causing pip to refuse to install ``nengo-edge``. (`#3`_)
```

### Comparing `nengo-edge-23.2.23/README.rst` & `nengo-edge-23.7.30/README.rst`

 * *Files identical despite different names*

### Comparing `nengo-edge-23.2.23/docs/_static/demo.png` & `nengo-edge-23.7.30/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `nengo-edge-23.2.23/docs/_static/favicon.ico` & `nengo-edge-23.7.30/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nengo-edge-23.2.23/docs/examples/microphone-demo/microphone-demo.ipynb` & `nengo-edge-23.7.30/docs/examples/microphone-demo/microphone-demo.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980113636363637%*

 * *Differences: {"'cells'": "{5: {'source': ['Make sure to set the string passed to `SavedModelRunner` to\\n', "*

 * *            "'the directory containing the extracted deployment files.\\n', '\\n', 'You can use "*

 * *            'either the "SavedModel" or "TFLite" deployment option.\\n\', \'If you use "TFLite", '*

 * *            "simply switch the import below to `TFLiteRunner`.']}, 6: {'source': {insert: [(3, "*

 * *            "'from nengo_edge import SavedModelRunner\\n'), (5, 'runner = "*

 * *            'SavedModelRunner(".")\')], delet […]*

```diff
@@ -109,35 +109,34 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f0cb2499",
             "metadata": {},
             "source": [
-                "You can use eithes the \"SavedModel\" or \"TFLite\" deployment option.\n",
-                "If you use \"TFLite\", simply switch the import below to `tflite_runner`.\n",
-                "Also make sure to set the string passed to `Runner` to\n",
-                "the directory containing the extracted deployment files."
+                "Make sure to set the string passed to `SavedModelRunner` to\n",
+                "the directory containing the extracted deployment files.\n",
+                "\n",
+                "You can use either the \"SavedModel\" or \"TFLite\" deployment option.\n",
+                "If you use \"TFLite\", simply switch the import below to `TFLiteRunner`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "879ba6a2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import sounddevice as sd  # pylint: disable=ungrouped-imports\n",
                 "\n",
-                "from nengo_edge.saved_model_runner import Runner\n",
-                "\n",
-                "# from nengo_edge.tflite_runner import Runner\n",
+                "from nengo_edge import SavedModelRunner\n",
                 "\n",
-                "runner = Runner(\".\")"
+                "runner = SavedModelRunner(\".\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3b77fde9",
             "metadata": {},
             "source": [
```

### Comparing `nengo-edge-23.2.23/docs/index.rst` & `nengo-edge-23.7.30/docs/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 ==========
 
 .. toctree::
    :maxdepth: 2
 
    installation
    examples/microphone-demo/microphone-demo
-
+   examples/coral_demo
+   examples/micro_device_demo
 .. * :ref:`genindex`  TODO include once we generate API docs
```

#### html2text {}

```diff
@@ -4,9 +4,9 @@
 accuracy, low power audio AI models on edge devices. This package contains
 tools and examples to assist in taking a trained model exported from NengoEdge
 and deploying it in your own application. To get started running NengoEdge
 models locally, set up a Python environment using the installation instructions
 below. Then download the :raw-html:`live_microphone_demo_notebook` and open it
 with:: jupyter notebook /path/to/microphone-demo.ipynb .. raw:: html  Learn
 more ========== .. toctree:: :maxdepth: 2 installation examples/microphone-
-demo/microphone-demo .. * :ref:`genindex` TODO include once we generate API
-docs
+demo/microphone-demo examples/coral_demo examples/micro_device_demo .. * :ref:
+`genindex` TODO include once we generate API docs
```

### Comparing `nengo-edge-23.2.23/docs/installation.rst` & `nengo-edge-23.7.30/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nengo-edge-23.2.23/nengo_edge/saved_model_runner.py` & `nengo-edge-23.7.30/nengo_edge/saved_model_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Dict, Union
 
 import numpy as np
 import tensorflow as tf
 
 
-class Runner:
+class SavedModelRunner:
     """Run a model exported in TensorFlow's SavedModel format."""
 
     def __init__(self, directory: Union[str, Path]):
         self.directory = Path(directory)
 
         self.model = tf.saved_model.load(str(self.directory)).signatures[
             "serving_default"
@@ -36,22 +36,22 @@
     def run(self, inputs: np.ndarray) -> np.ndarray:
         """
         Run the model on the given inputs.
 
         Parameters
         ----------
         inputs : np.ndarray
-            Model input values (should have shape ``(batch_size, input_steps)`` if
-            ``extract_features`` else ``(batch_size, input_steps, input_d)``).
+            Model input values (should have shape ``(batch_size, input_steps)``).
 
         Returns
         -------
         outputs : ``np.ndarray``
             Model output values (with shape ``(batch_size, output_d)`` if
-            ``return_sequences=False`` else ``(batch_size, output_steps, output_d)``).
+            the model was built to return only the final time step,
+            else ``(batch_size, output_steps, output_d)``).
         """
 
         inputs = tf.cast(inputs, "float32")
 
         kwargs = {}
         for name, sig in self.model.structured_input_signature[1].items():
             if name == self.input_names[0]:
```

### Comparing `nengo-edge-23.2.23/nengo_edge/tests/test_saved_model_runner.py` & `nengo-edge-23.7.30/nengo_edge/tests/test_saved_model_runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,73 +3,77 @@
 from pathlib import Path
 from typing import Literal
 
 import numpy as np
 import pytest
 import tensorflow as tf
 from nengo_edge_hw import gpu
-from nengo_edge_models.tests.test_models import _test_lmu
+from nengo_edge_models.kws.models import lmu_small
 
-from nengo_edge.saved_model_runner import Runner
+from nengo_edge.saved_model_runner import SavedModelRunner
 
 
 @pytest.mark.parametrize("mode", ("model-only", "feature-only", "full"))
 def test_runner(
     mode: Literal["model-only", "feature-only", "full"],
     rng: np.random.RandomState,
     seed: int,
     tmp_path: Path,
 ) -> None:
     tf.keras.utils.set_random_seed(seed)
 
-    interface = gpu.host.Interface(_test_lmu(), mode=mode, build_dir=tmp_path)
+    interface = gpu.host.Interface(lmu_small(), mode=mode, build_dir=tmp_path)
 
     inputs = rng.uniform(
         -1, 1, size=(32,) + ((49, 20) if mode == "model-only" else (16000,))
     ).astype("float32")
 
     output0 = interface.run(inputs)
 
     interface.export_model(tmp_path)
 
     assert interface.binary_path is not None
-    runner = Runner(tmp_path)
+    runner = SavedModelRunner(tmp_path)
 
     output1 = runner.run(inputs)
 
     assert np.allclose(output0, output1), np.max(np.abs(output0 - output1))
 
 
 def test_runner_streaming(
     rng: np.random.RandomState, seed: int, tmp_path: Path
 ) -> None:
     tf.keras.utils.set_random_seed(seed)
 
-    interface = gpu.host.Interface(_test_lmu(), mode="full", build_dir=tmp_path)
-
-    inputs = rng.uniform(-1, 1, size=(32, 16000)).astype("float32")
+    interface = gpu.host.Interface(lmu_small(), mode="full", build_dir=tmp_path)
 
+    # 3200 timesteps is equivalent to 200ms at 16 kHz
+    inputs = rng.uniform(-1, 1, size=(32, 3200)).astype("float32")
     output0 = interface.run(inputs)
 
-    interface.export_model(tmp_path / "streaming")
-
-    runner = Runner(tmp_path / "streaming")
+    interface.export_model(tmp_path / "streaming", streaming=True)
+    runner = SavedModelRunner(tmp_path / "streaming")
 
     # check that running in parts produces the same output
+    stream_chunk_size = inputs.shape[1] // 4
     for i in range(4):
-        output1 = runner.run(inputs[:, i * 4000 : (i + 1) * 4000])
+        output1 = runner.run(
+            inputs[:, i * stream_chunk_size : (i + 1) * stream_chunk_size]
+        )
 
-    assert np.allclose(output0, output1, atol=1e-5), np.max(np.abs(output0 - output1))
+    assert np.allclose(output0, output1, atol=1e-4), np.max(np.abs(output0 - output1))
 
     # check that resetting state works
     runner.reset_state()
     for i in range(4):
-        output2 = runner.run(inputs[:, i * 4000 : (i + 1) * 4000])
+        output2 = runner.run(
+            inputs[:, i * stream_chunk_size : (i + 1) * stream_chunk_size]
+        )
 
-    assert np.allclose(output0, output2, atol=1e-5), np.max(np.abs(output0 - output2))
+    assert np.allclose(output0, output2, atol=1e-4), np.max(np.abs(output0 - output2))
 
     # test zero padding
     runner.reset_state()
     pad_output = runner.run(inputs[:, :10])
     pad_output_gt = (
         interface.run(
             np.concatenate(
@@ -77,15 +81,15 @@
                     inputs[:, :10],
                     np.zeros((32, interface.audio_options.window_size_samples - 10)),
                 ],
                 axis=1,
             )
         ),
     )
-    assert np.allclose(pad_output, pad_output_gt), np.max(
+    assert np.allclose(pad_output, pad_output_gt, atol=2e-6), np.max(
         np.abs(pad_output - pad_output_gt)
     )
     pad_output_step = runner.run(inputs[:, -10:])
     pad_output_step_gt = interface.run(
         np.concatenate(
             [
                 inputs[:, :10],
```

### Comparing `nengo-edge-23.2.23/nengo_edge/tests/test_tflite_runner.py` & `nengo-edge-23.7.30/nengo_edge/tests/test_tflite_runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from pathlib import Path
 
 import numpy as np
 import pytest
 import tensorflow as tf
 from nengo_edge_hw import coral
-from nengo_edge_models.tests.test_models import _test_lmu
+from nengo_edge_models.kws.tests.test_models import _test_lmu
 
-from nengo_edge.tflite_runner import Runner
+from nengo_edge.tflite_runner import TFLiteRunner
 
 
 @pytest.mark.parametrize("return_sequences", (True, False))
 def test_runner_streaming(
     return_sequences: bool,
     tmp_path: Path,
     rng: np.random.RandomState,
@@ -28,89 +28,89 @@
         _test_lmu(),
         build_dir=tmp_path,
         use_device=False,
         return_sequences=return_sequences,
     )
 
     host.export_model(tmp_path / "exported")
-    host.export_model(tmp_path / "exported-batch", batch_size=batch_size)
 
     inputs = rng.uniform(-0.5, 0.5, size=(batch_size, 16000))
 
-    runner = Runner(
-        tmp_path / "exported", extract_features=True, return_sequences=return_sequences
-    )
-    runner_batch = Runner(
-        tmp_path / "exported-batch",
-        extract_features=True,
-        return_sequences=return_sequences,
-    )
+    runner = TFLiteRunner(tmp_path / "exported")
 
     # check that batched and non-batched models produce the same output (state is being
     # properly reset between batch items)
     out = []
     for i in range(batch_size):
         out.append(runner.run(inputs[i : i + 1]))
-        runner.reset_state()
+        runner.reset_state(batch_size=1)
     out0 = np.concatenate(out, axis=0)
 
-    out1 = runner_batch.run(inputs)
+    runner.reset_state(batch_size=batch_size)
+    out1 = runner.run(inputs)
 
     assert (
         out0.shape
         == out1.shape
         == ((batch_size, 49, 10) if return_sequences else (batch_size, 10))
     )
 
     # increased tolerance due to float32 variance
     assert np.allclose(out0, out1, atol=1e-5), np.max(abs(out0 - out1))
 
     # check that running sequentially produces the same output as running all at once
-    runner_batch.reset_state()
+    runner.reset_state(batch_size=batch_size)
     if return_sequences:
         out0 = np.concatenate(
-            [runner_batch.run(inputs[:, :4000]), runner_batch.run(inputs[:, 4000:])],
+            [runner.run(inputs[:, :4000]), runner.run(inputs[:, 4000:])],
             axis=1,
         )
     else:
-        runner_batch.run(inputs[:, :4000])
-        out0 = runner_batch.run(inputs[:, 4000:])
-    runner_batch.reset_state()
-    out1 = runner_batch.run(inputs)
+        runner.run(inputs[:, :4000])
+        out0 = runner.run(inputs[:, 4000:])
+    runner.reset_state(batch_size=batch_size)
+    out1 = runner.run(inputs)
     assert (
         out0.shape
         == out1.shape
         == ((batch_size, 49, 10) if return_sequences else (batch_size, 10))
     )
     assert np.allclose(out0, out1, atol=5e-5), np.max(abs(out0 - out1))
 
 
 def test_runner_errors(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> None:
     model_desc = _test_lmu()
     model_desc.n_unroll = 2
     monkeypatch.setattr(coral.host.Interface, "io_dtype", None)
-    host = coral.host.Interface(model_desc, build_dir=tmp_path, use_device=False)
+    host = coral.host.Interface(
+        model_desc, build_dir=tmp_path, use_device=False, mode="model-only"
+    )
     host.export_model(tmp_path)
 
-    runner = Runner(tmp_path, extract_features=False)
+    runner = TFLiteRunner(tmp_path)
 
     with pytest.raises(ValueError, match="evenly divided by unroll"):
         runner.run(np.zeros((1, 3, 10)))
 
+    Path(tmp_path / "model.tflite").unlink()
+
+    with pytest.raises(FileNotFoundError, match="Could not find model file"):
+        TFLiteRunner(tmp_path)
+
 
 def test_runner_quantized(tmp_path: Path, rng: np.random.RandomState) -> None:
     model_desc = _test_lmu()
     host = coral.host.Interface(
         model_desc,
         build_dir=tmp_path,
         use_device=False,
         representative_data=rng.uniform(-1, 1, size=(32, 16000)),
     )
     host.export_model(tmp_path)
 
-    runner = Runner(tmp_path)
+    runner = TFLiteRunner(tmp_path)
 
     x = rng.uniform(-1, 1, size=(1, 16000))
     y0 = runner.run(x)
     y1 = host.run(x)
 
     assert np.allclose(y0, y1, atol=5e-5), np.max(abs(y0 - y1))
```

### Comparing `nengo-edge-23.2.23/nengo_edge/tflite_runner.py` & `nengo-edge-23.7.30/nengo_edge/tflite_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,100 @@
 """Interface for running an exported NengoEdge model in TFLite format."""
 
+import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 import tensorflow as tf
 
+from nengo_edge import config
 
-class Runner:
+
+class TFLiteRunner:
     """
     Run an exported TFLite model.
 
     Parameters
     ----------
     directory : Union[str, Path]
         Path to the directory containing the exported model files.
-    extract_features : bool
-        Perform feature extraction on inputs if True (default). Otherwise, feature
-        extraction is assumed to be performed manually elsewhere in the pipeline.
-    return_sequences : bool
-        If True (default False), return output from every timestep instead of only
-        the last timestep.
     """
 
-    def __init__(
-        self,
-        directory: Union[str, Path],
-        extract_features: bool = True,
-        return_sequences: bool = False,
-    ):
+    def __init__(self, directory: Union[str, Path]):
         self.directory = Path(directory)
-        self.extract_features = extract_features
-        # TODO: automatically determine return_sequences from the exported model somehow
-        self.return_sequences = return_sequences
+        self.model_params, self.preprocessing = config.load_params(self.directory)
 
         # Build interpreters
-        self.model_interpreter = self._build_interpreter(
-            self.directory / "model.tflite"
-        )
-        if extract_features:
-            self.feature_interpreter = self._build_interpreter(
-                self.directory / "feature_extractor.tflite"
+        model_path = self.directory / "model.tflite"
+        if not model_path.exists():
+            raise FileNotFoundError(f"Could not find model file ({model_path})")
+        self.model_interpreter = tf.lite.Interpreter(model_path=str(model_path))
+        self.model_interpreter.allocate_tensors()
+
+        feature_path = self.directory / "feature_extractor.tflite"
+        if not feature_path.exists():
+            warnings.warn(
+                f"Could not find feature extractor model file ({feature_path}).\n"
+                f"Using the tflite runner without a compiled feature extractor is "
+                f"an experimental feature and may lead to poor model performance."
             )
+            self.feature_interpreter = None
+        else:
+            self.feature_interpreter = tf.lite.Interpreter(model_path=str(feature_path))
+            self.feature_interpreter.allocate_tensors()
 
         self.reset_state()
 
-    def reset_state(self) -> None:
+    def reset_state(self, batch_size: int = 1) -> None:
         """Reset the internal state of the model to initial conditions."""
-
+        assert self.model_interpreter is not None
         self.model_state = [
-            np.zeros(x["shape"], dtype=x["dtype"])
+            np.zeros([batch_size] + x["shape"].tolist()[1:], dtype=x["dtype"])
             for x in self.model_interpreter.get_input_details()[1:]
         ]
-        if self.extract_features:
+
+        if self.feature_interpreter is not None:
             self.feature_state = [
                 np.zeros(
                     [
                         # initialize dynamic state sizes to 0 to avoid startup artifacts
-                        0 if sig == -1 else val
-                        for sig, val in zip(x["shape_signature"], x["shape"])
+                        batch_size if i == 0 else (0 if sig == -1 else val)
+                        for i, (sig, val) in enumerate(
+                            zip(x["shape_signature"], x["shape"])
+                        )
                     ],
                     dtype=x["dtype"],
                 )
                 for x in self.feature_interpreter.get_input_details()[1:]
             ]
 
     def run(self, inputs: np.ndarray) -> np.ndarray:
         """
         Run the model on the given inputs.
 
         Parameters
         ----------
         inputs : np.ndarray
-            Model input values (should have shape ``(batch_size, input_steps)`` if
-            ``extract_features`` else ``(batch_size, input_steps, input_d)``).
+            Model input values (should have shape ``(batch_size, input_steps)``).
 
         Returns
         -------
         outputs : ``np.ndarray``
             Model output values (with shape ``(batch_size, output_d)`` if
-            ``return_sequences=False`` else ``(batch_size, output_steps, output_d)``).
+            ``self.model_params['return_sequences']=False``
+            else ``(batch_size, output_steps, output_d)``).
         """
-
-        if self.extract_features:
+        if self.feature_interpreter is not None:
             inputs, self.feature_state = self._run_feature_extractor(inputs)
 
         outputs, self.model_state = self._run_model(inputs)
 
         return outputs
 
-    def _build_interpreter(self, model_path: Path) -> tf.lite.Interpreter:
-        """Build a TFLite interpreter for the given model file."""
-
-        interpreter = tf.lite.Interpreter(model_path=str(model_path))
-
-        interpreter.allocate_tensors()
-
-        return interpreter
-
     def _resize_inputs(
         self, interpreter: tf.lite.Interpreter, input_vals: List[np.ndarray]
     ) -> None:
         reallocate = False
         for s0, s1 in zip(input_vals, interpreter.get_input_details()):
             if s0.shape != tuple(s1["shape"]):
                 # this will attempt to resize any dynamic dimensions (e.g. batch
@@ -112,14 +105,15 @@
         if reallocate:
             interpreter.allocate_tensors()
 
     def _run_feature_extractor(
         self, inputs: np.ndarray
     ) -> Tuple[np.ndarray, List[np.ndarray]]:
         """Run the feature extractor on the given inputs."""
+        assert self.feature_interpreter is not None
 
         self._resize_inputs(self.feature_interpreter, [inputs] + self.feature_state)
 
         for inp, val in zip(
             self.feature_interpreter.get_input_details(), [inputs] + self.feature_state
         ):
             self.feature_interpreter.set_tensor(inp["index"], val.astype(np.float32))
@@ -161,15 +155,15 @@
             for details in output_details
         ]
 
         # quantize all the inputs ahead of time (for efficiency)
         inputs = self.quantize(inputs, input_details[0])
 
         state_input = self.model_state
-        if self.return_sequences:
+        if self.model_params["return_sequences"]:
             output_sequences = []
 
         for step in range(0, n_steps, n_unroll):
             # set input for current block of unrolled steps
             input_tensors[0]()[:] = inputs[:, step : step + n_unroll]
             for inp, fp32_data, details in zip(
                 input_tensors[1:], state_input, input_details[1:]
@@ -181,19 +175,19 @@
 
             # get state input for next block of steps
             state_input = [
                 self.dequantize(out(), details)
                 for out, details in zip(output_tensors[1:], output_details[1:])
             ]
 
-            if self.return_sequences:
+            if self.model_params["return_sequences"]:
                 # Append all outputs from the past `unroll` timesteps
                 output_sequences.append(output_tensors[0]().copy())
 
-        if self.return_sequences:
+        if self.model_params["return_sequences"]:
             # concatenate outputs from each unroll block
             # note: because the model was built with return_sequences=True, this
             # represents the output from all the timesteps
             outputs = np.concatenate(output_sequences, axis=1)
         else:
             # only use the output from last unroll block
             # note: because the model was built with return_sequences=False, the
@@ -205,15 +199,14 @@
         outputs = self.dequantize(outputs, output_details[0])
 
         return outputs, state_input
 
     @staticmethod
     def quantize(val: np.ndarray, details: Dict[str, Any]) -> np.ndarray:
         """Quantize the given value based on quantization parameters."""
-
         n_scales = len(details["quantization_parameters"]["scales"])
         if n_scales == 0:
             # val is not quantized
             return np.array(val)
 
         assert n_scales == 1
         val = np.asarray(val)
@@ -222,15 +215,14 @@
         iinfo = np.iinfo(details["dtype"])
         q = np.round((val / scaling_factor) + zero_point)
         return np.clip(q, iinfo.min, iinfo.max).astype(details["dtype"])
 
     @staticmethod
     def dequantize(val: np.ndarray, details: Dict[str, Any]) -> np.ndarray:
         """Dequantize the given value based on quantization parameters."""
-
         n_scales = len(details["quantization_parameters"]["scales"])
         if n_scales == 0:
             # val is not quantized
             return np.array(val)
 
         assert n_scales == 1
         scaling_factor = details["quantization_parameters"]["scales"][0]
```

### Comparing `nengo-edge-23.2.23/nengo_edge/version.py` & `nengo-edge-23.7.30/nengo_edge/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 We use calendar versioning (see https://calver.org/) and conform to PEP440 (see
 https://www.python.org/dev/peps/pep-0440/). '.dev0' will be added to the version
 unless the code base represents a release version. Release versions are git
 tagged with the version.
 """
 
-version_info = (23, 2, 23)
+version_info = (23, 7, 30)
 
 name = "nengo-edge"
 dev = None
 
 # use old string formatting, so that this can still run in Python <= 3.5
 # (since this file is parsed in setup.py, before python_requires is applied)
 version = ".".join(str(v) for v in version_info)
```

### Comparing `nengo-edge-23.2.23/nengo_edge.egg-info/PKG-INFO` & `nengo-edge-23.7.30/nengo_edge.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nengo-edge
-Version: 23.2.23
+Version: 23.7.30
 Summary: Tools for working with NengoEdge
 Home-page: https://github.com/nengo/nengo-edge
 Author: Applied Brain Research
 Author-email: edge-info@appliedbrainresearch.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Nengo
@@ -76,14 +76,37 @@
 
    - Added
    - Changed
    - Deprecated
    - Removed
    - Fixed
 
+23.7.30 (July 30, 2023)
+=======================
+
+**Added**
+
+- Added ``CoralRunner`` for running models exported for the Coral board. (`#4`_)
+- Added ``DiscoRunner`` for running models exported for the Disco board. (`#4`_)
+- Added ``NordicRunner`` for running models exported for the Nordic board. (`#4`_)
+- Added on-device MFCC extraction code
+  (``device_modules.np_mfcc.LogMelFeatureExtractor``). (`#4`_)
+- Added two new examples demonstrating how to run models exported for the
+  Coral/Disco/Nordic devices. (`#4`_)
+
+**Changed**
+
+- Renamed ``tflite_runner.Runner`` to ``TFLiteRunner``. (`#4`_)
+- Renamed ``saved_model_runner.Runner`` to ``SavedModelRunner``. (`#4`_)
+- ``TFLiteRunner.reset_state`` now takes a ``batch_size`` argument, which can be used
+  to prepare the model to run with different batch sizes. (`#5`_)
+
+.. _#4: https://github.com/nengo/nengo-edge/pull/4
+.. _#5: https://github.com/nengo/nengo-edge/pull/5
+
 23.2.23 (February 23, 2023)
 ===========================
 
 **Fixed**
 
 - Fixed an issue causing pip to refuse to install ``nengo-edge``. (`#3`_)
```

### Comparing `nengo-edge-23.2.23/setup.cfg` & `nengo-edge-23.7.30/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -104,14 +104,23 @@
 
 [mypy]
 python_version = 3.8
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 plugins = numpy.typing.mypy_plugin
 
+[mypy-serial.*]
+ignore_missing_imports = True
+
 [mypy-tensorflow.*]
 ignore_missing_imports = True
 
+[mypy-tflite_runtime.*]
+ignore_missing_imports = True
+
+[mypy-rich.*]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `nengo-edge-23.2.23/setup.py` & `nengo-edge-23.7.30/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     return sep.join(buf)
 
 
 root = pathlib.Path(__file__).parent
 version = runpy.run_path(str(root / "nengo_edge" / "version.py"))["version"]
 
 install_req = [
+    "pyserial>=3.5",
     "tensorflow>=2.10.0",
 ]
 docs_req = [
     "jupyter>=1.0.0",
     "nbsphinx>=0.8.11",
     "nengo-sphinx-theme>=20.9",
     "numpydoc>=1.4.0",
+    "rich>=13.3.1",
     "sounddevice>=0.4.5",
     "sphinx-tabs~=3.2.0",
 ]
 optional_req = []
 tests_req = [
     "mypy>=0.901",
     "pytest>=7.1.1",
```

