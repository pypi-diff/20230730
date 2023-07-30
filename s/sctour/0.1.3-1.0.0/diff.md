# Comparing `tmp/sctour-0.1.3.tar.gz` & `tmp/sctour-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sctour-0.1.3.tar", last modified: Wed Aug 17 22:12:06 2022, max compression
+gzip compressed data, was "dist/sctour-1.0.0.tar", last modified: Sun Jul 30 20:47:04 2023, max compression
```

## Comparing `sctour-0.1.3.tar` & `sctour-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 ql312    (18375) ql312    (18387)        0 2022-08-17 22:12:06.000000 sctour-0.1.3/
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     1064 2022-02-15 22:21:40.000000 sctour-0.1.3/LICENSE
--rw-r--r--   0 ql312    (18375) ql312    (18387)       92 2022-04-17 19:21:31.000000 sctour-0.1.3/MANIFEST.in
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     2860 2022-08-17 22:12:06.000000 sctour-0.1.3/PKG-INFO
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     1924 2022-06-08 16:57:58.000000 sctour-0.1.3/README.md
-drwxrwxr-x   0 ql312    (18375) ql312    (18387)        0 2022-08-17 22:12:06.000000 sctour-0.1.3/sctour/
--rw-rw-r--   0 ql312    (18375) ql312    (18387)       75 2022-08-17 22:00:38.000000 sctour-0.1.3/sctour/__init__.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     2523 2022-02-15 23:36:51.000000 sctour-0.1.3/sctour/_utils.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     3712 2022-08-16 16:52:59.000000 sctour-0.1.3/sctour/data.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)      199 2022-08-09 11:26:17.000000 sctour-0.1.3/sctour/logger.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     6618 2022-08-16 15:52:46.000000 sctour-0.1.3/sctour/model.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     4016 2022-07-29 16:46:06.000000 sctour-0.1.3/sctour/module.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)    27508 2022-08-17 19:14:32.000000 sctour-0.1.3/sctour/train.py
--rw-rw-r--   0 ql312    (18375) ql312    (18387)    16344 2022-08-09 14:37:39.000000 sctour-0.1.3/sctour/vector_field.py
-drwxrwxr-x   0 ql312    (18375) ql312    (18387)        0 2022-08-17 22:12:06.000000 sctour-0.1.3/sctour.egg-info/
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     2860 2022-08-17 22:12:00.000000 sctour-0.1.3/sctour.egg-info/PKG-INFO
--rw-rw-r--   0 ql312    (18375) ql312    (18387)      327 2022-08-17 22:12:00.000000 sctour-0.1.3/sctour.egg-info/SOURCES.txt
--rw-rw-r--   0 ql312    (18375) ql312    (18387)        1 2022-08-17 22:12:00.000000 sctour-0.1.3/sctour.egg-info/dependency_links.txt
--rw-rw-r--   0 ql312    (18375) ql312    (18387)      139 2022-08-17 22:12:00.000000 sctour-0.1.3/sctour.egg-info/requires.txt
--rw-rw-r--   0 ql312    (18375) ql312    (18387)        7 2022-08-17 22:12:00.000000 sctour-0.1.3/sctour.egg-info/top_level.txt
--rw-rw-r--   0 ql312    (18375) ql312    (18387)       38 2022-08-17 22:12:06.000000 sctour-0.1.3/setup.cfg
--rw-rw-r--   0 ql312    (18375) ql312    (18387)     1101 2022-08-17 22:02:13.000000 sctour-0.1.3/setup.py
+drwxrwxr-x   0 ql312    (18375) ql312    (18387)        0 2023-07-30 20:47:04.000000 sctour-1.0.0/
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     1064 2022-02-15 22:21:40.000000 sctour-1.0.0/LICENSE
+-rw-r--r--   0 ql312    (18375) ql312    (18387)       92 2022-04-17 19:21:31.000000 sctour-1.0.0/MANIFEST.in
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     2692 2023-07-30 20:47:04.000000 sctour-1.0.0/PKG-INFO
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     1788 2023-06-30 10:13:32.000000 sctour-1.0.0/README.md
+drwxrwxr-x   0 ql312    (18375) ql312    (18387)        0 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour/
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)       97 2023-07-21 20:41:01.000000 sctour-1.0.0/sctour/__init__.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     2523 2022-02-15 23:36:51.000000 sctour-1.0.0/sctour/_utils.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     3712 2022-08-16 16:52:59.000000 sctour-1.0.0/sctour/data.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)      199 2022-08-09 11:26:17.000000 sctour-1.0.0/sctour/logger.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     6618 2022-08-16 15:52:46.000000 sctour-1.0.0/sctour/model.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     4016 2022-07-29 16:46:06.000000 sctour-1.0.0/sctour/module.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)    12284 2023-07-30 09:21:29.000000 sctour-1.0.0/sctour/predict.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)    21316 2023-07-30 09:30:25.000000 sctour-1.0.0/sctour/train.py
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)    17064 2023-07-30 14:44:14.000000 sctour-1.0.0/sctour/vector_field.py
+drwxrwxr-x   0 ql312    (18375) ql312    (18387)        0 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour.egg-info/
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     2692 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour.egg-info/PKG-INFO
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)      345 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour.egg-info/SOURCES.txt
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)        1 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour.egg-info/dependency_links.txt
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)      139 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour.egg-info/requires.txt
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)        7 2023-07-30 20:47:04.000000 sctour-1.0.0/sctour.egg-info/top_level.txt
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)       38 2023-07-30 20:47:04.000000 sctour-1.0.0/setup.cfg
+-rw-rw-r--   0 ql312    (18375) ql312    (18387)     1101 2023-07-24 21:55:16.000000 sctour-1.0.0/setup.py
```

### Comparing `sctour-0.1.3/LICENSE` & `sctour-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sctour-0.1.3/PKG-INFO` & `sctour-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 Metadata-Version: 2.1
 Name: sctour
-Version: 0.1.3
+Version: 1.0.0
 Summary: a deep learning architecture for robust inference and accurate prediction of cellular dynamics
 Home-page: https://github.com/LiQian-XC/sctour
 Author: Qian Li
 Author-email: liqian.picb@gmail.com
 License: UNKNOWN
 Description: 
-        # About scTour
+        # scTour
         
-        scTour is an innovative and comprehensive method for dissecting cellular dynamics by analysing datasets derived from single-cell genomics. It provides a unifying framework to depict the full picture of developmental processes from multiple angles including developmental pseudotime, vector field and latent space, and further generalises these functionalities to a multi-task architecture for within-dataset inference and cross-dataset prediction of cellular dynamics in a batch-insensitive manner.
+        <img src="https://github.com/LiQian-XC/sctour/blob/main/docs/source/_static/img/scTour_head_image.png" width="400px" align="left">
         
-        <p align="center"><img src="https://github.com/LiQian-XC/sctour/blob/ae9b45e69941bcabf3ad498dde781eb991168b83/docs/source/_static/img/scTour_head_image.png" width="700px" align="center"></p>
+        scTour is an innovative and comprehensive method for dissecting cellular dynamics by analysing datasets derived from single-cell genomics.
         
-        # Preprint
+        It provides a unifying framework to depict the full picture of developmental processes from multiple angles including the developmental pseudotime, vector field and latent space.
         
