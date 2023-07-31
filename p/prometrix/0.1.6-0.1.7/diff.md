# Comparing `tmp/prometrix-0.1.6.tar.gz` & `tmp/prometrix-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.6.tar", max compression
+gzip compressed data, was "prometrix-0.1.7.tar", max compression
```

## Comparing `prometrix-0.1.6.tar` & `prometrix-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4392 2023-07-31 07:28:51.099562 prometrix-0.1.6/README.md
--rw-r--r--   0        0        0      742 2023-07-31 07:28:54.103654 prometrix-0.1.6/prometrix/__init__.py
--rw-r--r--   0        0        0     2946 2023-07-31 07:28:54.101041 prometrix-0.1.6/prometrix/auth.py
--rw-r--r--   0        0        0     4471 2023-07-31 07:28:53.983203 prometrix-0.1.6/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     6237 2023-07-31 07:28:54.111542 prometrix-0.1.6/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-07-31 07:22:16.573550 prometrix-0.1.6/prometrix/exceptions.py
--rw-r--r--   0        0        0     1693 2023-07-31 07:28:53.976836 prometrix-0.1.6/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4241 2023-07-31 07:22:16.572938 prometrix-0.1.6/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1732 2023-07-31 07:28:54.104857 prometrix-0.1.6/prometrix/utils.py
--rw-r--r--   0        0        0      399 2023-07-31 07:29:44.079540 prometrix-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 prometrix-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4392 2023-07-31 07:28:51.099562 prometrix-0.1.7/README.md
+-rw-r--r--   0        0        0      824 2023-07-31 07:52:29.052957 prometrix-0.1.7/prometrix/__init__.py
+-rw-r--r--   0        0        0     2946 2023-07-31 07:28:54.101041 prometrix-0.1.7/prometrix/auth.py
+-rw-r--r--   0        0        0     4471 2023-07-31 07:28:53.983203 prometrix-0.1.7/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     6237 2023-07-31 07:28:54.111542 prometrix-0.1.7/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-31 07:22:16.573550 prometrix-0.1.7/prometrix/exceptions.py
+-rw-r--r--   0        0        0     1693 2023-07-31 07:28:53.976836 prometrix-0.1.7/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4241 2023-07-31 07:22:16.572938 prometrix-0.1.7/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1732 2023-07-31 07:28:54.104857 prometrix-0.1.7/prometrix/utils.py
+-rw-r--r--   0        0        0      399 2023-07-31 07:53:07.221285 prometrix-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 prometrix-0.1.7/PKG-INFO
```

### Comparing `prometrix-0.1.6/README.md` & `prometrix-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/__init__.py` & `prometrix-0.1.7/prometrix/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,9 +4,9 @@
 from prometrix.exceptions import (MetricsNotFound,
                                   PrometheusFlagsConnectionError,
                                   PrometheusNotFound, ThanosMetricsNotFound,
                                   VictoriaMetricsNotFound)
 from prometrix.models.prometheus_config import (
     AWSPrometheusConfig, AzurePrometheusConfig, CoralogixPrometheusConfig,
     PrometheusConfig, VictoriaMetricsPrometheusConfig)
-from prometrix.models.prometheus_result import PrometheusQueryResult
+from prometrix.models.prometheus_result import PrometheusQueryResult, PrometheusScalarValue, PrometheusScalarValue, PrometheusSeries, PrometheusMetric
 from prometrix.utils import get_custom_prometheus_connect
```

### Comparing `prometrix-0.1.6/prometrix/auth.py` & `prometrix-0.1.7/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/connect/aws_connect.py` & `prometrix-0.1.7/prometrix/connect/aws_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/connect/custom_connect.py` & `prometrix-0.1.7/prometrix/connect/custom_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/exceptions.py` & `prometrix-0.1.7/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/models/prometheus_config.py` & `prometrix-0.1.7/prometrix/models/prometheus_config.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/models/prometheus_result.py` & `prometrix-0.1.7/prometrix/models/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/prometrix/utils.py` & `prometrix-0.1.7/prometrix/utils.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.6/PKG-INFO` & `prometrix-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Avi Kotlicky
 Author-email: kotlickya@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

