# Comparing `tmp/NeuroGraph-1.1.2.tar.gz` & `tmp/NeuroGraph-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NeuroGraph-1.1.2.tar", last modified: Fri Jun 30 16:51:57 2023, max compression
+gzip compressed data, was "dist/NeuroGraph-2.0.0.tar", last modified: Mon Jul 31 16:06:26 2023, max compression
```

## Comparing `NeuroGraph-1.1.2.tar` & `NeuroGraph-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     1067 2023-06-24 14:47:00.000000 NeuroGraph-1.1.2/LICENSE.txt
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)        0 2023-06-25 15:58:57.000000 NeuroGraph-1.1.2/NeuroGraph/__init__.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     6848 2023-06-29 15:03:47.000000 NeuroGraph-1.1.2/NeuroGraph/datasets.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)    39747 2023-06-29 15:03:47.000000 NeuroGraph-1.1.2/NeuroGraph/preprocess.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      345 2023-06-30 16:44:30.000000 NeuroGraph-1.1.2/NeuroGraph/test.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     5663 2023-06-30 16:43:00.000000 NeuroGraph-1.1.2/NeuroGraph/utils.py
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/PKG-INFO
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      309 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/SOURCES.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/dependency_links.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       53 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/requires.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       11 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/top_level.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/PKG-INFO
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      522 2023-06-27 17:54:10.000000 NeuroGraph-1.1.2/README.md
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       38 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/setup.cfg
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      797 2023-06-30 16:51:00.000000 NeuroGraph-1.1.2/setup.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1067 2023-06-24 14:47:00.000000 NeuroGraph-2.0.0/LICENSE.txt
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        0 2023-06-25 15:58:57.000000 NeuroGraph-2.0.0/NeuroGraph/__init__.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     6853 2023-07-31 15:52:07.000000 NeuroGraph-2.0.0/NeuroGraph/datasets.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)    39747 2023-07-31 15:57:51.000000 NeuroGraph-2.0.0/NeuroGraph/preprocess.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      345 2023-06-30 16:44:30.000000 NeuroGraph-2.0.0/NeuroGraph/test.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     5663 2023-07-31 15:54:21.000000 NeuroGraph-2.0.0/NeuroGraph/utils.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph.egg-info/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph.egg-info/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      309 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       53 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph.egg-info/requires.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       11 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/NeuroGraph.egg-info/top_level.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1059 2023-07-09 18:52:46.000000 NeuroGraph-2.0.0/README.md
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       38 2023-07-31 16:06:26.000000 NeuroGraph-2.0.0/setup.cfg
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      797 2023-07-31 16:06:00.000000 NeuroGraph-2.0.0/setup.py
```

### Comparing `NeuroGraph-1.1.2/LICENSE.txt` & `NeuroGraph-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuroGraph-1.1.2/NeuroGraph/datasets.py` & `NeuroGraph-2.0.0/NeuroGraph/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,28 +86,25 @@
         if self.pre_transform is not None:
             data_list = [self.pre_transform(data) for data in data_list]
 
         data, slices = self.collate(data_list)
         torch.save((data, slices), self.processed_paths[0])
        
 class NeuroGraphDynamic():
-    """
-        Graph-based neuroimaging benchmark datasets, e.g.,
+    r"""Graph-based neuroimaging benchmark datasets, e.g.,
         :obj:`"DynHCPGender"`, :obj:`"DynHCPAge"`, :obj:`"DynHCPActivity"`,
         :obj:`"DynHCP-WM"`, or :obj:`"DynHCP-FI"`
 
         Args:
             root (str): Root directory where the dataset should be saved.
             name (str): The name of the dataset.
 
         Returns:
-            list: A list of graphs in PyTorch Geometric (pyg) format. Each graph has dynamic graphs batched in pyg batch.
+            list: A list of graphs in PyTorch Geometric (pyg) format. Each graph contains a list of dynamic graphs batched in pyg batch.
     """
-
-
     def __init__(self,root, name):
         self.root = root
         self.name = name
         self.urls = {"DynHCPGender":'https://vanderbilt.box.com/shared/static/mj0z6unea34lfz1hkdwsinj7g22yohxn.zip',
                     "DynHCPActivity":'https://vanderbilt.box.com/shared/static/2so3fnfqakeu6hktz322o3nm2c8ocus7.zip',
                     "DynHCPAge":'https://vanderbilt.box.com/shared/static/195f9teg4t4apn6kl6hbc4ib4g9addtq.zip',
                     "DynHCPWM":'https://vanderbilt.box.com/shared/static/mxy8fq3ghm60q6h7uhnu80pgvfxs6xo2.zip',
```

### Comparing `NeuroGraph-1.1.2/NeuroGraph/preprocess.py` & `NeuroGraph-2.0.0/NeuroGraph/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,15 +640,15 @@
             dataset = [self.pre_transform(data) for data in dataset]
 
         data, slices = self.collate(dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 
-class Brain_connectome_Rest_Download(InMemoryDataset):
+class Brain_Connectome_Rest_Download(InMemoryDataset):
     
     def __init__(self, root,name,n_rois, threshold,path_to_data,n_jobs,s3, transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name,self.n_rois,self.threshold,self.target_path,self.n_jobs,self.s3 = root, name,n_rois,threshold,path_to_data,n_jobs,s3
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
 
@@ -771,15 +771,15 @@
             dataset = [self.pre_transform(data) for data in dataset]
 
         data, slices = self.collate(dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 
-class Brain_connectome_Activity_Download(InMemoryDataset):
+class Brain_Connectome_Activity_Download(InMemoryDataset):
     
     def __init__(self, root, dataset_name,n_rois, threshold,path_to_data,n_jobs,s3,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name,self.n_rois,self.threshold,self.target_path,self.n_jobs,self.s3 = root, dataset_name,n_rois,threshold,path_to_data,n_jobs,s3
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
```

### Comparing `NeuroGraph-1.1.2/NeuroGraph/utils.py` & `NeuroGraph-2.0.0/NeuroGraph/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     # zscored upper triangle
     zd_fc *= 1 - np.tri(*zd_fc.shape, k=-1)
     np.fill_diagonal(zd_fc, 0)
     corr = fc + zd_fc
     return corr
 
 
-def construct_Adj(corr, threshold=5):
+def construct_adj(corr, threshold=5):
     """
     create adjacency matrix from functional connectome matrix
     
     Args:
     
     corr (n x n numpy matrix): functional connectome matrix
```

### Comparing `NeuroGraph-1.1.2/NeuroGraph.egg-info/PKG-INFO` & `NeuroGraph-2.0.0/NeuroGraph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroGraph
-Version: 1.1.2
+Version: 2.0.0
 Summary: A Python package for graph-based Neuroimaging benchmarks and tools
 Author: Anwar Said
 Author-email: <anwar.said@vanderbilt.edu>
 Keywords: python,neuroimaging,graph machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuroGraph-1.1.2/PKG-INFO` & `NeuroGraph-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroGraph
-Version: 1.1.2
+Version: 2.0.0
 Summary: A Python package for graph-based Neuroimaging benchmarks and tools
 Author: Anwar Said
 Author-email: <anwar.said@vanderbilt.edu>
 Keywords: python,neuroimaging,graph machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuroGraph-1.1.2/setup.py` & `NeuroGraph-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='NeuroGraph',
-    version='1.1.2',
+    version='2.0.0',
     description='A Python package for graph-based Neuroimaging benchmarks and tools',
     author='Anwar Said',
     author_email='<anwar.said@vanderbilt.edu>',
     packages=['NeuroGraph'],
     install_requires=[
         # List any dependencies your package requires
         'boto3==1.26.158',
```

