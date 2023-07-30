# Comparing `tmp/stable-trunc-gaussian-1.0.1.tar.gz` & `tmp/stable-trunc-gaussian-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-trunc-gaussian-1.0.1.tar", last modified: Tue Jul 25 20:54:32 2023, max compression
+gzip compressed data, was "stable-trunc-gaussian-1.1.0.tar", last modified: Sun Jul 30 04:24:30 2023, max compression
```

## Comparing `stable-trunc-gaussian-1.0.1.tar` & `stable-trunc-gaussian-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.0.1/LICENSE
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.0.1/MANIFEST.in
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     3407 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1557 2023-07-25 18:41:21.000000 stable-trunc-gaussian-1.0.1/README.md
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-25 20:47:54.000000 stable-trunc-gaussian-1.0.1/pyproject.toml
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/setup.cfg
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/src/
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       73 2023-07-25 20:47:19.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/__init__.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7319 2023-07-25 20:46:56.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/src.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4085 2023-07-25 20:50:46.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/tests.py
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     3407 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      394 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/SOURCES.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/dependency_links.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/requires.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/top_level.txt
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.1.0/LICENSE
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.1.0/MANIFEST.in
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4580 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     2730 2023-07-30 04:20:01.000000 stable-trunc-gaussian-1.1.0/README.md
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-30 04:22:54.000000 stable-trunc-gaussian-1.1.0/pyproject.toml
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/setup.cfg
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.741945 stable-trunc-gaussian-1.1.0/src/
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.741945 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      213 2023-07-30 04:23:15.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/__init__.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)    11308 2023-07-30 03:54:38.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/parallel_trunc_gaussian.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7429 2023-07-30 03:59:16.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/sequential_trunc_gaussian.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4095 2023-07-30 04:02:06.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/tests.py
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4580 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      469 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/SOURCES.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/dependency_links.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/requires.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/top_level.txt
```

### Comparing `stable-trunc-gaussian-1.0.1/LICENSE` & `stable-trunc-gaussian-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.0.1/PKG-INFO` & `stable-trunc-gaussian-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.0.1
+Version: 1.1.0
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+`[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+[![Downloads](https://static.pepy.tech/badge/stable-trunc-gaussian)](https://pepy.tech/project/stable-trunc-gaussian)
 
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
 Simply install with `pip`:
@@ -61,8 +62,21 @@
     print("Log-prob(10.5):", dist.log_prob(t(10.5)))
     
 Result:
 
     Mean: tensor(10.0981)
     Variance: tensor(0.0094)
     Log-prob(10.5): tensor(-2.8126)
-    
+
+## Parallel vs Sequential Implementation
+The class obtained by doing `from stable_trunc_gaussian import TruncatedGaussian` corresponds to a **parallel** implementation of the truncated gaussian, which makes possible to obtain several values (mean, variance and log-probs) in parallel. In case you are only interested in computing values sequentially, i.e., one at a time, we also provide a **sequential** implementation which results more efficient *only* for this case. In order to use this sequential implementation, simply do `from stable_trunc_gaussian import SeqTruncatedGaussian`. Here is an example:
+
+    from stable_trunc_gaussian import TruncatedGaussian, SeqTruncatedGaussian
+    from torch import tensor as t
+
+    # Parallel computation
+    means = TruncatedGaussian(t([0,0.5]),t(1,1),t(-1,2),t(1,5)).mean
+
+    # Sequential computation
+    # Note: the 'TruncatedGaussian' class can also be used for this sequential case
+    mean_0 = SeqTruncatedGaussian(t([0]),t(1),t(-1),t(1)).mean
+    mean_1 = SeqTruncatedGaussian(t([0.5]),t(1),t(2),t(5)).mean
```

### Comparing `stable-trunc-gaussian-1.0.1/README.md` & `stable-trunc-gaussian-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+`[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+[![Downloads](https://static.pepy.tech/badge/stable-trunc-gaussian)](https://pepy.tech/project/stable-trunc-gaussian)
 
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
 Simply install with `pip`:
@@ -25,8 +26,21 @@
     print("Log-prob(10.5):", dist.log_prob(t(10.5)))
     
 Result:
 
     Mean: tensor(10.0981)
     Variance: tensor(0.0094)
     Log-prob(10.5): tensor(-2.8126)
