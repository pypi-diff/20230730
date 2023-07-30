# Comparing `tmp/scoda-tk-0.2.0.tar.gz` & `tmp/scoda-tk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.2.0.tar", last modified: Sun Jul 30 12:22:12 2023, max compression
+gzip compressed data, was "scoda-tk-0.2.1.tar", last modified: Sun Jul 30 12:37:46 2023, max compression
```

## Comparing `scoda-tk-0.2.0.tar` & `scoda-tk-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.2.0/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.2.0/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.2.0/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 12:21:43.000000 scoda-tk-0.2.0/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.2.0/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.674178 scoda-tk-0.2.0/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.682178 scoda-tk-0.2.0/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.2.0/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.2.0/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.698178 scoda-tk-0.2.0/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.2.0/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 09:42:12.000000 scoda-tk-0.2.0/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.2.0/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.2.0/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.2.0/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.2.0/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    22667 2023-07-30 12:21:39.000000 scoda-tk-0.2.0/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.2.0/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:22:12.702178 scoda-tk-0.2.0/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 12:22:12.000000 scoda-tk-0.2.0/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.2.1/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.2.1/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.2.1/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 12:37:27.000000 scoda-tk-0.2.1/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.2.1/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.377102 scoda-tk-0.2.1/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.385102 scoda-tk-0.2.1/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.2.1/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.2.1/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.401102 scoda-tk-0.2.1/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 09:42:12.000000 scoda-tk-0.2.1/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.2.1/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.2.1/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.2.1/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.2.1/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    22679 2023-07-30 12:37:18.000000 scoda-tk-0.2.1/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.2.1/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.2.0/LICENSE` & `scoda-tk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/PKG-INFO` & `scoda-tk-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.0/pyproject.toml` & `scoda-tk-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.2.0"
+version = "0.2.1"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.2.0/src/scoda/cpdb.py` & `scoda-tk-0.2.1/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.2.1/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.2.1/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.2.1/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.2.1/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.2.1/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.2.1/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/deg.py` & `scoda-tk-0.2.1/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/gsea.py` & `scoda-tk-0.2.1/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/hicat.py` & `scoda-tk-0.2.1/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/icnv.py` & `scoda-tk-0.2.1/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/misc.py` & `scoda-tk-0.2.1/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda/pipeline.py` & `scoda-tk-0.2.1/src/scoda/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,17 +482,17 @@
         adata_t.uns['GSA_up'] = df_dct_dct_enr_up
         adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
     
     return
 
 
-def scoda_all_in_one( adata_t, mkr_db, cnv_gtf, cpdb_path, gsea_pw_db, 
-                      cond_col = 'condition', sample_col = 'sample', 
-                      cnv_ref_list = None, cci_run_unit = 'sample', cci_n_cells_min = 40, 
+def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
+                      cond_col = 'condition', sample_col = 'sample', cnv_ref_list = None,  
+                      cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
                       n_cores = 4, data_dir = '.', verbose = True, prefix = 'CLIENT INFO: '):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
@@ -539,15 +539,16 @@
         print('%s  %i major type, %i minor type, %i subset identified.' 
                % (prefix, len(ct_lst_maj), len(ct_lst_min), len(ct_lst_sub)))
         print('%s  Major types: %s' % (prefix, s))
         
     #################################
     ### tumor cell identification ###
     
-    if tumor_identification:
+    
+    if cnv_gtf is not None:
 
         ## Test without Reference 
         if verbose: print('%sIdentifying tumor cells .. ' % prefix)
         ref_types = tumor_id_ref_celltypes
 
         scoda_icnv_addon( adata_t, gtf_file, ref_types, 
                           ref_key = "celltype_major", n_cores = n_cores_to_use )
```

### Comparing `scoda-tk-0.2.0/src/scoda/viz.py` & `scoda-tk-0.2.1/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.0/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.2.1/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.0/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.2.1/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

