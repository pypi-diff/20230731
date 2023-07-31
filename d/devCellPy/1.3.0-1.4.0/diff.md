# Comparing `tmp/devCellPy-1.3.0.tar.gz` & `tmp/devCellPy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devCellPy-1.3.0.tar", last modified: Mon Jun 26 07:15:34 2023, max compression
+gzip compressed data, was "devCellPy-1.4.0.tar", last modified: Mon Jul 31 06:35:32 2023, max compression
```

## Comparing `devCellPy-1.3.0.tar` & `devCellPy-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-06-26 07:15:34.517479 devCellPy-1.3.0/
--rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devCellPy-1.3.0/LICENSE.txt
--rw-r--r--   0 vivian     (501) staff       (20)      756 2023-06-26 07:15:34.517162 devCellPy-1.3.0/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devCellPy-1.3.0/README.md
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-06-26 07:15:34.515044 devCellPy-1.3.0/devCellPy/
--rw-r--r--   0 vivian     (501) staff       (20)        0 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/__init__.py
--rw-r--r--   0 vivian     (501) staff       (20)    10300 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/__main__.py
--rw-r--r--   0 vivian     (501) staff       (20)      400 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/config.py
--rw-r--r--   0 vivian     (501) staff       (20)     2495 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/featurerank.py
--rw-r--r--   0 vivian     (501) staff       (20)     1200 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/helpers.py
--rw-r--r--   0 vivian     (501) staff       (20)      579 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/importing_modules.py
--rw-r--r--   0 vivian     (501) staff       (20)    30610 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/layer.py
--rw-r--r--   0 vivian     (501) staff       (20)     7118 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/predict.py
--rw-r--r--   0 vivian     (501) staff       (20)     6346 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/train.py
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-06-26 07:15:34.516668 devCellPy-1.3.0/devCellPy.egg-info/
--rw-r--r--   0 vivian     (501) staff       (20)      756 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)      398 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/SOURCES.txt
--rw-r--r--   0 vivian     (501) staff       (20)        1 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/dependency_links.txt
--rw-r--r--   0 vivian     (501) staff       (20)       54 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/entry_points.txt
--rw-r--r--   0 vivian     (501) staff       (20)       10 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/top_level.txt
--rw-r--r--   0 vivian     (501) staff       (20)       38 2023-06-26 07:15:34.517573 devCellPy-1.3.0/setup.cfg
--rw-r--r--   0 vivian     (501) staff       (20)     1095 2023-06-26 07:15:13.000000 devCellPy-1.3.0/setup.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-07-31 06:35:32.704937 devCellPy-1.4.0/
+-rw-r--r--   0 vivian     (501) staff       (20)     1090 2023-07-31 06:31:14.000000 devCellPy-1.4.0/LICENSE.md
+-rw-r--r--   0 vivian     (501) staff       (20)      755 2023-07-31 06:35:32.704435 devCellPy-1.4.0/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)     5048 2023-07-31 06:31:14.000000 devCellPy-1.4.0/README.md
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-07-31 06:35:32.701061 devCellPy-1.4.0/devCellPy/
+-rw-r--r--   0 vivian     (501) staff       (20)        0 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/__init__.py
+-rw-r--r--   0 vivian     (501) staff       (20)    10300 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/__main__.py
+-rw-r--r--   0 vivian     (501) staff       (20)      400 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/config.py
+-rw-r--r--   0 vivian     (501) staff       (20)     2495 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/featurerank.py
+-rw-r--r--   0 vivian     (501) staff       (20)     1268 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/helpers.py
+-rw-r--r--   0 vivian     (501) staff       (20)      579 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/importing_modules.py
+-rw-r--r--   0 vivian     (501) staff       (20)    30610 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/layer.py
+-rw-r--r--   0 vivian     (501) staff       (20)     6510 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/predict.py
+-rw-r--r--   0 vivian     (501) staff       (20)     6346 2023-07-31 06:31:14.000000 devCellPy-1.4.0/devCellPy/train.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-07-31 06:35:32.703809 devCellPy-1.4.0/devCellPy.egg-info/
+-rw-r--r--   0 vivian     (501) staff       (20)      755 2023-07-31 06:35:32.000000 devCellPy-1.4.0/devCellPy.egg-info/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)      397 2023-07-31 06:35:32.000000 devCellPy-1.4.0/devCellPy.egg-info/SOURCES.txt
+-rw-r--r--   0 vivian     (501) staff       (20)        1 2023-07-31 06:35:32.000000 devCellPy-1.4.0/devCellPy.egg-info/dependency_links.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       54 2023-07-31 06:35:32.000000 devCellPy-1.4.0/devCellPy.egg-info/entry_points.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       10 2023-07-31 06:35:32.000000 devCellPy-1.4.0/devCellPy.egg-info/top_level.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       38 2023-07-31 06:35:32.705118 devCellPy-1.4.0/setup.cfg
+-rw-r--r--   0 vivian     (501) staff       (20)     1095 2023-07-31 06:34:54.000000 devCellPy-1.4.0/setup.py
```

### Comparing `devCellPy-1.3.0/LICENSE.txt` & `devCellPy-1.4.0/LICENSE.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright <2021> <Stanford University>
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2021 Sean Wu Lab - Stanford University
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `devCellPy-1.3.0/PKG-INFO` & `devCellPy-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: devCellPy
-Version: 1.3.0
+Version: 1.4.0
 Summary: devCellPy -- hierarchical multilayered classification of cells based on scRNA-seq
 Home-page: https://github.com/devCellPy-Team/devCellPy
 Author: Sidra Xu
 Author-email: sidraxu@stanford.edu
 Maintainer: Sean Wu Lab
 Maintainer-email: smwu@stanford.edu
 License: MIT
 Requires-Python: >=3.7
-License-File: LICENSE.txt
+License-File: LICENSE.md
 
     devCellPy is a Python package designed for hierarchical
     multilayered classification of cells based on single-cell
     RNA-sequencing (scRNA-seq). It implements the machine
     learning algorithm Extreme Gradient Boost (XGBoost)
     (Chen and Guestrin, 2016) to automatically predict cell
     identities across complex permutations of layers and
```