-    
+
+## Parallel vs Sequential Implementation
+The class obtained by doing `from stable_trunc_gaussian import TruncatedGaussian` corresponds to a **parallel** implementation of the truncated gaussian, which makes possible to obtain several values (mean, variance and log-probs) in parallel. In case you are only interested in computing values sequentially, i.e., one at a time, we also provide a **sequential** implementation which results more efficient *only* for this case. In order to use this sequential implementation, simply do `from stable_trunc_gaussian import SeqTruncatedGaussian`. Here is an example:
+
+    from stable_trunc_gaussian import TruncatedGaussian, SeqTruncatedGaussian
+    from torch import tensor as t
+
+    # Parallel computation
+    means = TruncatedGaussian(t([0,0.5]),t(1,1),t(-1,2),t(1,5)).mean
+
+    # Sequential computation
+    # Note: the 'TruncatedGaussian' class can also be used for this sequential case
+    mean_0 = SeqTruncatedGaussian(t([0]),t(1),t(-1),t(1)).mean
+    mean_1 = SeqTruncatedGaussian(t([0.5]),t(1),t(2),t(5)).mean
```

### Comparing `stable-trunc-gaussian-1.0.1/pyproject.toml` & `stable-trunc-gaussian-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="stable-trunc-gaussian"
-version="1.0.1"
+version="1.1.0"
 description="A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch."
 readme="README.md"
 authors = [{ name = "Carlos Núñez Molina", email = "ccaarlos@ugr.es" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/src.py` & `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/sequential_trunc_gaussian.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 SQRT_2_PI = math.sqrt(2*math.pi)
 INV_SQRT_2 = 1/SQRT_2
 INV_SQRT_PI = 1/SQRT_PI
 INV_PI = 1/math.pi
 LOG_SQRT_2_PI = math.log(SQRT_2_PI)
 LOG_2 = math.log(2)
 
-class TruncatedGaussian(Distribution):
+class SequentialTruncatedGaussian(Distribution):
 
 	has_rsample = False
 
 	arg_constraints = {
 		'mu': constraints.real,
 		'sigma': constraints.positive,
 		'a': constraints.real,
@@ -128,43 +128,43 @@
 		t3 = -(1/3)*SQRT_PI*x*eps**3
 		t4 = (1/90)*SQRT_PI*(2*x**4+3*x**2-8)*eps**4
 		return t0 + t1 + t2 + t3 + t4
 	
 	@staticmethod
 	def _F_1(x, y):
 		if torch.abs(x) > torch.abs(y):
-			out = TruncatedGaussian._F_1(y, x)
+			out = SequentialTruncatedGaussian._F_1(y, x)
 		elif torch.abs(x - y) < 1e-7:
-			out = TruncatedGaussian._P_1(x, y-x)
+			out = SequentialTruncatedGaussian._P_1(x, y-x)
 		elif x <= 0 and y <= 0:
-			delt = TruncatedGaussian._delta(x, y)
+			delt = SequentialTruncatedGaussian._delta(x, y)
 			out = (1 - delt) / (delt*erfcx(-y) - erfcx(-x))  
 		elif x >= 0 and y >= 0:
-			delt = TruncatedGaussian._delta(x, y)
+			delt = SequentialTruncatedGaussian._delta(x, y)
 			out = (1 - delt) / (erfcx(x) - delt*erfcx(y))
 		else:
-			delt = TruncatedGaussian._delta(x, y)
+			delt = SequentialTruncatedGaussian._delta(x, y)
 			out = ((1-delt)*torch.exp(-x**2)) / (erf(y)-erf(x))
 
 		return out
 	
 	@staticmethod
 	def _F_2(x, y):
 		if torch.abs(x) > torch.abs(y):
-			out = TruncatedGaussian._F_2(y, x)
+			out = SequentialTruncatedGaussian._F_2(y, x)
 		elif torch.abs(x - y) < 1e-7:
-			out = TruncatedGaussian._P_2(x, y-x)
+			out = SequentialTruncatedGaussian._P_2(x, y-x)
 		elif x <= 0 and y <= 0:
-			delt = TruncatedGaussian._delta(x, y)
+			delt = SequentialTruncatedGaussian._delta(x, y)
 			out = (x - y*delt) / (delt*erfcx(-y) - erfcx(-x))  
 		elif x >= 0 and y >= 0:
-			delt = TruncatedGaussian._delta(x, y)
+			delt = SequentialTruncatedGaussian._delta(x, y)
 			out = (x - y*delt) / (erfcx(x) - delt*erfcx(y))
 		else:
-			delt = TruncatedGaussian._delta(x, y)
+			delt = SequentialTruncatedGaussian._delta(x, y)
 			out = ((x-y*delt)*torch.exp(-x**2)) / (erf(y)-erf(x))
 
 		return out
 	
 	# Numerically stable implementation of Z=log(big_phi(beta)-big_phi(alpha))
 	def _calculate_log_Z(self):
```

### Comparing `stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/tests.py` & `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Tests for truncated gaussian
 # I compare the values obtained with my code against those returned by scipy.stats.truncnorm
 
-from stable_trunc_gaussian import TruncatedGaussian as TG
+from parallel_trunc_gaussian import ParallelTruncatedGaussian as TG
 from scipy.stats import truncnorm
 from torch import tensor as t
 import math
 
 """
 Current results:
     - Variance calculation seems to differ sometimes with scipy.
```

### Comparing `stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/PKG-INFO` & `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.0.1
+Version: 1.1.0
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+`[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+[![Downloads](https://static.pepy.tech/badge/stable-trunc-gaussian)](https://pepy.tech/project/stable-trunc-gaussian)
 
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
 Simply install with `pip`:
@@ -61,8 +62,21 @@
     print("Log-prob(10.5):", dist.log_prob(t(10.5)))
     
 Result:
 
     Mean: tensor(10.0981)
     Variance: tensor(0.0094)
     Log-prob(10.5): tensor(-2.8126)
-    
+
+## Parallel vs Sequential Implementation
+The class obtained by doing `from stable_trunc_gaussian import TruncatedGaussian` corresponds to a **parallel** implementation of the truncated gaussian, which makes possible to obtain several values (mean, variance and log-probs) in parallel. In case you are only interested in computing values sequentially, i.e., one at a time, we also provide a **sequential** implementation which results more efficient *only* for this case. In order to use this sequential implementation, simply do `from stable_trunc_gaussian import SeqTruncatedGaussian`. Here is an example:
+
+    from stable_trunc_gaussian import TruncatedGaussian, SeqTruncatedGaussian
+    from torch import tensor as t
+
+    # Parallel computation
+    means = TruncatedGaussian(t([0,0.5]),t(1,1),t(-1,2),t(1,5)).mean
+
+    # Sequential computation
+    # Note: the 'TruncatedGaussian' class can also be used for this sequential case
+    mean_0 = SeqTruncatedGaussian(t([0]),t(1),t(-1),t(1)).mean
+    mean_1 = SeqTruncatedGaussian(t([0.5]),t(1),t(2),t(5)).mean
```

