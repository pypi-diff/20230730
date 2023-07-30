# Comparing `tmp/klib-1.1.1.tar.gz` & `tmp/klib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klib-1.1.1.tar", max compression
+gzip compressed data, was "klib-1.1.2.tar", max compression
```

## Comparing `klib-1.1.1.tar` & `klib-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2022-07-29 17:32:38.054377 klib-1.1.1/LICENSE
--rw-r--r--   0        0        0     6641 2023-07-27 15:29:23.883519 klib-1.1.1/README.md
--rw-r--r--   0        0        0     2791 2023-07-27 16:43:14.339407 klib-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1033 2023-07-27 16:15:40.773253 klib-1.1.1/src/klib/__init__.py
--rw-r--r--   0        0        0       54 2023-07-27 16:43:18.499492 klib-1.1.1/src/klib/_version.py
--rw-r--r--   0        0        0    20871 2023-07-27 15:29:23.896625 klib-1.1.1/src/klib/clean.py
--rw-r--r--   0        0        0    35202 2023-07-27 16:40:52.007334 klib-1.1.1/src/klib/describe.py
--rw-r--r--   0        0        0        0 2023-07-27 15:29:23.897081 klib-1.1.1/src/klib/scripts/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-27 15:29:23.897579 klib-1.1.1/src/klib/scripts/performance.py
--rw-r--r--   0        0        0     9779 2023-07-27 15:29:23.897878 klib-1.1.1/src/klib/utils.py
--rw-r--r--   0        0        0        0 2022-07-29 17:32:38.390459 klib-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0    10815 2023-07-27 15:29:23.898195 klib-1.1.1/tests/test_clean.py
--rw-r--r--   0        0        0     3799 2023-07-27 15:29:23.898345 klib-1.1.1/tests/test_describe.py
--rw-r--r--   0        0        0     9181 2023-07-27 15:29:23.898650 klib-1.1.1/tests/test_util.py
--rw-r--r--   0        0        0     7508 1970-01-01 00:00:00.000000 klib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-07-29 17:32:38.054377 klib-1.1.2/LICENSE
+-rw-r--r--   0        0        0     6749 2023-07-30 06:43:34.724229 klib-1.1.2/README.md
+-rw-r--r--   0        0        0     2791 2023-07-30 06:43:53.091898 klib-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1033 2023-07-27 16:15:40.773253 klib-1.1.2/src/klib/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-30 06:44:03.617140 klib-1.1.2/src/klib/_version.py
+-rw-r--r--   0        0        0    20871 2023-07-27 15:29:23.896625 klib-1.1.2/src/klib/clean.py
+-rw-r--r--   0        0        0    35343 2023-07-30 06:39:56.185238 klib-1.1.2/src/klib/describe.py
+-rw-r--r--   0        0        0        0 2023-07-27 15:29:23.897081 klib-1.1.2/src/klib/scripts/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-27 15:29:23.897579 klib-1.1.2/src/klib/scripts/performance.py
+-rw-r--r--   0        0        0     9779 2023-07-27 15:29:23.897878 klib-1.1.2/src/klib/utils.py
+-rw-r--r--   0        0        0        0 2022-07-29 17:32:38.390459 klib-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    10815 2023-07-27 15:29:23.898195 klib-1.1.2/tests/test_clean.py
+-rw-r--r--   0        0        0     3799 2023-07-27 15:29:23.898345 klib-1.1.2/tests/test_describe.py
+-rw-r--r--   0        0        0     9181 2023-07-27 15:29:23.898650 klib-1.1.2/tests/test_util.py
+-rw-r--r--   0        0        0     7616 1970-01-01 00:00:00.000000 klib-1.1.2/PKG-INFO
```

### Comparing `klib-1.1.1/LICENSE` & `klib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/README.md` & `klib-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 df = pd.DataFrame(data)
 
 # klib.describe - functions for visualizing datasets
 - klib.cat_plot(df) # returns a visualization of the number and frequency of categorical features
 - klib.corr_mat(df) # returns a color-encoded correlation matrix
 - klib.corr_plot(df) # returns a color-encoded heatmap, ideal for correlations
