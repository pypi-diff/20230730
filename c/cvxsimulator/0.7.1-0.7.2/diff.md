# Comparing `tmp/cvxsimulator-0.7.1.tar.gz` & `tmp/cvxsimulator-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.7.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.7.2.tar", max compression
```

## Comparing `cvxsimulator-0.7.1.tar` & `cvxsimulator-0.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10790 2023-07-27 23:06:56.107031 cvxsimulator-0.7.1/LICENSE
--rw-r--r--   0        0        0     5741 2023-07-27 23:06:56.107031 cvxsimulator-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    15915 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1924 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1570 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/month.py
--rw-r--r--   0        0        0    24512 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      965 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      114 2023-07-27 23:06:56.179032 cvxsimulator-0.7.1/cvx/simulator/types.py
--rw-r--r--   0        0        0     1114 2023-07-27 23:07:32.539874 cvxsimulator-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 cvxsimulator-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-07-30 18:39:04.756541 cvxsimulator-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5739 2023-07-30 18:39:04.756541 cvxsimulator-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    15915 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1924 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1570 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/month.py
+-rw-r--r--   0        0        0    24512 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      965 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      114 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/types.py
+-rw-r--r--   0        0        0     1114 2023-07-30 18:39:38.584475 cvxsimulator-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6386 1970-01-01 00:00:00.000000 cvxsimulator-0.7.2/PKG-INFO
```

### Comparing `cvxsimulator-0.7.1/LICENSE` & `cvxsimulator-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.1/README.md` & `cvxsimulator-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org).
 Once you have installed poetry you can perform
 
 ```bash
-poetry install
+make install
 ```
 
 to replicate the virtual environment we have defined in pyproject.toml.
 
 ## Kernel
 
 We install [JupyterLab](https://jupyter.org) within your new virtual
```

### Comparing `cvxsimulator-0.7.1/cvx/simulator/builder.py` & `cvxsimulator-0.7.2/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.1/cvx/simulator/grid.py` & `cvxsimulator-0.7.2/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.1/cvx/simulator/month.py` & `cvxsimulator-0.7.2/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.7.2/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.1/cvx/simulator/trading_costs.py` & `cvxsimulator-0.7.2/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.1/pyproject.toml` & `cvxsimulator-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.7.1"
+version = "v0.7.2"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.7.1/PKG-INFO` & `cvxsimulator-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.7.1
+Version: 0.7.2
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -179,15 +179,15 @@
 
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org).
 Once you have installed poetry you can perform
 
 ```bash
-poetry install
+make install
 ```
 
 to replicate the virtual environment we have defined in pyproject.toml.
 
 ## Kernel
 
 We install [JupyterLab](https://jupyter.org) within your new virtual
```

