# Comparing `tmp/prometrix-0.1.7.tar.gz` & `tmp/prometrix-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.7.tar", max compression
+gzip compressed data, was "prometrix-0.1.8.tar", max compression
```

## Comparing `prometrix-0.1.7.tar` & `prometrix-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4392 2023-07-31 07:28:51.099562 prometrix-0.1.7/README.md
--rw-r--r--   0        0        0      824 2023-07-31 07:52:29.052957 prometrix-0.1.7/prometrix/__init__.py
--rw-r--r--   0        0        0     2946 2023-07-31 07:28:54.101041 prometrix-0.1.7/prometrix/auth.py
--rw-r--r--   0        0        0     4471 2023-07-31 07:28:53.983203 prometrix-0.1.7/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     6237 2023-07-31 07:28:54.111542 prometrix-0.1.7/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-07-31 07:22:16.573550 prometrix-0.1.7/prometrix/exceptions.py
--rw-r--r--   0        0        0     1693 2023-07-31 07:28:53.976836 prometrix-0.1.7/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4241 2023-07-31 07:22:16.572938 prometrix-0.1.7/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1732 2023-07-31 07:28:54.104857 prometrix-0.1.7/prometrix/utils.py
--rw-r--r--   0        0        0      399 2023-07-31 07:53:07.221285 prometrix-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 prometrix-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4788 2023-07-31 10:20:04.427506 prometrix-0.1.8/README.md
+-rw-r--r--   0        0        0      947 2023-07-31 10:20:04.425526 prometrix-0.1.8/prometrix/__init__.py
+-rw-r--r--   0        0        0     2946 2023-07-31 08:48:09.363343 prometrix-0.1.8/prometrix/auth.py
+-rw-r--r--   0        0        0     4471 2023-07-31 10:20:04.426146 prometrix-0.1.8/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     6237 2023-07-31 10:20:04.427133 prometrix-0.1.8/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-31 08:10:29.276369 prometrix-0.1.8/prometrix/exceptions.py
+-rw-r--r--   0        0        0     1693 2023-07-31 10:20:04.427238 prometrix-0.1.8/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4241 2023-07-31 08:10:29.275964 prometrix-0.1.8/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1732 2023-07-31 10:20:04.427387 prometrix-0.1.8/prometrix/utils.py
+-rw-r--r--   0        0        0      399 2023-07-31 10:20:43.397883 prometrix-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 prometrix-0.1.8/PKG-INFO
```

### Comparing `prometrix-0.1.7/README.md` & `prometrix-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Prometrix - Unified Prometheus Client
 ======================================================
 
 Overview
 --------
 
