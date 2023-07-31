# Comparing `tmp/prometrix-0.1.5.tar.gz` & `tmp/prometrix-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.5.tar", max compression
+gzip compressed data, was "prometrix-0.1.6.tar", max compression
```

## Comparing `prometrix-0.1.5.tar` & `prometrix-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4605 2023-07-31 07:22:17.653547 prometrix-0.1.5/README.md
--rw-r--r--   0        0        0      887 2023-07-31 07:22:16.572848 prometrix-0.1.5/prometrix/__init__.py
--rw-r--r--   0        0        0     2946 2023-07-31 07:22:16.573672 prometrix-0.1.5/prometrix/auth.py
--rw-r--r--   0        0        0     4477 2023-07-31 07:22:16.573394 prometrix-0.1.5/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     6211 2023-07-31 07:22:16.573498 prometrix-0.1.5/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-07-31 07:22:16.573550 prometrix-0.1.5/prometrix/exceptions.py
--rw-r--r--   0        0        0     1692 2023-07-31 07:22:16.573623 prometrix-0.1.5/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4241 2023-07-31 07:22:16.572938 prometrix-0.1.5/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1738 2023-07-31 07:22:16.573724 prometrix-0.1.5/prometrix/utils.py
--rw-r--r--   0        0        0      399 2023-07-31 07:22:33.069947 prometrix-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 prometrix-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4392 2023-07-31 07:28:51.099562 prometrix-0.1.6/README.md
+-rw-r--r--   0        0        0      742 2023-07-31 07:28:54.103654 prometrix-0.1.6/prometrix/__init__.py
+-rw-r--r--   0        0        0     2946 2023-07-31 07:28:54.101041 prometrix-0.1.6/prometrix/auth.py
+-rw-r--r--   0        0        0     4471 2023-07-31 07:28:53.983203 prometrix-0.1.6/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     6237 2023-07-31 07:28:54.111542 prometrix-0.1.6/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-31 07:22:16.573550 prometrix-0.1.6/prometrix/exceptions.py
+-rw-r--r--   0        0        0     1693 2023-07-31 07:28:53.976836 prometrix-0.1.6/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4241 2023-07-31 07:22:16.572938 prometrix-0.1.6/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1732 2023-07-31 07:28:54.104857 prometrix-0.1.6/prometrix/utils.py
+-rw-r--r--   0        0        0      399 2023-07-31 07:29:44.079540 prometrix-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 prometrix-0.1.6/PKG-INFO
```

### Comparing `prometrix-0.1.5/README.md` & `prometrix-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -107,11 +107,7 @@
 
 This project is licensed under the MIT License - see the LICENSE.md file for details.
 
 Acknowledgments
 ---------------
 
 This package was inspired by the need to have a flexible and generic Prometheus client that can be easily extended to connect with different Prometheus types. Special thanks to the Prometheus team and the open-source community for their contributions.
-
-* * * * *
-
-Feel free to modify and add more details to this README as per your specific project's needs. Remember to include information about the package installation, setup, and any other relevant instructions.
```

### Comparing `prometrix-0.1.5/prometrix/__init__.py` & `prometrix-0.1.6/prometrix/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from prometrix.auth import PrometheusAuthorization
 from prometrix.connect.aws_connect import AWSPrometheusConnect
-from prometrix.connect.custom_connect import \
-    CustomPrometheusConnect
-from prometrix.exceptions import (
-    MetricsNotFound, PrometheusFlagsConnectionError, PrometheusNotFound,
-    ThanosMetricsNotFound, VictoriaMetricsNotFound)
-from prometrix.models.prometheus_config import (AWSPrometheusConfig,
-                                                AzurePrometheusConfig,
-                                                CoralogixPrometheusConfig,
-                                                PrometheusConfig,
-                                                VictoriaMetricsPrometheusConfig)
-from prometrix.models.prometheus_result import (
-                                              PrometheusQueryResult)
+from prometrix.connect.custom_connect import CustomPrometheusConnect
+from prometrix.exceptions import (MetricsNotFound,
+                                  PrometheusFlagsConnectionError,
+                                  PrometheusNotFound, ThanosMetricsNotFound,
+                                  VictoriaMetricsNotFound)
+from prometrix.models.prometheus_config import (
+    AWSPrometheusConfig, AzurePrometheusConfig, CoralogixPrometheusConfig,
+    PrometheusConfig, VictoriaMetricsPrometheusConfig)
+from prometrix.models.prometheus_result import PrometheusQueryResult
 from prometrix.utils import get_custom_prometheus_connect
