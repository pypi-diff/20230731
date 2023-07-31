# Comparing `tmp/earthformer-0.0.1.tar.gz` & `tmp/earthformer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthformer-0.0.1.tar", last modified: Mon Jul 31 03:59:20 2023, max compression
+gzip compressed data, was "earthformer-0.0.2.tar", last modified: Mon Jul 31 14:39:47 2023, max compression
```

## Comparing `earthformer-0.0.1.tar` & `earthformer-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 03:59:20.605140 earthformer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 03:59:11.000000 earthformer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 03:59:11.000000 earthformer-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-31 03:59:20.605140 earthformer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-31 03:59:11.000000 earthformer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 03:59:20.605140 earthformer-0.0.1/earthformer/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 03:59:11.000000 earthformer-0.0.1/earthformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 03:59:11.000000 earthformer-0.0.1/earthformer/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 03:59:11.000000 earthformer-0.0.1/earthformer/earthformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 03:59:20.605140 earthformer-0.0.1/earthformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-31 03:59:20.000000 earthformer-0.0.1/earthformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-31 03:59:20.000000 earthformer-0.0.1/earthformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 03:59:20.000000 earthformer-0.0.1/earthformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 03:59:20.000000 earthformer-0.0.1/earthformer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 03:59:20.000000 earthformer-0.0.1/earthformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 03:59:11.000000 earthformer-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 03:59:20.605140 earthformer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-31 03:59:11.000000 earthformer-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.115745 earthformer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-31 14:39:36.000000 earthformer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 14:39:36.000000 earthformer-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-31 14:39:47.115745 earthformer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 14:39:36.000000 earthformer-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.103745 earthformer-0.0.2/earthformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.107745 earthformer-0.0.2/earthformer/baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/baselines/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.107745 earthformer-0.0.2/earthformer/cuboid_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/cuboid_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142554 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/cuboid_transformer/cuboid_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/cuboid_transformer/cuboid_transformer_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46221 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/cuboid_transformer/cuboid_transformer_unet_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/cuboid_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.107745 earthformer-0.0.2/earthformer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.107745 earthformer-0.0.2/earthformer/datasets/earthnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet21x_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.111745 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)  5275247 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/coords_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74531 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/download_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25214 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/parallel_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/earthnet_toolkit/plot_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/earthnet/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.111745 earthformer-0.0.2/earthformer/datasets/enso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/enso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/enso/enso_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.111745 earthformer-0.0.2/earthformer/datasets/moving_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/moving_mnist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/moving_mnist/moving_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.111745 earthformer-0.0.2/earthformer/datasets/nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/nbody/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/nbody/nbody_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20811 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/nbody/nbody_mnist_torch_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.115745 earthformer-0.0.2/earthformer/datasets/sevir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/sevir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39089 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/sevir/sevir_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/datasets/sevir/sevir_torch_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/earthformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.115745 earthformer-0.0.2/earthformer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/metrics/enso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/metrics/sevir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/metrics/skill_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/metrics/torchmetrics_wo_compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.115745 earthformer-0.0.2/earthformer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/apex_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.115745 earthformer-0.0.2/earthformer/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/nbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.115745 earthformer-0.0.2/earthformer/visualization/sevir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/sevir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/sevir/dataset_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/sevir/sevir_cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/sevir/sevir_vis_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-31 14:39:36.000000 earthformer-0.0.2/earthformer/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:39:47.107745 earthformer-0.0.2/earthformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-31 14:39:47.000000 earthformer-0.0.2/earthformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-31 14:39:47.000000 earthformer-0.0.2/earthformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 14:39:47.000000 earthformer-0.0.2/earthformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:39:47.000000 earthformer-0.0.2/earthformer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 14:39:47.000000 earthformer-0.0.2/earthformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 14:39:47.000000 earthformer-0.0.2/earthformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-31 14:39:36.000000 earthformer-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 14:39:47.115745 earthformer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-31 14:39:36.000000 earthformer-0.0.2/setup.py
```

### Comparing `earthformer-0.0.1/PKG-INFO` & `earthformer-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthformer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for Earthformer
 Home-page: https://github.com/opengeos/earthformer
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: earthformer
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 # Earthformer
 
 [![image](https://img.shields.io/pypi/v/earthformer.svg)](https://pypi.python.org/pypi/earthformer)
 [![image](https://img.shields.io/conda/vn/conda-forge/earthformer.svg)](https://anaconda.org/conda-forge/earthformer)
 
 **A Python package for Earthformer**
 
--   Free software: MIT license
+-   Free software: Apache Software License 2.0
 -   Documentation: <https://opengeos.github.io/earthformer>
 
 ## Introduction
 
 Earthformer is a Python package for the [Earth forecasting transformer](https://github.com/amazon-science/earth-forecasting-transformer).
 
 ## Installation
```

### Comparing `earthformer-0.0.1/README.md` & `earthformer-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Earthformer
 
 [![image](https://img.shields.io/pypi/v/earthformer.svg)](https://pypi.python.org/pypi/earthformer)
 [![image](https://img.shields.io/conda/vn/conda-forge/earthformer.svg)](https://anaconda.org/conda-forge/earthformer)
 
 **A Python package for Earthformer**
 
--   Free software: MIT license
+-   Free software: Apache Software License 2.0
 -   Documentation: <https://opengeos.github.io/earthformer>
 
 ## Introduction
 
 Earthformer is a Python package for the [Earth forecasting transformer](https://github.com/amazon-science/earth-forecasting-transformer).
 
 ## Installation
```

### Comparing `earthformer-0.0.1/earthformer.egg-info/PKG-INFO` & `earthformer-0.0.2/earthformer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthformer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for Earthformer
 Home-page: https://github.com/opengeos/earthformer
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: earthformer
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 # Earthformer
 
 [![image](https://img.shields.io/pypi/v/earthformer.svg)](https://pypi.python.org/pypi/earthformer)
 [![image](https://img.shields.io/conda/vn/conda-forge/earthformer.svg)](https://anaconda.org/conda-forge/earthformer)
 
 **A Python package for Earthformer**
 
--   Free software: MIT license
+-   Free software: Apache Software License 2.0
 -   Documentation: <https://opengeos.github.io/earthformer>
 
 ## Introduction
 
 Earthformer is a Python package for the [Earth forecasting transformer](https://github.com/amazon-science/earth-forecasting-transformer).
 
 ## Installation
```

### Comparing `earthformer-0.0.1/setup.py` & `earthformer-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='earthformer',
     name='earthformer',
     packages=find_packages(include=['earthformer', 'earthformer.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/earthformer',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

