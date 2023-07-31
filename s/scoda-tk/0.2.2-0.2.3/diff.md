# Comparing `tmp/scoda-tk-0.2.2.tar.gz` & `tmp/scoda-tk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.2.2.tar", last modified: Mon Jul 31 05:16:59 2023, max compression
+gzip compressed data, was "scoda-tk-0.2.3.tar", last modified: Mon Jul 31 13:01:40 2023, max compression
```

## Comparing `scoda-tk-0.2.2.tar` & `scoda-tk-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.2/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-31 05:16:27.000000 scoda-tk-0.2.2/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.2/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.334592 scoda-tk-0.2.2/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.374591 scoda-tk-0.2.2/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.614586 scoda-tk-0.2.2/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.2/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.2/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    43161 2023-07-31 05:16:12.000000 scoda-tk-0.2.2/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.2/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23213 2023-07-31 05:16:08.000000 scoda-tk-0.2.2/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 05:16:15.000000 scoda-tk-0.2.2/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 05:16:59.622586 scoda-tk-0.2.2/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-31 05:16:59.000000 scoda-tk-0.2.2/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.3/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-31 13:01:22.000000 scoda-tk-0.2.3/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.3/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:39.988677 scoda-tk-0.2.3/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.012676 scoda-tk-0.2.3/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.160673 scoda-tk-0.2.3/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    43161 2023-07-31 13:01:09.000000 scoda-tk-0.2.3/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23351 2023-07-31 13:01:06.000000 scoda-tk-0.2.3/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 13:01:13.000000 scoda-tk-0.2.3/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.2.2/LICENSE` & `scoda-tk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/PKG-INFO` & `scoda-tk-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.2/pyproject.toml` & `scoda-tk-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.2.2"
+version = "0.2.3"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.2.2/src/scoda/cpdb.py` & `scoda-tk-0.2.3/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.2.3/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.2.3/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.2.3/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.2.3/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.2.3/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.2.3/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/deg.py` & `scoda-tk-0.2.3/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/gsea.py` & `scoda-tk-0.2.3/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/hicat.py` & `scoda-tk-0.2.3/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/icnv.py` & `scoda-tk-0.2.3/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/misc.py` & `scoda-tk-0.2.3/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda/pipeline.py` & `scoda-tk-0.2.3/src/scoda/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,41 +155,42 @@
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
     return
 
 
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
-               data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4 ):
+               data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4,
+               print_prefix = ''):
     
     if 'celltype_minor_rev' in list(adata_t.obs.columns.values):
         celltype_col = 'celltype_minor_rev'
     else:
         celltype_col = 'celltype_minor'
 
     if cond_col not in list(adata_t.obs.columns.values):
         adata_t.obs[cond_col] = 'Not specified'
-        print('WARNING in SCODA_CCI: \'condition\' column not specified. Will be set as \'unspecied\'')        
+        print('%sin SCODA_CCI: \'condition\' column not specified. Will be set as \'unspecied\'' % print_prefix)        
     cond_lst = list(adata_t.obs[cond_col].unique())
     
     if sample_col not in list(adata_t.obs.columns.values):
         adata_t.obs[sample_col] = 'Not specified'
-        print('WARNING in SCODA_CCI: \'sample\' column not specified. Will be set as \'unspecied\'')
+        print('%sin SCODA_CCI: \'sample\' column not specified. Will be set as \'unspecied\'' % print_prefix)
     sample_lst = list(adata_t.obs[sample_col].unique())
 
     # print(cond_lst)
     # print(sample_lst)
     t_col = cond_col
     t_lst = cond_lst
     
     if unit_of_cci_run == 'sample':
         t_col = sample_col
         t_lst = sample_lst
     else:
-        print('INFO in SCODA_CCI: Unit of CCI RUN is \'condition\'')        
+        print('%sin SCODA_CCI, Unit of CCI RUN is \'condition\'' % print_prefix)        
         
     df_cnt, df_pct= get_population( adata_t.obs[t_col], 
                                     adata_t.obs[celltype_col], sort_by = [] )
 
     ## Filter celltype with its number is below the minimum value
     N_cells_min = min_n_cells_for_cci
     
@@ -197,15 +198,15 @@
     cpdb_dir = data_dir + '/cpdb'
     if not os.path.isdir(cpdb_dir):
         os.mkdir(cpdb_dir)
 
     dfv_dct = {}
     for k, s in enumerate(t_lst):
 
-        print('CLIENT INFO:    %2i/%2i - %s' % (k+1, len(t_lst), s))
+        print('%s  %2i/%2i - %s' % (print_prefix, k+1, len(t_lst), s))
 
         out_dir = cpdb_dir + '/CPDB_res_%s' % (s)
 
         celltype_all = df_cnt.columns.values
         b = df_cnt.loc[s,:] >= N_cells_min
         celltype_lst = list(celltype_all[b])
         
@@ -304,15 +305,15 @@
                 dft['pv2'] = df.loc[idxt, 'pval']
                 dfv.loc[idxt, 'pval'] = dft.max(axis = 1)
 
             dfv['mean'] = dfv['mean']/len(lst) 
             df_dct[g] = dfv
 
         idx_lst_all = list(set(idx_lst_all))
