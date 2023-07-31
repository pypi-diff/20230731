# Comparing `tmp/dagshub-0.3.1.post1.tar.gz` & `tmp/dagshub-0.3.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.1.post1.tar", last modified: Sun Jul 30 14:28:08 2023, max compression
+gzip compressed data, was "dagshub-0.3.1.post2.tar", last modified: Mon Jul 31 10:34:25 2023, max compression
```

## Comparing `dagshub-0.3.1.post1.tar` & `dagshub-0.3.1.post2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.662541 dagshub-0.3.1.post1/dagshub/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.662541 dagshub-0.3.1.post1/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.666541 dagshub-0.3.1.post1/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/datasources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/model/query_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.662541 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   222423 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.670541 dagshub-0.3.1.post1/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40226 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.662541 dagshub-0.3.1.post1/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-30 14:28:08.000000 dagshub-0.3.1.post1/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-30 14:28:08.000000 dagshub-0.3.1.post1/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:28:08.000000 dagshub-0.3.1.post1/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 14:28:08.000000 dagshub-0.3.1.post1/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-30 14:28:08.000000 dagshub-0.3.1.post1/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 14:28:08.000000 dagshub-0.3.1.post1/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:28:08.674541 dagshub-0.3.1.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-30 14:27:58.000000 dagshub-0.3.1.post1/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.140602 dagshub-0.3.1.post2/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.144602 dagshub-0.3.1.post2/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.144602 dagshub-0.3.1.post2/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.144602 dagshub-0.3.1.post2/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.144602 dagshub-0.3.1.post2/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.144602 dagshub-0.3.1.post2/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.144602 dagshub-0.3.1.post2/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/datasources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/model/query_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.140602 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   222423 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.148602 dagshub-0.3.1.post2/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40226 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26699 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.140602 dagshub-0.3.1.post2/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-31 10:34:25.000000 dagshub-0.3.1.post2/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-31 10:34:25.000000 dagshub-0.3.1.post2/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:34:25.000000 dagshub-0.3.1.post2/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 10:34:25.000000 dagshub-0.3.1.post2/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 10:34:25.000000 dagshub-0.3.1.post2/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 10:34:25.000000 dagshub-0.3.1.post2/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:34:25.152602 dagshub-0.3.1.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 10:34:15.000000 dagshub-0.3.1.post2/tests/test_misc.py
```

### Comparing `dagshub-0.3.1.post1/LICENSE` & `dagshub-0.3.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/PKG-INFO` & `dagshub-0.3.1.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.1.post1
+Version: 0.3.1.post2
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.1.post1 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.1.post2 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
```

### Comparing `dagshub-0.3.1.post1/README.md` & `dagshub-0.3.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/auth/oauth.py` & `dagshub-0.3.1.post2/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/auth/token_auth.py` & `dagshub-0.3.1.post2/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/auth/tokens.py` & `dagshub-0.3.1.post2/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/analytics.py` & `dagshub-0.3.1.post2/dagshub/common/analytics.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/api/repo.py` & `dagshub-0.3.1.post2/dagshub/common/api/repo.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/api/responses.py` & `dagshub-0.3.1.post2/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/cli.py` & `dagshub-0.3.1.post2/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/config.py` & `dagshub-0.3.1.post2/dagshub/common/config.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/download.py` & `dagshub-0.3.1.post2/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/helpers.py` & `dagshub-0.3.1.post2/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/init.py` & `dagshub-0.3.1.post2/dagshub/common/init.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/logging_util.py` & `dagshub-0.3.1.post2/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/common/util.py` & `dagshub-0.3.1.post2/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.1.post2/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/data_client.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/base.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/models.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.1.post2/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/datasets.py` & `dagshub-0.3.1.post2/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/datasources.py` & `dagshub-0.3.1.post2/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.1.post2/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.1.post2/dagshub/data_engine/model/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.1.post2/dagshub/data_engine/model/datasource_state.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/model/errors.py` & `dagshub-0.3.1.post2/dagshub/data_engine/model/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/model/query.py` & `dagshub-0.3.1.post2/dagshub/data_engine/model/query.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.1.post2/dagshub/data_engine/model/query_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
                     if k in annotation_fields:
                         continue
                     if type(v) is not bytes:
                         sample[k] = v
                 samples.append(sample)
                 progress.update(task, advance=1, refresh=True)
 
