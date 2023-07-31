# Comparing `tmp/SC2Spa-1.2.0.tar.gz` & `tmp/SC2Spa-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC2Spa-1.2.0.tar", last modified: Tue Jul 11 14:12:51 2023, max compression
+gzip compressed data, was "SC2Spa-1.2.1.tar", last modified: Mon Jul 31 15:40:30 2023, max compression
```

## Comparing `SC2Spa-1.2.0.tar` & `SC2Spa-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 14:12:51.272389 SC2Spa-1.2.0/
--rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.2.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-11 14:12:51.271961 SC2Spa-1.2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.2.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 14:12:51.268163 SC2Spa-1.2.0/SC2Spa/
--rwxrwxrwx   0 root         (0) root         (0)    16137 2023-07-11 13:31:56.000000 SC2Spa-1.2.0/SC2Spa/BM.py
--rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.2.0/SC2Spa/ME.py
--rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.2.0/SC2Spa/PP.py
--rwxrwxrwx   0 root         (0) root         (0)    50744 2023-07-11 14:10:24.000000 SC2Spa-1.2.0/SC2Spa/SI.py
--rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.2.0/SC2Spa/SVA.py
--rwxrwxrwx   0 root         (0) root         (0)    23359 2023-07-03 11:43:39.000000 SC2Spa-1.2.0/SC2Spa/Vis.py
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.2.0/SC2Spa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-07-11 14:12:07.000000 SC2Spa-1.2.0/SC2Spa/__metadata__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 14:12:51.271101 SC2Spa-1.2.0/SC2Spa.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      274 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-07-11 14:11:48.000000 SC2Spa-1.2.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-11 14:12:51.272566 SC2Spa-1.2.0/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:40:30.140468 SC2Spa-1.2.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.2.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 15:40:30.139878 SC2Spa-1.2.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.2.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:40:30.135188 SC2Spa-1.2.1/SC2Spa/
+-rwxrwxrwx   0 root         (0) root         (0)    20229 2023-07-17 14:46:02.000000 SC2Spa-1.2.1/SC2Spa/BM.py
+-rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.2.1/SC2Spa/ME.py
+-rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.2.1/SC2Spa/PP.py
+-rwxrwxrwx   0 root         (0) root         (0)    50744 2023-07-11 14:10:24.000000 SC2Spa-1.2.1/SC2Spa/SI.py
+-rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.2.1/SC2Spa/SVA.py
+-rwxrwxrwx   0 root         (0) root         (0)    23478 2023-07-14 16:52:28.000000 SC2Spa-1.2.1/SC2Spa/Vis.py
+-rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.2.1/SC2Spa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      460 2023-07-31 15:40:12.000000 SC2Spa-1.2.1/SC2Spa/__metadata__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:40:30.138794 SC2Spa-1.2.1/SC2Spa.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      274 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      691 2023-07-31 15:40:00.000000 SC2Spa-1.2.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-31 15:40:30.140691 SC2Spa-1.2.1/setup.cfg
```

### Comparing `SC2Spa-1.2.0/LICENSE` & `SC2Spa-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.0/PKG-INFO` & `SC2Spa-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.0
+Version: 1.2.1
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.2.0/README.md` & `SC2Spa-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.0/SC2Spa/BM.py` & `SC2Spa-1.2.1/SC2Spa/BM.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,26 +7,107 @@
 import pandas as pd
 import os
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
 from scipy.stats import bootstrap
 
+from IPython.display import clear_output
 from . import PP
 
 #from matplotlib import rc
 #rc('font', **{'family':'sans-serif','sans-serif':['Helvetica']})
 
 import seaborn as sns
 cmap = sns.cubehelix_palette(n_colors = 32,start = 2, rot=1.5, as_cmap = True)
 
 #Number of columes for the prediction
 #Global variable
 n_col = 2
 
