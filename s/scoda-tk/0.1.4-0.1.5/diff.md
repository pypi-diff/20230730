# Comparing `tmp/scoda-tk-0.1.4.tar.gz` & `tmp/scoda-tk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.1.4.tar", last modified: Sun Jul 30 07:07:44 2023, max compression
+gzip compressed data, was "scoda-tk-0.1.5.tar", last modified: Sun Jul 30 08:54:15 2023, max compression
```

## Comparing `scoda-tk-0.1.4.tar` & `scoda-tk-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.4/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.4/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.4/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 07:03:31.000000 scoda-tk-0.1.4/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.4/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.724121 scoda-tk-0.1.4/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.728121 scoda-tk-0.1.4/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.4/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.4/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.4/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    16244 2023-07-29 16:28:13.000000 scoda-tk-0.1.4/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.4/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.4/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 06:58:11.000000 scoda-tk-0.1.4/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.4/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17988 2023-07-30 07:07:12.000000 scoda-tk-0.1.4/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    57779 2023-07-30 07:03:21.000000 scoda-tk-0.1.4/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 07:07:44.748120 scoda-tk-0.1.4/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 07:07:44.000000 scoda-tk-0.1.4/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.092862 scoda-tk-0.1.5/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.1.5/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.1.5/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 08:54:15.088862 scoda-tk-0.1.5/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.1.5/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 08:54:02.000000 scoda-tk-0.1.5/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 08:54:15.092862 scoda-tk-0.1.5/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.1.5/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.060862 scoda-tk-0.1.5/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.064862 scoda-tk-0.1.5/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.1.5/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.1.5/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.088862 scoda-tk-0.1.5/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.1.5/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    16728 2023-07-30 08:53:26.000000 scoda-tk-0.1.5/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.1.5/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.1.5/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.1.5/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.1.5/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18898 2023-07-30 08:53:23.000000 scoda-tk-0.1.5/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.1.5/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 08:54:15.088862 scoda-tk-0.1.5/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 08:54:15.000000 scoda-tk-0.1.5/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.1.4/LICENSE` & `scoda-tk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/PKG-INFO` & `scoda-tk-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.4/pyproject.toml` & `scoda-tk-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.1.4"
+version = "0.1.5"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.1.4/src/scoda/cpdb.py` & `scoda-tk-0.1.5/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.1.5/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.1.5/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.1.5/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.1.5/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.1.5/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.1.5/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/deg.py` & `scoda-tk-0.1.5/src/scoda/deg.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,15 @@
     glst = list(set(list(groups_in)))
     glst.sort()
     
     if not isinstance(groups_in, pd.Series):
         groups_in = pd.Series(groups_in, index = df_cbyg_in.index.values)
 
     df_lst = {}
+    n_cells_lst = {}
     for g in glst:
 
         if (ref_group is None):
             groups = groups_in.copy(deep = True).astype(str)
             ref_g = 'others'
             b = groups != g
             groups[b] = ref_group
@@ -360,27 +361,30 @@
                 df_cbyg = df_cbyg_in
             else:
                 ref_g = ref_group
                 b = groups_in.isin([g, ref_group])
                 groups = groups_in[b]
                 df_cbyg = df_cbyg_in.loc[b,:]
 
+        n_cells_info = {g: np.sum(~b), ref_g: np.sum(b)}
+                
         df_deg = perform_deg( df_cbyg, groups, target_group = g, 
                               min_ef = min_ef, exp_only = exp_only )
         key = '%s_vs_%s' % (g, ref_g)
         df_lst[key] = df_deg
+        n_cells_lst[key] = n_cells_info
 
         if samples_in is not None:
             if len(samples_in) == df_cbyg_in.shape[0]:
                 b = groups_in == g
                 dft = find_fraction_of_patients_for_vaild_marker_exp( df_lst[key], 
                             df_cbyg_in.loc[b,:], pids = samples_in[b], min_frac = min_frac )
                 df_lst[key]['Rp'] = dft['Rp'] 
         
