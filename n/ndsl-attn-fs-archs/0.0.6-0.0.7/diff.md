# Comparing `tmp/ndsl-attn-fs-archs-0.0.6.tar.gz` & `tmp/ndsl-attn-fs-archs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndsl-attn-fs-archs-0.0.6.tar", last modified: Sun Apr  3 06:34:36 2022, max compression
+gzip compressed data, was "ndsl-attn-fs-archs-0.0.7.tar", last modified: Mon Jul 31 17:15:43 2023, max compression
```

## Comparing `ndsl-attn-fs-archs-0.0.6.tar` & `ndsl-attn-fs-archs-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/
--rw-r--r--   0 uriel     (1000) uriel     (1000)    20130 2021-08-29 01:39:03.000000 ndsl-attn-fs-archs-0.0.6/LICENSE
--rw-r--r--   0 uriel     (1000) uriel     (1000)     1515 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/PKG-INFO
--rw-r--r--   0 uriel     (1000) uriel     (1000)      942 2021-08-29 23:17:02.000000 ndsl-attn-fs-archs-0.0.6/README.md
--rw-r--r--   0 uriel     (1000) uriel     (1000)      103 2021-08-24 22:50:16.000000 ndsl-attn-fs-archs-0.0.6/pyproject.toml
--rw-r--r--   0 uriel     (1000) uriel     (1000)       38 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/setup.cfg
--rw-r--r--   0 uriel     (1000) uriel     (1000)      827 2022-03-30 03:18:36.000000 ndsl-attn-fs-archs-0.0.6/setup.py
-drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2022-04-03 06:34:36.917686 ndsl-attn-fs-archs-0.0.6/src/
-drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/src/ndsl/
--rw-r--r--   0 uriel     (1000) uriel     (1000)        0 2021-08-24 22:49:08.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/__init__.py
-drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/src/ndsl/architecture/
--rw-r--r--   0 uriel     (1000) uriel     (1000)        0 2021-08-26 03:19:31.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/architecture/__init__.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)    15953 2022-04-03 02:32:40.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/architecture/attention.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)     2689 2021-12-03 03:29:02.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/architecture/cluster.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)       41 2021-08-24 22:53:58.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/example.py
-drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/src/ndsl/module/
--rw-r--r--   0 uriel     (1000) uriel     (1000)        0 2021-10-14 17:41:40.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/module/__init__.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)     1905 2022-03-30 03:18:13.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/module/aggregator.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)      470 2021-12-03 03:43:47.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/module/attention_aggregator.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)     1175 2022-04-01 23:14:11.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/module/encoder.py
--rw-r--r--   0 uriel     (1000) uriel     (1000)      630 2022-01-24 21:01:19.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl/module/preprocessor.py
-drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2022-04-03 06:34:36.921686 ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/
--rw-r--r--   0 uriel     (1000) uriel     (1000)     1515 2022-04-03 06:34:36.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/PKG-INFO
--rw-r--r--   0 uriel     (1000) uriel     (1000)      525 2022-04-03 06:34:36.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/SOURCES.txt
--rw-r--r--   0 uriel     (1000) uriel     (1000)        1 2022-04-03 06:34:36.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/dependency_links.txt
--rw-r--r--   0 uriel     (1000) uriel     (1000)        5 2022-04-03 06:34:36.000000 ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/top_level.txt
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.941089 ndsl-attn-fs-archs-0.0.7/
+-rw-r--r--   0 uriel     (1000) uriel     (1000)    20130 2021-08-29 01:39:03.000000 ndsl-attn-fs-archs-0.0.7/LICENSE
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     1469 2023-07-31 17:15:43.941089 ndsl-attn-fs-archs-0.0.7/PKG-INFO
+-rw-r--r--   0 uriel     (1000) uriel     (1000)      942 2021-08-29 23:17:02.000000 ndsl-attn-fs-archs-0.0.7/README.md
+-rw-r--r--   0 uriel     (1000) uriel     (1000)      103 2021-08-24 22:50:16.000000 ndsl-attn-fs-archs-0.0.7/pyproject.toml
+-rw-r--r--   0 uriel     (1000) uriel     (1000)       38 2023-07-31 17:15:43.941089 ndsl-attn-fs-archs-0.0.7/setup.cfg
+-rw-r--r--   0 uriel     (1000) uriel     (1000)      818 2023-07-31 17:15:11.000000 ndsl-attn-fs-archs-0.0.7/setup.py
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.937090 ndsl-attn-fs-archs-0.0.7/src/
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.937090 ndsl-attn-fs-archs-0.0.7/src/ndsl/
+-rw-r--r--   0 uriel     (1000) uriel     (1000)        0 2021-08-24 22:49:08.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/__init__.py
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.937090 ndsl-attn-fs-archs-0.0.7/src/ndsl/architecture/
+-rw-r--r--   0 uriel     (1000) uriel     (1000)        0 2021-08-26 03:19:31.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/architecture/__init__.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     9571 2023-02-13 18:56:43.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/architecture/attention.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)    11839 2023-02-19 00:37:13.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/architecture/feature_selection.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)       41 2021-08-24 22:53:58.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/example.py
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.937090 ndsl-attn-fs-archs-0.0.7/src/ndsl/module/
+-rw-r--r--   0 uriel     (1000) uriel     (1000)        0 2021-10-14 17:41:40.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/module/__init__.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     2165 2023-07-31 17:13:16.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/module/aggregator.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     1440 2022-12-28 04:52:59.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/module/encoder.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)      767 2022-12-28 06:04:28.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl/module/preprocessor.py
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.937090 ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     1469 2023-07-31 17:15:43.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/PKG-INFO
+-rw-r--r--   0 uriel     (1000) uriel     (1000)      630 2023-07-31 17:15:43.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/SOURCES.txt
+-rw-r--r--   0 uriel     (1000) uriel     (1000)        1 2023-07-31 17:15:43.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/dependency_links.txt
+-rw-r--r--   0 uriel     (1000) uriel     (1000)        5 2023-07-31 17:15:43.000000 ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/top_level.txt
+drwxr-xr-x   0 uriel     (1000) uriel     (1000)        0 2023-07-31 17:15:43.941089 ndsl-attn-fs-archs-0.0.7/tests/
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     2901 2022-11-25 02:12:25.000000 ndsl-attn-fs-archs-0.0.7/tests/test_aggregators.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     9085 2022-06-29 18:38:14.000000 ndsl-attn-fs-archs-0.0.7/tests/test_attention_archs.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     1961 2022-12-12 04:54:53.000000 ndsl-attn-fs-archs-0.0.7/tests/test_encoder_layer.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     1967 2022-11-25 04:03:33.000000 ndsl-attn-fs-archs-0.0.7/tests/test_encoders.py
+-rw-r--r--   0 uriel     (1000) uriel     (1000)     1035 2022-11-27 19:37:53.000000 ndsl-attn-fs-archs-0.0.7/tests/test_preprocessors.py
```

### Comparing `ndsl-attn-fs-archs-0.0.6/LICENSE` & `ndsl-attn-fs-archs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ndsl-attn-fs-archs-0.0.6/PKG-INFO` & `ndsl-attn-fs-archs-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ndsl-attn-fs-archs
-Version: 0.0.6
-Summary: Architectures involved in the investigation of Attention Mechanisms as Feature Selection
+Version: 0.0.7
+Summary: Architecture described in paper: Transformers for high-dimensional tabular data
 Home-page: https://github.com/cobu93/attn-fs-archs
 Author: Under ML
 Author-email: urielcoro@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,10 +67,8 @@
 
 
 
 
 
 
 
