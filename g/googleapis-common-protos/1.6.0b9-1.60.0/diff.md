# Comparing `tmp/googleapis-common-protos-1.6.0b9.tar.gz` & `tmp/googleapis-common-protos-1.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/googleapis-common-protos-1.6.0b9.tar", last modified: Tue Feb 26 16:43:15 2019, max compression
+gzip compressed data, was "googleapis-common-protos-1.60.0.tar", last modified: Mon Jul 31 14:13:33 2023, max compression
```

## Comparing `googleapis-common-protos-1.6.0b9.tar` & `googleapis-common-protos-1.60.0.tar`

### file list

```diff
@@ -1,81 +1,164 @@
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11352 2018-07-03 22:23:59.000000 googleapis-common-protos-1.6.0b9/LICENSE
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       27 2018-07-03 22:23:59.000000 googleapis-common-protos-1.6.0b9/MANIFEST.in
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1190 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/PKG-INFO
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)      275 2018-07-03 22:31:05.000000 googleapis-common-protos-1.6.0b9/README.rst
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       56 2018-07-03 22:27:00.000000 googleapis-common-protos-1.6.0b9/google/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/api/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:23.000000 googleapis-common-protos-1.6.0b9/google/api/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2080 2019-02-08 21:38:33.000000 googleapis-common-protos-1.6.0b9/google/api/annotations_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11462 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/auth_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4745 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/backend_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4341 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/billing_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6227 2019-02-13 04:02:06.000000 googleapis-common-protos-1.6.0b9/google/api/client_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6531 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/config_change_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5651 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/consumer_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4257 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/context_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2230 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/control_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    16037 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/distribution_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     8350 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/documentation_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4030 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/endpoint_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3618 2019-02-08 21:36:46.000000 googleapis-common-protos-1.6.0b9/google/api/field_behavior_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    10228 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/http_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3313 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/httpbody_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4162 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/label_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3816 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/log_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4896 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/logging_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4753 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/metadata_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11759 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/metric_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    12433 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/monitored_resource_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5059 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/monitoring_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    13136 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/quota_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     7879 2019-02-08 21:36:46.000000 googleapis-common-protos-1.6.0b9/google/api/resource_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    17859 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/service_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2553 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/source_info_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6374 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/system_parameter_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5334 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/usage_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/iam/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:30.000000 googleapis-common-protos-1.6.0b9/google/iam/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/iam/admin/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:37.000000 googleapis-common-protos-1.6.0b9/google/iam/admin/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:41.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9717 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/iam_policy_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9233 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/policy_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/logging/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       56 2018-07-03 22:27:29.000000 googleapis-common-protos-1.6.0b9/google/logging/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/logging/type/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:52:16.000000 googleapis-common-protos-1.6.0b9/google/logging/type/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9056 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/logging/type/http_request_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3541 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/logging/type/log_severity_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/longrunning/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:52.000000 googleapis-common-protos-1.6.0b9/google/longrunning/__init__.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)      220 2019-02-22 17:26:13.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_grpc.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1978 2019-02-22 18:17:43.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_grpc_pb2.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1115 2019-02-22 18:18:17.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_pb2.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)      221 2019-02-22 17:26:09.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_proto.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    19093 2019-02-08 22:15:36.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_proto_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/rpc/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:57.000000 googleapis-common-protos-1.6.0b9/google/rpc/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4612 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/rpc/code_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    22299 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/rpc/error_details_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3234 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/rpc/status_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/type/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:52:02.000000 googleapis-common-protos-1.6.0b9/google/type/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3632 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/color_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2904 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/date_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2977 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/dayofweek_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2574 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/latlng_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2941 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/money_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6647 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/postal_address_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3403 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/timeofday_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)     1190 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/PKG-INFO
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)     1983 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/SOURCES.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)        1 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/dependency_links.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)       22 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/namespace_packages.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)       38 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/requires.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)        7 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/top_level.txt
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       38 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/setup.cfg
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     1191 2019-02-26 16:42:30.000000 googleapis-common-protos-1.6.0b9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.666584 googleapis-common-protos-1.60.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     1312 2023-07-31 14:13:33.666584 googleapis-common-protos-1.60.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003      362 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.642581 googleapis-common-protos-1.60.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.654583 googleapis-common-protos-1.60.0/google/api/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1045 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/annotations.proto
+-rw-rw-r--   0 root         (0)     1003     2133 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/annotations_pb2.py
+-rw-rw-r--   0 root         (0)     1003     9257 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/auth.proto
+-rw-rw-r--   0 root         (0)     1003     5613 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/auth_pb2.py
+-rw-rw-r--   0 root         (0)     1003     7014 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/backend.proto
+-rw-rw-r--   0 root         (0)     1003     4838 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/backend_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3062 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/billing.proto
+-rw-rw-r--   0 root         (0)     1003     2933 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/billing_pb2.py
+-rw-rw-r--   0 root         (0)     1003    13316 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/client.proto
+-rw-rw-r--   0 root         (0)     1003    16867 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/client_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3166 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/config_change.proto
+-rw-rw-r--   0 root         (0)     1003     3374 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/config_change_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2717 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/consumer.proto
+-rw-rw-r--   0 root         (0)     1003     3138 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/consumer_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3067 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/context.proto
+-rw-rw-r--   0 root         (0)     1003     2844 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/context_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1436 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/control.proto
+-rw-rw-r--   0 root         (0)     1003     2300 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/control_pb2.py
+-rw-rw-r--   0 root         (0)     1003     8660 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/distribution.proto
+-rw-rw-r--   0 root         (0)     1003     7845 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/distribution_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6940 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/documentation.proto
+-rw-rw-r--   0 root         (0)     1003     3698 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/documentation_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3028 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/endpoint.proto
+-rw-rw-r--   0 root         (0)     1003     2380 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/endpoint_pb2.py
+-rw-rw-r--   0 root         (0)     1003    21934 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/error_reason.proto
+-rw-rw-r--   0 root         (0)     1003     4191 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/error_reason_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3604 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/field_behavior.proto
+-rw-rw-r--   0 root         (0)     1003     2824 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/field_behavior_pb2.py
+-rw-rw-r--   0 root         (0)     1003    15159 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/http.proto
+-rw-rw-r--   0 root         (0)     1003     3701 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/http_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2693 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/httpbody.proto
+-rw-rw-r--   0 root         (0)     1003     2344 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/httpbody_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1389 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/label.proto
+-rw-rw-r--   0 root         (0)     1003     2581 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/label_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3083 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/launch_stage.proto
+-rw-rw-r--   0 root         (0)     1003     2277 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/launch_stage_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2043 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/log.proto
+-rw-rw-r--   0 root         (0)     1003     2402 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/log_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3174 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/logging.proto
+-rw-rw-r--   0 root         (0)     1003     3014 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/logging_pb2.py
+-rw-rw-r--   0 root         (0)     1003    10605 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/metric.proto
+-rw-rw-r--   0 root         (0)     1003     6432 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/metric_pb2.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/monitored_resource.proto
+-rw-rw-r--   0 root         (0)     1003     6324 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/monitored_resource_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4457 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/monitoring.proto
+-rw-rw-r--   0 root         (0)     1003     3129 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/monitoring_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3254 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/policy.proto
+-rw-rw-r--   0 root         (0)     1003     3608 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/policy_pb2.py
+-rw-rw-r--   0 root         (0)     1003     7138 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/quota.proto
+-rw-rw-r--   0 root         (0)     1003     5303 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/quota_pb2.py
+-rw-rw-r--   0 root         (0)     1003     8744 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/resource.proto
+-rw-rw-r--   0 root         (0)     1003     4870 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/resource_pb2.py
+-rw-rw-r--   0 root         (0)     1003    14929 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/routing.proto
+-rw-rw-r--   0 root         (0)     1003     3189 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/routing_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6762 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/service.proto
+-rw-rw-r--   0 root         (0)     1003     5979 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/service_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1091 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/source_info.proto
+-rw-rw-r--   0 root         (0)     1003     2292 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/source_info_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3475 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/system_parameter.proto
+-rw-rw-r--   0 root         (0)     1003     3583 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/system_parameter_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3787 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/usage.proto
+-rw-rw-r--   0 root         (0)     1003     2791 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/usage_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3799 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/visibility.proto
+-rw-rw-r--   0 root         (0)     1003     4956 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/api/visibility_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.654583 googleapis-common-protos-1.60.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003     6308 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/cloud/extended_operations.proto
+-rw-rw-r--   0 root         (0)     1003     4032 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/cloud/extended_operations_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.654583 googleapis-common-protos-1.60.0/google/cloud/location/
+-rw-rw-r--   0 root         (0)     1003     3604 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/cloud/location/locations.proto
+-rw-rw-r--   0 root         (0)     1003     6899 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/cloud/location/locations_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.642581 googleapis-common-protos-1.60.0/google/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.654583 googleapis-common-protos-1.60.0/google/gapic/metadata/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/gapic/metadata/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3393 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/gapic/metadata/gapic_metadata.proto
+-rw-rw-r--   0 root         (0)     1003     8346 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/gapic/metadata/gapic_metadata_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.654583 googleapis-common-protos-1.60.0/google/logging/
+-rw-rw-r--   0 root         (0)     1003      774 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/logging/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.658583 googleapis-common-protos-1.60.0/google/logging/type/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/logging/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3601 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/logging/type/http_request.proto
+-rw-rw-r--   0 root         (0)     1003     3176 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/logging/type/http_request_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2555 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/logging/type/log_severity.proto
+-rw-rw-r--   0 root         (0)     1003     2622 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/logging/type/log_severity_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.658583 googleapis-common-protos-1.60.0/google/longrunning/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10513 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations.proto
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations_grpc.py
+-rw-rw-r--   0 root         (0)     1003      914 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations_grpc_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2253 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations_pb2.py
+-rw-rw-r--   0 root         (0)     1003    14464 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0)     1003      222 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations_proto.py
+-rw-rw-r--   0 root         (0)     1003    10443 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/longrunning/operations_proto_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.658583 googleapis-common-protos-1.60.0/google/rpc/
+-rw-rw-r--   0 root         (0)     1003      774 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7138 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/code.proto
+-rw-rw-r--   0 root         (0)     1003     2707 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/code_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.662584 googleapis-common-protos-1.60.0/google/rpc/context/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/context/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14852 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/context/attribute_context.proto
+-rw-rw-r--   0 root         (0)     1003    14660 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/context/attribute_context_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1861 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/context/audit_context.proto
+-rw-rw-r--   0 root         (0)     1003     2603 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/context/audit_context_pb2.py
+-rw-rw-r--   0 root         (0)     1003    10869 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/error_details.proto
+-rw-rw-r--   0 root         (0)     1003    11094 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/error_details_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1940 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/http.proto
+-rw-rw-r--   0 root         (0)     1003     3404 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/http_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1934 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/status.proto
+-rw-rw-r--   0 root         (0)     1003     2302 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/rpc/status_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.666584 googleapis-common-protos-1.60.0/google/type/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1762 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/calendar_period.proto
+-rw-rw-r--   0 root         (0)     1003     2343 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/calendar_period_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6376 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/color.proto
+-rw-rw-r--   0 root         (0)     1003     2343 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/color_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1955 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/date.proto
+-rw-rw-r--   0 root         (0)     1003     2138 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/date_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3905 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/datetime.proto
+-rw-rw-r--   0 root         (0)     1003     3165 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/datetime_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1204 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/dayofweek.proto
+-rw-rw-r--   0 root         (0)     1003     2278 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/dayofweek_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4213 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/decimal.proto
+-rw-rw-r--   0 root         (0)     1003     2132 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/decimal_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2730 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/expr.proto
+-rw-rw-r--   0 root         (0)     1003     2153 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/expr_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1156 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/fraction.proto
+-rw-rw-r--   0 root         (0)     1003     2166 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/fraction_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1667 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/interval.proto
+-rw-rw-r--   0 root         (0)     1003     2364 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/interval_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1447 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/latlng.proto
+-rw-rw-r--   0 root         (0)     1003     2144 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/latlng_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1303 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/localized_text.proto
+-rw-rw-r--   0 root         (0)     1003     2270 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/localized_text_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1603 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/money.proto
+-rw-rw-r--   0 root         (0)     1003     2151 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/money_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1479 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/month.proto
+-rw-rw-r--   0 root         (0)     1003     2398 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/month_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4744 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/phone_number.proto
+-rw-rw-r--   0 root         (0)     1003     3046 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/phone_number_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6235 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/postal_address.proto
+-rw-rw-r--   0 root         (0)     1003     2654 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/postal_address_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3791 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/quaternion.proto
+-rw-rw-r--   0 root         (0)     1003     2261 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/quaternion_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1667 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/timeofday.proto
+-rw-rw-r--   0 root         (0)     1003     2266 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/google/type/timeofday_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.666584 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/
+-rw-r--r--   0 root         (0)     1003     1312 2023-07-31 14:13:33.000000 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4346 2023-07-31 14:13:33.000000 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-31 14:13:33.000000 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       22 2023-07-31 14:13:33.000000 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003      127 2023-07-31 14:13:33.000000 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-31 14:13:33.000000 googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-31 14:13:33.670585 googleapis-common-protos-1.60.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2439 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.642581 googleapis-common-protos-1.60.0/tests/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-31 14:13:33.666584 googleapis-common-protos-1.60.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      663 2023-07-31 14:10:55.000000 googleapis-common-protos-1.60.0/tests/unit/test_google_api_error_reason.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `googleapis-common-protos-1.6.0b9/LICENSE` & `googleapis-common-protos-1.60.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-                            Apache License
+
+                                 Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `googleapis-common-protos-1.6.0b9/PKG-INFO` & `googleapis-common-protos-1.60.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: googleapis-common-protos
-Version: 1.6.0b9
+Version: 1.60.0
 Summary: Common protobufs used in Google APIs
