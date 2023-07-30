# Comparing `tmp/neuroimager-0.0.7.tar.gz` & `tmp/neuroimager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimager-0.0.7.tar", last modified: Sat Jul  1 04:32:47 2023, max compression
+gzip compressed data, was "neuroimager-0.0.8.tar", last modified: Sun Jul 30 13:45:59 2023, max compression
```

## Comparing `neuroimager-0.0.7.tar` & `neuroimager-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.119986 neuroimager-0.0.7/
--rw-r--r--   0 nij       (1000) nij       (1000)    35149 2023-06-05 13:40:29.000000 neuroimager-0.0.7/LICENSE
--rw-r--r--   0 nij       (1000) nij       (1000)     2458 2023-07-01 04:32:47.119986 neuroimager-0.0.7/PKG-INFO
--rw-r--r--   0 nij       (1000) nij       (1000)     1832 2023-07-01 04:30:46.000000 neuroimager-0.0.7/README.md
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.117986 neuroimager-0.0.7/neuroimager/
--rw-r--r--   0 nij       (1000) nij       (1000)      149 2023-06-05 13:02:03.000000 neuroimager-0.0.7/neuroimager/__init__.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.117986 neuroimager-0.0.7/neuroimager/pipes/
--rw-r--r--   0 nij       (1000) nij       (1000)        0 2023-06-05 13:00:13.000000 neuroimager-0.0.7/neuroimager/pipes/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     3188 2023-06-10 05:11:31.000000 neuroimager-0.0.7/neuroimager/pipes/bipartite.py
--rw-r--r--   0 nij       (1000) nij       (1000)     1400 2023-06-13 06:38:35.000000 neuroimager-0.0.7/neuroimager/pipes/brainage.py
--rw-r--r--   0 nij       (1000) nij       (1000)     7097 2023-06-08 17:19:10.000000 neuroimager-0.0.7/neuroimager/pipes/cca.py
--rw-r--r--   0 nij       (1000) nij       (1000)    15711 2023-06-13 06:49:44.000000 neuroimager-0.0.7/neuroimager/pipes/explore.py
--rw-r--r--   0 nij       (1000) nij       (1000)    39138 2023-07-01 03:39:37.000000 neuroimager-0.0.7/neuroimager/pipes/hmm.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.118986 neuroimager-0.0.7/neuroimager/plotting/
--rw-r--r--   0 nij       (1000) nij       (1000)      338 2023-06-30 10:01:02.000000 neuroimager-0.0.7/neuroimager/plotting/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     4034 2023-06-30 09:51:04.000000 neuroimager-0.0.7/neuroimager/plotting/plot.py
--rw-r--r--   0 nij       (1000) nij       (1000)      786 2023-06-30 13:44:07.000000 neuroimager-0.0.7/neuroimager/plotting/styler.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.118986 neuroimager-0.0.7/neuroimager/stats/
--rw-r--r--   0 nij       (1000) nij       (1000)      159 2023-06-13 07:01:27.000000 neuroimager-0.0.7/neuroimager/stats/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     5558 2023-06-09 10:11:35.000000 neuroimager-0.0.7/neuroimager/stats/correlation.py
--rw-r--r--   0 nij       (1000) nij       (1000)     1715 2023-06-13 06:59:17.000000 neuroimager-0.0.7/neuroimager/stats/perm_ttest.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.118986 neuroimager-0.0.7/neuroimager/utils/
--rw-r--r--   0 nij       (1000) nij       (1000)      560 2023-06-09 06:04:17.000000 neuroimager-0.0.7/neuroimager/utils/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     9900 2023-06-09 14:51:06.000000 neuroimager-0.0.7/neuroimager/utils/atlas.py
--rw-r--r--   0 nij       (1000) nij       (1000)     6704 2023-06-09 10:11:35.000000 neuroimager-0.0.7/neuroimager/utils/fc.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.117986 neuroimager-0.0.7/neuroimager.egg-info/
--rw-r--r--   0 nij       (1000) nij       (1000)     2458 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/PKG-INFO
--rw-r--r--   0 nij       (1000) nij       (1000)      663 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/SOURCES.txt
--rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/dependency_links.txt
--rw-r--r--   0 nij       (1000) nij       (1000)      110 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/requires.txt
--rw-r--r--   0 nij       (1000) nij       (1000)       12 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/top_level.txt
--rw-r--r--   0 nij       (1000) nij       (1000)       38 2023-07-01 04:32:47.119986 neuroimager-0.0.7/setup.cfg
--rw-r--r--   0 nij       (1000) nij       (1000)     1241 2023-07-01 04:32:00.000000 neuroimager-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.181077 neuroimager-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 13:45:44.000000 neuroimager-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 13:45:59.177077 neuroimager-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-30 13:45:44.000000 neuroimager-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.169077 neuroimager-0.0.8/neuroimager/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.173077 neuroimager-0.0.8/neuroimager/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/brainage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/task_fmri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.173077 neuroimager-0.0.8/neuroimager/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/plotting/styler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.177077 neuroimager-0.0.8/neuroimager/preproc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/preproc/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/preproc/prep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.177077 neuroimager-0.0.8/neuroimager/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/stats/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/stats/perm_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.177077 neuroimager-0.0.8/neuroimager/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/rbload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.169077 neuroimager-0.0.8/neuroimager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 13:45:59.181077 neuroimager-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-30 13:45:44.000000 neuroimager-0.0.8/setup.py
```

### Comparing `neuroimager-0.0.7/LICENSE` & `neuroimager-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/pipes/bipartite.py` & `neuroimager-0.0.8/neuroimager/pipes/graph.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/pipes/cca.py` & `neuroimager-0.0.8/neuroimager/pipes/cca.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/pipes/explore.py` & `neuroimager-0.0.8/neuroimager/pipes/explore.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/pipes/hmm.py` & `neuroimager-0.0.8/neuroimager/pipes/hmm.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/stats/correlation.py` & `neuroimager-0.0.8/neuroimager/stats/correlation.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/stats/perm_ttest.py` & `neuroimager-0.0.8/neuroimager/stats/perm_ttest.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.7/neuroimager/utils/__init__.py` & `neuroimager-0.0.8/neuroimager/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 from neuroimager.utils.atlas import (
     split_schafer_names,
     combine_atlases,
     combine_probabilistic_atlases,
     filter_rois,
+    resample_masks,
 )
 from neuroimager.utils.fc import (
     flatten_lower_triangular,
     unflatten_lower_triangular,
     filter_fcs,
     extract_bipartite_matrix,
     average_nodes,
 )
 
