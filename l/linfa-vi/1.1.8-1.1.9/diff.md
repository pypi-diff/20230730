# Comparing `tmp/linfa_vi-1.1.8.tar.gz` & `tmp/linfa_vi-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.1.8.tar", last modified: Sun Jul 30 14:10:22 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.9.tar", last modified: Sun Jul 30 14:27:30 2023, max compression
```

## Comparing `linfa_vi-1.1.8.tar` & `linfa_vi-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:10:22.717772 linfa_vi-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-30 14:10:22.717772 linfa_vi-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:10:22.717772 linfa_vi-1.1.8/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:10:22.717772 linfa_vi-1.1.8/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-30 14:10:22.000000 linfa_vi-1.1.8/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-30 14:10:22.000000 linfa_vi-1.1.8/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:10:22.000000 linfa_vi-1.1.8/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 14:10:22.000000 linfa_vi-1.1.8/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 14:10:22.000000 linfa_vi-1.1.8/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:10:22.717772 linfa_vi-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:10:09.000000 linfa_vi-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:30.405714 linfa_vi-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-30 14:27:30.405714 linfa_vi-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:30.405714 linfa_vi-1.1.9/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/run_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:30.405714 linfa_vi-1.1.9/linfa/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/tests/test_linfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:30.405714 linfa_vi-1.1.9/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-30 14:27:30.000000 linfa_vi-1.1.9/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-30 14:27:30.000000 linfa_vi-1.1.9/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:27:30.000000 linfa_vi-1.1.9/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 14:27:30.000000 linfa_vi-1.1.9/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 14:27:30.000000 linfa_vi-1.1.9/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:27:30.405714 linfa_vi-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:27:17.000000 linfa_vi-1.1.9/setup.py
```

### Comparing `linfa_vi-1.1.8/LICENSE` & `linfa_vi-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/PKG-INFO` & `linfa_vi-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.1.8/README.md` & `linfa_vi-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/linfa/maf.py` & `linfa_vi-1.1.9/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/linfa/nofas.py` & `linfa_vi-1.1.9/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/linfa/plot_res.py` & `linfa_vi-1.1.9/linfa/plot_res.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/linfa/run_experiment.py` & `linfa_vi-1.1.9/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/linfa/transform.py` & `linfa_vi-1.1.9/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.8/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.9/linfa_vi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.1.8/pyproject.toml` & `linfa_vi-1.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.1.8"
+version = "1.1.9"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -22,14 +22,14 @@
     "numpy==1.19.5",
     "matplotlib==3.5.3",
     'tomli; python_version < "3.11"',    
 ]
 requires-python = ">=3.7"
 
 [tool.setuptools]
-packages = ["linfa"]
+packages = ["linfa", "linfa.tests"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/desResLab/LINFA"
```