-    return df_lst
+    return df_lst, n_cells_lst
 
 
 def find_fraction_of_patients_for_vaild_marker_exp( df_deg, df_cbyg, pids, min_frac = 0.1 ):
     
     dft = pd.DataFrame(index = df_deg.index) 
     dft['Rp'] = 0
     X = df_cbyg
@@ -412,21 +416,22 @@
         df_lst[key]['Rp'] = dft['Rp'] 
 
     return df_lst
 
 
 def plot_deg( df_deg_dct, value = 'log2_FC', n_genes = 30, pval_cutoff = 0.05, 
               figsize = (6,4), text_fs = 10, title_fs = 12, label_fs = 11, 
-              tick_fs = 10, ncol = 2, ws_hs = (0.15, 0.2) ):
+              tick_fs = 10, ncol = 2, ws_hs = (0.15, 0.2), deg_stat_dct = None ):
 
     nr, nc = int(np.ceil(len(df_deg_dct.keys())/ncol)), int(ncol) # len(df_deg_dct.keys())
     fig, axes = plt.subplots(figsize = (figsize[0]*nc,figsize[1]*nr), nrows=nr, ncols=nc, # constrained_layout=True, 
                              gridspec_kw={'width_ratios': [1]*nc})
     fig.tight_layout() 
-    plt.subplots_adjust(left=0.05, bottom=0.05, right=0.95, top=0.95, wspace=0.15, hspace=0.2)
+    plt.subplots_adjust(left=0.05, bottom=0.05, right=0.95, top=0.95, 
+                        wspace=ws_hs[0], hspace=ws_hs[1])
 
     for j, key in enumerate(df_deg_dct.keys()):
         b = df_deg_dct[key]['pval_adj'] <= pval_cutoff
         dfs = df_deg_dct[key].loc[b,:].sort_values(value, ascending = False)
         dfs = dfs.iloc[:min(n_genes, np.sum(b))]
 
         plt.subplot(nr,nc,j+1)
@@ -437,15 +442,23 @@
         m = (np.max(Y)-np.min(Y))
         plt.ylim([np.min(Y)-m*0.4, np.max(Y) + m*0.5])
         tlst = list(dfs.index.values)
         for x, y, t in zip(X, Y, tlst):
             plt.text(x, y, '  %s' % (t), rotation = 90, fontsize = text_fs)
             lpv =  -np.log10(dfs.loc[t,'pval_adj'])
             plt.text(x, y, '(%3.1f) ' % (lpv), rotation = 90, va = 'top', fontsize = text_fs)
-        plt.title(key, fontsize = title_fs)
+        if deg_stat_dct is None:
+            plt.title(key, fontsize = title_fs)
+        else:
+            s = ' ('
+            for kk in deg_stat_dct[key].keys():
+                s = s + '%s: %i, ' % (kk, deg_stat_dct[key][kk])
+            s = '%s)' % s[:-2]
+            plt.title(key + s, fontsize = title_fs)
+            
         plt.xlabel('Genes', fontsize = label_fs)
         plt.yticks(fontsize=tick_fs)
         plt.xticks(fontsize=tick_fs)
         if j%nc == 0: plt.ylabel(value, fontsize = label_fs)
         plt.grid('on')
 
     if nc*nr > len(df_deg_dct.keys()):
```

### Comparing `scoda-tk-0.1.4/src/scoda/gsea.py` & `scoda-tk-0.1.5/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/hicat.py` & `scoda-tk-0.1.5/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/icnv.py` & `scoda-tk-0.1.5/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/misc.py` & `scoda-tk-0.1.5/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.1.4/src/scoda/pipeline.py` & `scoda-tk-0.1.5/src/scoda/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 from scoda.deg import deg_multi, get_population, plot_population
 from scoda.misc import plot_sankey_e, get_opt_files_path
 
 from scoda.hicat import HiCAT, show_summary, get_markers_major_type
 from scoda.hicat import get_markers_cell_type, get_markers_minor_type2, load_markers_all
 
 
