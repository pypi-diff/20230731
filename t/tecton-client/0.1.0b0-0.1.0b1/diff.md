# Comparing `tmp/tecton_client-0.1.0b0.tar.gz` & `tmp/tecton_client-0.1.0b1.tar.gz`

## Comparing `tecton_client-0.1.0b0.tar` & `tecton_client-0.1.0b1.tar`

### file list

```diff
@@ -1,34 +1,42 @@
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/requirements.txt
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/.github/pull_request_template.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/.github/workflows/testing.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/client_options.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/data_types.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/exceptions.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/http_client.py
--rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/requests.py
--rw-r--r--   0        0        0    12121 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/responses.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/tecton_client.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tecton_client/utils.py
--rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/data_types_test.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/http_client_test.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/requests_test.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/responses_test.py
--rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/tecton_client_test.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_utils.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response.json
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_list.json
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_long.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_metadata.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_mixed.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_null.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_slo.json
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/tests/test_data/sample_response_struct.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/.gitignore
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/LICENSE.md
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/README.md
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 tecton_client-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/requirements.txt
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/client_options.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/constants.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/data_types.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/exceptions.py
+-rw-r--r--   0        0        0     9201 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/http_client.py
+-rw-r--r--   0        0        0    21998 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/requests.py
+-rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/responses.py
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/tecton_client.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/utils.py
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/data_types_test.py
+-rw-r--r--   0        0        0    10133 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/http_client_test.py
+-rw-r--r--   0        0        0    18904 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/requests_test.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/responses_test.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/tecton_client_test.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_utils.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_1.json
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_2.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_3.json
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_4.json
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response.json
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response_long_slo.json
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response_slo.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response.json
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_list.json
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_long.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_metadata.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_mixed.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_null.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_slo.json
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_struct.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.gitignore
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/LICENSE.md
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/README.md
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/PKG-INFO
```

### Comparing `tecton_client-0.1.0b0/.pre-commit-config.yaml` & `tecton_client-0.1.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/.github/workflows/testing.yml` & `tecton_client-0.1.0b1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tecton_client/client_options.py` & `tecton_client-0.1.0b1/tecton_client/client_options.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tecton_client/data_types.py` & `tecton_client-0.1.0b1/tecton_client/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tecton_client/exceptions.py` & `tecton_client-0.1.0b1/tecton_client/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from enum import Enum
 from typing import Optional
 
+from tecton_client.constants import MAX_MICRO_BATCH_SIZE
+from tecton_client.constants import MIN_MICRO_BATCH_SIZE
+
 
 class TectonException(Exception):
     """Base class for all Tecton specific exceptions."""
 
 
 class TectonClientError(TectonException):
     """Raised for errors thrown by the Python client."""
@@ -36,14 +39,26 @@
     """Raised when one or more parameters passed in the request are invalid."""
 
 
 class InvalidURLError(TectonClientError):
     """Raised when the URL passed is invalid or empty."""
 
 
+class InvalidMicroBatchSizeError(TectonClientError):
+    """Raised when the micro batch size is invalid."""
+
+    def __init__(self) -> None:
+        """Initialize the error class with a custom error message related to micro batch size."""
+        message = (
+            f"Micro batch size for get features batch request must be between {MIN_MICRO_BATCH_SIZE} and "
+            f"{MAX_MICRO_BATCH_SIZE}"
+        )
+        super().__init__(message)
+
+
 class InvalidParameterMessage(str, Enum):
     """Error Messages for Invalid Parameters passed."""
 
     KEY = (
         "API Key cannot be empty. Please ensure that you have set the TECTON_API_KEY environment variable, "
         "or provided a valid API key."
     )
```

### Comparing `tecton_client-0.1.0b0/tests/data_types_test.py` & `tecton_client-0.1.0b1/tests/data_types_test.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/requests_test.py` & `tecton_client-0.1.0b1/tests/requests_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,139 @@
+import json
+import os
+from typing import List
 from typing import Union
 
 import pytest
 
+from tecton_client.constants import DEFAULT_WORKSPACE_NAME
+from tecton_client.exceptions import InvalidMicroBatchSizeError
 from tecton_client.exceptions import InvalidParameterError
 from tecton_client.exceptions import UnsupportedTypeError
