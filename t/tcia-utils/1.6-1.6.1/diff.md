# Comparing `tmp/tcia_utils-1.6.tar.gz` & `tmp/tcia_utils-1.6.1.tar.gz`

## Comparing `tcia_utils-1.6.tar` & `tcia_utils-1.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    71818 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6/LICENSE
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.6/README.md
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tcia_utils-1.6/pyproject.toml
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 tcia_utils-1.6/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    71871 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/PKG-INFO
```

### Comparing `tcia_utils-1.6/src/tcia_utils/datacite.py` & `tcia_utils-1.6.1/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6/src/tcia_utils/nbia.py` & `tcia_utils-1.6.1/src/tcia_utils/nbia.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 from enum import Enum
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import pydicom
 import numpy as np
 from ipywidgets import interact
-import tkinter, pydicom_seg, rt_utils 
-from tkinter import filedialog
 
 class StopExecution(Exception):
     def _render_traceback_(self):
         pass
 
 _log = logging.getLogger(__name__)
 logging.basicConfig(
@@ -1632,14 +1630,15 @@
 ####### viewSeriesSEG function
 # Visualizes a Series (scan) you've downloaded in the notebook
 # Adds an overlay from the SEG series
 # Requires a path parameter for the reference series
 # Requires the file path for the annotative series
 # Not recommended to be used as a standalone function
 def viewSeriesSEG(seriesPath = "", SEGPath = ""):
+    import pydicom_seg 
     """
     Visualizes a Series (scan) you've downloaded in the notebook
     Adds an overlay from the SEG series
     Requires a path parameter for the reference series
     Requires the file path for the annotative series
     Not recommended to be used as a standalone function
     """
@@ -1708,14 +1707,15 @@
 ####### viewSeriesRT function
 # Visualizes a Series (scan) you've downloaded in the notebook
 # Adds an overlay from the RTSTRUCT series
 # Requires a path parameter for the reference series
 # Requires the file path for the annotative series
 # Not recommended to be used as a standalone function
 def viewSeriesRT(seriesPath = "", RTPath = ""):
+    import rt_utils 
     """
     Visualizes a Series (scan) you've downloaded in the notebook
     Adds an overlay from the RTSTRUCT series
     Requires a path parameter for the reference series
     Requires the file path for the annotative series
     Not recommended to be used as a standalone function
     """
@@ -1782,14 +1782,16 @@
     Requires EITHER a seriesUid or path parameter for the reference series
     Requires EITHER a annotationUid or path parameter for the segmentation series
     Opens a file browser for users to choose folder/file if the required parameters are not specified
     Leave seriesUid and/or annotationUid empty if you want to provide a custom path
     The function assumes "tciaDownload/<UID>/" as path if seriesUid and/or annotationUid is provided since this is where downloadSeries() saves data.
     Note that non-axial images might not be correctly displayed.
     """
+    import tkinter, pydicom_seg, rt_utils 
+    from tkinter import filedialog
     def seriesInvalid(uid, path):
         if uid:
             link = f"https://nbia.cancerimagingarchive.net/viewer/?series={uid}"
         else:
             link = "https://nbia.cancerimagingarchive.net/viewer/?series=YOUR_SERIES_UID"
         _log.error(
             f"Cannot find a valid DICOM series at: {path}\n"
```

### Comparing `tcia_utils-1.6/src/tcia_utils/pathdb.py` & `tcia_utils-1.6.1/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6/.gitignore` & `tcia_utils-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6/LICENSE` & `tcia_utils-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6/README.md` & `tcia_utils-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6/pyproject.toml` & `tcia_utils-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.6"
+version = "1.6.1"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.6/PKG-INFO` & `tcia_utils-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.6
+Version: 1.6.1
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

