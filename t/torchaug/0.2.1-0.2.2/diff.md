# Comparing `tmp/torchaug-0.2.1.tar.gz` & `tmp/torchaug-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchaug-0.2.1.tar", last modified: Thu Jul 27 17:59:15 2023, max compression
+gzip compressed data, was "torchaug-0.2.2.tar", last modified: Sun Jul 30 17:21:32 2023, max compression
```

## Comparing `torchaug-0.2.1.tar` & `torchaug-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:59:15.460238 torchaug-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    21777 2023-07-27 17:59:05.000000 torchaug-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-27 17:59:15.460238 torchaug-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-27 17:59:05.000000 torchaug-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-27 17:59:05.000000 torchaug-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 17:59:05.000000 torchaug-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:59:15.460238 torchaug-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:59:15.460238 torchaug-0.2.1/torchaug/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 17:59:05.000000 torchaug-0.2.1/torchaug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:59:15.460238 torchaug-0.2.1/torchaug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:21:32.714282 torchaug-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    21777 2023-07-30 17:21:18.000000 torchaug-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-30 17:21:32.714282 torchaug-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-30 17:21:18.000000 torchaug-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-30 17:21:18.000000 torchaug-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-30 17:21:18.000000 torchaug-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:21:32.714282 torchaug-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:21:32.714282 torchaug-0.2.2/torchaug/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 17:21:18.000000 torchaug-0.2.2/torchaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-30 17:21:18.000000 torchaug-0.2.2/torchaug/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:21:32.714282 torchaug-0.2.2/torchaug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-30 17:21:32.000000 torchaug-0.2.2/torchaug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 17:21:32.000000 torchaug-0.2.2/torchaug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:21:32.000000 torchaug-0.2.2/torchaug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 17:21:32.000000 torchaug-0.2.2/torchaug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 17:21:32.000000 torchaug-0.2.2/torchaug.egg-info/top_level.txt
```

### Comparing `torchaug-0.2.1/LICENSE` & `torchaug-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchaug-0.2.1/PKG-INFO` & `torchaug-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaug
-Version: 0.2.1
+Version: 0.2.2
 Summary: Torchvision Complementary tool to perform batch and GPU data augmentations.
 Author-email: Julien Denize <julien.denize@hotmail.fr>
 Project-URL: Homepage, https://github.com/juliendenize/torchaug
 Project-URL: Bug Tracker, https://github.com/juliendenize/torchaug/issues
 Project-URL: Download, https://github.com/juliendenize/torchaug
 Project-URL: Source Code, https://github.com/juliendenize/torchaug
 Keywords: computer vision,deep learning,pytorch
@@ -44,28 +44,28 @@
 ## Introduction
 
 Torchvision has been implemented over Pytorch and Pillow to perform Computer Vision in the Pytorch Ecosystem. One of its core functionality is to perform Data augmentations. However because it has been implemented first for CPU and later with GPU in mind, it has several drawbacks to make it work on GPUs:
 
 - Some CPU/GPU synchronizations cannot be avoided.
 - Batch data augmentations are not completely random, meaning that random parameters are sampled for the whole batch and not each unique component.
 
-This library aims to remove these issues. It acts like a complementary library with Torchvision and does not use the same namespace. Still, it follows the same nomenclature as Torchvision with *functional* augmentations and *class* wrappers.
+This library aims to remove these issues. It acts like a complementary library to Torchvision and does not use the same namespace. Still, it follows the same nomenclature as Torchvision with *functional* augmentations and *transforms* class wrappers.
 
 To be sure to retrieve the same data augmentations as Torchvision, it has been tested on each of its augmentations.
 
-See [here](augmentations.md) the implemented data augmentations and [here](speed_comparison.md) the speed comparison with Torchvision.
+See [augmentations.md](augmentations.md) for the implemented data augmentations and [speed_comparison.md](speed_comparison.md) for the speed comparison with Torchvision.
 
 ## How to use
 
 0. Install a Pytorch >= 2.0 environment.
 
 1. Install Torchaug.
 
 ```bash
-pip3 install torchaug
+pip install torchaug
 ```
 
 2. Import data augmentations either from `torchaug.transforms` or `torchaug.batch_transforms` packages.
 
 ```python
 from torchaug.transforms import RandomColorJitter
 from torchaug.batch_transforms import BatchRandomColorJitter
```

