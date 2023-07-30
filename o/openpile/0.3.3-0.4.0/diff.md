# Comparing `tmp/openpile-0.3.3.tar.gz` & `tmp/openpile-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-_v5y9mi1/openpile-0.3.3.tar", last modified: Fri May 19 07:43:06 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-mvs9863j/openpile-0.4.0.tar", last modified: Sun Jul 30 20:31:00 2023, max compression
```

## Comparing `openpile-0.3.3.tar` & `openpile-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 07:42:56.000000 openpile-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-19 07:43:06.000000 openpile-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-19 07:42:56.000000 openpile-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-19 07:42:56.000000 openpile-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-19 07:43:06.000000 openpile-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-19 07:42:56.000000 openpile-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29182 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/Hb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/Mb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/mt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/py_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/qz_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-19 07:42:56.000000 openpile-0.3.3/src/openpile/utils/tz_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 07:43:06.000000 openpile-0.3.3/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:43:06.000000 openpile-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-19 07:42:56.000000 openpile-0.3.3/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-19 07:42:56.000000 openpile-0.3.3/test/test_pycurves.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 07:42:56.000000 openpile-0.3.3/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 20:30:51.000000 openpile-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-30 20:31:00.000000 openpile-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-30 20:30:51.000000 openpile-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 20:30:51.000000 openpile-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-30 20:31:00.000000 openpile-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 20:30:51.000000 openpile-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60358 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28674 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27008 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-30 20:30:51.000000 openpile-0.4.0/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-30 20:30:51.000000 openpile-0.4.0/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 20:30:51.000000 openpile-0.4.0/test/test_utils_misc.py
```

### Comparing `openpile-0.3.3/LICENSE.txt` & `openpile-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.3.3/PKG-INFO` & `openpile-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.3.3
+Version: 0.4.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
@@ -26,15 +26,15 @@
 # OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
