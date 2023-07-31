# Comparing `tmp/adapta-2.3.4.tar.gz` & `tmp/adapta-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.3.4.tar", max compression
+gzip compressed data, was "adapta-2.3.5.tar", max compression
```

## Comparing `adapta-2.3.4.tar` & `adapta-2.3.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0    10693 2023-07-25 13:35:11.160826 adapta-2.3.4/LICENSE
--rw-r--r--   0        0        0      811 2023-07-25 13:35:11.160826 adapta-2.3.4/README.md
--rw-r--r--   0        0        0      663 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/__init__.py
--rw-r--r--   0        0        0       22 2023-07-25 13:35:33.236918 adapta-2.3.4/adapta/_version.py
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      694 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1914 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/logs/README.md
--rw-r--r--   0        0        0      667 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/logs/__init__.py
--rw-r--r--   0        0        0    12390 2023-07-25 13:35:11.160826 adapta-2.3.4/adapta/logs/_base.py
--rw-r--r--   0        0        0     2950 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/_internal.py
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9167 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2211 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      741 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      794 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      963 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      672 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3215 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4466 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      653 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/ml/_model.py
--rw-r--r--   0        0        0      699 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5319 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     4012 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      674 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3362 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      732 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/schema_management/README.md
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/schema_management/__init__.py
--rw-r--r--   0        0        0     1219 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/schema_management/schema_entity.py
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/__init__.py
--rw-r--r--   0        0        0     2140 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/README.md
--rw-r--r--   0        0        0     1450 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     8358 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2396 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1787 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2695 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2601 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3454 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0     1952 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/security/clients/hashicorp_vault/token_client.py
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      622 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0     9605 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     4791 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/blob/base.py
--rw-r--r--   0        0        0      665 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3451 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3365 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2451 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/database/README.md
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4691 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      675 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1447 2023-07-25 13:35:11.164826 adapta-2.3.4/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7711 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     4523 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     2386 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      721 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11493 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2247 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0     1458 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/distributed_object_store/datastax_astra/README.md
--rw-r--r--   0        0        0      622 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/distributed_object_store/datastax_astra/__init__.py
--rw-r--r--   0        0        0    13880 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/distributed_object_store/datastax_astra/astra_client.py
--rw-r--r--   0        0        0      598 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     5302 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2063 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/models/base.py
--rw-r--r--   0        0        0     5711 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6630 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1519 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/models/local.py
--rw-r--r--   0        0        0     1953 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      666 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2216 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2358 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2887 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0     2761 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/utils/README.md
--rw-r--r--   0        0        0      668 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/utils/_common.py
--rw-r--r--   0        0        0     3930 2023-07-25 13:35:11.168826 adapta-2.3.4/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0     2296 2023-07-25 13:35:33.236918 adapta-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 adapta-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-07-31 13:04:08.508856 adapta-2.3.5/LICENSE
+-rw-r--r--   0        0        0      811 2023-07-31 13:04:08.508856 adapta-2.3.5/README.md
+-rw-r--r--   0        0        0      663 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-31 13:04:26.804831 adapta-2.3.5/adapta/_version.py
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      694 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1914 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/README.md
+-rw-r--r--   0        0        0      667 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/__init__.py
+-rw-r--r--   0        0        0    12390 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/_base.py
+-rw-r--r--   0        0        0     2950 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/_internal.py
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9167 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2211 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      741 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      963 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      672 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3215 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      653 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/ml/_model.py
+-rw-r--r--   0        0        0      699 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5319 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     4012 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      674 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3362 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      732 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/schema_management/README.md
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/schema_management/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/schema_management/schema_entity.py
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/__init__.py
+-rw-r--r--   0        0        0     2140 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/README.md
+-rw-r--r--   0        0        0     1450 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     8358 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2396 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1787 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2695 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2601 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3454 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0     1952 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/security/clients/hashicorp_vault/token_client.py
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      622 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0     9605 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     4791 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0      665 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3451 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3365 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2451 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4691 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      675 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7711 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     4523 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     2386 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      721 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11493 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2247 2023-07-31 13:04:08.508856 adapta-2.3.5/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0     1695 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/distributed_object_store/datastax_astra/README.md
+-rw-r--r--   0        0        0      622 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/distributed_object_store/datastax_astra/__init__.py
+-rw-r--r--   0        0        0    16011 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/distributed_object_store/datastax_astra/astra_client.py
+-rw-r--r--   0        0        0      598 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     5302 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2063 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/models/base.py
+-rw-r--r--   0        0        0     5711 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6630 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1519 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/models/local.py
+-rw-r--r--   0        0        0     1953 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      666 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2216 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2358 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2887 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0     2761 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/utils/README.md
+-rw-r--r--   0        0        0      668 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3930 2023-07-31 13:04:08.512856 adapta-2.3.5/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0     2296 2023-07-31 13:04:26.804831 adapta-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 adapta-2.3.5/PKG-INFO
```

### Comparing `adapta-2.3.4/LICENSE` & `adapta-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/README.md` & `adapta-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/__init__.py` & `adapta-2.3.5/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/connectors/__init__.py` & `adapta-2.3.5/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/connectors/service_bus/__init__.py` & `adapta-2.3.5/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/connectors/service_bus/_connector.py` & `adapta-2.3.5/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/README.md` & `adapta-2.3.5/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/__init__.py` & `adapta-2.3.5/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/_base.py` & `adapta-2.3.5/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/_internal.py` & `adapta-2.3.5/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/handlers/__init__.py` & `adapta-2.3.5/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.3.5/adapta/logs/handlers/datadog_api_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.3.5/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/models/__init__.py` & `adapta-2.3.5/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/models/_log_level.py` & `adapta-2.3.5/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/logs/models/_logs_metadata.py` & `adapta-2.3.5/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/metrics/__init__.py` & `adapta-2.3.5/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/metrics/_base.py` & `adapta-2.3.5/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/metrics/providers/README.md` & `adapta-2.3.5/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/metrics/providers/__init__.py` & `adapta-2.3.5/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/metrics/providers/datadog_provider.py` & `adapta-2.3.5/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/ml/__init__.py` & `adapta-2.3.5/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/ml/_model.py` & `adapta-2.3.5/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/ml/mlflow/__init__.py` & `adapta-2.3.5/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/ml/mlflow/_client.py` & `adapta-2.3.5/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/ml/mlflow/_functions.py` & `adapta-2.3.5/adapta/ml/mlflow/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/process_communication/__init__.py` & `adapta-2.3.5/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/process_communication/_models.py` & `adapta-2.3.5/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/schema_management/README.md` & `adapta-2.3.5/adapta/schema_management/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/schema_management/__init__.py` & `adapta-2.3.5/adapta/schema_management/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/schema_management/schema_entity.py` & `adapta-2.3.5/adapta/schema_management/schema_entity.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/__init__.py` & `adapta-2.3.5/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/README.md` & `adapta-2.3.5/adapta/security/clients/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/__init__.py` & `adapta-2.3.5/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/_azure_client.py` & `adapta-2.3.5/adapta/security/clients/_azure_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/_base.py` & `adapta-2.3.5/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/_local_client.py` & `adapta-2.3.5/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.3.5/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.3.5/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.3.5/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.3.5/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/security/clients/hashicorp_vault/token_client.py` & `adapta-2.3.5/adapta/security/clients/hashicorp_vault/token_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/__init__.py` & `adapta-2.3.5/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/blob/README.md` & `adapta-2.3.5/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/blob/__init__.py` & `adapta-2.3.5/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/blob/azure_storage_client.py` & `adapta-2.3.5/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/blob/base.py` & `adapta-2.3.5/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/cache/__init__.py` & `adapta-2.3.5/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/cache/_base.py` & `adapta-2.3.5/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/cache/redis_cache.py` & `adapta-2.3.5/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/README.md` & `adapta-2.3.5/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/__init__.py` & `adapta-2.3.5/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/azure_sql.py` & `adapta-2.3.5/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/models/__init__.py` & `adapta-2.3.5/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/models/_models.py` & `adapta-2.3.5/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/odbc.py` & `adapta-2.3.5/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/database/trino_sql.py` & `adapta-2.3.5/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/delta_lake/README.md` & `adapta-2.3.5/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/delta_lake/__init__.py` & `adapta-2.3.5/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/delta_lake/_functions.py` & `adapta-2.3.5/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/delta_lake/_models.py` & `adapta-2.3.5/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/distributed_object_store/datastax_astra/README.md` & `adapta-2.3.5/adapta/storage/distributed_object_store/datastax_astra/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ## Astra DB Client
 
 Create a table in Astra and insert some rows:
 ```cassandraql
 create table tmp.test_entity(
     col_a text PRIMARY KEY,
-    col_b text
+    col_b text,
+    col_c text
 );
 
-insert into tmp.test_entity (col_a, col_b) VALUES ('something1', 'else');
-insert into tmp.test_entity (col_a, col_b) VALUES ('something2', 'magic');
-insert into tmp.test_entity (col_a, col_b) VALUES ('something3', 'ordinal');
+insert into tmp.test_entity (col_a, col_b, col_c) VALUES ('something1', 'else', 'entirely');
+insert into tmp.test_entity (col_a, col_b, col_c) VALUES ('something2', 'magic', 'tomorrow');
+insert into tmp.test_entity (col_a, col_b, col_c) VALUES ('something3', 'ordinal', 'today');
 ```
 
 Instantiate a new client, map dataclass (model) to Cassandra model and query it:
 
 ```python
 from adapta.storage.distributed_object_store.datastax_astra.astra_client import AstraClient
 
 from dataclasses import dataclass, field
 
-import pandas
-
 @dataclass
 class TestEntity:
     col_a: str = field(metadata={
         "is_primary_key": True,
         "is_partition_key": True
     })
     col_b: str
+    col_c: str
 
 
 with AstraClient(
         client_name='test', 
         keyspace='tmp', 
         secure_connect_bundle_bytes='base64string', 
         client_id = 'Astra Token client_id', 
@@ -43,10 +43,14 @@
 
   multiple_entities = ac.get_entities_raw("select * from tmp.test_entity where col_a = 'something3'")
   print(multiple_entities)
   #         col_a     col_b
   # 0  something  ordinal
 
   print(ac.filter_entities(TestEntity, key_column_filter_values=[{"col_a": 'something1'}]))
-  #         col_a col_b
-  # 0  something1  else
+  #     col_a col_b     col_c
+  # 0  something1  else  entirely
+
+  print(ac.filter_entities(TestEntity, key_column_filter_values=[{"col_a": 'something1'}], select_columns=['col_c']))
+  #       col_c
+  # 0  entirely
 ```
