# Comparing `tmp/dispersenn2-0.0.3.tar.gz` & `tmp/dispersenn2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispersenn2-0.0.3.tar", max compression
+gzip compressed data, was "dispersenn2-0.0.4.tar", max compression
```

## Comparing `dispersenn2-0.0.3.tar` & `dispersenn2-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      599 2023-07-28 19:39:37.121430 dispersenn2-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-27 22:45:44.334779 dispersenn2-0.0.3/dispersenn2/check_params.py
--rw-r--r--   0        0        0    13167 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/data_generation.py
--rw-r--r--   0        0        0    24917 2023-07-28 20:57:42.467508 dispersenn2-0.0.3/dispersenn2/disperseNN2.py
--rw-r--r--   0        0        0     7097 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/process_input.py
--rw-r--r--   0        0        0     3824 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/read_input.py
--rw-r--r--   0        0        0      575 2023-07-28 20:58:14.295946 dispersenn2-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 dispersenn2-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-07-28 19:39:37.121430 dispersenn2-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 20:51:57.445326 dispersenn2-0.0.4/disperseNN2/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-27 22:45:44.334779 dispersenn2-0.0.4/disperseNN2/check_params.py
+-rw-r--r--   0        0        0    13167 2023-07-29 23:32:56.018528 dispersenn2-0.0.4/disperseNN2/data_generation.py
+-rw-r--r--   0        0        0    24859 2023-07-29 23:33:11.150694 dispersenn2-0.0.4/disperseNN2/disperseNN2.py
+-rw-r--r--   0        0        0     7097 2023-07-29 23:33:24.482841 dispersenn2-0.0.4/disperseNN2/process_input.py
+-rw-r--r--   0        0        0     3824 2023-07-27 20:51:57.445326 dispersenn2-0.0.4/disperseNN2/read_input.py
+-rw-r--r--   0        0        0      620 2023-07-29 23:41:53.716020 dispersenn2-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 dispersenn2-0.0.4/PKG-INFO
```

### Comparing `dispersenn2-0.0.3/README.md` & `dispersenn2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.3/dispersenn2/check_params.py` & `dispersenn2-0.0.4/disperseNN2/check_params.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.3/dispersenn2/data_generation.py` & `dispersenn2-0.0.4/disperseNN2/data_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import numpy as np
 import tensorflow as tf
 import msprime
 import tskit
 import warnings
 from attrs import define
-from dispersenn2.read_input import parse_provenance
+from disperseNN2.read_input import parse_provenance
 import gc
 
 
 @define
 class DataGenerator(tf.keras.utils.Sequence):
     "Generates data for Keras"
```

### Comparing `dispersenn2-0.0.3/dispersenn2/disperseNN2.py` & `dispersenn2-0.0.4/disperseNN2/disperseNN2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 # main code for disperseNN2
 
 import os
 import sys
 import random
 import argparse
 from sklearn.model_selection import train_test_split
-from dispersenn2.check_params import check_params
-from dispersenn2.read_input import list2dict
-from dispersenn2.read_input import read_list
-from dispersenn2.read_input import read_locs
-from dispersenn2.read_input import dict_from_preprocessed
-from dispersenn2.process_input import project_locs, vcf2genos
+from disperseNN2.check_params import check_params
+from disperseNN2.read_input import list2dict
+from disperseNN2.read_input import read_list
+from disperseNN2.read_input import read_locs
+from disperseNN2.read_input import dict_from_preprocessed
+from disperseNN2.process_input import project_locs, vcf2genos
 import gpustat
 import itertools
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 def load_dl_modules():  # load TF only if reading input is successfull
     print("loading bigger modules")
     global tf
     import tensorflow as tf
     global DataGenerator
-    from dispersenn2.data_generation import DataGenerator  # (loads TF)
+    from disperseNN2.data_generation import DataGenerator  # (loads TF)
 
     return
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--preprocess",
@@ -313,15 +313,14 @@
                 filter_size,
                 kernel_size=conv_kernal_size,
                 activation="relu",
                 name="CONV_" + str(i),
             )
         )
     DENSE_0 = tf.keras.layers.Dense(128, activation="relu", name="DENSE_0")
