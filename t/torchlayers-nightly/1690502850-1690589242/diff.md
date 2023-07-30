# Comparing `tmp/torchlayers-nightly-1690502850.tar.gz` & `tmp/torchlayers-nightly-1690589242.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchlayers-nightly-1690502850.tar", last modified: Fri Jul 28 00:07:35 2023, max compression
+gzip compressed data, was "dist/torchlayers-nightly-1690589242.tar", last modified: Sat Jul 29 00:07:31 2023, max compression
```

## Comparing `torchlayers-nightly-1690502850.tar` & `torchlayers-nightly-1690589242.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/attributes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/convolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/general_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/jit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/pickle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/tests/torchlayers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers/
--rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers/_dev_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/_dev_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/_dev_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/_dev_utils/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-28 00:07:30.000000 torchlayers-nightly-1690502850/torchlayers/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 00:07:35.000000 torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/convolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/general_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/jit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/pickle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/tests/torchlayers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers/_dev_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/_dev_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/_dev_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/_dev_utils/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-29 00:07:22.000000 torchlayers-nightly-1690589242/torchlayers/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 00:07:31.000000 torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/top_level.txt
```

### Comparing `torchlayers-nightly-1690502850/PKG-INFO` & `torchlayers-nightly-1690589242/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1690502850
+Version: 1690589242
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1690502850/README.md` & `torchlayers-nightly-1690589242/README.md`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/setup.py` & `torchlayers-nightly-1690589242/setup.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/convolution_test.py` & `torchlayers-nightly-1690589242/tests/convolution_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/general_test.py` & `torchlayers-nightly-1690589242/tests/general_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/jit_test.py` & `torchlayers-nightly-1690589242/tests/jit_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/pickle_test.py` & `torchlayers-nightly-1690589242/tests/pickle_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/preprocessing_test.py` & `torchlayers-nightly-1690589242/tests/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/regularization_test.py` & `torchlayers-nightly-1690589242/tests/regularization_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/tests/torchlayers_test.py` & `torchlayers-nightly-1690589242/tests/torchlayers_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/__init__.py` & `torchlayers-nightly-1690589242/torchlayers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/_dev_utils/helpers.py` & `torchlayers-nightly-1690589242/torchlayers/_dev_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/_dev_utils/infer.py` & `torchlayers-nightly-1690589242/torchlayers/_dev_utils/infer.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/activations.py` & `torchlayers-nightly-1690589242/torchlayers/activations.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/convolution.py` & `torchlayers-nightly-1690589242/torchlayers/convolution.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/module.py` & `torchlayers-nightly-1690589242/torchlayers/module.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/normalization.py` & `torchlayers-nightly-1690589242/torchlayers/normalization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/pooling.py` & `torchlayers-nightly-1690589242/torchlayers/pooling.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/preprocessing.py` & `torchlayers-nightly-1690589242/torchlayers/preprocessing.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/regularization.py` & `torchlayers-nightly-1690589242/torchlayers/regularization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers/upsample.py` & `torchlayers-nightly-1690589242/torchlayers/upsample.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/PKG-INFO` & `torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1690502850
+Version: 1690589242
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1690502850/torchlayers_nightly.egg-info/SOURCES.txt` & `torchlayers-nightly-1690589242/torchlayers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