-[![Downloads](https://static.pepy.tech/badge/openpile)](https://pepy.tech/project/openpile)
+[![Downloads](https://static.pepy.tech/badge/openpile/month)](https://pepy.tech/project/openpile)
 
 ![Tests](https://github.com/TchilDill/openpile/actions/workflows/Test.yml/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/openpile/badge/?version=latest)](https://openpile.readthedocs.io/en/latest/?badge=latest)
 
 
 [![issues closed](https://img.shields.io/github/issues-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/issues)
 [![PRs closed](https://img.shields.io/github/issues-pr-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/pulls)
```

### Comparing `openpile-0.3.3/README.md` & `openpile-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
-[![Downloads](https://static.pepy.tech/badge/openpile)](https://pepy.tech/project/openpile)
+[![Downloads](https://static.pepy.tech/badge/openpile/month)](https://pepy.tech/project/openpile)
 
 ![Tests](https://github.com/TchilDill/openpile/actions/workflows/Test.yml/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/openpile/badge/?version=latest)](https://openpile.readthedocs.io/en/latest/?badge=latest)
 
 
 [![issues closed](https://img.shields.io/github/issues-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/issues)
 [![PRs closed](https://img.shields.io/github/issues-pr-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/pulls)
```

### Comparing `openpile-0.3.3/setup.cfg` & `openpile-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 zip_safe = False
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	pandas
+	pandas < 2.0
 	numpy
 	matplotlib
 	numba
 	scipy
-	pydantic
+	pydantic < 2.0
 	typing_extensions
 
 [options.extras_require]
 dev = 
 	Sphinx==5.3.0
 	sphinx-rtd-theme==1.1.1
 	sphinxcontrib-applehelp==1.0.2
```

### Comparing `openpile-0.3.3/setup.py` & `openpile-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.3/src/openpile/analyses.py` & `openpile-0.4.0/src/openpile/analyze.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,95 @@
 """
-`Analyses` module
+`analyze` module
 ==================
 
-The `analyses` module is used to run various simulations. 
+The `analyze` module is used to run 1D Finite Element analyses. 
 
-Every function from this module returns an `openpile.compute.Result` object. 
+Every function from this module returns an `openpile.analyze.AnalyzeResult` object. 
 
 """
 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
+import warnings
 
-# from pydantic import BaseModel, Field, root_validator
-from pydantic.dataclasses import dataclass
+from dataclasses import dataclass
 
 from openpile.core import kernel
 import openpile.core.validation as validation
 import openpile.utils.graphics as graphics
 import openpile.core.misc as misc
 
 
 class PydanticConfig:
     arbitrary_types_allowed = True
+    frozen = True
+    underscore_attrs_are_private = True
 
 
 def springs_mob_to_df(model, d):
 
     # elevations
     x = model.nodes_coordinates["x [m]"].values
     x = kernel.double_inner_njit(x)
 
     # PY springs
     # py secant stiffness
     py_ks = kernel.calculate_py_springs_stiffness(
         u=d[1::3], springs=model._py_springs, kind="secant"
     ).flatten()
-    py_u = kernel.double_inner_njit(d[1::3])
-    py_mob = py_u * py_ks
+    py_mob = kernel.double_inner_njit(d[1::3]) * py_ks
     # calculate max spring values
-    max_springs_values = model._py_springs[:, :, 0].max(axis=2).flatten()
+    py_max = model._py_springs[:, :, 0].max(axis=2).flatten()
+
+    # mt springs
+    # mt secant stiffness
+    mt_ks = kernel.calculate_mt_springs_stiffness(
+        d[2::3], model._mt_springs, model._py_springs, py_mob.reshape((-1, 2, 1, 1)), kind="secant"
+    ).flatten()
+    mt_mob = kernel.double_inner_njit(d[2::3]) * mt_ks
+    # calculate max spring values
+    mt_max = model._mt_springs[:, :, 0, -1].max(axis=2).flatten()
 
     # create DataFrame
     df = pd.DataFrame(
         data={
             "Elevation [m]": x,
             "p_mobilized [kN/m]": np.abs(py_mob),
-            "p_max [kN/m]": max_springs_values,
+            "p_max [kN/m]": py_max,
+            "m_mobilized [kNm/m]": np.abs(mt_mob),
+            "m_max [kNm/m]": mt_max,
         }
     )
 
     return df
 
 
+def reaction_forces_to_df(model, Q):
+    x = model.nodes_coordinates["x [m]"].values
+    Q = Q.reshape(-1, 3)
+
+    df = pd.DataFrame(
+        data={
+            "Elevation [m]": x,
+            "Nr [kN]": Q[:, 0],
+            "Vr [kN]": Q[:, 1],
+            "Mr [kNm]": Q[:, 2],
+        }
+    )
+    df[["Nr [kN]"]] = df[["Nr [kN]"]].mask(df[["Nr [kN]"]].abs() < 1e-3, 0.0)
+    df[["Vr [kN]"]] = df[["Vr [kN]"]].mask(df[["Vr [kN]"]].abs() < 1e-3, 0.0)
+    df[["Mr [kNm]"]] = df[["Mr [kNm]"]].mask(df[["Mr [kNm]"]].abs() < 1e-3, 0.0)
+
+    return df[np.any(df[["Nr [kN]", "Vr [kN]", "Mr [kNm]"]].abs() > 1e-3, axis=1)].reset_index(
+        drop=True
+    )
+
+
 def structural_forces_to_df(model, q):
     x = model.nodes_coordinates["x [m]"].values
     x = misc.repeat_inner(x)
     L = kernel.mesh_to_element_length(model).reshape(-1)
 
     N = np.vstack((-q[0::6], q[3::6])).reshape(-1, order="F")
     V = np.vstack((-q[1::6], q[4::6])).reshape(-1, order="F")
@@ -89,67 +122,147 @@
             "Rotation [rad]": Rx,
         }
     )
 
     return disp_to_DataFrame
 
 
-@dataclass(config=PydanticConfig)
-class Result:
-    name: str
-    displacements: pd.DataFrame
-    forces: pd.DataFrame
-    springs_mobilization: pd.DataFrame
+@dataclass
+class AnalyzeResult:
+    """The `AnalyzeResult` class is created by any analyses from the :py:mod:`openpile.analyze` module.
+
+    As such the user can use the following properties and/or methods for any return values of an analysis.
 
-    class Config:
-        frozen = True
+    """
+
+    _name: str
+    _d: pd.DataFrame
+    _f: pd.DataFrame
+    _Q: pd.DataFrame
+    _dist_mob: pd.DataFrame = None
+    _hb_mob: tuple = None
+    _mb_mob: tuple = None
+    _details: dict = None
+
+    @property
+    def displacements(self):
+        """Retrieves displacements along each dimensions
+
+        Returns
+        -------
+        pandas.DataFrame
+            Table with the nodes elevations along the pile and their displacements
+        """
+        return self._d
+
+    @property
+    def forces(self):
+        """Retrieves forces along the pile (Normal force, shear force and bending moment)
+
+        Returns
+        -------
+        pandas.DataFrame
+            Table with the nodes elevations along the pile and their forces
+        """
+        return self._f
+
+    @property
+    def reactions(self):
+        """Retrieves reaction forces (where supports are given)
+
+        Returns
+        -------
+        pandas.DataFrame
+            Table with the nodes elevations along the pile and their forces
+        """
+        return self._Q
 
     @property
     def settlement(self):
         """Retrieves degrees of freedom for settlement
 
         Returns
         -------
         pandas.DataFrame
             Table with the nodes elevations along the pile and their normal displacements
         """
-        return self.displacements[["Elevation [m]", "Settlement [m]"]]
+        return self._d[["Elevation [m]", "Settlement [m]"]]
 
     @property
     def deflection(self):
         """Retrieves degrees of freedom for deflection
 
         Returns
         -------
         pandas.DataFrame
             Table with the nodes elevations along the pile and their transversal displacements
         """
-        return self.displacements[["Elevation [m]", "Deflection [m]"]]
+        return self._d[["Elevation [m]", "Deflection [m]"]]
 
     @property
     def rotation(self):
         """Retrieves rotational degrees of freedom
 
         Returns
         -------
         pandas.DataFrame
             Table with the nodes elevations along the pile and their rotations
         """
-        return self.displacements[["Elevation [m]", "Rotation [rad]"]]
+        return self._d[["Elevation [m]", "Rotation [rad]"]]
 
     @property
     def py_mobilization(self):
-        """Retrieves mobilized resistance of p-y curves.
+        """Retrieves mobilized resistance of districuted lateral p-y curves.
 
         Returns
         -------
         pandas.DataFrame
             Table with the nodes elevations along the pile and the mobilized resistance in kN/m.
         """
-        return self.springs_mobilization[["Elevation [m]", "p_mobilized [kN/m]", "p_max [kN/m]"]]
+
+        if self._dist_mob is None:
+            return None
+        else:
+            return self._dist_mob[["Elevation [m]", "p_mobilized [kN/m]", "p_max [kN/m]"]]
+
+    @property
+    def mt_mobilization(self):
+        """Retrieves mobilized resistance of distributed moment rotational curves.
+
+        Returns
+        -------
+        pandas.DataFrame
+            Table with the nodes elevations along the pile and the mobilized resistance in kNm/m.
+        """
+        if self._dist_mob is None:
+            return None
+        else:
+            return self._dist_mob[["Elevation [m]", "m_mobilized [kNm/m]", "m_max [kNm/m]"]]
+
+    @property
+    def Hb_mobilization(self):
+        """Retrieves mobilized resistance of base shear.
+
+        Returns
+        -------
+        tuple
+            the mobilised value and the maximum resistance in kN
+        """
+        return self._hb_mob if self._hb_mob is not None else None
+
+    @property
+    def Mb_mobilization(self):
+        """Retrieves mobilized resistance of base moment.
+
+        Returns
+        -------
+        tuple
+            the mobilised value and the maximum resistance in kNm
+        """
+        return self._mb_mob if self._mb_mob is not None else None
 
     def plot_deflection(self, assign=False):
         """
         Plots the deflection of the pile.
 
         Parameters
         ----------
@@ -188,15 +301,15 @@
 
         .. image:: ../../docs/source/_static/usage/analyses_plots/forces_results_plot.png
             :width: 60%
         """
         fig = graphics.plot_forces(self)
         return fig if assign else None
 
-    def plot(self, assign=False):
+    def plot_lateral_results(self, assign=False):
         """Plots the pile deflection and sectional forces.
 
         Parameters
         ----------
         assign : bool, optional
             by default False
 
@@ -210,16 +323,58 @@
 
         .. image:: ../../docs/source/_static/usage/analyses_plots/main_results_plot.png
             :width: 60%
         """
         fig = graphics.plot_results(self)
         return fig if assign else None
 
+    def plot(self, assign=False):
+        """Same behaviour as :py:meth:`openpile.analyze.plot_lateral_results`.
 
-def simple_beam_analysis(model):
+        Parameters
+        ----------
+        assign : bool, optional
+            by default False
+
+        Returns
+        -------
+        None or matplotlib.pyplot.figure
+            if assign is True, a matplotlib figure is returned
+
+        """
+        return self.plot_lateral_results(assign)
+
+    def details(self) -> dict:
+        """Provide a summary of the results.
+
+        Returns
+        -------
+        dict
+            info on the results
+
+        """
+
+        return {
+            **self._details,
+            "Max. normal force [kN]": round(self._f["N [kN]"].max(), 2),
+            "Min. normal force [kN]": round(self._f["N [kN]"].min(), 2),
+            "Max. shear force [kN]": round(self._f["V [kN]"].max(), 2),
+            "Min. shear force [kN]": round(self._f["V [kN]"].min(), 2),
+            "Max. moment [kNm]": round(self._f["M [kNm]"].max(), 2),
+            "Min. moment [kNm]": round(self._f["M [kNm]"].min(), 2),
+            "Max. settlement [m]": round(self._d["Settlement [m]"].max(), 3),
+            "Min. settlement [m]": round(self._d["Settlement [m]"].min(), 3),
+            "Max. deflection [m]": round(self._d["Deflection [m]"].max(), 3),
+            "Min. deflection [m]": round(self._d["Deflection [m]"].min(), 3),
+            "Max. rotation [rad]": round(self._d["Rotation [rad]"].max(), 3),
+            "Min. rotation [rad]": round(self._d["Rotation [rad]"].min(), 3),
+        }
+
+
+def beam(model):
     """
     Function where loading or displacement defined in the model boundary conditions
     are used to solve the system of equations, .
 
     Parameters
     ----------
     model : `openpile.construct.Model` object
@@ -227,48 +382,59 @@
 
     Returns
     -------
     results : `openpile.compute.Result` object
         Results of the analysis
     """
 
-    if model.soil is None:
-        # initialise global force
-        F = kernel.mesh_to_global_force_dof_vector(model.global_forces)
-        # initiliase prescribed displacement vector
-        U = kernel.mesh_to_global_disp_dof_vector(model.global_disp)
-        # initialise global stiffness matrix
-        K = kernel.build_stiffness_matrix(model)
-        # initialise global supports vector
-        supports = kernel.mesh_to_global_restrained_dof_vector(model.global_restrained)
-
-        # validate boundary conditions
-        validation.check_boundary_conditions(model)
-
-        u, _ = kernel.solve_equations(K, F, U, restraints=supports)
+    # validate boundary conditions
+    validation.check_boundary_conditions(model)
 
-        # internal forces
-        q_int = kernel.struct_internal_force(model, u)
+    # initialise global force
+    F = kernel.mesh_to_global_force_dof_vector(model.global_forces)
+    # initiliase prescribed displacement vector
+    U = kernel.mesh_to_global_disp_dof_vector(model.global_disp)
+    # initialise global supports vector
+    supports = kernel.mesh_to_global_restrained_dof_vector(model.global_restrained)
+
+    # initialise displacement vectors
+    d = np.zeros(U.shape)
+
+    # initialise global stiffness matrix
+    K = kernel.build_stiffness_matrix(model, d)
+    # first run with no stress stiffness matrix
+    d, Q = kernel.solve_equations(K, F, U, restraints=supports)
+    # rerun global stiffness matrix
+    K = kernel.build_stiffness_matrix(model, d)
+    # second run with stress stiffness matrix
+    d, Q = kernel.solve_equations(K, F, U, restraints=supports)
+
+    # internal forces
+    q_int = kernel.pile_internal_forces(model, d)
+
+    # Final results
+    results = AnalyzeResult(
+        _name=f"{model.name} ({model.pile.name})",
+        _d=disp_to_df(model, d),
+        _f=structural_forces_to_df(model, q_int),
+        _Q=reaction_forces_to_df(model, Q),
+        _details={
+            "converged @ iter no.": 1,
+            "error": 0.0,
+            "tolerance": None,
+        },
+    )
 
-        # Final results
-        results = Result(
-            name=f"{model.name} ({model.pile.name}/{model.soil.name})",
-            displacements=disp_to_df(model, u),
-            forces=structural_forces_to_df(model, q_int),
-        )
+    return results
 
-        return results
 
-
-def simple_winkler_analysis(model, max_iter: int = 100):
+def winkler(model, max_iter: int = 100):
     """
     Function where loading or displacement defined in the model boundary conditions
-    are used to solve the system of equations, .
-
-    #TODO
+    are used to solve the system of equations via the iterative Newton-Raphson scheme.
 
     Parameters
     ----------
     model : `openpile.construct.Model` object
         Model where structure and boundary conditions are defined.
     max_iter: int, by defaut 100
         maximum number of iterations for convergence
@@ -285,83 +451,119 @@
     else:
         # initialise global force
         F = kernel.mesh_to_global_force_dof_vector(model.global_forces)
         # initiliase prescribed displacement vector
         U = kernel.mesh_to_global_disp_dof_vector(model.global_disp)
         # initialise displacement vectors
         d = np.zeros(U.shape)
-
         # initialise global stiffness matrix
-        K = kernel.build_stiffness_matrix(model, f=None, u=d, kind="initial")
-        # initialise internal forces
-        q_int = np.zeros((model.element_number * 6))
+        K = kernel.build_stiffness_matrix(model, u=d, kind="initial")
         # initialise global supports vector
         supports = kernel.mesh_to_global_restrained_dof_vector(model.global_restrained)
 
         # validate boundary conditions
         # validation.check_boundary_conditions(model)
 
         # Initialise residual forces
         Rg = F
 
         # incremental calculations to convergence
         iter_no = 0
         while iter_no <= max_iter:
+
             # solve system
             try:
                 u_inc, Q = kernel.solve_equations(K, Rg, U, restraints=supports)
+                # bump iteration number
+                iter_no += 1
             except np.linalg.LinAlgError:
                 print(
                     """Cannot converge. Failure of the pile-soil system.\n
                       Boundary conditions may not be realistic or values may be too large."""
                 )
                 break
 
             # External forces
             F_ext = F - Q
             control = np.linalg.norm(F_ext)
+            nr_tol = 1e-4 * control
 
             # add up increment displacements
             d += u_inc
 
             # calculate internal forces
-            K_secant = kernel.build_stiffness_matrix(model, f=q_int, u=d, kind="secant")
+            K_secant = kernel.build_stiffness_matrix(model, u=d, kind="secant")
             F_int = -K_secant.dot(d)
 
             # calculate residual forces
             Rg = F_ext + F_int
 
             # check if converged
-            if np.linalg.norm(Rg[~supports]) < 1e-4 * control:
+            if np.linalg.norm(Rg[~supports]) < nr_tol:
                 # do not accept convergence without iteration (without a second call to solve equations)
-                if iter_no > 0:
-                    print(f"Converged at iteration no. {iter_no}")
-                    break
+                print(f"Converged at iteration no. {iter_no}")
+                break
 
             if iter_no == 100:
                 print("Not converged after 100 iterations.")
 
-            # Internal forces calculations with dim(nelem,6,6)
-            q_int = kernel.struct_internal_force(model, q_int, d)
-
             # re-calculate global stiffness matrix for next iterations
-            K = kernel.build_stiffness_matrix(model, f=q_int, u=d, kind="tangent")
+            K = kernel.build_stiffness_matrix(model, u=d, kind="tangent")
 
             # reset prescribed displacements to converge properly in case
             # of displacement-driven analysis
             U[:] = 0.0
 
-            # nump iteration number
-            iter_no += 1
-
         # Internal forces calculations with dim(nelem,6,6)
-        q_int = kernel.struct_internal_force(model, q_int, d)
+        q_int = kernel.pile_internal_forces(model, d)
 
         # Final results
-        results = Result(
-            name=f"{model.name} ({model.pile.name}/{model.soil.name})",
-            displacements=disp_to_df(model, d),
-            forces=structural_forces_to_df(model, q_int),
-            springs_mobilization=springs_mob_to_df(model, d),
+        results = AnalyzeResult(
+            _name=f"{model.name} ({model.pile.name}/{model.soil.name})",
+            _d=disp_to_df(model, d),
+            _f=structural_forces_to_df(model, q_int),
+            _Q=reaction_forces_to_df(model, Q),
+            _dist_mob=springs_mob_to_df(model, d),
+            _hb_mob=(
+                abs(d[-2])
+                * kernel.calculate_base_spring_stiffness(d[-2], model._Hb_spring, kind="secant"),
+                model._Hb_spring.flatten().max(),
+            ),
+            _mb_mob=(
+                abs(d[-1])
+                * kernel.calculate_base_spring_stiffness(d[-1], model._Mb_spring, kind="secant"),
+                model._Mb_spring.flatten().max(),
+            ),
+            _details={
+                "converged @ iter no.": iter_no,
+                "error [kN]": round(np.linalg.norm(Rg[~supports]), 3),
+                "tolerance [kN]": round(nr_tol, 3),
+            },
         )
 
         return results
+
+
+def simple_winkler_analysis(model, max_iter: int = 100):
+
+    # deprecation warning
+    warnings.warn(
+        "\nThe method Analyze.simple_winkler_analysis() will be removed in version 1.0.0."
+        "\nPlease use the Analyze.winkler() instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+
+    return winkler(model, max_iter)
+
+
+def simple_beam_analysis(model):
+
+    # deprecation warning
+    warnings.warn(
+        "\nThe method Analyze.simple_beam_analysis() will be removed in version 1.0.0."
+        "\nPlease use the Analyze.beam() instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+
+    return beam(model)
```

### Comparing `openpile-0.3.3/src/openpile/construct.py` & `openpile-0.4.0/src/openpile/construct.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     root_validator,
     validator,
     PositiveFloat,
     confloat,
     conlist,
     constr,
     Extra,
+    ValidationError,
 )
 from pydantic.dataclasses import dataclass
 import matplotlib.pyplot as plt
 
 import openpile.utils.graphics as graphics
 import openpile.core.validation as validation
 import openpile.soilmodels as soilmodels
@@ -645,14 +646,82 @@
 
         for i in range(len(top_sorted) - 1):
             if not m.isclose(top_sorted[i + 1], bottom_sorted[i], abs_tol=0.001):
                 raise ValueError("Layers' elevations overlap.")
 
         return values
 
+    @root_validator
+    def check_multipliers_in_lateral_model(cls, values):
+        def check_multipliers_callable(multiplier, ground_level, top, bottom, type):
+            # if not a float, it must be a callable, then we check for Real Positive float
+            if not isinstance(multiplier, float):
+                # defines depth below ground to check
+                depths = ground_level - np.linspace(start=top, stop=bottom, num=100)
+                # check if positive real float is returned
+                for depth in depths:
+                    result = multiplier(depth)
+                    if not isinstance(result, float):
+                        TypeError(
+                            f"One or more results of the {type}-multiplier callable is not a float"
+                        )
+                        return None
+                    else:
+                        if type in ["p", "m"]:
+                            if result < 0.0:
+                                print(
+                                    f"One or more results of the {type}-multiplier callable is negative"
+                                )
+                                return None
+                        elif type in ["y", "t"]:
+                            if not result > 0.0:
+                                ValueError(
+                                    f"One or more results of the {type}-multiplier callable is not strictly positive"
+                                )
+                                return None
+
+        layers = values["layers"]
+
+        for layer in layers:
+            if layer.lateral_model is not None:
+                # check p-multipliers
+                check_multipliers_callable(
+                    layer.lateral_model.p_multiplier,
+                    values["top_elevation"],
+                    layer.top,
+                    layer.bottom,
+                    "p",
+                )
+                # check y-multipliers
+                check_multipliers_callable(
+                    layer.lateral_model.y_multiplier,
+                    values["top_elevation"],
+                    layer.top,
+                    layer.bottom,
+                    "y",
+                )
+                # check m-multipliers
+                check_multipliers_callable(
+                    layer.lateral_model.m_multiplier,
+                    values["top_elevation"],
+                    layer.top,
+                    layer.bottom,
+                    "m",
+                )
+                # check t-multipliers
+                check_multipliers_callable(
+                    layer.lateral_model.t_multiplier,
+                    values["top_elevation"],
+                    layer.top,
+                    layer.bottom,
+                    "t",
+                )
+
+        return values
+
     def __post_init__(self):
         pass
 
     def __str__(self):
         """List all layers in table-like format"""
         out = ""
         i = 0
@@ -943,15 +1012,15 @@
                         # p-y curves
                         if (
                             layer.lateral_model.spring_signature[0] and self.distributed_lateral
                         ):  # True if py spring function exist
 
                             # calculate springs (top and) for each element
                             for j in [0, 1]:
-                                (py[i, j, 0], py[i, j, 1]) = layer.lateral_model.py_spring_fct(
+                                (py[i, j, 1], py[i, j, 0]) = layer.lateral_model.py_spring_fct(
                                     sig=sig_v[j],
                                     X=depth_from_ground[j],
                                     layer_height=(layer.top - layer.bottom),
                                     depth_from_top_of_layer=(layer.top - elevation[j]),
                                     D=pile_width,
                                     L=(self.soil.top_elevation - self.pile.bottom_elevation),
                                     below_water_table=elevation[j] <= self.soil.water_line,
@@ -960,67 +1029,63 @@
 
                         if (
                             layer.lateral_model.spring_signature[2] and self.distributed_moment
                         ):  # True if mt spring function exist
 
                             # calculate springs (top and) for each element
                             for j in [0, 1]:
-                                (mt[i, j, 0], mt[i, j, 1]) = layer.lateral_model.mt_spring_fct(
+                                (mt[i, j, 1], mt[i, j, 0]) = layer.lateral_model.mt_spring_fct(
                                     sig=sig_v[j],
                                     X=depth_from_ground[j],
                                     layer_height=(layer.top - layer.bottom),
                                     depth_from_top_of_layer=(layer.top - elevation[j]),
                                     D=pile_width,
                                     L=(self.soil.top_elevation - self.pile.bottom_elevation),
                                     below_water_table=elevation[j] <= self.soil.water_line,
                                     output_length=spring_dim,
                                 )
 
-                        # check if pile tip is within layer
-                        if (
-                            layer.top >= self.pile.bottom_elevation
-                            and layer.bottom <= self.pile.bottom_elevation
-                        ):
-
-                            # Hb curve
-                            sig_v_tip = self.soil_properties["sigma_v bottom [kPa]"].iloc[-1]
-
-                            if layer.lateral_model.spring_signature[1] and self.base_shear:
-
-                                # calculate Hb spring
-                                (Hb[0, 0, 0], Hb[0, 0, 1]) = layer.lateral_model.Hb_spring_fct(
-                                    sig=sig_v_tip,
-                                    X=self.pile.bottom_elevation,
-                                    layer_height=(layer.top - layer.bottom),
-                                    depth_from_top_of_layer=(
-                                        layer.top - self.pile.bottom_elevation
-                                    ),
-                                    D=pile_width,
-                                    L=(self.soil.top_elevation - self.pile.bottom_elevation),
-                                    below_water_table=self.pile.bottom_elevation
-                                    <= self.soil.water_line,
-                                    output_length=spring_dim,
-                                )
-
-                            # Mb curve
-                            if layer.lateral_model.spring_signature[3] and self.base_moment:
-
-                                (Mb[0, 0, 0], Mb[0, 0, 1]) = layer.lateral_model.Mb_spring_fct(
-                                    sig=sig_v_tip,
-                                    X=self.pile.bottom_elevation,
-                                    layer_height=(layer.top - layer.bottom),
-                                    depth_from_top_of_layer=(
-                                        layer.top - self.pile.bottom_elevation
-                                    ),
-                                    D=pile_width,
-                                    L=(self.soil.top_elevation - self.pile.bottom_elevation),
-                                    below_water_table=self.pile.bottom_elevation
-                                    <= self.soil.water_line,
-                                    output_length=spring_dim,
-                                )
+                    # check if pile tip is within layer
+                    if (
+                        layer.top >= self.pile.bottom_elevation
+                        and layer.bottom <= self.pile.bottom_elevation
+                    ):
+
+                        # Hb curve
+                        sig_v_tip = self.soil_properties["sigma_v bottom [kPa]"].iloc[-1]
+
+                        if layer.lateral_model.spring_signature[1] and self.base_shear:
+
+                            # calculate Hb spring
+                            (Hb[0, 0, 1], Hb[0, 0, 0]) = layer.lateral_model.Hb_spring_fct(
+                                sig=sig_v_tip,
+                                X=-self.pile.bottom_elevation,
+                                layer_height=(layer.top - layer.bottom),
+                                depth_from_top_of_layer=(layer.top - self.pile.bottom_elevation),
+                                D=pile_width,
+                                L=(self.soil.top_elevation - self.pile.bottom_elevation),
+                                below_water_table=self.pile.bottom_elevation
+                                <= self.soil.water_line,
+                                output_length=spring_dim,
+                            )
+
+                        # Mb curve
+                        if layer.lateral_model.spring_signature[3] and self.base_moment:
+
+                            (Mb[0, 0, 1], Mb[0, 0, 0]) = layer.lateral_model.Mb_spring_fct(
+                                sig=sig_v_tip,
+                                X=-self.pile.bottom_elevation,
+                                layer_height=(layer.top - layer.bottom),
+                                depth_from_top_of_layer=(layer.top - self.pile.bottom_elevation),
+                                D=pile_width,
+                                L=(self.soil.top_elevation - self.pile.bottom_elevation),
+                                below_water_table=self.pile.bottom_elevation
+                                <= self.soil.water_line,
+                                output_length=spring_dim,
+                            )
 
             if check_springs(py):
                 print("py springs have negative or NaN values.")
                 print(
                     """if using PISA type springs, this can be due to parameters behind out of the parameter space.
                 Please check that: 2 < L/D < 6.
                 """
@@ -1127,32 +1192,14 @@
         # Initialise nodal global support with link to nodes_coordinates (used for defining boundary conditions)
         self.global_restrained = self.nodes_coordinates.copy()
         self.global_restrained["Tx"] = False
         self.global_restrained["Ty"] = False
         self.global_restrained["Rz"] = False
 
     @property
-    def py_springs(self) -> pd.DataFrame:
-        """Table with p-y springs computed for the given Model.
-
-        Returns
-        -------
-        pd.DataFrame (or None if no SoilProfile is present)
-            Table with p-y springs, i.e. p-value [kN/m] and y-value [m].
-        """
-        if self.soil is None:
-            return None
-        else:
-            return misc.get_springs(
-                springs=self._py_springs,
-                elevations=self.nodes_coordinates["x [m]"].values,
-                kind="p-y",
-            )
-
-    @property
     def embedment(self) -> float:
         """Pile embedment length [m].
 
         Returns
         -------
         float (or None if no SoilProfile is present)
             Pile embedment
@@ -1411,14 +1458,136 @@
                     print(
                         "Support not applied! The chosen elevation is not meshed as a node. Please include elevation in `x2mesh` variable when creating the Model."
                     )
         except Exception:
             print("\n!User Input Error! Please create Model first with the Model.create().\n")
             raise
 
+    def get_py_springs(self, kind: str = "node") -> pd.DataFrame:
+        """Table with p-y springs computed for the given Model.
+
+        Posible to extract the springs at the node level (i.e. spring at each node)
+        or element level (i.e. top and bottom springs at each element)
+
+        Parameters
+        ----------
+        kind : str
+            can be of ("node", "element").
+
+        Returns
+        -------
+        pd.DataFrame (or None if no SoilProfile is present)
+            Table with p-y springs, i.e. p-value [kN/m] and y-value [m].
+        """
+        if self.soil is None:
+            return None
+        else:
+            if kind == "element":
+                return misc.get_full_springs(
+                    springs=self._py_springs,
+                    elevations=self.nodes_coordinates["x [m]"].values,
+                    kind="p-y",
+                )
+            elif kind == "node":
+                return misc.get_reduced_springs(
+                    springs=self._py_springs,
+                    elevations=self.nodes_coordinates["x [m]"].values,
+                    kind="p-y",
+                )
+            else:
+                return None
+
+    def get_mt_springs(self, kind: str = "node") -> pd.DataFrame:
+        """Table with m-t (rotational) springs computed for the given Model.
+
+        Posible to extract the springs at the node level (i.e. spring at each node)
+        or element level (i.e. top and bottom springs at each element)
+
+        Parameters
+        ----------
+        kind : str
+            can be of ("node", "element").
+
+        Returns
+        -------
+        pd.DataFrame (or None if no SoilProfile is present)
+            Table with m-t springs, i.e. m-value [kNm] and t-value [-].
+        """
+        if self.soil is None:
+            return None
+        else:
+            if kind == "element":
+                return misc.get_full_springs(
+                    springs=self._mt_springs,
+                    elevations=self.nodes_coordinates["x [m]"].values,
+                    kind="m-t",
+                )
+            elif kind == "node":
+                return misc.get_reduced_springs(
+                    springs=self._mt_springs,
+                    elevations=self.nodes_coordinates["x [m]"].values,
+                    kind="m-t",
+                )
+            else:
+                return None
+
+    def get_Hb_spring(self) -> pd.DataFrame:
+        """Table with Hb (base shear) spring computed for the given Model.
+
+
+        Returns
+        -------
+        pd.DataFrame (or None if no SoilProfile is present)
+            Table with Hb spring, i.e. H-value [kN] and y-value [m].
+        """
+        if self.soil is None:
+            return None
+        else:
+            spring_dim = self._Hb_spring.shape[-1]
+
+            column_values_spring = [f"VAL {i}" for i in range(spring_dim)]
+
+            df = pd.DataFrame(
+                data={
+                    "Node no.": [self.element_number + 1] * 2,
+                    "Elevation [m]": [self.pile.bottom_elevation] * 2,
+                }
+            )
+            df["type"] = ["Hb", "y"]
+            df[column_values_spring] = self._Hb_spring.reshape(2, spring_dim)
+
+            return df
+
+    def get_Mb_spring(self) -> pd.DataFrame:
+        """Table with Mb (base moment) spring computed for the given Model.
+
+
+        Returns
+        -------
+        pd.DataFrame (or None if no SoilProfile is present)
+            Table with Mb spring, i.e. M-value [kNn] and t-value [-].
+        """
+        if self.soil is None:
+            return None
+        else:
+            spring_dim = self._Hb_spring.shape[-1]
+
+            column_values_spring = [f"VAL {i}" for i in range(spring_dim)]
+
+            df = pd.DataFrame(
+                data={
+                    "Node no.": [self.element_number + 1] * 2,
+                    "Elevation [m]": [self.pile.bottom_elevation] * 2,
+                }
+            )
+            df["type"] = ["Mb", "t"]
+            df[column_values_spring] = self._Hb_spring.reshape(2, spring_dim)
+
+            return df
+
     def plot(self, assign=False):
         """Create a plot of the model with the mesh and boundary conditions.
 
         Parameters
         ----------
         assign : bool, optional
             this parameter can be set to True to return the figure, by default False.
```

### Comparing `openpile-0.3.3/src/openpile/core/kernel.py` & `openpile-0.4.0/src/openpile/core/kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -450,24 +450,24 @@
             [N, B, D, N, -B, C],
         ]
     ) * (0.5 * ksoil[:, 0] + 0.5 * ksoil[:, 1])
 
     return km
 
 
-def elem_p_delta_stiffness_matrix(model, f):
+def elem_p_delta_stiffness_matrix(model, u):
     """creates stress stiffness matrix based on axial stress in pile.
 
     #TODO: proof here
 
     Parameters
     ----------
     model : openpile class object `openpile.construct.Model`
         includes information on soil/structure, elements, nodes and other model-related data.
-    f: np.ndarray
+    u: np.ndarray
         Global displacement vector
 
     Returns
     -------
     k: numpy array (3d)
         stress stiffness matrix of all elememts related to axial stress
 
@@ -478,14 +478,15 @@
 
     """
 
     # calculate length vector
     L = mesh_to_element_length(model)
 
     # internal forces
+    f = pile_internal_forces(model, u)
     P = f[::6].reshape(-1, 1, 1)
 
     # elastic properties
     nu = model.pile._nu
     E = model.element_properties["E [kPa]"].to_numpy(dtype=float).reshape((-1, 1, 1))
     G = E / (2 + 2 * nu)
     # cross-section properties
@@ -493,14 +494,16 @@
     A = model.element_properties["Area [m2]"].to_numpy(dtype=float).reshape((-1, 1, 1))
     d = model.element_properties["Diameter [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
     wt = model.element_properties["Wall thickness [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
 
     # calculate shear component in stiffness matrix (if Timorshenko)
     if model.element_type == "EulerBernoulli":
         N = 0 * L
+        N1 = 0 * L
+        N2 = 0 * L
         A = 6 / (5 * L)
         B = N + 1 / 10
         C = 2 * L / 15
         D = -L / 30
     elif model.element_type == "Timoshenko":
         if model.pile.kind == "Circular":
             a = 0.5 * d
@@ -519,14 +522,16 @@
 
         else:
             raise ValueError("Timoshenko beams cannot be used yet for non-circular pile types")
 
         phi = (12 * omega + 1) ** 2
 
         N = 0 * L
+        N1 = 0 / L
+        N2 = 0 / L
         A = 6 * (120 * omega**2 + 20 * omega + 1) / ((5 * L) * phi) + 12 * I / (A * L**3 * phi)
         B = 1 / (10 * phi) + 6 * I / (A * L**2 * phi)
         C = (2 * L * (90 * omega**2 + 15 * omega + 1)) / (15 * phi) + 4 * I * (
             36 * omega**2 + 6 * omega + 1
         ) / (A * L * phi)
         D = -L * (360 * omega**2 + 60 * omega + 1) / (30 * phi) - 2 * I * (
             72 * omega**2 + 12 * omega - 1
@@ -536,20 +541,20 @@
         raise ValueError(
             "Model.element.type only accepts 'EB' type (for Euler-Bernoulli) of 'T' type (for Timoshenko)"
         )
 
     k = (
         np.block(
             [
-                [N, N, N, N, N, N],
+                [N, N, N1, N, N, N2],
                 [N, A, B, N, -A, B],
-                [N, B, C, N, -B, D],
-                [N, N, N, N, N, N],
+                [N1, B, C, -N1, -B, D],
+                [N, N, -N1, N, N, -N2],
                 [N, -A, -B, N, A, -B],
-                [N, B, D, N, -B, C],
+                [N2, B, D, -N2, -B, C],
             ]
         )
         * -P
     )
 
     return k
 
@@ -569,15 +574,15 @@
 
         # update global stiffness matrix
         K += K_temp
 
     return K
 
 
-def build_stiffness_matrix(model, f, u=None, kind=None):
+def build_stiffness_matrix(model, u=None, kind=None):
     """Builds the stiffness matrix based on the model(element and node) properties
 
     Element stiffness matrices are first computed for each element and then loaded in the global stiffness matrix through summation.
     Different element stiffness matrices are computed depending on the specifications found in the Model object.
 
     Parameters
     ----------
@@ -605,16 +610,16 @@
     # number of elements in mesh
     n_elem = model.element_number
     # global dimension of the global stiffness matrix can be inferred
     ndim_global = ndof_per_node * n_elem + ndof_per_node
 
     # mechanical stiffness properties
     k = elem_mechanical_stiffness_matrix(model)
-    if f is not None:
-        k += elem_p_delta_stiffness_matrix(model, f=f)
+    k += elem_p_delta_stiffness_matrix(model, u)
+
     # add soil contribution
     if model.soil is not None:
         # gives warning if soil is given without displacements or type of stiffness
         if u is None or kind is None:
             UserWarning("'u' and 'kind' must be stipulated.")
         else:
             if model.distributed_lateral:
@@ -625,15 +630,15 @@
                     raise UserInputError(
                         "Error: Distributed moment cannot be calculated without distributed lateral springs."
                     )
                 k += elem_mt_stiffness_matrix(model, u, kind)
 
     K = jit_build(k, ndim_global, n_elem, node_per_element, ndof_per_node)
 
-    # add soil contribution
+    # add base springs contribution
     if model.soil is not None:
         if model.base_shear:
             K[-2, -2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
 
         if model.base_moment:
             K[-1, -1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
 
@@ -657,36 +662,22 @@
 def mesh_to_global_restrained_dof_vector(df: pd.DataFrame) -> np.ndarray:
     # extract each column (one line per node)
     restrained_dof_vector = df[["Tx", "Ty", "Rz"]].values.reshape(-1)
 
     return restrained_dof_vector
 
 
-def struct_internal_force(model, f, u) -> np.ndarray:
+def pile_internal_forces(model, u):
     # number of dof per node
     ndof_per_node = 3
     # number of nodes per element
     node_per_element = 2
 
     # create mech consistent stiffness matrix
     k = elem_mechanical_stiffness_matrix(model)
-    if f is not None:
-        k += elem_p_delta_stiffness_matrix(model, f=f)
-
-    # add soil contribution
-    if model.soil is not None:
-        kind = "secant"
-        if model.distributed_lateral:
-            k += elem_py_stiffness_matrix(model, u, kind)
-        if model.distributed_moment:
-            k += elem_mt_stiffness_matrix(model, u, kind)
-        if model.base_shear:
-            k[-1, -2, -2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
-        if model.base_moment:
-            k[-1, -1, -1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
 
     # create array u of shape [n_elem x 6 x 1]
     u = global_dof_vector_to_consistent_stacked_array(u, ndof_per_node * node_per_element)
     # compute internal forces and reshape into global dof vector
     F_int = (-1) * np.matmul(k, u).reshape((-1))
 
     return F_int
```

### Comparing `openpile-0.3.3/src/openpile/core/txt.py` & `openpile-0.4.0/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.3/src/openpile/core/validation.py` & `openpile-0.4.0/src/openpile/core/validation.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.3/src/openpile/soilmodels.py` & `openpile-0.4.0/src/openpile/soilmodels.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """
 `SoilModels` module
 ===================
+
 """
 
+# Guide to create soil models
+# ---------------------------
+#
+#
+
+
 # Import libraries
 import math as m
 import numpy as np
 import pandas as pd
 from numba import njit, prange
 
-from typing import List, Dict, Optional, Union
+from typing import List, Dict, Optional, Union, Callable
 from typing_extensions import Literal
 from pydantic import (
     BaseModel,
     Field,
     root_validator,
     PositiveFloat,
     confloat,
     conlist,
     Extra,
 )
 from pydantic.dataclasses import dataclass
 
 from openpile.core.misc import from_list2x_parse_top_bottom, var_to_str
-from openpile.utils import py_curves, Hb_curves, mt_curves, Mb_curves
+from openpile.utils import py_curves, Hb_curves, mt_curves, Mb_curves, tz_curves
 
 
 # CONSTITUTIVE MODELS CLASSES ---------------------------------
 
 
 class PydanticConfigFrozen:
     arbitrary_types_allowed = True
     allow_mutation = False
-    extra = Extra.forbid
 
 
 class ConstitutiveModel:
     pass
 
 
 class LateralModel(ConstitutiveModel):
@@ -44,62 +50,70 @@
 
 
 class AxialModel(ConstitutiveModel):
     pass
 
 
 @dataclass(config=PydanticConfigFrozen)
-class API_clay(AxialModel):
+class API_clay_axial(AxialModel):
+
     #: undrained shear strength [kPa], if a variation in values, two values can be given.
     Su: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: t-multiplier
-    t_multiplier: confloat(ge=0.0) = 1.0
+    t_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: z-multiplier
-    z_multiplier: confloat(gt=0.0) = 1.0
+    z_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
     #: Q-multiplier
     Q_multiplier: confloat(ge=0.0) = 1.0
     #: w-multiplier
     w_multiplier: confloat(gt=0.0) = 1.0
 
     def __str__(self):
         return f"\tAPI clay\n\tSu = {var_to_str(self.Su)} kPa"
 
 
 @dataclass(config=PydanticConfigFrozen)
 class Cowden_clay(LateralModel):
-    """A class to establish the PISA Cowden clay model.
+    """A class to establish the PISA Cowden clay model as per Byrne et al 2020 (see [BHBG20]_).
 
     Parameters
     ----------
     Su: float or list[top_value, bottom_value]
         Undrained shear strength. Value to range from 0 to 100 [unit: kPa]
     G0: float or list[top_value, bottom_value]
         Small-strain shear modulus [unit: kPa]
-    p_multiplier: float
+    p_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for p-values
-    y_multiplier: float
+    y_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for y-values
-    m_multiplier: float
+    m_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for m-values
-    t_multiplier: float
+    t_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for t-values
+
+    See also
+    --------
+    :py:func:`openpile.utils.py_curves.cowden_clay`, :py:func:`openpile.utils.mt_curves.cowden_clay`,
+    :py:func:`openpile.utils.Hb_curves.cowden_clay`, :py:func:`openpile.utils.Mb_curves.cowden_clay`
+
+
     """
 
     #: Undrained shear strength [kPa], if a variation in values, two values can be given.
     Su: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: small-strain shear stiffness modulus [kPa]
     G0: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: p-multiplier
-    p_multiplier: confloat(ge=0.0) = 1.0
+    p_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: y-multiplier
-    y_multiplier: confloat(gt=0.0) = 1.0
+    y_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
     #: m-multiplier
-    m_multiplier: confloat(ge=0.0) = 1.0
+    m_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: t-multiplier
-    t_multiplier: confloat(gt=0.0) = 1.0
+    t_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
 
     # spring signature which tells that API sand only has p-y curves
     # signature if of the form [p-y:True, Hb:False, m-t:False, Mb:False]
     spring_signature = np.array([True, True, True, True], dtype=bool)
 
     def __str__(self):
         return f"\Cowden clay (PISA)\n\tSu = {var_to_str(self.Su)} kPa.\n\tG0 = {round(self.G0/1000,1)} MPa"
@@ -123,23 +137,27 @@
         # define Dr
         Su_t, Su_b = from_list2x_parse_top_bottom(self.Su)
         Su = Su_t + (Su_b - Su_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        p, y = py_curves.cowden_clay(
+        y, p = py_curves.cowden_clay(
             X=X,
             Su=Su,
             G0=Gmax,
             D=D,
             output_length=output_length,
         )
 
-        return p * self.p_multiplier, y * self.y_multiplier
+        # parse multipliers and apply results
+        y_mult = self.y_multiplier if isinstance(self.y_multiplier, float) else self.y_multiplier(X)
+        p_mult = self.p_multiplier if isinstance(self.p_multiplier, float) else self.p_multiplier(X)
+
+        return y * y_mult, p * p_mult
 
     def Hb_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -156,24 +174,24 @@
         # define Dr
         Su_t, Su_b = from_list2x_parse_top_bottom(self.Su)
         Su = Su_t + (Su_b - Su_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        Hb, y = Hb_curves.cowden_clay(
+        y, Hb = Hb_curves.cowden_clay(
             X=X,
             Su=Su,
             G0=Gmax,
             D=D,
             L=L,
             output_length=output_length,
         )
 
-        return Hb, y
+        return y, Hb
 
     def mt_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -190,35 +208,39 @@
         # define Dr
         Su_t, Su_b = from_list2x_parse_top_bottom(self.Su)
         Su = Su_t + (Su_b - Su_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        p_array, _ = py_curves.cowden_clay(
+        _, p_array = py_curves.cowden_clay(
             X=X,
             Su=Su,
             G0=Gmax,
             D=D,
             output_length=output_length,
         )
 
         m = np.zeros((output_length, output_length), dtype=np.float32)
         t = np.zeros((output_length, output_length), dtype=np.float32)
 
         for count, _ in enumerate(p_array):
-            m[count, :], t[count, :] = mt_curves.cowden_clay(
+            t[count, :], m[count, :] = mt_curves.cowden_clay(
                 X=X,
                 Su=Su,
                 G0=Gmax,
                 D=D,
                 output_length=output_length,
             )
 
-        return m * self.m_multiplier, t * self.t_multiplier
+        # parse multipliers and apply results
+        t_mult = self.t_multiplier if isinstance(self.t_multiplier, float) else self.t_multiplier(X)
+        m_mult = self.m_multiplier if isinstance(self.m_multiplier, float) else self.m_multiplier(X)
+
+        return t * t_mult, m * m_mult
 
     def Mb_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -235,58 +257,64 @@
         # define Dr
         Su_t, Su_b = from_list2x_parse_top_bottom(self.Su)
         Su = Su_t + (Su_b - Su_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        Mb, y = Mb_curves.cowden_clay(
+        y, Mb = Mb_curves.cowden_clay(
             X=X,
             Su=Su,
             G0=Gmax,
             D=D,
             L=L,
             output_length=output_length,
         )
 
-        return Mb, y
+        return y, Mb
 
 
 @dataclass(config=PydanticConfigFrozen)
 class Dunkirk_sand(LateralModel):
-    """A class to establish the PISA Dunkirk sand model.
+    """A class to establish the PISA Dunkirk sand model as per  Burd et al (2020) (see [BTZA20]_)..
 
     Parameters
     ----------
     Dr: float or list[top_value, bottom_value]
         relative density of sand. Value to range from 0 to 100. [unit: -]
     G0: float or list[top_value, bottom_value]
         Small-strain shear modulus [unit: kPa]
-    p_multiplier: float
+    p_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for p-values
-    y_multiplier: float
+    y_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for y-values
-    m_multiplier: float
+    m_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for m-values
-    t_multiplier: float
+    t_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for t-values
+
+    See also
+    --------
+    :py:func:`openpile.utils.py_curves.dunkirk_sand`, :py:func:`openpile.utils.mt_curves.dunkirk_sand`,
+    :py:func:`openpile.utils.Hb_curves.dunkirk_sand`, :py:func:`openpile.utils.Mb_curves.dunkirk_sand`
+
     """
 
     #: soil friction angle [deg], if a variation in values, two values can be given.
     Dr: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: small-strain shear stiffness modulus [kPa]
     G0: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: p-multiplier
-    p_multiplier: confloat(ge=0.0) = 1.0
+    p_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: y-multiplier
-    y_multiplier: confloat(gt=0.0) = 1.0
+    y_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
     #: m-multiplier
-    m_multiplier: confloat(ge=0.0) = 1.0
+    m_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: t-multiplier
-    t_multiplier: confloat(gt=0.0) = 1.0
+    t_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
 
     # spring signature which tells that API sand only has p-y curves
     # signature if of the form [p-y:True, Hb:False, m-t:False, Mb:False]
     spring_signature = np.array([True, True, True, True], dtype=bool)
 
     def __str__(self):
         return f"\tDunkirk sand (PISA)\n\tDr = {var_to_str(self.Dr)}%. \n\tG0 = {round(self.G0/1000,1)} MPa"
@@ -310,25 +338,29 @@
         # define Dr
         Dr_t, Dr_b = from_list2x_parse_top_bottom(self.Dr)
         Dr = Dr_t + (Dr_b - Dr_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        p, y = py_curves.dunkirk_sand(
+        y, p = py_curves.dunkirk_sand(
             sig=sig,
             X=X,
             Dr=Dr,
             G0=Gmax,
             D=D,
             L=L,
             output_length=output_length,
         )
 
-        return p * self.p_multiplier, y * self.y_multiplier
+        # parse multipliers and apply results
+        y_mult = self.y_multiplier if isinstance(self.y_multiplier, float) else self.y_multiplier(X)
+        p_mult = self.p_multiplier if isinstance(self.p_multiplier, float) else self.p_multiplier(X)
+
+        return y * y_mult, p * p_mult
 
     def Hb_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -345,25 +377,25 @@
         # define Dr
         Dr_t, Dr_b = from_list2x_parse_top_bottom(self.Dr)
         Dr = Dr_t + (Dr_b - Dr_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        Hb, y = Hb_curves.dunkirk_sand(
+        y, Hb = Hb_curves.dunkirk_sand(
             sig=sig,
             X=X,
             Dr=Dr,
             G0=Gmax,
             D=D,
             L=L,
             output_length=output_length,
         )
 
-        return Hb, y
+        return y, Hb
 
     def mt_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -380,40 +412,44 @@
         # define Dr
         Dr_t, Dr_b = from_list2x_parse_top_bottom(self.Dr)
         Dr = Dr_t + (Dr_b - Dr_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        p_array, _ = py_curves.dunkirk_sand(
+        _, p_array = py_curves.dunkirk_sand(
             sig=sig,
             X=X,
             Dr=Dr,
             G0=Gmax,
             D=D,
             L=L,
             output_length=output_length,
         )
 
         m = np.zeros((output_length, output_length), dtype=np.float32)
         t = np.zeros((output_length, output_length), dtype=np.float32)
 
         for count, p_iter in enumerate(p_array):
-            m[count], t[count, :] = mt_curves.dunkirk_sand(
+            t[count, :], m[count] = mt_curves.dunkirk_sand(
                 sig=sig,
                 X=X,
                 Dr=Dr,
                 G0=Gmax,
                 p=p_iter,
                 D=D,
                 L=L,
                 output_length=output_length,
             )
 
-        return m * self.m_multiplier, t * self.t_multiplier
+        # parse multipliers and apply results
+        t_mult = self.t_multiplier if isinstance(self.t_multiplier, float) else self.t_multiplier(X)
+        m_mult = self.m_multiplier if isinstance(self.m_multiplier, float) else self.m_multiplier(X)
+
+        return t * t_mult, m * m_mult
 
     def Mb_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -430,56 +466,77 @@
         # define Dr
         Dr_t, Dr_b = from_list2x_parse_top_bottom(self.Dr)
         Dr = Dr_t + (Dr_b - Dr_t) * depth_from_top_of_layer / layer_height
         # define G0
         G0_t, G0_b = from_list2x_parse_top_bottom(self.G0)
         Gmax = G0_t + (G0_b - G0_t) * depth_from_top_of_layer / layer_height
 
-        Mb, y = Mb_curves.dunkirk_sand(
+        y, Mb = Mb_curves.dunkirk_sand(
             sig=sig,
             X=X,
             Dr=Dr,
             G0=Gmax,
             D=D,
             L=L,
             output_length=output_length,
         )
 
-        return Mb, y
+        return y, Mb
 
 
 @dataclass(config=PydanticConfigFrozen)
 class API_sand(LateralModel):
     """A class to establish the API sand model.
 
     Parameters
     ----------
     phi: float or list[top_value, bottom_value]
         internal angle of friction in degrees
     kind: str, by default "static"
         types of curves, can be of ("static","cyclic")
-    p_multiplier: float
+    G0: float or list[top_value, bottom_value] or None
+        Small-strain shear modulus [unit: kPa], by default None
+    p_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for p-values
-    y_multiplier: float
+    y_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for y-values
+    extension: str, by default None
+        turn on extensions by calling them in this variable
+        for API_sand, rotational springs can be added to the model with the extension "mt_curves"
+
+    See also
+    --------
+    :py:func:`openpile.utils.py_curves.api_sand`
 
     """
 
     #: soil friction angle [deg], if a variation in values, two values can be given.
     phi: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: types of curves, can be of ("static","cyclic")
-    kind: Literal["static", "cyclic"]
+    kind: Literal["static", "cyclic"] = "static"
+    #: small-strain stiffness [kPa], if a variation in values, two values can be given.
+    G0: Optional[Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]] = None
     #: p-multiplier
-    p_multiplier: confloat(ge=0.0) = 1.0
+    p_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: y-multiplier
-    y_multiplier: confloat(gt=0.0) = 1.0
-
-    # spring signature which tells that API sand only has p-y curves
-    # signature if of the form [p-y:True, Hb:False, m-t:False, Mb:False]
-    spring_signature = np.array([True, False, False, False], dtype=bool)
+    y_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
+    #: extensions available for soil model
+    extension: Optional[Literal["mt_curves"]] = None
+
+    # define class variables needed for all soil models
+    m_multiplier = 1.0
+    t_multiplier = 1.0
+
+    def __post_init__(self):
+        # spring signature which tells that API sand only has p-y curves in normal conditions
+        # signature if e.g. of the form [p-y:True, Hb:False, m-t:False, Mb:False]
+        if self.extension == "mt_curves":
+            self.spring_signature = np.array([True, False, True, False], dtype=bool)
+        else:
+            self.spring_signature = np.array([True, False, False, False], dtype=bool)
 
     def __str__(self):
         return f"\tAPI sand\n\tphi = {var_to_str(self.phi)}°\n\t{self.kind} curves"
 
     def py_spring_fct(
         self,
         sig: float,
@@ -496,26 +553,91 @@
         if depth_from_top_of_layer > layer_height:
             raise ValueError("Spring elevation outside layer")
 
         # define phi
         phi_t, phi_b = from_list2x_parse_top_bottom(self.phi)
         phi = phi_t + (phi_b - phi_t) * depth_from_top_of_layer / layer_height
 
-        p, y = py_curves.api_sand(
+        y, p = py_curves.api_sand(
             sig=sig,
             X=X,
             phi=phi,
             D=D,
             kind=self.kind,
             below_water_table=below_water_table,
             ymax=ymax,
             output_length=output_length,
         )
 
-        return p * self.p_multiplier, y * self.y_multiplier
+        # parse multipliers and apply results
+        y_mult = self.y_multiplier if isinstance(self.y_multiplier, float) else self.y_multiplier(X)
+        p_mult = self.p_multiplier if isinstance(self.p_multiplier, float) else self.p_multiplier(X)
+
+        return y * y_mult, p * p_mult
+
+    def mt_spring_fct(
+        self,
+        sig: float,
+        X: float,
+        layer_height: float,
+        depth_from_top_of_layer: float,
+        D: float,
+        L: float = None,
+        below_water_table: bool = True,
+        ymax: float = 0.0,
+        output_length: int = 15,
+    ):
+        # validation
+        if depth_from_top_of_layer > layer_height:
+            raise ValueError("Spring elevation outside layer")
+
+        # define phi
+        phi_t, phi_b = from_list2x_parse_top_bottom(self.phi)
+        phi = phi_t + (phi_b - phi_t) * depth_from_top_of_layer / layer_height
+
+        # define p vector
+        _, p = py_curves.api_sand(
+            sig=sig,
+            X=X,
+            phi=phi,
+            D=D,
+            kind=self.kind,
+            below_water_table=below_water_table,
+            ymax=ymax,
+            output_length=output_length,
+        )
+
+        if p.max() > 0:
+            p_norm = p / p.max()
+        else:
+            p_norm = p
+
+        m = np.zeros((output_length, output_length), dtype=np.float32)
+        t = np.zeros((output_length, output_length), dtype=np.float32)
+
+        z, tz = tz_curves.api_sand(
+            sig=sig,
+            delta=phi - 5,
+            K=0.8,
+            tensile_factor=1.0,
+            output_length=output_length,
+        )
+
+        # trasnform tz vector
+        tz_pos = tz[tz >= 0]
+        z_pos = z[z >= 0]
+        diff_length_t = output_length - len(tz_pos)
+        diff_length_z = output_length - len(z_pos)
+        tz_pos = np.append(tz_pos, [tz_pos[-1]] * diff_length_t)
+        z_pos = np.append(z_pos, [z_pos[-1] + i * 0.1 for i in range(diff_length_z)])
+
+        t = np.arctan(z_pos.reshape((1, -1)) / (0.5 * D)) * np.ones((output_length, 1))
+        m = 1 / 4 * np.pi * D**2 * tz_pos.reshape((1, -1)) * p_norm.reshape((-1, 1))
+
+        return t, m
 
 
 @dataclass(config=PydanticConfigFrozen)
 class API_clay(LateralModel):
     """A class to establish the API clay model.
 
     Parameters
@@ -524,41 +646,63 @@
         Undrained shear strength in kPa
     eps50: float or list[top_value, bottom_value]
         strain at 50% failure load [-]
     J: float
         empirical factor varying depending on clay stiffness, varies between 0.25 and 0.50
     stiff_clay_threshold: float
         undrained shear strength [kPa] at which stiff clay curve is computed
+    G0: float or list[top_value, bottom_value] or None
+        Small-strain shear modulus [unit: kPa], by default None
     kind: str, by default "static"
         types of curves, can be of ("static","cyclic")
-    p_multiplier: float
+    p_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for p-values
-    y_multiplier: float
+    y_multiplier: float or function taking the depth as argument and returns the multiplier
         multiplier for y-values
+    extension: str, by default None
+        turn on extensions by calling them in this variable
+        for API_clay, rotational springs can be added to the model with the extension "mt_curves"
+
+
+    See also
+    --------
+    :py:func:`openpile.utils.py_curves.api_clay`
 
     """
 
     #: undrained shear strength [kPa], if a variation in values, two values can be given.
     Su: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: strain at 50% failure load [-], if a variation in values, two values can be given.
     eps50: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: types of curves, can be of ("static","cyclic")
-    kind: Literal["static", "cyclic"]
+    kind: Literal["static", "cyclic"] = "static"
+    #: small-strain stiffness [kPa], if a variation in values, two values can be given.
+    G0: Optional[Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]] = None
     #: empirical factor varying depending on clay stiffness
     J: confloat(ge=0.25, le=0.5) = 0.5
     #: undrained shear strength [kPa] at which stiff clay curve is computed
     stiff_clay_threshold: PositiveFloat = 96
     #: p-multiplier
-    p_multiplier: confloat(ge=0.0) = 1.0
+    p_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
     #: y-multiplier
-    y_multiplier: confloat(gt=0.0) = 1.0
-
-    # spring signature which tells that API sand only has p-y curves
-    # signature if of the form [p-y:True, Hb:False, m-t:False, Mb:False]
-    spring_signature = np.array([True, False, False, False], dtype=bool)
+    y_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
+    #: extensions available for soil model
+    extension: Optional[Literal["mt_curves"]] = None
+
+    # define class variables needed for all soil models
+    m_multiplier = 1.0
+    t_multiplier = 1.0
+
+    def __post_init__(self):
+        # spring signature which tells that API clay only has p-y curves in normal conditions
+        # signature if e.g. of the form [p-y:True, Hb:False, m-t:False, Mb:False]
+        if self.extension == "mt_curves":
+            self.spring_signature = np.array([True, False, True, False], dtype=bool)
+        else:
+            self.spring_signature = np.array([True, False, False, False], dtype=bool)
 
     def __str__(self):
         return f"\tAPI clay\n\tSu = {var_to_str(self.Su)} kPa\n\teps50 = {var_to_str(self.eps50)}\n\t{self.kind} curves"
 
     def py_spring_fct(
         self,
         sig: float,
@@ -579,21 +723,73 @@
         Su_t, Su_b = from_list2x_parse_top_bottom(self.Su)
         Su = Su_t + (Su_b - Su_t) * depth_from_top_of_layer / layer_height
 
         # define eps50
         eps50_t, eps50_b = from_list2x_parse_top_bottom(self.eps50)
         eps50 = eps50_t + (eps50_b - eps50_t) * depth_from_top_of_layer / layer_height
 
-        p, y = py_curves.api_clay(
+        y, p = py_curves.api_clay(
             sig=sig,
             X=X,
             Su=Su,
             eps50=eps50,
             D=D,
             J=self.J,
             stiff_clay_threshold=self.stiff_clay_threshold,
             kind=self.kind,
             ymax=ymax,
             output_length=output_length,
         )
 
-        return p * self.p_multiplier, y * self.y_multiplier
+        # parse multipliers and apply results
+        y_mult = self.y_multiplier if isinstance(self.y_multiplier, float) else self.y_multiplier(X)
+        p_mult = self.p_multiplier if isinstance(self.p_multiplier, float) else self.p_multiplier(X)
+
+        return y * y_mult, p * p_mult
+
+    def mt_spring_fct(
+        self,
+        sig: float,
+        X: float,
+        layer_height: float,
+        depth_from_top_of_layer: float,
+        D: float,
+        L: float = None,
+        below_water_table: bool = True,
+        ymax: float = 0.0,
+        output_length: int = 15,
+    ):
+        # validation
+        if depth_from_top_of_layer > layer_height:
+            raise ValueError("Spring elevation outside layer")
+
+        # define Su
+        Su_t, Su_b = from_list2x_parse_top_bottom(self.Su)
+        Su = Su_t + (Su_b - Su_t) * depth_from_top_of_layer / layer_height
+
+        m = np.zeros((output_length, output_length), dtype=np.float32)
+        t = np.zeros((output_length, output_length), dtype=np.float32)
+
+        z, tz = tz_curves.api_clay(
+            sig=sig,
+            Su=Su,
+            D=D,
+            residual=1.0,
+            tensile_factor=1.0,
+            output_length=output_length,
+        )
+
+        # trasnform tz vector so that we only get the positive side of the vectors
+        tz_pos = tz[tz >= 0]
+        z_pos = z[z >= 0]
+        # check how many elements we got rid off
+        diff_length_t = output_length - len(tz_pos)
+        diff_length_z = output_length - len(z_pos)
+        # add new elements at the end of the positive only vectors
+        tz_pos = np.append(tz_pos, [tz_pos[-1]] * diff_length_t)
+        z_pos = np.append(z_pos, [z_pos[-1] + i * 0.1 for i in range(diff_length_z)])
+
+        # calculate m and t vectors (they are all the same for clay)
+        t = np.arctan(z_pos.reshape((1, -1)) / (0.5 * D)) * np.ones((output_length, 1))
+        m = 1 / 4 * np.pi * D**2 * tz_pos.reshape((1, -1)) * np.ones((output_length, 1))
+
+        return t, m
```

### Comparing `openpile-0.3.3/src/openpile/utils/Hb_curves.py` & `openpile-0.4.0/src/openpile/utils/Hb_curves.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     G0: float,
     D: float,
     L: float,
     output_length: int = 20,
 ):
     """
     Creates the base shear spring from the PISA sand formulation
-    published by Burd et al (2020).
+    published by Burd et al (2020) (see [BTZA20]_).
     Also called the General Dunkirk Sand Model (GDSM).
 
     Parameters
     ----------
     sig : float
         vertical/overburden effective stress [unit: kPa]
     X : float
@@ -57,43 +57,43 @@
 
     # Generalised Dunkirk Sand Model parameters
     v_hu1 = 0.5150 + 2.883 * Dr
     v_hu2 = 0.1695 - 0.7018 * Dr
     k_h1 = 6.505 - 2.985 * Dr
     k_h2 = -0.007969 - 0.4299 * Dr
     n_h1 = 0.09978 + 0.7974 * Dr
-    n_h2 = 0.004994 + 0.07005 * Dr
+    n_h2 = 0.004994 - 0.07005 * Dr
     p_u1 = 0.09952 + 0.7996 * Dr
     p_u2 = 0.03988 - 0.1606 * Dr
 
     # Depth variation parameters
     v_max = v_hu1 + v_hu2 * L / D
     k = k_h1 + k_h2 * L / D
     n = n_h1 + n_h2 * L / D
     p_max = p_u1 + p_u2 * L / D
 
     # calculate normsalised conic function
     y, p = conic(v_max, n, k, p_max, output_length)
 
     # return non-normalised curve
-    return p * (sig * D**2), y * (sig * D / G0)
+    return y * (sig * D / G0), p * (sig * D**2)
 
 
 @njit(cache=True)
 def cowden_clay(
     X: float,
     Su: float,
     G0: float,
     D: float,
     L: float,
     output_length: int = 20,
 ):
     """
     Creates the base shear spring from the PISA clay formulation
-    published by Byrne et al (2020) and calibrated based pile
+    published by Byrne et al 2020 (see [BHBG20]_) and calibrated based pile
     load tests at Cowden (north east coast of England).
 
     Parameters
     ----------
     X : float
         Depth below ground level [unit: m]
     Su : float
@@ -109,14 +109,22 @@
 
     Returns
     -------
     1darray
         Hb vector [unit: kN]
     1darray
         y vector [unit: m]
+
+    References
+    ----------
+    .. [1] Byrne, B. W., Houlsby, G. T., Burd, H. J., Gavin, K. G., Igoe, D. J. P., Jardine,
+           R. J., Martin, C. M., McAdam, R. A., Potts, D. M., Taborda, D. M. G. & Zdravkovic ́,
+           L. (2020). PISA design model for monopiles for offshore wind turbines: application
+           to a stiff glacial clay till. Géotechnique, https://doi.org/10.1680/ jgeot.18.P.255.
+
     """
 
     # Generalised Dunkirk Sand Model parameters
     v_hu1 = 235.7
     v_hu2 = 0.00
     k_h1 = 2.717
     k_h2 = -0.3575
@@ -131,8 +139,8 @@
     n = n_h1 + n_h2 * L / D
     p_max = p_u1 + p_u2 * L / D
 
     # calculate normsalised conic function
     y, p = conic(v_max, n, k, p_max, output_length)
 
     # return non-normalised curve
-    return p * (Su * D**2), y * (Su * D / G0)
+    return y * (Su * D / G0), p * (Su * D**2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openpile-0.3.3/src/openpile/utils/Mb_curves.py` & `openpile-0.4.0/src/openpile/utils/Mb_curves.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     G0: float,
     D: float,
     L: float,
     output_length: int = 20,
 ):
     """
     Create the base moment springs from the PISA clay formulation
-    published by Byrne et al (2020) and calibrated based pile load tests
-    at Cowden (north east coast of England).
+    published by Byrne et al 2020 (see [BHBG20]_) and calibrated based pile
+    load tests at Cowden (north east coast of England).
 
     Parameters
     ----------
     X : float
         Depth below ground level [unit: m]
     Su : float
         Undrained shear strength [unit: kPa]
@@ -44,14 +44,15 @@
 
     Returns
     -------
     1darray
         Mb vector [unit: kN]
     1darray
         t vector of length [unit: rad]
+
     """
 
     # Cowden clay parameters
     k_m1 = 0.2146
     k_m2 = -0.002132
     n_m1 = 1.079
     n_m2 = -0.1087
@@ -65,30 +66,30 @@
     m_max = m_m1 + m_m2 * L / D
     psi_max = psi_u
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (Su * D**3), t * (Su / G0)
+    return t * (Su / G0), m * (Su * D**3)
 
 
 @njit(cache=True)
 def dunkirk_sand(
     sig: float,
     X: float,
     Dr: float,
     G0: float,
     D: float,
     L: float,
     output_length: int = 20,
 ):
     """
     Create the base moment spring from the PISA sand
-    formulation published by Burd et al (2020).
+    formulation published by Burd et al (2020) (see [BTZA20]_).
     Also called the General Dunkirk Sand Model (GDSM)
 
     Parameters
     ----------
     sig : float
         vertical/overburden effective stress [unit: kPa]
     X : float
@@ -128,8 +129,8 @@
     m_max = m_u1 + m_u2 * L / D
     psi_max = psi_u
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (sig * D**3), t * (sig / G0)
+    return t * (sig / G0), m * (sig * D**3)
```

### Comparing `openpile-0.3.3/src/openpile/utils/graphics.py` & `openpile-0.4.0/src/openpile/utils/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 mpl.rcParams["figure.subplot.wspace"] = 0.4
 
 
 def plot_deflection(result):
     fig, ax = plt.subplots()
 
-    fig.suptitle(f"{result.name} - Pile Deflection")
+    fig.suptitle(f"{result._name} - Pile Deflection")
 
     ax = U_plot(ax, result)
 
     return fig
 
 
 def plot_forces(result):
     # create 4 subplots with (deflectiom, normal force, shear force, bending moment)
 
     fig, (ax1, ax2, ax3) = plt.subplots(1, 3)
 
-    fig.suptitle(f"{result.name} - Sectional forces")
+    fig.suptitle(f"{result._name} - Sectional forces")
 
     ax1 = F_plot(ax1, result, "N [kN]")
     ax2 = F_plot(ax2, result, "V [kN]")
     ax3 = F_plot(ax3, result, "M [kNm]")
 
     for axis in [ax2, ax3]:
         axis.set_yticklabels("")
@@ -43,15 +43,15 @@
 
 
 def plot_results(result):
     # create 4 subplots with (deflectiom, normal force, shear force, bending moment)
 
     fig, (ax1, ax2, ax3, ax4) = plt.subplots(1, 4)
 
-    fig.suptitle(f"{result.name} - Analysis results")
+    fig.suptitle(f"{result._name} - Analysis results")
 
     ax1 = U_plot(ax1, result)
     ax2 = F_plot(ax2, result, "N [kN]")
     ax3 = F_plot(ax3, result, "V [kN]")
     ax4 = F_plot(ax4, result, "M [kNm]")
 
     for axis in [ax2, ax3, ax4]:
```

### Comparing `openpile-0.3.3/src/openpile/utils/mt_curves.py` & `openpile-0.4.0/src/openpile/utils/mt_curves.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     Su: float,
     G0: float,
     D: float,
     output_length: int = 20,
 ):
     """
     Create the rotational springs from the PISA clay formulation
-    published by Byrne et al (2020) and calibrated based pile load tests
-    at Cowden (north east coast of England).
+    published by Byrne et al 2020 (see [BHBG20]_) and calibrated based pile
+    load tests at Cowden (north east coast of England).
 
     Parameters
     ----------
     X : float
         Depth below ground level [unit: m]
     Su : float
         Undrained shear strength [unit: kPa]
@@ -41,14 +41,15 @@
 
     Returns
     -------
     1darray
         m vector [unit: kN]
     1darray
         t vector of length [unit: rad]
+
     """
 
     # Cowden clay parameters
     k_m1 = 1.420
     k_m2 = -0.09643
     n_m1 = 0.00
     n_m2 = 0.00
@@ -61,15 +62,15 @@
     m_max = m_m1 + m_m2 * X / D
     psi_max = m_max / k
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (Su * D**2), t * (Su / G0)
+    return t * (Su / G0), m * (Su * D**2)
 
 
 @njit(cache=True)
 def dunkirk_sand(
     sig: float,
     X: float,
     Dr: float,
@@ -77,15 +78,15 @@
     p: float,
     D: float,
     L: float,
     output_length: int = 20,
 ):
     """
     Create the rotational springs from the PISA sand
-    formulation published by Burd et al (2020).
+    formulation published by Burd et al (2020) (see [BTZA20]_).
     Also called the General Dunkirk Sand Model (GDSM)
 
     Parameters
     ----------
     sig : float
         vertical/overburden effective stress [unit: kPa]
     X : float
@@ -129,8 +130,8 @@
     m_max = m_u1 + m_u2 * X / L
     psi_max = m_max / k
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (p * D), t * (sig / G0)
+    return t * (sig / G0), m * (p * D)
```

### Comparing `openpile-0.3.3/src/openpile/utils/py_curves.py` & `openpile-0.4.0/src/openpile/utils/py_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Su: float,
     G0: float,
     D: float,
     output_length: int = 20,
 ):
     """
     Creates the lateral springs from the PISA clay formulation
-    published by Byrne et al (2020) and calibrated based pile
+    published by Byrne et al 2020 (see [BHBG20]_) and calibrated based pile
     load tests at Cowden (north east coast of England).
 
     Parameters
     ----------
     X : float
         Depth below ground level [unit: m]
     Su : float
@@ -41,14 +41,15 @@
 
     Returns
     -------
     1darray
         p vector [unit: kN/m]
     1darray
         y vector [unit: m]
+
     """
 
     # # Cowden clay parameters
     v_pu = 241.4
     k_p1 = 10.6
     k_p2 = -1.650
     n_p1 = 0.9390
@@ -62,30 +63,30 @@
     n = n_p1 + n_p2 * X / D
     p_max = p_u1 + p_u2 * m.exp(-0.3085 * X / D)
 
     # calculate normsalised conic function
     y, p = conic(v_max, n, k, p_max, output_length)
 
     # return non-normalised curve
-    return p * (Su * D), y * (Su * D / G0)
+    return y * (Su * D / G0), p * (Su * D)
 
 
 @njit(cache=True)
 def dunkirk_sand(
     sig: float,
     X: float,
     Dr: float,
     G0: float,
     D: float,
     L: float,
     output_length: int = 20,
 ):
     """
     Creates the lateral spring from the PISA sand formulation
-    published by Burd et al (2020).
+    published  by Burd et al (2020) (see [BTZA20]_).
     Also called the General Dunkirk Sand Model (GDSM).
 
     Parameters
     ----------
     sig : float
         vertical/overburden effective stress [unit: kPa]
     X : float
@@ -125,15 +126,15 @@
     n = n_p
     p_max = p_u1 + p_u2 * X / L
 
     # calculate normsalised conic function
     y, p = conic(v_max, n, k, p_max, output_length)
 
     # return non-normalised curve
-    return p * (sig * D), y * (sig * D / G0)
+    return y * (sig * D / G0), p * (sig * D)
 
 
 # API sand function
 @njit(parallel=True, cache=True)
 def api_sand(
     sig: float,
     X: float,
@@ -223,18 +224,18 @@
     p = np.zeros(shape=len(y), dtype=np.float32)
     for i in prange(len(y)):
         if Pmax == 0:
             p[i] = 0
         else:
             p[i] = A * Pmax * m.tanh((k_phi * X * y[i]) / (A * Pmax))
 
-    return p, y
+    return y, p
 
 
-# API sand function
+# API clay function
 @njit(parallel=True, cache=True)
 def api_clay(
     sig: float,
     X: float,
     Su: float,
     eps50: float,
     D: float,
@@ -350,8 +351,8 @@
                     else:
                         p[i] = 0.5 * Pmax * (y[i] / y50) ** 0.33
 
         # modification of initial slope of the curve (DNVGL RP-C203 B.2.2.4)
         if y[i] == 0.1 * y50:
             p[i] = 0.23 * Pmax
 
-    return p, y
+    return y, p
```

### Comparing `openpile-0.3.3/src/openpile/utils/qz_curves.py` & `openpile-0.4.0/src/openpile/utils/qz_curves.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # Import libraries
 import math as m
 import numpy as np
 from numba import njit, prange
 from random import random
 
+import openpile.utils.misc as misc
+
 # SPRING FUNCTIONS --------------------------------------------
 
 # API sand function
 @njit(cache=True)
 def api_sand(
     sig: float,
     delta: float,
@@ -41,24 +43,16 @@
     numpy 1darray
         z vector [unit: m]
     """
     # cannot have less than 8
     if output_length < 8:
         output_length = 8
 
-    # important variables
-    delta_table = np.array([0, 15, 20, 25, 30, 35, 100], dtype=np.float32)
-    Nq_table = np.array([8, 8, 12, 20, 40, 50, 50], dtype=np.float32)
-    Qmax_table = np.array([1900, 1900, 2900, 4800, 9600, 12000, 12000], dtype=np.float32)
-
-    Nq = np.interp(delta, delta_table, Nq_table)
-    Qmax = np.interp(delta, delta_table, Qmax_table)
-
-    # Unit end-bearing [kPa]
-    f = min(Qmax, sig * Nq)
+    # unit toe reistance [kPa]
+    f = misc._Qmax_api_sand(sig, delta)
 
     # piecewise function
     zlist = [-0.002, 0.0, 0.002, 0.013, 0.042, 0.073, 0.100, 0.200]
     Qlist = [0.0, 0.0, 0.25, 0.50, 0.75, 0.90, 1.00, 1.00]
 
     # determine z vector
     z = np.array(zlist, dtype=np.float32) * D
@@ -78,15 +72,15 @@
     Q = np.append(Q, add_Q_values)
 
     z = np.sort(z)
     z_id_sorted = np.argsort(z)
 
     Q = Q[z_id_sorted]
 
-    return Q, z
+    return z, Q
 
 
 # API clay Q-z function
 @njit(cache=True)
 def api_clay(
     Su: float,
     D: float,
@@ -111,16 +105,16 @@
     numpy 1darray
         z vector [unit: m]
     """
     # cannot have less than 8
     if output_length < 8:
         output_length = 8
 
-    # Unit end-bearing [kPa]
-    f = 9 * Su
+    # unit toe reistance [kPa]
+    f = misc._Qmax_api_clay
 
     # piecewise function
     zlist = [-0.002, 0.0, 0.002, 0.013, 0.042, 0.073, 0.100, 0.200]
     Qlist = [0.0, 0.0, 0.25, 0.50, 0.75, 0.90, 1.00, 1.00]
 
     # determine z vector
     z = np.array(zlist, dtype=np.float32) * D
@@ -140,8 +134,8 @@
     Q = np.append(Q, add_Q_values)
 
     z = np.sort(z)
     z_id_sorted = np.argsort(z)
 
     Q = Q[z_id_sorted]
 
-    return Q, z
+    return z, Q
```

### Comparing `openpile-0.3.3/src/openpile.egg-info/PKG-INFO` & `openpile-0.4.0/src/openpile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.3.3
+Version: 0.4.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
@@ -26,15 +26,15 @@
 # OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
-[![Downloads](https://static.pepy.tech/badge/openpile)](https://pepy.tech/project/openpile)
+[![Downloads](https://static.pepy.tech/badge/openpile/month)](https://pepy.tech/project/openpile)
 
 ![Tests](https://github.com/TchilDill/openpile/actions/workflows/Test.yml/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/openpile/badge/?version=latest)](https://openpile.readthedocs.io/en/latest/?badge=latest)
 
 
 [![issues closed](https://img.shields.io/github/issues-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/issues)
 [![PRs closed](https://img.shields.io/github/issues-pr-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/pulls)
```

### Comparing `openpile-0.3.3/src/openpile.egg-info/SOURCES.txt` & `openpile-0.4.0/src/openpile.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/openpile/__init__.py
-src/openpile/analyses.py
+src/openpile/analyze.py
+src/openpile/calculate.py
 src/openpile/construct.py
 src/openpile/globals.py
 src/openpile/soilmodels.py
 src/openpile.egg-info/PKG-INFO
 src/openpile.egg-info/SOURCES.txt
 src/openpile.egg-info/dependency_links.txt
 src/openpile.egg-info/not-zip-safe
@@ -19,14 +20,16 @@
 src/openpile/core/misc.py
 src/openpile/core/txt.py
 src/openpile/core/validation.py
 src/openpile/utils/Hb_curves.py
 src/openpile/utils/Mb_curves.py
 src/openpile/utils/__init__.py
 src/openpile/utils/graphics.py
+src/openpile/utils/misc.py
 src/openpile/utils/mt_curves.py
+src/openpile/utils/multipliers.py
 src/openpile/utils/py_curves.py
 src/openpile/utils/qz_curves.py
 src/openpile/utils/tz_curves.py
 test/test_construct.py
 test/test_pycurves.py
 test/test_utils_misc.py
```

### Comparing `openpile-0.3.3/test/test_construct.py` & `openpile-0.4.0/test/test_construct.py`

 * *Files 3% similar despite different names*

```diff
@@ -259,8 +259,11 @@
                                         )]
                 ),
                 )
         except Exception:
             assert False, f"Constructor does not work"
         
         # check that p_y springs are all zero
-        assert not np.all(model.py_springs[['VAL 0','VAL 1', 'VAL 2']].values)
+        assert not np.all( model.get_py_springs()[['VAL 0','VAL 1','VAL 2']].values )
+
+        # # check that m_t springs are all zero
+        # assert not np.all( model.get_mt_springs()[['VAL 0','VAL 1','VAL 2']].values )
```

### Comparing `openpile-0.3.3/test/test_pycurves.py` & `openpile-0.4.0/test/test_pycurves.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 @pytest.mark.parametrize("xX",[0.1,5,20])
 @pytest.mark.parametrize("xphi",[27,35,40])
 @pytest.mark.parametrize("xD",[0.2,1.5,5.0,10.0])
 @pytest.mark.parametrize("xkind",["static","cyclic"])
 @pytest.mark.parametrize("xwater",[True,False])
 def test_api_sand(make_pmax_api_sand,xsigma,xX, xphi, xD, xkind, xwater):
     #create spring
-    p, y = py.api_sand(sig=xsigma,X=xX,phi=xphi, D=xD, kind=xkind, below_water_table=xwater)
+    y, p = py.api_sand(sig=xsigma,X=xX,phi=xphi, D=xD, kind=xkind, below_water_table=xwater)
     #helper fct
     is_sorted = lambda a: np.all(a[:-1] <= a[1:])
     #check if sorted
     assert is_sorted(y)
     assert is_sorted(p)
     #check if origin is (0,0)
     assert p[0] == 0.0
@@ -80,15 +80,15 @@
 @pytest.mark.parametrize("xSu",[0.01,50,125,300])
 @pytest.mark.parametrize("xe50",[0.005,0.0125,0.03])
 @pytest.mark.parametrize("xD",[0.2,1.5,5.0,10.0])
 @pytest.mark.parametrize("xJ",[0.25,0.5])
 @pytest.mark.parametrize("xkind",["static","cyclic"])
 def test_api_clay(make_pmax_api_clay,xsigma, xX, xSu, xe50, xD, xJ, xkind):
     #create spring
-    p, y = py.api_clay(sig=xsigma, X=xX, Su=xSu, eps50=xe50, D=xD, J=xJ, kind=xkind)
+    y, p = py.api_clay(sig=xsigma, X=xX, Su=xSu, eps50=xe50, D=xD, J=xJ, kind=xkind)
     #helper fct
     is_sorted = lambda a: np.all(a[:-1] <= a[1:])
     #check if sorted
     assert is_sorted(y)
     #check if origin is (0,0)
     assert p[0] == 0.0
     assert y[0] == 0.0
```

### Comparing `openpile-0.3.3/test/test_utils_misc.py` & `openpile-0.4.0/test/test_utils_misc.py`

 * *Files identical despite different names*