-    DENSE_1 = tf.keras.layers.Dense(128, activation="relu", name="DENSE_1")
 
     # convolutions for each pair
     hs = []
     for comb in combinations:
         h = tf.gather(geno_input, comb, axis=2)
         locs = tf.gather(loc_input, comb, axis=2)
         d = locs[:, :, 0] - locs[:, :, 1]
@@ -341,22 +340,20 @@
             h = tf.keras.layers.Flatten()(h)
             h = tf.keras.layers.concatenate([h, d])
             h = tf.stop_gradient(DENSE_0(h))
         # (unindent)
         hs.append(h)
     # (unindent)
     feature_block = tf.stack(hs, axis=1)
-    print("\nfeature block:", feature_block.shape)
-
-    # apply 2d dense layer
-    h = DENSE_1(feature_block)
 
     # flatten and final dense
-    h = tf.keras.layers.Flatten()(h)
-    output = tf.keras.layers.Dense(1, activation="linear")(h)
+    feature_block = tf.keras.layers.Flatten()(feature_block)
+    output = tf.keras.layers.Dense(1,
+                                   activation="linear",
+                                   name="DENSE_1")(feature_block)
 
     # model overview and hyperparams
     opt = tf.keras.optimizers.Adam(learning_rate=args.learning_rate)
     model = tf.keras.Model(
         inputs=[geno_input, loc_input],
         outputs=[output],
     )
@@ -631,15 +628,15 @@
     else:
         args.n, args.num_snps, meanSid, sdSig = np.load(args.training_mean_sd)
     args.n, args.num_snps = int(args.n), int(args.num_snps)
 
     # grab num pairs from saved training params
     params = np.load(args.out + "/Train/training_params_"
                      + str(args.seed) + ".npy")
-    args.pairs, args.num_pairs = int(params[4]), int(params[5])
+    args.pairs, args.pairs_encode = int(params[4]), int(params[5])
 
     # load inputs
     targets, genos, locs = dict_from_preprocessed(args.out + "/Test/")
     total_sims = len(targets)
 
     # organize "partition" to hand to data generator
     partition = {}
@@ -701,15 +698,15 @@
     else:
         args.n, args.num_snps, meanSid, sdSig = np.load(args.training_mean_sd)
     args.n, args.num_snps = int(args.n), int(args.num_snps)
 
     # grab num pairs from saved training params
     params = np.load(args.out + "/Train/training_params_"
                      + str(args.seed) + ".npy")
-    args.pairs, args.num_pairs = int(params[4]), int(params[5])
+    args.pairs, args.pairs_encode = int(params[4]), int(params[5])
 
     # project locs
     locs = read_locs(args.empirical + ".locs")
     locs = np.array(locs)
     if len(locs) != args.n:
         print("length of locs file doesn't match n")
         exit()
```

### Comparing `dispersenn2-0.0.3/dispersenn2/process_input.py` & `dispersenn2-0.0.4/disperseNN2/process_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import sys
 from geopy import distance
 import random
 import utm
 import tskit
-from dispersenn2.read_input import parse_provenance
+from disperseNN2.read_input import parse_provenance
 
 
 # project sample locations
 def project_locs(locs, fp=None):
     # projection (plus some code for calculating error)
     locs = np.array(locs)
     locs = np.array(utm.from_latlon(locs[:, 0], locs[:, 1])[0:2]) / 1000
```

### Comparing `dispersenn2-0.0.3/dispersenn2/read_input.py` & `dispersenn2-0.0.4/disperseNN2/read_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.3/PKG-INFO` & `dispersenn2-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispersenn2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neural net for estimating dispersal distance
 Author: chriscrsmith
 Author-email: chriscs@uoregon.edu
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

