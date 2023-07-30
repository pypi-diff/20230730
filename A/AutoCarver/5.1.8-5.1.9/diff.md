# Comparing `tmp/AutoCarver-5.1.8.tar.gz` & `tmp/AutoCarver-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.8.tar", last modified: Thu Jul 20 10:59:00 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.9.tar", last modified: Sun Jul 30 11:57:57 2023, max compression
```

## Comparing `AutoCarver-5.1.8.tar` & `AutoCarver-5.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35655 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35455 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    32441 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 10:59:00.380810 AutoCarver-5.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35502 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35455 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32441 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.8/AutoCarver/auto_carver.py` & `AutoCarver-5.1.9/AutoCarver/auto_carver.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             **Tip**: should be set between 4 (faster, more robust) and 7 (slower, preciser, less robust)
 
         sort_by : str, optional
             To be choosen amongst ``["tschuprowt", "cramerv"]``, by default ``"tschuprowt"``
             Metric to be used to perform association measure between features and target.
 
             * ``"tschuprowt"``, Tschuprow's T will be used as the association measure (more robust).
-            * ``"cramerv"``, Cramer's V will be used as the association measure (less robust).
+            * ``"cramerv"``, Cramér's V will be used as the association measure (less robust).
 
             **Tip**: use ``"tschuprowt"`` for more robust, or less output modalities,
             use ``"cramerv"`` for more output modalities.
 
         output_dtype : str, optional
             To be choosen amongst ``["float", "str"]``, by default ``"float"``
 
@@ -543,44 +543,41 @@
 
             # storing results
             xtabs.update({feature: xtab})
 
     return xtabs
 
 
-def association_xtab(xtab: DataFrame, n_obs: int, n_mod_y: int) -> dict[str, float]:
+def association_xtab(xtab: DataFrame, n_obs: int) -> dict[str, float]:
     """Computes measures of association between feature and target by crosstab.
 
     Parameters
     ----------
     xtab : DataFrame
         Crosstab between feature and target.
 
     n_obs : int
         Sample total size.
 
-    n_mod_y : int
-        Number of modality of the target (and minimum number of modality).
-
     Returns
     -------
     dict[str, float]
-        Cramer's V and Tschuprow's as a dict.
+        Cramér's V and Tschuprow's as a dict.
     """
     # number of values taken by the features
     n_mod_x = xtab.shape[0]
 
     # Chi2 statistic
     chi2 = chi2_contingency(xtab)[0]
 
-    # Cramer's V
-    cramerv = sqrt(chi2 / n_obs / (n_mod_y - 1))
+    # Cramér's V
+    cramerv = sqrt(chi2 / n_obs)
 
     # Tschuprow's T
-    tschuprowt = sqrt(chi2 / n_obs / sqrt((n_mod_x - 1) * (n_mod_y - 1)))
+    tschuprowt = cramerv / sqrt(sqrt(n_mod_x - 1))
 
     return {"cramerv": cramerv, "tschuprowt": tschuprowt}
 
 
 def vectorized_groupby_sum(xtab: DataFrame, groupby: list[str]) -> DataFrame:
     """Groups a crosstab by groupby and sums column values by groups
 
@@ -767,15 +764,15 @@
         )
     ]
 
     # computing associations for each xtabs
     n_obs = xtab.sum().sum()  # number of observation
     n_mod_y = len(xtab.columns)  # number of modalities and minimum number of modalities
     associations_xtab = [
-        association_xtab(grouped_xtab, n_obs, n_mod_y)
+        association_xtab(grouped_xtab, n_obs)
         for grouped_xtab in tqdm(grouped_xtabs, disable=not verbose, desc="Computing associations")
     ]
 
     # adding corresponding combination to the association
     for combination, index_to_groupby, association, grouped_xtab in zip(
         combinations, indices_to_groupby, associations_xtab, grouped_xtabs
     ):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AutoCarver-5.1.8/AutoCarver/converters/converters.py` & `AutoCarver-5.1.9/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.9/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.9/AutoCarver/feature_selection/feature_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Tools to select the best Quantitative and Qualitative features."""
 
 from random import shuffle
 from typing import Any, Callable
 
 from pandas import DataFrame, Series
 
