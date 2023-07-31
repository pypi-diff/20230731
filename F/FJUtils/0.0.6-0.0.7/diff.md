# Comparing `tmp/FJUtils-0.0.6.tar.gz` & `tmp/FJUtils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.6.tar", last modified: Sat Jul 22 12:21:41 2023, max compression
+gzip compressed data, was "FJUtils-0.0.7.tar", last modified: Mon Jul 31 09:46:42 2023, max compression
```

## Comparing `FJUtils-0.0.6.tar` & `FJUtils-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-22 12:21:41.812266 FJUtils-0.0.6/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-22 12:21:41.812266 FJUtils-0.0.6/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      313 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.6/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-22 12:21:41.812266 FJUtils-0.0.6/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.6/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-22 12:21:41.812266 FJUtils-0.0.6/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-06-06 11:02:09.000000 FJUtils-0.0.6/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.6/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.6/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.6/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9724 2023-06-24 10:11:24.000000 FJUtils-0.0.6/fjutils/optimizers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.6/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.6/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-22 12:21:41.812266 FJUtils-0.0.6/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1216 2023-07-22 12:21:00.000000 FJUtils-0.0.6/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-31 09:46:42.471868 FJUtils-0.0.7/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-31 09:46:42.471868 FJUtils-0.0.7/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      362 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      116 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.7/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-31 09:46:42.471868 FJUtils-0.0.7/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.7/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-31 09:46:42.471868 FJUtils-0.0.7/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      885 2023-07-31 09:42:46.000000 FJUtils-0.0.7/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.7/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.7/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-07-31 09:40:02.000000 FJUtils-0.0.7/fjutils/flash_attention.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.7/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1931 2023-07-26 09:37:29.000000 FJUtils-0.0.7/fjutils/loss_funcs.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9724 2023-06-24 10:11:24.000000 FJUtils-0.0.7/fjutils/optimizers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.7/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.7/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-31 09:46:42.471868 FJUtils-0.0.7/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1209 2023-07-31 09:41:53.000000 FJUtils-0.0.7/setup.py
```

### Comparing `FJUtils-0.0.6/FJUtils.egg-info/PKG-INFO` & `FJUtils-0.0.7/FJUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.6/LICENSE` & `FJUtils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/PKG-INFO` & `FJUtils-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.6/README.md` & `FJUtils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/fjutils/__init__.py` & `FJUtils-0.0.7/fjutils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,7 +2,9 @@
 from fjutils.easylm import with_sharding_constraint, match_partition_rules, wrap_function_with_rng, tree_apply, \
     names_in_current_mesh, flatten_tree, get_jax_mesh, cross_entropy_loss_and_accuracy, tree_path_to_string, \
     average_metrics, float_tensor_to_dtype, get_float_dtype_by_name, float_to_dtype, get_metrics, \
     get_gradient_checkpoint_policy, get_names_from_partition_spec, global_norm, get_weight_decay_mask, mse_loss, \
     named_tree_map, make_shard_and_gather_fns
 from fjutils.load import load_pretrained_model
 from fjutils.utils import change_to_fp16, change_to_fp32, change_to_bf16, change, count_params, get_names, get_devices
+from fjutils.flash_attention import dot_product_attention_queries_per_head, dot_product_attention_multihead, \
+    dot_product_attention_multiquery, _memory_efficient_attention
```

### Comparing `FJUtils-0.0.6/fjutils/checkpointing.py` & `FJUtils-0.0.7/fjutils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/fjutils/easylm.py` & `FJUtils-0.0.7/fjutils/easylm.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/fjutils/load.py` & `FJUtils-0.0.7/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/fjutils/optimizers.py` & `FJUtils-0.0.7/fjutils/optimizers.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/fjutils/utils.py` & `FJUtils-0.0.7/fjutils/utils.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/pyproject.toml` & `FJUtils-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.6/setup.py` & `FJUtils-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.6',
+    version='0.0.7',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
-        'jax~=0.4.7',
+        'jax',
         'transformers~=4.30.2',
         'typing~=3.7.4.3',
         'numpy~=1.24.3',
         'flax~=0.6.4',
         'msgpack~=1.0.5',
         'setuptools~=59.6.0',
         'ml_collections'
```

