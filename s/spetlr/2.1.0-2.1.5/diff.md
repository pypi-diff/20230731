# Comparing `tmp/spetlr-2.1.0.tar.gz` & `tmp/spetlr-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-2.1.0.tar", last modified: Thu Jun 29 11:03:00 2023, max compression
+gzip compressed data, was "spetlr-2.1.5.tar", last modified: Mon Jul 31 11:40:58 2023, max compression
```

## Comparing `spetlr-2.1.0.tar` & `spetlr-2.1.5.tar`

### file list

```diff
@@ -1,282 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.478204 spetlr-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-29 11:02:42.000000 spetlr-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 11:02:42.000000 spetlr-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-29 11:03:00.478204 spetlr-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-29 11:02:42.000000 spetlr-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 11:02:42.000000 spetlr-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-29 11:03:00.478204 spetlr-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:02:42.000000 spetlr-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.446204 spetlr-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.454204 spetlr-2.1.0/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/_cli/ConfiguratorCli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/parse_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/configurator/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.458204 spetlr-2.1.0/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/extractors/stream_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/stream_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/loaders/upsert_loader_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/filehandle/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/filehandle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/filehandle/file_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.462204 spetlr-2.1.0/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.466204 spetlr-2.1.0/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.466204 spetlr-2.1.0/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.466204 spetlr-2.1.0/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.466204 spetlr-2.1.0/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.466204 spetlr-2.1.0/src/spetlr/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/testutils/CleanupTestDatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/testutils/stop_test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.466204 spetlr-2.1.0/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/dropColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/generate_md5_column_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/selectColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/transformers/validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/DeleteMismatchedSchemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 11:02:42.000000 spetlr-2.1.0/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.454204 spetlr-2.1.0/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 11:03:00.000000 spetlr-2.1.0/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.454204 spetlr-2.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.454204 spetlr-2.1.0/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/delta/
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/delta/test_cleanup_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/delta/test_delta_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/delta/test_delta_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/delta/test_filehandle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/delta/test_sparkexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_upsertloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/etl/test_upsertloader_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/sql/test_sql_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.470204 spetlr-2.1.0/tests/cluster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/utils/test_delete_schema_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/utils/test_spark_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/cluster/utils/test_stop_test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/entry_points/test_generalized_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/etl/test_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/sql/test_SqlExecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/streaming/test_deltahandle_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/streaming/test_filehandle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/streaming/test_stream_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.474204 spetlr-2.1.0/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_generate_md5_column_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:03:00.478204 spetlr-2.1.0/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_cleandatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_selectandcastcolumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-29 11:02:42.000000 spetlr-2.1.0/tests/local/utils/test_stop_test_streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 11:40:45.000000 spetlr-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 11:40:45.000000 spetlr-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-07-31 11:40:58.167729 spetlr-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-31 11:40:45.000000 spetlr-2.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 11:40:45.000000 spetlr-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-31 11:40:58.167729 spetlr-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:40:45.000000 spetlr-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.135729 spetlr-2.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/azure_log_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/azure_log_analytics/azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/_cli/ConfiguratorCli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/parse_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/configurator/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/extractors/stream_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/stream_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/loaders/upsert_loader_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/filehandle/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/filehandle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/filehandle/file_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.155729 spetlr-2.1.5/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/src/spetlr/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/testutils/CleanupTestDatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/testutils/stop_test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/dropColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/generate_md5_column_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/selectColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/transformers/validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/DeleteMismatchedSchemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 11:40:45.000000 spetlr-2.1.5/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.151729 spetlr-2.1.5/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-07-31 11:40:57.000000 spetlr-2.1.5/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-07-31 11:40:58.000000 spetlr-2.1.5/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:40:57.000000 spetlr-2.1.5/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 11:40:57.000000 spetlr-2.1.5/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:40:57.000000 spetlr-2.1.5/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 11:40:57.000000 spetlr-2.1.5/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 11:40:57.000000 spetlr-2.1.5/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.143729 spetlr-2.1.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.143729 spetlr-2.1.5/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/tests/cluster/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.159729 spetlr-2.1.5/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/delta/test_cleanup_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/delta/test_delta_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/delta/test_delta_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/delta/test_filehandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/delta/test_sparkexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_upsertloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/etl/test_upsertloader_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/sql/test_sql_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/cluster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/utils/test_delete_schema_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/utils/test_spark_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/cluster/utils/test_stop_test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/local/azure_log_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/azure_log_analytics/test_azure_log_analytics_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.163730 spetlr-2.1.5/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/entry_points/test_generalized_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/etl/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/etl/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/etl/test_transformer_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/sql/test_SqlExecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/streaming/test_deltahandle_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/streaming/test_filehandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/streaming/test_stream_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_generate_md5_column_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:40:58.167729 spetlr-2.1.5/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_cleandatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_selectandcastcolumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-31 11:40:45.000000 spetlr-2.1.5/tests/local/utils/test_stop_test_streams.py
```

### Comparing `spetlr-2.1.0/LICENSE` & `spetlr-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/PKG-INFO` & `spetlr-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 2.1.0
+Version: 2.1.5
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
@@ -89,14 +89,16 @@
         utilizes Azure Resource deployment - and can only be run by the spetlr-org admins.
         
         To deploy the necessary Azure resources to your own Azure Tenant, run the following command:
         
         ```powershell
         .\.github\deploy\deploy.ps1 -uniqueRunId "yourUniqueId"
         ```
