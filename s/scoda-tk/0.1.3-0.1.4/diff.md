# Comparing `tmp/scoda-tk-0.1.3.tar.gz` & `tmp/scoda-tk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.1.3.tar", last modified: Sun Jul 30 06:59:06 2023, max compression
+gzip compressed data, was "scoda-tk-0.1.4.tar", last modified: Sun Jul 30 07:07:44 2023, max compression
```

## Comparing `scoda-tk-0.1.3.tar` & `scoda-tk-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 06:59:06.267229 scoda-tk-0.1.3/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.3/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.3/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 06:59:06.267229 scoda-tk-0.1.3/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.3/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 06:58:08.000000 scoda-tk-0.1.3/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 06:59:06.267229 scoda-tk-0.1.3/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.3/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 06:59:06.251229 scoda-tk-0.1.3/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 06:59:06.251229 scoda-tk-0.1.3/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.3/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.3/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 06:59:06.267229 scoda-tk-0.1.3/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.3/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    16244 2023-07-29 16:28:13.000000 scoda-tk-0.1.3/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.3/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.3/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 06:58:11.000000 scoda-tk-0.1.3/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.3/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    57779 2023-07-30 06:58:15.000000 scoda-tk-0.1.3/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 06:59:06.267229 scoda-tk-0.1.3/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 06:59:06.000000 scoda-tk-0.1.3/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      754 2023-07-30 06:59:06.000000 scoda-tk-0.1.3/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 06:59:06.000000 scoda-tk-0.1.3/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 06:59:06.000000 scoda-tk-0.1.3/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 06:59:06.000000 scoda-tk-0.1.3/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 06:59:06.000000 scoda-tk-0.1.3/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.4/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.4/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.4/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 07:03:31.000000 scoda-tk-0.1.4/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.4/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.724121 scoda-tk-0.1.4/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.728121 scoda-tk-0.1.4/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.4/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.4/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    16244 2023-07-29 16:28:13.000000 scoda-tk-0.1.4/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.4/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.4/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 06:58:11.000000 scoda-tk-0.1.4/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.4/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17988 2023-07-30 07:07:12.000000 scoda-tk-0.1.4/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    57779 2023-07-30 07:03:21.000000 scoda-tk-0.1.4/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.1.3/LICENSE` & `scoda-tk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/PKG-INFO` & `scoda-tk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.3/src/scoda/cpdb.py` & `scoda-tk-0.1.4/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.1.4/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.1.4/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.1.4/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.1.4/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.1.4/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.1.4/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/deg.py` & `scoda-tk-0.1.4/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/gsea.py` & `scoda-tk-0.1.4/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/hicat.py` & `scoda-tk-0.1.4/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/icnv.py` & `scoda-tk-0.1.4/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/misc.py` & `scoda-tk-0.1.4/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.3/src/scoda/viz.py` & `scoda-tk-0.1.4/src/scoda/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
 
 
 def plot_cci_circ_m( df_lst, ncol = 3, figsize = (8,7), title = None, title_y = 1, title_fs = 18, 
                    text_fs = 16, num_fs = 12, margin = 0.08, alpha = 0.5, 
                    N = 500, R = 3, Rs = 0.1, lw_max = 20, lw_scale = 0.2, log_lw = False, 
                    node_size = 10, rot = False, cmap = 'Spectral', ws_hs = (0.2, 0.1) ):
     
-    cond_lst = list(df_dct.keys())
+    cond_lst = list(df_lst.keys())
     nc = ncol
     nr = int(np.ceil(len(cond_lst)/nc))
     # nr, nc = 1, int(len(cond_lst))
     fig, axes = plt.subplots(figsize = (figsize[0]*nc,figsize[1]*nr), nrows=nr, ncols=nc, # constrained_layout=True, 
                              gridspec_kw={'width_ratios': [1]*nc})
     fig.tight_layout() 
     plt.subplots_adjust(left=0.025, bottom=0.025, right=0.975, top=0.975, wspace=ws_hs[0], hspace=ws_hs[1])
```

### Comparing `scoda-tk-0.1.3/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.1.4/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.3/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.1.4/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/scoda/__init__.py
 src/scoda/cpdb.py
 src/scoda/deg.py
 src/scoda/gsea.py
 src/scoda/hicat.py
 src/scoda/icnv.py
 src/scoda/misc.py
+src/scoda/pipeline.py
 src/scoda/viz.py
 src/scoda/default_optional_files/analysis_config.py
 src/scoda/default_optional_files/cpdb.zip
 src/scoda/default_optional_files/hg38_gene_only.gtf
 src/scoda/default_optional_files/markers_hs.tsv
 src/scoda/default_optional_files/markers_mm.tsv
 src/scoda/default_optional_files/mm10_gene_only.gtf
```

