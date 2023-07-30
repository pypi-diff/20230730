# Comparing `tmp/manic-xai-0.1.1.tar.gz` & `tmp/manic-xai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manic-xai-0.1.1.tar", last modified: Fri Jul 28 00:13:42 2023, max compression
+gzip compressed data, was "manic-xai-1.0.4.tar", last modified: Sun Jul 30 17:33:33 2023, max compression
```

## Comparing `manic-xai-0.1.1.tar` & `manic-xai-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.517598 manic-xai-0.1.1/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-0.1.1/LICENSE
--rw-r--r--   0 craigpirie   (501) staff       (20)      315 2023-07-28 00:13:42.517204 manic-xai-0.1.1/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-0.1.1/README.md
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.509385 manic-xai-0.1.1/manic/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1305 2023-07-27 14:07:07.000000 manic-xai-0.1.1/manic/Baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2774 2023-07-27 23:07:34.000000 manic-xai-0.1.1/manic/Crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4367 2023-07-27 21:11:16.000000 manic-xai-0.1.1/manic/Disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     3050 2023-07-27 23:06:27.000000 manic-xai-0.1.1/manic/Evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 10:52:56.000000 manic-xai-0.1.1/manic/Fitness.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5392 2023-07-27 15:42:32.000000 manic-xai-0.1.1/manic/Initialise.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     8602 2023-07-27 23:08:52.000000 manic-xai-0.1.1/manic/Manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1688 2023-07-27 10:14:30.000000 manic-xai-0.1.1/manic/Mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2009 2023-07-27 23:52:30.000000 manic-xai-0.1.1/manic/Selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      379 2023-07-27 13:22:11.000000 manic-xai-0.1.1/manic/Termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5620 2023-07-27 20:53:42.000000 manic-xai-0.1.1/manic/Utility.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      400 2023-07-27 23:27:35.000000 manic-xai-0.1.1/manic/__init__.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.514073 manic-xai-0.1.1/manic/__tests__/
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-0.1.1/manic/__tests__/__init__.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     8075 2023-07-26 16:51:28.000000 manic-xai-0.1.1/manic/__tests__/test_attributes.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2021 2023-07-26 16:47:08.000000 manic-xai-0.1.1/manic/__tests__/test_crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     3400 2023-07-26 16:45:04.000000 manic-xai-0.1.1/manic/__tests__/test_initialise.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5512 2023-07-26 16:39:06.000000 manic-xai-0.1.1/manic/__tests__/test_initialise_population.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-0.1.1/manic/__tests__/test_manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2309 2023-07-26 16:41:56.000000 manic-xai-0.1.1/manic/__tests__/test_manic_reproducibility.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2106 2023-07-26 16:40:49.000000 manic-xai-0.1.1/manic/__tests__/test_mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2645 2023-07-28 00:03:18.000000 manic-xai-0.1.1/manic/__tests__/test_selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4412 2023-07-26 17:01:13.000000 manic-xai-0.1.1/manic/__tests__/test_validity.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1833 2023-07-27 09:50:27.000000 manic-xai-0.1.1/manic/test.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-28 00:13:42.516597 manic-xai-0.1.1/manic_xai.egg-info/
--rw-r--r--   0 craigpirie   (501) staff       (20)      315 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)      782 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/SOURCES.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/dependency_links.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       35 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/requires.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-07-28 00:13:42.000000 manic-xai-0.1.1/manic_xai.egg-info/top_level.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-07-28 00:13:42.517717 manic-xai-0.1.1/setup.cfg
--rw-r--r--   0 craigpirie   (501) staff       (20)      492 2023-07-28 00:13:17.000000 manic-xai-0.1.1/setup.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.237064 manic-xai-1.0.4/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.4/LICENSE
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-07-30 17:33:33.236779 manic-xai-1.0.4/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.4/README.md
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.226090 manic-xai-1.0.4/manic/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1305 2023-07-27 14:07:07.000000 manic-xai-1.0.4/manic/Baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3057 2023-07-28 17:08:55.000000 manic-xai-1.0.4/manic/Crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4913 2023-07-28 16:49:09.000000 manic-xai-1.0.4/manic/Disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3076 2023-07-28 15:13:20.000000 manic-xai-1.0.4/manic/Evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 10:52:56.000000 manic-xai-1.0.4/manic/Fitness.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5468 2023-07-29 20:37:26.000000 manic-xai-1.0.4/manic/Initialise.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     8533 2023-07-28 18:00:44.000000 manic-xai-1.0.4/manic/Manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2754 2023-07-28 12:57:57.000000 manic-xai-1.0.4/manic/Mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3470 2023-07-28 12:05:18.000000 manic-xai-1.0.4/manic/Selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      379 2023-07-27 13:22:11.000000 manic-xai-1.0.4/manic/Termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5693 2023-07-28 17:55:48.000000 manic-xai-1.0.4/manic/Utility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      400 2023-07-27 23:27:35.000000 manic-xai-1.0.4/manic/__init__.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.234849 manic-xai-1.0.4/manic/__tests__/
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.4/manic/__tests__/__init__.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.4/manic/__tests__/test_baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.4/manic/__tests__/test_crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.4/manic/__tests__/test_disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.4/manic/__tests__/test_evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3400 2023-07-26 16:45:04.000000 manic-xai-1.0.4/manic/__tests__/test_initialise.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5512 2023-07-26 16:39:06.000000 manic-xai-1.0.4/manic/__tests__/test_initialise_population.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.4/manic/__tests__/test_manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.4/manic/__tests__/test_mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.4/manic/__tests__/test_selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.4/manic/__tests__/test_termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.4/manic/__tests__/test_utility.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.236288 manic-xai-1.0.4/manic_xai.egg-info/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)      827 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/requires.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/top_level.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-07-30 17:33:33.237141 manic-xai-1.0.4/setup.cfg
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-07-30 17:33:29.000000 manic-xai-1.0.4/setup.py
```

### Comparing `manic-xai-0.1.1/LICENSE` & `manic-xai-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.1/README.md` & `manic-xai-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.1/manic/Baseline.py` & `manic-xai-1.0.4/manic/Baseline.py`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.1/manic/Crossover.py` & `manic-xai-1.0.4/manic/Crossover.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 class Crossover():
     def __init__(self, crossover_method, num_parents, population_size):
         self.crossover = self.set_crossover_method(crossover_method)
         self.num_parents = num_parents
         self.population_size = population_size
         self.parallel = False
 
+        self.validate_self()
+
     def set_crossover_method(self, crossover_method):
         if(crossover_method == "single_point"):
             return self.single_point_crossover
         elif(crossover_method == "uniform"):
             return self.single_point_crossover
         elif(crossover_method == "two_point"):
              return self.two_point_crossover
@@ -65,8 +67,15 @@
                 if random.random() < 0.5:
                     child.append(parent1[j])
                 else:
                     child.append(parent2[j])
             
             offspring.append(child)
         
-        return offspring
+        return offspring
+    
+    def validate_self(self):
+        if(self.population_size < 2):
+            raise ValueError("Population size must be at least 2.")
+        
+        if(self.num_parents < 2):
+            raise ValueError("Number of parents must be at least 2.")
```