-        print('Union of Interactions: ', len(idx_lst_all))    
+        print('%sNumber of common Interactions: ' % print_prefix, len(idx_lst_all))    
         
         adata_t.uns['CCI'] = df_dct
         
     return
 
 
 def scoda_deg_gsea( adata_t, pw_db, 
@@ -345,18 +346,18 @@
     cond_lst = list(adata_t.obs[cond_col].unique())
     
     if sample_col not in list(adata_t.obs.columns.values):
         adata_t.obs[sample_col] = 'Not specified'
     sample_lst = list(adata_t.obs[sample_col].unique())
     
     if len(cond_lst) <= 1:
-        print('CLIENT INFO: DEG analysis not performed.')
-        print('CLIENT INFO: (might be single sample or no sample condition provided.)')
+        print('%sDEG analysis not performed.' % print_prefix)
+        print('%s(might be single sample or no sample condition provided.)' % print_prefix)
     else:
-        print('CLIENT INFO: DEG/GSEA analysis running for each celltype .. ')
+        print('%sDEG/GSEA analysis running for each celltype .. ' % print_prefix)
         
         ## Normalize and log-transform
         adata = adata_t[:,:]
         # if not tumor_identification:    
         sc.pp.normalize_total(adata, target_sum=1e4)
         sc.pp.log1p(adata)
 
@@ -386,26 +387,26 @@
 
             pcnt = adata_s.obs[cond_col].value_counts()
             s = ''
             for i in pcnt.index.values:
                 s = s + '%i(%s), ' % (pcnt[i], i)
             s = s[:-2]
 
-            print('CLIENT INFO:   %s: %s' % (ct, s))
+            print('%s   %s: %s' % (print_prefix, ct, s))
 
             bx = True
             if ref_group_for_deg is not None:
                 if ref_group_for_deg not in list(adata_s.obs[cond_col].unique()):
                     bx = False
-                    print('CLIENT INFO: WARNING in GSEA: Ref group %s not present' \
-                          % ref_group_for_deg)
+                    print('%s   WARNING in GSEA: Ref group %s not present' \
+                           % (print_prefix, ref_group_for_deg))
                 
-            if (not bx) or (pcnt.mean() < N_cells_min_per_condition):
-                print('CLIENT INFO: WARNING in GSEA: The number of %s looks not enough.' \
-                      % ref_group_for_deg)
+            if ((not bx) or (pcnt.mean() < N_cells_min_per_condition)) & (ref_group_for_deg is not None):
+                print('%s   WARNING in GSEA: The number of %s looks not enough.' \
+                       % (print_prefix, ref_group_for_deg))
             else:
 
                 df_cbyg_in = adata_s.to_df()
                 groups_in = adata_s.obs[cond_col]
                 samples_in = adata_s.obs.index.values
 
                 ref_group = ref_group_for_deg
@@ -472,15 +473,15 @@
 
                 df_dct_dct_enr_up[ct] = df_lst_enrichr_up
                 df_dct_dct_enr_dn[ct] = df_lst_enrichr_dn
                 df_dct_dct_enr[ct] = df_lst_enrichr
                 df_dct_dct_pr[ct] = df_lst_prerank
                 # '''
 
-        print('CLIENT INFO: DEG/GSEA analysis done.       ')
+        print('%sDEG/GSEA analysis done.       ' % print_prefix)
 
         adata_t.uns['DEG_stat'] = df_dct_dct_n_cells
         adata_t.uns['DEG'] = df_dct_dct_deg
         # adata_t.uns['GSA'] = df_dct_dct_enr
         adata_t.uns['GSA_up'] = df_dct_dct_enr_up
         adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
@@ -490,15 +491,15 @@
 
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
                       cond_col = 'condition', sample_col = 'sample', 
                       cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
                       cnv_gcm = 0.05, cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
-                      n_cores = 4, data_dir = '.', verbose = True, prefix = 'CLIENT INFO: '):
+                      n_cores = 4, data_dir = '.', verbose = True, prefix = ''):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
     pw_db_for_gsea = gsea_pw_db 
     # cond_col = 'condition' 
     # sample_col = 'sample'
@@ -510,15 +511,15 @@
     Rth = cci_rth 
     deg_ref_group = deg_ref # None, 
     # deg_pval_cutoff = 0.01, 
     min_n_cells_for_deg = deg_n_cells_min 
     n_cores_to_use = n_cores 
     # data_dir = '.', 
     # verbose = True, 
-    # prefix = 'CLIENT INFO: '
+    # prefix = ''
     
     ################################
     ### Cell-type identification ###
 
     if verbose: print('%sCelltype annotation running .. ' % prefix)
         
     scoda_hicat(adata_t, df_mkr_db, verbose = False)
```

### Comparing `scoda-tk-0.2.2/src/scoda/viz.py` & `scoda-tk-0.2.3/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.2/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.2.3/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.2/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.2.3/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

