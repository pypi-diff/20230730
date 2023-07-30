# Comparing `tmp/tfc-1.0.5.tar.gz` & `tmp/tfc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfc-1.0.5.tar", last modified: Mon Jun  5 18:47:06 2023, max compression
+gzip compressed data, was "tfc-1.0.6.tar", last modified: Sun Jul 30 04:56:34 2023, max compression
```

## Comparing `tfc-1.0.5.tar` & `tfc-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 18:46:59.000000 tfc-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 18:46:59.000000 tfc-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-05 18:47:06.847995 tfc-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-05 18:46:59.000000 tfc-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 18:47:00.000000 tfc-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:47:06.847995 tfc-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-05 18:47:00.000000 tfc-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.843995 tfc-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.843995 tfc-1.0.5/src/tfc/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/mtfc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utfc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/src/tfc/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/src/tfc/utils/BF/
--rw-r--r--   0 runner    (1001) docker     (123)    44710 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.h
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.i
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.py
--rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF_Py.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/CeSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/Html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/Latex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/MakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/MayaviMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/PlotlyMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    58232 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/TFCUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/src/tfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.398536 tfc-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-30 04:56:27.000000 tfc-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 04:56:27.000000 tfc-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-30 04:56:34.398536 tfc-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-30 04:56:27.000000 tfc-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-30 04:56:27.000000 tfc-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:56:34.398536 tfc-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-30 04:56:27.000000 tfc-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/tfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/mtfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utfc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/tfc/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.398536 tfc-1.0.6/src/tfc/utils/BF/
+-rw-r--r--   0 runner    (1001) docker     (123)    44920 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    28381 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.i
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/BF_Py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/BF/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/CeSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/Html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/Latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/MakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/MayaviMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/PlotlyMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58232 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/TFCUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-30 04:56:27.000000 tfc-1.0.6/src/tfc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:56:34.394536 tfc-1.0.6/src/tfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-30 04:56:34.000000 tfc-1.0.6/src/tfc.egg-info/top_level.txt
```

### Comparing `tfc-1.0.5/LICENSE` & `tfc-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/PKG-INFO` & `tfc-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Education
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Theory of Functional Connections (TFC)
 **A functional interpolation framework with applications in solving differential equations.**
 
