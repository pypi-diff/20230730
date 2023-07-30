# Comparing `tmp/matan-0.1.5.3.tar.gz` & `tmp/matan-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matan-0.1.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "matan-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `matan-0.1.5.3.tar` & `matan-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,42 @@
--rw-r--r--   0        0        0     4562 2023-07-30 19:32:06.631919 matan-0.1.5.3/README.md
--rw-r--r--   0        0        0     4220 2023-06-27 14:13:41.650051 matan-0.1.5.3/matan/MatAn.egg-info/PKG-INFO
--rw-r--r--   0        0        0      348 2023-06-27 14:13:41.650051 matan-0.1.5.3/matan/MatAn.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-06-27 14:13:41.650051 matan-0.1.5.3/matan/MatAn.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       17 2023-06-27 14:13:41.650051 matan-0.1.5.3/matan/MatAn.egg-info/requires.txt
--rw-r--r--   0        0        0        1 2023-06-27 14:13:41.650051 matan-0.1.5.3/matan/MatAn.egg-info/top_level.txt
--rw-r--r--   0        0        0       87 2023-07-30 19:23:35.919927 matan-0.1.5.3/matan/__init__.py
--rw-r--r--   0        0        0      168 2023-07-30 19:23:35.919927 matan-0.1.5.3/matan/_misc.py
--rw-r--r--   0        0        0      300 2023-07-30 19:23:35.919927 matan-0.1.5.3/matan/fem/tensile/__init__.py
--rw-r--r--   0        0        0     5191 2023-07-30 19:23:35.919927 matan-0.1.5.3/matan/files.py
--rw-r--r--   0        0        0     4257 2023-06-27 14:37:51.319665 matan-0.1.5.3/matan/matan.egg-info/PKG-INFO
--rw-r--r--   0        0        0      348 2023-06-27 14:37:51.323665 matan-0.1.5.3/matan/matan.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-06-27 14:37:51.319665 matan-0.1.5.3/matan/matan.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       17 2023-06-27 14:37:51.319665 matan-0.1.5.3/matan/matan.egg-info/requires.txt
--rw-r--r--   0        0        0        9 2023-06-27 14:37:51.319665 matan-0.1.5.3/matan/matan.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2023-06-28 16:39:25.070676 matan-0.1.5.3/matan/polymers/__init__.py
--rw-r--r--   0        0        0      812 2023-07-30 19:23:35.923927 matan-0.1.5.3/matan/polymers/charpy/__init__.py
--rw-r--r--   0        0        0     2616 2023-07-30 19:23:35.923927 matan-0.1.5.3/matan/polymers/tensile/ISO527/__init__.py
--rw-r--r--   0        0        0    12062 2023-07-30 19:23:35.923927 matan-0.1.5.3/matan/polymers/tensile/__init__.py
--rw-r--r--   0        0        0       28 2023-07-30 19:23:35.923927 matan-0.1.5.3/matan/polymers/tensile/misc.py
--rw-r--r--   0        0        0     7894 2023-07-30 19:23:35.923927 matan-0.1.5.3/matan/sample.py
--rw-r--r--   0        0        0      362 2023-07-30 19:42:30.979910 matan-0.1.5.3/pyproject.toml
--rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 matan-0.1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     3651 2023-07-29 12:04:42.656318 matan-0.1.6/.gitignore
+-rw-r--r--   0        0        0      798 2023-07-29 12:04:42.656318 matan-0.1.6/.woodpecker.yml
+-rw-r--r--   0        0        0    34670 2023-07-29 12:04:42.656318 matan-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4846 2023-07-29 12:04:42.656318 matan-0.1.6/MANIFEST.org
+-rw-r--r--   0        0        0       99 2023-07-29 12:04:42.656318 matan-0.1.6/Makefile
+-rw-r--r--   0        0        0     3385 2023-07-29 12:04:42.660318 matan-0.1.6/README.md
+-rw-r--r--   0        0        0      638 2023-07-29 12:04:42.660318 matan-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-29 12:04:42.660318 matan-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0     3164 2023-07-29 12:04:42.660318 matan-0.1.6/docs/phinx-autogen
+-rw-r--r--   0        0        0   285099 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     1229 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0       95 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/api.rst
+-rw-r--r--   0        0        0     1462 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/conf.py
+-rw-r--r--   0        0        0      103 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/examples.rst
+-rw-r--r--   0        0        0      267 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/future.rst
+-rw-r--r--   0        0        0       73 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/generated/matan.files.rst
+-rw-r--r--   0        0        0      192 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/generated/matan.rst
+-rw-r--r--   0        0        0      400 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/generated/matan.sample.rst
+-rw-r--r--   0        0        0     2104 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/index.rst
+-rw-r--r--   0        0        0      408 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/matan.rst
+-rw-r--r--   0        0        0       52 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/modules.rst
+-rw-r--r--   0        0        0     2561 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2023-07-29 12:04:42.732318 matan-0.1.6/docs/source/whats_next.rst
+-rw-r--r--   0        0        0      388 2023-07-29 12:04:42.660318 matan-0.1.6/examples/composition.py
+-rw-r--r--   0        0        0       40 2023-07-29 12:04:42.660318 matan-0.1.6/examples/find_files.py
+-rw-r--r--   0        0        0       87 2023-07-29 12:04:42.660318 matan-0.1.6/examples/imp.py
+-rw-r--r--   0        0        0     2147 2023-07-29 12:04:42.660318 matan-0.1.6/examples/tensile_test.py
+-rw-r--r--   0        0        0      192 2023-07-29 12:04:42.660318 matan-0.1.6/is-uploaded.sh
+-rw-r--r--   0        0        0       87 2023-07-29 12:04:42.660318 matan-0.1.6/matan/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-29 12:04:42.660318 matan-0.1.6/matan/_misc.py
+-rw-r--r--   0        0        0      300 2023-07-29 12:04:42.660318 matan-0.1.6/matan/fem/tensile/__init__.py
+-rw-r--r--   0        0        0     5191 2023-07-29 12:04:42.660318 matan-0.1.6/matan/files.py
+-rw-r--r--   0        0        0        0 2023-07-29 12:04:42.732318 matan-0.1.6/matan/polymers/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-29 12:04:42.660318 matan-0.1.6/matan/polymers/charpy/__init__.py
+-rw-r--r--   0        0        0     2616 2023-07-29 12:04:42.660318 matan-0.1.6/matan/polymers/tensile/ISO527/__init__.py
+-rw-r--r--   0        0        0    12062 2023-07-29 12:04:42.664318 matan-0.1.6/matan/polymers/tensile/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 12:04:42.664318 matan-0.1.6/matan/polymers/tensile/misc.py
+-rw-r--r--   0        0        0     7894 2023-07-29 12:04:42.664318 matan-0.1.6/matan/sample.py
+-rw-r--r--   0        0        0      340 2023-07-29 12:04:42.664318 matan-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      941 2023-07-29 12:04:42.664318 matan-0.1.6/setup.cfg
+-rw-r--r--   0        0        0      160 2023-07-29 12:04:42.664318 matan-0.1.6/tests/sample_project/__main__.py
+-rw-r--r--   0        0        0      224 1970-01-01 00:00:00.000000 matan-0.1.6/PKG-INFO
```

### Comparing `matan-0.1.5.3/README.md` & `matan-0.1.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,44 @@
-**This package is still under development. Be aware of often updates, versions
-below 0.2 are pre-alpha, and can be changed without any warning, or without any
-backward compatibility! **
+**This package is still under development. Be aware of often updates!**
 # MaTan
