# Comparing `tmp/ml-management-0.0.45.tar.gz` & `tmp/ml-management-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.45.tar", last modified: Mon Jul 24 13:22:47 2023, max compression
+gzip compressed data, was "ml-management-0.0.46.tar", last modified: Mon Jul 31 17:14:38 2023, max compression
```

## Comparing `ml-management-0.0.45.tar` & `ml-management-0.0.46.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.699371 ml-management-0.0.45/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-06-05 10:13:00.000000 ml-management-0.0.45/MANIFEST.in
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/collectors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/collectors.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/collectors/dummy/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/collectors/s3/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9711 2023-07-10 10:57:45.000000 ml-management-0.0.45/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/collectors/topic_markers/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/dataset_loader_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4373 2023-07-20 08:04:45.000000 ml-management-0.0.45/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/executor_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/executor_template/default_executors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     6505 2023-07-20 08:04:45.000000 ml-management-0.0.45/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/mlmanagement/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      737 2023-07-03 06:55:20.000000 ml-management-0.0.45/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2639 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/mlmanagement/abstract_mlflow_client.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      380 2023-07-21 09:09:18.000000 ml-management-0.0.45/ML_management/mlmanagement/base_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    17348 2023-07-24 13:11:16.000000 ml-management-0.0.45/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10107 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2701 2023-07-20 08:04:45.000000 ml-management-0.0.45/ML_management/mlmanagement/module_finder.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5121 2023-07-21 09:09:18.000000 ml-management-0.0.45/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      371 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/mlmanagement/singleton_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      269 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.695371 ml-management-0.0.45/ML_management/models/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/models/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.699371 ml-management-0.0.45/ML_management/models/patterns/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4865 2023-07-20 08:04:45.000000 ml-management-0.0.45/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.699371 ml-management-0.0.45/ML_management/registry/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/registry/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3362 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/registry/abstract_registry_manager.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2765 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/registry/exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4264 2023-07-24 12:28:43.000000 ml-management-0.0.45/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.699371 ml-management-0.0.45/ML_management/tests/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/tests/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9858 2023-07-10 10:57:45.000000 ml-management-0.0.45/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.699371 ml-management-0.0.45/ML_management/uploader_data/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.45/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1914 2023-07-10 10:57:45.000000 ml-management-0.0.45/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1430 2023-07-10 10:57:45.000000 ml-management-0.0.45/ML_management/uploader_data/utils.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      367 2023-07-24 13:22:47.699371 ml-management-0.0.45/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-06-05 10:13:00.000000 ml-management-0.0.45/README.md
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        7 2023-07-24 13:06:09.000000 ml-management-0.0.45/VERSION
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-24 13:22:47.699371 ml-management-0.0.45/ml_management.egg-info/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      367 2023-07-24 13:22:47.000000 ml-management-0.0.45/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2729 2023-07-24 13:22:47.000000 ml-management-0.0.45/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-07-24 13:22:47.000000 ml-management-0.0.45/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      166 2023-07-24 13:22:47.000000 ml-management-0.0.45/ml_management.egg-info/requires.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-07-24 13:22:47.000000 ml-management-0.0.45/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-07-24 13:22:47.699371 ml-management-0.0.45/setup.cfg
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1076 2023-07-10 10:57:45.000000 ml-management-0.0.45/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.083144 ml-management-0.0.46/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       18 2023-07-06 14:54:04.000000 ml-management-0.0.46/MANIFEST.in
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.075144 ml-management-0.0.46/ML_management/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/__init__.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.075144 ml-management-0.0.46/ML_management/collectors/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      120 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1092 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      456 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1318 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/collectors.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.075144 ml-management-0.0.46/ML_management/collectors/dummy/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      463 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.075144 ml-management-0.0.46/ML_management/collectors/s3/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     9711 2023-07-14 16:19:07.000000 ml-management-0.0.46/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)   331440 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3167 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/dataset_loader_template/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     4373 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      457 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/executor_template/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      895 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      843 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      869 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     6505 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      402 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/mlmanagement/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      737 2023-07-14 16:19:07.000000 ml-management-0.0.46/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2639 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/mlmanagement/abstract_mlflow_client.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      380 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/mlmanagement/base_exceptions.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3392 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     5054 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    16951 2023-07-28 11:54:07.000000 ml-management-0.0.46/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    10107 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      201 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2701 2023-07-28 11:54:30.000000 ml-management-0.0.46/ML_management/mlmanagement/module_finder.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     5121 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      371 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/mlmanagement/singleton_pattern.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      269 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/models/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/models/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      949 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/models/patterns/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     4865 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      561 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      445 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      457 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.079144 ml-management-0.0.46/ML_management/registry/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/registry/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3362 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/registry/abstract_registry_manager.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2765 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/registry/exceptions.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     4264 2023-07-25 09:00:09.000000 ml-management-0.0.46/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.083144 ml-management-0.0.46/ML_management/tests/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/tests/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3361 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     9858 2023-07-14 16:19:07.000000 ml-management-0.0.46/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.083144 ml-management-0.0.46/ML_management/uploader_data/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-07-06 14:54:04.000000 ml-management-0.0.46/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1914 2023-07-14 16:19:07.000000 ml-management-0.0.46/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1430 2023-07-14 16:19:07.000000 ml-management-0.0.46/ML_management/uploader_data/utils.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      394 2023-07-31 17:14:38.083144 ml-management-0.0.46/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       56 2023-07-06 14:54:04.000000 ml-management-0.0.46/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        7 2023-07-31 17:13:22.000000 ml-management-0.0.46/VERSION
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-07-31 17:14:38.083144 ml-management-0.0.46/ml_management.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      394 2023-07-31 17:14:37.000000 ml-management-0.0.46/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2729 2023-07-31 17:14:37.000000 ml-management-0.0.46/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-07-31 17:14:37.000000 ml-management-0.0.46/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      166 2023-07-31 17:14:37.000000 ml-management-0.0.46/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       14 2023-07-31 17:14:37.000000 ml-management-0.0.46/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-07-31 17:14:38.083144 ml-management-0.0.46/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1076 2023-07-14 16:19:07.000000 ml-management-0.0.46/setup.py
```

### Comparing `ml-management-0.0.45/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.46/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/collectors/collectors.py` & `ml-management-0.0.46/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.46/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.46/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.46/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.46/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.46/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.46/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.46/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.46/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.46/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/abstract_mlflow_client.py` & `ml-management-0.0.46/ML_management/mlmanagement/abstract_mlflow_client.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.46/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.46/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.46/ML_management/mlmanagement/mlmanagement.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,130 +65,131 @@
 
 def get_experiment_by_name(name: str) -> Optional[Experiment]:
     """Retrieve an experiment by experiment name from the backend store."""
     return request_for_function(inspect.currentframe())
 
 
 def search_runs(
-        experiment_ids: Optional[List[str]] = None,
-        filter_string: str = "",
-        run_view_type: int = 1,
-        max_results: int = 100000,
-        order_by: Optional[List[str]] = None,
-        output_format: str = "pandas",
-        search_all_experiments: bool = False,
-        experiment_names: Optional[List[str]] = None,
+    experiment_ids: Optional[List[str]] = None,
+    filter_string: str = "",
+    run_view_type: int = 1,
+    max_results: int = 100000,
+    order_by: Optional[List[str]] = None,
+    output_format: str = "pandas",
+    search_all_experiments: bool = False,
+    experiment_names: Optional[List[str]] = None,
 ) -> Union[List[Run], "pandas.DataFrame"]:
     """Search experiments that fit the search criteria."""
     return request_for_function(inspect.currentframe())
 
 
 def start_run(
-        run_id: Optional[str] = None,
-        experiment_id: Optional[str] = None,
-        run_name: Optional[str] = None,
-        nested: bool = False,
-        tags: Optional[Dict[str, Any]] = None,
-        description: Optional[str] = None,
+    run_id: Optional[str] = None,
+    experiment_id: Optional[str] = None,
+    run_name: Optional[str] = None,
+    nested: bool = False,
+    tags: Optional[Dict[str, Any]] = None,
+    description: Optional[str] = None,
 ) -> ActiveRun:
     """
     Start a new MLflow run, setting it as the active run under which metrics and parameters will be logged.
 
     The return value can be used as a context manager within a with block; otherwise, you must call end_run() to
     terminate the current run.
     If you pass a run_id or the MLFLOW_RUN_ID environment variable is set, start_run attempts to resume a run with
     the specified run ID and other parameters are ignored. run_id takes precedence over MLFLOW_RUN_ID.
     If resuming an existing run, the run status is set to RunStatus.RUNNING.
     Add that created run to active_run_stack.
     """
     if len(active_run_stack) > 0 and not nested:
         raise Exception(
             (
-                    "Run with UUID {} is already active. To start a new run, first end the "
-                    + "current run with mlmanagement.end_run(). To start a nested "
-                    + "run, call start_run with nested=True"
+                "Run with UUID {} is already active. To start a new run, first end the "
+                + "current run with mlmanagement.end_run(). To start a nested "
+                + "run, call start_run with nested=True"
             ).format(active_run_stack[0].info.run_id)
         )
     _active_run = request_for_function(inspect.currentframe())
     active_run_stack.append(_active_run)
     return _active_run
 
 
 def _add_job_registration_metainfo(
-        registration_timestamp,
-        init_model_version_run_id,
-        dataset_loader_version_run_id,
-        executor_version_run_id,
-        name,
-        job_executor_name,
-        job_executor_version,
-        dataset_loader_name,
-        dataset_loader_version,
-        model_name,
-        model_version,
-        new_model_name,
-        experiment_name,
-        periodic_type,
-        cron_expression,
-        metric_name,
-        optimal_min,
-        choice_criteria,
-        executor_model_params_json,
-        data_params_json,
-        collector_name,
+    registration_timestamp,
+    init_model_version_run_id,
+    dataset_loader_version_run_id,
+    executor_version_run_id,
+    name,
+    job_executor_name,
+    job_executor_version,
+    dataset_loader_name,
+    dataset_loader_version,
+    model_name,
+    model_version,
+    new_model_name,
+    experiment_name,
+    periodic_type,
+    cron_expression,
+    metric_name,
+    optimal_min,
+    choice_criteria,
+    executor_model_params_json,
+    data_params_json,
+    collector_name,
+    gpu,
 ):
     """Add job metainfo on job registration. For internal use only."""
     return request_for_function(inspect.currentframe())
 
 
 def _add_job_start_metainfo(
-        job_name,
-        start_timestamp,
+    job_name,
+    start_timestamp,
 ):
     """Add job metainfo on execution start. For internal use only."""
     return request_for_function(inspect.currentframe())
 
 
 def _add_job_end_metainfo(
-        job_name,
-        end_timestamp,
+    job_name,
+    end_timestamp,
 ):
     """Add job metainfo on execution end. For internal use only."""
     return request_for_function(inspect.currentframe())
 
 
 def _add_job_fail_metainfo(
-        job_name,
-        end_timestamp,
+    job_name,
+    end_timestamp,
 ):
     """Add job metainfo on execution fail. For internal use only."""
     return request_for_function(inspect.currentframe())
 
 
 def log_model(
-        artifact_path,
-        loader_module=None,
-        data_path=None,
-        code_path=None,
-        conda_env=None,
-        python_model=None,
-        artifacts=None,
-        registered_model_name="default_name",
-        signature: mlflow.models.signature.ModelSignature = None,
-        input_example: Union[pandas.core.frame.DataFrame, numpy.ndarray, dict, list, csr_matrix, csc_matrix, str, bytes] = None,
-        await_registration_for=300,
-        pip_requirements=None,
-        extra_pip_requirements=None,
-        metadata=None,
-        source_model_name=None,
-        source_model_version=None,
-        upload_model_mode=None,
-        extra_modules_names=None,
-        used_modules_names=None,
-        root_module_name: str = "__main__",
+    artifact_path,
+    loader_module=None,
+    data_path=None,
+    code_path=None,
+    conda_env=None,
+    python_model=None,
+    artifacts=None,
+    registered_model_name="default_name",
+    signature: mlflow.models.signature.ModelSignature = None,
+    input_example: Union[pandas.core.frame.DataFrame, numpy.ndarray, dict, list, csr_matrix, csc_matrix, str, bytes] = None,
+    await_registration_for=300,
+    pip_requirements=None,
+    extra_pip_requirements=None,
+    metadata=None,
+    source_model_name=None,
+    source_model_version=None,
+    upload_model_mode=None,
+    extra_modules_names=None,
+    used_modules_names=None,
+    root_module_name: str = "__main__",
 ):
     """
     Log a Pyfunc model with custom inference logic and optional data dependencies as an MLflow artifact.
 
     Current run is using.
     You cannot specify the parameters: loader_module, data_path and the parameters: python_model, artifacts together.
     """