@@ -80,15 +81,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.5},
+    version = {1.0.6},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.5/README.md` & `tfc-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.5},
+    version = {1.0.6},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.5/pyproject.toml` & `tfc-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [project]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
+name = "tfc"
+version = "1.0.6"
 
 [build-system]
 requires = ["setuptools>=42", 
             "wheel", 
-            "numpy>=1.15",
+            "numpy>=1.22",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
-target-version = ['py38','py39','py310','py311']
+target-version = ['py39','py310','py311']
 
 [tool.cibuildwheel]
 before-build = "pip install setuptools wheel numpy"
 skip = "pp* *-musllinux*"
 manylinux-x86_64-image = "manylinux2014"
 test-requires = ["pytest"]
 test-command = "pytest {package}/tests"
 
 [tool.cibuildwheel.linux]
 before-all = "yum install -y swig"
 archs = ["x86_64"]
 
 [tool.cibuildwheel.macos]
 before-all = "brew install swig"
-archs = ["x86_64"]
+archs = ["x86_64", "arm64"]
+
+[tool.cibuildwheel.windows]
+archs = ["AMD64"]
 
 [[tool.cibuildwheel.overrides]]
 select = "*-musllinux*"
 before-all = "apk add swig"
```

### Comparing `tfc-1.0.5/setup.py` & `tfc-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from os import path
+from os import path, name
 import numpy
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_py import build_py as _build_py
 
 # Get long description
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
@@ -19,37 +19,41 @@
 # Get version info
 version_dict = {}
 with open('src/tfc/version.py') as f:
   exec(f.read(), version_dict)
   version = version_dict["__version__"]
 
 # In the future, can add -DHAS_CUDA to this to enable GPU support
-cxxFlags = ["-O3", "-std=c++17", "-Wall", "-Wextra", "-Wno-unused-parameter", "-fPIC"]
+if name == 'nt':
+    # Windows compile flags
+    cxxFlags = ["/O2", "/std:c++17", "/Wall", "/DWINDOWS_MSVC"]
+else:
+    cxxFlags = ["-O3", "-std=c++17", "-Wall", "-Wextra", "-Wno-unused-parameter", "-fPIC"]
+
+if sys.version_info >= (3, 8):	
+    numpy_version = "numpy>=1.23.0"	
+else:	
+    numpy_version = "numpy>=1.21.0"	
 
 # Create basis function c++ extension
 BF = Extension(
     "tfc.utils.BF._BF",
     sources=["src/tfc/utils/BF/BF.i","src/tfc/utils/BF/BF.cxx"],
     include_dirs=["src/tfc/utils/BF", numpy_include],
-    swig_opts=["-c++"],
+    swig_opts=["-c++", "-doxygen", "-O", "-olddefs"],
     extra_compile_args=cxxFlags,
     extra_link_args=cxxFlags,
 )
 
 # Custom build options to include swig Python files
 class build_py(_build_py):
     def run(self):
         self.run_command("build_ext")
         super(build_py, self).run()
 
-if sys.version_info >= (3, 8):
-    numpy_version = "numpy>=1.23.0"
-else:
-    numpy_version = "numpy>=1.21.0"
-
 # Setup
 setup(
     name="tfc",
     version=version,
     author="Carl Leake and Hunter Johnston",
     author_email="leakec57@gmail.com",
     description="Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.",
```

### Comparing `tfc-1.0.5/src/tfc/mtfc.py` & `tfc-1.0.6/src/tfc/mtfc.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     pint,
     NumberListOrArray,
     JaxOrNumpyArray,
     IntArrayLike,
     Array,
     Tuple,
 )
-from jax import core, abstract_arrays
+from jax import core
 from jax.interpreters import ad, batching, xla
 from jax.lib import xla_client
 
 from .utils.TFCUtils import TFCPrint
 
 
 class mtfc:
@@ -558,24 +558,24 @@
             return self.basisClass.H(np.array(x), d, full)
 
         H_p.def_impl(H_impl)
 
         # Define abstract evaluation
         def H_abstract_eval(
             *x, d: npt.NDArray[onp.int32] = d0, full: bool = False
-        ) -> abstract_arrays.ShapedArray:
+        ) -> core.ShapedArray:
             if full:
                 dim1 = self.basisClass.numBasisFuncFull
             else:
                 dim1 = self.basisClass.numBasisFunc
             if len(x[0].shape) == 0:
                 dims = (dim1,)
             else:
                 dims = (x[0].shape[0], dim1)
-            return abstract_arrays.ShapedArray(dims, x[0].dtype)
+            return core.ShapedArray(dims, x[0].dtype)
 
         H_p.def_abstract_eval(H_abstract_eval)
 
         if self._backend == "C++":
             # XLA compilation
             def H_xla(c, *x, d: npt.NDArray[onp.int32] = d0, full: bool = False):
                 c = _unpack_builder(c)
```

### Comparing `tfc-1.0.5/src/tfc/utfc.py` & `tfc-1.0.6/src/tfc/utfc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 config.update("jax_enable_x64", True)
 
 import numpy as onp
 import jax.numpy as np
 import numpy.typing as npt
 from typing import Optional, cast
 from .utils.types import Literal, uint, IntArrayLike, JaxOrNumpyArray
-from jax import core, abstract_arrays
+from jax import core
 from jax.interpreters import ad, batching, xla
 from jax.lib import xla_client
 
 from .utils.TFCUtils import TFCPrint
 
 
 class utfc:
