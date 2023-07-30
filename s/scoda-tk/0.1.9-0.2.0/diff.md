# Comparing `tmp/scoda-tk-0.1.9.tar.gz` & `tmp/scoda-tk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.1.9.tar", last modified: Sun Jul 30 11:59:25 2023, max compression
+gzip compressed data, was "scoda-tk-0.2.0.tar", last modified: Sun Jul 30 12:22:12 2023, max compression
```

## Comparing `scoda-tk-0.1.9.tar` & `scoda-tk-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 11:59:25.513253 scoda-tk-0.1.9/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.9/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.9/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 11:59:25.513253 scoda-tk-0.1.9/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.9/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 11:58:36.000000 scoda-tk-0.1.9/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 11:59:25.513253 scoda-tk-0.1.9/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.9/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 11:59:25.485253 scoda-tk-0.1.9/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 11:59:25.489253 scoda-tk-0.1.9/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.9/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.9/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 11:59:25.509253 scoda-tk-0.1.9/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.9/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 09:42:12.000000 scoda-tk-0.1.9/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.9/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.9/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.1.9/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.9/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    22096 2023-07-30 10:19:37.000000 scoda-tk-0.1.9/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.1.9/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 11:59:25.513253 scoda-tk-0.1.9/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 11:59:25.000000 scoda-tk-0.1.9/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 11:59:25.000000 scoda-tk-0.1.9/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 11:59:25.000000 scoda-tk-0.1.9/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 11:59:25.000000 scoda-tk-0.1.9/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 11:59:25.000000 scoda-tk-0.1.9/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 11:59:25.000000 scoda-tk-0.1.9/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.2.0/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.2.0/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.2.0/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 12:21:43.000000 scoda-tk-0.2.0/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.2.0/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.674178 scoda-tk-0.2.0/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.682178 scoda-tk-0.2.0/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.2.0/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.2.0/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.698178 scoda-tk-0.2.0/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 09:42:12.000000 scoda-tk-0.2.0/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.2.0/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.2.0/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.2.0/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.2.0/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    22667 2023-07-30 12:21:39.000000 scoda-tk-0.2.0/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.2.0/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.1.9/LICENSE` & `scoda-tk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/PKG-INFO` & `scoda-tk-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.9
+Version: 0.2.0
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.9/pyproject.toml` & `scoda-tk-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.1.9"
+version = "0.2.0"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.1.9/src/scoda/cpdb.py` & `scoda-tk-0.2.0/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.2.0/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.2.0/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.2.0/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.2.0/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.2.0/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.2.0/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/deg.py` & `scoda-tk-0.2.0/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/gsea.py` & `scoda-tk-0.2.0/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/hicat.py` & `scoda-tk-0.2.0/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/icnv.py` & `scoda-tk-0.2.0/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/misc.py` & `scoda-tk-0.2.0/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda/pipeline.py` & `scoda-tk-0.2.0/src/scoda/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -482,31 +482,51 @@
         adata_t.uns['GSA_up'] = df_dct_dct_enr_up
         adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
     
     return
 
 