-from tecton_client.requests import GetFeatureRequestData
+from tecton_client.requests import GetFeaturesBatchRequest
+from tecton_client.requests import GetFeatureServiceMetadataRequest
+from tecton_client.requests import GetFeaturesMicroBatchRequest
 from tecton_client.requests import GetFeaturesRequest
+from tecton_client.requests import GetFeaturesRequestData
 from tecton_client.requests import MetadataOptions
 from tests.test_utils import dict_equals
 
 
 class TestRequests:
     TEST_WORKSPACE_NAME = "test_workspace_name"
     TEST_FEATURE_SERVICE_NAME = "test_feature_service_name"
 
-    default_get_feature_request_data = GetFeatureRequestData(join_key_map={"test_key": "test_value"})
+    TEST_DATA_PATH = "tests/test_data"
+
+    default_request_data = GetFeaturesRequestData(join_key_map={"test_key": "test_value"})
 
     @pytest.mark.parametrize("key", ["", None])
     def test_error_join_key(self, key: str) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeatureRequestData(join_key_map={key: "test_value"})
+            GetFeaturesRequestData(join_key_map={key: "test_value"})
 
     @pytest.mark.parametrize("key", ["", None])
     def test_error_request_context_key(self, key: str) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeatureRequestData(request_context_map={key: "test_value"})
+            GetFeaturesRequestData(request_context_map={key: "test_value"})
 
     @pytest.mark.parametrize("key", [123, 123.45])
     def test_unsupported_request_context_key(self, key: str) -> None:
         with pytest.raises(UnsupportedTypeError):
-            GetFeatureRequestData(request_context_map={key: "test_value"})
+            GetFeaturesRequestData(request_context_map={key: "test_value"})
 
     def test_empty_join_value(self) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeatureRequestData(join_key_map={"test_key": ""})
+            GetFeaturesRequestData(join_key_map={"test_key": ""})
 
     def test_unsupported_join_value(self) -> None:
         with pytest.raises(UnsupportedTypeError):
-            GetFeatureRequestData(join_key_map={"test_key": 123.45})
+            GetFeaturesRequestData(join_key_map={"test_key": 123.45})
 
     def test_none_join_value(self) -> None:
-        get_feature_request_data = GetFeatureRequestData(join_key_map={"test_key": None})
-        assert get_feature_request_data.join_key_map["test_key"] is None
+        request_data = GetFeaturesRequestData(join_key_map={"test_key": None})
+        assert request_data.join_key_map["test_key"] is None
 
     def test_none_request_context_value(self) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeatureRequestData(request_context_map={"test_key": None})
+            GetFeaturesRequestData(request_context_map={"test_key": None})
 
     def test_empty_request_context_value(self) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeatureRequestData(request_context_map={"test_key": ""})
+            GetFeaturesRequestData(request_context_map={"test_key": ""})
 
     @pytest.mark.parametrize("value", [False, {"test_key": "test_value"}])
     def test_unsupported_request_context_value(self, value: Union[bool, dict]) -> None:
         with pytest.raises(UnsupportedTypeError):
-            GetFeatureRequestData(request_context_map={"test_key": value})
+            GetFeaturesRequestData(request_context_map={"test_key": value})
 
     def test_mixed_type_join_key_value(self) -> None:
