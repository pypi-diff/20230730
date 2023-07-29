# Comparing `tmp/Seance-0.0.4-py3-none-any.whl.zip` & `tmp/Seance-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15513 bytes, number of entries: 16
+Zip file size: 15609 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat     2360 b- defN 23-Jun-21 13:29 Seance/Explainer.py
--rw-rw-rw-  2.0 fat    11987 b- defN 23-Jul-22 12:20 Seance/Forecaster.py
--rw-rw-rw-  2.0 fat    10533 b- defN 23-Jul-22 03:43 Seance/Optimizer.py
+-rw-rw-rw-  2.0 fat    11987 b- defN 23-Jul-29 23:02 Seance/Forecaster.py
+-rw-rw-rw-  2.0 fat    10887 b- defN 23-Jul-29 23:01 Seance/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:41 Seance/__init__.py
 -rw-rw-rw-  2.0 fat     3358 b- defN 23-May-18 13:18 Seance/Builder/PanelAxis.py
 -rw-rw-rw-  2.0 fat     3916 b- defN 23-Jul-06 20:13 Seance/Builder/PreProcess.py
 -rw-rw-rw-  2.0 fat     6595 b- defN 23-May-31 15:17 Seance/Builder/Transformations.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:40 Seance/Builder/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Jun-03 01:07 Seance/basis_functions/__init__.py
 -rw-rw-rw-  2.0 fat      845 b- defN 23-Jul-06 19:45 Seance/basis_functions/fourier_basis.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-May-31 21:10 Seance/basis_functions/linear_basis.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2725 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1303 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/RECORD
-16 files, 47723 bytes uncompressed, 13365 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2725 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1303 b- defN 23-Jul-29 23:03 Seance-0.0.5.dist-info/RECORD
+16 files, 48077 bytes uncompressed, 13461 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: Seance/basis_functions/fourier_basis.py
 Comment: 
 
 Filename: Seance/basis_functions/linear_basis.py
 Comment: 
 
-Filename: Seance-0.0.4.dist-info/LICENSE
+Filename: Seance-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: Seance-0.0.4.dist-info/METADATA
+Filename: Seance-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: Seance-0.0.4.dist-info/WHEEL
+Filename: Seance-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: Seance-0.0.4.dist-info/top_level.txt
+Filename: Seance-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: Seance-0.0.4.dist-info/RECORD
+Filename: Seance-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Seance/Optimizer.py

```diff
@@ -148,18 +148,24 @@
                 params['lags'] = list(range(1, params['lags']))
             else:
                 params.update({'lags': trial.suggest_int(name="lags", low=1, high=13)})
                 params['lags'] = list(range(1, params['lags']))
         score = self.scorer(params, self.metric)
         return score
 
+    def callback(study, trial):
+        if len(study.get_trials()) == 2:
+            study.stop()
+
     def fit(self, seed):
         self.get_splits(self.df, self.id_column)
         study = optuna.create_study(direction="minimize", sampler=optuna.samplers.TPESampler(seed=seed))
-        study.optimize(self.objective, n_trials=self.n_trials)
+        study.optimize(self.objective,
+                       n_trials=self.n_trials,
+                       timeout=self.timeout)
         best_params = study.best_params
         if best_params['lags'] == 1:
             best_params.update({'lags': [study.best_params['lags']]})
         elif isinstance(best_params['lags'], list):
             pass
         else:
             best_params.update({'lags': list(range(1, best_params['lags']))})
@@ -174,26 +180,32 @@
     #             id_column='ID',
     #             freq='H',
     #             metric='smape',
     #             seasonal_period=24,
     #             test_size=72,
     #             n_trials=50)
     # best_params, study = opt.fit(seed=1)
-
+    import time
+    tic = time.perf_counter()
     opt = Optimize(train_df[['V', 'Datetime', 'ID']],
                 target_column='V',
                 date_column='Datetime',
                 id_column='ID',
                 freq='W',
                 metric='smape',
-                seasonal_period=[52],
+                seasonal_period=None,
+                # ar_lags=[list(range(1, 4))],
                 test_size=26,
-                n_trials=50)
+                n_trials=10,
+                timeout=60)
     best_params, study = opt.fit(seed=1)
+    toc = time.perf_counter()
+    print(toc - tic)
 
+#%%
     look = opt.test_df
     look2 = opt.predicted
     merged = opt.test_df.merge(opt.predicted, on=['ID', 'Datetime'])
     optuna.visualization.matplotlib.plot_param_importances(study)
     optuna.visualization.matplotlib.plot_optimization_history(study)
     optuna.visualization.plot_contour(study).show(renderer="browser")
     best_params = study.best_params
```

## Comparing `Seance-0.0.4.dist-info/LICENSE` & `Seance-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Seance-0.0.4.dist-info/METADATA` & `Seance-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Seance
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Wrapper around MLForecast.
 Home-page: https://github.com/tblume1992/Seance
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm,mlforecast
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `Seance-0.0.4.dist-info/RECORD` & `Seance-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Seance/Explainer.py,sha256=ViUQvXZhsyrKjAscA88NOmBZEXwBl6pldjKe8IJ_fT0,2360
 Seance/Forecaster.py,sha256=exTxoAirjiDFNlvKDHlovpHP5RH2LU8oEk3xCEIvyJ8,11987
-Seance/Optimizer.py,sha256=ekfQHFRtK_guUSkuE1l0ZBXVdKbwx6akOEVfv1U9DI4,10533
+Seance/Optimizer.py,sha256=rUcoC1Zv0YMS8riK7NW-Nei2t2j4Q_3MGnuk2yK0btU,10887
 Seance/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/Builder/PanelAxis.py,sha256=w5YYnDXgprHWUzCWcqqBEkV1xJ_6qLabzW_PIbQF9ZQ,3358
 Seance/Builder/PreProcess.py,sha256=lXDwzPEYw_01pDEB9533v60uqYJEQE7Jb12vjIxmWhA,3916
 Seance/Builder/Transformations.py,sha256=JY27tWWvxha2JXhVgOALQFJUhV-N2Hcmg2u9hhBSeaA,6595
 Seance/Builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/fourier_basis.py,sha256=8KePMSK7FGqu9t_mkir101B2OvJGZ-FY9kqepiJSCyw,845
 Seance/basis_functions/linear_basis.py,sha256=1RHj--VkbA4heV8QwzNE7a9O0-aPu3Br3EqLlcuUHWU,2834
-Seance-0.0.4.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
-Seance-0.0.4.dist-info/METADATA,sha256=WFmB5Z7q-op0jZHzpjRXWNlNVVrtfVyhoQNjJwmOako,2725
-Seance-0.0.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Seance-0.0.4.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
-Seance-0.0.4.dist-info/RECORD,,
+Seance-0.0.5.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
+Seance-0.0.5.dist-info/METADATA,sha256=MVj3RASdJ4lDUiAJY7_lepUNjZb0kZaFlu1jZluCcmc,2725
+Seance-0.0.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Seance-0.0.5.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
+Seance-0.0.5.dist-info/RECORD,,
```