-Shortcut comes from **Mat**erial **An**analysis - ultimately is should contains
-modules allowing user to calculate metals and polymers
-properties from tensile, HDT (polymers) and DSC tests, as well as the
-others. There are few similar packages in PyPI, but none of them I found good to
-me, so I wrote new one.
-
-For now it includes:
-- ISO:527-1 (polymers tensile test)
-
-In near future all the findings functions will be finished, so you can describe
-your sample with thermal modifications, comments and compositions as parameter,
-as well as CI/CD. This should be 0.1.6 version.
-
-Nextly the FEM module which will allow to create materials models will be
-implemented.  In the beginning, the first feature will allow to create tensile
-FEM material models, with calculation of mean/worst real values stress-strain
-curve, and extracting from this curve the needed parameters, like plastic
-strains, Young's Modulus etc. At this point export to .csv file will be
-implemented. This should be 0.1.7 version Next phase will be export these models
-directly to .xml file as ANSYS is using such type, and this seems to be a FEM
-tool I will be working with. ANSYS already have tool to import from .csv file,
-so it will just make whole process faster. Later I will try to make export to
-FreeCAD's/CalculiX material models. This will be 0.1.8.  Finally from that
-version to 0.2 we will try to make whole package robust, and stable as possible.
-
 
+Shortcut comes from **Mat**erial **An**analysis - ultimately is should contains modules allowing
+user to calculate metals and polymers properties from tensile, HDT (polymers) and DSC tests, as well
+as the others. There are few similar  packages in PyPI, but none of them I found good to me, so I
+wrote new one. 
 
