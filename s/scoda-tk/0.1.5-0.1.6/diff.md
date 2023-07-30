# Comparing `tmp/scoda-tk-0.1.5.tar.gz` & `tmp/scoda-tk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.1.5.tar", last modified: Sun Jul 30 08:54:15 2023, max compression
+gzip compressed data, was "scoda-tk-0.1.6.tar", last modified: Sun Jul 30 09:03:51 2023, max compression
```

## Comparing `scoda-tk-0.1.5.tar` & `scoda-tk-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.092862 scoda-tk-0.1.5/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.5/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.5/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 08:54:15.088862 scoda-tk-0.1.5/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.5/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 08:54:02.000000 scoda-tk-0.1.5/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 08:54:15.092862 scoda-tk-0.1.5/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.5/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.060862 scoda-tk-0.1.5/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.064862 scoda-tk-0.1.5/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.5/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.5/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.088862 scoda-tk-0.1.5/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    16728 2023-07-30 08:53:26.000000 scoda-tk-0.1.5/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.5/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.5/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.1.5/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.5/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18898 2023-07-30 08:53:23.000000 scoda-tk-0.1.5/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.1.5/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.088862 scoda-tk-0.1.5/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.6/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.6/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.6/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 09:03:34.000000 scoda-tk-0.1.6/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.6/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.267010 scoda-tk-0.1.6/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.267010 scoda-tk-0.1.6/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.6/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.6/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.6/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    16728 2023-07-30 08:53:26.000000 scoda-tk-0.1.6/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.6/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.6/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.1.6/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.6/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18987 2023-07-30 09:03:26.000000 scoda-tk-0.1.6/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.1.6/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 09:03:51.287009 scoda-tk-0.1.6/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 09:03:51.000000 scoda-tk-0.1.6/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.1.5/LICENSE` & `scoda-tk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/PKG-INFO` & `scoda-tk-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.5/pyproject.toml` & `scoda-tk-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.1.5"
+version = "0.1.6"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.1.5/src/scoda/cpdb.py` & `scoda-tk-0.1.6/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.1.6/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.1.6/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.1.6/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.1.6/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.1.6/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.1.6/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/deg.py` & `scoda-tk-0.1.6/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/gsea.py` & `scoda-tk-0.1.6/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/hicat.py` & `scoda-tk-0.1.6/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/icnv.py` & `scoda-tk-0.1.6/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/misc.py` & `scoda-tk-0.1.6/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda/pipeline.py` & `scoda-tk-0.1.6/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     mkr_info['subset_to_major_map'] = major_dict
     mkr_info['subset_to_minor_map'] = minor_dict
     adata.uns['Celltype_marker_DB'] = mkr_info
     
     return # adata
 
 
-def scoda_icnv_addon(adata_t, gtf_file, ref_types = None, ref_key = "celltype_major"):
+def scoda_icnv_addon(adata_t, gtf_file, ref_types = None, ref_key = "celltype_major", n_cores = 4 ):
     
     adata = adata_t[:,:]
 
     ref_types2 = ref_types
     ref_ind = None
     use_ref = False
 
@@ -98,30 +98,30 @@
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
                 use_ref = True
     #'''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 2, N_pca = 15, n_neighbors = 10,
                      cluster_key = 'cnv_leiden', umap = False,
-                     n_cores = n_cores_to_use )
+                     n_cores = n_cores )
 
     #'''
     # X_cnv = adata.obsm['X_cnv'].todense()
     # pca = False
 
     X_cnv = adata.obsm['X_cnv_pca']
     pca = True
 
     df_res, params, cobj = detect_tumor_cells(X_cnv, ref_ind, pca = pca, 
                            use_cnv_score = False, clust = None, 
                            Clustering_resolution = 1, N_clusters = 30,
                            gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                            dec_margin = 0.1, n_neighbors = 15, gcm = 0.05,
                            plot_stat = False, use_ref = use_ref, 
-                           suffix = '', Data = None, n_cores = 6)
+                           suffix = '', Data = None, n_cores = n_cores)
 
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
 
     # adata_t.obsm['X_cnv_umap'] = adata.obsm['X_cnv_umap']
     # adata_t.obs['cnv_leiden'] = adata.obs['cnv_leiden']
     # adata_t.obs['cnv_score'] = adata.obs['cnv_score']
@@ -152,15 +152,16 @@
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
     return
 
 
 
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
-               unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, data_dir = '.'):
+               unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
+               data_dir = '.', n_cores = 4 ):
     
     if 'celltype_minor_rev' in list(adata_t.obs.columns.values):
         celltype_col = 'celltype_minor_rev'
     else:
         celltype_col = 'celltype_minor'
 
     if cond_col not in list(adata_t.obs.columns.values):
@@ -209,15 +210,15 @@
         b1 = adata_t.obs[t_col] == s
         b2 = adata_t.obs[celltype_col].isin(celltype_lst)
         b = b1 & b2
         adata_s = adata_t[b,:]
         celltype = adata_s.obs[celltype_col]
 
         df_mn, df_pv = cpdb4_run( adata_s, celltype, db = cpdb_path,
-                                  out_dir = out_dir, n_cores = n_cores_to_use,
+                                  out_dir = out_dir, n_cores = n_cores,
                                   threshold = 0.05, gene_id_type = 'gene_name' )
 
         dfi, dfp, dfm, dfv = cpdb4_get_results( df_pv, df_mn, 
                                                 pval_max = 0.05, mean_min = 0.01 )
 
         dfv_dct[s] = dfv
     ## End for
@@ -314,15 +315,16 @@
         
     return
 
 
 def scoda_deg_gsea( adata_t, pw_db, 
                     cond_col = 'condition', sample_col = 'sample', 
                     ref_group = None, pval_cutoff = 0.05,
-                    N_cells_min_per_sample = 100, N_cells_min_per_condition = 100): 
+                    N_cells_min_per_sample = 100, 
+                    N_cells_min_per_condition = 100, n_cores = 4): 
         
     # ref_group_for_deg = ref_group
     ref_group_for_deg = None
     if ref_group is not None:
         if ref_group in list(adata_t.obs[cond_col].unique()):
             ref_group_for_deg = ref_group    
     
@@ -457,15 +459,15 @@
                     if df_res_enr_neg is not None:
                         df_lst_enrichr_dn[c] = df_res_enr_neg
 
                     ## Run gseapy.prerank
                     logfc = gene_rank[[log_fc_col]] ## index must be gene name
 
                     df_res_pr, pr_res = run_prerank(logfc, pw_db_sel, pval_max = 0.1, # pval_cutoff,
-                                        min_size = min_size, max_size = max_size )
+                                        min_size = min_size, max_size = max_size, n_cores = n_cores )
                     
                     # df_res_pr.drop(columns = ['Tag %', 'Gene %'], inplace = True)
                     if df_res_pr.shape[0] > 0:
                         df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']] = \
                             df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']].astype(float)
                         df_lst_prerank[c] = df_res_pr
```

### Comparing `scoda-tk-0.1.5/src/scoda/viz.py` & `scoda-tk-0.1.6/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.5/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.1.6/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.5/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.1.6/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