### Comparing `manic-xai-0.1.1/manic/Disagreement.py` & `manic-xai-1.0.4/manic/Disagreement.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,23 @@
         self.predict_proba_fn = predict_proba_fn
         self.target_class = target_class
         self.calculate_disagreement = self.set_disagreement_method(disagreement_method)
         self.feature_ranges = feature_ranges
         self.normalized_instance = self.normalize_instance(data_instance)
 
     def euclidean_distance(self, instance1, instance2):
+        self.validate_instances(instance1, instance2)
+        
         normalised_instance1 = np.array(self.normalize_instance(instance1))
         normalised_instance2 = np.array(self.normalize_instance(instance2))
         return np.sqrt(np.sum((normalised_instance1 - normalised_instance2) ** 2))
 
     def calculate_cosine_distance(self, counterfactual1, counterfactual2):
+        self.validate_instances(counterfactual1, counterfactual2)
+
         normalised_counterfactual1 = self.normalize_instance(counterfactual1)
         normalised_counterfactual2 = self.normalize_instance(counterfactual2)
         return cosine(normalised_counterfactual1, normalised_counterfactual2)
 
     @lru_cache(maxsize=None)
     def median_absolute_deviation(self, data):
         data_tuple = tuple(data)
@@ -34,16 +38,16 @@
         return np.median(absolute_deviations)
 
     def normalize_instance(self,instance):
         normalized_instance = []
 
         for i, (min_val, max_val) in enumerate(self.feature_ranges):
             # Make sure the feature range is valid
