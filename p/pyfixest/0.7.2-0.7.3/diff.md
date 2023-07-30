# Comparing `tmp/pyfixest-0.7.2.tar.gz` & `tmp/pyfixest-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.7.2.tar", max compression
+gzip compressed data, was "pyfixest-0.7.3.tar", max compression
```

## Comparing `pyfixest-0.7.2.tar` & `pyfixest-0.7.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.7.2/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.7.2/pyfixest/__init__.py
--rw-r--r--   0        0        0     4450 2023-07-18 14:22:36.978128 pyfixest-0.7.2/pyfixest/demean.py
--rw-r--r--   0        0        0      669 2023-07-29 18:02:45.424719 pyfixest-0.7.2/pyfixest/exceptions.py
--rw-r--r--   0        0        0    23413 2023-07-29 18:02:45.425729 pyfixest-0.7.2/pyfixest/feols.py
--rw-r--r--   0        0        0    43175 2023-07-29 18:03:32.047645 pyfixest-0.7.2/pyfixest/fixest.py
--rw-r--r--   0        0        0    17641 2023-07-18 14:22:36.974477 pyfixest-0.7.2/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.7.2/pyfixest/ssc_utils.py
--rw-r--r--   0        0        0     1312 2023-07-29 18:02:45.427468 pyfixest-0.7.2/pyfixest/utils.py
--rw-r--r--   0        0        0      939 2023-07-29 18:05:57.186682 pyfixest-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2320 2023-07-18 14:22:36.983620 pyfixest-0.7.2/readme.md
--rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 pyfixest-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.7.3/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.7.3/pyfixest/__init__.py
+-rw-r--r--   0        0        0     4450 2023-07-18 14:22:36.978128 pyfixest-0.7.3/pyfixest/demean.py
+-rw-r--r--   0        0        0      669 2023-07-30 13:07:57.172460 pyfixest-0.7.3/pyfixest/exceptions.py
+-rw-r--r--   0        0        0    23441 2023-07-30 16:36:15.854280 pyfixest-0.7.3/pyfixest/feols.py
+-rw-r--r--   0        0        0    43536 2023-07-30 16:37:59.174247 pyfixest-0.7.3/pyfixest/fixest.py
+-rw-r--r--   0        0        0    17641 2023-07-18 14:22:36.974477 pyfixest-0.7.3/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.7.3/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     1312 2023-07-30 13:07:57.174923 pyfixest-0.7.3/pyfixest/utils.py
+-rw-r--r--   0        0        0      939 2023-07-30 16:43:36.053557 pyfixest-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2320 2023-07-30 13:07:57.175928 pyfixest-0.7.3/readme.md
+-rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 pyfixest-0.7.3/PKG-INFO
```

### Comparing `pyfixest-0.7.2/LICENSE.md` & `pyfixest-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/pyfixest/demean.py` & `pyfixest-0.7.3/pyfixest/demean.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/pyfixest/exceptions.py` & `pyfixest-0.7.3/pyfixest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/pyfixest/feols.py` & `pyfixest-0.7.3/pyfixest/feols.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,26 +338,30 @@
 
         self._tstat = (
             self.beta_hat / self._se
         )
 
         if self.vcov_type in ["iid", "hetero"]:
             df = self.N - self.k
+
         else:
             df = self.G - 1
         self._pvalue = (
             2*(1-t.cdf(np.abs(self._tstat), df))
         )
 
-        z = norm.ppf(1 - (alpha / 2))
+        z = np.abs(t.ppf((1 - alpha) / 2, df))
+        z_se = z * self._se
+
         self.conf_int = (
-            np.array([z * self._se - self.beta_hat, z * self._se + self.beta_hat])
+            np.array([self.beta_hat - z_se, self.beta_hat + z_se])
         )
 
 
+
     def get_Ftest(self, vcov, is_iv = False):
 
         '''
         compute an F-test statistic of the form H0: R*beta = q
         Args: is_iv (bool): If True, the F-test is computed for the first stage regression of an IV model. Default is False.
         Returns: None
         '''
```

### Comparing `pyfixest-0.7.2/pyfixest/fixest.py` & `pyfixest-0.7.3/pyfixest/fixest.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,14 +652,23 @@
 
         Returns:
             A pd.DataFrame with coefficient names and p-values. The key indicates which models the estimated statistic derives from.
 
         '''
         return self.tidy()["Pr(>|t|)"]
 
+    def confint(self) -> pd.DataFrame:
+        '''
+        Obtain the confidence intervals of the fitted models.
+        Returns:
+            A pd.DataFrame with coefficient names and confidence intervals. The key indicates which models the estimated statistic derives from.
+        '''
+
+        return self.tidy()[["confint_lower", "confint_upper"]]
+
     def iplot(self, alpha: float = 0.05, figsize: tuple = (10, 10), yintercept: Union[int, str, None] = None, xintercept: Union[int, str, None] = None, rotate_xticks: int = 0) -> None:
         '''
         Plot model coefficients with confidence intervals for variable interactions specified via the `i()` syntax.
         Args:
             alpha: float, optional. The significance level for the confidence intervals. Default is 0.05.
             figsize: tuple, optional. The size of the figure. Default is (10, 10).
             yintercept: int or str (for a categorical x axis). The value at which to draw a horizontal line.
```

### Comparing `pyfixest-0.7.2/pyfixest/FormulaParser.py` & `pyfixest-0.7.3/pyfixest/FormulaParser.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/pyfixest/ssc_utils.py` & `pyfixest-0.7.3/pyfixest/ssc_utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/pyfixest/utils.py` & `pyfixest-0.7.3/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/pyproject.toml` & `pyfixest-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.7.2"
+version = "0.7.3"
 
 description = "Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation."
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://s3alfisc.github.io/pyfixest/"
 repository = "https://github.com/s3alfisc/pyfixest"
```

### Comparing `pyfixest-0.7.2/readme.md` & `pyfixest-0.7.3/readme.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.2/PKG-INFO` & `pyfixest-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.7.2
+Version: 0.7.3
 Summary: Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation.
 Home-page: https://s3alfisc.github.io/pyfixest/
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