+from neuroimager.utils.ml import (
+    evaluate_continuous,
+    evaluate_binary,
+)
+
+from neuroimager.utils.rbload import (
+    rbload_csv,
+    rbload_imgs,
+)
+
 __all__ = [
     "split_schafer_names",
     "combine_atlases",
     "combine_probabilistic_atlases",
+    "resample_masks",
     "filter_rois",
     "flatten_lower_triangular",
     "unflatten_lower_triangular",
     "filter_fcs",
     "extract_bipartite_matrix",
     "average_nodes",
+    "evaluate_continuous",
+    "evaluate_binary",
+    "rbload_csv",
+    "rbload_imgs",
 ]
```

### Comparing `neuroimager-0.0.7/neuroimager/utils/atlas.py` & `neuroimager-0.0.8/neuroimager/utils/atlas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,84 @@
 import re
 import pandas as pd
 import numpy as np
 import nibabel as nib
-from nilearn.image import index_img
+from nilearn.image import index_img, load_img, resample_to_img
+from neuroimager.utils.rbload import rbload_imgs
+
+
+def symmetrize_image_data(image_data, round: int or False = False):
+    mid_point = image_data.shape[0] // 2
+    left_hemisphere = image_data[:mid_point, :, :]
+    right_hemisphere = image_data[mid_point:, :, :]
+    right_hemisphere_flipped = np.flip(right_hemisphere, axis=0)
+    symmetrized_data = (left_hemisphere + right_hemisphere_flipped) / 2
+    full_symmetrized_data = np.concatenate(
+        (symmetrized_data, np.flip(symmetrized_data, axis=0)), axis=0
+    )
+
+    return full_symmetrized_data
+
+
+def symmetrize_image_nifti(input_file, output_paths: str or list = None):
+    """
+    Symmetrize a NIfTI image across the mid-sagittal plane.
+    Returns a NIfTI image object or a list of NIfTI image objects.
+    The images are saved if output_paths is specified.
+
+    """
+    nifti_images = rbload_imgs(input_file)
+    save = False
+    if isinstance(output_paths, str):
+        output_paths = [output_paths]
+        save = True
+    elif isinstance(output_paths, list):
+        save = True
+    if len(output_paths) != len(nifti_images):
+        raise ValueError(
+            "The number of output paths must match the number of input images."
+        )
+    symmetrized_nifti_images = []
+    for i, nifti_image in enumerate(nifti_images):
+        image_data = nifti_image.get_fdata()
+        symmetrized_data = symmetrize_image_data(image_data)
+        symmetrized_nifti_image = nib.Nifti1Image(
+            symmetrized_data, nifti_image.affine, nifti_image.header
+        )
+        if save:
+            nib.save(symmetrized_nifti_image, output_paths[i])
+        if len(nifti_images) == 1:
+            return symmetrized_nifti_image
+        symmetrized_nifti_images.append(symmetrized_nifti_image)
+
+    return symmetrized_nifti_images
+
+
+def resample_masks(source_img_name, target_img_name, interpolation="continuous"):
+    target_img = load_img(target_img_name)
+    source_img = load_img(source_img_name)
+    res_img = resample_to_img(
+        source_img,
+        target_img,
+        interpolation=interpolation,
+        copy=True,
+        order="F",
+        clip=False,
+        fill_value=0,
+        force_resample=False,
+    )
+
+    if interpolation != "nearest":
+        data = res_img.get_fdata()
+        data_rounded = data.round().astype(int)
+        res_img_rounded = nib.Nifti1Image(data_rounded, res_img.affine, res_img.header)
+
+        return res_img_rounded
+    else:
+        return res_img
 
 
 # TODO: Add support for nilean atlas objects
 def combine_atlases(atlases: list, output_path: str, return_combined_atlas=True):
     """
     This function combines multiple atlas files (in NIfTI format) into a single atlas file.
     Prioritize atlases in the atlas_paths list by placing them at the front.
```

### Comparing `neuroimager-0.0.7/neuroimager/utils/fc.py` & `neuroimager-0.0.8/neuroimager/utils/fc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,65 @@
 import numpy as np
 import math
+from sklearn.base import BaseEstimator, TransformerMixin
 
 
+# Part one: sklearn estimator types
+# These are the wrappers for the functions in part two
+class FCFilter(BaseEstimator, TransformerMixin):
+    def __init__(self, network_labels, excludes=None, includes=None):
+        self.network_labels = network_labels
+        self.excludes = excludes
+        self.includes = includes
+
+    def fit(self, X, y=None):
+        return self
+
+    def transform(self, X, y=None):
+        return filter_fcs(X, self.network_labels, self.excludes, self.includes)
+
+
+class BipartiteMatrixExtractor(BaseEstimator, TransformerMixin):
+    def __init__(self, network_labels, bp1_labels, bp2_labels):
+        self.network_labels = network_labels
+        self.bp1_labels = bp1_labels
+        self.bp2_labels = bp2_labels
+
+    def fit(self, X, y=None):
+        return self
+
+    def transform(self, X, y=None):
+        return extract_bipartite_matrix(
+            X, self.network_labels, self.bp1_labels, self.bp2_labels
+        )
+
+
+class AverageNodesTransformer(BaseEstimator, TransformerMixin):
+    def __init__(self, labels):
+        self.labels = labels
+
+    def fit(self, X, y=None):
+        return self
+
+    def transform(self, X, y=None):
+        return average_nodes(X, self.labels)
+
+
+class FlattenLowerTriangular(BaseEstimator, TransformerMixin):
+    def __init__(self):
+        pass
+
+    def fit(self, X, y=None):
+        return self
+
+    def transform(self, X, y=None):
+        return flatten_lower_triangular(X)
+
+
+# Part two: functions
 def filter_fcs(
     fcs: np.array, network_labels: list, excludes: list = None, includes: list = None
 ):
     """Filter FC matrix based on network labels
     :param fcs: A numpy matrix shaped (n_subjects, n_nodes, n_nodes) representing the functional connectivity data.
     :param network_labels: A list containing the network labels for each node.
     :param excludes: A list of network labels to exclude from the filtered FC matrix. Default is None.