-def scoda_hicat(adata, df_mkr_db, verbose = False):
+def scoda_hicat(adata, mkr_db, verbose = False):
     
     X1 = adata.to_df()
     
     PNSH12 = '100000'
     target_tissues = []
     target_cell_types = []
     # target_cell_types = ['T cell', 'B cell', 'Myeloid cell', 'Fibroblast',
     #                      'Epithelial cell', 'Endothelial cell', 'Mast cell', 
     #                      'Smooth muscle cell', 'Granulocyte'] 
     to_exclude = [] 
 
     df_pred, summary = \
-        HiCAT( X1, df_mkr_db, log_transformed = False,
+        HiCAT( X1, mkr_db, log_transformed = False,
                target_tissues = target_tissues, target_cell_types = target_cell_types, 
                minor_types_to_exclude = to_exclude, mkr_selector = PNSH12, 
                N_neighbors_minor = 31, N_neighbors_subset = 1,  
                Clustering_algo = 'lv', Clustering_resolution = 1, 
                Clustering_base = 'pca', N_pca_components = 15, 
                cycling_cell = False, copy_X = False, verbose = verbose,
                model = 'gmm', N_gmm_components = 20, cbc_cutoff = 0.01,
@@ -56,35 +56,39 @@
     adata.obs['celltype_major'] = df_pred['cell_type_major']
     adata.obs['celltype_minor'] = df_pred['cell_type_minor']
     adata.obs['celltype_subset'] = df_pred['cell_type_subset']
 
     adata.obsm['HiCAT_result'] = df_pred
     
     ## Store marker info.
-    mkr_dict, mkr_dict_neg, mkr_dict_sec, major_dict, minor_dict = load_markers_all(mkr_file, target_cells = [], 
+    mkr_dict, mkr_dict_neg, mkr_dict_sec, major_dict, minor_dict = load_markers_all(mkr_db, target_cells = [], 
                                                                                  pnsh12 = '111000', 
                                                                                  comb_mkrs = False)
     #'''
     mkr_dict, mkr_dict_neg = \
-    get_markers_minor_type2(mkr_file, target_cells = [], 
+    get_markers_minor_type2(mkr_db, target_cells = [], 
                             pnsh12 = '100000', comb_mkrs = False, 
                             rem_common = False, verbose = False)
     #'''
 
     mkr_info = {}
-    mkr_info['marker_db'] = df_mkr_db
+    if isinstance(mkr_db, pd.DataFrame):
+        mkr_info['marker_db'] = mkr_db
+    elif isinstance(mkr_db, str):
+        mkr_info['marker_db'] = pd.read_csv(mkr_db, sep = '\t')
+        
     mkr_info['subset_markers_dict'] = mkr_dict
     mkr_info['subset_to_major_map'] = major_dict
     mkr_info['subset_to_minor_map'] = minor_dict
     adata.uns['Celltype_marker_DB'] = mkr_info
     
     return # adata
 
 
-def scoda_icnv_addon(adata_t, ref_types = None, ref_key = "celltype_major"):
+def scoda_icnv_addon(adata_t, gtf_file, ref_types = None, ref_key = "celltype_major"):
     
     adata = adata_t[:,:]
 
     ref_types2 = ref_types
     ref_ind = None
     use_ref = False
 
@@ -147,15 +151,15 @@
     b = (adata_t.obs['tumor_dec'] == 'Tumor') & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
     return
 
 
 
-def scoda_cci( adata_t, cond_col = 'condition', sample_col = 'sample', 
+def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, data_dir = '.'):
     
     if 'celltype_minor_rev' in list(adata_t.obs.columns.values):
         celltype_col = 'celltype_minor_rev'
     else:
         celltype_col = 'celltype_minor'
 
@@ -204,15 +208,15 @@
         
         b1 = adata_t.obs[t_col] == s
         b2 = adata_t.obs[celltype_col].isin(celltype_lst)
         b = b1 & b2
         adata_s = adata_t[b,:]
         celltype = adata_s.obs[celltype_col]
 
-        df_mn, df_pv = cpdb4_run( adata_s, celltype, db = cellphone_db,
+        df_mn, df_pv = cpdb4_run( adata_s, celltype, db = cpdb_path,
                                   out_dir = out_dir, n_cores = n_cores_to_use,
                                   threshold = 0.05, gene_id_type = 'gene_name' )
 
         dfi, dfp, dfm, dfv = cpdb4_get_results( df_pv, df_mn, 
                                                 pval_max = 0.05, mean_min = 0.01 )
 
         dfv_dct[s] = dfv
@@ -355,16 +359,19 @@
         sc.pp.normalize_total(adata, target_sum=1e4)
         sc.pp.log1p(adata)
 
         cond_lst = list(adata.obs[cond_col].unique())
         celltype_lst = list(adata.obs[celltype_col].unique()) 
         genes_all = list(adata.var.index.values)
 
+        df_dct_dct_n_cells = {}
         df_dct_dct_deg = {}
         df_dct_dct_enr = {}
+        df_dct_dct_enr_up = {}
+        df_dct_dct_enr_dn = {}
         df_dct_dct_pr = {}
         
         if 'unassigned' in celltype_lst:
             celltype_lst = list(set(celltype_lst) - {'unassigned'})
         celltype_lst.sort()
         
         ref_group_for_deg = None
@@ -398,70 +405,83 @@
 
                 df_cbyg_in = adata_s.to_df()
                 groups_in = adata_s.obs[cond_col]
                 samples_in = adata_s.obs.index.values
 
                 ref_group = ref_group_for_deg
 
-                df_lst = deg_multi( df_cbyg_in, groups_in, ref_group = ref_group, 
+                df_lst, nc_lst = deg_multi( df_cbyg_in, groups_in, ref_group = ref_group, 
                                     samples_in = samples_in, min_ef = 0.05, 
                                     exp_only = False, min_frac = 0.05 )
                 df_dct_dct_deg[ct] = df_lst
+                df_dct_dct_n_cells[ct] = nc_lst
 
                 ## Run gseapy.prerank
                 df_lst_enrichr = {}
+                df_lst_enrichr_up = {}
+                df_lst_enrichr_dn = {}
                 df_lst_prerank = {}
                 #'''
                 for c in df_lst.keys():
                     gene_rank = df_lst[c].copy(deep = True)
                     gene_rank[gene_col] = list(gene_rank.index.values)
 
                     ## Run gseapy.enrichr
                     df_res_enr_pos = None
                     b = gene_rank[log_fc_col] > 0
                     if np.sum(b) > 0:
                         df_res_enr_pos = run_enrich(gene_rank.loc[b,gene_col], pw_db_sel, genes_all, pval_max = pval_cutoff)
-                        df_res_enr_pos['NES'] = 1
+                        df_res_enr_pos['Ind'] = 1
                         # if verbose: print('  Num. of selected pathways in Enrichr (+): ', df_res_enr_pos.shape[0])
 
                     df_res_enr_neg = None
                     b = gene_rank[log_fc_col] < 0
                     if np.sum(b) > 0:
                         df_res_enr_neg = run_enrich(gene_rank.loc[b,gene_col], pw_db_sel, genes_all, pval_max = pval_cutoff)
-                        df_res_enr_neg['NES'] = -1
+                        df_res_enr_neg['Ind'] = -1
                         # if verbose: print('  Num. of selected pathways in Enrichr (-): ', df_res_enr_neg.shape[0])
 
                     if (df_res_enr_pos is not None) & (df_res_enr_neg is not None):
                         df_res_enr = pd.concat([df_res_enr_pos, df_res_enr_neg], axis = 0)
                     elif (df_res_enr_pos is not None):
                         df_res_enr = df_res_enr_pos
                     elif (df_res_enr_neg is not None):
                         df_res_enr = df_res_enr_neg
                     else:
                         df_res_enr = None
                         
                     if df_res_enr is not None:
                         df_lst_enrichr[c] = df_res_enr
+                        
+                    if df_res_enr_pos is not None:
+                        df_lst_enrichr_up[c] = df_res_enr_pos
+                    if df_res_enr_neg is not None:
+                        df_lst_enrichr_dn[c] = df_res_enr_neg
 
                     ## Run gseapy.prerank
                     logfc = gene_rank[[log_fc_col]] ## index must be gene name
 
                     df_res_pr, pr_res = run_prerank(logfc, pw_db_sel, pval_max = 0.1, # pval_cutoff,
                                         min_size = min_size, max_size = max_size )
                     
                     # df_res_pr.drop(columns = ['Tag %', 'Gene %'], inplace = True)
                     if df_res_pr.shape[0] > 0:
                         df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']] = \
                             df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']].astype(float)
                         df_lst_prerank[c] = df_res_pr                        
 
+                df_dct_dct_enr_up[ct] = df_lst_enrichr_up
+                df_dct_dct_enr_dn[ct] = df_lst_enrichr_dn
                 df_dct_dct_enr[ct] = df_lst_enrichr
                 df_dct_dct_pr[ct] = df_lst_prerank
                 # '''
 
         print('CLIENT INFO: DEG/GSEA analysis done.       ')
 
+        adata_t.uns['DEG_stat'] = df_dct_dct_n_cells
         adata_t.uns['DEG'] = df_dct_dct_deg
-        adata_t.uns['GSA'] = df_dct_dct_enr
+        # adata_t.uns['GSA'] = df_dct_dct_enr
+        adata_t.uns['GSA_up'] = df_dct_dct_enr_up
+        adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
     
-    return
+    return
```

### Comparing `scoda-tk-0.1.4/src/scoda/viz.py` & `scoda-tk-0.1.5/src/scoda/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1625,19 +1625,19 @@
             ax.set_xticklabels(ylabels)
             ax.yaxis.set_ticks_position('left')
             ax.set_yticks( ticks = list(np.arange(len(categ_order))+0.5))
             ax.set_yticklabels(categ_order)
                 
     plt.show()
     return pe_lst, pex_lst, mkrs_dict
-    
+        
     
 def plot_deg( df_deg_dct, value = 'log2_FC', n_genes = 30, pval_cutoff = 0.05, 
               figsize = (6,4), text_fs = 10, title_fs = 12, label_fs = 11, 
-              tick_fs = 10, ncol = 2, ws_hs = (0.15, 0.2) ):
+              tick_fs = 10, ncol = 2, ws_hs = (0.15, 0.2), deg_stat_dct = None ):
 
     nr, nc = int(np.ceil(len(df_deg_dct.keys())/ncol)), int(ncol) # len(df_deg_dct.keys())
     fig, axes = plt.subplots(figsize = (figsize[0]*nc,figsize[1]*nr), nrows=nr, ncols=nc, # constrained_layout=True, 
                              gridspec_kw={'width_ratios': [1]*nc})
     fig.tight_layout() 
     plt.subplots_adjust(left=0.05, bottom=0.05, right=0.95, top=0.95, 
                         wspace=ws_hs[0], hspace=ws_hs[1])
@@ -1655,15 +1655,23 @@
         m = (np.max(Y)-np.min(Y))
         plt.ylim([np.min(Y)-m*0.4, np.max(Y) + m*0.5])
         tlst = list(dfs.index.values)
         for x, y, t in zip(X, Y, tlst):
             plt.text(x, y, '  %s' % (t), rotation = 90, fontsize = text_fs)
             lpv =  -np.log10(dfs.loc[t,'pval_adj'])
             plt.text(x, y, '(%3.1f) ' % (lpv), rotation = 90, va = 'top', fontsize = text_fs)
-        plt.title(key, fontsize = title_fs)
+        if deg_stat_dct is None:
+            plt.title(key, fontsize = title_fs)
+        else:
+            s = ' ('
+            for kk in deg_stat_dct[key].keys():
+                s = s + '%s: %i, ' % (kk, deg_stat_dct[key][kk])
+            s = '%s)' % s[:-2]
+            plt.title(key + s, fontsize = title_fs)
+            
         plt.xlabel('Genes', fontsize = label_fs)
         plt.yticks(fontsize=tick_fs)
         plt.xticks(fontsize=tick_fs)
         if j%nc == 0: plt.ylabel(value, fontsize = label_fs)
         plt.grid('on')
 
     if nc*nr > len(df_deg_dct.keys()):
```

### Comparing `scoda-tk-0.1.4/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.1.5/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.1.4/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.1.5/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

