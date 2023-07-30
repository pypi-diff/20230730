# Comparing `tmp/sen2nbar-2023.7.1.tar.gz` & `tmp/sen2nbar-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sen2nbar-2023.7.1.tar", last modified: Wed Jul 26 09:18:18 2023, max compression
+gzip compressed data, was "dist/sen2nbar-2023.7.2.tar", last modified: Sun Jul 30 07:12:29 2023, max compression
```

## Comparing `sen2nbar-2023.7.1.tar` & `sen2nbar-2023.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.7.1/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.7.1/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 09:18:18.868801 sen2nbar-2023.7.1/sen2nbar/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-07-26 09:08:17.000000 sen2nbar-2023.7.1/sen2nbar/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/axioms.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/brdf.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/c_factor.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/kernels.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4485 2023-07-26 08:46:17.000000 sen2nbar-2023.7.1/sen2nbar/metadata.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7546 2023-07-26 09:03:53.000000 sen2nbar-2023.7.1/sen2nbar/nbar.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/sen2nbar.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-07-26 09:08:23.000000 sen2nbar-2023.7.1/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-30 07:12:29.776848 sen2nbar-2023.7.2/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.7.2/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-30 07:12:29.773515 sen2nbar-2023.7.2/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.7.2/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-30 07:12:29.773515 sen2nbar-2023.7.2/sen2nbar/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-07-30 07:06:33.000000 sen2nbar-2023.7.2/sen2nbar/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/axioms.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/brdf.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/c_factor.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/kernels.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4602 2023-07-29 19:40:59.000000 sen2nbar-2023.7.2/sen2nbar/metadata.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     8292 2023-07-30 06:44:07.000000 sen2nbar-2023.7.2/sen2nbar/nbar.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-30 07:12:29.773515 sen2nbar-2023.7.2/sen2nbar.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-30 07:12:29.776848 sen2nbar-2023.7.2/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-07-30 07:06:48.000000 sen2nbar-2023.7.2/setup.py
```

### Comparing `sen2nbar-2023.7.1/LICENSE` & `sen2nbar-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/PKG-INFO` & `sen2nbar-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.1 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.2 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.7.1/README.md` & `sen2nbar-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/sen2nbar/axioms.py` & `sen2nbar-2023.7.2/sen2nbar/axioms.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/sen2nbar/brdf.py` & `sen2nbar-2023.7.2/sen2nbar/brdf.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/sen2nbar/c_factor.py` & `sen2nbar-2023.7.2/sen2nbar/c_factor.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/sen2nbar/kernels.py` & `sen2nbar-2023.7.2/sen2nbar/kernels.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/sen2nbar/metadata.py` & `sen2nbar-2023.7.2/sen2nbar/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,19 +99,22 @@
         )
 
     # x and y coordinates of the array to create
     y = np.arange(ULY, ULY - 5000 * 23, -5000) - 2500
     x = np.arange(ULX, ULX + 5000 * 23, 5000) + 2500
 
     # Create the array
-    da = xr.DataArray(
-        list(bands_dict.values()),
-        dims=["band", "angle", "y", "x"],
-        coords=dict(band=list(bands_dict.keys()), angle=ANGLES, x=x, y=y),
-    )
+    try:
+        da = xr.DataArray(
+            list(bands_dict.values()),
+            dims=["band", "angle", "y", "x"],
+            coords=dict(band=list(bands_dict.keys()), angle=ANGLES, x=x, y=y),
+        )
+    except ValueError:
+        raise ValueError("Not all bands include angles values.")
 
     # Add attributes
     da.attrs["epsg"] = Tile_Geocoding["HORIZONTAL_CS_CODE"]
 
     return da
```

### Comparing `sen2nbar-2023.7.1/sen2nbar/nbar.py` & `sen2nbar-2023.7.2/sen2nbar/nbar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
+import warnings
 from glob import glob
 
 import numpy as np
+import pandas as pd
 import planetary_computer as pc
 import pystac_client
 import rioxarray
 import xarray as xr
 from tqdm import tqdm
 
 from .axioms import bands
@@ -151,36 +153,51 @@
     # Get the items
     items = SEARCH.item_collection()
 
     # Sign the items if using PC
     if stac == "https://planetarycomputer.microsoft.com/api/stac/v1":
         items = pc.sign(items)
 
-    # Order items
-    items_ids = [item.id for item in items]
-    original_order = np.array(
-        [np.where(da.id.values == item) for item in items_ids]
-    ).ravel()
-    ordered_items = np.array(items)[original_order]
+    # Order items using pandas
+    df_items = pd.DataFrame(dict(id=[item.id for item in items], item=items)).set_index(
+        "id"
+    )
+    df_da_ids = pd.DataFrame(dict(id=da.id.values)).set_index("id")
+    ordered_df = df_da_ids.join(df_items)
+    ordered_items = ordered_df.item.values
 
     # Compute the c-factor per item and extract the processing baseline
     c_array = []
     processing_baseline = []
-    for item in tqdm(
-        ordered_items, disable=quiet, desc="Processing items", leave=False
+    exclude = []  # Save indices to exclude (this for not having angles for all bands)
+    for i, item in tqdm(
+        enumerate(ordered_items), disable=quiet, desc="Processing items", leave=False
     ):
-        c = c_factor_from_item(item, epsg)
-        c = c.interp(
-            y=da.y.values,
-            x=da.x.values,
-            method="linear",
-            kwargs={"fill_value": "extrapolate"},
-        )
-        c_array.append(c)
-        processing_baseline.append(item.properties["s2:processing_baseline"])
+        try:
+            c = c_factor_from_item(item, epsg)
+            c = c.interp(
+                y=da.y.values,
+                x=da.x.values,
+                method="linear",
+                kwargs={"fill_value": "extrapolate"},
+            )
+            c_array.append(c)
+            processing_baseline.append(item.properties["s2:processing_baseline"])
+        except ValueError:
+            # Append indices to exclude, then pass
+            exclude.append(i)
+            warnings.warn(
+                f"""Item {i} with datetime {item.properties['datetime']} omitted as it doesn't have angles for all bands."""
+            )
+            pass
+
+    # Exclude all timesteps were tile angles didn't exist for all bands
+    if len(exclude) > 0:
+        include = np.delete(np.arange(da.time.shape[0]), exclude)
+        da = da.isel(time=include)
 
     # Processing baseline as data array
     processing_baseline = xr.DataArray(
         [float(x) for x in processing_baseline],
         dims="time",
         coords=dict(time=da.time.values),
     )
```

### Comparing `sen2nbar-2023.7.1/sen2nbar/utils.py` & `sen2nbar-2023.7.2/sen2nbar/utils.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.1/sen2nbar.egg-info/PKG-INFO` & `sen2nbar-2023.7.2/sen2nbar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.1 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.2 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.7.1/setup.py` & `sen2nbar-2023.7.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="sen2nbar",
-    version="2023.7.1",
+    version="2023.7.2",
     url="https://github.com/ESDS-Leipzig/sen2nbar",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
     package_data={"sen2nbar": ["data/*.json"]},
     install_requires=[
-        "cubo>=2023.7.0",
+        "cubo>=2023.7.2",
         "pystac",
         "rasterio>=1.3.6",
         "requests",
         "rioxarray>=0.13.4",
         "scipy>=1.10.1",
         "tqdm",
         "xmltodict",
```

