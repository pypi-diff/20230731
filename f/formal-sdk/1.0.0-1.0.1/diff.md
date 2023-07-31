# Comparing `tmp/formal-sdk-1.0.0.tar.gz` & `tmp/formal-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-1.0.0.tar", last modified: Mon Jul 31 16:07:49 2023, max compression
+gzip compressed data, was "formal-sdk-1.0.1.tar", last modified: Mon Jul 31 16:36:50 2023, max compression
```

## Comparing `formal-sdk-1.0.0.tar` & `formal-sdk-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.136533 formal-sdk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-31 16:36:50.136533 formal-sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:36:50.136533 formal-sdk-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.116532 formal-sdk-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.120532 formal-sdk-1.0.1/src/formal_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/cord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.112532 formal-sdk-1.0.1/src/formal_sdk/gen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.112532 formal-sdk-1.0.1/src/formal_sdk/gen/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.128533 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/audit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/cord_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/datastore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/encryption_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/identities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_github_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/inventory_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/native_user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/outputs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/policies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/registry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/sidecar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.112532 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.136533 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/column_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/key_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/types/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/work_os_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.112532 formal-sdk-1.0.1/src/formal_sdk/gen/validate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.136533 formal-sdk-1.0.1/src/formal_sdk/gen/validate/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/validate/v1/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/gen/validate/v1/validate_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/identities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_code_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_datahub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_external_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/integration_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/native_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-31 16:36:33.000000 formal-sdk-1.0.1/src/formal_sdk/work_os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:36:50.120532 formal-sdk-1.0.1/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-31 16:36:50.000000 formal-sdk-1.0.1/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-31 16:36:50.000000 formal-sdk-1.0.1/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:36:50.000000 formal-sdk-1.0.1/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 16:36:50.000000 formal-sdk-1.0.1/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 16:36:50.000000 formal-sdk-1.0.1/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-1.0.0/LICENSE` & `formal-sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.0/PKG-INFO` & `formal-sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-sdk-1.0.0/README.md` & `formal-sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.0/pyproject.toml` & `formal-sdk-1.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-sdk"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal SDK"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-sdk-1.0.0/src/example.py` & `formal-sdk-1.0.1/src/example.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.0/src/formal_sdk.egg-info/PKG-INFO` & `formal-sdk-1.0.1/src/formal_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

