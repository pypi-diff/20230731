# Comparing `tmp/prometrix-0.1.8.tar.gz` & `tmp/prometrix-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.8.tar", max compression
+gzip compressed data, was "prometrix-0.1.9.tar", max compression
```

## Comparing `prometrix-0.1.8.tar` & `prometrix-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4788 2023-07-31 10:20:04.427506 prometrix-0.1.8/README.md
--rw-r--r--   0        0        0      947 2023-07-31 10:20:04.425526 prometrix-0.1.8/prometrix/__init__.py
--rw-r--r--   0        0        0     2946 2023-07-31 08:48:09.363343 prometrix-0.1.8/prometrix/auth.py
--rw-r--r--   0        0        0     4471 2023-07-31 10:20:04.426146 prometrix-0.1.8/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     6237 2023-07-31 10:20:04.427133 prometrix-0.1.8/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-07-31 08:10:29.276369 prometrix-0.1.8/prometrix/exceptions.py
--rw-r--r--   0        0        0     1693 2023-07-31 10:20:04.427238 prometrix-0.1.8/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4241 2023-07-31 08:10:29.275964 prometrix-0.1.8/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1732 2023-07-31 10:20:04.427387 prometrix-0.1.8/prometrix/utils.py
--rw-r--r--   0        0        0      399 2023-07-31 10:20:43.397883 prometrix-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 prometrix-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-31 10:33:26.887864 prometrix-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     4661 2023-07-31 10:24:44.811638 prometrix-0.1.9/README.md
+-rw-r--r--   0        0        0      947 2023-07-31 10:20:04.425526 prometrix-0.1.9/prometrix/__init__.py
+-rw-r--r--   0        0        0     2946 2023-07-31 08:48:09.363343 prometrix-0.1.9/prometrix/auth.py
+-rw-r--r--   0        0        0     4829 2023-07-31 10:31:09.999529 prometrix-0.1.9/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     6237 2023-07-31 10:20:04.427133 prometrix-0.1.9/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-31 08:10:29.276369 prometrix-0.1.9/prometrix/exceptions.py
+-rw-r--r--   0        0        0     1693 2023-07-31 10:20:04.427238 prometrix-0.1.9/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4241 2023-07-31 08:10:29.275964 prometrix-0.1.9/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1732 2023-07-31 10:20:04.427387 prometrix-0.1.9/prometrix/utils.py
+-rw-r--r--   0        0        0      399 2023-07-31 10:40:03.559812 prometrix-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 prometrix-0.1.9/PKG-INFO
```

### Comparing `prometrix-0.1.8/README.md` & `prometrix-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 1.  Coralogix
 2.  GKE (Google Kubernetes Engine)
 3.  Azure
 4.  EKS (Amazon Elastic Kubernetes Service)
 5.  Thanos
 6.  Victoria Metrics
 
-The main function, `get_custom_prometheus_connect`, allows you to create a custom Prometheus client based on the provided configuration. The configurations for special Prometheus versions are defined through specific classes, each extending the base `PrometheusConfig` class. Additionally, our package handles authorization and signatures for all the clients, ensuring a secure and seamless connection.
+The main function, `get_custom_prometheus_connect`, allows you to create a custom Prometheus client based on the provided configuration. The configurations for special Prometheus versions are defined through specific classes, each extending the base `PrometheusConfig` class.
 
 Installation
 ------------
 
 You can install the package using pip:
 
 ```
```

### Comparing `prometrix-0.1.8/prometrix/__init__.py` & `prometrix-0.1.9/prometrix/__init__.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/prometrix/auth.py` & `prometrix-0.1.9/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/prometrix/connect/aws_connect.py` & `prometrix-0.1.9/prometrix/connect/aws_connect.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,7 +105,19 @@
             return response.json()["data"]
         else:
             raise PrometheusApiClientException(
                 "HTTP Status Code {} ({!r})".format(
                     response.status_code, response.content
                 )
             )
+
+    def all_metrics(self, *args, **kwargs):
+        raise NotImplementedError()
+
+    def get_current_metric_value(self, *args, **kwargs):
+        raise NotImplementedError()
+
+    def get_metric_range_data(self, *args, **kwargs):
+        raise NotImplementedError()
+
+    def get_metric_aggregation(self, *args, **kwargs):
+        raise NotImplementedError()
```

### Comparing `prometrix-0.1.8/prometrix/connect/custom_connect.py` & `prometrix-0.1.9/prometrix/connect/custom_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/prometrix/exceptions.py` & `prometrix-0.1.9/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/prometrix/models/prometheus_config.py` & `prometrix-0.1.9/prometrix/models/prometheus_config.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/prometrix/models/prometheus_result.py` & `prometrix-0.1.9/prometrix/models/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/prometrix/utils.py` & `prometrix-0.1.9/prometrix/utils.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.8/PKG-INFO` & `prometrix-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Avi Kotlicky
 Author-email: kotlickya@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +28,15 @@
 1.  Coralogix
 2.  GKE (Google Kubernetes Engine)
 3.  Azure
 4.  EKS (Amazon Elastic Kubernetes Service)
 5.  Thanos
 6.  Victoria Metrics
 
-The main function, `get_custom_prometheus_connect`, allows you to create a custom Prometheus client based on the provided configuration. The configurations for special Prometheus versions are defined through specific classes, each extending the base `PrometheusConfig` class. Additionally, our package handles authorization and signatures for all the clients, ensuring a secure and seamless connection.
+The main function, `get_custom_prometheus_connect`, allows you to create a custom Prometheus client based on the provided configuration. The configurations for special Prometheus versions are defined through specific classes, each extending the base `PrometheusConfig` class.
 
 Installation
 ------------
 
 You can install the package using pip:
 
 ```
```