### Comparing `torchaug-0.2.1/README.md` & `torchaug-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 ## Introduction
 
 Torchvision has been implemented over Pytorch and Pillow to perform Computer Vision in the Pytorch Ecosystem. One of its core functionality is to perform Data augmentations. However because it has been implemented first for CPU and later with GPU in mind, it has several drawbacks to make it work on GPUs:
 
 - Some CPU/GPU synchronizations cannot be avoided.
 - Batch data augmentations are not completely random, meaning that random parameters are sampled for the whole batch and not each unique component.
 
-This library aims to remove these issues. It acts like a complementary library with Torchvision and does not use the same namespace. Still, it follows the same nomenclature as Torchvision with *functional* augmentations and *class* wrappers.
+This library aims to remove these issues. It acts like a complementary library to Torchvision and does not use the same namespace. Still, it follows the same nomenclature as Torchvision with *functional* augmentations and *transforms* class wrappers.
 
 To be sure to retrieve the same data augmentations as Torchvision, it has been tested on each of its augmentations.
 
-See [here](augmentations.md) the implemented data augmentations and [here](speed_comparison.md) the speed comparison with Torchvision.
+See [augmentations.md](augmentations.md) for the implemented data augmentations and [speed_comparison.md](speed_comparison.md) for the speed comparison with Torchvision.
 
 ## How to use
 
 0. Install a Pytorch >= 2.0 environment.
 
 1. Install Torchaug.
 
 ```bash
-pip3 install torchaug
+pip install torchaug
 ```
 
 2. Import data augmentations either from `torchaug.transforms` or `torchaug.batch_transforms` packages.
 
 ```python
 from torchaug.transforms import RandomColorJitter
 from torchaug.batch_transforms import BatchRandomColorJitter
```

### Comparing `torchaug-0.2.1/pyproject.toml` & `torchaug-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchaug-0.2.1/torchaug.egg-info/PKG-INFO` & `torchaug-0.2.2/torchaug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaug
-Version: 0.2.1
+Version: 0.2.2
 Summary: Torchvision Complementary tool to perform batch and GPU data augmentations.
 Author-email: Julien Denize <julien.denize@hotmail.fr>
 Project-URL: Homepage, https://github.com/juliendenize/torchaug
 Project-URL: Bug Tracker, https://github.com/juliendenize/torchaug/issues
 Project-URL: Download, https://github.com/juliendenize/torchaug
 Project-URL: Source Code, https://github.com/juliendenize/torchaug
 Keywords: computer vision,deep learning,pytorch
@@ -44,28 +44,28 @@
 ## Introduction
 
 Torchvision has been implemented over Pytorch and Pillow to perform Computer Vision in the Pytorch Ecosystem. One of its core functionality is to perform Data augmentations. However because it has been implemented first for CPU and later with GPU in mind, it has several drawbacks to make it work on GPUs:
 
 - Some CPU/GPU synchronizations cannot be avoided.
 - Batch data augmentations are not completely random, meaning that random parameters are sampled for the whole batch and not each unique component.
 
-This library aims to remove these issues. It acts like a complementary library with Torchvision and does not use the same namespace. Still, it follows the same nomenclature as Torchvision with *functional* augmentations and *class* wrappers.
+This library aims to remove these issues. It acts like a complementary library to Torchvision and does not use the same namespace. Still, it follows the same nomenclature as Torchvision with *functional* augmentations and *transforms* class wrappers.
 
 To be sure to retrieve the same data augmentations as Torchvision, it has been tested on each of its augmentations.
 
-See [here](augmentations.md) the implemented data augmentations and [here](speed_comparison.md) the speed comparison with Torchvision.
+See [augmentations.md](augmentations.md) for the implemented data augmentations and [speed_comparison.md](speed_comparison.md) for the speed comparison with Torchvision.
 
 ## How to use
 
 0. Install a Pytorch >= 2.0 environment.
 
 1. Install Torchaug.
 
 ```bash
-pip3 install torchaug
+pip install torchaug
 ```
 
 2. Import data augmentations either from `torchaug.transforms` or `torchaug.batch_transforms` packages.
 
 ```python
 from torchaug.transforms import RandomColorJitter
 from torchaug.batch_transforms import BatchRandomColorJitter
```