-from .filters import cramerv_filter, spearman_filter, thresh_filter
-from .measures import cramerv_measure, dtype_measure, kruskal_measure, mode_measure, nans_measure
+from .filters import spearman_filter, thresh_filter, tschuprowt_filter
+from .measures import (
+    dtype_measure,
+    kruskal_measure,
+    make_measure,
+    mode_measure,
+    nans_measure,
+    tschuprowt_measure,
+)
 
 # trying to import extra dependencies
 try:
     from IPython.display import display_html
 except ImportError:
     _has_idisplay = False
 else:
@@ -29,18 +36,18 @@
         self,
         n_best: int,
         *,
         quantitative_features: list[str] = None,
         qualitative_features: list[str] = None,
         measures: list[Callable] = None,
         filters: list[Callable] = None,
-        sample_size: float = 1.0,
+        colsample: float = 1.0,
         verbose: bool = False,
         pretty_print: bool = False,
-        **params,
+        **kwargs,
     ) -> None:
         """Initiates a ``FeatureSelector``.
 
         Parameters
         ----------
         n_best : int
             Number of features to select.
@@ -55,53 +62,47 @@
 
         measures : list[Callable], optional
             List of association measures to be used, by default ``None``.
             Ranks features based on last provided measure of the list.
             See :ref:`Measures`.
             Implemented measures are:
 
-            * [Quantitative Features] For association evaluation: ``kruskal_measure``, ``R_measure``
+            * [Quantitative Features] For association evaluation: ``kruskal_measure`` (default), ``R_measure``
             * [Quantitative Features] For outlier detection: ``zscore_measure``, ``iqr_measure``
-            * [Qualitative Features] For correlation: ``chi2_measure``, ``cramerv_measure``, ``tschuprowt_measure``
+            * [Qualitative Features] For association evaluation: ``chi2_measure``, ``cramerv_measure``, ``tschuprowt_measure`` (default)
 
         filters : list[Callable], optional
             List of filters to be used, by default ``None``.
             See :ref:`Filters`.
             Implemented filters are:
 
-            * [Quantitative Features] For linear correlation: ``spearman_filter``, ``pearson_filter``
-            * [Quantitative Features] For multicoloinearity: ``vif_filter``
-            * [Qualitative Features] For correlation: ``cramerv_filter``, ``tschuprowt_filter``
+            * [Quantitative Features] For linear correlation: ``spearman_filter`` (default), ``pearson_filter``
+            * [Qualitative Features] For correlation: ``cramerv_filter``, ``tschuprowt_filter`` (default)
 
-        sample_size : float, optional
-            _description_, by default ``1.0``
+        colsample : float, optional
+            Size of sampled list of features for sped up computation, between 0 and 1, by default ``1.0``
+            By default, all features are used.
+
+            For colsample=0.5, FeatureSelector will search for the best features in
+            ``features[:len(features)//2]`` and then in ``features[len(features)//2:]``.
+
+            **Tip:** for better performance, should be set such as ``len(features)//2 < 200``.
 
         verbose : bool, optional
             If ``True``, prints raw Discretizers Fit and Transform steps, as long as
             information on AutoCarver's processing and tables of target rates and frequencies for
             X, by default ``False``
 
         pretty_print : bool, optional
             If ``True``, adds to the verbose some HTML tables of target rates and frequencies for X and, if provided, X_dev.
             Overrides the value of ``verbose``, by default ``False``
 
-        **params
+        **kwargs
             Sets thresholds for ``measures`` and ``filters``, passed as keyword arguments.
 
-            * thresh_measure, float, minimum association between target and features, by default ``0``. To be used with: ``measure_filter``.
-            * name_measure, str, measure to be used for minimum association filtering. To be used with: ``measure_filter``.
-            * thresh_nan, float,aximum percentage of NaNs in a feature, by default ``1``. To be used with: ``nans_measure``.
-            * thresh_mode, float, maximum percentage of the mode of a feature, by default ``1``. To be used with: ``mode_measure``.
-            * thresh_outlier, float, maximum percentage of Outliers in a feature, by default ``1``. To be used with: ``iqr_measure``, ``zscore_measure``.
-            * thresh_corr, float, Maximum association between features, by default ``1``. To be used with: ``spearman_filter``, ``pearson_filter``, ``cramerv_filter``, ``tschuprowt_filter``.
-            * thresh_vif, float, maximum VIF between features, by default ``inf``. To be used with: ``vif_filter``.
-            * ascending, bool default ``False``
-                * ``True``: Lower values of the measure are to be considered as more associated to the target
-                * ``False``: Higher values of the measure are to be considered as more associated to the target
-
         Examples
         --------
         See `FeatureSelector examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
         # settinp up list of features
         if quantitative_features is None:
             quantitative_features = []
@@ -118,30 +119,30 @@
         # number of features selected
         self.n_best = n_best
         assert (
             0 < int(n_best // 2) <= len(self.features) + 1
         ), "Must set 0 < n_best // 2 <= len(features)"
 
         # feature sample size per iteration
-        self.sample_size = sample_size
+        self.colsample = colsample
 
         # initiating measures
         if measures is None:
             if any(quantitative_features):  # quantitative feature association measure
                 measures = [kruskal_measure]
             else:  # qualitative feature association measure
-                measures = [cramerv_measure]
+                measures = [tschuprowt_measure]
         self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
 
         # initiating filters
         if filters is None:
             if any(quantitative_features):  # quantitative feature association measure
                 filters = [spearman_filter]
             else:  # qualitative feature association measure
-                filters = [cramerv_filter]
+                filters = [tschuprowt_filter]
         self.filters = [thresh_filter] + filters[:]
 
         # names of measures to sort by
         self.measure_names = [measure.__name__ for measure in measures[::-1]]
 
         # wether or not to print tables
         self.verbose = bool(max(verbose, pretty_print))
@@ -151,15 +152,15 @@
             else:
                 self.verbose = True
                 print(
                     "Package not found: ipython. Defaulting to verbose=True. Install extra dependencies with pip install autocarver[jupyter]"
                 )
 
         # keyword arguments
-        self.params = params
+        self.kwargs = kwargs
 
     def _select_features(
         self, X: DataFrame, y: Series, features: list[str], n_best: int
     ) -> list[str]:
         """Selects the n_best features amongst the specified ones
 
         Parameters
