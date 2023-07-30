# Comparing `tmp/PyOnlineSVR-0.0.3.tar.gz` & `tmp/PyOnlineSVR-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyOnlineSVR-0.0.3.tar", last modified: Thu Jun 24 09:38:37 2021, max compression
+gzip compressed data, was "dist/PyOnlineSVR-0.0.4.tar", last modified: Sun Jul 30 20:25:25 2023, max compression
```

## Comparing `PyOnlineSVR-0.0.3.tar` & `PyOnlineSVR-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6060 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6060 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4027 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/pyonlinesvr/
--rw-r--r--   0 runner    (1001) docker     (121)      876 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     7424 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/CrossValidation.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10503 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/File.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5418 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/Forget.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/Kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    16149 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/OnlineSVR.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9244 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/OnlineSVR.i
--rw-r--r--   0 runner    (1001) docker     (121)    10939 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/Show.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6405 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/Stabilize.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9032 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/Train.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    19870 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/Variations.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/
--rw-r--r--   0 runner    (1001) docker     (121)    17870 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     9713 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/OnlineSVR.h
--rw-r--r--   0 runner    (1001) docker     (121)    16102 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/Vector.h
--rw-r--r--   0 runner    (1001) docker     (121)    14569 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/osvr.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/pyonlinesvr/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6070 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 09:38:37.000000 PyOnlineSVR-0.0.3/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/tests/lib/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2021-06-24 09:38:08.000000 PyOnlineSVR-0.0.3/tests/test_osvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/pyonlinesvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/CrossValidation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/File.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/Forget.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/Kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16149 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/OnlineSVR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/OnlineSVR.i
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/Show.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/Stabilize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/Train.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19870 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/Variations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/OnlineSVR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/Vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/osvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/pyonlinesvr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:25:25.000000 PyOnlineSVR-0.0.4/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/tests/lib/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-30 20:24:56.000000 PyOnlineSVR-0.0.4/tests/test_osvr.py
```

### Comparing `PyOnlineSVR-0.0.3/LICENSE` & `PyOnlineSVR-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/PyOnlineSVR.egg-info/SOURCES.txt` & `PyOnlineSVR-0.0.4/PyOnlineSVR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/README.md` & `PyOnlineSVR-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PyOnlineSVR
 
 [![pipeline status](https://github.com/CodeLionX/pyonlinesvr/actions/workflows/conda-python-test.yml/badge.svg)](https://github.com/CodeLionX/pyonlinesvr/actions/workflows/conda-python-test.yml)
 ![coverage report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/CodeLionX/6762bee806477c52e079f21d2f252688/raw/pyonlinesvr__heads_main.json)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![release info](https://img.shields.io/badge/Release-0.0.2-blue)](https://gitlab.hpi.de/akita/pyonlinesvr/-/releases/v0.0.2)
+[![PyPI package](https://badge.fury.io/py/PyOnlineSVR.svg)](https://badge.fury.io/py/PyOnlineSVR)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![python version 3.7|3.8|3.9](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 
 Python-Wrapper for Francesco Parrella's OnlineSVR [[PAR2007]](#PAR2007) C++ implementation with [scikit-learn](https://sklearn.org/)-compatible interfaces.
 You can find more information about the OnlineSVR [here](http://onlinesvr.altervista.org/) and the original source code [here](https://github.com/fp2556/onlinesvr/tree/master/c%2B%2B).
 
 ## Installation
@@ -61,15 +61,15 @@
 ```bash
 conda install -n pyonlinesvr numpy scipy scikit-learn
 ```
 
 #### Get the source code
 
 ```bash
-git clone https://gitlab.hpi.de/akita/pyonlinesvr
+git clone https://github.com/CodeLionX/pyonlinesvr.git
 cd pyonlinesvr
 ```
 
 #### Install PyOnlineSVR
 
 ```bash
 python setup.py install
```

### Comparing `PyOnlineSVR-0.0.3/dependencies.py` & `PyOnlineSVR-0.0.4/dependencies.py`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/__init__.py` & `PyOnlineSVR-0.0.4/pyonlinesvr/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/_version.py` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,9 +12,7 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PyOnlineSVR. If not, see
 # <https://www.gnu.org/licenses/gpl-3.0.html>.
-
-__version__: str = "0.0.3"
```

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/CrossValidation.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/CrossValidation.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/File.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/File.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/Forget.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/Forget.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/Kernel.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/Kernel.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/OnlineSVR.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/OnlineSVR.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/OnlineSVR.i` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/OnlineSVR.i`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/Show.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/Show.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/Stabilize.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/Stabilize.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/Train.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/Train.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/Variations.cpp` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/Variations.cpp`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/__init__.py` & `PyOnlineSVR-0.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/compat.py` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/compat.py`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/Matrix.h` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/Matrix.h`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/OnlineSVR.h` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/OnlineSVR.h`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/lib/include/Vector.h` & `PyOnlineSVR-0.0.4/pyonlinesvr/lib/include/Vector.h`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/pyonlinesvr/osvr.py` & `PyOnlineSVR-0.0.4/pyonlinesvr/osvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PyOnlineSVR. If not, see
 # <https://www.gnu.org/licenses/gpl-3.0.html>.
-
 from typing import Any, ContextManager, Optional
+
 import numpy as np
 import scipy as sp
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.utils import check_X_y
 from sklearn.utils.validation import check_array, column_or_1d, check_is_fitted
-from pyonlinesvr.lib.onlinesvr import OnlineSVR as LibOnlineSVR
+
 from pyonlinesvr.lib.compat import (
     double_matrix_to_np,
     double_vector_to_np,
     int_vector_to_np,
     kernel_map,
     kernels,
     np_to_double_matrix,
     np_to_double_vector,
     np_to_int_vector,
 )
+from pyonlinesvr.lib.onlinesvr import OnlineSVR as LibOnlineSVR
 
 
 class wrap_output(ContextManager):
     def __init__(self, verbose: int = 0, context: str = "") -> None:
         self.verbose = bool(verbose)
         self.context = context
 
@@ -311,16 +312,16 @@
 
         Notes
         ------
         If X and y are not C-ordered and contiguous arrays of np.float64, X and/or y
         may be copied.
         """
         check_is_fitted(self, ["_libosvr_", "n_features_in_"])
-        X = np.array(X)
-        if len(X.shape) == 1 and X.dtype == np.int64:
+        X = np.asarray(X)
+        if len(X.shape) == 1 and np.issubdtype(X.dtype, np.integer):
             return self._forget_indices(X)
         else:
             return self._forget_values(X)
 
     @property
     def support_(self) -> np.ndarray:
         """Indices of support vectors"""
@@ -404,29 +405,33 @@
         with wrap_output(self.verbose, "Forgetting indices"):
             self._libosvr_.Forget(X)
 
     def __getstate__(self):
         dd = super().__getstate__()
         if "_libosvr_" in dd:
             import tempfile
-            import os
+            from pathlib import Path
 
-            _, filename = tempfile.mkstemp(text=True)
-            self._libosvr_.SaveOnlineSVR(filename)
-            with open(filename, "r") as fp:
-                dd["_libosvr_"] = fp.readlines()
-            os.remove(filename)
+            dd = dd.copy()
+            with tempfile.TemporaryDirectory() as tmp:
+                path = Path(tmp).resolve()
+                path /= "osvr-dump.txt"
+                self._libosvr_.SaveOnlineSVR(str(path))
+                with path.open("r") as fp:
+                    dd["_libosvr_"] = fp.readlines()
         return dd
 
     def __setstate__(self, state):
         if "_libosvr_" in state:
             import tempfile
-            import os
+            from pathlib import Path
 
-            with tempfile.NamedTemporaryFile(mode="w", delete=False) as fp:
-                fp.writelines(state["_libosvr_"])
-                filename = fp.name
-            libosvr = LibOnlineSVR()
-            libosvr.LoadOnlineSVR(filename)
-            state["_libosvr_"] = libosvr
-            os.remove(filename)
+            state = state.copy()
+            with tempfile.TemporaryDirectory() as tmp:
+                path = Path(tmp).resolve()
+                path /= "osvr-load.txt"
+                with path.open("w") as fp:
+                    fp.writelines(state["_libosvr_"])
+                libosvr = LibOnlineSVR()
+                libosvr.LoadOnlineSVR(str(path))
+                state["_libosvr_"] = libosvr
         return super().__setstate__(state)
```

### Comparing `PyOnlineSVR-0.0.3/setup.cfg` & `PyOnlineSVR-0.0.4/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [metadata]
-description-file = README.md
-license_file = LICENSE
+description_file = README.md
+license_files = 
+	LICENSE
 
 [aliases]
 test = pytest
 
 [tool:pytest]
-addopts = --cov=pyonlinesvr
-testpaths = 
-	tests
 
 [coverage:run]
 branch = False
 parallel = True
 omit = 
 	pyonlinesvr/__version__.py
 	pyonlinesvr/lib/onlinesvr.py
```

### Comparing `PyOnlineSVR-0.0.3/setup.py` & `PyOnlineSVR-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,38 +46,14 @@
 if sys.version_info < python_min_version:
     print(
         f"You are using Python {platform.python_version()}. "
         f"Python >={python_min_version_str} is required."
     )
     sys.exit(-1)
 
-
-# Check if swig is available
-def which(program: str) -> bool:
-    """Adapted from https://stackoverflow.com/a/377028"""
-    import os
-
-    def is_exe(fpath):
-        return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
-
-    fpath, _ = os.path.split(program)
-    if fpath:
-        return is_exe(program)
-    else:
-        for path in os.environ["PATH"].split(os.pathsep):
-            exe_file = os.path.join(path, program)
-            if is_exe(exe_file):
-                return True
-    return False
-
-
-if not which("swig"):
-    raise Exception("Building PyOnlineSVR requires swig <http://swig.org/>!")
-
-
 # populate vars
 cwd = Path(os.path.dirname(__file__)).absolute()
 lib_path = Path("pyonlinesvr") / "lib"
 readme = (cwd / "README.md").read_text(encoding="UTF-8")
 install_requires = packages_for_tag["install"]
 extras_require = {
     "test": [dep for dep in packages_for_tag["test"] if dep not in install_requires],
@@ -197,10 +173,11 @@
         "Operating System :: POSIX :: Linux",
         # "Operating System :: Microsoft :: Windows",
         # "Operating System :: MacOS",
         "Programming Language :: C++",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Typing :: Typed",
     ],
 )
```

### Comparing `PyOnlineSVR-0.0.3/tests/__init__.py` & `PyOnlineSVR-0.0.4/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/tests/lib/__init__.py` & `PyOnlineSVR-0.0.4/pyonlinesvr/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PyOnlineSVR. If not, see
 # <https://www.gnu.org/licenses/gpl-3.0.html>.
+
+__version__: str = "0.0.4"
```

### Comparing `PyOnlineSVR-0.0.3/tests/lib/test_compat.py` & `PyOnlineSVR-0.0.4/tests/lib/test_compat.py`

 * *Files identical despite different names*

### Comparing `PyOnlineSVR-0.0.3/tests/test_osvr.py` & `PyOnlineSVR-0.0.4/tests/test_osvr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,34 @@
-import pytest
+#                         PyOnlineSVR
+#               Copyright 2023 - Sebastian Schmidl
+#
+# This file is part of PyOnlineSVR.
+#
+# PyOnlineSVR is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# PyOnlineSVR is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with PyOnlineSVR. If not, see
+# <https://www.gnu.org/licenses/gpl-3.0.html>.
+
+from pathlib import Path
+
 import numpy as np
+import pytest
 from joblib import load, dump
-from pathlib import Path
-from sklearn.utils.estimator_checks import check_estimator
 from sklearn.exceptions import NotFittedError
+from sklearn.utils.estimator_checks import check_estimator
+
 from pyonlinesvr import OnlineSVR
 
 a = np.sin(np.arange(0, 8, 0.1))
 X = a.reshape(-1, 1)[:-1]
 y = np.roll(a, -1)[:-1]
 del a
 
@@ -127,15 +148,15 @@
     y_hat = rgr.predict(X[-5:])
     np.testing.assert_array_almost_equal(y[-5:], y_hat, decimal=2)
 
 
 def test_forget_indices():
     rgr = OnlineSVR(epsilon=1e-3, verbose=0)
     rgr.fit(X, y)
-    rgr.forget(range(X.shape[0] - 5, X.shape[0]))
+    rgr.forget(np.arange(X.shape[0] - 5, X.shape[0], dtype=np.int_))
     y_hat = rgr.predict(X[-5:])
     np.testing.assert_array_almost_equal(y[-5:], y_hat, decimal=2)
 
 
 def test_pickle_predict(tmp_path: Path) -> None:
     filename = tmp_path / "svr.pkl"
     rgr = OnlineSVR(epsilon=1e-3, verbose=0)
```