+        Be aware that the applied name for *uniqueRunId* should only contain lower case and numbers, and its length should not
+        exceed 12 characters.
         
         Afterward, execute the following commands:
         
         ```powershell 
         .\.github\submit\build.ps1
         .\.github\submit\submit_test_job.ps1
         ```
```

### Comparing `spetlr-2.1.0/README.md` & `spetlr-2.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 utilizes Azure Resource deployment - and can only be run by the spetlr-org admins.
 
 To deploy the necessary Azure resources to your own Azure Tenant, run the following command:
 
 ```powershell
 .\.github\deploy\deploy.ps1 -uniqueRunId "yourUniqueId"
 ```
+Be aware that the applied name for *uniqueRunId* should only contain lower case and numbers, and its length should not
+exceed 12 characters.
 
 Afterward, execute the following commands:
 
 ```powershell 
 .\.github\submit\build.ps1
 .\.github\submit\submit_test_job.ps1
 ```
```

### Comparing `spetlr-2.1.0/setup.cfg` & `spetlr-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/cache/CachedLoader.py` & `spetlr-2.1.5/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-2.1.5/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/_cli/ConfiguratorCli.py` & `spetlr-2.1.5/src/spetlr/configurator/_cli/ConfiguratorCli.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-2.1.5/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,28 +39,31 @@
 
         new_conts = black.format_file_contents(
             new_conts, fast=False, mode=black.FileMode()
         )
     except ModuleNotFoundError:
         pass
 
-    if not options.output_file:
+    output_file = options.output_file or ""
+    output_file = output_file.replace("\\", "/")
+
+    if not output_file:
         # without output file, output to console
         print(new_conts, end="")
         return
 
     if not options.check:
-        with open(options.output_file, "w") as f:
+        with open(output_file, "w") as f:
             f.write(new_conts)
         return
 
-    if not os.path.exists(options.output_file):
-        raise SpetlrCliCheckFailed(f"Output file {options.output_file} does not exist.")
+    if not os.path.exists(output_file):
+        raise SpetlrCliCheckFailed(f"Output file {output_file} does not exist.")
 
-    old_conts = open(options.output_file).read()
+    old_conts = open(output_file).read()
     if new_conts != old_conts:
         raise SpetlrCliCheckFailed(
-            f"Output file {options.output_file} does not have correct contents."
+            f"Output file {output_file} does not have correct contents."
         )
 
     # all checks passed. Return without error.
     return
