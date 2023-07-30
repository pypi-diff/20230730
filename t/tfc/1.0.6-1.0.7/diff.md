# Comparing `tmp/tfc-1.0.6.tar.gz` & `tmp/tfc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfc-1.0.6.tar", last modified: Sun Jul 30 04:56:34 2023, max compression
+gzip compressed data, was "tfc-1.0.7.tar", last modified: Sun Jul 30 05:42:11 2023, max compression
```

## Comparing `tfc-1.0.6.tar` & `tfc-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.398536 tfc-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-30 04:56:27.000000 tfc-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 04:56:27.000000 tfc-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-30 04:56:34.398536 tfc-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-30 04:56:27.000000 tfc-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-30 04:56:27.000000 tfc-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:56:34.398536 tfc-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-30 04:56:27.000000 tfc-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/tfc/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/mtfc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utfc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/tfc/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.398536 tfc-1.0.6/src/tfc/utils/BF/
--rw-r--r--   0 runner    (1001) docker     (123)    44920 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    28381 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.h
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.i
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.py
--rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF_Py.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/CeSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/Html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/Latex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/MakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/MayaviMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/PlotlyMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    58232 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/TFCUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/tfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:11.047412 tfc-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-30 05:42:04.000000 tfc-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 05:42:04.000000 tfc-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-07-30 05:42:11.047412 tfc-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-30 05:42:04.000000 tfc-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-30 05:42:04.000000 tfc-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:42:11.047412 tfc-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-30 05:42:04.000000 tfc-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:11.043412 tfc-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:11.043412 tfc-1.0.7/src/tfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/mtfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utfc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:11.047412 tfc-1.0.7/src/tfc/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:11.047412 tfc-1.0.7/src/tfc/utils/BF/
+-rw-r--r--   0 runner    (1001) docker     (123)    44920 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/BF.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    28381 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/BF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/BF.i
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/BF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/BF_Py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/BF/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/CeSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/Html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/Latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/MakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/MayaviMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/PlotlyMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58232 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/TFCUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-30 05:42:04.000000 tfc-1.0.7/src/tfc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:42:11.043412 tfc-1.0.7/src/tfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-07-30 05:42:11.000000 tfc-1.0.7/src/tfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-30 05:42:11.000000 tfc-1.0.7/src/tfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:42:11.000000 tfc-1.0.7/src/tfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 05:42:11.000000 tfc-1.0.7/src/tfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-30 05:42:11.000000 tfc-1.0.7/src/tfc.egg-info/top_level.txt
```

### Comparing `tfc-1.0.6/LICENSE` & `tfc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/PKG-INFO` & `tfc-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.6
+Version: 1.0.7
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 * More accurate solutions
 * Faster solutions
 * Robustness to initial guess
 
 For more information on the appliation of TFC to differential equations and its benefits see the [Mathematical documentation](#mathematical-documentation).
 
 ## Installation:
-The following instructions can be used to install a source distribution via pip or build TFC directly from source. Currently, we support building TFC navitely on Linux or macOS, but Windows users can still use TFC via the Windows Subsystem for Linux.
+The following instructions can be used to install a source distribution via pip or build TFC directly from source. 
 
 To install via pip run:
 ```bash
 pip install --upgrade pip setuptools wheel numpy
 pip install --upgrade tfc
 ```
 The above will install a binary TFC wheel. The developers have found that installing a source distribution leads to code that is slightly faster on some machines, as the code is compiled using potentially newer versions of compilers and swig. If you would like the source distribution, then you can use the following:
@@ -81,15 +81,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.6},
+    version = {1.0.7},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.6/README.md` & `tfc-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 * More accurate solutions
 * Faster solutions
 * Robustness to initial guess
 
 For more information on the appliation of TFC to differential equations and its benefits see the [Mathematical documentation](#mathematical-documentation).
 
 ## Installation:
-The following instructions can be used to install a source distribution via pip or build TFC directly from source. Currently, we support building TFC navitely on Linux or macOS, but Windows users can still use TFC via the Windows Subsystem for Linux.
+The following instructions can be used to install a source distribution via pip or build TFC directly from source. 
 
 To install via pip run:
 ```bash
 pip install --upgrade pip setuptools wheel numpy
 pip install --upgrade tfc
 ```
 The above will install a binary TFC wheel. The developers have found that installing a source distribution leads to code that is slightly faster on some machines, as the code is compiled using potentially newer versions of compilers and swig. If you would like the source distribution, then you can use the following:
@@ -62,15 +62,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.6},
+    version = {1.0.7},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.6/pyproject.toml` & `tfc-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">=3.9"
 name = "tfc"