-        ds.add_samples(samples)
+        ds.merge_samples(samples)
         return ds
 
     def _check_downloaded_dataset_size(self):
         download_size_prompt_threshold = 100 * (2 ** 20)  # 100 Megabytes
         dp_size = self._calculate_datapoint_size()
         if dp_size is not None and dp_size > download_size_prompt_threshold:
             prompt = f"You're about to download {sizeof_fmt(dp_size)} of images locally."
```

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.1.post2/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/fastai/logger.py` & `dagshub-0.3.1.post2/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/keras/logger.py` & `dagshub-0.3.1.post2/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/logger.py` & `dagshub-0.3.1.post2/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/notebook.py` & `dagshub-0.3.1.post2/dagshub/notebook.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.1.post2/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/streaming/dataclasses.py` & `dagshub-0.3.1.post2/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/streaming/filesystem.py` & `dagshub-0.3.1.post2/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/streaming/mount.py` & `dagshub-0.3.1.post2/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/upload/errors.py` & `dagshub-0.3.1.post2/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/dagshub/upload/wrapper.py` & `dagshub-0.3.1.post2/dagshub/upload/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
         self._api = RepoAPI(f"{owner}/{name}", host=self.host, auth=self.auth)
 
         # For mirror uploading: store the last revision for which we uploaded
         # When the last revision changes, that means the sync has been complete and we can upload a new batch
         self._last_upload_revision: Optional[str] = None
         self._last_upload_had_changes: bool = False
 
+        self.current_progress: Optional[rich.progress.Progress] = None
+
         if self.branch is None:
             logger.debug("Branch wasn't provided. Fetching default branch...")
             self.branch = self._api.default_branch
         logger.debug(f"Set branch: {self.branch}")
 
     def upload(
         self,
@@ -275,14 +277,17 @@
             new_branch: Create a new branch with the name of the passed argument
             last_commit: Consistency argument - last revision of the files you want to upgrade.
                 Exists to prevent accidental overwrites
             force (bool): Force the upload of a file even if it is already present on the server.
                 Sets last_commit to be the tip of the branch
         """
 
+        # Truncate the commit message because the max we allow is 100 symbols
+        commit_message = commit_message[:100]
+
         data = {
             "commit_choice": "direct",
             "commit_summary": commit_message,
             "versioning": versioning,
             "last_commit": last_commit,
             "is_dvc_dir": directory_path != "" and versioning != "git",
         }
@@ -370,21 +375,35 @@
         if self._last_upload_revision is None or not self._last_upload_had_changes:
             return
 
         poll_interval = 1.0  # seconds
         poll_timeout = 600.0
         start_time = time.time()
 
-        with rich.status.Status("Waiting for the mirror to sync", console=rich_console):
-            while time.time() - start_time < poll_timeout:
-                new_revision = self._api.last_commit_sha(self.branch)
-                if new_revision == self._last_upload_revision:
-                    time.sleep(poll_interval)
-                else:
-                    return
+        if self.current_progress is not None:
+            task = self.current_progress.add_task("Waiting for the mirror to sync", total=None)
+
+            def finish():
+                self.current_progress.remove_task(task)
+        else:
+            status = rich.status.Status("Waiting for the mirror to sync", console=rich_console)
+            status.start()
+
+            def finish():
+                status.stop()
+
+        while time.time() - start_time < poll_timeout:
+            new_revision = self._api.last_commit_sha(self.branch)
+            if new_revision == self._last_upload_revision:
+                time.sleep(poll_interval)
+            else:
+                finish()
+                return
+
+        finish()
         logger.warning(f"Timed out while polling for a mirror sync finishing after {poll_timeout} s. "
                        f"Trying to push anyway, which might not work.")
 
     @property
     def auth(self):
         """
         The auth function is used to authenticate the user with the dagshub API.
@@ -498,58 +517,63 @@
         :return: None
 
         """
         upload_file_number = 100
         file_counter = 0
 
         progress = rich.progress.Progress(rich.progress.SpinnerColumn(), *rich.progress.Progress.get_default_columns(),
+                                          rich.progress.MofNCompleteColumn(),
                                           console=rich_console, transient=True, disable=config.quiet)
-        total_task = progress.add_task("Uploading files...")
+        total_task = progress.add_task("Uploading files...", total=None)
+        self.repo.current_progress = progress
 
         # If user hasn't specified versioning, then assume we're uploading dvc (this makes most sense for folders)
         if "versioning" not in upload_kwargs:
             upload_kwargs["versioning"] = "dvc"
 
-        with progress:
-            for root, dirs, files in os.walk(local_path):
-                folder_task = progress.add_task(f"Uploading files from {root}", total=len(files))
-
-                if commit_message is None:
-                    commit_message = upload_kwargs.get("commit_message", f"Commit data points in folder {root}")
-                if "commit_message" in upload_kwargs:
-                    del upload_kwargs["commit_message"]
-
-                if len(files) > 0:
-                    for filename in files:
-                        rel_file_path = posixpath.join(root, filename)
-                        rel_remote_file_path = rel_file_path.replace(local_path, "")
-                        if (
-                            glob_exclude == ""
-                            or fnmatch.fnmatch(rel_file_path, glob_exclude) is False
-                        ):
-                            self.add(file=rel_file_path, path=rel_remote_file_path)
-                            if len(self.files) >= upload_file_number:
-                                file_counter += len(self.files)
-                                self.commit(commit_message, **upload_kwargs)
-                                progress.update(folder_task, advance=len(self.files), refresh=True)
-                                progress.update(total_task, completed=file_counter, refresh=True)
-                    if len(self.files) >= upload_file_number:
-                        file_counter += len(self.files)
-                        self.commit(commit_message, **upload_kwargs)
-                        progress.update(folder_task, advance=len(self.files), refresh=True)
-                        progress.update(total_task, completed=file_counter, refresh=True)
-                progress.remove_task(folder_task)
-
-            if len(self.files) > 0:
-                file_counter += len(self.files)
-                self.commit(commit_message, **upload_kwargs)
-                progress.update(total_task, completed=file_counter)
-
-        log_message(f"Directory upload complete, uploaded {file_counter} files"
-                    f" to {self.repo.get_files_ui_url(self.directory)}", logger)
+        try:
+            with progress:
+                for root, dirs, files in os.walk(local_path):
+                    folder_task = progress.add_task(f"Uploading files from {root}", total=len(files))
+
+                    if commit_message is None:
+                        commit_message = upload_kwargs.get("commit_message", f"Commit data points in folder {root}")
+                    if "commit_message" in upload_kwargs:
+                        del upload_kwargs["commit_message"]
+
+                    if len(files) > 0:
+                        for filename in files:
+                            rel_file_path = posixpath.join(root, filename)
+                            rel_remote_file_path = rel_file_path.replace(local_path, "")
+                            if (
+                                glob_exclude == ""
+                                or fnmatch.fnmatch(rel_file_path, glob_exclude) is False
+                            ):
+                                self.add(file=rel_file_path, path=rel_remote_file_path)
+                                if len(self.files) >= upload_file_number:
+                                    file_counter += len(self.files)
+                                    self.commit(commit_message, **upload_kwargs)
+                                    progress.update(folder_task, advance=len(self.files), refresh=True)
+                                    progress.update(total_task, completed=file_counter, refresh=True)
+                        if len(self.files) >= upload_file_number:
+                            file_counter += len(self.files)
+                            self.commit(commit_message, **upload_kwargs)
+                            progress.update(folder_task, advance=len(self.files), refresh=True)
+                            progress.update(total_task, completed=file_counter, refresh=True)
+                    progress.remove_task(folder_task)
+
+                if len(self.files) > 0:
+                    file_counter += len(self.files)
+                    self.commit(commit_message, **upload_kwargs)
+                    progress.update(total_task, completed=file_counter)
+
+            log_message(f"Directory upload complete, uploaded {file_counter} files"
+                        f" to {self.repo.get_files_ui_url(self.directory)}", logger)
+        finally:
+            self.repo.current_progress = None
 
     @staticmethod
     def _clean_directory_name(directory: str):
         """
         The _clean_directory_name function takes a directory name as an argument
         and returns the normalized path of that directory.
         For example, if the input is ../../../ then it will return /. If the input is ./ then it will return ..
```

### Comparing `dagshub-0.3.1.post1/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.1.post2/dagshub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.1.post1
+Version: 0.3.1.post2
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.1.post1 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.1.post2 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
```

### Comparing `dagshub-0.3.1.post1/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.1.post2/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/setup.py` & `dagshub-0.3.1.post2/setup.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/tests/test_dagshub_logger.py` & `dagshub-0.3.1.post2/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.1.post1/tests/test_misc.py` & `dagshub-0.3.1.post2/tests/test_misc.py`

 * *Files identical despite different names*