-Home-page: https://github.com/googleapis/api-common-protos
+Home-page: https://github.com/googleapis/python-api-common-protos
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache-2.0
-Description: =========================
-        Google APIs common protos
-        =========================
-        
-        googleapis-common-protos contains Python classes generated from the common
-        protos in the `api-common-protos`_ repository.
-        
-        .. _`api-common-protos`: https://github.com/googleapis/api-common-protos
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: grpc
+License-File: LICENSE
+
+Google APIs common protos
+-------------------------
+
+.. image:: https://img.shields.io/pypi/v/googleapis-common-protos.svg
+    :target: https://pypi.org/project/googleapis-common-protos/
+
+
+googleapis-common-protos contains the python classes generated from the common
+protos in the `googleapis/googleapis <https://github.com/googleapis/googleapis>`_ repository.
```

### Comparing `googleapis-common-protos-1.6.0b9/google/api/annotations_pb2.py` & `googleapis-common-protos-1.60.0/google/api/log_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/annotations.proto
+# -*- coding: utf-8 -*-
+
+# Copyright 2020 Google LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: google/api/log.proto
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.api import http_pb2 as google_dot_api_dot_http__pb2
-from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='google/api/annotations.proto',
-  package='google.api',
-  syntax='proto3',
-  serialized_options=_b('\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'),
-  serialized_pb=_b('\n\x1cgoogle/api/annotations.proto\x12\ngoogle.api\x1a\x15google/api/http.proto\x1a google/protobuf/descriptor.proto:E\n\x04http\x12\x1e.google.protobuf.MethodOptions\x18\xb0\xca\xbc\" \x01(\x0b\x32\x14.google.api.HttpRuleBn\n\x0e\x63om.google.apiB\x10\x41nnotationsProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
-  ,
-  dependencies=[google_dot_api_dot_http__pb2.DESCRIPTOR,google_dot_protobuf_dot_descriptor__pb2.DESCRIPTOR,])
-
-
-HTTP_FIELD_NUMBER = 72295728
-http = _descriptor.FieldDescriptor(
-  name='http', full_name='google.api.http', index=0,
-  number=72295728, type=11, cpp_type=10, label=1,
-  has_default_value=False, default_value=None,
-  message_type=None, enum_type=None, containing_type=None,
-  is_extension=True, extension_scope=None,
-  serialized_options=None, file=DESCRIPTOR)
-
-DESCRIPTOR.extensions_by_name['http'] = http
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+from google.api import label_pb2 as google_dot_api_dot_label__pb2
 
