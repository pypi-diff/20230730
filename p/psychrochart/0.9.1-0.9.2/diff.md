# Comparing `tmp/psychrochart-0.9.1.tar.gz` & `tmp/psychrochart-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.9.1.tar", max compression
+gzip compressed data, was "psychrochart-0.9.2.tar", max compression
```

## Comparing `psychrochart-0.9.1.tar` & `psychrochart-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11655 2023-06-13 09:33:41.663741 psychrochart-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-13 09:33:41.663741 psychrochart-0.9.1/LICENSE
--rw-r--r--   0        0        0     7883 2023-06-13 09:33:41.663741 psychrochart-0.9.1/README.md
--rw-r--r--   0        0        0      739 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/__main__.py
--rw-r--r--   0        0        0    15292 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart.py
--rw-r--r--   0        0        0     2231 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_entities.py
--rw-r--r--   0        0        0     2157 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3097 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    15847 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chartdata.py
--rw-r--r--   0        0        0    18332 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/chartzones.py
--rw-r--r--   0        0        0        0 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     3298 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/annots.py
--rw-r--r--   0        0        0     1246 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/base.py
--rw-r--r--   0        0        0     8674 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/config.py
--rw-r--r--   0        0        0     3945 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5844 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     2079 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1924 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/models/validators.py
--rw-r--r--   0        0        0    16203 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     8135 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/process_logic.py
--rw-r--r--   0        0        0     4631 2023-06-13 09:33:41.675741 psychrochart-0.9.1/psychrochart/util.py
--rw-r--r--   0        0        0     2222 2023-06-13 09:33:41.675741 psychrochart-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     9212 1970-01-01 00:00:00.000000 psychrochart-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-07-30 10:32:10.109106 psychrochart-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-07-30 10:32:10.109106 psychrochart-0.9.2/LICENSE
+-rw-r--r--   0        0        0     7883 2023-07-30 10:32:10.109106 psychrochart-0.9.2/README.md
+-rw-r--r--   0        0        0      739 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/__main__.py
+-rw-r--r--   0        0        0    15292 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart.py
+-rw-r--r--   0        0        0     2231 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_entities.py
+-rw-r--r--   0        0        0     2157 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3097 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    15847 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chartdata.py
+-rw-r--r--   0        0        0    18332 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chartzones.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     3298 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/base.py
+-rw-r--r--   0        0        0     8674 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/config.py
+-rw-r--r--   0        0        0     3945 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5844 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     2079 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1924 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/validators.py
+-rw-r--r--   0        0        0    16203 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     8135 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     4631 2023-07-30 10:32:10.125106 psychrochart-0.9.2/psychrochart/util.py
+-rw-r--r--   0        0        0     2271 2023-07-30 10:32:10.125106 psychrochart-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     9266 1970-01-01 00:00:00.000000 psychrochart-0.9.2/PKG-INFO
```

### Comparing `psychrochart-0.9.1/CHANGELOG.md` & `psychrochart-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.2] - 🐛 Fix install with new pydantic v2 - 2023-07-30
+
+##### Changes
+
+- 🎨 lint: pre-commit autoupdate
+- 📦️ env: Bump patch version and fix deps with pydantic version < v2, and enabling new Python 3.12
+- 📝 Update CHANGELOG
+
 ## [0.9.1] - ✨ Add zone kind 'dbt-wmax' with vapour content limit - 2023-06-13
 
 ##### Changes
 
 - ✨ Add new kind of overlay **zone 'dbt-wmax'**, to define chart areas delimited between db-temps and absolute humidity values, solving #28
 - 🐛 Enable zones defined by 2 points (assume a rectangle defined by left-bottom/right-top coords)
 - 🐛 Fix logic for plot regeneration, to plot again if config changes _AFTER_ plotting the chart
```

### Comparing `psychrochart-0.9.1/LICENSE` & `psychrochart-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/README.md` & `psychrochart-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/__init__.py` & `psychrochart-0.9.2/psychrochart/__init__.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart.py` & `psychrochart-0.9.2/psychrochart/chart.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_entities.py` & `psychrochart-0.9.2/psychrochart/chart_entities.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.9.2/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.9.2/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.9.2/psychrochart/chart_styles/default_chart_config.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.9.2/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.9.2/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.9.2/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chartdata.py` & `psychrochart-0.9.2/psychrochart/chartdata.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/chartzones.py` & `psychrochart-0.9.2/psychrochart/chartzones.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/annots.py` & `psychrochart-0.9.2/psychrochart/models/annots.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/base.py` & `psychrochart-0.9.2/psychrochart/models/base.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/config.py` & `psychrochart-0.9.2/psychrochart/models/config.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/curves.py` & `psychrochart-0.9.2/psychrochart/models/curves.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/parsers.py` & `psychrochart-0.9.2/psychrochart/models/parsers.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/styles.py` & `psychrochart-0.9.2/psychrochart/models/styles.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/models/validators.py` & `psychrochart-0.9.2/psychrochart/models/validators.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/plot_logic.py` & `psychrochart-0.9.2/psychrochart/plot_logic.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/process_logic.py` & `psychrochart-0.9.2/psychrochart/process_logic.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/psychrochart/util.py` & `psychrochart-0.9.2/psychrochart/util.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.1/pyproject.toml` & `psychrochart-0.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.9.1"
+version = "0.9.2"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
@@ -60,24 +60,25 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 keywords=["psychrometrics", "moist", "humid air", "climate control", "matplotlib"]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<3.13"
 matplotlib = ">=3.7"
 scipy = ">=1.10"
 psychrolib = ">=2.5"
-pydantic = ">=1.8"
+pydantic = ">=1.8,<2"
 python-slugify = ">=8.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.10.0"
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `psychrochart-0.9.1/PKG-INFO` & `psychrochart-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: matplotlib (>=3.7)
 Requires-Dist: psychrolib (>=2.5)
-Requires-Dist: pydantic (>=1.8)
+Requires-Dist: pydantic (>=1.8,<2)
 Requires-Dist: python-slugify (>=8.0.1)
 Requires-Dist: scipy (>=1.10)
 Project-URL: Repository, https://github.com/azogue/psychrochart
 Description-Content-Type: text/markdown
 
 [![pre-commit.ci Status][pre-commit-ci-image]][pre-commit-ci-url]
 [![Build Status][build-image]][build-url]
```