@@ -179,38 +180,34 @@
             _description_
         """
         if self.verbose:  # verbose if requested
             print(f"------\n[FeatureSelector] Selecting from Features: {str(features)}\n---")
 
         # Computes association between X and y
         initial_associations = apply_measures(
-            X, y, measures=self.measures, features=features, **self.params
+            X, y, measures=self.measures, features=features, **self.kwargs
         )
 
         # sorting statistics
         measure_names = evaluated_measure_names(initial_associations, self.measure_names)
-        initial_associations = initial_associations.sort_values(
-            measure_names, ascending=self.params.get("ascending", False)
-        )
+        initial_associations = initial_associations.sort_values(measure_names, ascending=False)
 
         if self.verbose:  # displaying association measure
             print("\n - Association between X and y")
             print_associations(initial_associations, self.pretty_print)
 
         # applying filtering for each measure
         all_best_features: dict[str, Any] = {}
         for measure_name in measure_names:
             # sorting association for each measure
-            associations = initial_associations.sort_values(
-                measure_name, ascending=self.params.get("ascending", False)
-            )
+            associations = initial_associations.sort_values(measure_name, ascending=False)
 
             # filtering for each measure, as each measure ranks the features differently
             filtered_association = apply_filters(
-                X, associations, filters=self.filters, **self.params
+                X, associations, filters=self.filters, **self.kwargs
             )
 
             # selected features for the measure
             selected_features = [
                 feature
                 for feature in initial_associations.index
                 if feature in filtered_association.index[:n_best]
@@ -255,29 +252,29 @@
 
         Returns
         -------
         list[str]
             List of selected features
         """
         # splitting features in chunks
-        if self.sample_size < 1:
+        if self.colsample < 1:
             # shuffling features to get random samples of features
             shuffle(self.features)
 
             # number of features per sample