-http.message_type = google_dot_api_dot_http__pb2._HTTPRULE
-google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(http)
 
-DESCRIPTOR._options = None
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x14google/api/log.proto\x12\ngoogle.api\x1a\x16google/api/label.proto"u\n\rLogDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x06labels\x18\x02 \x03(\x0b\x32\x1b.google.api.LabelDescriptor\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x04 \x01(\tBj\n\x0e\x63om.google.apiB\x08LogProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3'
+)
+
+
+_LOGDESCRIPTOR = DESCRIPTOR.message_types_by_name["LogDescriptor"]
+LogDescriptor = _reflection.GeneratedProtocolMessageType(
+    "LogDescriptor",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _LOGDESCRIPTOR,
+        "__module__": "google.api.log_pb2"
+        # @@protoc_insertion_point(class_scope:google.api.LogDescriptor)
+    },
+)
+_sym_db.RegisterMessage(LogDescriptor)
+
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = b"\n\016com.google.apiB\010LogProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI"
+    _LOGDESCRIPTOR._serialized_start = 60
+    _LOGDESCRIPTOR._serialized_end = 177
 # @@protoc_insertion_point(module_scope)
```

### Comparing `googleapis-common-protos-1.6.0b9/google/api/control_pb2.py` & `googleapis-common-protos-1.60.0/google/api/label_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,57 @@
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/api/control.proto
+# -*- coding: utf-8 -*-
+
+# Copyright 2020 Google LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: google/api/label.proto
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='google/api/control.proto',
-  package='google.api',
-  syntax='proto3',
-  serialized_options=_b('\n\016com.google.apiB\014ControlProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'),
-  serialized_pb=_b('\n\x18google/api/control.proto\x12\ngoogle.api\"\x1e\n\x07\x43ontrol\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\tBn\n\x0e\x63om.google.apiB\x0c\x43ontrolProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x16google/api/label.proto\x12\ngoogle.api"\x9c\x01\n\x0fLabelDescriptor\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x39\n\nvalue_type\x18\x02 \x01(\x0e\x32%.google.api.LabelDescriptor.ValueType\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t",\n\tValueType\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x42OOL\x10\x01\x12\t\n\x05INT64\x10\x02\x42_\n\x0e\x63om.google.apiB\nLabelProtoP\x01Z5google.golang.org/genproto/googleapis/api/label;label\xf8\x01\x01\xa2\x02\x04GAPIb\x06proto3'
 )
 
 
