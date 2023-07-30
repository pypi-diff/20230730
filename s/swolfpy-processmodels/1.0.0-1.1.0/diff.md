# Comparing `tmp/swolfpy_processmodels-1.0.0.tar.gz` & `tmp/swolfpy_processmodels-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swolfpy_processmodels-1.0.0.tar", last modified: Sun Jun  4 18:01:52 2023, max compression
+gzip compressed data, was "C:\Users\msa75\Documents\Repos\github\swolfpy-processmodels\dist\.tmp-8053tyy3\swolfpy_processmodels-1.1.0.tar", last modified: Sun Jul 30 16:16:47 2023, max compression
```

## Comparing `swolfpy_processmodels-1.0.0.tar` & `swolfpy_processmodels-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.603304 swolfpy_processmodels-1.0.0/
--rw-rw-rw-   0        0        0      748 2023-06-04 17:34:44.000000 swolfpy_processmodels-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     1674 2022-11-25 05:39:51.000000 swolfpy_processmodels-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      768 2023-06-04 17:34:44.000000 swolfpy_processmodels-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2022-11-25 05:03:08.000000 swolfpy_processmodels-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      273 2023-02-26 03:37:23.000000 swolfpy_processmodels-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7498 2023-06-04 18:01:52.602305 swolfpy_processmodels-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5365 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/README.rst
--rw-rw-rw-   0        0        0    10501 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      124 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 18:01:52.604305 swolfpy_processmodels-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.529304 swolfpy_processmodels-1.0.0/swolfpy_processmodels/
--rw-rw-rw-   0        0        0    24138 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD.py
--rw-rw-rw-   0        0        0    26334 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD_subprocess.py
--rw-rw-rw-   0        0        0     8517 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/AnF.py
--rw-rw-rw-   0        0        0    38421 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/COM_Col.py
--rw-rw-rw-   0        0        0    14792 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Common_subprocess.py
--rw-rw-rw-   0        0        0    14479 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Comp.py
--rw-rw-rw-   0        0        0    14643 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Comp_subprocess.py
--rw-rw-rw-   0        0        0     3388 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Distance.py
--rw-rw-rw-   0        0        0    26389 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/GC.py
--rw-rw-rw-   0        0        0     6748 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC.py
--rw-rw-rw-   0        0        0     3998 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC_subprocess.py
--rw-rw-rw-   0        0        0    44003 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/LF.py
--rw-rw-rw-   0        0        0    37798 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/MF_Col.py
--rw-rw-rw-   0        0        0    30289 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/MRF_subprocess.py
--rw-rw-rw-   0        0        0      858 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModel.py
--rw-rw-rw-   0        0        0     4335 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModelsMetaData.py
--rw-rw-rw-   0        0        0    10116 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/RDF.py
--rw-rw-rw-   0        0        0     1848 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Reproc.py
--rw-rw-rw-   0        0        0    42618 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/SF_Col.py
--rw-rw-rw-   0        0        0    14816 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/SS_MRF.py
--rw-rw-rw-   0        0        0     5203 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS.py
--rw-rw-rw-   0        0        0     5036 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS_subprocess.py
--rw-rw-rw-   0        0        0    17518 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/WTE.py
--rw-rw-rw-   0        0        0      744 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.571304 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/
--rw-rw-rw-   0        0        0     7498 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1188 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.597305 swolfpy_processmodels-1.0.0/tests/
--rw-rw-rw-   0        0        0       79 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4801 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/tests/test_processmodels.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/
+-rw-rw-rw-   0        0        0      748 2023-06-20 02:22:04.000000 swolfpy_processmodels-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1674 2023-06-20 02:22:04.000000 swolfpy_processmodels-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      841 2023-07-30 15:33:03.000000 swolfpy_processmodels-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    18431 2023-06-20 02:22:04.000000 swolfpy_processmodels-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0      273 2023-07-30 16:15:29.000000 swolfpy_processmodels-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7568 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-07-30 15:33:18.000000 swolfpy_processmodels-1.1.0/README.rst
+-rw-rw-rw-   0        0        0    10475 2023-07-30 16:15:13.000000 swolfpy_processmodels-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      124 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/
+-rw-rw-rw-   0        0        0    24138 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/AD.py
+-rw-rw-rw-   0        0        0    26334 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/AD_subprocess.py
+-rw-rw-rw-   0        0        0     8517 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/AnF.py
+-rw-rw-rw-   0        0        0    38421 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/COM_Col.py
+-rw-rw-rw-   0        0        0    14792 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/Common_subprocess.py
+-rw-rw-rw-   0        0        0    14479 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/Comp.py
+-rw-rw-rw-   0        0        0    14643 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/Comp_subprocess.py
+-rw-rw-rw-   0        0        0     3388 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/Distance.py
+-rw-rw-rw-   0        0        0    26389 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/GC.py
+-rw-rw-rw-   0        0        0     6748 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/HC.py
+-rw-rw-rw-   0        0        0     3998 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/HC_subprocess.py
+-rw-rw-rw-   0        0        0    44003 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/LF.py
+-rw-rw-rw-   0        0        0    37798 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/MF_Col.py
+-rw-rw-rw-   0        0        0    30289 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/MRF_subprocess.py
+-rw-rw-rw-   0        0        0      858 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/ProcessModel.py
+-rw-rw-rw-   0        0        0     4335 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/ProcessModelsMetaData.py
+-rw-rw-rw-   0        0        0    10116 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/RDF.py
+-rw-rw-rw-   0        0        0     1848 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/Reproc.py
+-rw-rw-rw-   0        0        0    42618 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/SF_Col.py
+-rw-rw-rw-   0        0        0    14816 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/SS_MRF.py
+-rw-rw-rw-   0        0        0     5203 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/TS.py
+-rw-rw-rw-   0        0        0     5036 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/TS_subprocess.py
+-rw-rw-rw-   0        0        0    17518 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/WTE.py
+-rw-rw-rw-   0        0        0      744 2023-07-30 16:15:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/
+-rw-rw-rw-   0        0        0     7568 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 16:16:47.000000 swolfpy_processmodels-1.1.0/tests/
+-rw-rw-rw-   0        0        0       79 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4801 2023-06-20 02:22:05.000000 swolfpy_processmodels-1.1.0/tests/test_processmodels.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `swolfpy_processmodels-1.0.0/AUTHORS.rst` & `swolfpy_processmodels-1.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/CONTRIBUTING.rst` & `swolfpy_processmodels-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/HISTORY.rst` & `swolfpy_processmodels-1.1.0/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy_processmodels-1.0.0/LICENSE.md` & `swolfpy_processmodels-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/PKG-INFO` & `swolfpy_processmodels-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: swolfpy_processmodels
-Version: 1.0.0
+Version: 1.1.0
 Summary: Life-Cylce Process Models for swolfpy (swolfpy_processmodels).
 Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
 Project-URL: Homepage, https://swolfpy-project.github.io/
 Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-processmodels
 Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 .. General
 
 ==============================================================
@@ -139,15 +139,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10
+        conda create --name swolfpy python=3.9
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_processmodels in the environment::
 
@@ -163,14 +163,20 @@
 
 .. endInstallation
 
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy_processmodels-1.0.0/README.rst` & `swolfpy_processmodels-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10
+        conda create --name swolfpy python=3.9
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_processmodels in the environment::
```