@@ -300,24 +300,24 @@
         # Implicit translation
         def H_impl(x: npt.NDArray, d: uint = 0, full=False) -> npt.NDArray:
             return self.basisClass.H(x, d, full)
 
         H_p.def_impl(H_impl)
 
         # Abstract evaluation
-        def H_abstract_eval(x, d: uint = 0, full: bool = False) -> abstract_arrays.ShapedArray:
+        def H_abstract_eval(x, d: uint = 0, full: bool = False) -> core.ShapedArray:
             if full:
                 dim1 = self.basisClass.m
             else:
                 dim1 = self.basisClass.m - self.basisClass.numC
             if len(x.shape) == 0:
                 dims = (dim1,)
             else:
                 dims = (x.shape[0], dim1)
-            return abstract_arrays.ShapedArray(dims, x.dtype)
+            return core.ShapedArray(dims, x.dtype)
 
         H_p.def_abstract_eval(H_abstract_eval)
 
         if self._backend == "C++":
             # XLA compilation
             def H_xla(c, x, d: uint = 0, full: bool = False):
                 c = _unpack_builder(c)
```

### Comparing `tfc-1.0.5/src/tfc/utils/BF/BF.cxx` & `tfc-1.0.6/src/tfc/utils/BF/BF.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-#include <iostream>
-#include <vector>
-#include <math.h>
-#include <float.h>
-#include <Python.h>
-#ifdef HAS_CUDA
-	#include <cuda.h>
-	#include <cuda_runtime.h>
-	#include <cuda_runtime_api.h>
-#endif
 #include "BF.h"
 
 // Initialize static BasisFunc variables
 int BasisFunc::nIdentifier = 0;
 std::vector<BasisFunc*> BasisFunc::BasisFuncContainer;
 
 // xlaWrapper function
@@ -853,15 +843,20 @@
 	return;
 };
 
 // ELM Swish: **********************************************************************
 
 void ELMSwish::Hint(const int d, const double* x, const int nOut, double* dark){
 	int j,k;
+#ifdef WINDOWS_MSVC
+    double* sig = new double[nOut*m];
+    double* zint = new double[nOut*m];
+#else
 	double sig[nOut*m], zint[nOut*m];
+#endif
 
 	if (d == 0){
 		for (j=0;j<nOut;j++){
 			for (k=0;k<m;k++)
 				dark[m*j+k] =  (w[k]*x[j]+b[k]) * 1./(1.+exp(-w[k]*x[j]-b[k]));
 		}
 
@@ -928,14 +923,20 @@
 					for (k=0;k<m;k++)
 						dark[m*j+k] = pow(w[k],8)*( 8.*( sig[m*j+k]-127.*pow(sig[m*j+k],2)+1932.*pow(sig[m*j+k],3)-10206.*pow(sig[m*j+k],4)+25200.*pow(sig[m*j+k],5)-31920.*pow(sig[m*j+k],6)+20160.*pow(sig[m*j+k],7)-5040.*pow(sig[m*j+k],8) ) + zint[m*j+k] * ( sig[m*j+k]-255.*pow(sig[m*j+k],2)+6050.*pow(sig[m*j+k],3)-46620.*pow(sig[m*j+k],4)+166824.*pow(sig[m*j+k],5)-317520.*pow(sig[m*j+k],6)+332640.*pow(sig[m*j+k],7)-181440.*pow(sig[m*j+k],8)+40320.*pow(sig[m*j+k],9) ));
 				}
 				break;
 		    }
 		}
 	}
