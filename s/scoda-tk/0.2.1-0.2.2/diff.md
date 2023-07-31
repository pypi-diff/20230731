# Comparing `tmp/scoda-tk-0.2.1.tar.gz` & `tmp/scoda-tk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.2.1.tar", last modified: Sun Jul 30 12:37:46 2023, max compression
+gzip compressed data, was "scoda-tk-0.2.2.tar", last modified: Mon Jul 31 05:16:59 2023, max compression
```

## Comparing `scoda-tk-0.2.1.tar` & `scoda-tk-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-29 11:43:39.000000 scoda-tk-0.2.1/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-29 11:43:39.000000 scoda-tk-0.2.1/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-29 11:43:51.000000 scoda-tk-0.2.1/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-30 12:37:27.000000 scoda-tk-0.2.1/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-29 11:43:39.000000 scoda-tk-0.2.1/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.377102 scoda-tk-0.2.1/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.385102 scoda-tk-0.2.1/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-29 11:43:49.000000 scoda-tk-0.2.1/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-29 11:43:42.000000 scoda-tk-0.2.1/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.401102 scoda-tk-0.2.1/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-29 11:43:44.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-29 11:43:44.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-29 11:43:45.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-29 11:43:43.000000 scoda-tk-0.2.1/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 09:42:12.000000 scoda-tk-0.2.1/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-29 16:25:48.000000 scoda-tk-0.2.1/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 06:58:42.000000 scoda-tk-0.2.1/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37098 2023-07-30 08:53:31.000000 scoda-tk-0.2.1/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-29 11:43:50.000000 scoda-tk-0.2.1/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    22679 2023-07-30 12:37:18.000000 scoda-tk-0.2.1/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-30 08:53:37.000000 scoda-tk-0.2.1/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-30 12:37:46.405102 scoda-tk-0.2.1/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-30 12:37:46.000000 scoda-tk-0.2.1/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.2/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-31 05:16:27.000000 scoda-tk-0.2.2/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.2/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.334592 scoda-tk-0.2.2/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.374591 scoda-tk-0.2.2/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.614586 scoda-tk-0.2.2/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    43161 2023-07-31 05:16:12.000000 scoda-tk-0.2.2/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23213 2023-07-31 05:16:08.000000 scoda-tk-0.2.2/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 05:16:15.000000 scoda-tk-0.2.2/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.2.1/LICENSE` & `scoda-tk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/PKG-INFO` & `scoda-tk-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.1/pyproject.toml` & `scoda-tk-0.2.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.2.1"
+version = "0.2.2"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.2.1/src/scoda/cpdb.py` & `scoda-tk-0.2.2/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.2.2/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.2.2/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.2.2/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.2.2/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.2.2/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.2.2/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/deg.py` & `scoda-tk-0.2.2/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/gsea.py` & `scoda-tk-0.2.2/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/hicat.py` & `scoda-tk-0.2.2/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/icnv.py` & `scoda-tk-0.2.2/src/scoda/icnv.py`

 * *Files 9% similar despite different names*

```diff
@@ -244,15 +244,18 @@
         if m == len(odr):
             m = m-1
         if m < 0: m = 0
         # print(' ns = %i -> m = %i' % (ns, m))
         th2 = cmeans[odr[m]]
         # th2 = cmeans.max()
         b2 = df['cmean'] <= th2
-        # b = b & b2
+        if np.sum(b&b2) == 0:
+            df2 = df.sort_values(by = 'cmean').iloc[:2]
+            th2 = df2['cmean'].max()
+            b2 = df['cmean'] <= th2
     
     ns = np.sum(~b)
     if ns > 0:
         cmeans = np.array(df.loc[~b,'cmean'])
         odr = cmeans.argsort()
 
         m = int(round(ns*(p_exc)))
@@ -269,19 +272,20 @@
     
     # print(th2, th3)
     
     w0 = np.sum(b&b2)/(len(b)*p_exc)
     m0 = df.loc[b&b2,'cmean'].mean()
     if np.sum(b&b2) > 1:
         v0 = df.loc[b&b2,'cmean'].var()
+    #'''
     else:
         idx = df.index.values[b&b2][0]
         bt = obs[cluster_key] == idx
         v0 = obs.loc[bt, score_key].var()
-        
+    #'''        
 
     for k, idx in enumerate(idx_lst):
         if df.loc[idx, 'cmean'] <= (m0 + np.sqrt(v0)):
             b[k] = True
                     
     if np.sum((~b)&b3) > 0:
         w1 = np.sum((~b)&b3)/(len(b)*p_exc)