### Comparing `devCellPy-1.3.0/devCellPy/__main__.py` & `devCellPy-1.4.0/devCellPy/__main__.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.3.0/devCellPy/featurerank.py` & `devCellPy-1.4.0/devCellPy/featurerank.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.3.0/devCellPy/helpers.py` & `devCellPy-1.4.0/devCellPy/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,23 @@
     tp = pd.read_csv(csvpath, iterator=True, chunksize=1000)
     norm_express = pd.concat(tp, ignore_index=True)
     norm_express.set_index('gene', inplace=True)
     norm_express.index.names = [None]
     norm_express = norm_express.T
     print (norm_express.head())
     norm_express.to_pickle(csvpath[:-3] + 'pkl')
+    return norm_express
 
 
 # Converts the Seurat h5ad object into a pkl
 def h5ad2pkl(h5adpath):
     adata = sc.read_h5ad(h5adpath)
-    df = pd.DataFrame(adata.X.toarray(), columns = adata.var.index, index = adata.obs.index)
-    df.to_pickle(h5adpath[:-4] + 'pkl')
+    norm_express = pd.DataFrame(adata.X.toarray(), columns = adata.var.index, index = adata.obs.index)
+    norm_express.to_pickle(h5adpath[:-4] + 'pkl')
+    return norm_express
 
 
 # Remove non-alphanumeric characters from string
 def alphanumeric(str):
     temparr = list([val for val in str if val.isalpha() or val.isnumeric()])
     cleanstr = ''.join(temparr)
     return cleanstr
```

### Comparing `devCellPy-1.3.0/devCellPy/importing_modules.py` & `devCellPy-1.4.0/devCellPy/importing_modules.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.3.0/devCellPy/layer.py` & `devCellPy-1.4.0/devCellPy/layer.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.3.0/devCellPy/predict.py` & `devCellPy-1.4.0/devCellPy/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,25 +56,20 @@
     os.makedirs(config.path)
     os.chdir(config.path)
 
     all_layers = helpers.import_layers(object_paths)
     print(all_layers)
     featurenames = all_layers[0].xgbmodel.feature_names
     reorder_pickle(val_normexpr, featurenames)
-    if val_normexpr[-3:] == 'csv':
-        val_normexpr = val_normexpr[:-3] + 'pkl'
-    elif val_normexpr[-4:] == 'h5ad':
-        val_normexpr = val_normexpr[:-4] + 'pkl'
+    val_normexpr = val_normexpr[:val_normexpr.index('.')] + '_reordered.pkl'
 
     norm_express = pd.read_pickle(val_normexpr)
     feature_names = list(norm_express)
     print(norm_express.shape)
     X = norm_express.values