+- klib.corr_interactive_plot(df, split="neg").show() # returns an interactive correlation plot using plotly
 - klib.dist_plot(df) # returns a distribution plot for every numeric feature
 - klib.missingval_plot(df) # returns a figure containing information about missing values
 
 # klib.clean - functions for cleaning datasets
 - klib.data_cleaning(df) # performs datacleaning (drop duplicates & empty rows/cols, adjust dtypes,...)
 - klib.clean_column_names(df) # cleans and standardizes column names, also called inside data_cleaning()
 - klib.convert_datatypes(df) # converts existing to more efficient dtypes, also called inside data_cleaning()
```

#### html2text {}

```diff
@@ -25,29 +25,30 @@
 klib) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/
 klib.svg)](https://anaconda.org/conda-forge/klib) ```bash conda install -
 c conda-forge klib ``` ## Usage ```python import klib import pandas as pd df =
 pd.DataFrame(data) # klib.describe - functions for visualizing datasets -
 klib.cat_plot(df) # returns a visualization of the number and frequency of
 categorical features - klib.corr_mat(df) # returns a color-encoded correlation
 matrix - klib.corr_plot(df) # returns a color-encoded heatmap, ideal for
-correlations - klib.dist_plot(df) # returns a distribution plot for every
-numeric feature - klib.missingval_plot(df) # returns a figure containing
-information about missing values # klib.clean - functions for cleaning datasets
-- klib.data_cleaning(df) # performs datacleaning (drop duplicates & empty rows/
-cols, adjust dtypes,...) - klib.clean_column_names(df) # cleans and
-standardizes column names, also called inside data_cleaning() -
-klib.convert_datatypes(df) # converts existing to more efficient dtypes, also
-called inside data_cleaning() - klib.drop_missing(df) # drops missing values,
-also called in data_cleaning() - klib.mv_col_handling(df) # drops features with
-high ratio of missing vals based on informational content -
-klib.pool_duplicate_subsets(df) # pools subset of cols based on duplicates with
-min. loss of information ``` ## Examples Find all available examples as well as
-applications of the functions in **klib.clean()** with detailed descriptions
-here. ```python klib.missingval_plot(df) # default representation of missing
-values in a DataFrame, plenty of settings are available ```
+correlations - klib.corr_interactive_plot(df, split="neg").show() # returns an
+interactive correlation plot using plotly - klib.dist_plot(df) # returns a
+distribution plot for every numeric feature - klib.missingval_plot(df) #
+returns a figure containing information about missing values # klib.clean -
+functions for cleaning datasets - klib.data_cleaning(df) # performs
+datacleaning (drop duplicates & empty rows/cols, adjust dtypes,...) -
+klib.clean_column_names(df) # cleans and standardizes column names, also called
+inside data_cleaning() - klib.convert_datatypes(df) # converts existing to more
+efficient dtypes, also called inside data_cleaning() - klib.drop_missing(df) #
+drops missing values, also called in data_cleaning() - klib.mv_col_handling(df)
+# drops features with high ratio of missing vals based on informational content
+- klib.pool_duplicate_subsets(df) # pools subset of cols based on duplicates
+with min. loss of information ``` ## Examples Find all available examples as
+well as applications of the functions in **klib.clean()** with detailed
+descriptions here. ```python klib.missingval_plot(df) # default representation
+of missing values in a DataFrame, plenty of settings are available ```
                           [Missingvalue Plot Example]
 ```python klib.corr_plot(df, split='pos') # displaying only positive
 correlations, other settings include threshold, cmap... klib.corr_plot(df,
 split='neg') # displaying only negative correlations ```
                               [Corr Plot Example]
 ```python klib.corr_plot(df, target='wine') # default representation of
 correlations with the feature column ```
