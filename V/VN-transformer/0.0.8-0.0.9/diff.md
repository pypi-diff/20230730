# Comparing `tmp/VN-transformer-0.0.8.tar.gz` & `tmp/VN-transformer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.8.tar", last modified: Sat Jul 29 17:31:54 2023, max compression
+gzip compressed data, was "VN-transformer-0.0.9.tar", last modified: Sat Jul 29 18:34:56 2023, max compression
```

## Comparing `VN-transformer-0.0.8.tar` & `VN-transformer-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.498180 VN-transformer-0.0.9/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/tests/test.py
```

### Comparing `VN-transformer-0.0.8/LICENSE` & `VN-transformer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.8/PKG-INFO` & `VN-transformer-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.8/README.md` & `VN-transformer-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 
 model = VNTransformer(
     dim = 64,
     depth = 2,
     dim_head = 64,
     heads = 8,
     dim_feat = 64,       # will default to early fusion, since this was the best performing
-    beta_epsilon = 1e-6  # in this paper, they propose breaking equivariance with a tiny bit of bias noise in the VN linear. they claim this leads to improved stability. setting this to 0 would turn off the epsilon approximate equivariance
+    bias_epsilon = 1e-6  # in this paper, they propose breaking equivariance with a tiny bit of bias noise in the VN linear. they claim this leads to improved stability. setting this to 0 would turn off the epsilon approximate equivariance
 )
 
 feats = torch.randn(1, 32, 64)
 coors = torch.randn(1, 32, 3)    # (batch, sequence, spatial coordinates)
 
-feats, coors = model(feats, coors)
+out = model(coors, feats = feats) # (1, 32, 64 + 3 = 67)
 ```
 
 ## Tests
 
 Confidence in equivariance
 
 ```bash
 $ python setup.py test
 ```
 
 ## Todo
 
-- [ ] complete the perceiver like feature aggregation
-- [ ] offer both early and late fusion within `VNTransformer`
+- [x] complete the perceiver like feature aggregation
+- [x] offer early fusion within `VNTransformer` with setting of `dim_feat`
 - [ ] see if it is straightforward to make translation in/equivariant
     - [ ] test on protein backbone denoising if above could be done
 
 ## Citations
 
 ```bibtex
 @inproceedings{Assaad2022VNTransformerRA,
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
 [./vn-transformer.png] ## VN (Vector Neuron) Transformer A Transformer_made_of
 Rotation-equivariant_Attention using Vector_Neurons Open_Review ## Install
 ```bash $ pip install VN-transformer ``` ## Usage ```python import torch from
 VN_transformer import VNTransformer model = VNTransformer( dim = 64, depth = 2,
 dim_head = 64, heads = 8, dim_feat = 64, # will default to early fusion, since
-this was the best performing beta_epsilon = 1e-6 # in this paper, they propose
+this was the best performing bias_epsilon = 1e-6 # in this paper, they propose
 breaking equivariance with a tiny bit of bias noise in the VN linear. they
 claim this leads to improved stability. setting this to 0 would turn off the
 epsilon approximate equivariance ) feats = torch.randn(1, 32, 64) coors =
-torch.randn(1, 32, 3) # (batch, sequence, spatial coordinates) feats, coors =
-model(feats, coors) ``` ## Tests Confidence in equivariance ```bash $ python
-setup.py test ``` ## Todo - [ ] complete the perceiver like feature aggregation
-- [ ] offer both early and late fusion within `VNTransformer` - [ ] see if it
-is straightforward to make translation in/equivariant - [ ] test on protein
-backbone denoising if above could be done ## Citations ```bibtex @inproceedings
+torch.randn(1, 32, 3) # (batch, sequence, spatial coordinates) out = model
+(coors, feats = feats) # (1, 32, 64 + 3 = 67) ``` ## Tests Confidence in
+equivariance ```bash $ python setup.py test ``` ## Todo - [x] complete the
+perceiver like feature aggregation - [x] offer early fusion within
+`VNTransformer` with setting of `dim_feat` - [ ] see if it is straightforward
+to make translation in/equivariant - [ ] test on protein backbone denoising if
+above could be done ## Citations ```bibtex @inproceedings
 {Assaad2022VNTransformerRA, title = {VN-Transformer: Rotation-Equivariant
 Attention for Vector Neurons}, author = {Serge Assaad and C. Downey and Rami
 Al-Rfou and Nigamaa Nayakanti and Benjamin Sapp}, year = {2022} } ``` ```bibtex
 @article{Deng2021VectorNA, title = {Vector Neurons: A General Framework for SO
 (3)-Equivariant Networks}, author = {Congyue Deng and Or Litany and Yueqi Duan
 and Adrien Poulenard and Andrea Tagliasacchi and Leonidas J. Guibas}, journal =
 {2021 IEEE/CVF International Conference on Computer Vision (ICCV)}, year =
```

### Comparing `VN-transformer-0.0.8/VN_transformer/VN_transformer.py` & `VN-transformer-0.0.9/VN_transformer/VN_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,8 +300,8 @@
             coors = torch.cat((coors, feats), dim = -1)
 
         assert coors.shape[-1] == self.dim_coor_total
 
         coors = self.vn_proj_in(coors)
         coors = self.encoder(coors, mask = mask)
         coors = self.vn_proj_out(coors)
-        return feats, coors
+        return coors
```

### Comparing `VN-transformer-0.0.8/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.0.9/VN_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.8/setup.py` & `VN-transformer-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

### Comparing `VN-transformer-0.0.8/tests/test.py` & `VN-transformer-0.0.9/tests/test.py`

 * *Files identical despite different names*