-version = "1.0.6"
+version = "1.0.7"
 
 [build-system]
 requires = ["setuptools>=42", 
             "wheel", 
             "numpy>=1.22",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `tfc-1.0.6/setup.py` & `tfc-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/mtfc.py` & `tfc-1.0.7/src/tfc/mtfc.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utfc.py` & `tfc-1.0.7/src/tfc/utfc.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/BF/BF.cxx` & `tfc-1.0.7/src/tfc/utils/BF/BF.cxx`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/BF/BF.h` & `tfc-1.0.7/src/tfc/utils/BF/BF.h`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/BF/BF.i` & `tfc-1.0.7/src/tfc/utils/BF/BF.i`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     #include <cuda.h>
     #include <cuda_runtime.h>
     #include <cuda_runtime_api.h>
 #endif
 #include "BF.h"
 %}
 
+%feature("python:annotations", "c");
+
 %include "numpy.i"
 %include <typemaps.i>
 %include <attribute.i>
 %apply bool* INPUT {bool* useVal};
 
 %init %{
         import_array();
```

### Comparing `tfc-1.0.6/src/tfc/utils/BF/BF.py` & `tfc-1.0.7/src/tfc/utils/BF/BF.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/BF/BF_Py.py` & `tfc-1.0.7/src/tfc/utils/BF/BF_Py.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/BF/numpy.i` & `tfc-1.0.7/src/tfc/utils/BF/numpy.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/CeSolver.py` & `tfc-1.0.7/src/tfc/utils/CeSolver.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/Html.py` & `tfc-1.0.7/src/tfc/utils/Html.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/Latex.py` & `tfc-1.0.7/src/tfc/utils/Latex.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/MakePlot.py` & `tfc-1.0.7/src/tfc/utils/MakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/MayaviMakePlot.py` & `tfc-1.0.7/src/tfc/utils/MayaviMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/PlotlyMakePlot.py` & `tfc-1.0.7/src/tfc/utils/PlotlyMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/TFCUtils.py` & `tfc-1.0.7/src/tfc/utils/TFCUtils.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc/utils/types.py` & `tfc-1.0.7/src/tfc/utils/types.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.6/src/tfc.egg-info/PKG-INFO` & `tfc-1.0.7/src/tfc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.6
+Version: 1.0.7
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 * More accurate solutions
 * Faster solutions
 * Robustness to initial guess
 
 For more information on the appliation of TFC to differential equations and its benefits see the [Mathematical documentation](#mathematical-documentation).
 
 ## Installation:
-The following instructions can be used to install a source distribution via pip or build TFC directly from source. Currently, we support building TFC navitely on Linux or macOS, but Windows users can still use TFC via the Windows Subsystem for Linux.
+The following instructions can be used to install a source distribution via pip or build TFC directly from source. 
 
 To install via pip run:
 ```bash
 pip install --upgrade pip setuptools wheel numpy
 pip install --upgrade tfc
 ```
 The above will install a binary TFC wheel. The developers have found that installing a source distribution leads to code that is slightly faster on some machines, as the code is compiled using potentially newer versions of compilers and swig. If you would like the source distribution, then you can use the following:
@@ -81,15 +81,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.6},
+    version = {1.0.7},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.6/src/tfc.egg-info/SOURCES.txt` & `tfc-1.0.7/src/tfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