```

### Comparing `klib-1.1.1/pyproject.toml` & `klib-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "klib"
-version = "1.1.1"
+version = "1.1.2"
 description = "Customized data preprocessing functions for frequent tasks."
 authors = ["Andreas Kanz <andreas@akanz.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [{ include = "klib", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
@@ -144,14 +144,14 @@
 
 ignore = ["T201", "FBT001", "FBT002", "PLR0913", "D213", "D203"]
 
 line-length = 88
 target-version = "py38"
 
 [tool.ruff.mccabe]
-max-complexity = 7
+max-complexity = 8
 
 [tool.ruff.per-file-ignores]
 "test**" = ["ANN", "D", "S101", "PLR", "PT009", "N", "E501"]
 "**/scripts/**" = ["ANN", "D", "S101", "PLR", "PT009", "N", "E501"]
 [tool.ruff.isort]
 force-single-line = true
```

### Comparing `klib-1.1.1/src/klib/__init__.py` & `klib-1.1.2/src/klib/__init__.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/src/klib/clean.py` & `klib-1.1.2/src/klib/clean.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/src/klib/describe.py` & `klib-1.1.2/src/klib/describe.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import scipy
 import seaborn as sns
 from matplotlib import ticker
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.colors import to_rgb
 from matplotlib.gridspec import GridSpec  # noqa: TCH002
 from screeninfo import get_monitors
+from screeninfo import ScreenInfoError
 
 from klib.utils import _corr_selector
 from klib.utils import _missing_vals
 from klib.utils import _validate_input_bool
 from klib.utils import _validate_input_int
 from klib.utils import _validate_input_num_data
 from klib.utils import _validate_input_range
@@ -611,27 +612,30 @@
             xgap=1,
             ygap=1,
             **kwargs,
         ),
     )
 
     dpi = None
-    for monitor in get_monitors():
-        if monitor.is_primary:
+    try:
+        for monitor in get_monitors():
+            if monitor.is_primary:
+                if monitor.width_mm is None or monitor.height_mm is None:
+                    continue
+                dpi = monitor.width / (monitor.width_mm / 25.4)
+                break
+
+        if dpi is None:
+            monitor = get_monitors()[0]
             if monitor.width_mm is None or monitor.height_mm is None:
-                continue
-            dpi = monitor.width / (monitor.width_mm / 25.4)
-            break
-
-    if dpi is None:
-        monitor = get_monitors()[0]
-        if monitor.width_mm is None or monitor.height_mm is None:
-            dpi = 96  # more or less arbitrary default value
-        else:
-            dpi = monitor.width / (monitor.width_mm / 25.4)
+                dpi = 96  # more or less arbitrary default value
+            else:
+                dpi = monitor.width / (monitor.width_mm / 25.4)
+    except ScreenInfoError:
+        dpi = 96
 
     heatmap.update_layout(
         title=f"Feature-correlation ({method})",
         title_font={"size": 24},
         title_x=0.5,
         autosize=True,
         width=figsize[0] * dpi,
```

### Comparing `klib-1.1.1/src/klib/scripts/performance.py` & `klib-1.1.2/src/klib/scripts/performance.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/src/klib/utils.py` & `klib-1.1.2/src/klib/utils.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/tests/test_clean.py` & `klib-1.1.2/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/tests/test_describe.py` & `klib-1.1.2/tests/test_describe.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/tests/test_util.py` & `klib-1.1.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.1/PKG-INFO` & `klib-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Customized data preprocessing functions for frequent tasks.
 License: MIT
 Author: Andreas Kanz
 Author-email: andreas@akanz.de
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -61,14 +61,15 @@
 
 df = pd.DataFrame(data)
 
 # klib.describe - functions for visualizing datasets
 - klib.cat_plot(df) # returns a visualization of the number and frequency of categorical features
 - klib.corr_mat(df) # returns a color-encoded correlation matrix
 - klib.corr_plot(df) # returns a color-encoded heatmap, ideal for correlations
+- klib.corr_interactive_plot(df, split="neg").show() # returns an interactive correlation plot using plotly
 - klib.dist_plot(df) # returns a distribution plot for every numeric feature
 - klib.missingval_plot(df) # returns a figure containing information about missing values
 
 # klib.clean - functions for cleaning datasets
 - klib.data_cleaning(df) # performs datacleaning (drop duplicates & empty rows/cols, adjust dtypes,...)
 - klib.clean_column_names(df) # cleans and standardizes column names, also called inside data_cleaning()
 - klib.convert_datatypes(df) # converts existing to more efficient dtypes, also called inside data_cleaning()
```