```

### Comparing `spetlr-2.1.0/src/spetlr/configurator/configurator.py` & `spetlr-2.1.5/src/spetlr/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/comments.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/comments.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/create.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/create.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/db.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/substructures.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/substructures.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/configurator/sql/table.py` & `spetlr-2.1.5/src/spetlr/configurator/sql/table.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/cosmos/cosmos.py` & `spetlr-2.1.5/src/spetlr/cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-2.1.5/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-2.1.5/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/db_auto.py` & `spetlr-2.1.5/src/spetlr/db_auto.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/delta/db_handle.py` & `spetlr-2.1.5/src/spetlr/delta/db_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/delta/delta_handle.py` & `spetlr-2.1.5/src/spetlr/delta/delta_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/eh/EventHubCapture.py` & `spetlr-2.1.5/src/spetlr/eh/EventHubCapture.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-2.1.5/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-2.1.5/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/eh/EventHubStream.py` & `spetlr-2.1.5/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/eh/PartitionSpec.py` & `spetlr-2.1.5/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-2.1.5/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/entry_points/task_entry_point.py` & `spetlr-2.1.5/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/extractor.py` & `spetlr-2.1.5/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-2.1.5/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-2.1.5/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/loader.py` & `spetlr-2.1.5/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-2.1.5/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-2.1.5/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-2.1.5/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/loaders/stream_loader.py` & `spetlr-2.1.5/src/spetlr/etl/loaders/stream_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/loaders/upsert_loader_streaming.py` & `spetlr-2.1.5/src/spetlr/etl/loaders/upsert_loader_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/orchestrator.py` & `spetlr-2.1.5/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/etl/transformer.py` & `spetlr-2.1.5/src/spetlr/etl/transformer_nc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,46 @@
+from abc import abstractmethod
+from typing import List, Union
+
+from deprecated import deprecated
 from pyspark.sql import DataFrame
 
-from .types import EtlBase, dataset_group
+from spetlr.etl.types import dataset_group
+
+from .transformer import Transformer
 
 
-class Transformer(EtlBase):
+@deprecated(reason="Use Transformer with consume_inputs=False instead")
+class TransformerNC(Transformer):
     """If you only want to transform a single input dataframe,
     implement `process`
-    if you want to transform a set of dataframes,
+    If you want to transform a set of dataframes,
     implement `process_many`
 
-    In regards to the etl step, the transformer CONSUMES the inputs
-    and ADDs the result of its transformation stage.
+    In regards to the etl step, the TransformerNC does NOT CONSUME the inputs
+    and ADDs the result of its transformation stage to the dataset dict.
     """
 
-    def __init__(self, dataset_key: str = None):
-        super().__init__()
-        if dataset_key is None:
-            dataset_key = type(self).__name__
-        self.dataset_key = dataset_key
-
-    def etl(self, inputs: dataset_group) -> dataset_group:
-        if len(inputs) == 1:
-            df = next(iter(inputs.values()))
-            return {self.dataset_key: self.process(df)}
-        return {self.dataset_key: self.process_many(inputs)}
+    def __init__(
+        self,
+        *,
+        dataset_input_keys: Union[str, List[str]] = None,
+        dataset_output_key: str = None,
+    ):
+        if isinstance(dataset_input_keys, str):
+            dataset_input_keys = [dataset_input_keys]
+        else:
+            dataset_input_keys = dataset_input_keys
+
+        super().__init__(
+            dataset_input_keys=dataset_input_keys,
+            dataset_output_key=dataset_output_key,
+            consume_inputs=False,
+        )
 
+    @abstractmethod
     def process(self, df: DataFrame) -> DataFrame:
         raise NotImplementedError()
 
+    @abstractmethod
     def process_many(self, datasets: dataset_group) -> DataFrame:
         raise NotImplementedError()
```

### Comparing `spetlr-2.1.0/src/spetlr/etl/transformer_nc.py` & `spetlr-2.1.5/src/spetlr/etl/transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,83 @@
-from abc import abstractmethod
-from typing import List, Union
+import warnings
+from typing import List
 
 from pyspark.sql import DataFrame
 
-from spetlr.etl.types import EtlBase, dataset_group
+from .types import EtlBase, dataset_group
 
 
-class TransformerNC(EtlBase):
-    """If you only want to transform a single input dataframe,
+class Transformer(EtlBase):
+    """
+    This is the base Transformer class for the OETL framework.
+
+    If you only want to transform a single input dataframe,
     implement `process`
     If you want to transform a set of dataframes,
     implement `process_many`
 
