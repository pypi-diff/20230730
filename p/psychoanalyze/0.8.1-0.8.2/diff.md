# Comparing `tmp/psychoanalyze-0.8.1.tar.gz` & `tmp/psychoanalyze-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.8.1.tar", max compression
+gzip compressed data, was "psychoanalyze-0.8.2.tar", max compression
```

## Comparing `psychoanalyze-0.8.1.tar` & `psychoanalyze-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.1/LICENSE
--rw-r--r--   0        0        0     1274 2023-07-26 11:57:00.456909 psychoanalyze-0.8.1/README.md
--rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.1/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.1/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.1/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.1/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.1/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.1/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.1/psychoanalyze/dashboard/__init__.py
--rw-r--r--   0        0        0    12468 2023-07-28 02:10:21.380217 psychoanalyze-0.8.1/psychoanalyze/dashboard/app.py
--rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
--rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
--rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/logo_bgwhite.png
--rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
--rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/styles.css
--rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.1/psychoanalyze/dashboard/components.py
--rw-r--r--   0        0        0     9143 2023-07-28 09:06:06.449424 psychoanalyze-0.8.1/psychoanalyze/dashboard/layout.py
--rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.1/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     6031 2023-07-28 00:17:06.312544 psychoanalyze-0.8.1/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     6787 2023-07-28 00:17:06.312544 psychoanalyze-0.8.1/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.1/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.1/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.1/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5225 2023-07-20 09:41:06.475106 psychoanalyze-0.8.1/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.1/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.1/psychoanalyze/main.py
--rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.1/psychoanalyze/params.py
--rw-r--r--   0        0        0     2116 2023-07-21 02:42:52.381174 psychoanalyze-0.8.1/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.1/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     3249 2023-07-29 22:04:12.392670 psychoanalyze-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 psychoanalyze-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1274 2023-07-26 11:57:00.456909 psychoanalyze-0.8.2/README.md
+-rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.2/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.2/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.2/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.2/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.2/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.2/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.2/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0    12468 2023-07-28 02:10:21.380217 psychoanalyze-0.8.2/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
+-rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
+-rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/logo_bgwhite.png
+-rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
+-rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/styles.css
+-rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.2/psychoanalyze/dashboard/components.py
+-rw-r--r--   0        0        0     9143 2023-07-28 09:06:06.449424 psychoanalyze-0.8.2/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.2/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     6031 2023-07-28 00:17:06.312544 psychoanalyze-0.8.2/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     6787 2023-07-28 00:17:06.312544 psychoanalyze-0.8.2/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.2/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.2/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.2/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5225 2023-07-20 09:41:06.475106 psychoanalyze-0.8.2/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.2/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.2/psychoanalyze/main.py
+-rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.2/psychoanalyze/params.py
+-rw-r--r--   0        0        0     2116 2023-07-21 02:42:52.381174 psychoanalyze-0.8.2/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.2/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     3255 2023-07-29 23:59:27.293309 psychoanalyze-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 psychoanalyze-0.8.2/PKG-INFO
```

### Comparing `psychoanalyze-0.8.1/LICENSE` & `psychoanalyze-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/README.md` & `psychoanalyze-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/__init__.py` & `psychoanalyze-0.8.2/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.8.2/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.8.2/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.8.2/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.8.2/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.8.2/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/__init__.py` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/app.py` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/PsychoAnalyze.svg` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/PsychoAnalyze.svg`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/favicon.ico` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/logo_bgwhite.png` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/logo_bgwhite.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/logo_transparent_100x100.png` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/logo_transparent_100x100.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/assets/styles.css` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/components.py` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/components.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/dashboard/layout.py` & `psychoanalyze-0.8.2/psychoanalyze/dashboard/layout.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/__init__.py` & `psychoanalyze-0.8.2/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/blocks.py` & `psychoanalyze-0.8.2/psychoanalyze/data/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/points.py` & `psychoanalyze-0.8.2/psychoanalyze/data/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/sessions.py` & `psychoanalyze-0.8.2/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.8.2/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/subjects.py` & `psychoanalyze-0.8.2/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/trials.py` & `psychoanalyze-0.8.2/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/data/types.py` & `psychoanalyze-0.8.2/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/main.py` & `psychoanalyze-0.8.2/psychoanalyze/main.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/params.py` & `psychoanalyze-0.8.2/psychoanalyze/params.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/plot.py` & `psychoanalyze-0.8.2/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/psychoanalyze/sigmoids.py` & `psychoanalyze-0.8.2/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.1/pyproject.toml` & `psychoanalyze-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.8.1"
+version = "0.8.2"
 description = "Interactive analysis and simulation of psychophysical data."
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://psychoanalyze.io"
 repository = "https://github.com/psychoanalyze/psychoanalyze"
 documentation = "https://docs.psychoanalyze.io"
@@ -12,23 +12,23 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Framework :: Dash",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 urls = { JupyterHub = "https://nb.psychoanalyze.io" }
 
 [tool.poetry.dependencies]
-python = "3.11.4"
+python = ">=3.9.0,<3.12.0"
 pandas = "^2.0.2"
 scipy = "^1.10.1"
 numpy = "^1.25.0"
 dash-bootstrap-components = "^1.4.1"
 statsmodels = "^0.14.0"
 dash-daq = "^0.5.0"
 dash = "^2.11.1"
```

### Comparing `psychoanalyze-0.8.1/PKG-INFO` & `psychoanalyze-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.8.1
+Version: 0.8.2
 Summary: Interactive analysis and simulation of psychophysical data.
 Home-page: https://psychoanalyze.io
 License: GPL-3.0-or-later
 Keywords: psychophysics,neuroscience,psychology
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
-Requires-Python: ==3.11.4
+Requires-Python: >=3.9.0,<3.12.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Dash
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: docs
 Requires-Dist: bambi (>=0.11.0,<0.12.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
```

