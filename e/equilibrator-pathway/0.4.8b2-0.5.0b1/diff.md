# Comparing `tmp/equilibrator-pathway-0.4.8b2.tar.gz` & `tmp/equilibrator-pathway-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-pathway-0.4.8b2.tar", last modified: Sun Jul  2 13:52:51 2023, max compression
+gzip compressed data, was "equilibrator-pathway-0.5.0b1.tar", last modified: Sun Jul 30 13:07:49 2023, max compression
```

## Comparing `equilibrator-pathway-0.4.8b2.tar` & `equilibrator-pathway-0.5.0b1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.281863 equilibrator-pathway-0.4.8b2/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4118 2023-07-02 13:52:51.281863 equilibrator-pathway-0.4.8b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2047 2023-07-02 13:52:51.282863 equilibrator-pathway-0.4.8b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.275863 equilibrator-pathway-0.4.8b2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.282863 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-02 13:52:51.282863 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/analysis_solution.py
--rwxrwxrwx   0 root         (0) root         (0)    23350 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/cost_function.py
--rw-rw-rw-   0 root         (0) root         (0)    12964 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10311 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_solution.py
--rw-rw-rw-   0 root         (0) root         (0)     6600 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdf_solution.py
--rwxrwxrwx   0 root         (0) root         (0)     7446 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdmc_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    10429 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/pathway.py
--rw-rw-rw-   0 root         (0) root         (0)     4343 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    10878 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/thermo_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4363 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:52:51.280863 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4118 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      832 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      323 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 13:52:51.000000 equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-02 13:52:40.000000 equilibrator-pathway-0.4.8b2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.531733 equilibrator-pathway-0.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-30 13:07:49.531733 equilibrator-pathway-0.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-07-30 13:07:49.532733 equilibrator-pathway-0.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.524733 equilibrator-pathway-0.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.532733 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 13:07:49.532733 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/analysis_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)    23350 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/cost_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    12964 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10311 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)     6600 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdf_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)     7446 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdmc_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    10429 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/pathway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4343 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10878 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/thermo_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.531733 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      294 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/versioneer.py
```

### Comparing `equilibrator-pathway-0.4.8b2/LICENSE` & `equilibrator-pathway-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/PKG-INFO` & `equilibrator-pathway-0.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.4.8b2
+Version: 0.5.0b1
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 equilibrator-pathway
```

### Comparing `equilibrator-pathway-0.4.8b2/README.md` & `equilibrator-pathway-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/setup.cfg` & `equilibrator-pathway-0.5.0b1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -30,23 +30,20 @@
 	pathway analysis
 	enzyme cost minimization
 	max-min driving force
 
 [options]
 zip_safe = True
 install_requires = 
-	pint~=0.21
-	pandas~=1.5
 	seaborn~=0.12
-	uncertainties~=3.1
 	osqp~=0.6
 	cvxpy~=1.3
 	sbtab~=1.0
-	equilibrator-api==0.4.8b1
-python_requires = >=3.8
+	equilibrator-api==0.5.0b1
+python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
@@ -56,18 +53,19 @@
 test = 
 	pytest
 	pytest-cov
 	pytest-raises
 development = 
 	jupyter~=1.0
 	jupyterlab~=4.0
-	black[jupyter]~=23.3
+	black[jupyter]~=23.7
+	flake8~=6.1
 	isort~=5.12
 	safety~=2.3
-	tox~=4.6
+	tox==3.28
 	twine~=4.0
 deployment = 
 	click
 	click-log
 	python-dateutil
 	requests
 	tqdm
```

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/__init__.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/analysis_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/analysis_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/cost_function.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/cost_function.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_model.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_model.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/ecm_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdf_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdf_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/mdmc_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdmc_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/pathway.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/pathway.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/simulator.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/simulator.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/thermo_models.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/thermo_models.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway/util.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/util.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/PKG-INFO` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.4.8b2
+Version: 0.5.0b1
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 equilibrator-pathway
```

### Comparing `equilibrator-pathway-0.4.8b2/src/equilibrator_pathway.egg-info/SOURCES.txt` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.8b2/versioneer.py` & `equilibrator-pathway-0.5.0b1/versioneer.py`

 * *Files identical despite different names*

