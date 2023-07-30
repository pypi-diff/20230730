# Comparing `tmp/copulogram-0.0.2.tar.gz` & `tmp/copulogram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copulogram-0.0.2.tar", last modified: Mon Jul  3 18:27:50 2023, max compression
+gzip compressed data, was "copulogram-0.0.3.tar", last modified: Sun Jul 30 13:45:05 2023, max compression
```

## Comparing `copulogram-0.0.2.tar` & `copulogram-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 g88077   (71962) rdusers  (61000)        0 2023-07-03 18:27:50.951418 copulogram-0.0.2/
--rw-r--r--   0 g88077   (71962) rdusers  (61000)    26526 2023-03-22 09:29:34.000000 copulogram-0.0.2/LICENSE
--rw-r--r--   0 g88077   (71962) rdusers  (61000)     3372 2023-07-03 18:27:50.951418 copulogram-0.0.2/PKG-INFO
--rw-r--r--   0 g88077   (71962) rdusers  (61000)     2687 2023-07-03 17:17:12.000000 copulogram-0.0.2/README.md
-drwxr-xr-x   0 g88077   (71962) rdusers  (61000)        0 2023-07-03 18:27:50.951418 copulogram-0.0.2/copulogram/
--rw-r--r--   0 g88077   (71962) rdusers  (61000)    11184 2023-07-03 18:20:34.000000 copulogram-0.0.2/copulogram/Copulogram.py
--rw-r--r--   0 g88077   (71962) rdusers  (61000)     2676 2023-03-31 09:19:32.000000 copulogram-0.0.2/copulogram/NonParametricModel.py
--rw-r--r--   0 g88077   (71962) rdusers  (61000)      193 2023-07-03 18:26:07.000000 copulogram-0.0.2/copulogram/__init__.py
-drwxr-xr-x   0 g88077   (71962) rdusers  (61000)        0 2023-07-03 18:27:50.951418 copulogram-0.0.2/copulogram.egg-info/
--rw-r--r--   0 g88077   (71962) rdusers  (61000)     3372 2023-07-03 18:27:50.000000 copulogram-0.0.2/copulogram.egg-info/PKG-INFO
--rw-r--r--   0 g88077   (71962) rdusers  (61000)      276 2023-07-03 18:27:50.000000 copulogram-0.0.2/copulogram.egg-info/SOURCES.txt
--rw-r--r--   0 g88077   (71962) rdusers  (61000)        1 2023-07-03 18:27:50.000000 copulogram-0.0.2/copulogram.egg-info/dependency_links.txt
--rw-r--r--   0 g88077   (71962) rdusers  (61000)       53 2023-07-03 18:27:50.000000 copulogram-0.0.2/copulogram.egg-info/requires.txt
--rw-r--r--   0 g88077   (71962) rdusers  (61000)       11 2023-07-03 18:27:50.000000 copulogram-0.0.2/copulogram.egg-info/top_level.txt
--rw-r--r--   0 g88077   (71962) rdusers  (61000)       38 2023-07-03 18:27:50.951418 copulogram-0.0.2/setup.cfg
--rw-r--r--   0 g88077   (71962) rdusers  (61000)     1702 2023-07-03 18:24:03.000000 copulogram-0.0.2/setup.py
+drwxr-xr-x   0 g88077   (71962) rdusers  (61000)        0 2023-07-30 13:45:05.701940 copulogram-0.0.3/
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)    26526 2023-03-22 09:29:34.000000 copulogram-0.0.3/LICENSE
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)     3372 2023-07-30 13:45:05.701940 copulogram-0.0.3/PKG-INFO
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)     2687 2023-07-03 17:17:12.000000 copulogram-0.0.3/README.md
+drwxr-xr-x   0 g88077   (71962) rdusers  (61000)        0 2023-07-30 13:45:05.701940 copulogram-0.0.3/copulogram/
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)    11555 2023-07-30 12:12:25.000000 copulogram-0.0.3/copulogram/Copulogram.py
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)     2676 2023-03-31 09:19:32.000000 copulogram-0.0.3/copulogram/NonParametricModel.py
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)      193 2023-07-30 13:36:17.000000 copulogram-0.0.3/copulogram/__init__.py
+drwxr-xr-x   0 g88077   (71962) rdusers  (61000)        0 2023-07-30 13:45:05.701940 copulogram-0.0.3/copulogram.egg-info/
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)     3372 2023-07-30 13:45:05.000000 copulogram-0.0.3/copulogram.egg-info/PKG-INFO
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)      276 2023-07-30 13:45:05.000000 copulogram-0.0.3/copulogram.egg-info/SOURCES.txt
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)        1 2023-07-30 13:45:05.000000 copulogram-0.0.3/copulogram.egg-info/dependency_links.txt
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)       53 2023-07-30 13:45:05.000000 copulogram-0.0.3/copulogram.egg-info/requires.txt
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)       11 2023-07-30 13:45:05.000000 copulogram-0.0.3/copulogram.egg-info/top_level.txt
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)       38 2023-07-30 13:45:05.701940 copulogram-0.0.3/setup.cfg
+-rw-r--r--   0 g88077   (71962) rdusers  (61000)     1702 2023-07-30 13:31:21.000000 copulogram-0.0.3/setup.py
```

### Comparing `copulogram-0.0.2/LICENSE` & `copulogram-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `copulogram-0.0.2/PKG-INFO` & `copulogram-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copulogram
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data visualization for multivariate datasets with a nonlinear dependence structure
 Home-page: https://github.com/efekhari27/copulogram
 Author: Elias Fekhari, Vincent Chabridon
 Author-email: elias.fekhari@edf.fr
 License: LGPLv3+
 Keywords: OpenTURNS,Copula
 Classifier: Environment :: Console
```