@@ -263,23 +264,23 @@
 def set_tag(key: str, value: Any) -> None:
     """Set a tag under the current run. If no run is active, this method will create a new active run."""
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
 
 
 def autolog(
-        log_every_n_epoch=1,
-        log_every_n_step=None,
-        log_models=True,
-        log_datasets=True,
-        disable=False,
-        exclusive=False,
-        disable_for_unsupported_versions=False,
-        silent=False,
-        registered_model_name=None,
+    log_every_n_epoch=1,
+    log_every_n_step=None,
+    log_models=True,
+    log_datasets=True,
+    disable=False,
+    exclusive=False,
+    disable_for_unsupported_versions=False,
+    silent=False,
+    registered_model_name=None,
 ) -> None:
     """
     Enable (or disable) and configure autologging for all supported integrations.
 
     The parameters are passed to any autologging integrations that support them.
     """
     start_run_if_not_exist()
@@ -291,16 +292,15 @@
     return request_for_function(inspect.currentframe(), ["pyfunc"])
 
 
 default_model = Model()
 
 
 def save_model(
-        path, loader_module=None, data_path=None, code_path=None, conda_env=None, mlflow_model=default_model, python_model=None,
-        artifacts=None
+    path, loader_module=None, data_path=None, code_path=None, conda_env=None, mlflow_model=default_model, python_model=None, artifacts=None
 ):
     """
     Save a Pyfunc model with custom inference logic and optional data dependencies to a path on the local filesystem.
 
     You cannot specify the parameters: loader_module, data_path and the parameters: python_model, artifacts together.
     """
     return request_for_function(inspect.currentframe(), ["pyfunc"])