-            chunks = int(len(self.features) // (1 / self.sample_size))
+            chunks = int(len(self.features) // (1 / self.colsample))
 
             # splitting feature list in samples
             feature_samples = [
                 self.features[chunks * i : chunks * (i + 1)]
-                for i in range(int(1 / self.sample_size) - 1)
+                for i in range(int(1 / self.colsample) - 1)
             ]
 
             # adding last sample with all remaining features
-            feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1) :]]
+            feature_samples += [self.features[chunks * (int(1 / self.colsample) - 1) :]]
 
             # iterating over each feature samples
             best_features = []
             for features in feature_samples:
                 # fitting association on features
                 best_features += self._select_features(X, y, features, int(self.n_best // 2))
 
@@ -319,15 +316,15 @@
         nicer_association = association.style.background_gradient(cmap="coolwarm", subset=subset)
         nicer_association = nicer_association.set_table_attributes("style='display:inline'")
 
         # displaying html of colored DataFrame
         display_html(nicer_association._repr_html_(), raw=True)
 
 
-def feature_association(x: Series, y: Series, measures: list[Callable], **params) -> dict[str, Any]:
+def feature_association(x: Series, y: Series, measures: list[Callable], **kwargs) -> dict[str, Any]:
     """Measures association between x and y
 
     Parameters
     ----------
     x : Series
         Sample of a feature.
     y : Series
@@ -340,48 +337,46 @@
     """
     # measures keep going only if previous basic tests are passed
     passed = True
     association = {}
 
     # iterating over each measure
     for measure in measures:
-        passed, association = measure(passed, association, x, y, **params)
+        passed, association = make_measure(
+            measure, passed, association, x, y, **kwargs, **association
+        )
 
     return association
 
 
 def apply_measures(
-    X: DataFrame, y: Series, measures: list[Callable], features: list[str], **params
+    X: DataFrame, y: Series, measures: list[Callable], features: list[str], **kwargs
 ) -> DataFrame:
     """Measures association between columns of X and y
 
     Parameters
     ----------
     X : DataFrame
         _description_
     y : Series
         _description_
     features : list[str]
         _description_
     measure_names : list[str]
         _description_
-    ascending, bool default False
-        According to this measure:
-            - True: Lower values of the measure are to be considered as more associated to the target
-            - False: Higher values of the measure are to be considered as more associated to the target
 
     Returns
     -------
     DataFrame
         _description_
     """
     # applying association measure to each column
     associations = (
         X[features]
-        .apply(feature_association, y=y, measures=measures, **params, result_type="expand", axis=0)
+        .apply(feature_association, y=y, measures=measures, **kwargs, result_type="expand", axis=0)
         .T
     )
 
     return associations
 
 
 def evaluated_measure_names(associations: DataFrame, measure_names: list[str]) -> list[str]:
@@ -406,37 +401,33 @@
         if measure_name in associations and "_measure" in measure_name
     ]
 
     return sort_by
 
 
 def apply_filters(
-    X: DataFrame, associations: DataFrame, filters: list[Callable], **params
+    X: DataFrame, associations: DataFrame, filters: list[Callable], **kwargs
 ) -> DataFrame:
     """Filters out too correlated features (least relevant first)
 
     Parameters
     ----------
     X : DataFrame
         _description_
     associations : DataFrame
         _description_
     filters : list[Callable]
         _description_
     measure_name : str
         _description_
-    ascending, bool default False
-        According to this measure:
-            - True: Lower values of the measure are to be considered as more associated to the target
-            - False: Higher values of the measure are to be considered as more associated to the target
 
     Returns
     -------
     DataFrame
         _description_
     """
     # applying successive filters
     filtered_associations = associations.copy()
     for filtering in filters:
-        filtered_associations = filtering(X, filtered_associations, **params)
+        filtered_associations = filtering(X, filtered_associations, **kwargs)
 
     return filtered_associations
```

### Comparing `AutoCarver-5.1.8/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.9/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,94 +4,117 @@
 from typing import Any
 
 from numpy import inf, nan, ones, triu
 from pandas import DataFrame, notna
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 
 
-def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
-    """Computes max Spearman between X and X (quantitative) excluding features
-    that are correlated to a feature more associated with the target
-    (defined by the ranks).
+def spearman_filter(
+    X: DataFrame, ranks: DataFrame, thresh_corr: float = 1, **params
+) -> dict[str, Any]:
+    """Computes maximum Spearman's rho between X and X (quantitative).
+    Features too correlated to a feature more associated with the target
+    are excluded (according to provided ``ranks``).
 
     Parameters
     ----------
-    thresh_corr, float: default 1.
-      Maximum association between features
+    X : DataFrame
+        Contains columns named after ``ranks``'s index (feature names)
+    ranks : DataFrame
+        Ranked features as index of the association table
+    thresh_corr : float, optional
+        Maximum Spearman's rho bewteen features, by default ``1``
+
+    Returns
+    -------
+    dict[str, Any]
+        Maximum Spearman's rho with a better features
     """
 
     # applying quantitative filter with spearman correlation
-    return quantitative_filter(X, ranks, "spearman", **params)
+    return quantitative_filter(X, ranks, "spearman", thresh_corr, **params)
 
 
-def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
-    """Computes max Pearson between X and X (quantitative) excluding features
-    that are correlated to a feature more associated with the target
-    (defined by the ranks).
+def pearson_filter(
+    X: DataFrame, ranks: DataFrame, thresh_corr: float = 1, **params
+) -> dict[str, Any]:
+    """Computes maximum Pearson's r between X and X (quantitative).
+    Features too correlated to a feature more associated with the target
+    are excluded (according to provided ``ranks``).
 
     Parameters
     ----------
-    thresh_corr, float: default 1.
-      Maximum association between features
+    X : DataFrame
+        Contains columns named after ``ranks``'s index (feature names)
+    ranks : DataFrame
+        Ranked features as index of the association table
+    thresh_corr : float, optional
+        Maximum Pearson's r bewteen features, by default ``1``
+
+    Returns
+    -------
+    dict[str, Any]
+        Maximum Pearson's r with a better feature
     """
 
     # applying quantitative filter with spearman correlation
-    return quantitative_filter(X, ranks, "pearson", **params)
+    return quantitative_filter(X, ranks, "pearson", thresh_corr, **params)
 
 
-def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
-    """Computes Variance Inflation Factor (multicolinearity)
+# TODO
+# def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
+#     """Computes Variance Inflation Factor (multicolinearity)
 
-    Parameters
-    ----------
-    thresh_vif, float: default inf
-      Maximum VIF between features
-    """
+#     Parameters
+#     ----------
+#     thresh_vif, float: default inf
+#       Maximum VIF between features
+#     """
 
-    # accessing the prefered order
-    prefered_order = ranks.index
+#     # accessing the prefered order
+#     prefered_order = ranks.index
 
-    # initiating list association per feature
-    associations = []
+#     # initiating list association per feature
+#     associations = []
 
-    # list of dropped features
-    dropped = []
+#     # list of dropped features
+#     dropped = []
 
-    # iterating over each column
-    for i, feature in enumerate(prefered_order):
-        # identifying remaining more associated features
-        better_features = [f for f in prefered_order[: i + 1] if f not in dropped]
-
-        X_vif = X[better_features]  # keeping only better features
-        X_vif = X_vif.dropna(axis=0)  # dropping NaNs for OLS
-
-        # computation of VIF
-        vif = nan
-        if len(better_features) > 1 and len(X_vif) > 0:
-            vif = variance_inflation_factor(X_vif.values, len(better_features) - 1)
+#     # iterating over each column
+#     for i, feature in enumerate(prefered_order):
+#         # identifying remaining more associated features
+#         better_features = [f for f in prefered_order[: i + 1] if f not in dropped]
 
-        # dropping the feature if it was too correlated to a better feature
-        if vif > params.get("thresh_vif", inf) and notna(vif):
-            dropped += [feature]
+#         X_vif = X[better_features]  # keeping only better features
+#         X_vif = X_vif.dropna(axis=0)  # dropping NaNs for OLS
 
-        # kept feature: updating associations with this feature
-        else:
-            associations += [{"feature": feature, "vif_filter": vif}]
+#         # computation of VIF
+#         vif = nan
+#         if len(better_features) > 1 and len(X_vif) > 0:
+#             vif = variance_inflation_factor(X_vif.values, len(better_features) - 1)
+
+#         # dropping the feature if it was too correlated to a better feature
+#         if vif > params.get("thresh_vif", inf) and notna(vif):
+#             dropped += [feature]
+
+#         # kept feature: updating associations with this feature
+#         else:
+#             associations += [{"feature": feature, "vif_filter": vif}]
 
-    # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index("feature")
+#     # formatting ouput to DataFrame
+#     associations = DataFrame(associations).set_index("feature")
 
-    # applying filter on association
-    associations = ranks.join(associations, how="right")
+#     # applying filter on association
+#     associations = ranks.join(associations, how="right")
 
-    return associations
+#     return associations
 
 
 def quantitative_filter(
-    X: DataFrame, ranks: DataFrame, corr_measure: str, **params
+    X: DataFrame, ranks: DataFrame, corr_measure: str, thresh_corr: float = 1, **params
 ) -> dict[str, Any]:
     """Computes max association between X and X (quantitative) excluding features
     that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
@@ -114,15 +137,15 @@
         # correlation with features more associated to the target
         corr_with_better_features = X_corr.loc[:feature, feature]
 
         # maximum correlation with a better feature
         corr_with, worst_corr = corr_with_better_features.agg(["idxmax", "max"])
 
         # dropping the feature if it was too correlated to a better feature
-        if worst_corr > params.get("thresh_corr", 1):
+        if worst_corr > thresh_corr:
             X_corr = X_corr.drop(feature, axis=0).drop(feature, axis=1)
 
         # kept feature: updating associations with this feature
         else:
             associations += [
                 {
                     "feature": feature,
```

### Comparing `AutoCarver-5.1.8/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.9/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,145 @@
 """ Base measures that defines Quantitative and Qualitative features.
 """
-from typing import Any
+from typing import Any, Callable
 
 from pandas import Series
 
 
-def nans_measure(
+def make_measure(
+    measure: Callable,
     active: bool,
     association: dict[str, Any],
     x: Series,
+    y: Series,
+    **kwargs,
+) -> tuple[bool, dict[str, Any]]:
+    """Wrapper to make measures from base metrics
+
+    Parameters
+    ----------
+    measure : Callable
+        _description_
+    active : bool
+        _description_
+    association : dict[str, Any]
+        _description_
+    x : Series
+        Feature to measure
+    y : Series
+        Binary target feature
+
+    Returns
+    -------
+    tuple[bool, dict[str, Any]]
+        _description_
+    """
+    # check that previous steps where passed for computational optimization
+    if active:
+        # use the measure
+        active, measurement = measure(x, y, **kwargs)
+
+        # update association table
+        association.update(measurement)
+
+    return active, association
+
+
+def nans_measure(
+    x: Series,
     y: Series = None,
-    **params,
+    thresh_nan: float = 0.999,
+    **kwargs,
 ) -> tuple[bool, dict[str, Any]]:
     """Measure of the percentage of NaNs
 
     Parameters
     ----------
-    thresh_nan, float: default 1.
-      Maximum percentage of NaNs in a feature
+    x : Series
+        Feature to measure
+    y : Series, optional
+        Binary target feature, by default ``None``
+    thresh_nan : float, optional
+        Maximum percentage of NaNs in a feature, by default ``0.999``
+
+    Returns
+    -------
+    tuple[bool, dict[str, Any]]
+        Whether or not there are to many NaNs and the percentage of NaNs
     """
+    nans = x.isnull()  # ckecking for nans
+    pct_nan = nans.mean()  # Computing percentage of nans
 
-    # whether or not tests where passed
-    if active:
-        nans = x.isnull()  # ckecking for nans
-        pct_nan = nans.mean()  # Computing percentage of nans
-
-        # updating association
-        association.update({"pct_nan": pct_nan})
+    # updating association
+    measurement = {"pct_nan": pct_nan}
 
-        # Excluding feature that have to many NaNs
-        thresh_nan = params.get("thresh_nan", 0.999)
-        active = pct_nan < thresh_nan
-        if not active:
-            print(
-                f"Feature {x.name} will be discarded (more than {thresh_nan:2.2%} of nans). Otherwise, set a greater value for thresh_nan."
-            )
+    # Excluding feature that have to many NaNs
+    active = pct_nan < thresh_nan
+    if not active:
+        print(
+            f"Feature {x.name} will be discarded (more than {thresh_nan:2.2%} of nans). Otherwise, set a greater value for thresh_nan."
+        )
 
-    return active, association
+    return active, measurement
 
 
 def dtype_measure(
-    active: bool,
-    association: dict[str, Any],
     x: Series,
     y: Series = None,
-    **params,
+    **kwargs,
 ) -> tuple[bool, dict[str, Any]]:
-    """Gets dtype"""
+    """Feature's dtype
 
-    # updating association
-    association.update({"dtype": x.dtype})
+    Parameters
+    ----------
+    x : Series
+        Feature to measure
+    y : Series, optional
+        Binary target feature, by default ``None``
+
+    Returns
+    -------
+    tuple[bool, dict[str, Any]]
+        True and the feature's dtype
+    """
+    # getting dtype
+    measurement = {"dtype": x.dtype}
 
-    return active, association
+    return True, measurement
 
 
 def mode_measure(
-    active: bool,
-    association: dict[str, Any],
     x: Series,
     y: Series = None,
-    **params,
+    thresh_mode: float = 0.999,
+    **kwargs,
 ) -> tuple[bool, dict[str, Any]]:
     """Measure of the percentage of the Mode
 
     Parameters
     ----------
-    thresh_mode, float: default 1.
-      Maximum percentage of the mode of a feature
+    x : Series
+        Feature to measure
+    y : Series, optional
+        Binary target feature, by default ``None``
+    thresh_mode : float, optional
+        Maximum percentage of a feature's mode, by default ``0.999``
+
+    Returns
+    -------
+    tuple[bool, dict[str, Any]]
+        Whether or not the mode is overrepresented and the percentage of mode
     """
+    mode = x.mode(dropna=True).values[0]  # computing mode
+    pct_mode = (x == mode).mean()  # Computing percentage of the mode
 
-    # whether or not tests where passed
-    if active:
-        mode = x.mode(dropna=True).values[0]  # computing mode
-        pct_mode = (x == mode).mean()  # Computing percentage of the mode
-
-        # updating association
-        association.update({"pct_mode": pct_mode, "mode": mode})
+    # updating association
+    measurement = {"pct_mode": pct_mode, "mode": mode}
 
-        # Excluding feature with too frequent modes
-        thresh_mode = params.get("thresh_mode", 0.999)
-        active = pct_mode < thresh_mode
-        if not active:
-            print(
-                f"Feature {x.name} will be discarded (more than {thresh_mode:2.2%} of its mode). Otherwise, set a greater value for thresh_mode."
-            )
+    # Excluding feature with too frequent modes
+    active = pct_mode < thresh_mode
+    if not active:
+        print(
+            f"Feature {x.name} will be discarded (more than {thresh_mode:2.2%} of its mode). Otherwise, set a greater value for thresh_mode."
+        )
 
-    return active, association
+    return active, measurement
```

### Comparing `AutoCarver-5.1.8/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.9/AutoCarver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.8
+Version: 5.1.9
 Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -53,15 +53,26 @@
 4. **Statistical Accuracy and Relevance**: ``AutoCarver`` incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your binary classification models.
 
 5. **Robustness Testing**: ``AutoCarver`` goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
 
 ``AutoCarver`` is a valuable tool for data scientists and practitioners involved in binary classification problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
 
 
-## Install
+# Install
 
-AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+**AutoCarver** can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+
+## Minimal install
+
+To install the base features (without vizualization tools), use the following:
 
 <pre>
 pip install autocarver
 </pre>
 
+## Unabling pretty printing
+
+To enable ``pretty_print`` features (nice colorful html tables in jupyter), use the following:
+
+<pre>
+pip install autocarver[jupyter]
+</pre>
```

### Comparing `AutoCarver-5.1.8/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.9/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/LICENSE` & `AutoCarver-5.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.8/PKG-INFO` & `AutoCarver-5.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.8
+Version: 5.1.9
 Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -53,15 +53,26 @@
 4. **Statistical Accuracy and Relevance**: ``AutoCarver`` incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your binary classification models.
 
 5. **Robustness Testing**: ``AutoCarver`` goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
 
 ``AutoCarver`` is a valuable tool for data scientists and practitioners involved in binary classification problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
 
 
-## Install
+# Install
 
-AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+**AutoCarver** can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+
+## Minimal install
+
+To install the base features (without vizualization tools), use the following:
 
 <pre>
 pip install autocarver
 </pre>
 
+## Unabling pretty printing
+
+To enable ``pretty_print`` features (nice colorful html tables in jupyter), use the following:
+
+<pre>
+pip install autocarver[jupyter]
+</pre>
```

### Comparing `AutoCarver-5.1.8/README.md` & `AutoCarver-5.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,26 @@
 4. **Statistical Accuracy and Relevance**: ``AutoCarver`` incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your binary classification models.
 
 5. **Robustness Testing**: ``AutoCarver`` goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
 
 ``AutoCarver`` is a valuable tool for data scientists and practitioners involved in binary classification problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
 
 
-## Install
+# Install
 
-AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+**AutoCarver** can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+
+## Minimal install
+
+To install the base features (without vizualization tools), use the following:
 
 <pre>
 pip install autocarver
 </pre>
 
+## Unabling pretty printing
+
+To enable ``pretty_print`` features (nice colorful html tables in jupyter), use the following:
+
+<pre>
+pip install autocarver[jupyter]
+</pre>
```

### Comparing `AutoCarver-5.1.8/setup.py` & `AutoCarver-5.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.8",
+    version="5.1.9",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Discretization of Features with Optimal Target Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.1.8/tests/test_auto_carver.py` & `AutoCarver-5.1.9/tests/test_auto_carver.py`

 * *Files identical despite different names*