-
-    X = norm_express.values
     norm_express.index.name = 'cells'
     norm_express.reset_index(inplace=True)
     Y = norm_express.values
     all_cellnames = Y[:,0]
     all_cellnames = all_cellnames.ravel()
     Y = None
 
@@ -120,40 +115,31 @@
 # First column name (cell A1) is 'gene'
 # Reorders the csv file to match the features in a given featurenames list
 # Returns path to the new pkl file
 def reorder_pickle(path, featurenames):
     # Convert data into pickles
     if path[-3:] == 'csv':
         csvpath = path
-        tp = pd.read_csv(csvpath, iterator=True, chunksize=1000)
-        norm_express = pd.concat(tp, ignore_index=True)
-        norm_express.set_index('gene', inplace=True)
-        norm_express.index.names = [None]
-        norm_express = norm_express.T
-        # print (norm_express.head())
-        # print(norm_express.T.duplicated().any())
-        norm_express.to_pickle(csvpath[:-3] + 'pkl')
+        norm_express = helpers.csv2pkl(csvpath)
     elif path[-4:] == 'h5ad':
         h5adpath = path
-        adata = sc.read_h5ad(h5adpath)
-        norm_express = pd.DataFrame(adata.X.toarray(), columns = adata.var.index, index = adata.obs.index)
-        norm_express.to_pickle(h5adpath[:-4] + 'pkl')
+        norm_express = helpers.h5ad2pkl(h5adpath)
     elif path[-3:] == 'pkl':
         norm_express = pd.read_pickle(path)
     else:
         raise ValueError('Format of normalized expression data file not recognized')
     print ('Training Data # of  genes: ' + str(len(featurenames)))
     origfeat = list(norm_express)
     print ('Validation Data # of genes: ' + str(len(origfeat)))
     print ('Overlapping # of genes: ' + str(len(set(featurenames).intersection(origfeat))))
 
     ## Manually reorder columns according to training data index
     # Reorder overlapping genes, remove genes not in training data
     norm_express = norm_express.reindex(columns=featurenames, fill_value=None)
-    norm_express.to_pickle(path[:-4] + '_reordered.pkl')
+    norm_express.to_pickle(path[:path.index('.')] + '_reordered.pkl')
 
 
 # Utility function, searches a list of all_layers for a layer with the given name
 def find_predictlayer(all_layers, name):
     for layer in all_layers:
         if layer.predictname == name:
             return layer
```

### Comparing `devCellPy-1.3.0/devCellPy/train.py` & `devCellPy-1.4.0/devCellPy/train.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.3.0/devCellPy.egg-info/PKG-INFO` & `devCellPy-1.4.0/devCellPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: devCellPy
-Version: 1.3.0
+Version: 1.4.0
 Summary: devCellPy -- hierarchical multilayered classification of cells based on scRNA-seq
 Home-page: https://github.com/devCellPy-Team/devCellPy
 Author: Sidra Xu
 Author-email: sidraxu@stanford.edu
 Maintainer: Sean Wu Lab
 Maintainer-email: smwu@stanford.edu
 License: MIT
 Requires-Python: >=3.7
-License-File: LICENSE.txt
+License-File: LICENSE.md
 
     devCellPy is a Python package designed for hierarchical
     multilayered classification of cells based on single-cell
     RNA-sequencing (scRNA-seq). It implements the machine
     learning algorithm Extreme Gradient Boost (XGBoost)
     (Chen and Guestrin, 2016) to automatically predict cell
     identities across complex permutations of layers and
```

### Comparing `devCellPy-1.3.0/setup.py` & `devCellPy-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     multilayered classification of cells based on single-cell
     RNA-sequencing (scRNA-seq). It implements the machine
     learning algorithm Extreme Gradient Boost (XGBoost)
     (Chen and Guestrin, 2016) to automatically predict cell
     identities across complex permutations of layers and
     sublayers of annotation.""",  # wrap at col 60
     url = 'https://github.com/devCellPy-Team/devCellPy',
-    version = '1.3.0',
+    version = '1.4.0',
     author = 'Sidra Xu',
     author_email = 'sidraxu@stanford.edu',
     maintainer = 'Sean Wu Lab',
     maintainer_email = 'smwu@stanford.edu',
     license = 'MIT',
     python_requires = '>=3.7',
     include_package_data = True,
```

