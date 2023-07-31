# Comparing `tmp/nhs_aws_helpers-0.2.1.tar.gz` & `tmp/nhs_aws_helpers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_aws_helpers-0.2.1.tar", max compression
+gzip compressed data, was "nhs_aws_helpers-0.2.2.tar", max compression
```

## Comparing `nhs_aws_helpers-0.2.1.tar` & `nhs_aws_helpers-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1078 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/LICENSE.md
--rw-r--r--   0        0        0      666 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/README.md
--rw-r--r--   0        0        0    39862 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/__init__.py
--rw-r--r--   0        0        0     7980 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_reader.py
--rw-r--r--   0        0        0     6673 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_writer.py
--rw-r--r--   0        0        0     1331 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/common.py
--rw-r--r--   0        0        0        0 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/base_model.py
--rw-r--r--   0        0        0    26465 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/base_model_store.py
--rw-r--r--   0        0        0     4618 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/fixtures.py
--rw-r--r--   0        0        0        0 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/py.typed
--rw-r--r--   0        0        0     7916 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_reader.py
--rw-r--r--   0        0        0     6681 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_writer.py
--rw-r--r--   0        0        0     3056 2023-07-07 19:42:25.635909 nhs_aws_helpers-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0    10996 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/async_s3_object_buffer_tests.py
--rw-r--r--   0        0        0     7558 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/aws_tests.py
--rw-r--r--   0        0        0    21983 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/base_model_store_tests.py
--rw-r--r--   0        0        0      280 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     2272 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/ddb_tests.py
--rw-r--r--   0        0        0    10316 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/s3_object_buffer_tests.py
--rw-r--r--   0        0        0      518 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/utils.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0      666 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/README.md
+-rw-r--r--   0        0        0    39862 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/__init__.py
+-rw-r--r--   0        0        0     7980 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/async_s3_object_reader.py
+-rw-r--r--   0        0        0     6673 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/async_s3_object_writer.py
+-rw-r--r--   0        0        0     1331 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/common.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/dynamodb_model_store/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/dynamodb_model_store/base_model.py
+-rw-r--r--   0        0        0    26408 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/dynamodb_model_store/base_model_store.py
+-rw-r--r--   0        0        0     4618 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/py.typed
+-rw-r--r--   0        0        0     7916 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/s3_object_reader.py
+-rw-r--r--   0        0        0     6681 2023-07-31 09:57:30.836442 nhs_aws_helpers-0.2.2/nhs_aws_helpers/s3_object_writer.py
+-rw-r--r--   0        0        0     3056 2023-07-31 09:57:56.036902 nhs_aws_helpers-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0    10996 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/async_s3_object_buffer_tests.py
+-rw-r--r--   0        0        0     7558 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/aws_tests.py
+-rw-r--r--   0        0        0    21991 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/base_model_store_tests.py
+-rw-r--r--   0        0        0      280 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     2272 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/ddb_tests.py
+-rw-r--r--   0        0        0    10316 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/s3_object_buffer_tests.py
+-rw-r--r--   0        0        0      518 2023-07-31 09:57:30.840442 nhs_aws_helpers-0.2.2/tests/utils.py
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.2.2/PKG-INFO
```

### Comparing `nhs_aws_helpers-0.2.1/LICENSE.md` & `nhs_aws_helpers-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/README.md` & `nhs_aws_helpers-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/__init__.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_reader.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/async_s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_writer.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/async_s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/common.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/common.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/base_model.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/dynamodb_model_store/base_model.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/base_model_store.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/dynamodb_model_store/base_model_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 )
 
 from boto3.dynamodb.conditions import Attr, Key
 from botocore.exceptions import ClientError
 from mypy_boto3_dynamodb import DynamoDBClient
 from mypy_boto3_dynamodb.service_resource import DynamoDBServiceResource, Table
 from mypy_boto3_dynamodb.type_defs import (
-    BatchGetItemOutputServiceResourceTypeDef,
-    QueryOutputTableTypeDef,
+    BatchGetItemOutputTypeDef,
+    QueryOutputTypeDef,
     TransactGetItemTypeDef,
-    UpdateItemOutputTableTypeDef,
-    WriteRequestTypeDef,
+    UpdateItemOutputTypeDef,
+    WriteRequestOutputTypeDef,
 )
 
 from nhs_aws_helpers import dynamodb, dynamodb_retry_backoff
 from nhs_aws_helpers.common import (
     is_dataclass_instance,
     optional_origin_type,
     run_in_executor,
@@ -456,15 +456,15 @@
     ) -> AsyncGenerator[PagedItems[dict], None]:
         async for page in self.paginate(paginator_type, **kwargs):
             items = page.get("Items", [])
             last_evaluated_key = page.get("LastEvaluatedKey", None)
             yield PagedItems(items, last_evaluated_key)
 
     @dynamodb_retry_backoff()
-    async def query(self, **kwargs) -> QueryOutputTableTypeDef:
+    async def query(self, **kwargs) -> QueryOutputTypeDef:
         return await run_in_executor(self.table.query, **kwargs)
 
     async def query_items(self, **kwargs) -> PagedItems[dict]:
         page = await self.query(**kwargs)
         return PagedItems(page.get("Items", []), cast(Optional[Dict[str, Any]], page.get("LastEvaluatedKey", None)))
 
     @dynamodb_retry_backoff()