```

### Comparing `prometrix-0.1.5/prometrix/auth.py` & `prometrix-0.1.6/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.5/prometrix/connect/aws_connect.py` & `prometrix-0.1.6/prometrix/connect/aws_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import requests
 from botocore.auth import *
 from botocore.awsrequest import AWSRequest
 from botocore.credentials import Credentials
 from prometheus_api_client import PrometheusApiClientException
 
-from prometrix.connect.custom_connect import \
-    CustomPrometheusConnect
+from prometrix.connect.custom_connect import CustomPrometheusConnect
 
 
 class AWSPrometheusConnect(CustomPrometheusConnect):
     def __init__(
         self, access_key: str, secret_key: str, region: str, service_name: str, **kwargs
     ):
         super().__init__(**kwargs)
```

### Comparing `prometrix-0.1.5/prometrix/connect/custom_connect.py` & `prometrix-0.1.6/prometrix/connect/custom_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Dict, Optional
 from datetime import datetime
+from typing import Dict, Optional
+
 import requests
 from prometheus_api_client import (PrometheusApiClientException,
                                    PrometheusConnect)
 from requests.adapters import HTTPAdapter
 from requests.exceptions import ConnectionError, HTTPError
 
 from prometrix.auth import PrometheusAuthorization
-from prometrix.exceptions import (
-    PrometheusFlagsConnectionError, PrometheusNotFound,
-    VictoriaMetricsNotFound)
+from prometrix.exceptions import (PrometheusFlagsConnectionError,
+                                  PrometheusNotFound, VictoriaMetricsNotFound)
 from prometrix.models.prometheus_config import PrometheusApis, PrometheusConfig
 
 
 class CustomPrometheusConnect(PrometheusConnect):
     def __init__(self, config: PrometheusConfig):
         super().__init__(
             url=config.url, disable_ssl=config.disable_ssl, headers=config.headers
```

### Comparing `prometrix-0.1.5/prometrix/exceptions.py` & `prometrix-0.1.6/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.5/prometrix/models/prometheus_config.py` & `prometrix-0.1.6/prometrix/models/prometheus_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import Dict, List, Optional
 
 from pydantic import BaseModel, SecretStr
 
+
 class PrometheusApis(Enum):
     QUERY = 0
     QUERY_RANGE = 1
     LABELS = 2
     FLAGS = 3
     VM_FLAGS = 4
```

### Comparing `prometrix-0.1.5/prometrix/models/prometheus_result.py` & `prometrix-0.1.6/prometrix/models/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.5/prometrix/utils.py` & `prometrix-0.1.6/prometrix/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from typing import Dict, List
 from urllib.parse import parse_qs
 
 from requests.sessions import merge_setting
 
 from prometrix.auth import PrometheusAuthorization
 from prometrix.connect.aws_connect import AWSPrometheusConnect
-from prometrix.connect.custom_connect import \
-    CustomPrometheusConnect
+from prometrix.connect.custom_connect import CustomPrometheusConnect
 from prometrix.models.prometheus_config import (AWSPrometheusConfig,
                                                 PrometheusConfig)
 
 
 def _parse_query_string(query_string: str) -> Dict[str, List[str]]:
     if not query_string:
         return {}
```

### Comparing `prometrix-0.1.5/PKG-INFO` & `prometrix-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Avi Kotlicky
 Author-email: kotlickya@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -126,10 +126,7 @@
 This project is licensed under the MIT License - see the LICENSE.md file for details.
 
 Acknowledgments
 ---------------
 
 This package was inspired by the need to have a flexible and generic Prometheus client that can be easily extended to connect with different Prometheus types. Special thanks to the Prometheus team and the open-source community for their contributions.
 
-* * * * *
-
-Feel free to modify and add more details to this README as per your specific project's needs. Remember to include information about the package installation, setup, and any other relevant instructions.
```

