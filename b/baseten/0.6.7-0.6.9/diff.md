# Comparing `tmp/baseten-0.6.7.tar.gz` & `tmp/baseten-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.6.7.tar", max compression
+gzip compressed data, was "baseten-0.6.9.tar", max compression
```

## Comparing `baseten-0.6.7.tar` & `baseten-0.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     5041 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/__init__.py
--rw-r--r--   0        0        0    29519 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/lib_support.py
--rw-r--r--   0        0        0    18701 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2288 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/settings.py
--rw-r--r--   0        0        0     1787 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     5130 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/training/datasets.py
--rw-r--r--   0        0        0    33964 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/training/logs.py
--rw-r--r--   0        0        0      479 2023-07-20 20:54:26.910287 baseten-0.6.7/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-07-20 20:54:26.914287 baseten-0.6.7/pypi_readme.md
--rw-r--r--   0        0        0     1960 2023-07-20 20:55:14.211849 baseten-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 baseten-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/__init__.py
+-rw-r--r--   0        0        0    12867 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/__init__.py
+-rw-r--r--   0        0        0    29519 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    17743 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2288 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-07-27 22:01:49.137425 baseten-0.6.9/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-07-27 22:01:49.141425 baseten-0.6.9/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-07-27 22:01:49.141425 baseten-0.6.9/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-07-27 22:01:49.145425 baseten-0.6.9/pypi_readme.md
+-rw-r--r--   0        0        0     1960 2023-07-27 22:02:29.381171 baseten-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 baseten-0.6.9/PKG-INFO
```

### Comparing `baseten-0.6.7/baseten/__init__.py` & `baseten-0.6.9/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/baseten_deployed_model.py` & `baseten-0.6.9/baseten/baseten_deployed_model.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/cli.py` & `baseten-0.6.9/baseten/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import platform
 import sys
 import time
 
 import click
 import requests
 from requests.exceptions import RequestException