@@ -498,27 +498,27 @@
     async def transact_write(self, actions: List[Dict[str, Any]]):
         transaction = self._prepare_transaction(actions=actions, table_name=self._table_name)
         return await self.transact_write_items(transaction)
 
     @dynamodb_retry_backoff()
     async def update_item_with_retry_info(
         self, key: TModelKey, **kwargs
-    ) -> Tuple[UpdateItemOutputTableTypeDef, float, str, int]:
+    ) -> Tuple[UpdateItemOutputTypeDef, float, str, int]:
         kwargs["Key"] = cast(Dict[str, str], key)
 
         started = time()
         response = await run_in_executor(self.table.update_item, **kwargs)
         duration = time() - started
 
         aws_request_id = response["ResponseMetadata"]["RequestId"]
         aws_retries = response["ResponseMetadata"]["RetryAttempts"]
 
         return response, duration, aws_request_id, aws_retries
 
-    async def update_item(self, key: TModelKey, **kwargs) -> UpdateItemOutputTableTypeDef:
+    async def update_item(self, key: TModelKey, **kwargs) -> UpdateItemOutputTypeDef:
 
         response, _, _, _ = await self.update_item_with_retry_info(key, **kwargs)
         return response
 
     def batch_writer(self, flush_amount: int = 25) -> "_AsyncBatchWriter":
         return _AsyncBatchWriter(
             store=self,
@@ -572,17 +572,15 @@
     async def query_all_models(self, model_type: Type[TBaseModel_co], **kwargs) -> List[TBaseModel_co]:
         result = []
 
         async for models, _ in self.paginate_models("query", model_type, **kwargs):
             result.extend(models)
         return result
 
-    def _get_batch_results(
-        self, response: BatchGetItemOutputServiceResourceTypeDef
-    ) -> Tuple[List[Dict[str, Any]], List[TModelKey]]:
+    def _get_batch_results(self, response: BatchGetItemOutputTypeDef) -> Tuple[List[Dict[str, Any]], List[TModelKey]]:
         assert response["ResponseMetadata"]["HTTPStatusCode"] == 200
         results: List[Dict[str, Any]] = response.get("Responses", {}).get(self._table_name) or []
         unprocessed_keys: Dict[str, Any] = response.get("UnprocessedKeys", {})
         unprocessed = cast(List[TModelKey], unprocessed_keys.get(self._table_name, {}).get("Keys") or [])
 
         return results, unprocessed
 
@@ -666,15 +664,15 @@
     """
 
     def __init__(self, store: BaseModelStore, flush_amount=25):
 
         self._store = store
         self._table_name = store.table.table_name
         self._client = store.client
-        self._items_buffer: List[WriteRequestTypeDef] = []
+        self._items_buffer: List[WriteRequestOutputTypeDef] = []
         self._flush_amount = flush_amount
         self._overwrite_by_keys = store.table_key_fields
 
     async def put_item(self, item, **kwargs):
         await self._add_request_and_process({"PutRequest": {"Item": self._store.serialise_value(item, **kwargs)}})
 
     async def delete_item(self, key, **kwargs):
```

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/fixtures.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_reader.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_writer.py` & `nhs_aws_helpers-0.2.2/nhs_aws_helpers/s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/pyproject.toml` & `nhs_aws_helpers-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_aws_helpers"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "nhs_aws_helpers" },
     { include = "tests", format = "sdist" },
 ]
```

### Comparing `nhs_aws_helpers-0.2.1/tests/async_s3_object_buffer_tests.py` & `nhs_aws_helpers-0.2.2/tests/async_s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/tests/aws_tests.py` & `nhs_aws_helpers-0.2.2/tests/aws_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/tests/base_model_store_tests.py` & `nhs_aws_helpers-0.2.2/tests/base_model_store_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,27 +314,27 @@
     expected = MyDerivedModel(id=uuid4().hex)
 
     await store.put_model(expected)
 
     actual = await store.get_model(expected.model_key(), MyDerivedModel)
 
     assert actual
-    assert type(actual) == MyDerivedModel
+    assert isinstance(actual, MyDerivedModel)
 
 
 async def test_store_put_update_get_model(store: MyModelStore):
 
     expected = MyDerivedModel(id=uuid4().hex)
 
     await store.put_model(expected)
 
     actual = await store.get_model(expected.model_key(), MyDerivedModel)
 
     assert actual
-    assert type(actual) == MyDerivedModel
+    assert isinstance(actual, MyDerivedModel)
 
     await store.update_item(
         expected.model_key(), UpdateExpression="SET optional_thing = :val", ExpressionAttributeValues={":val": "BOB"}
     )
 
     actual = await store.get_model(expected.model_key(), MyDerivedModel)
     assert actual
```

### Comparing `nhs_aws_helpers-0.2.1/tests/ddb_tests.py` & `nhs_aws_helpers-0.2.2/tests/ddb_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/tests/s3_object_buffer_tests.py` & `nhs_aws_helpers-0.2.2/tests/s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/tests/utils.py` & `nhs_aws_helpers-0.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.2.1/PKG-INFO` & `nhs_aws_helpers-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-aws-helpers
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