@@ -802,14 +806,15 @@
     
     start_time = time.time()
     print('Running iCNV addon .. ', end = '', flush = True)
     
     if use_cnv_cluster:      
         y_clust = adata.obs[cluster_key].copy(deep = True)
         cnv_clust_lst = list(set(y_clust))
+        cobj = None
     else:
         # y_clust, cobj = clustering_alg(X_pca, clust_algo = 'lv', 
         #                                resolution = clustering_res, N_neighbors = n_neighbors)         
         adj = kneighbors_graph(X_pca, int(n_neighbors), mode='connectivity', include_self=True)
         etime = round(time.time() - start_time) 
         print('N(%i).' % etime, end = '', flush = True)
             
@@ -848,15 +853,36 @@
                 adata.obs['tumor_prob'+ suffix] = 0
                 adata.obs['tumor_dec'+ suffix] = 'NA'
                 adata.obs['tumor_cluster'+ suffix] = ''
                 return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
                           'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
             X_pca_sel = X_pca[b,:]
         else:
-            X_pca_sel = X_pca
+            
+            if cobj is None:
+                X_pca_sel = X_pca
+            else:
+                communities = detect_communities(X_pca, y_clust, cobj, pmaj = 0.7, 
+                                 cutoff = 0.01, verbose = False )
+                cluster_sel = merge_communities( communities )
+
+                if len(cluster_sel) > 0:
+                    b = y_clust == cluster_sel[0]
+                    for c in cluster_sel[1:]:
+                        b = b | (y_clust == c)
+                else:
+                    print('ERROR: No reference cell types found.')
+                    adata.obs[score_key] = 0
+                    adata.obs['tumor_prob'+ suffix] = 0
+                    adata.obs['tumor_dec'+ suffix] = 'NA'
+                    adata.obs['tumor_cluster'+ suffix] = ''
+                    return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
+                              'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+                
+                X_pca_sel = X_pca[b,:]
 
 
         etime = round(time.time() - start_time) 
         # print('C(%i).' % etime, end = '', flush = True)
 
         ## Get GMM model parameters
         gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
@@ -881,24 +907,26 @@
     ## Replace GMM scores with their cluster mean
     '''
     cnv_clust_lst = list(set(adata.obs[cluster_key]))
     for c in cnv_clust_lst:
         b = adata.obs[cluster_key] == c
         adata.obs.loc[b, score_key] = adata.obs.loc[b, score_key].mean()
     '''
-    if use_ref:
-        df, params = get_cnv_threshold_useref( adata.obs, ref_ind, 
-                                       score_key = score_key, cluster_key = cluster_key,
-                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
-                                       plot_stat = plot_stat, suffix = suffix, Data = Data )
+    # if use_ref:
+    df, params = get_cnv_threshold_useref( adata.obs, ref_ind, 
+                                   score_key = score_key, cluster_key = cluster_key,
+                                   th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
+                                   plot_stat = plot_stat, suffix = suffix, Data = Data )
+    '''
     else:
         df, params = get_cnv_threshold_bimodal( adata.obs, ref_ind, 
                                         score_key = score_key, cluster_key = cluster_key, 
                                         th_min = th_min, refp_min = refp_min, ucr = dec_margin,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
+    #'''
     
     etime = round(time.time() - start_time) 
     print(' .. done (%i) ' % etime) #, end = '', flush = True)
     
     return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
                       'tumor_prob'+suffix, 'tumor_cluster'+ suffix]], params
 
@@ -920,15 +948,15 @@
         # sc.tl.score_genes_cell_cycle(adata, cell_cycle_genes_s, cell_cycle_genes_g2m)
 
         cnv.io.genomic_position_from_gtf(gtf_file, adata, gtf_gene_id='gene_name', adata_gene_id=None, inplace=True)
         cnv.tl.infercnv(adata, reference_key = ref_key, reference_cat=ref_types, 
                         window_size=100, n_jobs = n_cores)
 
         print('PCA .. ', end = '')
-        cnv.tl.pca(adata, svd_solver='arpack', n_comps = N_pca) 
+        cnv.tl.pca(adata, n_comps = N_pca) 
         
         if umap:
             print('Finding neighbors .. ', end = '')
             cnv.pp.neighbors(adata, key_added = 'cnv_neighbors', n_neighbors=n_neighbors, n_pcs=N_pca)
             print('Clustering .. ', end = '')
             cnv.tl.leiden(adata, neighbors_key='cnv_neighbors', key_added=cluster_key, resolution = resolution)
             print('UMAP .. ', end = '')