```

### Comparing `neuroimager-0.0.7/neuroimager.egg-info/SOURCES.txt` & `neuroimager-0.0.8/neuroimager.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,27 @@
 neuroimager/__init__.py
 neuroimager.egg-info/PKG-INFO
 neuroimager.egg-info/SOURCES.txt
 neuroimager.egg-info/dependency_links.txt
 neuroimager.egg-info/requires.txt
 neuroimager.egg-info/top_level.txt
 neuroimager/pipes/__init__.py
-neuroimager/pipes/bipartite.py
 neuroimager/pipes/brainage.py
 neuroimager/pipes/cca.py
 neuroimager/pipes/explore.py
+neuroimager/pipes/graph.py
 neuroimager/pipes/hmm.py
+neuroimager/pipes/task_fmri.py
 neuroimager/plotting/__init__.py
 neuroimager/plotting/plot.py
 neuroimager/plotting/styler.py
+neuroimager/preproc/__init__.py
+neuroimager/preproc/decompose.py
+neuroimager/preproc/prep.py
 neuroimager/stats/__init__.py
 neuroimager/stats/correlation.py
 neuroimager/stats/perm_ttest.py
 neuroimager/utils/__init__.py
 neuroimager/utils/atlas.py
-neuroimager/utils/fc.py
+neuroimager/utils/fc.py
+neuroimager/utils/ml.py
+neuroimager/utils/rbload.py
```

### Comparing `neuroimager-0.0.7/setup.py` & `neuroimager-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 # Read the contents of your README file
 with open(os.path.join(current_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="neuroimager",
-    version="0.0.7",
+    version="0.0.8",
     description="A collection of utilities used for MRI data analysis",
     author="Wetiqe",
     author_email="jzni132134@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Wetiqe/neuroimager",
     packages=find_packages(),
@@ -25,14 +25,15 @@
         "seaborn",
         "sklearn",
         "nilearn",
         "networkx",
         "munkres",
         "scikit-network",
     ],
+    extras_require={"torch": ["torch>=1.0.0"]},
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