-
-
-_CONTROL = _descriptor.Descriptor(
-  name='Control',
-  full_name='google.api.Control',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='environment', full_name='google.api.Control.environment', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=40,
-  serialized_end=70,
+_LABELDESCRIPTOR = DESCRIPTOR.message_types_by_name["LabelDescriptor"]
+_LABELDESCRIPTOR_VALUETYPE = _LABELDESCRIPTOR.enum_types_by_name["ValueType"]
+LabelDescriptor = _reflection.GeneratedProtocolMessageType(
+    "LabelDescriptor",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _LABELDESCRIPTOR,
+        "__module__": "google.api.label_pb2"
+        # @@protoc_insertion_point(class_scope:google.api.LabelDescriptor)
+    },
 )
+_sym_db.RegisterMessage(LabelDescriptor)
 
-DESCRIPTOR.message_types_by_name['Control'] = _CONTROL
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-Control = _reflection.GeneratedProtocolMessageType('Control', (_message.Message,), dict(
-  DESCRIPTOR = _CONTROL,
-  __module__ = 'google.api.control_pb2'
-  # @@protoc_insertion_point(class_scope:google.api.Control)
-  ))
-_sym_db.RegisterMessage(Control)
-
+if _descriptor._USE_C_DESCRIPTORS == False:
 