-
-
```

### Comparing `ndsl-attn-fs-archs-0.0.6/README.md` & `ndsl-attn-fs-archs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ndsl-attn-fs-archs-0.0.6/setup.py` & `ndsl-attn-fs-archs-0.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()    
 
 
 setuptools.setup(
      name='ndsl-attn-fs-archs',  
-     version='0.0.6',
+     version='0.0.7',
      author="Under ML",
      author_email="urielcoro@gmail.com",
-     description="Architectures involved in the investigation of Attention Mechanisms as Feature Selection",
+     description="Architecture described in paper: Transformers for high-dimensional tabular data",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/cobu93/attn-fs-archs",
      package_dir={"": "src"},
      packages=setuptools.find_packages(where="src"),
      classifiers=[
          "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `ndsl-attn-fs-archs-0.0.6/src/ndsl/module/aggregator.py` & `ndsl-attn-fs-archs-0.0.7/src/ndsl/module/aggregator.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,31 +24,38 @@
 class MaxAggregator(BaseAggregator):
     def forward(self, src):
         return torch.max(src, dim=1, keepdim=False)[0]
 
 class CLSAggregator(BaseAggregator):
     def forward(self, src):
         #src with shape [batch_size, seq_len, num_features]
-        return src[:,0,:]
+        return src[:, 0]
         #src with shape [batch_size, num_features]
 
 class RNNAggregator(BaseAggregator):
-    def __init__(self, output_size, cell, input_size, hidden_size,
-                 num_layers, dropout):
+    def __init__(self, output_size, cell, input_size, num_layers, dropout):
         super(RNNAggregator, self).__init__(output_size)
         self.output_size = output_size
 
         if cell == 'GRU':
-            self.rnn = nn.GRU(input_size, hidden_size, num_layers,
+            self.rnn = nn.GRU(input_size, output_size, num_layers,
                             batch_first=True, dropout=dropout)
         elif cell == 'LSTM':
-            self.rnn = nn.LSTM(input_size, hidden_size, num_layers,
+            self.rnn = nn.LSTM(input_size, output_size, num_layers,
                             batch_first=True, dropout=dropout)
         else:
             raise TypeError("{} is not a valid cell, try with 'LSTM' or 'GRU'.".format(cell))
 
     def forward(self, src):
         #src with shape [batch_size, seq_len, num_features]
         output, _ = self.rnn(src)
         #output: [batch_size, seq_len, hidden_size]
         return output[:, -1, :]
-        #src with shape [batch_size, num_features]
+        #src with shape [batch_size, num_features]
+
+class LearnableAggregator(BaseAggregator):
+    def __init__(self, output_size):
+        super(LearnableAggregator, self).__init__(output_size)
+        self.learnable = nn.Parameter(torch.randn(output_size))
+
+    def forward(self, src):
+        return self.learnable.repeat(src.shape[0], 1)
```

### Comparing `ndsl-attn-fs-archs-0.0.6/src/ndsl/module/encoder.py` & `ndsl-attn-fs-archs-0.0.7/src/ndsl/module/encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,39 @@
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 class FeatureEncoder(nn.Module):
     def __init__(self, output_size):
         super(FeatureEncoder, self).__init__()
         self.output_size = output_size
     
     def forward(self, src):
         raise NotImplementedError("This feature hasn't been implemented yet!")
 
 
 class CategoricalOneHotEncoder(FeatureEncoder):
-    def __init__(self, output_size, n_labels, eps=1e-15):
+    def __init__(self, output_size, n_labels, eps=1e-15, include_nan=True):
         super(CategoricalOneHotEncoder, self).__init__(output_size)
         self.eps = eps
         self.output_size = output_size
-        self.n_labels = n_labels + 1
+        if include_nan:
+            self.n_labels = n_labels + 1
+        else:
+            self.n_labels = n_labels
         self.embedding = nn.Linear(self.n_labels, output_size)
 
-    def forward(self, src):
-        src = F.one_hot(src.squeeze().long() % self.n_labels, num_classes=self.n_labels).float()
+    def forward(self, src): 
+        src = F.one_hot(src.squeeze().long(), num_classes=self.n_labels).float()
         out = self.embedding(src)
-        return out / out.sum()+ self.eps
+        return out / out.sum(dim=-1, keepdim=True) + self.eps
 
 class NumericalEncoder(FeatureEncoder):
-    def __init__(self, output_size):
+    def __init__(self, output_size, n_numerical):
         super(NumericalEncoder, self).__init__(output_size)
         self.output_size = output_size
-        self.embedding = nn.utils.weight_norm(nn.Linear(1, output_size))
-
+        self.weights = nn.Parameter(torch.randn(n_numerical, output_size))
+        self.biases = nn.Parameter(torch.randn(n_numerical, output_size))
+        
     def forward(self, src):
-        return self.embedding(src)
+        output = src.unsqueeze(-1) * self.weights + self.biases
+        return output
```

### Comparing `ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/PKG-INFO` & `ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ndsl-attn-fs-archs
-Version: 0.0.6
-Summary: Architectures involved in the investigation of Attention Mechanisms as Feature Selection
+Version: 0.0.7
+Summary: Architecture described in paper: Transformers for high-dimensional tabular data
 Home-page: https://github.com/cobu93/attn-fs-archs
 Author: Under ML
 Author-email: urielcoro@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,10 +67,8 @@
 
 
 
 
 
 
 
-
-
```

### Comparing `ndsl-attn-fs-archs-0.0.6/src/ndsl_attn_fs_archs.egg-info/SOURCES.txt` & `ndsl-attn-fs-archs-0.0.7/src/ndsl_attn_fs_archs.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 README.md
 pyproject.toml
 setup.py
 src/ndsl/__init__.py
 src/ndsl/example.py
 src/ndsl/architecture/__init__.py
 src/ndsl/architecture/attention.py
-src/ndsl/architecture/cluster.py
+src/ndsl/architecture/feature_selection.py
 src/ndsl/module/__init__.py
 src/ndsl/module/aggregator.py
-src/ndsl/module/attention_aggregator.py
 src/ndsl/module/encoder.py
 src/ndsl/module/preprocessor.py
 src/ndsl_attn_fs_archs.egg-info/PKG-INFO
 src/ndsl_attn_fs_archs.egg-info/SOURCES.txt
 src/ndsl_attn_fs_archs.egg-info/dependency_links.txt
-src/ndsl_attn_fs_archs.egg-info/top_level.txt
+src/ndsl_attn_fs_archs.egg-info/top_level.txt
+tests/test_aggregators.py
+tests/test_attention_archs.py
+tests/test_encoder_layer.py
+tests/test_encoders.py
+tests/test_preprocessors.py
```

