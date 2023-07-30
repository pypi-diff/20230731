# Comparing `tmp/iomete_sdk-1.2.1.tar.gz` & `tmp/iomete_sdk-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iomete_sdk-1.2.1.tar", last modified: Tue Jul 25 18:02:34 2023, max compression
+gzip compressed data, was "iomete_sdk-1.2.2.tar", last modified: Sun Jul 30 23:57:20 2023, max compression
```

## Comparing `iomete_sdk-1.2.1.tar` & `iomete_sdk-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.894188 iomete_sdk-1.2.1/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-25 18:02:34.894249 iomete_sdk-1.2.1/PKG-INFO
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2038 2023-07-19 22:03:57.000000 iomete_sdk-1.2.1/README.md
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       38 2023-07-25 18:02:34.894407 iomete_sdk-1.2.1/setup.cfg
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     1407 2023-07-25 18:01:42.000000 iomete_sdk-1.2.1/setup.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.890796 iomete_sdk-1.2.1/src/
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.891380 iomete_sdk-1.2.1/src/iomete_sdk/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     1298 2023-07-25 03:41:17.000000 iomete_sdk-1.2.1/src/iomete_sdk/api_utils.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.892889 iomete_sdk-1.2.1/src/iomete_sdk/security/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       68 2023-07-17 22:30:18.000000 iomete_sdk-1.2.1/src/iomete_sdk/security/__init__.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     7487 2023-07-25 17:59:20.000000 iomete_sdk-1.2.1/src/iomete_sdk/security/data_security.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     3719 2023-07-25 17:58:18.000000 iomete_sdk-1.2.1/src/iomete_sdk/security/policy_models.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.893312 iomete_sdk-1.2.1/src/iomete_sdk/spark/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       57 2023-07-17 22:30:18.000000 iomete_sdk-1.2.1/src/iomete_sdk/spark/__init__.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2658 2023-07-18 22:38:50.000000 iomete_sdk-1.2.1/src/iomete_sdk/spark/spark_job.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.892280 iomete_sdk-1.2.1/src/iomete_sdk.egg-info/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-25 18:02:34.000000 iomete_sdk-1.2.1/src/iomete_sdk.egg-info/PKG-INFO
--rw-r--r--   0 fuadmusayev   (501) staff       (20)      504 2023-07-25 18:02:34.000000 iomete_sdk-1.2.1/src/iomete_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 fuadmusayev   (501) staff       (20)        1 2023-07-25 18:02:34.000000 iomete_sdk-1.2.1/src/iomete_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       56 2023-07-25 18:02:34.000000 iomete_sdk-1.2.1/src/iomete_sdk.egg-info/requires.txt
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       11 2023-07-25 18:02:34.000000 iomete_sdk-1.2.1/src/iomete_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 18:02:34.893914 iomete_sdk-1.2.1/tests/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)    11694 2023-07-25 03:41:33.000000 iomete_sdk-1.2.1/tests/test_data_security_api_client.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     4529 2023-07-18 20:56:50.000000 iomete_sdk-1.2.1/tests/test_spark_job_api_client.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.462952 iomete_sdk-1.2.2/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-30 23:57:20.463000 iomete_sdk-1.2.2/PKG-INFO
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2038 2023-07-19 22:03:57.000000 iomete_sdk-1.2.2/README.md
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       38 2023-07-30 23:57:20.463146 iomete_sdk-1.2.2/setup.cfg
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     1407 2023-07-30 23:57:12.000000 iomete_sdk-1.2.2/setup.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.459592 iomete_sdk-1.2.2/src/
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.460170 iomete_sdk-1.2.2/src/iomete_sdk/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     1298 2023-07-25 03:41:17.000000 iomete_sdk-1.2.2/src/iomete_sdk/api_utils.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.461808 iomete_sdk-1.2.2/src/iomete_sdk/security/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       68 2023-07-17 22:30:18.000000 iomete_sdk-1.2.2/src/iomete_sdk/security/__init__.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     7484 2023-07-30 23:54:45.000000 iomete_sdk-1.2.2/src/iomete_sdk/security/data_security.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     3719 2023-07-25 17:58:18.000000 iomete_sdk-1.2.2/src/iomete_sdk/security/policy_models.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.462221 iomete_sdk-1.2.2/src/iomete_sdk/spark/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       57 2023-07-17 22:30:18.000000 iomete_sdk-1.2.2/src/iomete_sdk/spark/__init__.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2658 2023-07-18 22:38:50.000000 iomete_sdk-1.2.2/src/iomete_sdk/spark/spark_job.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.461192 iomete_sdk-1.2.2/src/iomete_sdk.egg-info/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-30 23:57:20.000000 iomete_sdk-1.2.2/src/iomete_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)      504 2023-07-30 23:57:20.000000 iomete_sdk-1.2.2/src/iomete_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)        1 2023-07-30 23:57:20.000000 iomete_sdk-1.2.2/src/iomete_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       56 2023-07-30 23:57:20.000000 iomete_sdk-1.2.2/src/iomete_sdk.egg-info/requires.txt
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       11 2023-07-30 23:57:20.000000 iomete_sdk-1.2.2/src/iomete_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-30 23:57:20.462718 iomete_sdk-1.2.2/tests/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)    11678 2023-07-30 23:57:03.000000 iomete_sdk-1.2.2/tests/test_data_security_api_client.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     4529 2023-07-18 20:56:50.000000 iomete_sdk-1.2.2/tests/test_spark_job_api_client.py
```

### Comparing `iomete_sdk-1.2.1/PKG-INFO` & `iomete_sdk-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iomete_sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: IOMETE SDK for Python.
 Home-page: https://github.com/iomete/iomete-sdk
 Author: IOMETE
 Author-email: vusal@iomete.com
 License: Apache License 2.0
 Keywords: iomete,sdk,spark-job,data-security-api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iomete_sdk-1.2.1/README.md` & `iomete_sdk-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.2.1/setup.py` & `iomete_sdk-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from distutils.core import setup
 
 package_name = "iomete_sdk"