@@ -1002,18 +1030,19 @@
         return cluster_label, km
     '''
 
 def detect_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
                        clust = None, Clustering_resolution = 1, N_clusters = 30,
                        # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                       dec_margin = 0.05, n_neighbors = 10, gcm = 0.05,
-                       plot_stat = False, use_ref = True, n_cores = 4,
-                       suffix = '', Data = None):
+                       dec_margin = 0.05, n_neighbors = 10, cmd_cutoff = 0.03, 
+                       gcm = 0.05, plot_stat = False, use_ref = False, 
+                       n_cores = 4, suffix = '', Data = None):
     
+    ref_addon = None
     score_key = 'tumor_score' + suffix
     cluster_key = 'cnv_cluster' 
     ## Get X_pca for ref_type cells
 
     start_time = time.time()
     start_time_a = start_time
     print('Running iCNV addon .. ', end = '', flush = True)
@@ -1033,30 +1062,34 @@
         etime = round(time.time() - start_time) 
         print('P(%i) .. ' % etime, end = '', flush = True)
         start_time = time.time()
            
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
-    if clust is not None:      
+    if (clust is not None) & (use_ref):      
         y_clust = list(clust)
         cobj = None
     else:
         y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
                                        resolution = Clustering_resolution, N_neighbors = n_neighbors, 
                                        n_cores = n_cores)
         
         etime = round(time.time() - start_time) 
         print('C(%i) .. ' % etime, end = '', flush = True)
         start_time = time.time()
     
     cnv_clust_lst = list(set(y_clust))
     df[cluster_key] = y_clust
         
-    if use_ref:
+    cluster_sel = None
+    
+    if ref_ind is not None: # use_ref:
+        b = ref_ind
+        #'''
         cnv_clust_lst.sort()
         b_inc = []
         for idx in cnv_clust_lst:
             b = y_clust == idx
             bt = b & ref_ind
             cnt = np.sum(bt)
 
@@ -1074,17 +1107,55 @@
             print('ERROR: No reference cell types found.')
             df[score_key] = 0
             df['tumor_prob'+ suffix] = 0
             df['tumor_dec'+ suffix] = 'NA'
             df['tumor_cluster'+ suffix] = ''
             return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
                       'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+        #'''
+        
+        X_pca_sel = X_pca[b,:]
+    # else:
+    
+    if (cobj is None) & (ref_ind is None):
+        y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
+                                       resolution = Clustering_resolution, N_neighbors = n_neighbors, 
+                                       n_cores = n_cores)
+        
+        etime = round(time.time() - start_time) 
+        print('C(%i) .. ' % etime, end = '', flush = True)
+        start_time = time.time()
+        
+    if (cobj is not None) & ((ref_ind is None) | (not use_ref)):
+        
+        communities = detect_communities(X_pca, y_clust, cobj, pmaj = 0.7, 
+                         cutoff = cmd_cutoff, verbose = False )
+        cluster_sel_addon = merge_communities( communities )
+        
+        if cluster_sel is None:
+            cluster_sel = cluster_sel_addon
+        else:
+            cluster_sel = list(set(cluster_sel).union(cluster_sel_addon))
+
+        if len(cluster_sel) > 0:
+            b = y_clust == cluster_sel[0]
+            if len(cluster_sel) > 1:
+                for c in cluster_sel[1:]:
+                    b = b | (y_clust == c)
+            ref_addon = b
+        else:
+            print('ERROR: No reference cell types found.')
+            adata.obs[score_key] = 0
+            adata.obs['tumor_prob'+ suffix] = 0
+            adata.obs['tumor_dec'+ suffix] = 'NA'
+            adata.obs['tumor_cluster'+ suffix] = ''
+            return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
+                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+
         X_pca_sel = X_pca[b,:]
-    else:
-        X_pca_sel = X_pca
 
     ## Get GMM model parameters
     gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
     gmm.fit(X_pca_sel)
     y_conf_gmm = -gmm.score_samples(X_pca)
     #'''
     y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
@@ -1092,29 +1163,126 @@
     yc = np.array(y_conf)
     odr = yc.argsort()
     n = int(len(yc)*0.975)
     ymax = yc[odr[n]]
     b = y_conf > ymax
     y_conf[b] = ymax
 
-    df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm*gcm)))
+    # df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm)))
+    df[score_key] = np.log(y_conf*(1/(1+np.exp(-y_conf_gmm*gcm)))) 
 
     etime = round(time.time() - start_time) 
     print('G(%i) .. ' % etime, end = '', flush = True)
     start_time = time.time()
     
     ## Replace GMM scores with their cluster mean
