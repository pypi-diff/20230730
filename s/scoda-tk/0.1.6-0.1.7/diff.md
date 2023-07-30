# Comparing `tmp/scoda-tk-0.1.6.tar.gz` & `tmp/scoda-tk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.1.6.tar", last modified: Sun Jul 30 09:03:51 2023, max compression
+gzip compressed data, was "scoda-tk-0.1.7.tar", last modified: Sun Jul 30 09:23:06 2023, max compression
```

## Comparing `scoda-tk-0.1.6.tar` & `scoda-tk-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.6/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.6/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.6/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 09:03:34.000000 scoda-tk-0.1.6/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.6/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.267010 scoda-tk-0.1.6/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.267010 scoda-tk-0.1.6/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.6/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.6/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    16728 2023-07-30 08:53:26.000000 scoda-tk-0.1.6/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.6/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.6/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.1.6/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.6/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18987 2023-07-30 09:03:26.000000 scoda-tk-0.1.6/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.1.6/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:23:06.205342 scoda-tk-0.1.7/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.7/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.7/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 09:23:06.205342 scoda-tk-0.1.7/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.7/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 09:14:33.000000 scoda-tk-0.1.7/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 09:23:06.205342 scoda-tk-0.1.7/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.7/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:23:06.185342 scoda-tk-0.1.7/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:23:06.185342 scoda-tk-0.1.7/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.7/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.7/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:23:06.205342 scoda-tk-0.1.7/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.7/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    16728 2023-07-30 08:53:26.000000 scoda-tk-0.1.7/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.7/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.7/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.1.7/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.7/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18965 2023-07-30 09:22:41.000000 scoda-tk-0.1.7/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.1.7/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:23:06.205342 scoda-tk-0.1.7/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 09:23:06.000000 scoda-tk-0.1.7/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 09:23:06.000000 scoda-tk-0.1.7/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 09:23:06.000000 scoda-tk-0.1.7/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 09:23:06.000000 scoda-tk-0.1.7/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 09:23:06.000000 scoda-tk-0.1.7/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 09:23:06.000000 scoda-tk-0.1.7/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.1.6/LICENSE` & `scoda-tk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/PKG-INFO` & `scoda-tk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.6/pyproject.toml` & `scoda-tk-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.1.6"
+version = "0.1.7"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.1.6/src/scoda/cpdb.py` & `scoda-tk-0.1.7/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.1.7/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.1.7/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.1.7/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.1.7/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.1.7/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.1.7/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/deg.py` & `scoda-tk-0.1.7/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/gsea.py` & `scoda-tk-0.1.7/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/hicat.py` & `scoda-tk-0.1.7/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/icnv.py` & `scoda-tk-0.1.7/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/misc.py` & `scoda-tk-0.1.7/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda/pipeline.py` & `scoda-tk-0.1.7/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     return
 
 
 
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
-               data_dir = '.', n_cores = 4 ):
+               data_dir = '.', pval_max = 0.1, mean_min = 0, n_cores = 4 ):
     
     if 'celltype_minor_rev' in list(adata_t.obs.columns.values):
         celltype_col = 'celltype_minor_rev'
     else:
         celltype_col = 'celltype_minor'
 
     if cond_col not in list(adata_t.obs.columns.values):
@@ -214,23 +214,20 @@
         celltype = adata_s.obs[celltype_col]
 
         df_mn, df_pv = cpdb4_run( adata_s, celltype, db = cpdb_path,
                                   out_dir = out_dir, n_cores = n_cores,
                                   threshold = 0.05, gene_id_type = 'gene_name' )
 
         dfi, dfp, dfm, dfv = cpdb4_get_results( df_pv, df_mn, 
-                                                pval_max = 0.05, mean_min = 0.01 )
+                                                pval_max = pval_max, mean_min = mean_min )
 
         dfv_dct[s] = dfv
     ## End for
         
-    pval_max = cci_pval_max
-    mean_min = cci_mean_min
-
-    if unit_of_cci_run == 'condition':
+    if unit_of_cci_run == cond_col:
         
         adata_t.uns['CCI'] = dfv_dct
         
     else: 
         
         s2c_map = {}
         group_lst = []
```

### Comparing `scoda-tk-0.1.6/src/scoda/viz.py` & `scoda-tk-0.1.7/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.6/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.1.7/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.6/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.1.7/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