-    In regards to the etl step, the TransformerNC does NOT CONSUME the inputs
-    and ADDs the result of its transformation stage to the dataset dict.
+    In regards to the etl step, the behavior of the transformation is controlled
+    by the parameters dataset_input_keys, dataset_output_key and consume_inputs.
+
+    Attributes:
+    ----------
+        dataset_input_keys : Union[str, List[str]]
+            str or list of input dataset keys that will be used for
+            either process or process_many
+        dataset_output_key : str
+            name of the output key that we be added to the dataset after transformation
+        consume_inputs : bool
+            Flag to control dataset consuming behavior
     """
 
     def __init__(
         self,
+        dataset_key: str = None,
         *,
-        dataset_input_keys: Union[str, List[str]] = None,
+        dataset_input_keys: List[str] = None,
         dataset_output_key: str = None,
+        consume_inputs: bool = True,
     ):
-        if dataset_output_key is not None:
-            self.dataset_output_key = dataset_output_key
-        else:
-            self.dataset_output_key = type(self).__name__
+        if dataset_key is not None:
+            warnings.warn(
+                "The parameter dataset_key is deprecated, use dataset_output_key instead."  # noqa: E501
+            )
+            dataset_output_key = dataset_key
 
-        if dataset_input_keys is None:
-            self.dataset_input_key_list = []
-        elif isinstance(dataset_input_keys, str):
-            self.dataset_input_key_list = [dataset_input_keys]
+        self.dataset_input_keys = dataset_input_keys
+
+        if dataset_output_key is None:
+            self.dataset_output_key = type(self).__name__
         else:
-            self.dataset_input_key_list = dataset_input_keys
+            self.dataset_output_key = dataset_output_key
+
+        self.consume_inputs = consume_inputs
 
     def etl(self, inputs: dataset_group) -> dataset_group:
-        if len(self.dataset_input_key_list) > 0:
-            if len(self.dataset_input_key_list) == 1:
-                df = self.process(inputs[self.dataset_input_key_list[0]])
-            else:
-                datasetFilteret = {
-                    datasetKey: df
-                    for datasetKey, df in inputs.items()
-                    if datasetKey in self.dataset_input_key_list
-                }
-                df = self.process_many(datasetFilteret)
-        elif len(inputs) == 1:
-            df = self.process(next(iter(inputs.values())))
+        # If dataset_input_keys is None, it will be set to all keys in inputs
+        dataset_input_keys = self.dataset_input_keys or list(inputs.keys())
+
+        # Call process or process_many depending on the input_key count
+        if len(dataset_input_keys) == 1:
+            df = self.process(inputs[dataset_input_keys[0]])
         else:
-            df = self.process_many(inputs)
+            inputs_filtered = {
+                datasetKey: df
+                for datasetKey, df in inputs.items()
+                if datasetKey in dataset_input_keys
+            }
+            df = self.process_many(inputs_filtered)
+
+        if self.consume_inputs:
+            for key in dataset_input_keys:
+                inputs.pop(key)
 
+        # dataset_output_key is added to inputs after pop is called
+        # This ensures that dataset_output_key is not popped.
         inputs[self.dataset_output_key] = df
         return inputs
 
-    @abstractmethod
     def process(self, df: DataFrame) -> DataFrame:
         raise NotImplementedError()
 
-    @abstractmethod
     def process_many(self, datasets: dataset_group) -> DataFrame:
         raise NotImplementedError()
```

### Comparing `spetlr-2.1.0/src/spetlr/exceptions/__init__.py` & `spetlr-2.1.5/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-2.1.5/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/filehandle/file_handle.py` & `spetlr-2.1.5/src/spetlr/filehandle/file_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/formatting/git_hooks.py` & `spetlr-2.1.5/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/functions.py` & `spetlr-2.1.5/src/spetlr/functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/mount/main.py` & `spetlr-2.1.5/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-2.1.5/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-2.1.5/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-2.1.5/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-2.1.5/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/reporting/JobReflection.py` & `spetlr-2.1.5/src/spetlr/reporting/JobReflection.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/reporting/SlackNotifier.py` & `spetlr-2.1.5/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/schema_manager/schema_manager.py` & `spetlr-2.1.5/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/schema_manager/spark_schema.py` & `spetlr-2.1.5/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/spark.py` & `spetlr-2.1.5/src/spetlr/spark.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/sql/CommonBaseServer.py` & `spetlr-2.1.5/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/sql/SqlBaseServer.py` & `spetlr-2.1.5/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/sql/SqlExecutor.py` & `spetlr-2.1.5/src/spetlr/sql/SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/sql/SqlServer.py` & `spetlr-2.1.5/src/spetlr/sql/SqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/sql/sql_handle.py` & `spetlr-2.1.5/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/tables/TableHandle.py` & `spetlr-2.1.5/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/testutils/CleanupTestDatabases.py` & `spetlr-2.1.5/src/spetlr/testutils/CleanupTestDatabases.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/testutils/stop_test_streams.py` & `spetlr-2.1.5/src/spetlr/testutils/stop_test_streams.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformations.py` & `spetlr-2.1.5/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/__init__.py` & `spetlr-2.1.5/src/spetlr/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/country_to_alphacode_transformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/country_to_alphacode_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/dropColumnsTransformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/dropColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-2.1.5/src/spetlr/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/fuzzy_select.py` & `spetlr-2.1.5/src/spetlr/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/generate_md5_column_transformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/generate_md5_column_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/join_dataframes_transformer.py` & `spetlr-2.1.5/src/spetlr/transformers/join_dataframes_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List
 
 from pyspark.sql import DataFrame
 
 from spetlr.etl import TransformerNC
 from spetlr.etl.types import dataset_group
 from spetlr.exceptions import (
     ColumnDoesNotExistException,
@@ -34,37 +34,37 @@
     """
 
     def __init__(
         self,
         first_dataframe_join_key: str,
         second_dataframe_join_key: str,
         join_type: str = "inner",
-        dataset_input_keys: Union[str, List[str]] = None,
+        dataset_input_keys: List[str] = None,
         dataset_output_key: str = None,
     ):