+
+#ifdef WINDOWS_MSVC
+    delete[] sig;
+    delete[] zint;
+#endif
+
 	return;
 };
 
 // Parent n-dimensional basis function class: **********************************************************************
 nBasisFunc::nBasisFunc(double* x0in, int x0Dim0, double* xf, int xfDim0, int* nCin, int ncDim0, int ncDim1, int min, double z0in, double zfin){
 
 	// Initialize internal variables based on user givens
@@ -952,19 +953,30 @@
 	memcpy(nC,nCin,ncDim0*ncDim1*sizeof(int));
 
 	c = new double[dim];
 	for (int k=0; k<dim; k++)
 		c[k] = (zf-z0)/(xf[k]-x0[k]);
 
 	// Calculate the number of basis functions
-	int vec[dim];
 	numBasisFunc = 0; numBasisFuncFull = 0;
+
+#ifdef WINDOWS_MSVC
+	int* vec = new int[dim];
+#else
+	int vec[dim];
+#endif
+
 	NumBasisFunc(dim-1, &vec[0], numBasisFunc, false);
 	NumBasisFunc(dim-1, &vec[0], numBasisFuncFull, true);
 
+#ifdef WINDOWS_MSVC
+	delete[] vec;
+#endif
+
+
 	// Track this instance of BasisFunc 
 	BasisFuncContainer.push_back(this);
 	identifier = nIdentifier;
 	nIdentifier++;
 
 	// Create a PyCapsule with xla function for XLA compilation
 	xlaCapsule = GetXlaCapsule();
@@ -1033,16 +1045,27 @@
 			T[j+k*m*n] = dark[j]*dMult;
 	}
 
 	for (k=0;k<n*numBasis;k++)
 		F[k] = 1.;
 
 	int count = 0;
+
+#ifdef WINDOWS_MSVC
+	int* vec = new int[dim];
+#else
 	int vec[dim];
-	RecurseBasis(dim-1, &vec[0], count, full, n, numBasis, &T[0], F);
+#endif
+
+	RecurseBasis(dim-1, vec, count, full, n, numBasis, &T[0], F);
+
+#ifdef WINDOWS_MSVC
+	delete[] vec;
+#endif
+
 	delete[] dark; delete[] T; delete[] z;
 };
 
 void nBasisFunc::NumBasisFunc(int dimCurr, int* vec, int &count, const bool full){
 	int k;
 	if (dimCurr > 0){
 		for (k=0;k<m;k++){
```

### Comparing `tfc-1.0.5/src/tfc/utils/BF/BF.h` & `tfc-1.0.6/src/tfc/utils/BF/BF.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#define _USE_MATH_DEFINES // Needed by Windows
 #include <iostream>
 #include <vector>
 #include <math.h>
 #include <float.h>
 #include <Python.h>
 #ifdef HAS_CUDA
 	#include <cuda.h>
```

### Comparing `tfc-1.0.5/src/tfc/utils/BF/BF.i` & `tfc-1.0.6/src/tfc/utils/BF/BF.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/BF/BF.py` & `tfc-1.0.6/src/tfc/utils/BF/BF.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/BF/BF_Py.py` & `tfc-1.0.6/src/tfc/utils/BF/BF_Py.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/BF/numpy.i` & `tfc-1.0.6/src/tfc/utils/BF/numpy.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/CeSolver.py` & `tfc-1.0.6/src/tfc/utils/CeSolver.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/Html.py` & `tfc-1.0.6/src/tfc/utils/Html.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/Latex.py` & `tfc-1.0.6/src/tfc/utils/Latex.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/MakePlot.py` & `tfc-1.0.6/src/tfc/utils/MakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/MayaviMakePlot.py` & `tfc-1.0.6/src/tfc/utils/MayaviMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/PlotlyMakePlot.py` & `tfc-1.0.6/src/tfc/utils/PlotlyMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/TFCUtils.py` & `tfc-1.0.6/src/tfc/utils/TFCUtils.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc/utils/types.py` & `tfc-1.0.6/src/tfc/utils/types.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.5/src/tfc.egg-info/PKG-INFO` & `tfc-1.0.6/src/tfc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Education
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Theory of Functional Connections (TFC)
 **A functional interpolation framework with applications in solving differential equations.**
 
@@ -80,15 +81,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.5},
+    version = {1.0.6},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.5/src/tfc.egg-info/SOURCES.txt` & `tfc-1.0.6/src/tfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