-package_version = "1.2.1"
+package_version = "1.2.2"
 
 description = """IOMETE SDK for Python."""
 
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), "r", encoding="utf8") as f:
     long_description = f.read()
```

### Comparing `iomete_sdk-1.2.1/src/iomete_sdk/api_utils.py` & `iomete_sdk-1.2.2/src/iomete_sdk/api_utils.py`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.2.1/src/iomete_sdk/security/data_security.py` & `iomete_sdk-1.2.2/src/iomete_sdk/security/data_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.logger.debug(f"Controller host: {controller_host}")
 
         self.base_url = f"https://{self._get_controller_host()}"
         self.data_security_endpoint = self.base_url + DATA_SECURITY_ENDPOINT.format(workspace_id=self.workspace_id)
 
     def _get_controller_host(self):
         result = self.api_utils.call(
-            method="GET", url=f"https://devaccount.iomete.com/api/v1/workspaces/{self.workspace_id}/info")
+            method="GET", url=f"https://account.iomete.com/api/v1/workspaces/{self.workspace_id}/info")
         return result["controller_endpoint"]
 
     def create_access_policy(self, policy: AccessPolicyView) -> AccessPolicyView:
         data = self.api_utils.call(method="POST",
                                    url=f"{self.data_security_endpoint}/access/policy",
                                    payload=policy.to_dict())
```

### Comparing `iomete_sdk-1.2.1/src/iomete_sdk/security/policy_models.py` & `iomete_sdk-1.2.2/src/iomete_sdk/security/policy_models.py`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.2.1/src/iomete_sdk/spark/spark_job.py` & `iomete_sdk-1.2.2/src/iomete_sdk/spark/spark_job.py`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.2.1/src/iomete_sdk.egg-info/PKG-INFO` & `iomete_sdk-1.2.2/src/iomete_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iomete-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: IOMETE SDK for Python.
 Home-page: https://github.com/iomete/iomete-sdk
 Author: IOMETE
 Author-email: vusal@iomete.com
 License: Apache License 2.0
 Keywords: iomete,sdk,spark-job,data-security-api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iomete_sdk-1.2.1/tests/test_data_security_api_client.py` & `iomete_sdk-1.2.2/tests/test_data_security_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from iomete_sdk.api_utils import ClientError
 from iomete_sdk.security import DataSecurityApiClient
 from iomete_sdk.security.policy_models import AccessPolicyView, DataMaskPolicyView, RowFilterPolicyView, \
     DataMaskPolicyItem, RowFilterPolicyItem, AccessPolicyResource, AccessType, AccessPolicyItem, DataMaskPolicyResource, \
     RowFilterPolicyResource, ValidityPeriod, ResourceInclusionType
 
 # Replace with your own token and workspace id
-TEST_TOKEN = "FdVawCi9GZW0P8sWuWdx0Xl0r6rLVpqEiX2LB7KLB/I="
-WORKSPACE_ID = "pw9if-p22"
+TEST_TOKEN = "YOUR_TOKEN_HERE"
+WORKSPACE_ID = "YOUR_WORKSPACE_ID_HERE"
 
 
 class TestDataSecurityApiClient(unittest.TestCase):
     def setUp(self):
         self.client = DataSecurityApiClient(
             workspace_id=WORKSPACE_ID,
             api_key=TEST_TOKEN,
```

### Comparing `iomete_sdk-1.2.1/tests/test_spark_job_api_client.py` & `iomete_sdk-1.2.2/tests/test_spark_job_api_client.py`

 * *Files identical despite different names*