+
+def BVMI(adata1: anndata.AnnData, adata2: anndata.AnnData,
+         GL: list, coords_name = 'spatial', n_neighbors=300, max_dis=1700):
+
+    '''
+    Caculaate bivariate Moran's I of the genes of two ST data that contains the
+    same ST voxels but different gene expression
+
+    Parameters
+    ---------
+    adata1
+        a anndata object.
+    adata2
+        a anndata object that has the same voxels as or share part of the voxels
+        with adata1. The obs_names of the two objects should be consistent to
+        extract the overlapped voxels.
+    GL: The list of genes to be calculated. The genes should be in var_names of
+        adata1 and adata2
+    coords_name
+        the spatial information should be stored in adata2.obsm[coords_name]
+    n_neighbors
+        the number of max neighbors for the knn algorithm
+    max_dis
+        max distance of two neighbors
+
+    Returns
+    -------
+    MoranI_BV
+        a dataframe contains the gene name information and bivariate
+         moran's I values
+    '''
+
+    MoranI_BV = pd.DataFrame(np.zeros((len(GL), 2)), columns=['gene', 'I_BV'])
+    MoranI_BV['gene'] = GL
+    MoranI_BV.index = MoranI_BV['gene']
+
+    JCs = sorted(list(set(adata1.obs_names).intersection(set(adata2.obs_names))))
+    adata1 = adata1[JCs]
+    adata2 = adata2[JCs]
+
+    neigh = NearestNeighbors(n_neighbors=n_neighbors, radius=max_dis)
+    neigh.fit(adata2.obsm[coords_name])
+    dis, neighbors = neigh.kneighbors(adata2.obsm[coords_name], n_neighbors)
+
+    min_dis = dis[:, 1:].min()
+    dis[dis < min_dis] = min_dis
+
+    mask = (dis < max_dis).sum(axis=1)
+
+    for i, gene in enumerate(GL):
+
+        Dev1 = adata1[:, gene].X.toarray() - adata1[:, gene].X.mean()
+        Dev2 = adata2[:, gene].X.toarray() - adata2[:, gene].X.mean()
+
+        numerator = 0
+        W0 = 0
+        n = adata2.shape[0]
+
+        for j in range(n):
+
+            if (mask[j] < 1):
+                continue
+            t1 = neighbors[j][:mask[j]]
+            t2 = 100 / dis[j][:mask[j]]
+            W0 += t2.sum()
+            length = len(t1)
+            t_sum = (Dev1[[t1[0]] * length].flatten() * Dev2[t1].flatten() * t2).sum()
+            # Sum up "t_sum" of all genes
+            numerator += t_sum
+
+        # Standardization
+        MoransI_BV = numerator / ((Dev1 ** 2).sum() ** 0.5) / ((Dev2 ** 2).sum() ** 0.5) / W0 * n
+
+        print(i, gene, ':', MoransI_BV)
+        MoranI_BV.loc[gene, 'I_BV'] = MoransI_BV
+        clear_output(wait=True)
+
+    return MoranI_BV
+
+
 def my_pearsonr(Y_pred, Y_true):
     '''
     Function for caculaating the bootstraping confidence interval of
     Pearson Correlation Coefficient of the predicted locations
       and the original locations
 
     Parameters
@@ -108,17 +189,20 @@
     Y_true
         The original locations
     n_resamples
         The number of resamples performed to form the bootstrap distribution of the statistic
 
     Returns
     -------
-    Two lists. The first list stores the values of Pearson Correlation Coefficient, Root Mean Square Error
-     and Coefficient of Determination. The second list stores the confidence intervals of the corresponding
-     statistics.
+    statistics
+        A list storing the values of Pearson Correlation Coefficient, Root Mean Square Error
+         and Coefficient of Determination.
+    CI_BS
+        A list containing the confidence interval objects of the scipy.stats.bootstrap function
+        of the corresponding statistics.
     '''
 
     # Calculate confidence interval from bootstrap
     rng = np.random.default_rng()
 
     CI_pearsonr = bootstrap((Y_true.flatten(), Y_pred.flatten()), my_pearsonr, n_resamples=n_resamples,
                             vectorized=False, paired=True, method='percentile', random_state=rng)
@@ -205,14 +289,51 @@
         PD_Pearson = stats.pearsonr(PD_pred, PD_true)[0]
 
         PDRMSEs.append(PDRMSE)
         PD_Pearsons.append(PD_Pearson)
 
     return PDRMSEs, PD_Pearsons
 