-    if ref_ind is not None:
-        dft, params = get_cnv_threshold_useref( df, ref_ind, 
+    #'''
+    if (ref_ind is not None):
+        #'''
+        if (ref_addon is not None):
+            ref_ind2 = ref_ind | ref_addon
+            print('N_ref: %i + %i -> %i .. ' % \
+                  (np.sum(ref_ind), np.sum(ref_addon), np.sum(ref_ind2)), end = '')
+        else:
+            #'''
+            ref_ind2 = ref_ind
+            print('N_ref: %i + X .. ' % (np.sum(ref_ind2)), end = '')
+    else:
+        ref_ind2 = ref_addon
+        print('N_ref: X + %i ..' % (np.sum(ref_ind2)), end = '')
+    #'''
+        
+    dft, params = get_cnv_threshold_useref( df, ref_ind2, 
                                        score_key = score_key, cluster_key = cluster_key,
-                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
-                                       plot_stat = plot_stat, suffix = suffix, Data = Data )
+                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, 
+                                       ucr = dec_margin, plot_stat = plot_stat, 
+                                       suffix = suffix, Data = Data )
+    '''
     else:
         dft, params = get_cnv_threshold_bimodal( df, ref_ind, 
                                         score_key = score_key, cluster_key = cluster_key, 
                                         th_min = th_min, refp_min = refp_min, ucr = dec_margin,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
+    #'''
     
     etime = round(time.time() - start_time_a) 
     print('done (%i) ' % etime) #, end = '', flush = True)
     
     return df, params, cobj
+
+
+def plot_td_stats( params, n_bins = 30, title = None, title_fs = 14,
+                   label_fs = 12, tick_fs = 11, legend_fs = 11, 
+                   legend_loc = 'upper left', bbox_to_anchor = (1, 1),
+                   figsize = (4,3), log = True, alpha = 0.8 ):
+    
+    th = params['th']
+    m0 = params['m0']
+    v0 = params['v0']
+    w0 = params['w0']
+    m1 = params['m1']
+    v1 = params['v1']
+    w1 = params['w1']
+    df = params['df']
+        
+    mxv = df['cmean'].max()
+    mnv = df['cmean'].min()
+    Dv = mxv - mnv
+    dv = Dv/200
+
+    x = np.arange(mnv,mxv,dv)
+    pdf0, xs0 = get_normal_pdf( x, m0, v0, 100)
+    pdf1, xs1 = get_normal_pdf( x, m1, v1, 100)
+    
+    pr = pdf1/(pdf1 + pdf0) # get_malignancy_prob( xs0, [w0, m0, v0, w1, m1, v1] )
+    bx = (xs0 >= m0) & ((xs1 <= m1))
+
+    nn = len(df['cmean'])
+    pdf0 = pdf0*(w0*nn*(200/n_bins)/pdf0.sum())
+    pdf1 = pdf1*(w1*nn*(200/n_bins)/(pdf1.sum())) 
+
+    max_pdf = max(pdf0.max(), pdf1.max())
+    
+    plt.figure(figsize = figsize)
+    ax = plt.gca()
+    
+    counts, bins = np.histogram(df['cmean'], bins = n_bins)
+    # max_cnt = np.max(counts)
+
+    legend_labels = []
+    
+    max_cnt = 0
+    b = df['dec'] == 'Normal'
+    if np.sum(b) > 0:
+        legend_labels.append('Normal')
+        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
+        max_cnt = max(max_cnt, np.max(counts))
+    b = df['dec'] == 'Tumor'
+    if np.sum(b) > 0:
+        legend_labels.append('Tumor')
+        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
+        max_cnt = max(max_cnt, np.max(counts))
+    b = df['dec'] == 'unclear'
+    if np.sum(b) > 0:
+        legend_labels.append('unclear')
+        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
+        max_cnt = max(max_cnt, np.max(counts))
+    
+    sf = 0.9*max_cnt/max_pdf
+    plt.plot(xs0, pdf0*sf)
+    plt.plot(xs1, pdf1*sf)
+    plt.plot([th, th], [0, max_cnt]) # max(pdf0.max()*sf, pdf1.max()*sf)])
+    plt.plot(xs0[bx], pr[bx]*max_cnt)
+
+    if title is not None: plt.title(title, fontsize = title_fs)
+    plt.xlabel('CNV_score', fontsize = label_fs)
+    plt.ylabel('Number of clusters', fontsize = label_fs)
+    plt.legend(['Normal distr.', 'Tumor distr.', 'Threshold', 'Tumor Prob.'], #, 'Score hist.'], 
+               loc = legend_loc, bbox_to_anchor = bbox_to_anchor, fontsize = legend_fs)
+    if log: plt.yscale('log')
+    ax.tick_params(axis='x', labelsize=tick_fs)
+    ax.tick_params(axis='y', labelsize=tick_fs)
+    plt.grid()
+    plt.show()
+        
+    return 
+
```

### Comparing `scoda-tk-0.2.1/src/scoda/misc.py` & `scoda-tk-0.2.2/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda/pipeline.py` & `scoda-tk-0.2.2/src/scoda/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,28 +80,29 @@
     mkr_info['subset_to_major_map'] = major_dict
     mkr_info['subset_to_minor_map'] = minor_dict
     adata.uns['Celltype_marker_DB'] = mkr_info
     
     return # adata
 
 