+For now it includes:
+- ISO:527-1 (polymers analysis)
 
 _**[Documentation](https://matan.codeberg.page)**_
 
 # Abstract
 
-Nowadays, Python is one of the most popular programming languages, even in
-non-informatics fields like mechanical engineering, due to its simplicity, and
-computer analysis solvers using FEM methods are part of almost all components,
-albeit access to material data is sometimes hard due to inadequate data in the
-datasheets, problems with calculations, inconsistent information, etc. To
-overcome this problem, the Python package was created, which allows to calculate
-the stress, strains, tensile modulus, and other properties from force and
-elongation data from a machine. For now, it includes only polymer tests
-according to the ISO-527-1 standard, but in the future, other standards should
-be included.
-
-Moreover, the package would need a graphical user interface, which could make it
-even simpler to use and, more importantly, allow users to upload their obtained
-results into OpenAccess databases and export plastic strains, tensile modulus,
-and other properties needed to perform FEM and other numerical analysis. That
-could make FEM methods even more accessible, which would lead to a decrease in
-the use of unnecessary materials and, due to this, less CO2 pollution.
+Nowadays, Python is one of the most popular programming languages, even in non-informatics fields
+like mechanical engineering, due to its simplicity, and computer analysis solvers using FEM methods
+are part of almost all components, albeit access to material data is sometimes hard due to
+inadequate data in the datasheets, problems with calculations, inconsistent information, etc. To
+overcome this problem, the Python package was created, which allows to calculate the stress,
+strains, tensile modulus, and other properties from force and elongation data from a machine. For
+now, it includes only polymer tests according to the ISO-527-1 standard, but in the future, other
+standards should be included.
+
+Moreover, the package would need a graphical user interface, which could make it even simpler to use
+and, more importantly, allow users to upload their obtained results into OpenAccess databases and
+export plastic strains, tensile modulus, and other properties needed to perform FEM and other
+numerical analysis. That could make FEM methods even more accessible, which would lead to a decrease
+in the use of unnecessary materials and, due to this, less CO2 pollution.
 
 
 # How to use it?
 
 Just simply put elongation and force arrays into sample.
 
-Be aware that sometimes csv files can have diffrent extension depends on machine
-manufacturer. To be sure just check it using simples notepad, or try to read it
-by pandas.
+Be aware that sometimes csv files can have diffrent extension depends on machine manufacturer. To be
+sure just check it using simples notepad, or try to read it by pandas.
 
 ```python
 import matan as mt
 import pandas as pd
 
 path_to_your_CSV = r"path/to/your/CSV"
```

### Comparing `matan-0.1.5.3/matan/files.py` & `matan-0.1.6/matan/files.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.3/matan/polymers/charpy/__init__.py` & `matan-0.1.6/matan/polymers/charpy/__init__.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.3/matan/polymers/tensile/ISO527/__init__.py` & `matan-0.1.6/matan/polymers/tensile/ISO527/__init__.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.3/matan/polymers/tensile/__init__.py` & `matan-0.1.6/matan/polymers/tensile/__init__.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.3/matan/sample.py` & `matan-0.1.6/matan/sample.py`

 * *Files identical despite different names*