+def eval_PD_CI(PD_true, PD_pred, n_resamples = 200):
+    '''
+    Caculaate the Pearson Correlation Coefficient, Root Mean Square Error
+    of the predicted pairwise distances and the true pairwise distances
+     and corresponding confidence intervals
+
+    Parameters
+    ---------
+    PD_true
+        The original normalized distances of bead/cell pairs
+    PD_pred
+        The predicted normalized distances of bead/cell pairs
+
+    Returns
+    -------
+    statistics
+        A list storing the values of Pearson Correlation Coefficient and Root Mean Square Error
+        of the original and predicted pairwise distances
+    CI_BS
+        A list containing the confidence interval objects of the scipy.stats.bootstrap function
+        of the corresponding statistics.
+    '''
+
+    rng = np.random.default_rng()
+
+    CI_PD_pearsonr = bootstrap((PD_true, PD_pred), my_pearsonr, n_resamples=n_resamples,
+                               vectorized=False, paired=True, method='percentile', random_state=rng)
+    CI_PD_rmse = bootstrap((PD_true, PD_pred), PD_rmse, n_resamples=n_resamples,
+                           vectorized=False, paired=True, method='percentile', random_state=rng)
+    CI_BS = [CI_PD_pearsonr, CI_PD_rmse]
+
+    PDRMSE = PD_rmse(PD_pred, PD_true)
+    PD_Pearson = stats.pearsonr(PD_pred, PD_true)[0]
+    statistics = [PD_Pearson, PDRMSE]
+
+    return statistics, CI_BS
+
 def eval_cv(preds: list, YNorm: np.array, test_indices: list, CPs: np.array,
             CI_BS = False, n_resamples=200):
     '''
     Caculaate the Pearson Correlation Coefficient, Root Mean Square Error
      and Coefficient of Determination between the predicted locations
       and the original locations for the test beads in Cross-Validation.
     Corresponding confidence intervals will be calculated if `CI_BS` is True.
```

### Comparing `SC2Spa-1.2.0/SC2Spa/ME.py` & `SC2Spa-1.2.1/SC2Spa/ME.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.0/SC2Spa/PP.py` & `SC2Spa-1.2.1/SC2Spa/PP.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.0/SC2Spa/SI.py` & `SC2Spa-1.2.1/SC2Spa/SI.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.0/SC2Spa/SVA.py` & `SC2Spa-1.2.1/SC2Spa/SVA.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.0/SC2Spa/Vis.py` & `SC2Spa-1.2.1/SC2Spa/Vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                 plt.savefig(root + Genes[i] + '_' + CT + '.png', )
             else:
                 plt.savefig(root + Genes[i] + '.png', )
         plt.show()
 
 
 def DrawGenes2(adata:anndata.AnnData, gene:str, coords_name='spatial', lim = False,
-               xlim = [650, 5750], ylim = [650, 5750], figsize = (10,10),
+               xlim = [650, 5750], ylim = [650, 5750], figsize = (10,10), alpha = 0.7.
                cmap = cmap, FM = True, scST = False, CTL = None, c_name = 'simp_name',
                root = 'transfer2/FM_Valid1/', s = 2, Sparse = True, title = False, save = None):
 
     '''
     Show the expression of a gene in cells or ST beads
 
     The figure will be saved as `root + save + '_' + gene + '.png'`
@@ -284,14 +284,17 @@
         colormap. See matplotlib
     FM
         Draw finely mapped beads of cells if True
     scST
         Draw reconstructed single-cell ST data if True
     Sparse
         True if the gene expression matrix is saved in sparse format
+    alpha
+        control the transparency of the scatters. 1 is transparent.
+        0 is opaque.
     figsize
         figure size
 
     Returns
     -------
     None
 
@@ -314,20 +317,20 @@
         plt.figure(figsize=figsize)
     if(lim):
         plt.xlim(xlim)
         plt.ylim(ylim)
 
     if(Sparse):
         plt.scatter(adata.obsm[coords_name][:, 0], adata.obsm[coords_name][:, 1],\
-                    marker='o', s = s, alpha = 0.7,\
+                    marker='o', s = s, alpha = alpha,\
                     c = adata[:, gene].X.toarray().flatten(),\
                     cmap = cmap)
     else:
         plt.scatter(adata.obsm[coords_name][:, 0], adata.obsm[coords_name][:, 1], \
-                    marker='o', s=s, alpha=0.7, \
+                    marker='o', s=s, alpha=alpha, \
                     c=adata[:, gene].X.flatten(), \
                     cmap=cmap)
 
     plt.grid(False)
     plt.axis('off')
     if(title):
         plt.title(gene, fontsize = 12)
```

### Comparing `SC2Spa-1.2.0/SC2Spa.egg-info/PKG-INFO` & `SC2Spa-1.2.1/SC2Spa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.0
+Version: 1.2.1
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.2.0/pyproject.toml` & `SC2Spa-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