-            # if min_val > max_val:
-            #     raise ValueError("Invalid feature range: min_val must be less than or equal to max_val.")
+            if min_val > max_val:
+                raise ValueError("Invalid feature range: min_val must be less than or equal to max_val.")
             
             # Normalize the feature value using min-max scaling
             feature_value = instance[i]
             if(min_val == max_val):
                 normalized_instance.append(feature_value)
             else:
                 normalized_value = (feature_value - min_val) / (max_val - min_val)
@@ -91,8 +95,16 @@
 
         for i in range(len(cf)):
             if(cf[i] != self.data_instance[i]):
                 num_changes += 1
 
         sparsity = num_changes / len(cf)
 
-        return sparsity, num_changes
+        return sparsity, num_changes
+    
+    def validate_instances(self, instance1, instance2):
+        assert len(instance1) == len(instance2), "Input instances must have the same length."
+        assert len(instance1) > 0 and len(instance2) > 0,  "Instances must not be empty"
+
+        for element in instance1 + instance2:
+            if not isinstance(element, int):
+                raise AssertionError("Instances must only contain integer values.")
```

### Comparing `manic-xai-0.1.1/manic/Evaluation.py` & `manic-xai-1.0.4/manic/Evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import concurrent.futures
 
 class Evaluation:
     def __init__(self, alpha, beta, predict_proba_fn, instance_probability, base_counterfactuals, disagreement, data_instance, theta):
         self.alpha = alpha
         self.beta = beta
         self.predict_proba_fn = predict_proba_fn
         self.instance_probability = instance_probability
```

### Comparing `manic-xai-0.1.1/manic/Initialise.py` & `manic-xai-1.0.4/manic/Initialise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import random
 import heapq
 import numpy as np
 
-import Baseline
-import Disagreement
-import Evaluation
-import Selection
-import Utility
+from Baseline import Baseline
+from Disagreement import Disagreement
+from Evaluation import Evaluation
+from Selection import Selection
+from Utility import Utility
 
 class Initialise:
     def __init__(self, disagreement_method, data_instance, base_counterfactuals, predict_fn, predict_proba_fn, seed, population_size, categorical_features, feature_ranges, immutable_features, data, class_labels, theta, alpha, beta, num_parents, verbose, labels):
         self.seed = seed
         self.population_size = population_size
         self.base_counterfactuals = base_counterfactuals
         self.data = data
```

### Comparing `manic-xai-0.1.1/manic/Manic.py` & `manic-xai-1.0.4/manic/Manic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import time
-import concurrent.futures
+import os
+
+from Crossover import Crossover
+from Initialise import Initialise
+from Mutation import Mutation
 
 class Manic:
     def __init__(self, data_instance, base_counterfactuals, categorical_features, immutable_features, feature_ranges, data, predict_fn, predict_proba_fn, class_labels, population_size=100, num_generations=50, alpha=0.5, beta=0.5, crossover_method="uniform", mutation_method="random_resetting", perturbation_fraction=0.1, num_parents=2, seed=42, verbose=1, early_stopping=None, max_time=None, disagreement_method="euclidean_distance", theta=0.3, labels=[]):
         self.initialise = Initialise(disagreement_method, data_instance, base_counterfactuals, predict_fn, predict_proba_fn, seed, population_size, categorical_features, feature_ranges, immutable_features, data, class_labels, theta, alpha, beta, num_parents, verbose, labels)
         self.immutable_features_set = self.initialise.immutable_features_set
         self.target_class = self.initialise.target_class
         self.instance_probability = self.initialise.instance_probability
@@ -159,20 +163,18 @@
 
         end_time = time.time()
         cpu_end_time = self.get_cpu_time()
 
                 # Calculate elapsed CPU time in seconds
         elapsed_cpu_time_seconds = cpu_end_time - cpu_start_time
 
-        # Convert CPU time to CPU cycles
         cpu_cycles = self.get_cpu_cycles(elapsed_cpu_time_seconds)
 