-        get_feature_request_data = GetFeatureRequestData(
+        request_data = GetFeaturesRequestData(
             join_key_map={"test_string_key": "test_string_value", "test_long_key": 1234}
         )
-        join_key_map = get_feature_request_data.join_key_map
+        join_key_map = request_data.join_key_map
 
         assert join_key_map is not None
         assert len(join_key_map) == 2
         assert join_key_map.get("test_string_key") == "test_string_value"
         assert join_key_map.get("test_long_key") == "1234"
 
     def test_mixed_type_request_context_key_value(self) -> None:
-        get_feature_request_data = GetFeatureRequestData(
+        request_data = GetFeaturesRequestData(
             request_context_map={
                 "test_string_key": "test_string_value",
                 "test_long_key": 1234,
                 "test_float_key": 123.45,
             }
         )
 
-        request_context_map = get_feature_request_data.request_context_map
+        request_context_map = request_data.request_context_map
 
         assert request_context_map is not None
         assert len(request_context_map) == 3
         assert request_context_map.get("test_string_key") == "test_string_value"
         assert request_context_map.get("test_long_key") == "1234"
         assert request_context_map.get("test_float_key") == 123.45
 
     def test_join_key_and_request_context(self) -> None:
         join_key_map = {"test_join_key_1": "test_join_value_1", "test_join_key_2": "test_join_value_2"}
         request_context_map = {"test_request_context_1": 1234, "test_request_context_2": "test_string_value"}
 
-        get_feature_request_data = GetFeatureRequestData(join_key_map, request_context_map)
+        request_data = GetFeaturesRequestData(join_key_map, request_context_map)
+
+        assert request_data.join_key_map is not None
+        assert request_data.request_context_map is not None
 
-        assert get_feature_request_data.join_key_map is not None
-        assert get_feature_request_data.request_context_map is not None
+        assert len(request_data.join_key_map) == 2
+        assert len(request_data.request_context_map) == 2
 
-        assert len(get_feature_request_data.join_key_map) == 2
-        assert len(get_feature_request_data.request_context_map) == 2
+        assert dict_equals(join_key_map, request_data.join_key_map)
+        assert dict_equals(request_context_map, request_data.request_context_map)
 
-        assert dict_equals(join_key_map, get_feature_request_data.join_key_map)
-        assert dict_equals(request_context_map, get_feature_request_data.request_context_map)
+    def test_empty_maps(self) -> None:
+        with pytest.raises(InvalidParameterError):
+            GetFeaturesRequestData()
 
     @pytest.mark.parametrize("workspace", ["", None])
     def test_error_workspace_name(self, workspace: str) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeaturesRequest(workspace, self.TEST_FEATURE_SERVICE_NAME, self.default_get_feature_request_data)
+            GetFeaturesRequest(workspace, self.TEST_FEATURE_SERVICE_NAME, self.default_request_data)
 
     @pytest.mark.parametrize("feature_service", ["", None])
     def test_error_feature_service_name(self, feature_service: str) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeaturesRequest(self.TEST_WORKSPACE_NAME, feature_service, self.default_get_feature_request_data)
-
-    def test_empty_maps(self) -> None:
-        with pytest.raises(InvalidParameterError):
-            GetFeatureRequestData()
+            GetFeaturesRequest(self.TEST_WORKSPACE_NAME, feature_service, self.default_request_data)
 
     def test_simple_request_with_none_join_key(self) -> None:
-        local_get_feature_request_data = GetFeatureRequestData(
-            join_key_map={"test_key": "test_value", "test_none_key": None}
-        )
+        local_request_data = GetFeaturesRequestData(join_key_map={"test_key": "test_value", "test_none_key": None})
 
         get_features_request = GetFeaturesRequest(
             self.TEST_WORKSPACE_NAME,
             self.TEST_FEATURE_SERVICE_NAME,
-            local_get_feature_request_data,
+            local_request_data,
             {MetadataOptions.NAME, MetadataOptions.DATA_TYPE},
         )
 
         assert get_features_request.ENDPOINT == GetFeaturesRequest.ENDPOINT
         assert get_features_request.workspace_name == self.TEST_WORKSPACE_NAME
         assert get_features_request.feature_service_name == self.TEST_FEATURE_SERVICE_NAME
 
@@ -145,23 +153,23 @@
 
         expected_json_request = {"params": expected_response}
         json_request = get_features_request.to_json()
 
         assert dict_equals(json_request, expected_json_request)
 
     def test_request_with_request_context_map(self) -> None:
-        local_get_feature_request_data = GetFeatureRequestData(
+        local_request_data = GetFeaturesRequestData(
             join_key_map={"test_key": "test_value"},
             request_context_map={"test_key_1": 123.45, "test_key_2": "test_val"},
         )
 
         get_features_request = GetFeaturesRequest(
             self.TEST_WORKSPACE_NAME,
             self.TEST_FEATURE_SERVICE_NAME,
-            local_get_feature_request_data,
+            local_request_data,
             {MetadataOptions.NAME, MetadataOptions.DATA_TYPE},
         )
 
         assert get_features_request.ENDPOINT == GetFeaturesRequest.ENDPOINT
         assert get_features_request.workspace_name == self.TEST_WORKSPACE_NAME
         assert get_features_request.feature_service_name == self.TEST_FEATURE_SERVICE_NAME
 
@@ -185,15 +193,15 @@
 
         assert dict_equals(json_request, expected_json_request)
 
     def test_all_metadata_options(self) -> None:
         get_features_request = GetFeaturesRequest(
             self.TEST_WORKSPACE_NAME,
             self.TEST_FEATURE_SERVICE_NAME,
-            self.default_get_feature_request_data,
+            self.default_request_data,
             {
                 MetadataOptions.NAME,
                 MetadataOptions.SLO_INFO,
                 MetadataOptions.EFFECTIVE_TIME,
                 MetadataOptions.FEATURE_STATUS,
             },
         )
@@ -228,15 +236,15 @@
 
         assert dict_equals(actual_json, expected_json)
 
     def test_custom_metadata_options(self) -> None:
         get_features_request = GetFeaturesRequest(
             self.TEST_WORKSPACE_NAME,
             self.TEST_FEATURE_SERVICE_NAME,
-            self.default_get_feature_request_data,
+            self.default_request_data,
             {MetadataOptions.NAME, MetadataOptions.SLO_INFO},
         )
 
         assert len(get_features_request.metadata_options) == 3
 
         metadata_options = get_features_request.metadata_options
         expected_metadata_options = {MetadataOptions.NAME, MetadataOptions.DATA_TYPE, MetadataOptions.SLO_INFO}
@@ -253,15 +261,15 @@
         expected_json = {"params": expected_response}
         actual_json = get_features_request.to_json()
 
         assert dict_equals(actual_json, expected_json)
 
     def test_default_metadata_options(self) -> None:
         get_features_request = GetFeaturesRequest(
-            self.TEST_WORKSPACE_NAME, self.TEST_FEATURE_SERVICE_NAME, self.default_get_feature_request_data
+            self.TEST_WORKSPACE_NAME, self.TEST_FEATURE_SERVICE_NAME, self.default_request_data
         )
         assert len(get_features_request.metadata_options) == 2
 
         metadata_options = get_features_request.metadata_options
         expected_metadata_options = {MetadataOptions.NAME, MetadataOptions.DATA_TYPE}
 
         assert expected_metadata_options == metadata_options
@@ -273,7 +281,156 @@
             "join_key_map": {"test_key": "test_value"},
         }
 
         expected_json = {"params": expected_response}
         actual_json = get_features_request.to_json()
 
         assert dict_equals(actual_json, expected_json)
+
+    @pytest.mark.parametrize("workspace", ["", None])
+    def test_error_workspace_name_batch(self, workspace: str) -> None:
+        with pytest.raises(InvalidParameterError):
+            GetFeaturesBatchRequest(workspace, self.TEST_FEATURE_SERVICE_NAME, [self.default_request_data])
+
+    @pytest.mark.parametrize("feature_service", ["", None])
+    def test_error_feature_service_name_batch(self, feature_service: str) -> None:
+        with pytest.raises(InvalidParameterError):
+            GetFeaturesBatchRequest(self.TEST_WORKSPACE_NAME, feature_service, [self.default_request_data])
+
+    def test_batch_request_with_none_join_keys(self) -> None:
+        local_request_data = GetFeaturesRequestData(join_key_map={"test_key": "test_value", "test_none_key": None})
+
+        request = GetFeaturesBatchRequest(
+            workspace_name=self.TEST_WORKSPACE_NAME,
+            feature_service_name=self.TEST_FEATURE_SERVICE_NAME,
+            request_data_list=[local_request_data],
+            metadata_options={MetadataOptions.NAME, MetadataOptions.DATA_TYPE},
+            micro_batch_size=1,
+        )
+
+        assert request.workspace_name == self.TEST_WORKSPACE_NAME
+        assert request.feature_service_name == self.TEST_FEATURE_SERVICE_NAME
+
+        for get_features_request in request.request_list:
+            assert get_features_request.ENDPOINT == GetFeaturesRequest.ENDPOINT
+            assert get_features_request.request_data.request_context_map is None
+            assert len(get_features_request.request_data.join_key_map) == 2
+            assert get_features_request.request_data.join_key_map.get("test_key") == "test_value"
+            assert get_features_request.request_data.join_key_map.get("test_none_key") is None
+
+        expected_response = {
+            "feature_service_name": "test_feature_service_name",
+            "workspace_name": "test_workspace_name",
+            "metadata_options": {"include_data_types": True, "include_names": True},
+            "join_key_map": {"test_key": "test_value", "test_none_key": None},
+        }
+
+        expected_json_request = {"params": expected_response}
+        json_requests = request.to_json_list()
+
+        for json_request in json_requests:
+            assert dict_equals(json_request, expected_json_request)
+
+    request_list = [
+        GetFeaturesRequestData(join_key_map={"test_key": "test_value"}),
+        GetFeaturesRequestData(request_context_map={"test_key": "test_value"}),
+        GetFeaturesRequestData(join_key_map={"test_key": "test_value"}, request_context_map={"test_key": "test_value"}),
+    ]
+
+    @pytest.mark.parametrize(
+        "request_list, micro_batch_size, expected_json_file_name",
+        [
+            (request_list, 1, "batch_expected_request_1"),
+            (request_list, 2, "batch_expected_request_2"),
+            (request_list, 3, "batch_expected_request_3"),
+            (request_list, 4, "batch_expected_request_3"),
+            (request_list * 7, 3, "batch_expected_request_4"),
+        ],
+    )
+    def test_batch_requests(
+        self, request_list: List[GetFeaturesRequestData], micro_batch_size: int, expected_json_file_name: str
+    ) -> None:
+        with open(os.path.join(self.TEST_DATA_PATH, "batch", f"{expected_json_file_name}.json"), "r") as f:
+            expected_json_list = json.load(f)
+
+        get_features_request_batch = GetFeaturesBatchRequest(
+            workspace_name=self.TEST_WORKSPACE_NAME,
+            feature_service_name=self.TEST_FEATURE_SERVICE_NAME,
+            request_data_list=request_list,
+            metadata_options={MetadataOptions.NAME, MetadataOptions.SLO_INFO},
+            micro_batch_size=micro_batch_size,
+        )
+
+        if micro_batch_size != 1:
+            assert get_features_request_batch.request_list[0].ENDPOINT == GetFeaturesMicroBatchRequest.ENDPOINT
+
+        for actual_json, expected_json in zip(get_features_request_batch.to_json_list(), expected_json_list):
+            assert dict_equals(actual_json, expected_json)
+
+    @pytest.mark.parametrize("request_list", [[], [None]])
+    def test_error_batch_request_list(self, request_list: List[GetFeaturesRequestData]) -> None:
+        with pytest.raises(InvalidParameterError):
+            GetFeaturesBatchRequest(
+                workspace_name=self.TEST_WORKSPACE_NAME,
+                feature_service_name=self.TEST_FEATURE_SERVICE_NAME,
+                request_data_list=request_list,
+                metadata_options={MetadataOptions.NAME, MetadataOptions.DATA_TYPE},
+                micro_batch_size=1,
+            )
+
+    @pytest.mark.parametrize("micro_batch_size", [-1, 0, 11])
+    def test_error_micro_batch_size(self, micro_batch_size: int) -> None:
+        with pytest.raises(InvalidMicroBatchSizeError):
+            GetFeaturesBatchRequest(
+                workspace_name=self.TEST_WORKSPACE_NAME,
+                feature_service_name=self.TEST_FEATURE_SERVICE_NAME,
+                request_data_list=self.request_list,
+                metadata_options={MetadataOptions.NAME, MetadataOptions.DATA_TYPE},
+                micro_batch_size=micro_batch_size,
+            )
+
+    @pytest.mark.parametrize(
+        "workspace_name, expected_response",
+        [
+            (
+                TEST_WORKSPACE_NAME,
+                {
+                    "feature_service_name": "test_feature_service_name",
+                    "workspace_name": "test_workspace_name",
+                },
+            ),
+            (
+                None,
+                {
+                    "feature_service_name": "test_feature_service_name",
+                    "workspace_name": "prod",
+                },
+            ),
+            (
+                "",
+                {
+                    "feature_service_name": "test_feature_service_name",
+                    "workspace_name": "prod",
+                },
+            ),
+        ],
+    )
+    def test_metadata_request(self, workspace_name: str, expected_response: dict) -> None:
+        request = GetFeatureServiceMetadataRequest(
+            feature_service_name=self.TEST_FEATURE_SERVICE_NAME, workspace_name=workspace_name
+        )
+        if workspace_name:
+            assert request.workspace_name == workspace_name
+        else:
+            assert request.workspace_name == DEFAULT_WORKSPACE_NAME
+
+        assert request.feature_service_name == self.TEST_FEATURE_SERVICE_NAME
+        assert request.ENDPOINT == GetFeatureServiceMetadataRequest.ENDPOINT
+
+        assert request.to_json() == {"params": expected_response}
+
+    @pytest.mark.parametrize("feature_service", ["", None])
+    def test_error_feature_service_name_metadata(self, feature_service: str) -> None:
+        with pytest.raises(InvalidParameterError):
+            GetFeatureServiceMetadataRequest(
+                workspace_name=self.TEST_WORKSPACE_NAME, feature_service_name=feature_service
+            )
```

### Comparing `tecton_client-0.1.0b0/tests/tecton_client_test.py` & `tecton_client-0.1.0b1/tests/tecton_client_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 from tecton_client.exceptions import GatewayTimeoutError
 from tecton_client.exceptions import InvalidParameterError
 from tecton_client.exceptions import NotFoundError
 from tecton_client.exceptions import ResourcesExhaustedError
 from tecton_client.exceptions import ServiceUnavailableError
 from tecton_client.exceptions import TectonServerException
 from tecton_client.exceptions import UnauthorizedError
-from tecton_client.requests import GetFeatureRequestData
+from tecton_client.requests import GetFeaturesBatchRequest
 from tecton_client.requests import GetFeaturesRequest
+from tecton_client.requests import GetFeaturesRequestData
 from tecton_client.requests import MetadataOptions
 from tecton_client.responses import FeatureStatus
 from tecton_client.tecton_client import TectonClient
 from tecton_client.tecton_client import TectonClientOptions
 from tests.test_utils import dict_equals
 
 
@@ -37,16 +38,19 @@
 
 
 class TestTectonClient:
     api_key: Final[str] = "1234"
     url: Final[str] = "https://thisisaurl.ai"
 
     final_url: Final[str] = urljoin(url, "api/v1/feature-service/get-features")
+    batch_url: Final[str] = urljoin(url, "api/v1/feature-service/get-features-batch")
 
-    TEST_DATA_REL_PATH: Final[str] = "tests/test_data/"
+    TEST_DATA_ROOT: Final[str] = "tests/test_data/"
+    TEST_DATA_REL_PATH_SINGLE: Final[str] = os.path.join(TEST_DATA_ROOT, "single/")
+    TEST_DATA_REL_PATH_BATCH: Final[str] = os.path.join(TEST_DATA_ROOT, "batch/")
 
     expected_response_mixed = {
         "test.output_struct1": None,
         "test.output_struct2": {"float64_field": 2.46, "string_field": "2.46"},
         "test.output_array": [1, 2, 3, None, 5],
         "test.output_string": "test",
         "test.output_int1": 24,
@@ -104,60 +108,67 @@
     }
 
     join_key_map = {"test_join_key_1": "test_join_value_1", "test_join_key_2": "test_join_value_2"}
     request_context_map = {"test_request_context_1": 1234, "test_request_context_2": "test_string_value"}
 
     test_request_normal = GetFeaturesRequest(
         feature_service_name="test_feature_service",
-        request_data=GetFeatureRequestData(join_key_map, request_context_map),
+        request_data=GetFeaturesRequestData(join_key_map, request_context_map),
         workspace_name="test-workspace",
     )
     test_request_metadata = GetFeaturesRequest(
         feature_service_name="test_feature_service",
-        request_data=GetFeatureRequestData(join_key_map, request_context_map),
+        request_data=GetFeaturesRequestData(join_key_map, request_context_map),
         workspace_name="test-workspace",
         metadata_options={MetadataOptions.SLO_INFO, MetadataOptions.FEATURE_STATUS, MetadataOptions.EFFECTIVE_TIME},
     )
+    test_request_batch = GetFeaturesBatchRequest(
+        feature_service_name="test_feature_service",
+        request_data_list=[GetFeaturesRequestData(join_key_map, request_context_map)] * 10,
+        workspace_name="test-workspace",
+        metadata_options={MetadataOptions.SLO_INFO, MetadataOptions.FEATURE_STATUS, MetadataOptions.EFFECTIVE_TIME},
+        micro_batch_size=5,
+    )
+
+    tecton_client = TectonClient(url=url, api_key=api_key)
 
     @pytest.mark.parametrize(
         "file_name, expected_response",
         [
             ("sample_response_mixed.json", expected_response_mixed),
             ("sample_response_long.json", expected_response_long),
         ],
     )
     def test_get_features(self, mocked: aioresponses, file_name: str, expected_response: dict) -> None:
-        tecton_client = TectonClient(TestTectonClient.url, TestTectonClient.api_key)
+        TectonClient(TestTectonClient.url, TestTectonClient.api_key)
 
-        with open(f"{TestTectonClient.TEST_DATA_REL_PATH}{file_name}") as json_file:
+        with open(os.path.join(TestTectonClient.TEST_DATA_REL_PATH_SINGLE, file_name)) as json_file:
             mocked.post(url=self.final_url, payload=json.load(json_file))
-            response = tecton_client.get_features(self.test_request_normal)
+            response = self.tecton_client.get_features(self.test_request_normal)
 
         assert dict_equals({k: v.feature_value for k, v in response.feature_values.items()}, expected_response)
-        tecton_client.close()
 
     @pytest.mark.parametrize("metadata_path, expected_metadata", [("sample_response_metadata.json", expected_metadata)])
     def test_get_features_metadata(self, mocked: aioresponses, metadata_path: str, expected_metadata: list) -> None:
-        tecton_client = TectonClient(TestTectonClient.url, TestTectonClient.api_key)
-        with open(f"{TestTectonClient.TEST_DATA_REL_PATH}{metadata_path}") as json_file:
+        TectonClient(TestTectonClient.url, TestTectonClient.api_key)
+        with open(os.path.join(TestTectonClient.TEST_DATA_REL_PATH_SINGLE, metadata_path)) as json_file:
             mocked.post(url=self.final_url, payload=json.load(json_file))
-            response = tecton_client.get_features(self.test_request_metadata)
+            response = self.tecton_client.get_features(self.test_request_metadata)
 
         assert response.slo_info is not None
         assert dict_equals(vars(response.slo_info), self.expected_slo_info)
 
         for feature, metadata in zip(response.feature_values.values(), expected_metadata):
             assert isinstance(feature.data_type, metadata[0])
             assert feature.feature_status == metadata[1]
             assert feature.effective_time.isoformat(timespec="seconds") == metadata[2]
 
         assert dict_equals(
             {k: v.feature_value for k, v in response.feature_values.items()}, self.expected_response_metadata
         )
-        tecton_client.close()
 
     @pytest.mark.parametrize(
         "exception, status_code, error_json",
         [
             (
                 BadRequestError,
                 400,
@@ -224,23 +235,21 @@
                 {"error": "Timed out", "message": "Timed out", "code": 4},
             ),
         ],
     )
     def test_get_features_error_response(
         self, mocked: aioresponses, exception: TectonServerException, status_code: int, error_json: dict
     ) -> None:
-        tecton_client = TectonClient(TestTectonClient.url, TestTectonClient.api_key)
         with pytest.raises(exception):
             mocked.post(
                 url=self.final_url,
                 status=status_code,
                 payload=error_json,
             )
-            tecton_client.get_features(self.test_request_normal)
-        tecton_client.close()
+            self.tecton_client.get_features(self.test_request_normal)
 
     def test_error_response_no_duplicate_codes(self) -> None:
         response_codes = set()
         for exception in TectonServerException.__subclasses__():
             assert exception.STATUS_CODE not in response_codes
             response_codes.add(exception.STATUS_CODE)
 
@@ -256,30 +265,32 @@
     def test_custom_client_with_options(self, mocked: aioresponses, client: aiohttp.ClientSession) -> None:
         if client is None:
             client_options = TectonClientOptions(
                 connect_timeout=timedelta(seconds=10),
                 read_timeout=timedelta(seconds=15),
                 keepalive_expiry=timedelta(seconds=500),
             )
-            tecton_client = TectonClient(TestTectonClient.url, TestTectonClient.api_key, client_options=client_options)
+            local_tecton_client = TectonClient(
+                TestTectonClient.url, TestTectonClient.api_key, client_options=client_options
+            )
             assert client_options.connect_timeout.seconds == 10
             assert client_options.read_timeout.seconds == 15
             assert client_options.keepalive_expiry.seconds == 500
             assert client_options.max_connections == 10
         else:
-            tecton_client = TectonClient(TestTectonClient.url, TestTectonClient.api_key, client=client)
+            local_tecton_client = TectonClient(TestTectonClient.url, TestTectonClient.api_key, client=client)
 
-        with open(f"{TestTectonClient.TEST_DATA_REL_PATH}sample_response_mixed.json") as json_file:
+        with open(os.path.join(TestTectonClient.TEST_DATA_REL_PATH_SINGLE, "sample_response_mixed.json")) as json_file:
             mocked.post(url=self.final_url, payload=json.load(json_file))
-            response = tecton_client.get_features(self.test_request_normal)
+            response = local_tecton_client.get_features(self.test_request_normal)
 
         assert dict_equals(
             {k: v.feature_value for k, v in response.feature_values.items()}, self.expected_response_mixed
         )
-        tecton_client.close()
+        local_tecton_client.close()
 
     def test_no_api_key(self) -> None:
         # Testing that no API key is provided as a parameter and the environment variable `TECTON_API_KEY` is not set
         with pytest.raises(InvalidParameterError):
             TectonClient(url="https://thisisaurl.ai")
 
     def test_api_key_env_var(self) -> None:
@@ -292,7 +303,40 @@
     async def test_client_and_client_options(self) -> None:
         client = aiohttp.ClientSession(connector=aiohttp.TCPConnector(limit=2))
         with pytest.raises(InvalidParameterError):
             TectonClient(
                 url="https://thisisaurl.ai", client_options=TectonClientOptions(max_connections=1), client=client
             )
         await client.close()
+
+    @pytest.mark.parametrize(
+        "file_name, feature_vector_len, feature_name, order_of_responses",
+        [
+            (
+                "sample_batch_response_long_slo.json",
+                14,
+                "user_distinct_merchant_transaction_count_30d.distinct_merchant_transaction_count_30d",
+                [672, 668, 697, 690, 688, 685, 676, 672, 668, 697, 690, 688, 685, 676],
+            ),
+        ],
+    )
+    def test_get_features_batch(
+        self, mocked: aioresponses, file_name: str, feature_vector_len: int, feature_name: str, order_of_responses: list
+    ) -> None:
+        with open(f"{TestTectonClient.TEST_DATA_REL_PATH_BATCH}{file_name}") as json_file:
+            mocked.post(url=self.batch_url, payload=json.load(json_file), repeat=True)
+            batch_response = self.tecton_client.get_features_batch(self.test_request_batch)
+
+            # Test that the number of feature values in each response corresponds to the individual
+            # feature vector length
+            assert all(
+                len(response.feature_values) == feature_vector_len for response in batch_response.batch_response_list
+            )
+
+            # Test that the order of responses is retained by comparing a random feature within each response
+            assert all(
+                response.feature_values[feature_name].feature_value == order_of_responses.pop(0)
+                for response in batch_response.batch_response_list
+            )
+
+    def pytest_sessionfinish(self) -> None:
+        self.tecton_client.close()
```

### Comparing `tecton_client-0.1.0b0/tests/test_utils.py` & `tecton_client-0.1.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_list.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_list.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_long.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_long.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_metadata.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_metadata.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_mixed.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_mixed.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_null.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_null.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_slo.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_slo.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/tests/test_data/sample_response_struct.json` & `tecton_client-0.1.0b1/tests/test_data/single/sample_response_struct.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/LICENSE.md` & `tecton_client-0.1.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/README.md` & `tecton_client-0.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/pyproject.toml` & `tecton_client-0.1.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b0/PKG-INFO` & `tecton_client-0.1.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tecton-client
-Version: 0.1.0b0
+Version: 0.1.0b1
 Summary: A Python Client for the Tecton FeatureService API
 Project-URL: Source, https://github.com/tecton-ai/tecton-http-client-python
 Project-URL: Documentation, https://tecton-ai.github.io/tecton-http-client-python/html/index.html
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 Requires-Python: >=3.8
 Requires-Dist: aiohttp~=3.8.4
 Requires-Dist: aioresponses~=0.7.4
+Requires-Dist: nest-asyncio~=1.5.6
 Requires-Dist: pytest~=7.3.1
 Description-Content-Type: text/markdown
 
 # Python Client Library for Tecton Online Feature Store
 
 A simple Python client for the Feature Server HTTP API that helps customers integrate with Tecton easily.
```

