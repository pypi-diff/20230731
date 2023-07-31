# Comparing `tmp/stigg_api_client-0.514.0.tar.gz` & `tmp/stigg_api_client-0.515.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.514.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.515.3.tar", max compression
```

## Comparing `stigg_api_client-0.514.0.tar` & `stigg_api_client-0.515.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-31 04:59:45.179336 stigg_api_client-0.514.0/README.md
--rw-r--r--   0        0        0      480 2023-07-31 05:00:23.679189 stigg_api_client-0.514.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-31 04:59:45.179336 stigg_api_client-0.514.0/stigg/__init__.py
--rw-r--r--   0        0        0     3699 2023-07-31 04:59:45.179336 stigg_api_client-0.514.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-31 05:00:21.799199 stigg_api_client-0.514.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-07-31 05:00:22.227197 stigg_api_client-0.514.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   467233 2023-07-31 05:00:22.063197 stigg_api_client-0.514.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.514.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-31 10:12:28.144694 stigg_api_client-0.515.3/README.md
+-rw-r--r--   0        0        0      480 2023-07-31 10:13:03.168762 stigg_api_client-0.515.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-31 10:12:28.144694 stigg_api_client-0.515.3/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-07-31 10:12:28.144694 stigg_api_client-0.515.3/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:13:01.252756 stigg_api_client-0.515.3/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-07-31 10:13:01.680757 stigg_api_client-0.515.3/stigg/generated/operations.py
+-rw-r--r--   0        0        0   467319 2023-07-31 10:13:01.512757 stigg_api_client-0.515.3/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.515.3/PKG-INFO
```

### Comparing `stigg_api_client-0.514.0/README.md` & `stigg_api_client-0.515.3/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.514.0/stigg/client.py` & `stigg_api_client-0.515.3/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.514.0/stigg/generated/operations.py` & `stigg_api_client-0.515.3/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.514.0/stigg/generated/schema.py` & `stigg_api_client-0.515.3/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -3234,15 +3234,15 @@
     timestamp = sgqlc.types.Field(DateTime, graphql_name='timestamp')
 
 
 class UsageEventsInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('environment_id', 'filters')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
-    filters = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MeterFilterDefinitionInput))), graphql_name='filters')
+    filters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(MeterFilterDefinitionInput)), graphql_name='filters')
 
 
 class UsageEventsReportInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('environment_id', 'usage_events')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     usage_events = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(UsageEventReportInput))), graphql_name='usageEvents')
@@ -7309,15 +7309,16 @@
     __field_names__ = ('id', 'order')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     order = sgqlc.types.Field(Float, graphql_name='order')
 
 
 class UsageEvent(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('dimensions', 'event_name', 'id', 'timestamp')
+    __field_names__ = ('customer_id', 'dimensions', 'event_name', 'id', 'timestamp')
+    customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     dimensions = sgqlc.types.Field(JSON, graphql_name='dimensions')
     event_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='eventName')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     timestamp = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='timestamp')
 
 
 class UsageEventsPreview(sgqlc.types.Type):
```

### Comparing `stigg_api_client-0.514.0/PKG-INFO` & `stigg_api_client-0.515.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.514.0
+Version: 0.515.3
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

