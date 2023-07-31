# Comparing `tmp/En-transformer-1.0.3.tar.gz` & `tmp/En-transformer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "En-transformer-1.0.3.tar", last modified: Fri Mar 17 02:32:13 2023, max compression
+gzip compressed data, was "En-transformer-1.1.0.tar", last modified: Mon Jul 31 20:37:14 2023, max compression
```

## Comparing `En-transformer-1.0.3.tar` & `En-transformer-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 02:32:13.189192 En-transformer-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 02:32:13.189192 En-transformer-1.0.3/En_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-17 02:32:13.000000 En-transformer-1.0.3/En_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-17 02:32:13.000000 En-transformer-1.0.3/En_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 02:32:13.000000 En-transformer-1.0.3/En_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-17 02:32:13.000000 En-transformer-1.0.3/En_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-17 02:32:13.000000 En-transformer-1.0.3/En_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-17 02:32:01.000000 En-transformer-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-17 02:32:13.189192 En-transformer-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-03-17 02:32:01.000000 En-transformer-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 02:32:13.189192 En-transformer-1.0.3/en_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-17 02:32:01.000000 En-transformer-1.0.3/en_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-03-17 02:32:01.000000 En-transformer-1.0.3/en_transformer/en_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-17 02:32:01.000000 En-transformer-1.0.3/en_transformer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-17 02:32:13.189192 En-transformer-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-17 02:32:01.000000 En-transformer-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:37:14.325400 En-transformer-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:37:14.325400 En-transformer-1.1.0/En_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 20:37:01.000000 En-transformer-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-31 20:37:14.325400 En-transformer-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-31 20:37:01.000000 En-transformer-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:37:14.325400 En-transformer-1.1.0/en_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 20:37:01.000000 En-transformer-1.1.0/en_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-07-31 20:37:01.000000 En-transformer-1.1.0/en_transformer/en_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 20:37:01.000000 En-transformer-1.1.0/en_transformer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 20:37:14.325400 En-transformer-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 20:37:01.000000 En-transformer-1.1.0/setup.py
```

### Comparing `En-transformer-1.0.3/En_transformer.egg-info/PKG-INFO` & `En-transformer-1.1.0/En_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: En-transformer
-Version: 1.0.3
+Version: 1.1.0
 Summary: E(n)-Equivariant Transformer
 Home-page: https://github.com/lucidrains/En-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,transformer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `En-transformer-1.0.3/LICENSE` & `En-transformer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `En-transformer-1.0.3/PKG-INFO` & `En-transformer-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: En-transformer
-Version: 1.0.3
+Version: 1.1.0
 Summary: E(n)-Equivariant Transformer
 Home-page: https://github.com/lucidrains/En-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,transformer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `En-transformer-1.0.3/README.md` & `En-transformer-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -175,7 +175,17 @@
 ```bibtex
 @inproceedings{Shen2018DecomposedAS,
     title   = {Decomposed Attention: Self-Attention with Linear Complexities},
     author  = {Zhuoran Shen and Mingyuan Zhang and Haiyu Zhao and Shuai Yi and Hongsheng Li},
     year    = {2018}
 }
 ```
+
+```bibtex
+@inproceedings{Kim2020TheLC,
+    title   = {The Lipschitz Constant of Self-Attention},
+    author  = {Hyunjik Kim and George Papamakarios and Andriy Mnih},
+    booktitle = {International Conference on Machine Learning},
+    year    = {2020},
+    url     = {https://api.semanticscholar.org/CorpusID:219530837}
+}
+```
```

#### html2text {}

```diff
@@ -58,8 +58,12 @@
 } ``` ```bibtex @misc{liu2021swin, title = {Swin Transformer V2: Scaling Up
 Capacity and Resolution}, author = {Ze Liu and Han Hu and Yutong Lin and
 Zhuliang Yao and Zhenda Xie and Yixuan Wei and Jia Ning and Yue Cao and Zheng
 Zhang and Li Dong and Furu Wei and Baining Guo}, year = {2021}, eprint =
 {2111.09883}, archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex
 @inproceedings{Shen2018DecomposedAS, title = {Decomposed Attention: Self-
 Attention with Linear Complexities}, author = {Zhuoran Shen and Mingyuan Zhang
-and Haiyu Zhao and Shuai Yi and Hongsheng Li}, year = {2018} } ```
+and Haiyu Zhao and Shuai Yi and Hongsheng Li}, year = {2018} } ``` ```bibtex
+@inproceedings{Kim2020TheLC, title = {The Lipschitz Constant of Self-
+Attention}, author = {Hyunjik Kim and George Papamakarios and Andriy Mnih},
+booktitle = {International Conference on Machine Learning}, year = {2020}, url
+= {https://api.semanticscholar.org/CorpusID:219530837} } ```
```

### Comparing `En-transformer-1.0.3/en_transformer/en_transformer.py` & `En-transformer-1.1.0/en_transformer/en_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 from torch.utils.checkpoint import checkpoint_sequential
 
-from einops import rearrange, repeat
+from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
 # helper functions
 
 def exists(val):
     return val is not None
 
@@ -196,22 +196,20 @@
         valid_neighbor_radius = float('inf'),
         init_eps = 1e-3,
         rel_pos_emb = None,
         edge_mlp_mult = 2,
         norm_rel_coors = True,
         norm_coors_scale_init = 1.,
         use_cross_product = False,
-        talking_heads = False,
-        scale = 8,
+        talking_heads = False,        
         dropout = 0.,
         num_global_linear_attn_heads = 0
     ):
         super().__init__()