+        if len(dataset_input_keys) > 2:
+            raise MoreThanTwoDataFramesException(
+                """More than two DataFrames are specified in 'dataset_input_keys'.
+                This transformer can only join two DataFrames at a time."""
+            )
+
         super().__init__(
             dataset_input_keys=dataset_input_keys, dataset_output_key=dataset_output_key
         )
         self.first_dataframe_join_key = first_dataframe_join_key
         self.second_dataframe_join_key = second_dataframe_join_key
         self.join_type = join_type
 
     def process_many(self, dataset: dataset_group) -> DataFrame:
         """
-        Takes a dictionary of datasets and joins two specified datasets together.
+        Takes a dictionary of datasets and joins two specified dataframes together.
         """
 
-        if len(self.dataset_input_key_list) > 2:
-            raise MoreThanTwoDataFramesException(
-                """More than two DataFrames are specified in 'dataset_input_keys'.
-                This transformer can only join two DataFrames at a time."""
-            )
-
-        first_df = dataset[self.dataset_input_key_list[0]]
-        second_df = dataset[self.dataset_input_key_list[1]]
+        first_df = dataset[self.dataset_input_keys[0]]
+        second_df = dataset[self.dataset_input_keys[1]]
 
         if self.first_dataframe_join_key not in first_df.columns:
             raise ColumnDoesNotExistException(
                 f"""'{self.first_dataframe_join_key}' cannot be found in
                 the first DataFrame."""
             )
```

### Comparing `spetlr-2.1.0/src/spetlr/transformers/selectColumnsTransformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/selectColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/simple_dataframe_filter_transformer.py` & `spetlr-2.1.5/src/spetlr/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/simple_sql_transformer.py` & `spetlr-2.1.5/src/spetlr/transformers/simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/timezone_transformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/union_transformer.py` & `spetlr-2.1.5/src/spetlr/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/union_transformer_nc.py` & `spetlr-2.1.5/src/spetlr/transformers/union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/transformers/validfromto_transformer.py` & `spetlr-2.1.5/src/spetlr/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/CheckDfMerge.py` & `spetlr-2.1.5/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/DataframeCreator.py` & `spetlr-2.1.5/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/DeleteMismatchedSchemas.py` & `spetlr-2.1.5/src/spetlr/utils/DeleteMismatchedSchemas.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-2.1.5/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/GetMergeStatement.py` & `spetlr-2.1.5/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/MockLoader.py` & `spetlr-2.1.5/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-2.1.5/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr/utils/__init__.py` & `spetlr-2.1.5/src/spetlr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/src/spetlr.egg-info/PKG-INFO` & `spetlr-2.1.5/src/spetlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 2.1.0
+Version: 2.1.5
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
@@ -89,14 +89,16 @@
         utilizes Azure Resource deployment - and can only be run by the spetlr-org admins.
         
         To deploy the necessary Azure resources to your own Azure Tenant, run the following command:
         
         ```powershell
         .\.github\deploy\deploy.ps1 -uniqueRunId "yourUniqueId"
         ```
+        Be aware that the applied name for *uniqueRunId* should only contain lower case and numbers, and its length should not
+        exceed 12 characters.
         
         Afterward, execute the following commands:
         
         ```powershell 
         .\.github\submit\build.ps1
         .\.github\submit\submit_test_job.ps1
         ```