-def scoda_all_in_one( adata_t, df_mkr_db, gtf_file, cpdb_path, pw_db_for_gsea, 
-                      cond_col = 'condition', sample_col = 'sample', tumor_id_ref_celltypes = None, 
-                      unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
-                      cci_pval_max = 0.1, cci_mean_min = 0, Rth = 0.5, 
-                      deg_ref_group = None, deg_pval_cutoff = 0.01, min_n_cells_for_deg = 100, 
-                      n_cores_to_use = 4, data_dir = '.', verbose = True, prefix = 'CLIENT INFO: '):
-
+def scoda_all_in_one( adata_t, mkr_db, cnv_gtf, cpdb_path, gsea_pw_db, 
+                      cond_col = 'condition', sample_col = 'sample', 
+                      cnv_ref_list = None, cci_run_unit = 'sample', cci_n_cells_min = 40, 
+                      cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
+                      deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
+                      n_cores = 4, data_dir = '.', verbose = True, prefix = 'CLIENT INFO: '):
+
+    df_mkr_db = mkr_db
+    gtf_file = cnv_gtf 
+    # cpdb_path = , 
+    pw_db_for_gsea = gsea_pw_db 
+    # cond_col = 'condition' 
+    # sample_col = 'sample'
+    tumor_id_ref_celltypes = cnv_ref_list 
+    unit_of_cci_run = cci_run_unit 
+    min_n_cells_for_cci = cci_n_cells_min 
+    cci_pval_max = cci_pval_cutoff 
+    cci_mean_min = cci_mean_cutoff 
+    Rth = cci_rth 
+    deg_ref_group = deg_ref # None, 
+    # deg_pval_cutoff = 0.01, 
+    min_n_cells_for_deg = deg_n_cells_min 
+    n_cores_to_use = n_cores 
+    # data_dir = '.', 
+    # verbose = True, 
+    # prefix = 'CLIENT INFO: '
+    
     ################################
     ### Cell-type identification ###
 
     if verbose: print('%sCelltype annotation running .. ' % prefix)
         
     scoda_hicat(adata_t, df_mkr_db, verbose = False)
     
     if verbose: print('%sCelltype annotation done.' % prefix)
 
-    adata_t.write(file_h5ad)
+    # adata_t.write(file_h5ad)
       
     ## For client info.
     ct_lst_maj = list(adata_t.obs['celltype_major'].unique())
     ct_lst_min = list(adata_t.obs['celltype_minor'].unique())
     ct_lst_sub = list(adata_t.obs['celltype_subset'].unique())
 
     ct_lst_maj.sort()
@@ -529,39 +549,39 @@
         if verbose: print('%sIdentifying tumor cells .. ' % prefix)
         ref_types = tumor_id_ref_celltypes
 
         scoda_icnv_addon( adata_t, gtf_file, ref_types, 
                           ref_key = "celltype_major", n_cores = n_cores_to_use )
         
         if verbose: print('%sTumor cells identification done. ' % prefix)
-        adata_t.write(file_h5ad)
+        # adata_t.write(file_h5ad)
         
         
     #############################
     ### Cell-cell interaction ###
 
     if verbose: print('%sInfering cell-cell interactions .. ' % prefix)
 
     scoda_cci( adata_t, cpdb_path, cond_col = cond_col, sample_col = sample_col, 
                unit_of_cci_run = unit_of_cci_run, n_cores = n_cores_to_use, 
                min_n_cells_for_cci = min_n_cells_for_cci, Rth = Rth,
                pval_max = cci_pval_max, mean_min = cci_mean_min, data_dir = data_dir)
     
     if verbose: print('%sInfering cell-cell interactions done. ' % prefix)    
-    adata_t.write(file_h5ad)
+    # adata_t.write(file_h5ad)
         
     ####################
     ### DEG analysis ###
 
     if verbose: print('%sDEG/GSEA analysis ..       ' % prefix)
     scoda_deg_gsea( adata_t, pw_db = pw_db_for_gsea, 
                     cond_col = cond_col, sample_col = sample_col, 
                     ref_group = deg_ref_group, pval_cutoff = deg_pval_cutoff, 
                     N_cells_min_per_sample = min_n_cells_for_deg, 
                     N_cells_min_per_condition = min_n_cells_for_deg, 
                     n_cores = n_cores_to_use)
         
     ## Overwrite 
-    adata_t.write(file_h5ad)        
+    # adata_t.write(file_h5ad)        
     if verbose: print('%sDEG/GSEA analysis done.       ' % prefix)
         
     return
```

### Comparing `scoda-tk-0.1.9/src/scoda/viz.py` & `scoda-tk-0.2.0/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.9/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.2.0/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.9
+Version: 0.2.0
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.9/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.2.0/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