-        self.scale = scale
-
+        self.scale = dim_head ** -0.5
         self.norm = LayerNorm(dim)
 
         self.neighbors = neighbors
         self.only_sparse_neighbors = only_sparse_neighbors
         self.valid_neighbor_radius = valid_neighbor_radius
 
         attn_inner_dim = heads * dim_head
@@ -308,29 +306,29 @@
         feats = self.norm(feats)
 
         assert not (only_sparse_neighbors and not exists(adj_mat)), 'adjacency matrix must be passed in if only_sparse_neighbors is turned on'
 
         if exists(mask):
             num_nodes = mask.sum(dim = -1)
 
-        rel_coors = rearrange(coors, 'b i d -> b i () d') - rearrange(coors, 'b j d -> b () j d')
+        rel_coors = rearrange(coors, 'b i d -> b i 1 d') - rearrange(coors, 'b j d -> b 1 j d')
         rel_dist = rel_coors.norm(p = 2, dim = -1)
 
         # calculate neighborhood indices
 
         nbhd_indices = None
         nbhd_masks = None
         nbhd_ranking = rel_dist.clone()
 
         if exists(adj_mat):
             if len(adj_mat.shape) == 2:
                 adj_mat = repeat(adj_mat, 'i j -> b i j', b = b)
 
             self_mask = torch.eye(n, device = device).bool()
-            self_mask = rearrange(self_mask, 'i j -> () i j')
+            self_mask = rearrange(self_mask, 'i j -> 1 i j')
             adj_mat.masked_fill_(self_mask, False)
 
             max_adj_neighbors = adj_mat.long().sum(dim = -1).max().item() + 1
 
             num_nn = max_adj_neighbors if only_sparse_neighbors else (num_nn + max_adj_neighbors)
             valid_neighbor_radius = 0 if only_sparse_neighbors else valid_neighbor_radius
 
@@ -378,18 +376,14 @@
             k_mask = rearrange(k_mask, 'b i j -> b 1 i j')
 
             mask = q_mask * k_mask
 
             if exists(nbhd_masks):
                 mask &= rearrange(nbhd_masks, 'b i j -> b 1 i j')
 
-        # cosine sim attention
-
-        q, k = map(l2norm, (q, k))
-
         # generate and apply rotary embeddings
 
         rel_dist = -rel_dist
         rel_dist = rearrange(rel_dist, 'b i j -> b 1 i j 1')
 
         if self.rel_pos_emb:
             seq = torch.arange(n, device = device, dtype = q.dtype)
@@ -398,15 +392,24 @@
             seq_rel_dist = repeat(seq_rel_dist, 'b i j -> b 1 i j 1', b = b)
             rel_dist = torch.cat((rel_dist, seq_rel_dist), dim = -1)
 
         qk_pos, value_pos = self.dynamic_pos_bias_mlp(rel_dist)
 
         # calculate inner product for queries and keys
 
-        qk = einsum('b h i d, b h i j d -> b h i j', q, k) * (self.scale if not exists(edges) else 1)
+        q = repeat(q, 'b h i d -> b h i j d', j = k.shape[-2])
+
+        # l2 distance
+        # -cdist(q, k).pow(2)
+
+        qk = -((q - k) ** 2).sum(dim = -1)
+
+        qk = qk * self.scale
+
+        # add relative positions to qk as well as values
 
         qk = qk + qk_pos
 
         v = v + value_pos
 
         # add edge information and pass through edges MLP if needed
```

### Comparing `En-transformer-1.0.3/setup.py` & `En-transformer-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'En-transformer',
   packages = find_packages(),
-  version = '1.0.3',
+  version = '1.1.0',
   license='MIT',
   description = 'E(n)-Equivariant Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/En-transformer',
   keywords = [
     'artificial intelligence',
```