-from truss.cli import cli_group as truss_commands
+from truss.cli import truss_cli as truss_commands
 
 from baseten import version as b10_version
 from baseten.client_commands import (
     baseten_cli,
     dataset_cli,
     finetuning_cli,
     models_cli,
```

### Comparing `baseten-0.6.7/baseten/client_commands/baseten_cli.py` & `baseten-0.6.9/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/client_commands/dataset_cli.py` & `baseten-0.6.9/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/client_commands/finetuning_cli.py` & `baseten-0.6.9/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/client_commands/models_cli.py` & `baseten-0.6.9/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/client_commands/pretrained_cli.py` & `baseten-0.6.9/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/api.py` & `baseten-0.6.9/baseten/common/api.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/core.py` & `baseten-0.6.9/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/error_handler.py` & `baseten-0.6.9/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/files.py` & `baseten-0.6.9/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/lib_support.py` & `baseten-0.6.9/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/model_deployer.py` & `baseten-0.6.9/baseten/common/model_deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,68 +236,41 @@
 
 
 def try_patch_draft_truss(
     model_name: str,
     truss_handle: TrussHandle,
 ) -> TryPatchDraftTrussResponse:
     dev_model_version_info = _get_draft_model_version_info(model_name)
+
     if dev_model_version_info is None:
-        return TryPatchDraftTrussResponse(
-            succeeded=False,
-            needs_full_deploy=True,
-            model_version_info=None,
-            error_message=f"No draft version found for model {model_name}.",
+        return TryPatchDraftTrussResponse.needs_full_deploy_response(
+            f"No draft model found for model {model_name}."
         )
 
+    # We need this check because a model that has not finished building will
+    # not have Truss hash and signature.
     model_deployment_status = dev_model_version_info["current_model_deployment_status"]["status"]
     if model_deployment_status == "BUILDING_MODEL":
         return TryPatchDraftTrussResponse(
             succeeded=False,
             needs_full_deploy=False,
             model_version_info=dev_model_version_info,
             error_message=f"model {model_name} is currently building, please retry after it's finished.",
         )
-    if model_deployment_status == "DEPLOYING_MODEL":
-        return TryPatchDraftTrussResponse(
-            succeeded=False,
-            needs_full_deploy=False,
-            model_version_info=dev_model_version_info,
-            error_message=f"model {model_name} is currently deploying, please retry after it's finished.",
-        )
-
-    if model_deployment_status not in [
-        "MODEL_READY",
-        "SCALED_TO_ZERO",
-        "SCALING_FROM_ZERO",
-        "MODEL_LOADING",
-        "MODEL_DEPLOY_FAILED",
-    ]:
-        return TryPatchDraftTrussResponse(
-            succeeded=False,
-            needs_full_deploy=True,
-            model_version_info=dev_model_version_info,
-            error_message=f"model {model_name} is not ready for patching.",
-        )
-
-    if dev_model_version_info is None:
-        return TryPatchDraftTrussResponse.needs_full_deploy_response(
-            f"no draft model found for model {model_name}."
-        )
 
-    # todo: check if model is deploying
     truss_hash = dev_model_version_info["truss_hash"]
     if truss_hash is None:
         return TryPatchDraftTrussResponse.needs_full_deploy_response(
-            f"no truss_hash found for model {model_name}."
+            f"No truss_hash found for model {model_name}."
         )
 
     truss_signature = dev_model_version_info["truss_signature"]
     if truss_signature is None:
         return TryPatchDraftTrussResponse.needs_full_deploy_response(
-            f"no truss_signature found for model {model_name}."
+            f"No truss_signature found for model {model_name}."
         )
 
     TrussLocalConfigHandler.add_signature(truss_hash, truss_signature)
 
     patch_request = truss_handle.calc_patch(truss_hash)
     if patch_request is None:
         return TryPatchDraftTrussResponse.needs_full_deploy_response("unable to calculate patch.")
```

### Comparing `baseten-0.6.7/baseten/common/settings.py` & `baseten-0.6.9/baseten/common/settings.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/tar.py` & `baseten-0.6.9/baseten/common/tar.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/types.py` & `baseten-0.6.9/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/common/util.py` & `baseten-0.6.9/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/models/flan_t5.py` & `baseten-0.6.9/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/models/llama.py` & `baseten-0.6.9/baseten/models/llama.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/models/stable_diffusion.py` & `baseten-0.6.9/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/models/util.py` & `baseten-0.6.9/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/models/whisper.py` & `baseten-0.6.9/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/training/datasets.py` & `baseten-0.6.9/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/training/finetuning.py` & `baseten-0.6.9/baseten/training/finetuning.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/baseten/training/logs.py` & `baseten-0.6.9/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/pypi_readme.md` & `baseten-0.6.9/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.6.7/pyproject.toml` & `baseten-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.6.7"
+version = "0.6.9"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
@@ -25,15 +25,15 @@
 coolname = ">=1.1.0"
 pyyaml = ">=5.1"
 tqdm = "^4.62.1"
 requests-toolbelt = "^0.9.1"
 tenacity = "^8.0.1"
 single-source = "^0.3.0"
 semantic-version = "^2.10.0"
-truss = "0.5.0"
+truss = "0.5.1"
 Pillow = "^9.3.0"
 types-requests = "^2.28.11.7"
 types-setuptools = "^65.6.0.2"
 types-pillow = "^9.3.0.4"
 types-pyyaml = "^6.0.12.2"
 halo = "^0.0.31"
 types-pytz = "^2022.7.1.0"
```

### Comparing `baseten-0.6.7/PKG-INFO` & `baseten-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.6.7
+Version: 0.6.9
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: requests (>=2.22)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tqdm (>=4.62.1,<5.0.0)
-Requires-Dist: truss (==0.5.0)
+Requires-Dist: truss (==0.5.1)
 Requires-Dist: types-pillow (>=9.3.0.4,<10.0.0.0)
 Requires-Dist: types-pytz (>=2022.7.1.0,<2023.0.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.2,<7.0.0.0)
 Requires-Dist: types-requests (>=2.28.11.7,<3.0.0.0)
 Requires-Dist: types-setuptools (>=65.6.0.2,<66.0.0.0)
 Project-URL: Documentation, https://docs.baseten.co
 Project-URL: Homepage, https://baseten.co
```

