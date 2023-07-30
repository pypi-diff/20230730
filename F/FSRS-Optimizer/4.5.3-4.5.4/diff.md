# Comparing `tmp/FSRS-Optimizer-4.5.3.tar.gz` & `tmp/FSRS-Optimizer-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.5.3.tar", last modified: Sun Jul 30 03:06:24 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.5.4.tar", last modified: Sun Jul 30 06:24:25 2023, max compression
```

## Comparing `FSRS-Optimizer-4.5.3.tar` & `FSRS-Optimizer-4.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 03:06:24.000000 FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:06:24.232139 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52297 2023-07-30 03:06:10.000000 FSRS-Optimizer-4.5.3/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.339409 FSRS-Optimizer-4.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52608 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.5.3/LICENSE` & `FSRS-Optimizer-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.3/PKG-INFO` & `FSRS-Optimizer-4.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.3
+Version: 4.5.4
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.3/README.md` & `FSRS-Optimizer-4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.3/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.3
+Version: 4.5.4
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.3/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.5.4/src/fsrs_optimizer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,17 @@
     print("Paste this into your scheduling code")
     print(profile)
 
     if args.out:
         with open(args.out, "a+") as f:
             f.write(profile)
 
-    optimizer.evaluate()
+    loss_before, loss_after = optimizer.evaluate()
+    print(f"Loss before training: {loss_before:.4f}")
+    print(f"Loss after training: {loss_after:.4f}")
     if save_graphs:
         for i, f in enumerate(optimizer.calibration_graph()):
             f.savefig(f"calibration_{i}.png")
         for i, f in enumerate(optimizer.compare_with_sm2()):
             f.savefig(f"compare_with_sm2_{i}.png")
 
 if __name__ == "__main__":
@@ -139,14 +141,15 @@
     curdir = os.getcwd()
     for filename in args.filenames:
         if os.path.isdir(filename):
             files = [f for f in os.listdir(filename) if f.lower().endswith('.apkg')]
             files = [os.path.join(filename, f) for f in files]
             for file_path in files:
                 try:
+                    print(f"Processing {file_path}")
                     process(file_path)
                 except Exception as e:
                     print(e)
                     print(f"Failed to process {file_path}")
                 finally:
                     plt.close('all')
                     os.chdir(curdir)
```

### Comparing `FSRS-Optimizer-4.5.3/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.5.4/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch
 from torch import nn
 from torch import Tensor
 from torch.utils.data import Dataset, DataLoader, Sampler
 from torch.nn.utils.rnn import pad_sequence, pack_padded_sequence, pad_packed_sequence
 from sklearn.model_selection import StratifiedGroupKFold
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score
-from scipy.optimize import curve_fit
+from scipy.optimize import curve_fit, minimize
 from itertools import accumulate
 from tqdm.auto import tqdm
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 
 New = 0
 Learning = 1
@@ -493,28 +493,42 @@
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         if self.dataset.empty:
             raise ValueError('Training data is inadequate.')
         rating_stability = {}
         rating_count = {}
         average_recall = self.dataset['y'].mean()
         plots = []
+        s0_size = self.S0_dataset_group.shape[0]
+        rating_s0 = {
+            "1": 0.4,
+            "2": 0.6,
+            "3": 2.4,
+            "4": 5.8
+        }
 
         for first_rating in ("1", "2", "3", "4"):
             group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
             if group.empty:
-                tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got 0.')
+                tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 1, got 0.')
                 continue
             delta_t = group['delta_t']
             recall = (group['y']['mean'] * group['y']['count'] + average_recall * 1) / (group['y']['count'] + 1)
             count = group['y']['count']
             total_count = sum(count)
-            if total_count < 100:
-                tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got {total_count}.')
-                continue
-            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (30 if total_count < 1000 else 365)))
+
+            init_s0 = rating_s0[first_rating]
+            
+            def loss(stability):
+                y_pred = power_forgetting_curve(delta_t, stability)
+                rmse = np.sqrt(np.sum((recall - y_pred)** 2 * count) / total_count)
+                l1 = np.abs(stability - init_s0) / np.sqrt(s0_size) / total_count
+                return rmse + l1
+
+            res = minimize(loss, x0=init_s0, bounds=((0.1, 365),), options={"maxiter": int(np.sqrt(total_count))})
+            params = res.x
             stability = params[0]
             rating_stability[int(first_rating)] = stability
             rating_count[int(first_rating)] = total_count
             predict_recall = power_forgetting_curve(delta_t, *params)
             rmse = mean_squared_error(recall, predict_recall, sample_weight=count, squared=False)
 
             if verbose:
@@ -523,15 +537,14 @@
                 ax.plot(delta_t, recall, label='Exact')
                 ax.plot(np.linspace(0, 30), power_forgetting_curve(np.linspace(0, 30), *params), label=f'Weighted fit (RMSE: {rmse:.4f})')
                 count_percent = np.array([x/total_count for x in count])
                 ax.scatter(delta_t, recall, s=count_percent * 1000, alpha=0.5)
                 ax.legend(loc='upper right', fancybox=True, shadow=False)
                 ax.grid(True)
                 ax.set_ylim(0, 1)
-                ax.set_xlim(0, 30)
                 ax.set_xlabel('Interval')
                 ax.set_ylabel('Recall')
                 ax.set_title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
                 plots.append(fig)
                 tqdm.write(str(rating_stability))
 
         if len(rating_stability) == 0:
```

