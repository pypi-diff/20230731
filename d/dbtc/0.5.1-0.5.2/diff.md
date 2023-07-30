# Comparing `tmp/dbtc-0.5.1.tar.gz` & `tmp/dbtc-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtc-0.5.1.tar", max compression
+gzip compressed data, was "dbtc-0.5.2.tar", max compression
```

## Comparing `dbtc-0.5.1.tar` & `dbtc-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3827 2023-07-30 13:05:07.582308 dbtc-0.5.1/README.md
--rw-r--r--   0        0        0      124 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/__init__.py
--rw-r--r--   0        0        0       22 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/_version.py
--rw-r--r--   0        0        0    39135 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/cli.py
--rw-r--r--   0        0        0        0 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/__init__.py
--rw-r--r--   0        0        0    67683 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/admin.py
--rw-r--r--   0        0        0   352525 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/artifacts/metadata_schema.json
--rw-r--r--   0        0        0     2349 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/base.py
--rw-r--r--   0        0        0      258 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/main.py
--rw-r--r--   0        0        0    24548 2023-07-30 13:05:07.582308 dbtc-0.5.1/dbtc/client/metadata.py
--rw-r--r--   0        0        0    62305 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/client/schema.py
--rw-r--r--   0        0        0      103 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/console.py
--rw-r--r--   0        0        0       44 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/models/__init__.py
--rw-r--r--   0        0        0      524 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/models/webhooks.py
--rw-r--r--   0        0        0      428 2023-07-30 13:05:07.586309 dbtc-0.5.1/dbtc/utils.py
--rw-r--r--   0        0        0      905 2023-07-30 13:05:25.415146 dbtc-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 dbtc-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3827 2023-07-30 22:04:59.015237 dbtc-0.5.2/README.md
+-rw-r--r--   0        0        0      124 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/_version.py
+-rw-r--r--   0        0        0    39135 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/cli.py
+-rw-r--r--   0        0        0        0 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/__init__.py
+-rw-r--r--   0        0        0    67682 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/admin.py
+-rw-r--r--   0        0        0   352525 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/artifacts/metadata_schema.json
+-rw-r--r--   0        0        0     2349 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/base.py
+-rw-r--r--   0        0        0      258 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/main.py
+-rw-r--r--   0        0        0    24548 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/metadata.py
+-rw-r--r--   0        0        0    62305 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/client/schema.py
+-rw-r--r--   0        0        0      103 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/console.py
+-rw-r--r--   0        0        0       44 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/models/webhooks.py
+-rw-r--r--   0        0        0      428 2023-07-30 22:04:59.015237 dbtc-0.5.2/dbtc/utils.py
+-rw-r--r--   0        0        0      905 2023-07-30 22:05:14.131212 dbtc-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 dbtc-0.5.2/PKG-INFO
```

### Comparing `dbtc-0.5.1/README.md` & `dbtc-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/dbtc/cli.py` & `dbtc-0.5.2/dbtc/cli.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/dbtc/client/admin.py` & `dbtc-0.5.2/dbtc/client/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1776,15 +1776,15 @@
         Args:
             account_id (int): Numeric ID of the account
             project_id (int): Numeric ID of the project
             payload (dict): Dictionary representing the environment to update
         """
         return self._simple_request(
             f'accounts/{account_id}/projects/{project_id}/environment-variables/bulk',  # noqa: E501
-            method='post',
+            method='put',
             json=payload,
         )
 
     @v2
     def update_job(self, account_id: int, job_id: int, payload: Dict) -> Dict:
         """Update a job by its ID.
```

### Comparing `dbtc-0.5.1/dbtc/client/artifacts/metadata_schema.json` & `dbtc-0.5.2/dbtc/client/artifacts/metadata_schema.json`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/dbtc/client/base.py` & `dbtc-0.5.2/dbtc/client/base.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/dbtc/client/metadata.py` & `dbtc-0.5.2/dbtc/client/metadata.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/dbtc/client/schema.py` & `dbtc-0.5.2/dbtc/client/schema.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/dbtc/models/webhooks.py` & `dbtc-0.5.2/dbtc/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.5.1/pyproject.toml` & `dbtc-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbtc"
-version = "0.5.1"
+version = "0.5.2"
 description = "An unaffiliated python wrapper for dbt Cloud APIs"
 authors = ["Doug Guthrie <douglas.p.guthrie@gmail.com>"]
 documentation = "https://dbtc.dpguthrie.com"
 keywords=["dbt", "requests", "API", "dbt Cloud"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `dbtc-0.5.1/PKG-INFO` & `dbtc-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtc
-Version: 0.5.1
+Version: 0.5.2
 Summary: An unaffiliated python wrapper for dbt Cloud APIs
 License: MIT
 Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie
 Author-email: douglas.p.guthrie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbtc Version: 0.5.1 Summary: An unaffiliated python
+Metadata-Version: 2.1 Name: dbtc Version: 0.5.2 Summary: An unaffiliated python
 wrapper for dbt Cloud APIs License: MIT Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie Author-email: douglas.p.guthrie@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist:
```