### Comparing `swolfpy_processmodels-1.0.0/pyproject.toml` & `swolfpy_processmodels-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swolfpy_processmodels"
 dynamic = ["version", "readme", "dependencies"]
 description = "Life-Cylce Process Models for swolfpy (swolfpy_processmodels)."
 license = {text = "GNU GENERAL PUBLIC LICENSE V2"}
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 authors = [
   {name = "Mojtaba Sardarmehni", email = "msardar2@alumni.ncsu.edu"},
 ]
 maintainers = [
   {name = "Mojtaba Sardarmehni", email = "msardar2@alumni.ncsu.edu"},
 ]
 keywords = [
@@ -23,15 +23,15 @@
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
     'Natural Language :: English',
-    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.9',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     'Topic :: Scientific/Engineering :: Information Analysis',
     'Topic :: Scientific/Engineering :: Mathematics',
     'Topic :: Scientific/Engineering :: Visualization',
     'Natural Language :: English',
 ]
@@ -43,19 +43,18 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "swolfpy_processmodels.__version__"}
 readme = {file = ["README.rst", "HISTORY.rst"]}
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools]
-packages = ["swolfpy_processmodels"]
 include-package-data = true
 
-[tool.setuptools.package-data]
-package_input_data = []
+[tool.setuptools.packages.find]
+include = ["swolfpy_processmodels*"]
 
 [tool.black]
 line-length = 100
 preview = false
 
 [tool.isort]
 profile = "black"
```

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/AD.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD_subprocess.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/AD_subprocess.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/AnF.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/AnF.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/COM_Col.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/COM_Col.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Common_subprocess.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/Common_subprocess.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Comp.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/Comp.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Comp_subprocess.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/Comp_subprocess.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Distance.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/Distance.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/GC.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/GC.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/HC.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC_subprocess.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/HC_subprocess.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/LF.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/LF.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/MF_Col.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/MF_Col.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/MRF_subprocess.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/MRF_subprocess.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModel.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/ProcessModel.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModelsMetaData.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/ProcessModelsMetaData.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/RDF.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/RDF.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Reproc.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/Reproc.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/SF_Col.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/SF_Col.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/SS_MRF.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/SS_MRF.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/TS.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS_subprocess.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/TS_subprocess.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/WTE.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/WTE.py`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels/__init__.py` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     "TS",
     "HC",
     "GC",
     "RDF",
     "AnF",
 ]
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/PKG-INFO` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: swolfpy-processmodels
-Version: 1.0.0
+Version: 1.1.0
 Summary: Life-Cylce Process Models for swolfpy (swolfpy_processmodels).
 Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
 Project-URL: Homepage, https://swolfpy-project.github.io/
 Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-processmodels
 Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 .. General
 
 ==============================================================
@@ -139,15 +139,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10
+        conda create --name swolfpy python=3.9
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_processmodels in the environment::
 
@@ -163,14 +163,20 @@
 
 .. endInstallation
 
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/SOURCES.txt` & `swolfpy_processmodels-1.1.0/swolfpy_processmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-1.0.0/tests/test_processmodels.py` & `swolfpy_processmodels-1.1.0/tests/test_processmodels.py`

 * *Files identical despite different names*

