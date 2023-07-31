# Comparing `tmp/mesh_common-0.1.5.tar.gz` & `tmp/mesh_common-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesh_common-0.1.5.tar", max compression
+gzip compressed data, was "mesh_common-0.1.6.tar", max compression
```

## Comparing `mesh_common-0.1.5.tar` & `mesh_common-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1078 2023-07-07 20:59:49.946360 mesh_common-0.1.5/LICENSE.md
--rw-r--r--   0        0        0      352 2023-07-07 20:59:49.946360 mesh_common-0.1.5/README.md
--rw-r--r--   0        0        0     7521 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/aws.py
--rw-r--r--   0        0        0     2976 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/concurrency.py
--rw-r--r--   0        0        0     2106 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/constants.py
--rw-r--r--   0        0        0    10606 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/encoding.py
--rw-r--r--   0        0        0     2139 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/env_config.py
--rw-r--r--   0        0        0      745 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/fernet.py
--rw-r--r--   0        0        0     1258 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/fixtures.py
--rw-r--r--   0        0        0     4671 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/httpx_retry_transport.py
--rw-r--r--   0        0        0     1937 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/lambdas.py
--rw-r--r--   0        0        0     3537 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/oas.py
--rw-r--r--   0        0        0        0 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/py.typed
--rw-r--r--   0        0        0     3306 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/singletons.py
--rw-r--r--   0        0        0     1565 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/sqs_helper.py
--rw-r--r--   0        0        0     9538 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/store.py
--rw-r--r--   0        0        0     6909 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/test_helpers.py
--rw-r--r--   0        0        0    10117 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/test_helpers_logs.py
--rw-r--r--   0        0        0      732 2023-07-07 20:59:49.946360 mesh_common-0.1.5/mesh_common/text.py
--rw-r--r--   0        0        0     2762 2023-07-07 21:00:07.750462 mesh_common-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     2404 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/common_tests.py
--rw-r--r--   0        0        0     6014 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/concurrency_tests.py
--rw-r--r--   0        0        0      673 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     8775 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/encoding_tests.py
--rw-r--r--   0        0        0     1711 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/env_config_tests.py
--rw-r--r--   0        0        0     4329 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/httpx_retry_transport_tests.py
--rw-r--r--   0        0        0     5638 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/singletons_tests.py
--rw-r--r--   0        0        0     1128 2023-07-07 20:59:49.946360 mesh_common-0.1.5/tests/test_helpers_tests.py
--rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 mesh_common-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-31 10:29:04.527494 mesh_common-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0      352 2023-07-31 10:29:04.527494 mesh_common-0.1.6/README.md
+-rw-r--r--   0        0        0     7521 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/aws.py
+-rw-r--r--   0        0        0     2976 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/concurrency.py
+-rw-r--r--   0        0        0     2106 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/constants.py
+-rw-r--r--   0        0        0    10606 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/encoding.py
+-rw-r--r--   0        0        0     2139 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/env_config.py
+-rw-r--r--   0        0        0      745 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/fernet.py
+-rw-r--r--   0        0        0     1258 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/fixtures.py
+-rw-r--r--   0        0        0     4671 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/httpx_retry_transport.py
+-rw-r--r--   0        0        0     1937 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/lambdas.py
+-rw-r--r--   0        0        0     3537 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/oas.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/py.typed
+-rw-r--r--   0        0        0     3306 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/singletons.py
+-rw-r--r--   0        0        0     1565 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/sqs_helper.py
+-rw-r--r--   0        0        0     9518 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/store.py
+-rw-r--r--   0        0        0     6909 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/test_helpers.py
+-rw-r--r--   0        0        0    10117 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/test_helpers_logs.py
+-rw-r--r--   0        0        0      732 2023-07-31 10:29:04.527494 mesh_common-0.1.6/mesh_common/text.py
+-rw-r--r--   0        0        0     2762 2023-07-31 10:29:20.599503 mesh_common-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     2404 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/common_tests.py
+-rw-r--r--   0        0        0     6014 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/concurrency_tests.py
+-rw-r--r--   0        0        0      673 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     8775 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/encoding_tests.py
+-rw-r--r--   0        0        0     1711 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/env_config_tests.py
+-rw-r--r--   0        0        0     4329 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/httpx_retry_transport_tests.py
+-rw-r--r--   0        0        0     5638 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/singletons_tests.py
+-rw-r--r--   0        0        0     1128 2023-07-31 10:29:04.531494 mesh_common-0.1.6/tests/test_helpers_tests.py
+-rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 mesh_common-0.1.6/PKG-INFO
```

### Comparing `mesh_common-0.1.5/LICENSE.md` & `mesh_common-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/__init__.py` & `mesh_common-0.1.6/mesh_common/__init__.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/aws.py` & `mesh_common-0.1.6/mesh_common/aws.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/concurrency.py` & `mesh_common-0.1.6/mesh_common/concurrency.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/constants.py` & `mesh_common-0.1.6/mesh_common/constants.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/encoding.py` & `mesh_common-0.1.6/mesh_common/encoding.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/env_config.py` & `mesh_common-0.1.6/mesh_common/env_config.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/fernet.py` & `mesh_common-0.1.6/mesh_common/fernet.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/fixtures.py` & `mesh_common-0.1.6/mesh_common/fixtures.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/httpx_retry_transport.py` & `mesh_common-0.1.6/mesh_common/httpx_retry_transport.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/lambdas.py` & `mesh_common-0.1.6/mesh_common/lambdas.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/oas.py` & `mesh_common-0.1.6/mesh_common/oas.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/singletons.py` & `mesh_common-0.1.6/mesh_common/singletons.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/sqs_helper.py` & `mesh_common-0.1.6/mesh_common/sqs_helper.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/store.py` & `mesh_common-0.1.6/mesh_common/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     Tuple,
     TypeVar,
     cast,
 )
 
 from botocore.exceptions import ClientError
 from mypy_boto3_dynamodb.type_defs import (
-    QueryOutputTableTypeDef,
+    QueryOutputTypeDef,
     TransactGetItemTypeDef,
-    UpdateItemOutputTableTypeDef,
+    UpdateItemOutputTypeDef,
 )
 from nhs_aws_helpers.dynamodb_model_store.base_model import (
     BaseModel,
     model_properties_cache,
     serialised_property,
 )
 from nhs_aws_helpers.dynamodb_model_store.base_model_store import (
@@ -219,15 +219,15 @@
 
     @log_action(log_level=logging.DEBUG, expected_errors=(ClientError,))
     async def delete_item(self, key: ModelKey, **kwargs):
         add_fields(pk=key.get("pk"), sk=key.get("sk"))
         await super().delete_item(key, **kwargs)
 
     @log_action(log_level=logging.DEBUG, expected_errors=(ClientError,))
-    async def query(self, **kwargs) -> QueryOutputTableTypeDef:
+    async def query(self, **kwargs) -> QueryOutputTypeDef:
         add_fields(**kwargs)
         return await super().query(**kwargs)
 
     @log_action(log_level=logging.DEBUG, expected_errors=(ClientError,))
     async def query_items(self, **kwargs) -> PagedItems[dict]:
         add_fields(**kwargs)
         return await super().query_items(**kwargs)
@@ -242,15 +242,15 @@
 
     @log_action(log_level=logging.DEBUG, expected_errors=(ClientError,))
     async def query_count(self, **kwargs) -> int:
         add_fields(**kwargs)
         return await super().query_count(**kwargs)
 
     @log_action(log_level=logging.DEBUG, log_args=["key"], expected_errors=(ClientError,))
-    async def update_item(self, key: ModelKey, duration_warning: float = 1, **kwargs) -> UpdateItemOutputTableTypeDef:
+    async def update_item(self, key: ModelKey, duration_warning: float = 1, **kwargs) -> UpdateItemOutputTypeDef:
         res = await maybe_log_warning(super().update_item_with_retry_info(key, **kwargs), duration_warning)
         return res
 
     @log_action(log_level=logging.DEBUG, expected_errors=(ClientError,))
     async def transact_write(self, actions: list[dict[str, Any]]):
         return await super().transact_write(actions)
```

### Comparing `mesh_common-0.1.5/mesh_common/test_helpers.py` & `mesh_common-0.1.6/mesh_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/test_helpers_logs.py` & `mesh_common-0.1.6/mesh_common/test_helpers_logs.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/mesh_common/text.py` & `mesh_common-0.1.6/mesh_common/text.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/pyproject.toml` & `mesh_common-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mesh_common"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "mesh_common" },
     { include = "tests", format = "sdist" },
 ]