-DESCRIPTOR._options = None
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = b"\n\016com.google.apiB\nLabelProtoP\001Z5google.golang.org/genproto/googleapis/api/label;label\370\001\001\242\002\004GAPI"
+    _LABELDESCRIPTOR._serialized_start = 39
+    _LABELDESCRIPTOR._serialized_end = 195
+    _LABELDESCRIPTOR_VALUETYPE._serialized_start = 151
+    _LABELDESCRIPTOR_VALUETYPE._serialized_end = 195
 # @@protoc_insertion_point(module_scope)
```

### Comparing `googleapis-common-protos-1.6.0b9/google/api/source_info_pb2.py` & `googleapis-common-protos-1.60.0/google/api/source_info_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,57 @@
+# -*- coding: utf-8 -*-
+
+# Copyright 2020 Google LLC
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/source_info.proto
-
-import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='google/api/source_info.proto',
-  package='google.api',
-  syntax='proto3',
-  serialized_options=_b('\n\016com.google.apiB\017SourceInfoProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI'),
-  serialized_pb=_b('\n\x1cgoogle/api/source_info.proto\x12\ngoogle.api\x1a\x19google/protobuf/any.proto\"8\n\nSourceInfo\x12*\n\x0csource_files\x18\x01 \x03(\x0b\x32\x14.google.protobuf.AnyBq\n\x0e\x63om.google.apiB\x0fSourceInfoProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3')
-  ,
-  dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,])
-
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x1cgoogle/api/source_info.proto\x12\ngoogle.api\x1a\x19google/protobuf/any.proto"8\n\nSourceInfo\x12*\n\x0csource_files\x18\x01 \x03(\x0b\x32\x14.google.protobuf.AnyBq\n\x0e\x63om.google.apiB\x0fSourceInfoProtoP\x01ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\xa2\x02\x04GAPIb\x06proto3'
+)
 
 
-_SOURCEINFO = _descriptor.Descriptor(
-  name='SourceInfo',
-  full_name='google.api.SourceInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='source_files', full_name='google.api.SourceInfo.source_files', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=71,
-  serialized_end=127,
+_SOURCEINFO = DESCRIPTOR.message_types_by_name["SourceInfo"]
+SourceInfo = _reflection.GeneratedProtocolMessageType(
+    "SourceInfo",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _SOURCEINFO,
+        "__module__": "google.api.source_info_pb2"
+        # @@protoc_insertion_point(class_scope:google.api.SourceInfo)
+    },
 )