@@ -340,44 +340,38 @@
 
 
 class MlflowClient(AbstractMlflowClient):
     """Initialize an MLflow Client."""
 
     def __init__(self):
         self.extra_attrs = ["tracking"]
-        self.for_class = {
-            "class_name": self.__class__.__name__,
-            "class_kwargs": {}
-        }
+        self.for_class = {"class_name": self.__class__.__name__, "class_kwargs": {}}
 
     def set_model_version_tag(
-            self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None,
-            stage: Optional[str] = None
+        self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None, stage: Optional[str] = None
     ) -> None:
         """Set model version tag."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
 
     def set_dataset_loader_version_tag(
-            self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None,
-            stage: Optional[str] = None
+        self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None, stage: Optional[str] = None
     ) -> None:
         """Set dataset loader version tag."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
 
     def set_executor_version_tag(
-            self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None,
-            stage: Optional[str] = None
+        self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None, stage: Optional[str] = None
     ) -> None:
         """Set executor version tag."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
@@ -413,19 +407,19 @@
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
 
     # TODO after updating to a new version, the result is paginated
     # and needs to be converted to pagination scheme of our project.
     def search_model_versions(
-            self,
-            filter_string: Optional[str] = None,
-            max_results: int = 10000,
-            order_by: Optional[List[str]] = None,
-            page_token: Optional[str] = None,
+        self,
+        filter_string: Optional[str] = None,
+        max_results: int = 10000,
+        order_by: Optional[List[str]] = None,
+        page_token: Optional[str] = None,
     ) -> PagedList[ModelVersion]:
         """Search for model versions in backend that satisfy the filter criteria."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
```

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.46/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/module_finder.py` & `ml-management-0.0.46/ML_management/mlmanagement/module_finder.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.46/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.46/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.46/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.46/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/registry/abstract_registry_manager.py` & `ml-management-0.0.46/ML_management/registry/abstract_registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/registry/exceptions.py` & `ml-management-0.0.46/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/registry/registry_manager.py` & `ml-management-0.0.46/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.46/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.46/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.46/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ML_management/uploader_data/utils.py` & `ml-management-0.0.46/ML_management/uploader_data/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.46/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.45/setup.py` & `ml-management-0.0.46/setup.py`

 * *Files identical despite different names*