-        print("Elapsed CPU Time (seconds):", elapsed_cpu_time_seconds)
         print(end_time - start_time)
-        print("Estimated CPU Cycles:", cpu_cycles)
+
 
         time_taken = end_time - start_time
 
         if self.verbose > 0:
-            self.print_results(self.best_counterfactual, self.best_fitness, generation + 1, self.generation_found, time_taken, self.time_found)
+            self.print_results(self.best_counterfactual, self.best_fitness, generation + 1, self.generation_found, time_taken, self.time_found, cpu_cycles)
 
         return self.best_counterfactual
```

### Comparing `manic-xai-0.1.1/manic/Utility.py` & `manic-xai-1.0.4/manic/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         # All conditions are met, counterfactual is valid
         if self.verbose > 0:
             print("Valid Counterfactual: No immutable features were changed and the counterfactual causes the correct prediction change.")
 
         return True
     
-    def print_results(self, best_counterfactual, best_fitness, num_generations, generation_found, time_taken, time_found):
+    def print_results(self, best_counterfactual, best_fitness, num_generations, generation_found, time_taken, time_found, cpu_cycles):
         print("\n------ Counterfactual Generation Results ------")
         if best_counterfactual is not None:
             proximity_score = self.disagreement.calculate_proximity(self.data_instance, best_counterfactual, True)
             sparsity_score, number_of_changes = self.disagreement.calculate_sparsity(best_counterfactual)
             agreement_score = self.evaluation.calculate_base_cf_scores([best_counterfactual], self.base_counterfactuals[0])
             print(f"{np.array2string(np.array(best_counterfactual), separator=', ')}: Best Counterfactual 👑")
             print(f"{np.array2string(np.array(self.data_instance), separator=', ')}: Instance Explained 🔍")
@@ -74,14 +74,15 @@
             print("Number of changes made to produce the counterfactual:", number_of_changes)
             print("Agreement Score against Base Counterfactuals:", agreement_score)
             print("Number of Generations:", num_generations)
             print(f"Counterfactual found after {generation_found + 1} generations")
             print("Fitness Score:", best_fitness)
             print(f"Time taken to find counterfactual: {time_found:.4f} seconds")
             print(f"Total time searched: {time_taken:.4f} seconds")
+            print(f"Total CPU cycles ran: {cpu_cycles:.4f}")
         else:
             print("No valid counterfactual found within the specified number of generations.")
             print("Try increasing the number of generations or population size and/or altering alpha, beta and/or perturbation_fraction. As a last resort, you can also try changing the seed.")
         print("------ End of Results ------\n")
```

### Comparing `manic-xai-0.1.1/manic/__tests__/test_initialise.py` & `manic-xai-1.0.4/manic/__tests__/test_initialise.py`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.1/manic/__tests__/test_initialise_population.py` & `manic-xai-1.0.4/manic/__tests__/test_initialise_population.py`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.1/manic/__tests__/test_manic.py` & `manic-xai-1.0.4/manic/__tests__/test_manic.py`

 * *Files identical despite different names*

### Comparing `manic-xai-0.1.1/manic_xai.egg-info/SOURCES.txt` & `manic-xai-1.0.4/manic_xai.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 manic/Initialise.py
 manic/Manic.py
 manic/Mutation.py
 manic/Selection.py
 manic/Termination.py
 manic/Utility.py
 manic/__init__.py
-manic/test.py
 manic/__tests__/__init__.py
-manic/__tests__/test_attributes.py
+manic/__tests__/test_baseline.py
 manic/__tests__/test_crossover.py
+manic/__tests__/test_disagreement.py
+manic/__tests__/test_evaluation.py
 manic/__tests__/test_initialise.py
 manic/__tests__/test_initialise_population.py
 manic/__tests__/test_manic.py
-manic/__tests__/test_manic_reproducibility.py
 manic/__tests__/test_mutation.py
 manic/__tests__/test_selection.py
-manic/__tests__/test_validity.py
+manic/__tests__/test_termination.py
+manic/__tests__/test_utility.py
 manic_xai.egg-info/PKG-INFO
 manic_xai.egg-info/SOURCES.txt
 manic_xai.egg-info/dependency_links.txt
 manic_xai.egg-info/requires.txt
 manic_xai.egg-info/top_level.txt
```