```

### Comparing `adapta-2.3.4/adapta/storage/distributed_object_store/datastax_astra/__init__.py` & `adapta-2.3.5/adapta/storage/distributed_object_store/datastax_astra/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/distributed_object_store/datastax_astra/astra_client.py` & `adapta-2.3.5/adapta/storage/distributed_object_store/datastax_astra/astra_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 import base64
 import datetime
+import enum
 import os
 import re
 import shutil
 import tempfile
+import typing
 import uuid
 from dataclasses import fields, is_dataclass
-from typing import Optional, Dict, TypeVar, Callable, Type, List
+from typing import Optional, Dict, TypeVar, Callable, Type, List, Any, get_origin
 
 from _socket import IPPROTO_TCP, TCP_NODELAY, TCP_USER_TIMEOUT
 
 import pandas
 from cassandra import ConsistencyLevel
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.cluster import (  # pylint: disable=E0611
@@ -177,14 +179,15 @@
         return pandas.DataFrame([mapper(entity) for entity in self._session.execute(query)])
 
     def filter_entities(
         self,
         model_class: Type[TModel],
         key_column_filter_values: List[Dict[str, str]],
         table_name: Optional[str] = None,
+        select_columns: Optional[List[str]] = None,
         primary_keys: Optional[List[str]] = None,
         partition_keys: Optional[List[str]] = None,
         deduplicate=False,
     ) -> pandas.DataFrame:
         """
         Run a filter query on the entity of type TModel backed by table `table_name`.
 
@@ -197,30 +200,49 @@
 
          with AstraClient(...) as ac:
              data = ac.filter_entities("test_table", Test, ['col_a'], [{'col_a': 123},{'col_a': 345}])
 
         :param: model_class: A dataclass type that should be mapped to Astra Model.
         :param: key_column_filter_values: Primary key filters in a form of list of dictionaries of my_key: my_value. Multiple entries will result in multiple queries being run and concatenated
         :param: table_name: Optional Astra table name, if it cannot be inferred from class name by converting it to snake_case.
+        :param: select_columns: An optional list of columns to return with the query.
         :param: primary_keys: An optional list of columns that constitute a primary key, if it cannot be inferred from is_primary_key metadata on a dataclass field.
         :param: partition_keys: An optional list of columns that constitute a partition key, if it cannot be inferred from is_partition_key metadata on a dataclass field.
         param: deduplicate: Optionally deduplicate query result, for example when only the partition key part of a primary key is used to fetch results.
         """
+
+        def apply(model: Type[Model], key_column_filter: Dict[str, Any], columns_to_select: Optional[List[str]]):
+            if columns_to_select:
+                return model.filter(**key_column_filter).only(select_columns)
+
+            return model.filter(**key_column_filter)
+
         assert (
             self._session is not None
         ), "Please instantiate an AstraClient using with AstraClient(...) before calling this method"
 
-        model_class: Model = self._model_dataclass(model_class, table_name, primary_keys, partition_keys)
+        model_class: Type[Model] = self._model_dataclass(
+            value=model_class,
+            table_name=table_name,
+            primary_keys=primary_keys,
+            partition_keys=partition_keys,
+            select_columns=select_columns,
+        )
+
         result = pandas.concat(
             [
-                pandas.DataFrame([dict(v.items()) for v in list(model_class.filter(**key_column_filter))])
+                pandas.DataFrame([dict(v.items()) for v in list(apply(model_class, key_column_filter, select_columns))])
                 for key_column_filter in key_column_filter_values
             ]
         )
 
+        if select_columns:
+            filter_columns = {key for key_column_filter in key_column_filter_values for key in key_column_filter.keys()}
+            result = result.drop(columns=list(set(filter_columns) - set(select_columns)))
+
         if deduplicate:
             return result.drop_duplicates()
 
         return result
 
     def get_entities_raw(self, query: str) -> pandas.DataFrame:
         """
@@ -232,78 +254,121 @@
 
     def _model_dataclass(
         self,
         value: Type[TModel],
         table_name: Optional[str] = None,
         primary_keys: Optional[List[str]] = None,
         partition_keys: Optional[List[str]] = None,
-    ) -> Model:
+        select_columns: Optional[List[str]] = None,
+    ) -> Type[Model]:
         """
         Maps a Python dataclass to Cassandra model.
 
         :param: value: A dataclass type that should be mapped to Astra Model.
         :param: table_name: Astra table name, if it cannot be inferred from class name by converting it to snake_case.
         :param: primary_keys: An optional list of columns that constitute a primary key, if it cannot be inferred from is_primary_key metadata on a dataclass field.
         :param: partition_keys: An optional list of columns that constitute a partition key, if it cannot be inferred from is_partition_key metadata on a dataclass field.
+        :param: select_columns: An optional list of columns to select from the entity. If omitted, all columns will be selected.
         """
 
-        def map_to_cassandra(  # pylint: disable=R0911
-            python_type: Type, db_field: str, is_primary_key: bool, is_partition_key: bool
-        ) -> Column:
+        def map_to_column(  # pylint: disable=R0911
+            python_type: Type,
+        ) -> typing.Union[
+            typing.Tuple[
+                Type[columns.List],
+            ],
+            typing.Tuple[
+                Type[columns.Map],
+            ],
+            typing.Tuple[
+                Type[Column],
+            ],
+            typing.Tuple[Type[Column], Type[Column]],
+            typing.Tuple[Type[Column], Type[Column], Type[Column]],
+        ]:
             if python_type is type(None):
                 raise TypeError("NoneType cannot be mapped to any existing table column types")
             if python_type is bool:
-                return columns.Boolean(primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
+                return (columns.Boolean,)
             if python_type is str:
-                return columns.Text(primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
+                return (columns.Text,)
             if python_type is bytes:
-                return columns.Blob(primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
+                return (columns.Blob,)
             if python_type is datetime.datetime:
-                return columns.DateTime(primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
+                return (columns.DateTime,)
             if python_type is int:
-                return columns.Integer(primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
+                return (columns.Integer,)
             if python_type is float:
-                return columns.Double(primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
-            if python_type is List[str]:
-                return columns.List(primary_key=False, partition_key=False, value_type=columns.Text, db_field=db_field)
-            if python_type is List[int]:
-                return columns.List(
-                    primary_key=False, partition_key=False, value_type=columns.Integer, db_field=db_field
+                return (columns.Double,)
+            if python_type is enum.EnumType:  # assume all enums are strings - for now
+                return (columns.Text,)
+            if get_origin(python_type) == list:
+                return (
+                    columns.List,
+                    map_to_column(typing.get_args(python_type)[0])[0],
                 )
-            if python_type is List[float]:
-                return columns.List(
-                    primary_key=False, partition_key=False, value_type=columns.Double, db_field=db_field
+            if get_origin(python_type) == dict:
+                return (
+                    columns.Map,
+                    map_to_column(typing.get_args(python_type)[0])[0],
+                    map_to_column(typing.get_args(python_type)[1])[0],
                 )
-            if python_type is Dict[str, str]:
-                return columns.Map(
-                    primary_key=False,
-                    partition_key=False,
-                    key_type=columns.Text,
-                    value_type=columns.Text,
+
+            if get_origin(python_type) == typing.Union:
+                return map_to_column(typing.get_args(python_type)[0])
+
+            raise TypeError(f"Unsupported type: {python_type}")
+
+        def map_to_cassandra(python_type: Type, db_field: str, is_primary_key: bool, is_partition_key: bool) -> Column:
+            cassandra_types = map_to_column(python_type)
+            if len(cassandra_types) == 1:  # simple type
+                return cassandra_types[0](primary_key=is_primary_key, partition_key=is_partition_key, db_field=db_field)
+            if len(cassandra_types) == 2:  # list
+                return cassandra_types[0](
+                    primary_key=is_primary_key,
+                    partition_key=is_partition_key,
+                    db_field=db_field,
+                    value_type=cassandra_types[1],
+                )
+            if len(cassandra_types) == 3:  # dict
+                return cassandra_types[0](
+                    primary_key=is_primary_key,
+                    partition_key=is_partition_key,
                     db_field=db_field,
+                    key_type=cassandra_types[1],
+                    value_type=cassandra_types[2],
                 )
 
-            raise TypeError(f"Unsupported type: {python_type}")
+            raise TypeError(f"Unsupported type mapping: {cassandra_types}")
 
         assert is_dataclass(value)
 
         primary_keys = primary_keys or [
             field.name for field in fields(value) if field.metadata.get("is_primary_key", False)
         ]
         partition_keys = partition_keys or [
             field.name for field in fields(value) if field.metadata.get("is_partition_key", False)
         ]
+        selected_fields = (
+            [
+                field
+                for field in fields(value)
+                if field.name in select_columns or field.name in primary_keys or field.name in partition_keys
+            ]
+            if select_columns
+            else fields(value)
+        )
 
         table_name = table_name or self._snake_pattern.sub("_", value.__name__).lower()
 
         models_attributes: Dict[str, Column] = {
             field.name: map_to_cassandra(
                 field.type, field.name, field.name in primary_keys, field.name in partition_keys
             )
-            for field in fields(value)
+            for field in selected_fields
         }
 
         return type(table_name, (Model,), models_attributes)
 
     def set_table_option(self, table_name: str, option_name: str, option_value: str) -> None:
         """
         Sets a table property: https://docs.datastax.com/en/cql-oss/3.1/cql/cql_reference/tabProp.html
```

### Comparing `adapta-2.3.4/adapta/storage/models/__init__.py` & `adapta-2.3.5/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/models/azure.py` & `adapta-2.3.5/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/models/base.py` & `adapta-2.3.5/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/models/format.py` & `adapta-2.3.5/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/models/hive.py` & `adapta-2.3.5/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/models/local.py` & `adapta-2.3.5/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/secrets/README.md` & `adapta-2.3.5/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/secrets/__init__.py` & `adapta-2.3.5/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/secrets/_base.py` & `adapta-2.3.5/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.3.5/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.3.5/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/utils/README.md` & `adapta-2.3.5/adapta/utils/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/utils/__init__.py` & `adapta-2.3.5/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/utils/_common.py` & `adapta-2.3.5/adapta/utils/_common.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/adapta/utils/concurrent_task_runner.py` & `adapta-2.3.5/adapta/utils/concurrent_task_runner.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.4/pyproject.toml` & `adapta-2.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adapta"
-version = "2.3.4"
+version = "2.3.5"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
```

### Comparing `adapta-2.3.4/PKG-INFO` & `adapta-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.3.4
+Version: 2.3.5
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