```

### Comparing `spetlr-2.1.0/src/spetlr.egg-info/SOURCES.txt` & `spetlr-2.1.5/src/spetlr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 src/spetlr.egg-info/PKG-INFO
 src/spetlr.egg-info/SOURCES.txt
 src/spetlr.egg-info/dependency_links.txt
 src/spetlr.egg-info/entry_points.txt
 src/spetlr.egg-info/not-zip-safe
 src/spetlr.egg-info/requires.txt
 src/spetlr.egg-info/top_level.txt
+src/spetlr/azure_log_analytics/__init__.py
+src/spetlr/azure_log_analytics/azure_log_analytics_handle.py
 src/spetlr/cache/CachedLoader.py
 src/spetlr/cache/CachedLoaderParameters.py
 src/spetlr/cache/__init__.py
 src/spetlr/config_master/__init__.py
 src/spetlr/configurator/__init__.py
 src/spetlr/configurator/configurator.py
 src/spetlr/configurator/_cli/ConfiguratorCli.py
@@ -139,14 +141,15 @@
 src/spetlr/utils/DeleteMismatchedSchemas.py
 src/spetlr/utils/DropOldestDuplicates.py
 src/spetlr/utils/GetMergeStatement.py
 src/spetlr/utils/MockExtractor.py
 src/spetlr/utils/MockLoader.py
 src/spetlr/utils/SelectAndCastColumns.py
 src/spetlr/utils/__init__.py
+tests/cluster/azure_log_analytics/test_azure_log_analytics_handle.py
 tests/cluster/cache/test_cache.py
 tests/cluster/cosmos/test_cosmos.py
 tests/cluster/db/test_db_api.py
 tests/cluster/delta/test_cleanup_databases.py
 tests/cluster/delta/test_delta_class.py
 tests/cluster/delta/test_delta_stream.py
 tests/cluster/delta/test_filehandle.py
@@ -156,16 +159,14 @@
 tests/cluster/eh/test_eh_saving.py
 tests/cluster/etl/test_delete_data_loader.py
 tests/cluster/etl/test_deltaupsert.py
 tests/cluster/etl/test_extractor.py
 tests/cluster/etl/test_incremental_extractor.py
 tests/cluster/etl/test_loader.py
 tests/cluster/etl/test_orchestrator_etl_warning.py
-tests/cluster/etl/test_transformer.py
-tests/cluster/etl/test_transformer_nc.py
 tests/cluster/etl/test_upsertloader.py
 tests/cluster/etl/test_upsertloader_streaming.py
 tests/cluster/reporting/test_slack_reporting.py
 tests/cluster/schema_manager/test_schema_manager.py
 tests/cluster/sql/test_deliveryexecutor.py
 tests/cluster/sql/test_deliverysql.py
 tests/cluster/sql/test_deliverysqlspn.py
@@ -178,24 +179,27 @@
 tests/cluster/utils/test_spark_version.py
 tests/cluster/utils/test_stop_test_stream.py
 tests/local/test_functions.py
 tests/local/test_get_schema.py
 tests/local/test_spark.py
 tests/local/test_sqlServer.py
 tests/local/test_transformations.py
+tests/local/azure_log_analytics/test_azure_log_analytics_handle.py
 tests/local/configurator/test_configurator.py
 tests/local/configurator/test_configurator_cli.py
 tests/local/eh/test_EventHubCaptureExtractor.py
 tests/local/eh/test_ehto_bronze_and_silver.py
 tests/local/eh/test_ehtodeltabronze_orchestrator.py
 tests/local/eh/test_ehtodeltabronze_transformer.py
 tests/local/eh/test_ehtodeltasilver_orchestrator.py
 tests/local/entry_points/test_generalized_entry_points.py
 tests/local/entry_points/test_task_entry_point.py
 tests/local/etl/test_orchestrator.py
+tests/local/etl/test_transformer.py
+tests/local/etl/test_transformer_nc.py
 tests/local/extractors/test_eventhub_stream_extractor.py
 tests/local/reporting/test_slack_reporting.py
 tests/local/schema_manager/test_schema_manager.py
 tests/local/sql/test_SqlExecutor.py
 tests/local/streaming/test_deltahandle_stream.py
 tests/local/streaming/test_filehandle.py
 tests/local/streaming/test_stream_loader.py