-def scoda_icnv_addon(adata_t, gtf_file, ref_types = None, ref_key = "celltype_major", n_cores = 4 ):
+def scoda_icnv_addon( adata_t, gtf_file, ref_types = None, 
+                      ref_key = "celltype_major", n_cores = 4,
+                      use_ref_only = False, cmd_cutoff = 0.03, 
+                      gcm = 0.05 ):
     
     adata = adata_t[:,:]
 
     ref_types2 = ref_types
     ref_ind = None
-    use_ref = False
 
     if ref_types is not None:
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
-                use_ref = True
     #'''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 2, N_pca = 15, n_neighbors = 10,
                      cluster_key = 'cnv_leiden', umap = False,
                      n_cores = n_cores )
 
     #'''
@@ -111,16 +112,16 @@
     X_cnv = adata.obsm['X_cnv_pca']
     pca = True
 
     df_res, params, cobj = detect_tumor_cells(X_cnv, ref_ind, pca = pca, 
                            use_cnv_score = False, clust = None, 
                            Clustering_resolution = 1, N_clusters = 30,
                            gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                           dec_margin = 0.1, n_neighbors = 15, gcm = 0.05,
-                           plot_stat = False, use_ref = use_ref, 
+                           dec_margin = 0.05, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
+                           gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
                            suffix = '', Data = None, n_cores = n_cores)
 
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
 
     # adata_t.obsm['X_cnv_umap'] = adata.obsm['X_cnv_umap']
     # adata_t.obs['cnv_leiden'] = adata.obs['cnv_leiden']
@@ -144,21 +145,22 @@
     lst2 = list(adata_t.obs.index.values)
     rend = dict(zip(lst1, lst2))
     df_res.rename(index = rend, inplace = True)
 
     adata_t.obsm['cnv_results'] = df_res[df_res.columns.values[:-1]] ## except tumor_cluster
 
     adata_t.obs['celltype_minor_rev'] = adata_t.obs['celltype_minor'].copy(deep = True).astype(str)
-    b = (adata_t.obs['tumor_dec'] == 'Tumor') & (~adata_t.obs['celltype_major'].isin(ref_types))
+    b = (adata_t.obs['tumor_dec'] == 'Tumor')
+    if ref_types is not None:
+        b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
     return
 
 
-
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
                data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4 ):
     
     if 'celltype_minor_rev' in list(adata_t.obs.columns.values):
         celltype_col = 'celltype_minor_rev'
     else:
@@ -483,16 +485,17 @@
         adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
     
     return
 
 
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
-                      cond_col = 'condition', sample_col = 'sample', cnv_ref_list = None,  
-                      cci_run_unit = 'sample', cci_n_cells_min = 40, 
+                      cond_col = 'condition', sample_col = 'sample', 
+                      cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
+                      cnv_gcm = 0.05, cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
                       n_cores = 4, data_dir = '.', verbose = True, prefix = 'CLIENT INFO: '):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
@@ -545,17 +548,22 @@
     
     
     if cnv_gtf is not None:
 
         ## Test without Reference 
         if verbose: print('%sIdentifying tumor cells .. ' % prefix)
         ref_types = tumor_id_ref_celltypes
-
+        '''
         scoda_icnv_addon( adata_t, gtf_file, ref_types, 
                           ref_key = "celltype_major", n_cores = n_cores_to_use )
+        #'''
+        scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
+                          ref_key = "celltype_major", n_cores = n_cores_to_use,
+                          use_ref_only = cnv_use_ref_only, cmd_cutoff = cnv_cmd_cutoff,
+                          gcm = cnv_gcm )
         
         if verbose: print('%sTumor cells identification done. ' % prefix)
         # adata_t.write(file_h5ad)
         
         
     #############################
     ### Cell-cell interaction ###
```

### Comparing `scoda-tk-0.2.1/src/scoda/viz.py` & `scoda-tk-0.2.2/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.1/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.2.2/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.1/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.2.2/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