-        Consider citing this [paper](https://www.biorxiv.org/content/10.1101/2022.04.17.488600v1) if you use scTour in your analysis.
+        It further generalises these functionalities to a multi-task architecture for within-dataset inference and cross-dataset prediction of cellular dynamics in a batch-insensitive manner.  
+          
+        ## Key features
         
-        # scTour features
+        - cell pseudotime estimation with no need for specifying starting cells.
+        - transcriptomic vector field inference with no discrimination between spliced and unspliced mRNAs.
+        - latent space mapping by combining intrinsic transcriptomic structure with extrinsic pseudotime ordering.
+        - model-based prediction of pseudotime, vector field, and latent space for query cells/datasets/time intervals.
+        - insensitive to batch effects; robust to cell subsampling; scalable to large datasets.
         
-        - unsupervised estimates of cell pseudotime along the trajectory with no need for specifying starting cells
-        - efficient inference of vector field with no dependence on the discrimination between spliced and unspliced mRNAs
-        - cell trajectory reconstruction using latent space that incorporates both intrinsic transcriptome and extrinsic time information
-        - model-based prediction of pseudotime, vector field, and latent space for query cells/datasets
-        - reconstruction of transcriptomic space given an unobserved time interval
-        
-        # scTour performance
-        
-        ✅ insensitive to batch effects  
-        
-        ✅ robust to cell subsampling  
-        
-        ✅ scalable to large datasets
-        
-        # Installation
+        ## Installation
         
         [![Python Versions](https://img.shields.io/badge/python-3.7+-brightgreen.svg)](https://pypi.org/project/sctour)
         
         ```console
         pip install sctour
         ```
         
-        # Documentation
+        ## Documentation
         
         [![Documentation Status](https://readthedocs.org/projects/sctour/badge/?version=latest)](https://sctour.readthedocs.io/en/latest/?badge=latest)
         
         Full documentation can be found [here](https://sctour.readthedocs.io/en/latest/).
         
+        ## Reference
+        
+        [Qian Li, scTour: a deep learning architecture for robust inference and accurate prediction of cellular dynamics. Genome Biology, 2023](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02988-9)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sctour-0.1.3/README.md` & `sctour-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 
-# About scTour
+# scTour
 
-scTour is an innovative and comprehensive method for dissecting cellular dynamics by analysing datasets derived from single-cell genomics. It provides a unifying framework to depict the full picture of developmental processes from multiple angles including developmental pseudotime, vector field and latent space, and further generalises these functionalities to a multi-task architecture for within-dataset inference and cross-dataset prediction of cellular dynamics in a batch-insensitive manner.
+<img src="https://github.com/LiQian-XC/sctour/blob/main/docs/source/_static/img/scTour_head_image.png" width="400px" align="left">
 
-<p align="center"><img src="https://github.com/LiQian-XC/sctour/blob/ae9b45e69941bcabf3ad498dde781eb991168b83/docs/source/_static/img/scTour_head_image.png" width="700px" align="center"></p>
+scTour is an innovative and comprehensive method for dissecting cellular dynamics by analysing datasets derived from single-cell genomics.
 
-# Preprint
+It provides a unifying framework to depict the full picture of developmental processes from multiple angles including the developmental pseudotime, vector field and latent space.
 
-Consider citing this [paper](https://www.biorxiv.org/content/10.1101/2022.04.17.488600v1) if you use scTour in your analysis.
+It further generalises these functionalities to a multi-task architecture for within-dataset inference and cross-dataset prediction of cellular dynamics in a batch-insensitive manner.  
+  
+## Key features
 
-# scTour features
+- cell pseudotime estimation with no need for specifying starting cells.
+- transcriptomic vector field inference with no discrimination between spliced and unspliced mRNAs.
+- latent space mapping by combining intrinsic transcriptomic structure with extrinsic pseudotime ordering.
+- model-based prediction of pseudotime, vector field, and latent space for query cells/datasets/time intervals.
+- insensitive to batch effects; robust to cell subsampling; scalable to large datasets.
 
-- unsupervised estimates of cell pseudotime along the trajectory with no need for specifying starting cells
-- efficient inference of vector field with no dependence on the discrimination between spliced and unspliced mRNAs
-- cell trajectory reconstruction using latent space that incorporates both intrinsic transcriptome and extrinsic time information
-- model-based prediction of pseudotime, vector field, and latent space for query cells/datasets
-- reconstruction of transcriptomic space given an unobserved time interval
-
-# scTour performance
-
-✅ insensitive to batch effects  
-
-✅ robust to cell subsampling  
-
-✅ scalable to large datasets
-
-# Installation
+## Installation
 
 [![Python Versions](https://img.shields.io/badge/python-3.7+-brightgreen.svg)](https://pypi.org/project/sctour)
 
 ```console
 pip install sctour
 ```
 
-# Documentation
+## Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/sctour/badge/?version=latest)](https://sctour.readthedocs.io/en/latest/?badge=latest)
 
 Full documentation can be found [here](https://sctour.readthedocs.io/en/latest/).
+
+## Reference
+
+[Qian Li, scTour: a deep learning architecture for robust inference and accurate prediction of cellular dynamics. Genome Biology, 2023](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02988-9)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sctour-0.1.3/sctour/_utils.py` & `sctour-1.0.0/sctour/_utils.py`

 * *Files identical despite different names*

### Comparing `sctour-0.1.3/sctour/data.py` & `sctour-1.0.0/sctour/data.py`

 * *Files identical despite different names*

### Comparing `sctour-0.1.3/sctour/model.py` & `sctour-1.0.0/sctour/model.py`

 * *Files identical despite different names*

### Comparing `sctour-0.1.3/sctour/module.py` & `sctour-1.0.0/sctour/module.py`

 * *Files identical despite different names*

### Comparing `sctour-0.1.3/sctour/train.py` & `sctour-1.0.0/sctour/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,29 +10,46 @@
 from tqdm import tqdm
 import os
 from collections import defaultdict
 
 from .model import TNODE
 from ._utils import get_step_size
 from .data import split_data, MakeDataset, BatchSampler
+from . import logger
 
 
 ##reverse time
-def reverse_time(t):
-    return 1 - t
+def reverse_time(
+    T: np.ndarray,
+) -> np.ndarray:
+    """
+    Post-inference adjustment to reverse the pseudotime.
+
+    Parameters
+    ----------
+    T
+        The pseudotime inferred for each cell.
+
+    Returns
+    ----------
+    :class:`~numpy.ndarray`
+        The reversed pseudotime.
+    """
+
+    return 1 - T
 
 
 class Trainer:
     """
     Class for implementing the scTour training process.
 
     Parameters
     ----------
     adata
-        An :class:`~anndata.AnnData` object.
+        An :class:`~anndata.AnnData` object for the training data.
     percent
         The percentage of cells used for model training. Default to 0.2 when the cell number > 10,000 and to 0.9 otherwise.
     n_latent
         The dimensionality of the latent space.
         (Default: 5)
     n_ode_hidden
         The dimensionality of the hidden layer for the latent ODE function.
@@ -40,60 +57,60 @@
     n_vae_hidden
         The dimensionality of the hidden layer for the VAE.
         (Default: 128)
     batch_norm
         Whether to include a `BatchNorm` layer.
         (Default: `False`)
     ode_method
-        The solver for integration.
+        The solver for ODE. List of ODE solvers can be found in `torchdiffeq`.
         (Default: `'euler'`)
     step_size
         The step size during integration.
     alpha_recon_lec
-        The scaling factor for the reconstruction loss from encoder-derived latent space.
+        The scaling factor for the reconstruction error from encoder-derived latent space.
         (Default: 0.5)
     alpha_recon_lode
-        The scaling factor for the reconstruction loss from ODE-solver latent space.
+        The scaling factor for the reconstruction error from ODE-solver-derived latent space.
         (Default: 0.5)
     alpha_kl
-        The scaling factor for the KL divergence.
+        The scaling factor for the KL divergence in the loss function.
         (Default: 1.0)
     loss_mode
         The mode for calculating the reconstruction error.
         (Default: `'nb'`)
-        Three modes are included
-        ``'mse'``: mean squared error
-        ``'nb'``: negative binomial conditioned likelihood
-        ``'zinb'``: zero-inflated negative binomial conditioned likelihood
+        Three modes are included:
+        ``'mse'``: mean squared error;
+        ``'nb'``: negative binomial conditioned likelihood;
+        ``'zinb'``: zero-inflated negative binomial conditioned likelihood.
     nepoch
         Number of epochs.
     batch_size
         The batch size during training.
         (Default: 1024)
     drop_last
-        Whether or not drop the last batch when its size is smaller than the batch_size
+        Whether or not drop the last batch when its size is smaller than `batch_size`.
         (Default: `False`)
     lr
         The learning rate.
         (Default: 1e-3)
     wt_decay
-        The weight decay for Adam optimizer.
+        The weight decay (L2 penalty) for Adam optimizer.
         (Default: 1e-6)
     eps
-        The eps for Adam optimizer.
+        The `eps` parameter for Adam optimizer.
         (Default: 0.01)
     random_state
         The seed for generating random numbers.
         (Default: 0)
     val_frac
         The percentage of data used for validation.
         (Default: 0.1)
     use_gpu
-        Whether to use GPU when available
-        (Default: True)
+        Whether to use GPU when available.
+        (Default: `True`)
     """
 
     def __init__(
         self,
         adata: AnnData,
         percent: Optional[float] = None,
         n_latent: int = 5,
@@ -114,49 +131,67 @@
         eps: float = 0.01,
         random_state: int = 0,
         val_frac: float = 0.1,
         use_gpu: bool = True,
     ):
         self.loss_mode = loss_mode
         if self.loss_mode not in ['mse', 'nb', 'zinb']:
-            raise ValueError(f"`loss_mode` must be one of ['mse', 'nb', 'zinb'], but input was '{self.loss_mode}'.")
+            raise ValueError(
+                    f"`loss_mode` must be one of ['mse', 'nb', 'zinb'], but input was '{self.loss_mode}'."
+                    )
 
         if (alpha_recon_lec < 0) or (alpha_recon_lec > 1):
-            raise ValueError('`alpha_recon_lec` must be between 0 and 1.')
+            raise ValueError(
+                    '`alpha_recon_lec` must be between 0 and 1.'
+                    )
         if (alpha_recon_lode < 0) or (alpha_recon_lode > 1):
-            raise ValueError('`alpha_recon_lode` must be between 0 and 1.')
+            raise ValueError(
+                    '`alpha_recon_lode` must be between 0 and 1.'
+                    )
         if alpha_recon_lec + alpha_recon_lode != 1:
-            raise ValueError('The sum of `alpha_recon_lec` and `alpha_recon_lode` must be 1.')
+            raise ValueError(
+                    'The sum of `alpha_recon_lec` and `alpha_recon_lode` must be 1.'
+                    )
 
         self.adata = adata
         if 'n_genes_by_counts' not in self.adata.obs:
-            raise KeyError("`n_genes_by_counts` not found in `.obs` of the AnnData. Please run `scanpy.pp.calculate_qc_metrics` first to calculate the number of genes detected in each cell.")
+            raise KeyError(
+                    "`n_genes_by_counts` not found in `.obs` of the AnnData. Please run `scanpy.pp.calculate_qc_metrics` first to calculate the number of genes detected in each cell."
+                    )
         if loss_mode == 'mse':
             if (self.adata.X.min() < 0) or (self.adata.X.max() > np.log1p(1e6)):
-                raise ValueError("Invalid expression matrix in `.X`. `mse` mode expects log1p(normalized expression) in `.X` of the AnnData.")
+                raise ValueError(
+                        "Invalid expression matrix in `.X`. `mse` mode expects log1p(normalized expression) in `.X` of the AnnData."
+                        )
         else:
             X = self.adata.X.data if sparse.issparse(self.adata.X) else self.adata.X
             if (X.min() < 0) or np.any(~np.equal(np.mod(X, 1), 0)):
-                raise ValueError(f"Invalid expression matrix in `.X`. `{self.loss_mode}` mode expects raw UMI counts in `.X` of the AnnData.")
+                raise ValueError(
+                        f"Invalid expression matrix in `.X`. `{self.loss_mode}` mode expects raw UMI counts in `.X` of the AnnData."
+                        )
 
         self.n_cells = adata.n_obs
         self.batch_size = batch_size
         self.drop_last = drop_last
         self.percent = percent
         if self.percent is None:
             if self.n_cells > 10000:
                 self.percent = .2
             else:
                 self.percent = .9
         else:
             if (self.percent < 0) or (self.percent > 1):
-                raise ValueError("`percent` must be between 0 and 1.")
+                raise ValueError(
+                        "`percent` must be between 0 and 1."
+                        )
         self.val_frac = val_frac
         if (self.val_frac < 0) or (self.val_frac > 1):
-            raise ValueError('`val_frac` must be between 0 and 1.')
+            raise ValueError(
+                    '`val_frac` must be between 0 and 1.'
+                    )
 
         if nepoch is None:
             ncells = round(self.n_cells * self.percent)
             self.nepoch = np.min([round((10000 / ncells) * 400), 400])
         else:
             self.nepoch = nepoch
 
@@ -168,20 +203,24 @@
         self.random_state = random_state
         np.random.seed(random_state)
 #       random.seed(random_state)
         torch.manual_seed(random_state)
 #       torch.backends.cudnn.benchmark = False
 #       torch.use_deterministic_algorithms(True)
 
+        self.use_gpu = use_gpu
         gpu = torch.cuda.is_available() and use_gpu
         if gpu:
             torch.cuda.manual_seed(random_state)
             self.device = torch.device('cuda')
+            logger.info('Running using GPU.')
         else:
             self.device = torch.device('cpu')
+            logger.info('Running using CPU.')
+
         self.n_int = adata.n_vars
         self.model_kwargs = dict(
             device = self.device,
             n_int = self.n_int,
             n_latent = n_latent,
             n_ode_hidden = n_ode_hidden,
             n_vae_hidden = n_vae_hidden,
@@ -193,15 +232,15 @@
             alpha_kl = alpha_kl,
             loss_mode = loss_mode,
         )
         self.model = TNODE(**self.model_kwargs)
         self.log = defaultdict(list)
 
 
-    def get_data_loaders(self) -> None:
+    def _get_data_loaders(self) -> None:
         """
         Generate Data Loaders for training and validation datasets.
         """
 
         train_data, val_data = split_data(self.adata, self.percent, self.val_frac)
         self.train_dataset = MakeDataset(train_data, self.loss_mode)
         self.val_dataset = MakeDataset(val_data, self.loss_mode)
@@ -209,31 +248,34 @@
 #        sampler = BatchSampler(train_data.n_obs, self.batch_size, self.drop_last)
 #        self.train_dl = DataLoader(self.train_dataset, batch_sampler = sampler)
         self.train_dl = DataLoader(self.train_dataset, batch_size = self.batch_size, shuffle = True)
         self.val_dl = DataLoader(self.val_dataset, batch_size = self.batch_size)
 
 
     def train(self):
-        self.get_data_loaders()
+        """
+        Model training.
+        """
+        self._get_data_loaders()
 
         params = filter(lambda p: p.requires_grad, self.model.parameters())
         self.optimizer = torch.optim.Adam(params, lr = self.lr, weight_decay = self.wt_decay, eps = self.eps)
 
         with tqdm(total=self.nepoch, unit='epoch') as t:
             for tepoch in range(t.total):
-                train_loss = self.on_epoch_train(self.train_dl)
-                val_loss = self.on_epoch_val(self.val_dl)
+                train_loss = self._on_epoch_train(self.train_dl)
+                val_loss = self._on_epoch_val(self.val_dl)
                 self.log['train_loss'].append(train_loss)
                 self.log['validation_loss'].append(val_loss)
                 t.set_description(f"Epoch {tepoch + 1}")
                 t.set_postfix({'train_loss': train_loss, 'val_loss': val_loss}, refresh=False)
                 t.update()
 
 
-    def on_epoch_train(self, DL) -> float:
+    def _on_epoch_train(self, DL) -> float:
         """
         Go through the model and update the model parameters.
 
         Parameters
         ----------
         DL
             DataLoader for training dataset.
@@ -259,15 +301,15 @@
             ss += X.size(0)
 
         train_loss = total_loss/ss
         return train_loss
 
 
     @torch.no_grad()
-    def on_epoch_val(self, DL) -> float:
+    def _on_epoch_val(self, DL) -> float:
         """
         Validate using validation dataset.
 
         Parameters
         ----------
         DL
             DataLoader for validation dataset.
@@ -288,36 +330,32 @@
             total_loss += loss.item() * X.size(0)
             ss += X.size(0)
 
         val_loss = total_loss/ss
         return val_loss
 
 
-    @torch.no_grad()
-    def get_time(self) -> np.ndarray:
+    def get_time(
+        self,
+        ) -> np.ndarray:
         """
-        Get the developmental pseudotime for all cells.
+        Infer the developmental pseudotime.
 
         Returns
         ----------
         :class:`~numpy.ndarray`
-            The estimated pseudotime of cells.
+            The pseudotime inferred for each cell.
         """
 
-        self.model.eval()
         X = self.adata.X
         if self.loss_mode in ['nb', 'zinb']:
             X = np.log1p(X)
-        if sparse.issparse(X):
-            X = X.A
-        X = torch.tensor(X).to(self.device)
-        ts, _, _ = self.model.encoder(X)
-        ts = ts.ravel()
+        ts = self._get_time(self.model, X)
 
-        ## The model might return reversed time. Check this based on number of genes expressed in cells
+        ## The model might return pseudotime in reverse order. Check this based on number of genes expressed in each cell.
         if self.time_reverse is None:
             n_genes = torch.tensor(self.adata.obs['n_genes_by_counts'].values).float().log1p().to(self.device)
             m_ts = ts.mean()
             m_ngenes = n_genes.mean()
             beta_direction = (ts * n_genes).sum() - len(ts) * m_ts * m_ngenes
             if beta_direction > 0:
                 self.time_reverse = True
@@ -325,142 +363,265 @@
                 self.time_reverse = False
         if self.time_reverse:
             ts = 1 - ts
 
         return ts.cpu().numpy()
 
 
-    @torch.no_grad()
     def get_vector_field(
         self,
         T: np.ndarray,
         Z: np.ndarray,
-        model: Optional[str] = None,
     ) -> np.ndarray:
         """
-        Get the vector field.
+        Infer the vector field.
 
         Parameters
         ----------
         T
-            The estimated pseudotime for each cell.
+            The pseudotime estimated for each cell.
         Z
             The latent representation for each cell.
-        model
-            The model used to get the vector field. Only provided when using the saved model.
 
         Returns
         ----------
         :class:`~numpy.ndarray`
             The estimated vector field.
         """
 
-        model = self.get_model(model)
-        model.eval()
-        if not (isinstance(T, np.ndarray) and isinstance(Z, np.ndarray)):
-            raise TypeError('The inputs must be numpy arrays.')
-        Z = torch.tensor(Z)
-        T = torch.tensor(T)
-        if self.time_reverse is None:
-            raise RuntimeError('It seems you did not run get_time() function first. Please run get_time() before you run get_vector_field().')
-        direction = 1
-        if self.time_reverse:
-            direction = -1
-        return direction * model.lode_func(T, Z).numpy()
+        vf = self._get_vector_field(
+                                    self.model,
+                                    T,
+                                    Z,
+                                    self.time_reverse,
+                                    )
+        return vf
+
+
+    def get_latentsp(
+        self,
+        alpha_z: float = .5,
+        alpha_predz: float = .5,
+        step_size: Optional[int] = None,
+        step_wise: bool = False,
+        batch_size: Optional[int] = None,
+    ) -> tuple:
+        """
+        Infer the latent space.
+
+        Parameters
+        ----------
+        alpha_z
+            Scaling factor for encoder-derived latent space.
+            (Default: 0.5)
+        alpha_predz
+            Scaling factor for ODE-solver-derived latent space.
+            (Default: 0.5)
+        step_size
+            Step size during integration.
+        step_wise
+            Whether to perform step-wise integration by iteratively considering only two time points each time.
+            (Default: `False`)
+        batch_size
+            Batch size when deriving the latent space. The default is no mini-batching.
+
+        Returns
+        ----------
+        tuple
+            3-tuple of weighted combined latent space, encoder-derived latent space, and ODE-solver-derived latent space.
+        """
+
+        X = self.adata.X
+        if self.model.loss_mode in ['nb', 'zinb']:
+            X = np.log1p(X)
+        mix_zs, zs, pred_zs = self._get_latentsp(self.model,
+                                                 X,
+                                                 alpha_z,
+                                                 alpha_predz,
+                                                 step_size,
+                                                 step_wise,
+                                                 batch_size,
+                                                 )
+        return mix_zs, zs, pred_zs
 
 
     def save_model(
         self,
         save_dir: str,
         save_prefix: str,
     ) -> None:
         """
-        Save the trained model.
+        Save the trained scTour model.
 
         Parameters
         ----------
         save_dir
             The directory where the model will be saved.
         save_prefix
-            The prefix for model name.
+            The prefix for model name. The model will be saved in 'save_dir/save_prefix.pth'.
         """
 
         save_path = os.path.abspath(os.path.join(save_dir, f'{save_prefix}.pth'))
+#        save_path = os.path.abspath(os.path.join(save_dir, f'{save_prefix}.tar'))
         torch.save(
             {
                 'model_state_dict': self.model.state_dict(),
                 'optimizer_state_dict': self.optimizer.state_dict(),
-                'var_names': self.adata.var_names,
+                'model_kwargs': self.model_kwargs,
+                'time_reverse': self.time_reverse,
+                'adata': self.adata,
+                'percent': self.percent,
                 'nepoch': self.nepoch,
+                'batch_size': self.batch_size,
                 'random_state': self.random_state,
-                'percent': self.percent,
-                'time_reverse': self.time_reverse,
-                'model_kwargs': self.model_kwargs,
+                'drop_last': self.drop_last,
+                'lr': self.lr,
+                'wt_decay': self.wt_decay,
+                'eps': self.eps,
+                'val_frac': self.val_frac,
+                'use_gpu': self.use_gpu,
             },
             save_path
         )
 
 
+    @staticmethod
     @torch.no_grad()
-    def get_latentsp(
-        self,
-        X: Optional[Union[np.ndarray, spmatrix]] = None,
+    def _get_time(
+        model: TNODE,
+        X: Union[np.ndarray, spmatrix],
+        ) -> torch.tensor:
+        """
+        Derive the developmental pseudotime for cells.
+
+        Parameters
+        ----------
+        model
+            The trained scTour model.
+        X
+            The data matrix.
+
+        Returns
+        ----------
+        :class:`torch.Tensor`
+            The pseudotime estimated for each cell.
+        """
+
+        model.eval()
+        if sparse.issparse(X):
+            X = X.A
+        X = torch.tensor(X).to(model.device)
+        ts, _, _ = model.encoder(X)
+        ts = ts.ravel()
+        return ts
+
+
+    @staticmethod
+    @torch.no_grad()
+    def _get_vector_field(
+        model: TNODE,
+        T: np.ndarray,
+        Z: np.ndarray,
+        time_reverse: bool,
+    ) -> np.ndarray:
+        """
+        Derive the vector field for cells.
+
+        Parameters
+        ----------
+        model
+            The trained scTour model.
+        T
+            The pseudotime for each cell.
+        Z
+            The latent representation for each cell.
+        time_reverse
+            Whether to reverse the vector field.
+
+        Returns
+        ----------
+        :class:`~numpy.ndarray`
+            The estimated vector field.
+        """
+
+        model.eval()
+        if not (isinstance(T, np.ndarray) and isinstance(Z, np.ndarray)):
+            raise TypeError(
+                    'The inputs must be numpy arrays.'
+                    )
+        Z = torch.tensor(Z)
+        T = torch.tensor(T)
+        if time_reverse is None:
+            raise RuntimeError(
+                    'It seems you did not run `get_time()` function first after model training.'
+                    )
+        direction = 1
+        if time_reverse:
+            direction = -1
+        return direction * model.lode_func(T, Z).numpy()
+
+
+    @staticmethod
+    @torch.no_grad()
+    def _get_latentsp(
+        model: TNODE,
+        X: Union[np.ndarray, spmatrix],
         alpha_z: float = .5,
         alpha_predz: float = .5,
         step_size: Optional[int] = None,
         step_wise: bool = False,
         batch_size: Optional[int] = None,
-        model: Optional[str] = None,
     ):
         """
-        Get the latent representations of cells.
+        Derive the latent representations of cells.
 
         Parameters
         ----------
+        model
+            The trained scTour model.
         X
-            The data matrix. Only provided when you want to get the latent representations for data not used for training.
+            The data matrix.
         alpha_z
             Scaling factor for encoder-derived latent space.
             (Default: 0.5)
         alpha_predz
             Scaling factor for ODE-solver-derived latent space.
             (Default: 0.5)
         step_size
             Step size during integration.
         step_wise
-            Whether to perform step-wise integration by providing just two time points at a time.
+            Whether to perform step-wise integration by iteratively considering only two time points each time.
             (Default: `False`)
         batch_size
-            Batch size during getting the latent space. The default is no mini-batching.
-        model
-            The model used to get the latent space. Only provided when you use the saved model.
+            Batch size when deriving the latent space. The default is no mini-batching.
 
         Returns
         ----------
         tuple
-            3-tuple of mixed latent space, encoder-derived latent space, and ODE-solver-derived latent space.
+            3-tuple of weighted combined latent space, encoder-derived latent space, and ODE-solver-derived latent space.
         """
 
-        model = self.get_model(model)
         model.eval()
 
         if (alpha_z < 0) or (alpha_z > 1):
-            raise ValueError('`alpha_z` must be between 0 and 1.')
+            raise ValueError(
+                    '`alpha_z` must be between 0 and 1.'
+                    )
         if (alpha_predz < 0) or (alpha_predz > 1):
-            raise ValueError('`alpha_predz` must be between 0 and 1.')
+            raise ValueError(
+                    '`alpha_predz` must be between 0 and 1.'
+                    )
         if alpha_z + alpha_predz != 1:
-            raise ValueError('The sum of `alpha_z` and `alpha_predz` must be 1.')
+            raise ValueError(
+                    'The sum of `alpha_z` and `alpha_predz` must be 1.'
+                    )
 
-        if X is None:
-            X = self.adata.X
-            if model.loss_mode in ['nb', 'zinb']:
-                X = np.log1p(X)
         if sparse.issparse(X):
             X = X.A
-        X = torch.tensor(X).to(self.device)
+        X = torch.tensor(X).to(model.device)
         T, qz_mean, qz_logvar = model.encoder(X)
         T = T.ravel().cpu()
         epsilon = torch.randn(qz_mean.size())
         zs = epsilon * torch.exp(.5 * qz_logvar.cpu()) + qz_mean.cpu()
 
         sort_T, sort_idx, sort_ridx = np.unique(T, return_index=True, return_inverse=True)
         sort_T = torch.tensor(sort_T)
@@ -490,261 +651,20 @@
                 pred_z = torch.empty((len(t), z.size(1)))
                 pred_z[0] = z0
                 for j in range(len(t) - 1):
                     t2 = t[j:(j + 2)]
                     options = get_step_size(step_size, t2[0], t2[-1], len(t2))
                     pred_z[j + 1] = odeint(
                                             model.lode_func,
-                                            z0,
+                                            z[j],
                                             t2,
                                             method = model.ode_method,
                                             options = options
                                     )[1]
-                    z0 = z[j + 1]
 
             pred_zs += [pred_z]
 
         pred_zs = torch.cat(pred_zs)
         pred_zs = pred_zs[sort_ridx]
         mix_zs = alpha_z * zs + alpha_predz * pred_zs
 
         return mix_zs.numpy(), zs.numpy(), pred_zs.numpy()
-
-
-    @torch.no_grad()
-    def predict_time(
-        self,
-        adata: Optional[AnnData] = None,
-        reverse: bool = False,
-        get_ltsp: bool = True,
-        mode: Literal['coarse', 'fine'] = 'fine',
-        alpha_z: float = .5,
-        alpha_predz: float = .5,
-        step_size: Optional[int] = None,
-        step_wise: bool = False,
-        batch_size: Optional[int] = None,
-        model: Optional[str] = None,
-    ) -> Union[np.ndarray, tuple]:
-        """
-        Predict the pseudotime of cells given their transcriptomes, as well as their latent representations when get_ltsp is set to True.
-
-        Parameters
-        ----------
-        adata
-            An :class:`~anndata.AnnData` object from the dataset that will be predicted.
-        reverse
-            Whether to reverse the predicted pseudotime. When the pseudotime returned by get_time() function was in reverse order and you used the post-inference adjustment (reverse_time() function), please set this parameter to `True`.
-            (Default: `False`)
-        get_ltsp
-            Whether to get the latent space as well.
-            (Default: `False`)
-        mode
-            The method for getting the latent space.
-            Two modes are included
-            ``'fine'``: take the training dataset into consideration when predicting the latent space.
-            ``'coarse'``: derive the latent space of the given dataset directly without involving the training data.
-        alpha_z
-            Scaling factor for encoder-derived latent space.
-            (Default: 0.5)
-        alpha_predz
-            Scaling factor for ODE-solver-derived latent space.
-            (Default: 0.5)
-        step_size
-            The step size during integration.
-        step_wise
-            Whether to perform step-wise integration by providing just two time points at a time.
-            (Default: `False`)
-        batch_size
-            Batch size during getting the latent space. The default is no mini-batching.
-        model
-            The model used to predict the pseudotime. Only provided when using the saved model.
-
-        Returns
-        ----------
-        The predicted pseudotime and (if `get_ltsp = True`) the latent space.
-        """
-
-        model = self.get_model(model)
-        model.eval()
-
-        if self.time_reverse is None:
-            raise RuntimeError('It seems you did not run get_time() function first. Please run get_time() using training data before you run predict_time() using test data.')
-
-        if adata is None:
-            X = self.adata.X
-            if model.loss_mode in ['nb', 'zinb']:
-                X = np.log1p(X)
-        else:
-            if len(adata.var_names.intersection(self.adata.var_names)) != self.adata.n_vars:
-                raise ValueError("The given AnnData must contain all the genes that are used for model training from the training dataset.")
-
-            adata = adata[:, self.adata.var_names]
-            X = adata.X
-            if model.loss_mode == 'mse':
-                if (X.min() < 0) or (X.max() > np.log1p(1e6)):
-                    raise ValueError("Invalid expression matrix in `.X`. Model trained from `mse` mode expects log1p(normalized expression) in `.X` of the AnnData.")
-            else:
-                data = X.data if sparse.issparse(X) else X
-                if (data.min() < 0) or np.any(~np.equal(np.mod(data, 1), 0)):
-                    raise ValueError(f"Invalid expression matrix in `.X`. Model trained from `{model.loss_mode}` mode expects raw UMI counts in `.X` of the AnnData.")
-                else:
-                    X = np.log1p(X)
-
-        if sparse.issparse(X):
-            X = X.A
-        X = torch.tensor(X).to(self.device)
-        ts, _, _ = model.encoder(X)
-        ts = ts.ravel()
-        if self.time_reverse:
-            ts = 1 - ts
-        if reverse:
-            ts = 1 - ts
-
-        if get_ltsp:
-            if mode == 'coarse':
-                mix_zs, zs, pred_zs = self.get_latentsp(
-                                        X = X.cpu().numpy(),
-                                        alpha_z = alpha_z,
-                                        alpha_predz = alpha_predz,
-                                        step_size = step_size,
-                                        step_wise = step_wise,
-                                        batch_size = batch_size,
-                                        model = model,
-                                        )
-            if mode == 'fine':
-                X2 = self.adata.X
-                if model.loss_mode in ['nb', 'zinb']:
-                    X2 = np.log1p(X2)
-                if sparse.issparse(X2):
-                    X2 = X2.A
-                mix_zs, zs, pred_zs = self.get_latentsp(
-                                        X = np.vstack((X.cpu().numpy(), X2)),
-                                        alpha_z = alpha_z,
-                                        alpha_predz = alpha_predz,
-                                        step_size = step_size,
-                                        step_wise = step_wise,
-                                        batch_size = batch_size,
-                                        model = model,
-                                        )
-                mix_zs = mix_zs[:len(X)]
-                zs = zs[:len(X)]
-                pred_zs = pred_zs[:len(X)]
-
-        if not get_ltsp:
-            return ts.cpu().numpy()
-        else:
-            return ts.cpu().numpy(), mix_zs, zs, pred_zs
-
-
-    @torch.no_grad()
-    def predict_ltsp_from_time(
-        self,
-        T: np.ndarray,
-        reverse: bool = False,
-        step_wise: bool = True,
-        step_size: Optional[int] = None,
-        alpha_z: float = 0.5,
-        alpha_predz: float = 0.5,
-        k: int = 20,
-        model: Optional[str] = None,
-    ) -> np.ndarray:
-        """
-        Predict the transcriptomic latent space for unobserved time intervals.
-
-        Parameters
-        ----------
-        T
-            A 1D numpy array containing the time points (unobserved time interval) with values between 0 and 1.
-        reverse
-            Whether to reverse the reference pseudotime from training data. When the pseudotime returned by get_time() function was in reverse order and you used the post-inference adjustment (reverse_time() function), please set this parameter to `True`.
-            (Default: `False`)
-        step_wise
-            Whether to perform step-wise integration by providing just two time points at a time when inferring the reference latent space from training data.
-            (Default: `True`)
-        step_size
-            The step size during integration.
-        alpha_z
-            Scaling factor for encoder-derived latent space when inferring the reference latent space from training data.
-            (Default: 0.5)
-        alpha_predz
-            Scaling factor for ODE-solver-derived latent space when inferring the reference latent space from training data.
-            (Default: 0.5)
-        k
-            The k nearest neighbors in the time space used to predict the latent space for each unobserved time point.
-            (Default: 20)
-        model
-            The model used to predict the transcriptomic latent space. Only provided when using the saved model.
-
-        Returns
-        ----------
-        :class:`~numpy.ndarray`
-            Predicted latent space for the unobserved time interval.
-        """
-
-        model = self.get_model(model)
-        model.eval()
-
-        if not isinstance(T, np.ndarray):
-            raise TypeError("The input time interval must be a numpy array.")
-        if len(T.shape) > 1:
-            raise TypeError("The input time interval must be a 1D numpy array.")
-        if np.any(T < 0) or np.any(T > 1):
-            raise ValueError("The provided time points must be between 0 and 1.")
-
-        ridx = np.random.permutation(len(T))
-        rT = torch.tensor(T[ridx])
-        ## get the reference time and latent space from the training data
-        mix_zs, zs, pred_zs = self.get_latentsp(step_wise = step_wise, step_size = step_size, model = model, alpha_z = alpha_z, alpha_predz = alpha_predz)
-        ts = self.predict_time(reverse = reverse, get_ltsp = False, model = model)
-#       zs = torch.tensor(zs).to(self.device)
-        zs = torch.tensor(mix_zs)
-        ts = torch.tensor(ts)
-
-        pred_T_zs = torch.empty((len(rT), model.n_latent))
-        for i, t in enumerate(rT):
-            diff = torch.abs(t - ts)
-            idxs = torch.argsort(diff)
-#            n = (diff == 0).sum()
-#            idxs = idxs[n:(k + n)]
-            if (diff == 0).any():
-                pred_T_zs[i] = zs[idxs[0]]
-            else:
-                idxs = idxs[:k]
-                k_zs = torch.empty((k, model.n_latent))
-                for j, idx in enumerate(idxs):
-                    z0 = zs[idx]
-                    t0 = ts[idx]
-                    pred_t = torch.stack((t0, t))
-                    if pred_t[0] < pred_t[1]:
-                        options = get_step_size(step_size, pred_t[0], pred_t[-1], len(pred_t))
-                    else:
-                        options = get_step_size(step_size, pred_t[-1], pred_t[0], len(pred_t))
-                    k_zs[j] = odeint(
-                                    model.lode_func,
-                                    z0,
-                                    pred_t,
-                                    method = model.ode_method,
-                                    options = options
-                                )[1]
-                k_zs = torch.mean(k_zs, dim = 0)
-                pred_T_zs[i] = k_zs
-                ts = torch.cat((ts, t.unsqueeze(0)))
-                zs = torch.cat((zs, k_zs.unsqueeze(0)))
-
-        pred_T_zs = pred_T_zs[np.argsort(ridx)]
-#       return pred_T_zs.numpy(), pred_zs
-        return pred_T_zs.numpy()
-
-
-    def get_model(self, model):
-        """
-        Get the model for inference/prediction (for internal use).
-        """
-
-        if isinstance(model, str):
-            checkpoint = torch.load(model, map_location=self.device)
-            model = TNODE(**checkpoint['model_kwargs'])
-            model.load_state_dict(checkpoint['model_state_dict'])
-            self.time_reverse = checkpoint['time_reverse']
-        if model is None:
-            model = self.model
-        return model
```

### Comparing `sctour-0.1.3/sctour/vector_field.py` & `sctour-1.0.0/sctour/vector_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     The calculation borrows the ideas from scvelo: https://github.com/theislab/scvelo/blob/master/scvelo/tools/velocity_graph.py.
 
     Parameters
     ----------
     adata
         An :class:`~anndata.AnnData` object.
     reverse
-        Whether to reverse the direction of the vector field. When the pseudotime returned by get_time() function was in reverse order and you used the post-inference adjustment (reverse_time() function), please set this parameter to `True`.
+        Whether to reverse the direction of the vector field. When the pseudotime returned by `get_time()` function was in reverse order and you used the post-inference adjustment (`reverse_time()` function), please set this parameter to `True`.
         (Default: `False`)
     zs_key
         The key in `.obsm` for storing the latent space.
     vf_key
         The key in `.obsm` for storing the vector field.
         (Default: `'X_VF'`)
     run_neigh
@@ -70,22 +70,26 @@
 
     if run_neigh or ('neighbors' not in adata.uns):
         if use_rep_neigh is None:
             use_rep_neigh = zs_key
             logger.warn(f"Warning: the parameter `use_rep_neigh` in function `plot_vector_field` is not provided. Use `{zs_key}` in `.obsm` of the AnnData instead.")
         else:
             if use_rep_neigh not in adata.obsm:
-                raise KeyError(f"`{use_rep_neigh}` not found in `.obsm` of the AnnData. Please provide valid `use_rep_neigh` for neighbor detection.")
+                raise KeyError(
+                        f"`{use_rep_neigh}` not found in `.obsm` of the AnnData. Please provide valid `use_rep_neigh` for neighbor detection."
+                        )
         sc.pp.neighbors(adata, use_rep = use_rep_neigh, n_neighbors = n_neigh)
     n_neigh = adata.uns['neighbors']['params']['n_neighbors'] - 1
 #    indices_matrix = adata.obsp['distances'].indices.reshape(-1, n_neigh)
 
     if t_key is not None:
         if t_key not in adata.obs:
-            raise KeyError(f"`{t_key}` not found in `.obs` of the AnnData. Please provide valid `t_key` for estimated pseudotime.")
+            raise KeyError(
+                    f"`{t_key}` not found in `.obs` of the AnnData. Please provide valid `t_key` for estimated pseudotime."
+                    )
         ts = adata.obs[t_key].values
         indices_matrix2 = np.zeros((ncells, n_neigh), dtype = int)
         for i in range(ncells):
             idx = np.abs(ts - ts[i]).argsort()[:(n_neigh + 1)]
             idx = np.setdiff1d(idx, i) if i in idx else idx[:-1]
             indices_matrix2[i] = idx
 #        indices_matrix = np.hstack([indices_matrix, indices_matrix2])
@@ -237,15 +241,15 @@
     density
         grid density
         (Default: 1.0)
 
     Returns
     ----------
     tuple
-        The embedding and unitary displacement vectors in grid level.
+        The embedding and unitary displacement vectors at grid level.
     """
 
     grs = []
     for i in range(E.shape[1]):
         m, M = np.min(E[:, i]), np.max(E[:, i])
         diff = M - m
         m = m - 0.01 * diff
@@ -312,14 +316,16 @@
     stream_color: str = 'k',
     stream_linewidth: int = 1,
     stream_arrowsize: int = 1,
     grid_density: float = 1.,
     grid_arrowcolor: str = 'grey',
     grid_arrowlength: int = 1,
     grid_arrowsize: int = 1,
+    show: bool = True,
+    save: Optional[Union[str, bool]] = None,
 #    color: Optional[str] = None,
 #    ax: Optional[Axes] = None,
     **kwargs,
 ):
     """
     Visualize the vector field.
     The visualization of vector field under an embedding borrows the ideas from scvelo: https://github.com/theislab/scvelo.
@@ -327,15 +333,15 @@
     Parameters
     ----------
     adata
         An :class:`~anndata.AnnData` object.
     zs_key
         The key in `.obsm` for storing the latent space.
     reverse
-        Whether to reverse the direction of the vector field. When the pseudotime returned by get_time() function was in reverse order and you used the post-inference adjustment (reverse_time() function), please set this parameter to `True`.
+        Whether to reverse the direction of the vector field. When the pseudotime returned by `get_time()` function was in reverse order and you used the post-inference adjustment (`reverse_time()` function), please set this parameter to `True`.
         (Default: `False`)
     vf_key
         The key in `.obsm` for storing the vector field.
     run_neigh
         Whether to run neighbor detection.
         (Default: `True`)
     use_rep_neigh
@@ -357,18 +363,18 @@
     self_transition
         Whether to take self-transition into consideration.
         (Default: `False`)
     smooth
         The factor for scale in Gaussian pdf.
         (Default: 0.5)
     density
-        Percentage of cells to show when displaying the vector field in the per-cell level.
-        (Default: 1.)
+        Percentage of cells to show when displaying the vector field at per-cell level.
+        (Default: 1.0)
     grid
-        Whether to display vector field as arrows in grid level.
+        Whether to display vector field as arrows at grid level.
         (Default: `False`)
     stream
         Whether to display vector field as streamplot.
         (Default: `True`)
     stream_density
         The density parameter in streamplot for controlling the closeness of the streamlines.
         (Default: 2)
@@ -378,44 +384,58 @@
     stream_linewidth
         The line width for streamplot.
         (Default: 1)
     stream_arrowsize
         The arrow size for streamplot.
         (Default: 1)
     grid_density
-        The grid-level density for showing vector field.
-        (Default: 1.)
+        The density for showing vector field as arrows at grid level.
+        (Default: 1.0)
     grid_arrowcolor
-        The arrow color when showing vector field as arrows in grid level.
+        The arrow color when showing vector field as arrows at grid level.
         (Default: `'grey'`)
     grid_arrowlength
-        The arrow length when showing vector field as arrows in grid level.
+        The arrow length when showing vector field as arrows at grid level.
         (Default: 1)
     grid_arrowsize
-        The arrow size when showing vector field as arrows in grid level.
+        The arrow size when showing vector field as arrows at grid level.
         (Default: 1)
+    show
+        Whether to show the plot.
+        (Default: `True`)
+    save
+        Whether to save the figure. If `True` or a `str`, the figure will be saved as 'sctour_vector_field.png' (if `True` provided) or a given filename (if a `str` provided).
     kwargs
         Parameters passed to :func:`scanpy.pl.embedding`.
 
     Returns
     ----------
-    :class:`~matplotlib.axes.Axes`
-        An :class:`~matplotlib.axes.Axes` object.
+    None
     """
 
     if zs_key not in adata.obsm:
-        raise KeyError(f"`{zs_key}` not found in `.obsm` of the AnnData. Please provide valid `zs_key` for latent space.")
+        raise KeyError(
+                f"`{zs_key}` not found in `.obsm` of the AnnData. Please provide valid `zs_key` for latent space."
+                )
     if vf_key not in adata.obsm:
-        raise KeyError(f"`{vf_key}` not found in `.obsm` of the AnnData. Please provide valid `vf_key` for vector field.")
+        raise KeyError(
+                f"`{vf_key}` not found in `.obsm` of the AnnData. Please provide valid `vf_key` for vector field."
+                )
     if E_key not in adata.obsm:
-        raise KeyError(f"`{E_key}` not found in `.obsm` of the AnnData. Please provide valid `E_key` for embedding.")
+        raise KeyError(
+                f"`{E_key}` not found in `.obsm` of the AnnData. Please provide valid `E_key` for embedding."
+                )
     if (grid_density < 0) or (grid_density > 1):
-        raise ValueError("`grid_density` must be between 0 and 1.")
+        raise ValueError(
+                "`grid_density` must be between 0 and 1."
+                )
     if (density < 0) or (density > 1):
-        raise ValueError("`density` must be between 0 and 1.")
+        raise ValueError(
+                "`density` must be between 0 and 1."
+                )
 
     ##calculate cosine similarity
     adata.obsp['cosine_similarity'] = cosine_similarity(
                                         adata,
                                         reverse = reverse,
                                         zs_key = zs_key,
                                         vf_key = vf_key,
@@ -483,8 +503,16 @@
             headaxislength = hal,
             color = grid_arrowcolor,
             linewidth = 0.2,
             zorder = 3,
         )
         ax.quiver(E[:, 0], E[:, 1], V[:, 0], V[:, 1], **quiver_kwargs)
 
-    return ax
+    if save:
+        if isinstance(save, str):
+            plt.savefig(save)
+        else:
+            plt.savefig('sctour_vector_field.png')
+    if show:
+        plt.show()
+    if save:
+        plt.close()
```

### Comparing `sctour-0.1.3/sctour.egg-info/PKG-INFO` & `sctour-1.0.0/sctour.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 Metadata-Version: 2.1
 Name: sctour
-Version: 0.1.3
+Version: 1.0.0
 Summary: a deep learning architecture for robust inference and accurate prediction of cellular dynamics
 Home-page: https://github.com/LiQian-XC/sctour
 Author: Qian Li
 Author-email: liqian.picb@gmail.com
 License: UNKNOWN
 Description: 
-        # About scTour
+        # scTour
         
-        scTour is an innovative and comprehensive method for dissecting cellular dynamics by analysing datasets derived from single-cell genomics. It provides a unifying framework to depict the full picture of developmental processes from multiple angles including developmental pseudotime, vector field and latent space, and further generalises these functionalities to a multi-task architecture for within-dataset inference and cross-dataset prediction of cellular dynamics in a batch-insensitive manner.
+        <img src="https://github.com/LiQian-XC/sctour/blob/main/docs/source/_static/img/scTour_head_image.png" width="400px" align="left">
         
-        <p align="center"><img src="https://github.com/LiQian-XC/sctour/blob/ae9b45e69941bcabf3ad498dde781eb991168b83/docs/source/_static/img/scTour_head_image.png" width="700px" align="center"></p>
+        scTour is an innovative and comprehensive method for dissecting cellular dynamics by analysing datasets derived from single-cell genomics.
         
-        # Preprint
+        It provides a unifying framework to depict the full picture of developmental processes from multiple angles including the developmental pseudotime, vector field and latent space.
         
-        Consider citing this [paper](https://www.biorxiv.org/content/10.1101/2022.04.17.488600v1) if you use scTour in your analysis.
+        It further generalises these functionalities to a multi-task architecture for within-dataset inference and cross-dataset prediction of cellular dynamics in a batch-insensitive manner.  
+          
+        ## Key features
         
-        # scTour features
+        - cell pseudotime estimation with no need for specifying starting cells.
+        - transcriptomic vector field inference with no discrimination between spliced and unspliced mRNAs.
+        - latent space mapping by combining intrinsic transcriptomic structure with extrinsic pseudotime ordering.
+        - model-based prediction of pseudotime, vector field, and latent space for query cells/datasets/time intervals.
+        - insensitive to batch effects; robust to cell subsampling; scalable to large datasets.
         
-        - unsupervised estimates of cell pseudotime along the trajectory with no need for specifying starting cells
-        - efficient inference of vector field with no dependence on the discrimination between spliced and unspliced mRNAs
-        - cell trajectory reconstruction using latent space that incorporates both intrinsic transcriptome and extrinsic time information
-        - model-based prediction of pseudotime, vector field, and latent space for query cells/datasets
-        - reconstruction of transcriptomic space given an unobserved time interval
-        
-        # scTour performance
-        
-        ✅ insensitive to batch effects  
-        
-        ✅ robust to cell subsampling  
-        
-        ✅ scalable to large datasets
-        
-        # Installation
+        ## Installation
         
         [![Python Versions](https://img.shields.io/badge/python-3.7+-brightgreen.svg)](https://pypi.org/project/sctour)
         
         ```console
         pip install sctour
         ```
         
-        # Documentation
+        ## Documentation
         
         [![Documentation Status](https://readthedocs.org/projects/sctour/badge/?version=latest)](https://sctour.readthedocs.io/en/latest/?badge=latest)
         
         Full documentation can be found [here](https://sctour.readthedocs.io/en/latest/).
         
+        ## Reference
+        
+        [Qian Li, scTour: a deep learning architecture for robust inference and accurate prediction of cellular dynamics. Genome Biology, 2023](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02988-9)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sctour-0.1.3/setup.py` & `sctour-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_readme():
     with open("README.md", "rt", encoding="utf-8") as fh:
         return fh.read()
 
 setuptools.setup(
     name='sctour',
-    version='0.1.3',
+    version='1.0.0',
     author='Qian Li',
     author_email='liqian.picb@gmail.com',
     description='a deep learning architecture for robust inference and accurate prediction of cellular dynamics',
     long_description=get_readme(),
     long_description_content_type="text/markdown",
     url='https://github.com/LiQian-XC/sctour',
     packages=setuptools.find_packages(),
```