-
-_SOURCEINFO.fields_by_name['source_files'].message_type = google_dot_protobuf_dot_any__pb2._ANY
-DESCRIPTOR.message_types_by_name['SourceInfo'] = _SOURCEINFO
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-SourceInfo = _reflection.GeneratedProtocolMessageType('SourceInfo', (_message.Message,), dict(
-  DESCRIPTOR = _SOURCEINFO,
-  __module__ = 'google.api.source_info_pb2'
-  # @@protoc_insertion_point(class_scope:google.api.SourceInfo)
-  ))
 _sym_db.RegisterMessage(SourceInfo)
 
+if _descriptor._USE_C_DESCRIPTORS == False:
 
-DESCRIPTOR._options = None
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = b"\n\016com.google.apiB\017SourceInfoProtoP\001ZEgoogle.golang.org/genproto/googleapis/api/serviceconfig;serviceconfig\242\002\004GAPI"
+    _SOURCEINFO._serialized_start = 71
+    _SOURCEINFO._serialized_end = 127
 # @@protoc_insertion_point(module_scope)
```

### Comparing `googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/PKG-INFO` & `googleapis-common-protos-1.60.0/googleapis_common_protos.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: googleapis-common-protos
-Version: 1.6.0b9
+Version: 1.60.0
 Summary: Common protobufs used in Google APIs
-Home-page: https://github.com/googleapis/api-common-protos
+Home-page: https://github.com/googleapis/python-api-common-protos
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache-2.0
-Description: =========================
-        Google APIs common protos
-        =========================
-        
-        googleapis-common-protos contains Python classes generated from the common
-        protos in the `api-common-protos`_ repository.
-        
-        .. _`api-common-protos`: https://github.com/googleapis/api-common-protos
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: grpc
+License-File: LICENSE
+
+Google APIs common protos
+-------------------------
+
+.. image:: https://img.shields.io/pypi/v/googleapis-common-protos.svg
+    :target: https://pypi.org/project/googleapis-common-protos/
+
+
+googleapis-common-protos contains the python classes generated from the common
+protos in the `googleapis/googleapis <https://github.com/googleapis/googleapis>`_ repository.
```