```

### Comparing `spetlr-2.1.0/tests/cluster/cache/test_cache.py` & `spetlr-2.1.5/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/cosmos/test_cosmos.py` & `spetlr-2.1.5/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/delta/test_cleanup_databases.py` & `spetlr-2.1.5/tests/cluster/delta/test_cleanup_databases.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/delta/test_delta_class.py` & `spetlr-2.1.5/tests/cluster/delta/test_delta_class.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/delta/test_delta_stream.py` & `spetlr-2.1.5/tests/cluster/delta/test_delta_stream.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/delta/test_filehandle.py` & `spetlr-2.1.5/tests/cluster/delta/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/delta/test_sparkexecutor.py` & `spetlr-2.1.5/tests/cluster/delta/test_sparkexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-2.1.5/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-2.1.5/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/eh/test_eh_saving.py` & `spetlr-2.1.5/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-2.1.5/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_deltaupsert.py` & `spetlr-2.1.5/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_extractor.py` & `spetlr-2.1.5/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-2.1.5/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_loader.py` & `spetlr-2.1.5/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-2.1.5/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_transformer_nc.py` & `spetlr-2.1.5/tests/local/etl/test_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_upsertloader.py` & `spetlr-2.1.5/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/etl/test_upsertloader_streaming.py` & `spetlr-2.1.5/tests/cluster/etl/test_upsertloader_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-2.1.5/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-2.1.5/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-2.1.5/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/sql/test_deliverysql.py` & `spetlr-2.1.5/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-2.1.5/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/sql/test_sql_streaming.py` & `spetlr-2.1.5/tests/cluster/sql/test_sql_streaming.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/sql/test_sqlhandle.py` & `spetlr-2.1.5/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-2.1.5/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/transformations/test_union_transformer.py` & `spetlr-2.1.5/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/utils/test_delete_schema_mismatch.py` & `spetlr-2.1.5/tests/cluster/utils/test_delete_schema_mismatch.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/utils/test_spark_version.py` & `spetlr-2.1.5/tests/cluster/utils/test_spark_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/cluster/utils/test_stop_test_stream.py` & `spetlr-2.1.5/tests/cluster/utils/test_stop_test_stream.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/configurator/test_configurator.py` & `spetlr-2.1.5/tests/local/configurator/test_configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/configurator/test_configurator_cli.py` & `spetlr-2.1.5/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-2.1.5/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-2.1.5/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-2.1.5/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-2.1.5/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-2.1.5/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/entry_points/test_generalized_entry_points.py` & `spetlr-2.1.5/tests/local/entry_points/test_generalized_entry_points.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-2.1.5/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/reporting/test_slack_reporting.py` & `spetlr-2.1.5/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/schema_manager/test_schema_manager.py` & `spetlr-2.1.5/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/sql/test_SqlExecutor.py` & `spetlr-2.1.5/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/streaming/test_filehandle.py` & `spetlr-2.1.5/tests/local/streaming/test_filehandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/streaming/test_stream_loader.py` & `spetlr-2.1.5/tests/local/streaming/test_stream_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/test_functions.py` & `spetlr-2.1.5/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/test_get_schema.py` & `spetlr-2.1.5/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/test_sqlServer.py` & `spetlr-2.1.5/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/test_transformations.py` & `spetlr-2.1.5/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_concat_df.py` & `spetlr-2.1.5/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_country_to_alphacode_transformer.py` & `spetlr-2.1.5/tests/local/transformers/test_country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_drop_columns.py` & `spetlr-2.1.5/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-2.1.5/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_fuzzy_select.py` & `spetlr-2.1.5/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_generate_md5_column_transformer_nc.py` & `spetlr-2.1.5/tests/local/transformers/test_generate_md5_column_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-2.1.5/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py` & `spetlr-2.1.5/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_select_columns.py` & `spetlr-2.1.5/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-2.1.5/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py` & `spetlr-2.1.5/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_timezone_transformer_nc.py` & `spetlr-2.1.5/tests/local/transformers/test_timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_union_transformer.py` & `spetlr-2.1.5/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_union_transformer_nc.py` & `spetlr-2.1.5/tests/local/transformers/test_union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-2.1.5/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/utils/test_dataframe_creation.py` & `spetlr-2.1.5/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-2.1.5/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/utils/test_getmergestatement.py` & `spetlr-2.1.5/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/utils/test_mock_etl.py` & `spetlr-2.1.5/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.1.0/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-2.1.5/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

