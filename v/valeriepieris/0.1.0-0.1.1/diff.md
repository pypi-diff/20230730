# Comparing `tmp/valeriepieris-0.1.0.tar.gz` & `tmp/valeriepieris-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valeriepieris-0.1.0.tar", last modified: Sun Jul 30 07:50:19 2023, max compression
+gzip compressed data, was "valeriepieris-0.1.1.tar", last modified: Sun Jul 30 08:10:30 2023, max compression
```

## Comparing `valeriepieris-0.1.0.tar` & `valeriepieris-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 07:50:19.911950 valeriepieris-0.1.0/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)    35149 2023-07-30 06:24:37.000000 valeriepieris-0.1.0/LICENSE.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       45 2023-07-30 07:20:50.000000 valeriepieris-0.1.0/MANIFEST.in
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     2120 2023-07-30 07:50:19.911950 valeriepieris-0.1.0/PKG-INFO
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      521 2023-07-30 07:35:31.000000 valeriepieris-0.1.0/README.md
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      609 2023-07-30 07:50:11.000000 valeriepieris-0.1.0/pyproject.toml
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:20:20.000000 valeriepieris-0.1.0/requirements.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     1509 2023-07-30 07:50:19.915950 valeriepieris-0.1.0/setup.cfg
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      414 2023-07-30 07:45:27.000000 valeriepieris-0.1.0/setup.py
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 07:50:19.911950 valeriepieris-0.1.0/src/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)  1696289 2023-07-30 07:45:29.000000 valeriepieris-0.1.0/src/valeriepieris.c
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 07:50:19.911950 valeriepieris-0.1.0/src/valeriepieris.egg-info/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     2120 2023-07-30 07:50:19.000000 valeriepieris-0.1.0/src/valeriepieris.egg-info/PKG-INFO
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      308 2023-07-30 07:50:19.000000 valeriepieris-0.1.0/src/valeriepieris.egg-info/SOURCES.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:50:19.000000 valeriepieris-0.1.0/src/valeriepieris.egg-info/dependency_links.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:45:30.000000 valeriepieris-0.1.0/src/valeriepieris.egg-info/not-zip-safe
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:50:19.000000 valeriepieris-0.1.0/src/valeriepieris.egg-info/top_level.txt
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)    35149 2023-07-30 06:24:37.000000 valeriepieris-0.1.1/LICENSE.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       45 2023-07-30 07:20:50.000000 valeriepieris-0.1.1/MANIFEST.in
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     2151 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/PKG-INFO
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      544 2023-07-30 08:08:11.000000 valeriepieris-0.1.1/README.md
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      609 2023-07-30 08:09:20.000000 valeriepieris-0.1.1/pyproject.toml
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:20:20.000000 valeriepieris-0.1.1/requirements.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     1509 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/setup.cfg
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      414 2023-07-30 07:45:27.000000 valeriepieris-0.1.1/setup.py
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 08:10:30.352798 valeriepieris-0.1.1/src/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)  1696289 2023-07-30 07:45:29.000000 valeriepieris-0.1.1/src/valeriepieris.c
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/src/valeriepieris.egg-info/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     2151 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/PKG-INFO
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      308 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/SOURCES.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/dependency_links.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:45:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/not-zip-safe
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/top_level.txt
```

### Comparing `valeriepieris-0.1.0/LICENSE.txt` & `valeriepieris-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `valeriepieris-0.1.0/PKG-INFO` & `valeriepieris-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valeriepieris
-Version: 0.1.0
+Version: 0.1.1
 Summary: Finding valeriepieris circles
 Home-page: https://github.com/rudyarthur/valeriepieris
 Author: Rudy Arthur
 Author-email: rudy.d.arthur@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Documentation, https://github.com/rudyarthur/valeriepieris
 Project-URL: Code, https://github.com/rudyarthur/valeriepieris
@@ -12,19 +12,20 @@
 Description: # valeriepieris
         Find valeriepieris circles.
         
         Expects 2d-numpy arrays from e.g. [SEDAC](https://sedac.ciesin.columbia.edu/data/set/gpw-v4-population-count-rev11/data-download)
         
         ```
         import numpy as np
-        input_data = np.loadtxt("../gpw_v4_population_count_rev11_{}_2pt5_min.asc".format(year), skiprows=6 )
+        input_data = np.loadtxt("gpw_v4_population_count_rev11_2020_1_deg.asc", skiprows=6 )
         input_data[ input_data < 0] = 0
         ```
         Then call
         ```
+        from valeriepieris import valeriepieris
         data_bounds = [ -90,90, -180,180 ]
         target_fracs = [0.25, 0.5, 1]
         rmin, smin, best_latlon, data, new_bounds  = valeriepieris(input_data,  data_bounds, target_fracs)		
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `valeriepieris-0.1.0/pyproject.toml` & `valeriepieris-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "valeriepieris"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Rudy Arthur", email="rudy.d.arthur@gmail.com" },
 ]
 description = "calculate valeriepieris circles"
 readme = "README.md"
 requires-python = ">=3.8"
 requires = ["setuptools", "wheel", "numpy >= 1.24", "Cython>=0.29.33"]
```

### Comparing `valeriepieris-0.1.0/setup.cfg` & `valeriepieris-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = valeriepieris
-version = 0.1.0
+version = 0.1.1
 description = Finding valeriepieris circles
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU GENERAL PUBLIC LICENSE Version 3
 author = Rudy Arthur
 author_email = rudy.d.arthur@gmail.com
 url = https://github.com/rudyarthur/valeriepieris
```

### Comparing `valeriepieris-0.1.0/src/valeriepieris.c` & `valeriepieris-0.1.1/src/valeriepieris.c`

 * *Files identical despite different names*

### Comparing `valeriepieris-0.1.0/src/valeriepieris.egg-info/PKG-INFO` & `valeriepieris-0.1.1/src/valeriepieris.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valeriepieris
-Version: 0.1.0
+Version: 0.1.1
 Summary: Finding valeriepieris circles
 Home-page: https://github.com/rudyarthur/valeriepieris
 Author: Rudy Arthur
 Author-email: rudy.d.arthur@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Documentation, https://github.com/rudyarthur/valeriepieris
 Project-URL: Code, https://github.com/rudyarthur/valeriepieris
@@ -12,19 +12,20 @@
 Description: # valeriepieris
         Find valeriepieris circles.
         
         Expects 2d-numpy arrays from e.g. [SEDAC](https://sedac.ciesin.columbia.edu/data/set/gpw-v4-population-count-rev11/data-download)
         
         ```
         import numpy as np
-        input_data = np.loadtxt("../gpw_v4_population_count_rev11_{}_2pt5_min.asc".format(year), skiprows=6 )
+        input_data = np.loadtxt("gpw_v4_population_count_rev11_2020_1_deg.asc", skiprows=6 )
         input_data[ input_data < 0] = 0
         ```
         Then call
         ```
+        from valeriepieris import valeriepieris
         data_bounds = [ -90,90, -180,180 ]
         target_fracs = [0.25, 0.5, 1]
         rmin, smin, best_latlon, data, new_bounds  = valeriepieris(input_data,  data_bounds, target_fracs)		
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

