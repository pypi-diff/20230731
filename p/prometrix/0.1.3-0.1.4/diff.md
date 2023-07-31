# Comparing `tmp/prometrix-0.1.3.tar.gz` & `tmp/prometrix-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometrix-0.1.3.tar", max compression
+gzip compressed data, was "prometrix-0.1.4.tar", max compression
```

## Comparing `prometrix-0.1.3.tar` & `prometrix-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-07-30 10:21:35.279123 prometrix-0.1.3/README.md
--rw-r--r--   0        0        0      887 2023-07-31 06:48:02.676636 prometrix-0.1.3/prometrix/__init__.py
--rw-r--r--   0        0        0     2946 2023-07-31 06:48:02.671620 prometrix-0.1.3/prometrix/auth.py
--rw-r--r--   0        0        0     4477 2023-07-31 06:48:02.673686 prometrix-0.1.3/prometrix/connect/aws_connect.py
--rw-r--r--   0        0        0     6187 2023-07-31 06:48:02.667549 prometrix-0.1.3/prometrix/connect/custom_connect.py
--rw-r--r--   0        0        0      660 2023-07-30 14:04:35.247967 prometrix-0.1.3/prometrix/exceptions.py
--rw-r--r--   0        0        0     1692 2023-07-30 14:06:47.984025 prometrix-0.1.3/prometrix/models/prometheus_config.py
--rw-r--r--   0        0        0     4241 2023-07-30 14:08:10.168954 prometrix-0.1.3/prometrix/models/prometheus_result.py
--rw-r--r--   0        0        0     1738 2023-07-31 06:48:02.675172 prometrix-0.1.3/prometrix/utils.py
--rw-r--r--   0        0        0      399 2023-07-31 06:47:36.762098 prometrix-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 prometrix-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 10:21:35.279123 prometrix-0.1.4/README.md
+-rw-r--r--   0        0        0      887 2023-07-31 06:48:02.676636 prometrix-0.1.4/prometrix/__init__.py
+-rw-r--r--   0        0        0     2946 2023-07-31 06:48:02.671620 prometrix-0.1.4/prometrix/auth.py
+-rw-r--r--   0        0        0     4477 2023-07-31 06:48:02.673686 prometrix-0.1.4/prometrix/connect/aws_connect.py
+-rw-r--r--   0        0        0     6211 2023-07-31 06:51:55.090912 prometrix-0.1.4/prometrix/connect/custom_connect.py
+-rw-r--r--   0        0        0      660 2023-07-30 14:04:35.247967 prometrix-0.1.4/prometrix/exceptions.py
+-rw-r--r--   0        0        0     1692 2023-07-30 14:06:47.984025 prometrix-0.1.4/prometrix/models/prometheus_config.py
+-rw-r--r--   0        0        0     4241 2023-07-30 14:08:10.168954 prometrix-0.1.4/prometrix/models/prometheus_result.py
+-rw-r--r--   0        0        0     1738 2023-07-31 06:48:02.675172 prometrix-0.1.4/prometrix/utils.py
+-rw-r--r--   0        0        0      399 2023-07-31 06:52:17.985722 prometrix-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 prometrix-0.1.4/PKG-INFO
```

### Comparing `prometrix-0.1.3/prometrix/__init__.py` & `prometrix-0.1.4/prometrix/__init__.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/prometrix/auth.py` & `prometrix-0.1.4/prometrix/auth.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/prometrix/connect/aws_connect.py` & `prometrix-0.1.4/prometrix/connect/aws_connect.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/prometrix/connect/custom_connect.py` & `prometrix-0.1.4/prometrix/connect/custom_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any, Dict, Optional
-
+from typing import Dict, Optional
+from datetime import datetime
 import requests
 from prometheus_api_client import (PrometheusApiClientException,
                                    PrometheusConnect)
 from requests.adapters import HTTPAdapter
 from requests.exceptions import ConnectionError, HTTPError
 
 from prometrix.auth import PrometheusAuthorization
```

### Comparing `prometrix-0.1.3/prometrix/exceptions.py` & `prometrix-0.1.4/prometrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/prometrix/models/prometheus_config.py` & `prometrix-0.1.4/prometrix/models/prometheus_config.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/prometrix/models/prometheus_result.py` & `prometrix-0.1.4/prometrix/models/prometheus_result.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/prometrix/utils.py` & `prometrix-0.1.4/prometrix/utils.py`

 * *Files identical despite different names*

### Comparing `prometrix-0.1.3/PKG-INFO` & `prometrix-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometrix
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Avi Kotlicky
 Author-email: kotlickya@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

