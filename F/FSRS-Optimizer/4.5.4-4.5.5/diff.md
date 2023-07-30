# Comparing `tmp/FSRS-Optimizer-4.5.4.tar.gz` & `tmp/FSRS-Optimizer-4.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.5.4.tar", last modified: Sun Jul 30 06:24:25 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.5.5.tar", last modified: Sun Jul 30 07:29:37 2023, max compression
```

## Comparing `FSRS-Optimizer-4.5.4.tar` & `FSRS-Optimizer-4.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.339409 FSRS-Optimizer-4.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 06:24:25.000000 FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:24:25.343409 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52608 2023-07-30 06:24:14.000000 FSRS-Optimizer-4.5.4/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 07:29:37.194986 FSRS-Optimizer-4.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52743 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.5.4/LICENSE` & `FSRS-Optimizer-4.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.4/PKG-INFO` & `FSRS-Optimizer-4.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.4
+Version: 4.5.5
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.4/README.md` & `FSRS-Optimizer-4.5.5/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.4/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.4
+Version: 4.5.5
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.5.4/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.5.5/src/fsrs_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.4/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.5.5/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         :return state:
         '''
         if torch.equal(state, torch.zeros_like(state)):
             keys = torch.tensor([1, 2, 3, 4])
             keys = keys.view(1, -1).expand(X[:,1].long().size(0), -1)
             index = (X[:,1].long().unsqueeze(1) == keys).nonzero(as_tuple=True)
             # first learn, init memory states
-            new_s = self.w[index[1]]
+            new_s = torch.ones_like(state[:,0])
+            new_s[index[0]] = self.w[index[1]]
             new_d = self.w[4] - self.w[5] * (X[:,1] - 3)
             new_d = new_d.clamp(1, 10)
         else:
             r = power_forgetting_curve(X[:,0], state[:,0])
             new_d = state[:,1] - self.w[6] * (X[:,1] - 3)
             new_d = self.mean_reversion(self.w[4], new_d)
             new_d = new_d.clamp(1, 10)
@@ -397,28 +398,29 @@
             return list(accumulate(x))
 
         t_history = df.groupby('card_id', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
         r_history = df.groupby('card_id', group_keys=False)['review_rating'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
         df = df.groupby('card_id').filter(lambda group: group['review_time'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
-        df = df[df['review_rating'] != 0].copy()
+        df = df[(df['review_rating'] != 0) & (df['r_history'].str.contains("0") == 0)].copy()
         df['y'] = df['review_rating'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
 
         def remove_outliers(group: pd.DataFrame) -> pd.DataFrame:
             # threshold = np.mean(group['delta_t']) * 1.5
             # threshold = group['delta_t'].quantile(0.95)
             Q1 = group['delta_t'].quantile(0.25)
             Q3 = group['delta_t'].quantile(0.75)
             IQR = Q3 - Q1
             threshold = Q3 + 1.5 * IQR
             group = group[group['delta_t'] <= threshold]
             return group
 
         df[df['i'] == 2] = df[df['i'] == 2].groupby(by=['r_history', 't_history'], as_index=False, group_keys=False).apply(remove_outliers)
+        df.dropna(inplace=True)
 
         def remove_non_continuous_rows(group):
             discontinuity = group['i'].diff().fillna(1).ne(1)
             if not discontinuity.any():
                 return group
             else:
                 first_non_continuous_index = discontinuity.idxmax()
```