-This Python package provides a unified Prometheus client that can be used to connect to and query various types of Prometheus instances. The package supports the following additional Prometheus types:
+This Python package provides a unified Prometheus client that can be used to connect to and query various types of Prometheus instances. The package is based on the [prometheus-api-client](https://pypi.org/project/prometheus-api-client/)  package , which serves as the foundation for our extended functionality.
 
+The prometrix package enhances the prometheus-api-client by adding vendor-specific authentication methods and other features to handle authorization and signatures for all supported clients. This ensures a secure and seamless connection to the various types of Prometheus instances.
 1.  Coralogix
 2.  GKE (Google Kubernetes Engine)
 3.  Azure
 4.  EKS (Amazon Elastic Kubernetes Service)
 5.  Thanos
 6.  Victoria Metrics
 
 The main function, `get_custom_prometheus_connect`, allows you to create a custom Prometheus client based on the provided configuration. The configurations for special Prometheus versions are defined through specific classes, each extending the base `PrometheusConfig` class. Additionally, our package handles authorization and signatures for all the clients, ensuring a secure and seamless connection.
+
 Installation
 ------------
 
 You can install the package using pip:
 
 ```
 pip install generic-prometheus-client
@@ -74,17 +76,17 @@
     azure_tenant_id="YOUR_AZURE_TENANT_ID",
     azure_client_secret="YOUR_AZURE_CLIENT_SECRET",
     additional_labels={"job": "azure-prometheus"},
 )
 azure_client = get_custom_prometheus_connect(azure_config)
 ```
 
-# Similar configuration and creation can be done for EKS, Thanos, and Victoria Metrics Prometheus.`
+Similar configuration and creation can be done for EKS, Thanos, and Victoria Metrics Prometheus.
 
-Note that you need to replace the placeholder values (e.g., YOUR_CORALOGIX_PROMETHEUS_TOKEN) with your actual credentials and endpoints.
+> **_NOTE:_** You need to replace the placeholder values (e.g., YOUR_CORALOGIX_PROMETHEUS_TOKEN) with your actual credentials and endpoints.
 
 ### Supported APIs
 
 The `prometrix` package extends the prometheus-api-client class PrometheusConnect with the following additional functionality:
 
 ```
 get_prometheus_flags(self) -> Optional[Dict]
```

### Comparing `prometrix-0.1.7/prometrix/__init__.py` & `prometrix-0.1.8/prometrix/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,9 +4,12 @@
 from prometrix.exceptions import (MetricsNotFound,
                                   PrometheusFlagsConnectionError,
                                   PrometheusNotFound, ThanosMetricsNotFound,
                                   VictoriaMetricsNotFound)
 from prometrix.models.prometheus_config import (
     AWSPrometheusConfig, AzurePrometheusConfig, CoralogixPrometheusConfig,
     PrometheusConfig, VictoriaMetricsPrometheusConfig)
-from prometrix.models.prometheus_result import PrometheusQueryResult, PrometheusScalarValue, PrometheusScalarValue, PrometheusSeries, PrometheusMetric
+from prometrix.models.prometheus_result import (PrometheusMetric,
+                                                PrometheusQueryResult,
+                                                PrometheusScalarValue,
+                                                PrometheusSeries)
 from prometrix.utils import get_custom_prometheus_connect
```

### Comparing `prometrix-0.1.7/prometrix/auth.py` & `prometrix-0.1.8/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/prometrix/connect/aws_connect.py` & `prometrix-0.1.8/prometrix/connect/aws_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/prometrix/connect/custom_connect.py` & `prometrix-0.1.8/prometrix/connect/custom_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/prometrix/exceptions.py` & `prometrix-0.1.8/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/prometrix/models/prometheus_config.py` & `prometrix-0.1.8/prometrix/models/prometheus_config.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/prometrix/models/prometheus_result.py` & `prometrix-0.1.8/prometrix/models/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/prometrix/utils.py` & `prometrix-0.1.8/prometrix/utils.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.7/PKG-INFO` & `prometrix-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Avi Kotlicky
 Author-email: kotlickya@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,24 +18,26 @@
 
 Prometrix - Unified Prometheus Client
 ======================================================
 
 Overview
 --------
 
-This Python package provides a unified Prometheus client that can be used to connect to and query various types of Prometheus instances. The package supports the following additional Prometheus types:
+This Python package provides a unified Prometheus client that can be used to connect to and query various types of Prometheus instances. The package is based on the [prometheus-api-client](https://pypi.org/project/prometheus-api-client/)  package , which serves as the foundation for our extended functionality.
 
+The prometrix package enhances the prometheus-api-client by adding vendor-specific authentication methods and other features to handle authorization and signatures for all supported clients. This ensures a secure and seamless connection to the various types of Prometheus instances.
 1.  Coralogix
 2.  GKE (Google Kubernetes Engine)
 3.  Azure
 4.  EKS (Amazon Elastic Kubernetes Service)
 5.  Thanos
 6.  Victoria Metrics
 
 The main function, `get_custom_prometheus_connect`, allows you to create a custom Prometheus client based on the provided configuration. The configurations for special Prometheus versions are defined through specific classes, each extending the base `PrometheusConfig` class. Additionally, our package handles authorization and signatures for all the clients, ensuring a secure and seamless connection.
+
 Installation
 ------------
 
 You can install the package using pip:
 
 ```
 pip install generic-prometheus-client
@@ -92,17 +94,17 @@
     azure_tenant_id="YOUR_AZURE_TENANT_ID",
     azure_client_secret="YOUR_AZURE_CLIENT_SECRET",
     additional_labels={"job": "azure-prometheus"},
 )
 azure_client = get_custom_prometheus_connect(azure_config)
 ```
 
-# Similar configuration and creation can be done for EKS, Thanos, and Victoria Metrics Prometheus.`
+Similar configuration and creation can be done for EKS, Thanos, and Victoria Metrics Prometheus.
 
-Note that you need to replace the placeholder values (e.g., YOUR_CORALOGIX_PROMETHEUS_TOKEN) with your actual credentials and endpoints.
+> **_NOTE:_** You need to replace the placeholder values (e.g., YOUR_CORALOGIX_PROMETHEUS_TOKEN) with your actual credentials and endpoints.
 
 ### Supported APIs
 
 The `prometrix` package extends the prometheus-api-client class PrometheusConnect with the following additional functionality:
 
 ```
 get_prometheus_flags(self) -> Optional[Dict]
```

