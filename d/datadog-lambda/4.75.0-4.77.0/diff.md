# Comparing `tmp/datadog_lambda-4.75.0.tar.gz` & `tmp/datadog_lambda-4.77.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.75.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.77.0.tar", max compression
```

## Comparing `datadog_lambda-4.75.0.tar` & `datadog_lambda-4.77.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11379 2022-09-22 18:30:00.504292 datadog_lambda-4.75.0/LICENSE
--rw-r--r--   0        0        0      394 2022-09-22 18:30:00.504380 datadog_lambda-4.75.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3422 2023-04-18 14:29:41.172896 datadog_lambda-4.75.0/README.md
--rw-r--r--   0        0        0      538 2023-02-13 20:46:09.160997 datadog_lambda-4.75.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2022-09-22 18:30:00.504778 datadog_lambda-4.75.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     8013 2023-06-30 13:40:04.094622 datadog_lambda-4.75.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-01-25 19:31:51.675529 datadog_lambda-4.75.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2022-09-22 18:30:00.505031 datadog_lambda-4.75.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2022-09-22 18:30:00.505121 datadog_lambda-4.75.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2022-09-22 18:30:00.505207 datadog_lambda-4.75.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2022-09-22 18:30:00.505343 datadog_lambda-4.75.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2022-09-22 18:30:00.505417 datadog_lambda-4.75.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2022-09-22 18:30:00.505516 datadog_lambda-4.75.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2022-09-22 18:30:00.505686 datadog_lambda-4.75.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2022-09-22 18:30:00.505792 datadog_lambda-4.75.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2022-09-22 18:30:00.505884 datadog_lambda-4.75.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2022-09-22 18:30:00.505984 datadog_lambda-4.75.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2022-09-22 18:30:00.506089 datadog_lambda-4.75.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    47331 2023-06-30 13:40:04.095181 datadog_lambda-4.75.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-04-12 17:19:32.172228 datadog_lambda-4.75.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    14393 2023-06-30 13:40:04.095559 datadog_lambda-4.75.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-03-22 12:07:02.672991 datadog_lambda-4.75.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1271 2023-06-30 13:41:37.444527 datadog_lambda-4.75.0/pyproject.toml
--rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 datadog_lambda-4.75.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2023-07-29 00:54:04.905729 datadog_lambda-4.77.0/LICENSE
+-rw-r--r--   0        0        0      394 2023-07-29 00:54:04.905809 datadog_lambda-4.77.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3428 2023-07-29 00:54:04.905961 datadog_lambda-4.77.0/README.md
+-rw-r--r--   0        0        0      538 2023-07-29 00:54:04.906090 datadog_lambda-4.77.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2023-07-29 00:54:04.906180 datadog_lambda-4.77.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     8013 2023-07-29 00:54:04.906280 datadog_lambda-4.77.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-07-29 00:54:04.906364 datadog_lambda-4.77.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2023-07-29 00:54:04.906451 datadog_lambda-4.77.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2023-07-29 00:54:04.906536 datadog_lambda-4.77.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2023-07-29 00:54:04.906616 datadog_lambda-4.77.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2023-07-29 00:54:04.906722 datadog_lambda-4.77.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2023-07-29 00:54:04.906797 datadog_lambda-4.77.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2023-07-29 00:54:04.906895 datadog_lambda-4.77.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2023-07-29 00:54:04.906974 datadog_lambda-4.77.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2023-07-29 00:54:04.907059 datadog_lambda-4.77.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2023-07-29 00:54:04.907139 datadog_lambda-4.77.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2023-07-29 00:54:04.907240 datadog_lambda-4.77.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2023-07-29 00:54:04.907335 datadog_lambda-4.77.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    47331 2023-07-29 00:54:04.907532 datadog_lambda-4.77.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-07-29 00:54:04.907647 datadog_lambda-4.77.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    14393 2023-07-29 00:54:04.907751 datadog_lambda-4.77.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-07-29 00:54:04.907833 datadog_lambda-4.77.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1313 2023-07-31 14:07:04.189029 datadog_lambda-4.77.0/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 datadog_lambda-4.77.0/PKG-INFO
```

### Comparing `datadog_lambda-4.75.0/LICENSE` & `datadog_lambda-4.77.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/README.md` & `datadog_lambda-4.77.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)
 [![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)
 
-Datadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
+Datadog Lambda Library for Python (3.7, 3.8, 3.9, 3.10, and 3.11) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
 
 ## Installation
 
 Follow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.
 
 ## Configuration
```

### Comparing `datadog_lambda-4.75.0/datadog_lambda/__init__.py` & `datadog_lambda-4.77.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/api.py` & `datadog_lambda-4.77.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.77.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/constants.py` & `datadog_lambda-4.77.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.77.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/extension.py` & `datadog_lambda-4.77.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/handler.py` & `datadog_lambda-4.77.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/metric.py` & `datadog_lambda-4.77.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/patch.py` & `datadog_lambda-4.77.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.77.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/tags.py` & `datadog_lambda-4.77.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.77.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/tracing.py` & `datadog_lambda-4.77.0/datadog_lambda/tracing.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/trigger.py` & `datadog_lambda-4.77.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.77.0/datadog_lambda/wrapper.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/datadog_lambda/xray.py` & `datadog_lambda-4.77.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.75.0/pyproject.toml` & `datadog_lambda-4.77.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.75.0"
+version = "4.77.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
@@ -16,23 +16,24 @@
     { include = "datadog_lambda" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 datadog = ">=0.41.0,<1.0.0"
 wrapt = "^1.11.2"
-ddtrace = "^1.15.0"
+ddtrace = "1.15.2"
 urllib3 = "<2.0.0"
-importlib_metadata = {version = "^1.0", python = "<3.8"}
+importlib_metadata = {version = "*", python = "<3.8"}
 boto3 = { version = "^1.10.33", optional = true }
 typing_extensions = {version = "^4.0", python = "<3.8"}
 requests = { version ="^2.22.0", optional = true }
 nose2 = { version= "^0.9.1", optional = true }
 flake8 = { version = "^3.7.9", optional = true }
 httpretty = {version = "^0.9.7", optional = true }
```

### Comparing `datadog_lambda-4.75.0/PKG-INFO` & `datadog_lambda-4.77.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.75.0
+Version: 4.77.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Requires-Dist: boto3 (>=1.10.33,<2.0.0) ; extra == "dev"
 Requires-Dist: datadog (>=0.41.0,<1.0.0)
-Requires-Dist: ddtrace (>=1.15.0,<2.0.0)
+Requires-Dist: ddtrace (==1.15.2)
 Requires-Dist: flake8 (>=3.7.9,<4.0.0) ; extra == "dev"
 Requires-Dist: httpretty (>=0.9.7,<0.10.0) ; extra == "dev"
-Requires-Dist: importlib_metadata (>=1.0,<2.0) ; python_version < "3.8"
+Requires-Dist: importlib_metadata ; python_version < "3.8"
 Requires-Dist: nose2 (>=0.9.1,<0.10.0) ; extra == "dev"
 Requires-Dist: requests (>=2.22.0,<3.0.0) ; extra == "dev"
 Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version < "3.8"
 Requires-Dist: urllib3 (<2.0.0)
 Requires-Dist: wrapt (>=1.11.2,<2.0.0)
 Project-URL: Repository, https://github.com/DataDog/datadog-lambda-python
 Description-Content-Type: text/markdown
@@ -34,15 +34,15 @@
 
 ![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)
 [![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)
 
-Datadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
+Datadog Lambda Library for Python (3.7, 3.8, 3.9, 3.10, and 3.11) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
 
 ## Installation
 
 Follow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.
 
 ## Configuration
```