@@ -16,15 +16,15 @@
 boto3 = "^1.26.159"
 boto3-stubs = {extras = ["s3", "ssm", "secretsmanager", "dynamodb", "sqs", "lambda", "logs", "sns", "events"], version = "^1.26.159"}
 httpx = "^0.24.1"
 types-urllib3 = "^1.26.25.13"
 types-cryptography = "^3.3.23.2"
 types-python-dateutil = "^2.8.19.13"
 nhs-context-logging = "^0.2.5"
-nhs-aws-helpers = "^0.2.1"
+nhs-aws-helpers = "^0.2.2"
 
 [tool.setuptools.package-data]
 "mesh_common" = ["py.typed"]
 
 [tool.poetry.group.dev.dependencies]
 # ci / testing dependencies
 black = "^22.12.0"
```

### Comparing `mesh_common-0.1.5/tests/common_tests.py` & `mesh_common-0.1.6/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/concurrency_tests.py` & `mesh_common-0.1.6/tests/concurrency_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/conftest.py` & `mesh_common-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/encoding_tests.py` & `mesh_common-0.1.6/tests/encoding_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/env_config_tests.py` & `mesh_common-0.1.6/tests/env_config_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/httpx_retry_transport_tests.py` & `mesh_common-0.1.6/tests/httpx_retry_transport_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/singletons_tests.py` & `mesh_common-0.1.6/tests/singletons_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/tests/test_helpers_tests.py` & `mesh_common-0.1.6/tests/test_helpers_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.1.5/PKG-INFO` & `mesh_common-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mesh-common
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.159,<2.0.0)
 Requires-Dist: boto3-stubs[dynamodb,events,lambda,logs,s3,secretsmanager,sns,sqs,ssm] (>=1.26.159,<2.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: nhs-aws-helpers (>=0.2.1,<0.3.0)
+Requires-Dist: nhs-aws-helpers (>=0.2.2,<0.3.0)
 Requires-Dist: nhs-context-logging (>=0.2.5,<0.3.0)
 Requires-Dist: types-cryptography (>=3.3.23.2,<4.0.0.0)
 Requires-Dist: types-python-dateutil (>=2.8.19.13,<3.0.0.0)
 Requires-Dist: types-urllib3 (>=1.26.25.13,<2.0.0.0)
 Description-Content-Type: text/markdown
 
 # MESH Common
```

