# Comparing `tmp/stigg_api_client-0.512.0.tar.gz` & `tmp/stigg_api_client-0.514.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.512.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.514.0.tar", max compression
```

## Comparing `stigg_api_client-0.512.0.tar` & `stigg_api_client-0.514.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-30 10:08:16.305889 stigg_api_client-0.512.0/README.md
--rw-r--r--   0        0        0      480 2023-07-30 10:09:02.802063 stigg_api_client-0.512.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-30 10:08:16.305889 stigg_api_client-0.512.0/stigg/__init__.py
--rw-r--r--   0        0        0     3699 2023-07-30 10:08:16.305889 stigg_api_client-0.512.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-30 10:09:00.326046 stigg_api_client-0.512.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-07-30 10:09:00.866050 stigg_api_client-0.512.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   467141 2023-07-30 10:09:00.666049 stigg_api_client-0.512.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.512.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-31 04:59:45.179336 stigg_api_client-0.514.0/README.md
+-rw-r--r--   0        0        0      480 2023-07-31 05:00:23.679189 stigg_api_client-0.514.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-31 04:59:45.179336 stigg_api_client-0.514.0/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-07-31 04:59:45.179336 stigg_api_client-0.514.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-31 05:00:21.799199 stigg_api_client-0.514.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-07-31 05:00:22.227197 stigg_api_client-0.514.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   467233 2023-07-31 05:00:22.063197 stigg_api_client-0.514.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.514.0/PKG-INFO
```

### Comparing `stigg_api_client-0.512.0/README.md` & `stigg_api_client-0.514.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.512.0/stigg/client.py` & `stigg_api_client-0.514.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.512.0/stigg/generated/operations.py` & `stigg_api_client-0.514.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.512.0/stigg/generated/schema.py` & `stigg_api_client-0.514.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -2944,16 +2944,17 @@
     not_ilike = sgqlc.types.Field(SubscriptionStatus, graphql_name='notILike')
     not_in = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionStatus)), graphql_name='notIn')
     not_like = sgqlc.types.Field(SubscriptionStatus, graphql_name='notLike')
 
 
 class SubscriptionUpdateScheduleCancellationInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('environment_id', 'subscription_id')
+    __field_names__ = ('environment_id', 'status', 'subscription_id')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    status = sgqlc.types.Field(SubscriptionScheduleStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='subscriptionId')
 
 
 class SyncTaxRatesInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('environment_id',)
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
```

### Comparing `stigg_api_client-0.512.0/PKG-INFO` & `stigg_api_client-0.514.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.512.0
+Version: 0.514.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