### Comparing `copulogram-0.0.2/README.md` & `copulogram-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `copulogram-0.0.2/copulogram/Copulogram.py` & `copulogram-0.0.3/copulogram/Copulogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,18 @@
             if kde_on_marginals:
                 copulogram.map_diag(sns.kdeplot, color=color)
             else:
                 copulogram.map_diag(sns.histplot, color=color, bins=20)
 
             if quantile_contour_levels is None:
                 copulogram.map_lower(plt.scatter, color=color, alpha=alpha, marker=marker)
-                temp = df_numeric.rank() / self.N * df_numeric.max().values
+                temp = (df_numeric.rank() / self.N)
+                xmaxs = df_numeric.max().values
+                xmins = df_numeric.min().values
+                temp = temp * (xmaxs - xmins) + xmins
                 copulogram.data = temp
                 copulogram = copulogram.map_upper(plt.scatter, color=color, alpha=alpha, marker=marker)
             else:
                 copulogram.map_lower(sns.kdeplot, levels=quantile_contour_levels, color=color)
                 temp = df_numeric.rank() / self.N * df_numeric.max().values
                 copulogram.data = temp
                 copulogram.map_upper(sns.kdeplot, levels=quantile_contour_levels, color=color)
@@ -136,15 +139,19 @@
                 if df[hue].dtype =='O':
                     copulogram.map_diag(sns.histplot, color=".3", bins=20)
                 else:
                     copulogram.map_diag(sns.histplot, hue=None, color=".3", bins=20)
             
             if quantile_contour_levels is None:
                 copulogram.map_lower(sns.scatterplot, alpha=alpha, marker=marker)
-                temp = df_numeric[plotted_cols].rank() / self.N * df_numeric[plotted_cols].max().values
+                #temp = df_numeric[plotted_cols].rank() / self.N * df_numeric[plotted_cols].max().values
+                temp = (df_numeric[plotted_cols].rank() / self.N)
+                xmaxs = df_numeric[plotted_cols].max().values
+                xmins = df_numeric[plotted_cols].min().values
+                temp = temp * (xmaxs - xmins) + xmins
                 temp[hue] = df[hue]
                 copulogram.data = temp
                 copulogram = copulogram.map_upper(sns.scatterplot, alpha=alpha, marker=marker)
             else:
                 copulogram.map_lower(sns.kdeplot, levels=quantile_contour_levels)
                 temp = df_numeric[plotted_cols].rank() / self.N * df_numeric[plotted_cols].max().values
                 temp[hue] = df[hue]
```

### Comparing `copulogram-0.0.2/copulogram/NonParametricModel.py` & `copulogram-0.0.3/copulogram/NonParametricModel.py`

 * *Files identical despite different names*

### Comparing `copulogram-0.0.2/copulogram.egg-info/PKG-INFO` & `copulogram-0.0.3/copulogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copulogram
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data visualization for multivariate datasets with a nonlinear dependence structure
 Home-page: https://github.com/efekhari27/copulogram
 Author: Elias Fekhari, Vincent Chabridon
 Author-email: elias.fekhari@edf.fr
 License: LGPLv3+
 Keywords: OpenTURNS,Copula
 Classifier: Environment :: Console
```

### Comparing `copulogram-0.0.2/setup.py` & `copulogram-0.0.3/setup.py`

 * *Files identical despite different names*

