# Comparing `tmp/mmengine-0.8.2.tar.gz` & `tmp/mmengine-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.8.2.tar", last modified: Wed Jul 12 03:01:45 2023, max compression
+gzip compressed data, was "dist/mmengine-0.8.3.tar", last modified: Mon Jul 31 09:23:23 2023, max compression
```

## Comparing `mmengine-0.8.2.tar` & `mmengine-0.8.3.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 03:00:23.000000 mmengine-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-12 03:01:45.000000 mmengine-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-07-12 03:00:23.000000 mmengine-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/_strategy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72405 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/_flexible_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)   101587 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-07-12 03:00:23.000000 mmengine-0.8.2/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 03:01:45.000000 mmengine-0.8.2/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-12 03:01:45.000000 mmengine-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-12 03:00:23.000000 mmengine-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 09:20:06.000000 mmengine-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-31 09:23:23.000000 mmengine-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-31 09:20:06.000000 mmengine-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26838 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73964 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29994 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/efficient_conv_bn_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102028 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53635 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-31 09:23:23.000000 mmengine-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-31 09:20:06.000000 mmengine-0.8.3/setup.py
```

### Comparing `mmengine-0.8.2/PKG-INFO` & `mmengine-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.2
+Version: 0.8.3
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -62,33 +62,49 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.8.0 was released on 2023-06-30.
+        v0.8.3 was released on 2023-07-31.
         
         Highlights:
         
+        - Support enabling `efficient_conv_bn_eval` for efficient convolution and batch normalization. See [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#save-memory-on-gpu) for more details
+        
+        - Add an [example](./examples/llama2/) to finetune Llama2.
+        
         - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for more detailed usages.
         
         - Introduce the pure Python style configuration file:
         
           - Support navigating to base configuration file in IDE
           - Support navigating to base variable in IDE
           - Support navigating to source code of class in IDE
           - Support inheriting two configuration files containing the same field
           - Load the configuration file without other third-party requirements
         
           Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
         
           ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
         
-        Read [Changelog](./docs/en/notes/changelog.md#v080-06302023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v083-07312023) for more details.
+        
+        ## Table of Contents
+        
+        - [Introduction](#introduction)
+        - [Installation](#installation)
+        - [Get Started](#get-started)
+        - [Learn More](#learn-more)
+        - [Contributing](#contributing)
+        - [Citation](#citation)
+        - [License](#license)
+        - [Ecosystem](#ecosystem)
+        - [Projects in OpenMMLab](#projects-in-openmmlab)
         
         ## Introduction
         
         MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
         
         Major features:
         
@@ -104,14 +120,16 @@
         
         3. **Customizable training process**:
         
            - Defines the training process just like playing with Legos.
            - Provides rich components and strategies.
            - Complete controls on the training process with different levels of APIs.
         
+        ![mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/267db9cb-72e4-4af2-a58b-877b30091acc)
+        
         ## Installation
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
         
         ```bash
@@ -344,14 +362,18 @@
         }
         ```
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE).
         
+        ## Ecosystem
+        
+        - [APES: Attention-based Point Cloud Edge Sampling](https://github.com/JunweiZheng93/APES)
+        
         ## Projects in OpenMMLab
         
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
         - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
         - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.2 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.3 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
@@ -17,62 +17,71 @@
    badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
 mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
      ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## What's New v0.8.0 was released on 2023-06-30. Highlights: - Support training
-with [FSDP](https://pytorch.org/tutorials/intermediate/
-FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://
-www.deepspeed.ai/). Refer to the [Training Large Models](https://
-mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for
-more detailed usages. - Introduce the pure Python style configuration file: -
-Support navigating to base configuration file in IDE - Support navigating to
-base variable in IDE - Support navigating to source code of class in IDE -
-Support inheriting two configuration files containing the same field - Load the
-configuration file without other third-party requirements Refer to the
-[tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/
-config.html#a-pure-python-style-configuration-file-beta) for more detailed
-usages. ![new-config-en](https://github.com/open-mmlab/mmengine/assets/
-57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1) Read [Changelog](./docs/en/
-notes/changelog.md#v080-06302023) for more details. ## Introduction MMEngine is
-a foundational library for training deep learning models based on PyTorch. It
-provides a solid engineering foundation and frees developers from writing
-redundant codes on workflows. It serves as the training engine of all OpenMMLab
-codebases, which support hundreds of algorithms in various research areas.
-Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
-Major features: 1. **A universal and powerful runner**: - Supports training
-different tasks with a small amount of code, e.g., ImageNet can be trained with
-only 80 lines of code (400 lines of the original PyTorch example). - Easily
-compatible with models from popular algorithm libraries such as TIMM,
+## What's New v0.8.3 was released on 2023-07-31. Highlights: - Support enabling
+`efficient_conv_bn_eval` for efficient convolution and batch normalization. See
+[save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/
+save_gpu_memory.html#save-memory-on-gpu) for more details - Add an [example](./
+examples/llama2/) to finetune Llama2. - Support training with [FSDP](https://
+pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp)
+and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large
+Models](https://mmengine.readthedocs.io/en/latest/common_usage/
+large_model_training.html) for more detailed usages. - Introduce the pure
+Python style configuration file: - Support navigating to base configuration
+file in IDE - Support navigating to base variable in IDE - Support navigating
+to source code of class in IDE - Support inheriting two configuration files
+containing the same field - Load the configuration file without other third-
+party requirements Refer to the [tutorial](https://mmengine.readthedocs.io/en/
+latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
+beta) for more detailed usages. ![new-config-en](https://github.com/open-mmlab/
+mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1) Read [Changelog]
+(./docs/en/notes/changelog.md#v083-07312023) for more details. ## Table of
+Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
+Started](#get-started) - [Learn More](#learn-more) - [Contributing]
+(#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
+(#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
+MMEngine is a foundational library for training deep learning models based on
+PyTorch. It provides a solid engineering foundation and frees developers from
+writing redundant codes on workflows. It serves as the training engine of all
+OpenMMLab codebases, which support hundreds of algorithms in various research
+areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab
+projects. Major features: 1. **A universal and powerful runner**: - Supports
+training different tasks with a small amount of code, e.g., ImageNet can be
+trained with only 80 lines of code (400 lines of the original PyTorch example).
+- Easily compatible with models from popular algorithm libraries such as TIMM,
 TorchVision, and Detectron2. 2. **Open architecture with unified interfaces**:
 - Handles different algorithm tasks with unified APIs, e.g., implement a method
 and apply it to all compatible models. - Provides a unified abstraction for
 upper-level algorithm libraries, which supports various back-end devices such
 as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training. 3.
 **Customizable training process**: - Defines the training process just like
 playing with Legos. - Provides rich components and strategies. - Complete
-controls on the training process with different levels of APIs. ## Installation
-Before installing MMEngine, please ensure that PyTorch has been successfully
-installed following the [official guide](https://pytorch.org/get-started/
-locally/). Install MMEngine ```bash pip install -U openmim mim install mmengine
-``` Verify the installation ```bash python -c 'from mmengine.utils.dl_utils
-import collect_env;print(collect_env())' ``` ## Get Started Taking the training
-of a ResNet-50 model on the CIFAR-10 dataset as an example, we will use
-MMEngine to build a complete, configurable training and validation process in
-less than 80 lines of code.  Build Models First, we need to define a **model**
-which 1) inherits from `BaseModel` and 2) accepts an additional argument `mode`
-in the `forward` method, in addition to those arguments related to the dataset.
-- During training, the value of `mode` is "loss", and the `forward` method
-should return a `dict` containing the key "loss". - During validation, the
-value of `mode` is "predict", and the forward method should return results
-containing both predictions and labels. ```python import torch.nn.functional as
-F import torchvision from mmengine.model import BaseModel class MMResNet50
-(BaseModel): def __init__(self): super().__init__() self.resnet =
+controls on the training process with different levels of APIs. !
+[mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/
+267db9cb-72e4-4af2-a58b-877b30091acc) ## Installation Before installing
+MMEngine, please ensure that PyTorch has been successfully installed following
+the [official guide](https://pytorch.org/get-started/locally/). Install
+MMEngine ```bash pip install -U openmim mim install mmengine ``` Verify the
+installation ```bash python -c 'from mmengine.utils.dl_utils import
+collect_env;print(collect_env())' ``` ## Get Started Taking the training of a
+ResNet-50 model on the CIFAR-10 dataset as an example, we will use MMEngine to
+build a complete, configurable training and validation process in less than 80
+lines of code.  Build Models First, we need to define a **model** which 1)
+inherits from `BaseModel` and 2) accepts an additional argument `mode` in the
+`forward` method, in addition to those arguments related to the dataset. -
+During training, the value of `mode` is "loss", and the `forward` method should
+return a `dict` containing the key "loss". - During validation, the value of
+`mode` is "predict", and the forward method should return results containing
+both predictions and labels. ```python import torch.nn.functional as F import
+torchvision from mmengine.model import BaseModel class MMResNet50(BaseModel):
+def __init__(self): super().__init__() self.resnet =
 torchvision.models.resnet50() def forward(self, imgs, labels, mode): x =
 self.resnet(imgs) if mode == 'loss': return {'loss': F.cross_entropy(x,
 labels)} elif mode == 'predict': return x, labels ```   Build Datasets Next, we
 need to create **Dataset**s and **DataLoader**s for training and validation. In
 this case, we simply use built-in datasets supported in TorchVision. ```python
 import torchvision.transforms as transforms from torch.utils.data import
 DataLoader norm_cfg = dict(mean=[0.491, 0.482, 0.447], std=[0.202, 0.199,
@@ -154,46 +163,47 @@
 Contributing We appreciate all contributions to improve MMEngine. Please refer
 to [CONTRIBUTING.md](CONTRIBUTING.md) for the contributing guideline. ##
 Citation If you find this project useful in your research, please consider
 cite: ``` @article{mmengine2022, title = {{MMEngine}: OpenMMLab Foundational
 Library for Training Deep Learning Models}, author = {MMEngine Contributors},
 howpublished = {\url{https://github.com/open-mmlab/mmengine}}, year={2022} }
 ``` ## License This project is released under the [Apache 2.0 license]
-(LICENSE). ## Projects in OpenMMLab - [MIM](https://github.com/open-mmlab/mim):
-MIM installs OpenMMLab packages. - [MMCV](https://github.com/open-mmlab/mmcv):
-OpenMMLab foundational library for computer vision. - [MMEval](https://
-github.com/open-mmlab/mmeval): A unified evaluation library for multiple
-machine learning libraries. - [MMPreTrain](https://github.com/open-mmlab/
-mmpretrain): OpenMMLab pre-training toolbox and benchmark. - [MMagic](https://
-github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
-**I**ntelligent **C**reation toolbox. - [MMDetection](https://github.com/open-
-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark. - [MMYOLO]
-(https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and
-benchmark. - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d):
-OpenMMLab's next-generation platform for general 3D object detection. -
-[MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object
-detection toolbox and benchmark. - [MMTracking](https://github.com/open-mmlab/
-mmtracking): OpenMMLab video perception toolbox and benchmark. - [MMPose]
-(https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and
-benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
-OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR](https://
-github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and
-understanding toolbox. - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d):
-OpenMMLab 3D human parametric model toolbox and benchmark. - [MMSelfSup](https:
-//github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox
-and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
-OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
-github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
-understanding toolbox and benchmark. - [MMFlow](https://github.com/open-mmlab/
-mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework. -
-[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
-toolbox and benchmark. - [Playground](https://github.com/open-mmlab/
-playground): A central hub for gathering and showcasing amazing projects built
-upon OpenMMLab. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
+(LICENSE). ## Ecosystem - [APES: Attention-based Point Cloud Edge Sampling]
+(https://github.com/JunweiZheng93/APES) ## Projects in OpenMMLab - [MIM](https:
+//github.com/open-mmlab/mim): MIM installs OpenMMLab packages. - [MMCV](https:/
+/github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
+vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation
+library for multiple machine learning libraries. - [MMPreTrain](https://
+github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+benchmark. - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab
+**A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMYOLO](https://github.com/open-mmlab/mmyolo):
+OpenMMLab YOLO series toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
+general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
+mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video
+perception toolbox and benchmark. - [MMPose](https://github.com/open-mmlab/
+mmpose): OpenMMLab pose estimation toolbox and benchmark. - [MMSegmentation]
+(https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation
+toolbox and benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr):
+OpenMMLab text detection, recognition, and understanding toolbox. - [MMHuman3D]
+(https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model
+toolbox and benchmark. - [MMSelfSup](https://github.com/open-mmlab/mmselfsup):
+OpenMMLab self-supervised learning toolbox and benchmark. - [MMFewShot](https:/
+/github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and
+benchmark. - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's
+next-generation action understanding toolbox and benchmark. - [MMFlow](https://
+github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model
+compression toolbox and benchmark. - [Playground](https://github.com/open-
+mmlab/playground): A central hub for gathering and showcasing amazing projects
+built upon OpenMMLab. Platform: UNKNOWN Classifier: Development Status :: 4 -
+Beta Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Utilities Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests
```

### Comparing `mmengine-0.8.2/README.md` & `mmengine-0.8.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,33 +54,49 @@
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
 </div>
 
 ## What's New
 
-v0.8.0 was released on 2023-06-30.
+v0.8.3 was released on 2023-07-31.
 
 Highlights:
 
+- Support enabling `efficient_conv_bn_eval` for efficient convolution and batch normalization. See [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#save-memory-on-gpu) for more details
+
+- Add an [example](./examples/llama2/) to finetune Llama2.
+
 - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for more detailed usages.
 
 - Introduce the pure Python style configuration file:
 
   - Support navigating to base configuration file in IDE
   - Support navigating to base variable in IDE
   - Support navigating to source code of class in IDE
   - Support inheriting two configuration files containing the same field
   - Load the configuration file without other third-party requirements
 
   Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
 
   ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
 
-Read [Changelog](./docs/en/notes/changelog.md#v080-06302023) for more details.
+Read [Changelog](./docs/en/notes/changelog.md#v083-07312023) for more details.
+
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Installation](#installation)
+- [Get Started](#get-started)
+- [Learn More](#learn-more)
+- [Contributing](#contributing)
+- [Citation](#citation)
+- [License](#license)
+- [Ecosystem](#ecosystem)
+- [Projects in OpenMMLab](#projects-in-openmmlab)
 
 ## Introduction
 
 MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
 
 Major features:
 
@@ -96,14 +112,16 @@
 
 3. **Customizable training process**:
 
    - Defines the training process just like playing with Legos.
    - Provides rich components and strategies.
    - Complete controls on the training process with different levels of APIs.
 
+![mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/267db9cb-72e4-4af2-a58b-877b30091acc)
+
 ## Installation
 
 Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
 
 Install MMEngine
 
 ```bash
@@ -336,14 +354,18 @@
 }
 ```
 
 ## License
 
 This project is released under the [Apache 2.0 license](LICENSE).
 
+## Ecosystem
+
+- [APES: Attention-based Point Cloud Edge Sampling](https://github.com/JunweiZheng93/APES)
+
 ## Projects in OpenMMLab
 
 - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
 - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
 - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
 - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
 - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
```

### Comparing `mmengine-0.8.2/mmengine/_strategy/__init__.py` & `mmengine-0.8.3/mmengine/_strategy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from mmengine.utils import digit_version, is_installed
+from mmengine.utils import digit_version
 from mmengine.utils.dl_utils import TORCH_VERSION
 from .base import BaseStrategy
+from .deepspeed import DeepSpeedStrategy
 from .distributed import DDPStrategy
 from .single_device import SingleDeviceStrategy
 
-__all__ = ['BaseStrategy', 'DDPStrategy', 'SingleDeviceStrategy']
-
-if is_installed('deepspeed'):
-    from .deepspeed import DeepSpeedStrategy  # noqa: F401
-    __all__.append('DeepSpeedStrategy')
+__all__ = [
+    'BaseStrategy', 'DDPStrategy', 'SingleDeviceStrategy', 'DeepSpeedStrategy'
+]
 
 if digit_version(TORCH_VERSION) >= digit_version('2.0.0'):
     try:
         from .fsdp import FSDPStrategy  # noqa:F401
         __all__.append('FSDPStrategy')
     except:  # noqa: E722
         pass
```

### Comparing `mmengine-0.8.2/mmengine/_strategy/base.py` & `mmengine-0.8.3/mmengine/_strategy/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/_strategy/deepspeed.py` & `mmengine-0.8.3/mmengine/_strategy/deepspeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import json
 import os.path as osp
 import time
 from typing import Callable, Dict, List, Optional, Union
 
-import deepspeed
+try:
+    import deepspeed
+except ImportError:
+    deepspeed = None
+
 import torch.nn as nn
 
 import mmengine
 from mmengine.dist import init_dist
 from mmengine.model.wrappers._deepspeed import MMDeepSpeedEngineWrapper
 from mmengine.optim import BaseOptimWrapper, _ParamScheduler
 from mmengine.registry import STRATEGIES
@@ -67,14 +71,18 @@
         train_micro_batch_size_per_gpu: Optional[int] = None,
         gradient_accumulation_steps: int = 1,
         # disable the log printed by deepseed
         steps_per_print: int = 10000000000000,
         # the following args are for BaseStrategy
         **kwargs,
     ):
+        assert deepspeed is not None, \
+            'DeepSpeed is not installed. Please check ' \
+            'https://github.com/microsoft/DeepSpeed#installation.'
+
         super().__init__(**kwargs)
 
         self.config = self._parse_config(config)
         if zero_optimization is not None:
             self.config['zero_optimization'] = zero_optimization
         self.config['gradient_clipping'] = gradient_clipping
         if fp16 is not None:
```

### Comparing `mmengine-0.8.2/mmengine/_strategy/distributed.py` & `mmengine-0.8.3/mmengine/_strategy/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/_strategy/fsdp.py` & `mmengine-0.8.3/mmengine/_strategy/fsdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     FullOptimStateDictConfig, LocalOptimStateDictConfig, OptimStateDictConfig,
     StateDictConfig)
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 
 import mmengine
 from mmengine.config import Config, ConfigDict
+from mmengine.device import get_device
 from mmengine.dist import get_rank, is_main_process
-from mmengine.model import is_model_wrapper
+from mmengine.model import BaseDataPreprocessor, is_model_wrapper
 from mmengine.optim import (AmpOptimWrapper, BaseOptimWrapper, OptimWrapper,
                             OptimWrapperDict, _ParamScheduler,
                             build_optim_wrapper)
 from mmengine.registry import (MODEL_WRAPPERS, OPTIM_WRAPPERS,
                                PARAM_SCHEDULERS, STRATEGIES, Registry)
 from mmengine.utils import get_git_hash, mkdir_or_exist
 from .distributed import DDPStrategy
@@ -114,14 +115,18 @@
         Args:
             model (nn.Module): Model to be wrapped.
 
         Returns:
             FullyShardedDataParallel: ``MMFullyShardedDataParallel``
             or subclass of ``FullyShardedDataParallel``.
         """
+        for module in model.modules():
+            if isinstance(module, BaseDataPreprocessor):
+                module.to(get_device())
+
         if is_model_wrapper(model):
             return
 
         if self.model_wrapper is None:
             self.model_wrapper = dict(type='MMFullyShardedDataParallel')
 
         default_args = dict(
```

### Comparing `mmengine-0.8.2/mmengine/_strategy/single_device.py` & `mmengine-0.8.3/mmengine/_strategy/single_device.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/_strategy/utils.py` & `mmengine-0.8.3/mmengine/_strategy/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/analysis/complexity_analysis.py` & `mmengine-0.8.3/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/analysis/jit_analysis.py` & `mmengine-0.8.3/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/analysis/jit_handles.py` & `mmengine-0.8.3/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/analysis/print_helper.py` & `mmengine-0.8.3/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/config/config.py` & `mmengine-0.8.3/mmengine/config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import ast
 import copy
+import difflib
 import os
 import os.path as osp
 import platform
 import shutil
 import sys
 import tempfile
 import types
@@ -13,20 +14,23 @@
 from argparse import Action, ArgumentParser, Namespace
 from collections import OrderedDict, abc
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Optional, Sequence, Tuple, Union
 
 from addict import Dict
+from rich.console import Console
+from rich.text import Text
 from yapf.yapflib.yapf_api import FormatCode
 
 from mmengine.fileio import dump, load
 from mmengine.logging import print_log
-from mmengine.utils import (check_file_exist, get_installed_path,
-                            import_modules_from_strings, is_installed)
+from mmengine.utils import (check_file_exist, digit_version,
+                            get_installed_path, import_modules_from_strings,
+                            is_installed)
 from .lazy import LazyAttr, LazyObject
 from .utils import (ConfigParsingError, ImportTransformer, RemoveAssignFromAST,
                     _gather_abs_import_lazyobj, _get_external_cfg_base_path,
                     _get_external_cfg_path, _get_package_and_cfg_path,
                     _is_builtin_module)
 
 BASE_KEY = '_base_'
@@ -257,23 +261,26 @@
                 return a if a is not default else b
 
         merged = _merge_a_into_b(copy.deepcopy(other), copy.deepcopy(self))
         self.clear()
         for key, value in merged.items():
             self[key] = value
 
-    def __getstate__(self):
-        state = {}
-        for key, value in super().items():
-            state[key] = value
-        return state
-
-    def __setstate__(self, state):
-        for key, value in state.items():
-            self[key] = value
+    def __reduce_ex__(self, proto):
+        # Override __reduce_ex__ to avoid `self.items` will be
+        # called by CPython interpreter during pickling. See more details in
+        # https://github.com/python/cpython/blob/8d61a71f9c81619e34d4a30b625922ebc83c561b/Objects/typeobject.c#L6196  # noqa: E501
+        if digit_version(platform.python_version()) < digit_version('3.8'):
+            return (self.__class__, ({k: v
+                                      for k, v in super().items()}, ), None,
+                    None, None)
+        else:
+            return (self.__class__, ({k: v
+                                      for k, v in super().items()}, ), None,
+                    None, None, None)
 
     def __eq__(self, other):
         if isinstance(other, ConfigDict):
             return other.to_dict() == self.to_dict()
         elif isinstance(other, dict):
             return {k: v for k, v in self.items()} == other
         else:
@@ -899,15 +906,15 @@
                     base_cfg_dict.update(_cfg_dict)
 
                 if filename.endswith('.py'):
                     with open(temp_config_file.name, encoding='utf-8') as f:
                         parsed_codes = ast.parse(f.read())
                         parsed_codes = RemoveAssignFromAST(BASE_KEY).visit(
                             parsed_codes)
-                    codeobj = compile(parsed_codes, '', mode='exec')
+                    codeobj = compile(parsed_codes, filename, mode='exec')
                     # Support load global variable in nested function of the
                     # config.
                     global_locals_var = {BASE_KEY: base_cfg_dict}
                     ori_keys = set(global_locals_var.keys())
                     eval(codeobj, global_locals_var, global_locals_var)
                     cfg_dict = {
                         key: value
@@ -1217,16 +1224,17 @@
                 else:
                     base_files = []
         elif file_format in ('.yml', '.yaml', '.json'):
             import mmengine
             cfg_dict = mmengine.load(filename)
             base_files = cfg_dict.get(BASE_KEY, [])
         else:
-            raise TypeError('The config type should be py, json, yaml or '
-                            f'yml, but got {file_format}')
+            raise ConfigParsingError(
+                'The config type should be py, json, yaml or '
+                f'yml, but got {file_format}')
         base_files = base_files if isinstance(base_files,
                                               list) else [base_files]
         return base_files
 
     @staticmethod
     def _get_cfg_path(cfg_path: str,
                       filename: str) -> Tuple[str, Optional[str]]:
@@ -1428,15 +1436,16 @@
         def _format_dict(input_dict, outest_level=False):
             r = ''
             s = []
 
             use_mapping = _contain_invalid_identifier(input_dict)
             if use_mapping:
                 r += '{'
-            for idx, (k, v) in enumerate(input_dict.items()):
+            for idx, (k, v) in enumerate(
+                    sorted(input_dict.items(), key=lambda x: str(x[0]))):
                 is_last = idx >= len(input_dict) - 1
                 end = '' if outest_level or is_last else ','
                 if isinstance(v, dict):
                     v_str = '\n' + _format_dict(v)
                     if use_mapping:
                         k_str = f"'{k}'" if isinstance(k, str) else str(k)
                         attr_str = f'{k_str}: dict({v_str}'
@@ -1602,14 +1611,44 @@
         cfg_dict = super().__getattribute__('_cfg_dict')
         super().__setattr__(
             '_cfg_dict',
             Config._merge_a_into_b(
                 option_cfg_dict, cfg_dict, allow_list_keys=allow_list_keys))
 
     @staticmethod
+    def diff(cfg1: Union[str, 'Config'], cfg2: Union[str, 'Config']) -> str:
+        if isinstance(cfg1, str):
+            cfg1 = Config.fromfile(cfg1)
+
+        if isinstance(cfg2, str):
+            cfg2 = Config.fromfile(cfg2)
+
+        res = difflib.unified_diff(
+            cfg1.pretty_text.split('\n'), cfg2.pretty_text.split('\n'))
+
+        # Convert into rich format for better visualization
+        console = Console()
+        text = Text()
+        for line in res:
+            if line.startswith('+'):
+                color = 'bright_green'
+            elif line.startswith('-'):
+                color = 'bright_red'
+            else:
+                color = 'bright_white'
+            _text = Text(line + '\n')
+            _text.stylize(color)
+            text.append(_text)
+
+        with console.capture() as capture:
+            console.print(text)
+
+        return capture.get()
+
+    @staticmethod
     def _is_lazy_import(filename: str) -> bool:
         if not filename.endswith('.py'):
             return False
         with open(filename, encoding='utf-8') as f:
             codes_str = f.read()
             parsed_codes = ast.parse(codes_str)
         for node in ast.walk(parsed_codes):
```

### Comparing `mmengine-0.8.2/mmengine/config/lazy.py` & `mmengine-0.8.3/mmengine/config/lazy.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/config/utils.py` & `mmengine-0.8.3/mmengine/config/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dataset/__init__.py` & `mmengine-0.8.3/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dataset/base_dataset.py` & `mmengine-0.8.3/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.8.3/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dataset/sampler.py` & `mmengine-0.8.3/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dataset/utils.py` & `mmengine-0.8.3/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/device/utils.py` & `mmengine-0.8.3/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dist/__init__.py` & `mmengine-0.8.3/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dist/dist.py` & `mmengine-0.8.3/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/dist/utils.py` & `mmengine-0.8.3/mmengine/dist/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,16 @@
         backend (str): Backend of torch.distributed. Supported backends are
             'nccl', 'gloo' and 'mpi'. Defaults to 'nccl'.
         **kwargs: keyword arguments are passed to ``init_process_group``.
     """
     rank = int(os.environ['RANK'])
     if is_mlu_available():
         import torch_mlu  # noqa: F401
-        torch.mlu.set_device(rank)
+        local_rank = int(os.environ['LOCAL_RANK'])
+        torch.mlu.set_device(local_rank)
         torch_dist.init_process_group(
             backend='cncl',
             rank=rank,
             world_size=int(os.environ['WORLD_SIZE']),
             **kwargs)
     elif is_npu_available():
         import torch_npu  # noqa: F401
```

### Comparing `mmengine-0.8.2/mmengine/evaluator/evaluator.py` & `mmengine-0.8.3/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/evaluator/metric.py` & `mmengine-0.8.3/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/evaluator/utils.py` & `mmengine-0.8.3/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/__init__.py` & `mmengine-0.8.3/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/__init__.py` & `mmengine-0.8.3/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/base.py` & `mmengine-0.8.3/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/http_backend.py` & `mmengine-0.8.3/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.8.3/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/local_backend.py` & `mmengine-0.8.3/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.8.3/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.8.3/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.8.3/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/file_client.py` & `mmengine-0.8.3/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/handlers/base.py` & `mmengine-0.8.3/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.8.3/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.8.3/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.8.3/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.8.3/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/io.py` & `mmengine-0.8.3/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/fileio/parse.py` & `mmengine-0.8.3/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/__init__.py` & `mmengine-0.8.3/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.8.3/mmengine/hooks/checkpoint_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,19 @@
             prefix of uri corresponding backend. Defaults to None.
             `New in version 0.2.0.`
         published_keys (str, List[str], optional): If ``save_last`` is ``True``
             or ``save_best`` is not ``None``, it will automatically
             publish model with keys in the list after training.
             Defaults to None.
             `New in version 0.7.1.`
+        save_begin (int): Control the epoch number or iteration number
+            at which checkpoint saving begins. Defaults to 0, which means
+            saving at the beginning.
+            `New in version 0.8.3.`
+
     Examples:
         >>> # Save best based on single metric
         >>> CheckpointHook(interval=2, by_epoch=True, save_best='acc',
         >>>                rule='less')
         >>> # Save best based on multi metrics with the same comparison rule
         >>> CheckpointHook(interval=2, by_epoch=True,
         >>>                save_best=['acc', 'mIoU'], rule='greater')
@@ -135,14 +140,15 @@
                  rule: Union[str, List[str], None] = None,
                  greater_keys: Optional[Sequence[str]] = None,
                  less_keys: Optional[Sequence[str]] = None,
                  file_client_args: Optional[dict] = None,
                  filename_tmpl: Optional[str] = None,
                  backend_args: Optional[dict] = None,
                  published_keys: Union[str, List[str], None] = None,
+                 save_begin: int = 0,
                  **kwargs) -> None:
         self.interval = interval
         self.by_epoch = by_epoch
         self.save_optimizer = save_optimizer
         self.save_param_scheduler = save_param_scheduler
         self.out_dir = out_dir  # type: ignore
         self.max_keep_ckpts = max_keep_ckpts
@@ -240,14 +246,18 @@
             published_keys = [published_keys]
         elif isinstance(published_keys, (list, tuple)):
             assert len(published_keys) == len(set(published_keys)), (
                 'Find duplicate elements in "published_keys".')
         self.published_keys = published_keys
 
         self.last_ckpt = None
+        if save_begin < 0:
+            raise ValueError(
+                'save_begin should not be less than 0, but got {save_begin}')
+        self.save_begin = save_begin
 
     def before_train(self, runner) -> None:
         """Finish all operations, related to checkpoint.
 
         This function will get the appropriate file client, and the directory
         to save these checkpoints of the model.
 
@@ -322,17 +332,17 @@
         Args:
             runner (Runner): The runner of the training process.
         """
         if not self.by_epoch:
             return
 
         # save checkpoint for following cases:
-        # 1. every ``self.interval`` epochs
+        # 1. every ``self.interval`` epochs which start at ``self.save_begin``
         # 2. reach the last epoch of training
-        if self.every_n_epochs(runner, self.interval) or (
+        if self.every_n_epochs(runner, self.interval, self.save_begin) or (
                 self.save_last and self.is_last_train_epoch(runner)):
             runner.logger.info(
                 f'Saving checkpoint at {runner.epoch + 1} epochs')
             self._save_checkpoint(runner)
 
     def after_val_epoch(self, runner, metrics):
         """Save the checkpoint and synchronize buffers after each evaluation
@@ -640,14 +650,16 @@
             outputs (dict, optional): Outputs from model.
         """
         if self.by_epoch:
             return
 
         # save checkpoint for following cases:
         # 1. every ``self.interval`` iterations
+        #       which start at ``self.save_begin``
         # 2. reach the last iteration of training
-        if self.every_n_train_iters(runner, self.interval) or \
+        if self.every_n_train_iters(runner, self.interval,
+                                    self.save_begin) or \
                 (self.save_last and
                  self.is_last_train_iter(runner)):
             runner.logger.info(
                 f'Saving checkpoint at {runner.iter + 1} iterations')
             self._save_checkpoint(runner)
```

### Comparing `mmengine-0.8.2/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.8.3/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/ema_hook.py` & `mmengine-0.8.3/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.8.3/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/hook.py` & `mmengine-0.8.3/mmengine/hooks/hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,26 +331,29 @@
                 process.
             batch_idx (int): The index of the current batch in the loop.
             data_batch (dict or tuple or list, optional): Data from dataloader.
             outputs (dict or Sequence, optional): Outputs from model.
             mode (str): Current mode of runner. Defaults to 'train'.
         """
 
-    def every_n_epochs(self, runner, n: int) -> bool:
+    def every_n_epochs(self, runner, n: int, start: int = 0) -> bool:
         """Test whether current epoch can be evenly divided by n.
 
         Args:
             runner (Runner): The runner of the training, validation or testing
                 process.
             n (int): Whether current epoch can be evenly divided by n.
+            start (int): Starting from `start` to check the logic for
+                every n epochs. Defaults to 0.
 
         Returns:
             bool: Whether current epoch can be evenly divided by n.
         """
-        return (runner.epoch + 1) % n == 0 if n > 0 else False
+        dividend = runner.epoch + 1 - start
+        return dividend % n == 0 if dividend >= 0 and n > 0 else False
 
     def every_n_inner_iters(self, batch_idx: int, n: int) -> bool:
         """Test whether current inner iteration can be evenly divided by n.
 
         Args:
             batch_idx (int): Current batch index of the training, validation
                 or testing loop.
@@ -359,27 +362,30 @@
 
         Returns:
             bool: Whether current inner iteration can be evenly
             divided by n.
         """
         return (batch_idx + 1) % n == 0 if n > 0 else False
 
-    def every_n_train_iters(self, runner, n: int) -> bool:
+    def every_n_train_iters(self, runner, n: int, start: int = 0) -> bool:
         """Test whether current training iteration can be evenly divided by n.
 
         Args:
             runner (Runner): The runner of the training, validation or testing
                 process.
             n (int): Whether current iteration can be evenly divided by n.
+            start (int): Starting from `start` to check the logic for
+                every n iterations. Defaults to 0.
 
         Returns:
             bool: Return True if the current iteration can be evenly divided
             by n, otherwise False.
         """
-        return (runner.iter + 1) % n == 0 if n > 0 else False
+        dividend = runner.iter + 1 - start
+        return dividend % n == 0 if dividend >= 0 and n > 0 else False
 
     def end_of_epoch(self, dataloader, batch_idx: int) -> bool:
         """Check whether the current iteration reaches the last iteration of
         the dataloader.
 
         Args:
             dataloader (Dataloader): The dataloader of the training,
```

### Comparing `mmengine-0.8.2/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.8.3/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/logger_hook.py` & `mmengine-0.8.3/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.8.3/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.8.3/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/profiler_hook.py` & `mmengine-0.8.3/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.8.3/mmengine/hooks/runtime_info_hook.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         value (Any): value of log.
 
     Returns:
         bool: whether the value is a scalar type value.
     """
     if isinstance(value, np.ndarray):
         return value.size == 1
-    elif isinstance(value, (int, float)):
+    elif isinstance(value, (int, float, np.number)):
         return True
     elif isinstance(value, torch.Tensor):
         return value.numel() == 1
     return False
 
 
 @HOOKS.register_module()
@@ -50,28 +50,34 @@
         metainfo = dict(
             cfg=runner.cfg.pretty_text,
             seed=runner.seed,
             experiment_name=runner.experiment_name,
             mmengine_version=__version__ + get_git_hash())
         runner.message_hub.update_info_dict(metainfo)
 
+        self.last_loop_stage = None
+
     def before_train(self, runner) -> None:
         """Update resumed training state.
 
         Args:
             runner (Runner): The runner of the training process.
         """
+        runner.message_hub.update_info('loop_stage', 'train')
         runner.message_hub.update_info('epoch', runner.epoch)
         runner.message_hub.update_info('iter', runner.iter)
         runner.message_hub.update_info('max_epochs', runner.max_epochs)
         runner.message_hub.update_info('max_iters', runner.max_iters)
         if hasattr(runner.train_dataloader.dataset, 'metainfo'):
             runner.message_hub.update_info(
                 'dataset_meta', runner.train_dataloader.dataset.metainfo)
 
+    def after_train(self, runner) -> None:
+        runner.message_hub.pop_info('loop_stage')
+
     def before_train_epoch(self, runner) -> None:
         """Update current epoch information before every epoch.
 
         Args:
             runner (Runner): The runner of the training process.
         """
         runner.message_hub.update_info('epoch', runner.epoch)
@@ -115,14 +121,18 @@
                 Defaults to None.
             outputs (dict, optional): Outputs from model. Defaults to None.
         """
         if outputs is not None:
             for key, value in outputs.items():
                 runner.message_hub.update_scalar(f'train/{key}', value)
 
+    def before_val(self, runner) -> None:
+        self.last_loop_stage = runner.message_hub.get_info('loop_stage')
+        runner.message_hub.update_info('loop_stage', 'val')
+
     def after_val_epoch(self,
                         runner,
                         metrics: Optional[Dict[str, float]] = None) -> None:
         """All subclasses should override this method, if they need any
         operations after each validation epoch.
 
         Args:
@@ -134,14 +144,30 @@
         if metrics is not None:
             for key, value in metrics.items():
                 if _is_scalar(value):
                     runner.message_hub.update_scalar(f'val/{key}', value)
                 else:
                     runner.message_hub.update_info(f'val/{key}', value)
 
+    def after_val(self, runner) -> None:
+        # ValLoop may be called within the TrainLoop, so we need to reset
+        # the loop_stage
+        # workflow: before_train -> before_val -> after_val -> after_train
+        if self.last_loop_stage == 'train':
+            runner.message_hub.update_info('loop_stage', self.last_loop_stage)
+            self.last_loop_stage = None
+        else:
+            runner.message_hub.pop_info('loop_stage')
+
+    def before_test(self, runner) -> None:
+        runner.message_hub.update_info('loop_stage', 'test')
+
+    def after_test(self, runner) -> None:
+        runner.message_hub.pop_info('loop_stage')
+
     def after_test_epoch(self,
                          runner,
                          metrics: Optional[Dict[str, float]] = None) -> None:
         """All subclasses should override this method, if they need any
         operations after each test epoch.
 
         Args:
```

### Comparing `mmengine-0.8.2/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.8.3/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.8.3/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.8.3/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hub/hub.py` & `mmengine-0.8.3/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hub/mmcls.json` & `mmengine-0.8.3/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hub/openmmlab.json` & `mmengine-0.8.3/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/hub/torchvision_0.12.json` & `mmengine-0.8.3/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/infer/infer.py` & `mmengine-0.8.3/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/logging/history_buffer.py` & `mmengine-0.8.3/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/logging/logger.py` & `mmengine-0.8.3/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/logging/message_hub.py` & `mmengine-0.8.3/mmengine/logging/message_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,28 @@
             value (Any): Value of runtime information.
             resumed (bool): Whether the corresponding ``HistoryBuffer``
                 could be resumed.
         """
         self._set_resumed_keys(key, resumed)
         self._runtime_info[key] = value
 
+    def pop_info(self, key: str, default: Optional[Any] = None) -> Any:
+        """Remove runtime information by key. If the key does not exist, this
+        method will return the default value.
+
+        Args:
+            key (str): Key of runtime information.
+            default (Any, optional): The default returned value for the
+                given key.
+
+        Returns:
+            Any: The runtime information if the key exists.
+        """
+        return self._runtime_info.pop(key, default)
+
     def update_info_dict(self, info_dict: dict, resumed: bool = True) -> None:
         """Update runtime information with dictionary.
 
         The key corresponding runtime information will be overwritten each
         time calling ``update_info``.
 
         Note:
@@ -285,15 +299,15 @@
         """
         if key not in self.log_scalars:
             raise KeyError(f'{key} is not found in Messagehub.log_buffers: '
                            f'instance name is: {MessageHub.instance_name}')
         return self.log_scalars[key]
 
     def get_info(self, key: str, default: Optional[Any] = None) -> Any:
-        """Get runtime information by key. if the key does not exist, this
+        """Get runtime information by key. If the key does not exist, this
         method will return default information.
 
         Args:
             key (str): Key of runtime information.
             default (Any, optional): The default returned value for the
                 given key.
```

### Comparing `mmengine-0.8.2/mmengine/model/__init__.py` & `mmengine-0.8.3/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/averaged_model.py` & `mmengine-0.8.3/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/base_model/base_model.py` & `mmengine-0.8.3/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.8.3/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/base_module.py` & `mmengine-0.8.3/mmengine/model/base_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,18 @@
         #         key, please consider using init_cfg')
         #     self.init_cfg = dict(type='Pretrained', checkpoint=pretrained)
 
     @property
     def is_init(self):
         return self._is_init
 
+    @is_init.setter
+    def is_init(self, value):
+        self._is_init = value
+
     def init_weights(self):
         """Initialize the weights."""
 
         is_top_level_module = False
         # check if it is top-level module
         if not hasattr(self, '_params_init_info'):
             # The `_params_init_info` is used to record the initialization
@@ -123,15 +127,16 @@
                         other_cfgs.append(init_cfg)
 
                 initialize(self, other_cfgs)
 
             for m in self.children():
                 if is_model_wrapper(m) and not hasattr(m, 'init_weights'):
                     m = m.module
-                if hasattr(m, 'init_weights'):
+                if hasattr(m, 'init_weights') and not getattr(
+                        m, 'is_init', False):
                     m.init_weights()
                     # users may overload the `init_weights`
                     update_init_info(
                         m,
                         init_info=f'Initialized by '
                         f'user-defined `init_weights`'
                         f' in {m.__class__.__name__} ')
```

### Comparing `mmengine-0.8.2/mmengine/model/test_time_aug.py` & `mmengine-0.8.3/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/utils.py` & `mmengine-0.8.3/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/weight_init.py` & `mmengine-0.8.3/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/wrappers/__init__.py` & `mmengine-0.8.3/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/wrappers/_deepspeed.py` & `mmengine-0.8.3/mmengine/model/wrappers/_deepspeed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import Any, Dict, List, Optional, Union
 
 import torch
-from deepspeed.runtime.engine import DeepSpeedEngine
 
 from mmengine.optim.optimizer._deepspeed import DeepSpeedOptimWrapper
 from mmengine.registry import MODEL_WRAPPERS
 
+try:
+    from deepspeed.runtime.engine import DeepSpeedEngine
+except ImportError:
+    DeepSpeedEngine = None
+
 
 @MODEL_WRAPPERS.register_module()
 class MMDeepSpeedEngineWrapper:
 
     def __init__(
         self,
         *,
```

### Comparing `mmengine-0.8.2/mmengine/model/wrappers/distributed.py` & `mmengine-0.8.3/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.8.3/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.8.3/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/model/wrappers/utils.py` & `mmengine-0.8.3/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/__init__.py` & `mmengine-0.8.3/mmengine/optim/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from mmengine.utils import is_installed
 from .optimizer import (OPTIM_WRAPPER_CONSTRUCTORS, OPTIMIZERS,
                         AmpOptimWrapper, ApexOptimWrapper, BaseOptimWrapper,
-                        DefaultOptimWrapperConstructor, OptimWrapper,
-                        OptimWrapperDict, ZeroRedundancyOptimizer,
-                        build_optim_wrapper)
+                        DeepSpeedOptimWrapper, DefaultOptimWrapperConstructor,
+                        OptimWrapper, OptimWrapperDict,
+                        ZeroRedundancyOptimizer, build_optim_wrapper)
 # yapf: disable
 from .scheduler import (ConstantLR, ConstantMomentum, ConstantParamScheduler,
                         CosineAnnealingLR, CosineAnnealingMomentum,
                         CosineAnnealingParamScheduler, ExponentialLR,
                         ExponentialMomentum, ExponentialParamScheduler,
                         LinearLR, LinearMomentum, LinearParamScheduler,
                         MultiStepLR, MultiStepMomentum,
@@ -28,13 +27,9 @@
     'MultiStepMomentum', 'StepMomentum', 'ConstantParamScheduler',
     'CosineAnnealingParamScheduler', 'ExponentialParamScheduler',
     'LinearParamScheduler', 'MultiStepParamScheduler', 'StepParamScheduler',
     '_ParamScheduler', 'OptimWrapper', 'AmpOptimWrapper', 'ApexOptimWrapper',
     'OptimWrapperDict', 'OneCycleParamScheduler', 'OneCycleLR', 'PolyLR',
     'PolyMomentum', 'PolyParamScheduler', 'ReduceOnPlateauLR',
     'ReduceOnPlateauMomentum', 'ReduceOnPlateauParamScheduler',
-    'ZeroRedundancyOptimizer', 'BaseOptimWrapper'
+    'ZeroRedundancyOptimizer', 'BaseOptimWrapper', 'DeepSpeedOptimWrapper'
 ]
-
-if is_installed('deepspeed'):
-    from .optimizer import DeepSpeedOptimWrapper  # noqa:F401
-    __all__.append('DeepSpeedOptimWrapper')
```

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/__init__.py` & `mmengine-0.8.3/mmengine/optim/optimizer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from mmengine.utils import is_installed
+from ._deepspeed import DeepSpeedOptimWrapper
 from .amp_optimizer_wrapper import AmpOptimWrapper
 from .apex_optimizer_wrapper import ApexOptimWrapper
 from .base import BaseOptimWrapper
 from .builder import (OPTIM_WRAPPER_CONSTRUCTORS, OPTIMIZERS,
                       build_optim_wrapper)
 from .default_constructor import DefaultOptimWrapperConstructor
 from .optimizer_wrapper import OptimWrapper
 from .optimizer_wrapper_dict import OptimWrapperDict
 from .zero_optimizer import ZeroRedundancyOptimizer
 
 __all__ = [
     'OPTIM_WRAPPER_CONSTRUCTORS', 'OPTIMIZERS',
     'DefaultOptimWrapperConstructor', 'build_optim_wrapper', 'OptimWrapper',
     'AmpOptimWrapper', 'ApexOptimWrapper', 'OptimWrapperDict',
-    'ZeroRedundancyOptimizer', 'BaseOptimWrapper'
+    'ZeroRedundancyOptimizer', 'BaseOptimWrapper', 'DeepSpeedOptimWrapper'
 ]
-
-if is_installed('deepspeed'):
-    from ._deepspeed import DeepSpeedOptimWrapper  # noqa:F401
-    __all__.append('DeepSpeedOptimWrapper')
```

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/_deepspeed.py` & `mmengine-0.8.3/mmengine/optim/optimizer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.8.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.8.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/base.py` & `mmengine-0.8.3/mmengine/optim/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/builder.py` & `mmengine-0.8.3/mmengine/optim/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.8.3/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.8.3/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/scheduler/__init__.py` & `mmengine-0.8.3/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.8.3/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.8.3/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.8.3/mmengine/optim/scheduler/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/registry/__init__.py` & `mmengine-0.8.3/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/registry/build_functions.py` & `mmengine-0.8.3/mmengine/registry/build_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,60 +94,51 @@
     scope = args.pop('_scope_', None)
     with registry.switch_scope_and_registry(scope) as registry:
         obj_type = args.pop('type')
         if isinstance(obj_type, str):
             obj_cls = registry.get(obj_type)
             if obj_cls is None:
                 raise KeyError(
-                    f'{obj_type} is not in the {registry.name} registry. '
+                    f'{obj_type} is not in the {registry.scope}::{registry.name} registry. '  # noqa: E501
                     f'Please check whether the value of `{obj_type}` is '
                     'correct or it was registered as expected. More details '
                     'can be found at '
                     'https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#import-the-custom-module'  # noqa: E501
                 )
         # this will include classes, functions, partial functions and more
         elif callable(obj_type):
             obj_cls = obj_type
         else:
             raise TypeError(
                 f'type must be a str or valid type, but got {type(obj_type)}')
 
-        try:
-            # If `obj_cls` inherits from `ManagerMixin`, it should be
-            # instantiated by `ManagerMixin.get_instance` to ensure that it
-            # can be accessed globally.
-            if inspect.isclass(obj_cls) and \
-                    issubclass(obj_cls, ManagerMixin):  # type: ignore
-                obj = obj_cls.get_instance(**args)  # type: ignore
-            else:
-                obj = obj_cls(**args)  # type: ignore
-
-            if (inspect.isclass(obj_cls) or inspect.isfunction(obj_cls)
-                    or inspect.ismethod(obj_cls)):
-                print_log(
-                    f'An `{obj_cls.__name__}` instance is built from '  # type: ignore # noqa: E501
-                    'registry, and its implementation can be found in '
-                    f'{obj_cls.__module__}',  # type: ignore
-                    logger='current',
-                    level=logging.DEBUG)
-            else:
-                print_log(
-                    'An instance is built from registry, and its constructor '
-                    f'is {obj_cls}',
-                    logger='current',
-                    level=logging.DEBUG)
-            return obj
-
-        except Exception as e:
-            # Normal TypeError does not print class name.
-            cls_location = '/'.join(
-                obj_cls.__module__.split('.'))  # type: ignore
-            raise type(e)(
-                f'class `{obj_cls.__name__}` in '  # type: ignore
-                f'{cls_location}.py: {e}')
+        # If `obj_cls` inherits from `ManagerMixin`, it should be
+        # instantiated by `ManagerMixin.get_instance` to ensure that it
+        # can be accessed globally.
+        if inspect.isclass(obj_cls) and \
+                issubclass(obj_cls, ManagerMixin):  # type: ignore
+            obj = obj_cls.get_instance(**args)  # type: ignore
+        else:
+            obj = obj_cls(**args)  # type: ignore
+
+        if (inspect.isclass(obj_cls) or inspect.isfunction(obj_cls)
+                or inspect.ismethod(obj_cls)):
+            print_log(
+                f'An `{obj_cls.__name__}` instance is built from '  # type: ignore # noqa: E501
+                'registry, and its implementation can be found in '
+                f'{obj_cls.__module__}',  # type: ignore
+                logger='current',
+                level=logging.DEBUG)
+        else:
+            print_log(
+                'An instance is built from registry, and its constructor '
+                f'is {obj_cls}',
+                logger='current',
+                level=logging.DEBUG)
+        return obj
 
 
 def build_runner_from_cfg(cfg: Union[dict, ConfigDict, Config],
                           registry: Registry) -> 'Runner':
     """Build a Runner object.
 
     Examples:
@@ -198,31 +189,22 @@
                 )
         elif inspect.isclass(obj_type):
             runner_cls = obj_type
         else:
             raise TypeError(
                 f'type must be a str or valid type, but got {type(obj_type)}')
 
-        try:
-            runner = runner_cls.from_cfg(args)  # type: ignore
-            print_log(
-                f'An `{runner_cls.__name__}` instance is built from '  # type: ignore # noqa: E501
-                'registry, its implementation can be found in'
-                f'{runner_cls.__module__}',  # type: ignore
-                logger='current',
-                level=logging.DEBUG)
-            return runner
-
-        except Exception as e:
-            # Normal TypeError does not print class name.
-            cls_location = '/'.join(
-                runner_cls.__module__.split('.'))  # type: ignore
-            raise type(e)(
-                f'class `{runner_cls.__name__}` in '  # type: ignore
-                f'{cls_location}.py: {e}')
+        runner = runner_cls.from_cfg(args)  # type: ignore
+        print_log(
+            f'An `{runner_cls.__name__}` instance is built from '  # type: ignore # noqa: E501
+            'registry, its implementation can be found in'
+            f'{runner_cls.__module__}',  # type: ignore
+            logger='current',
+            level=logging.DEBUG)
+        return runner
 
 
 def build_model_from_cfg(
     cfg: Union[dict, ConfigDict, Config],
     registry: Registry,
     default_args: Optional[Union[dict, 'ConfigDict', 'Config']] = None
 ) -> 'nn.Module':
```

### Comparing `mmengine-0.8.2/mmengine/registry/default_scope.py` & `mmengine-0.8.3/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/registry/registry.py` & `mmengine-0.8.3/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/registry/root.py` & `mmengine-0.8.3/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/registry/utils.py` & `mmengine-0.8.3/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/__init__.py` & `mmengine-0.8.3/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/_flexible_runner.py` & `mmengine-0.8.3/mmengine/runner/_flexible_runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/amp.py` & `mmengine-0.8.3/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/base_loop.py` & `mmengine-0.8.3/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/checkpoint.py` & `mmengine-0.8.3/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/log_processor.py` & `mmengine-0.8.3/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/loops.py` & `mmengine-0.8.3/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/priority.py` & `mmengine-0.8.3/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/runner/runner.py` & `mmengine-0.8.3/mmengine/runner/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
                            is_distributed, master_only)
 from mmengine.evaluator import Evaluator
 from mmengine.fileio import FileClient, join_path
 from mmengine.hooks import Hook
 from mmengine.logging import MessageHub, MMLogger, print_log
 from mmengine.model import (MMDistributedDataParallel, convert_sync_batchnorm,
                             is_model_wrapper, revert_sync_batchnorm)
+from mmengine.model.efficient_conv_bn_eval import \
+    turn_on_efficient_conv_bn_eval
 from mmengine.optim import (OptimWrapper, OptimWrapperDict, _ParamScheduler,
                             build_optim_wrapper)
 from mmengine.registry import (DATA_SAMPLERS, DATASETS, EVALUATOR, FUNCTIONS,
                                HOOKS, LOG_PROCESSORS, LOOPS, MODEL_WRAPPERS,
                                MODELS, OPTIM_WRAPPERS, PARAM_SCHEDULERS,
                                RUNNERS, VISUALIZERS, DefaultScope)
 from mmengine.utils import apply_to, digit_version, get_git_hash, is_seq_of
@@ -1715,14 +1717,22 @@
             self._val_loop = self.build_val_loop(
                 self._val_loop)  # type: ignore
         # TODO: add a contextmanager to avoid calling `before_run` many times
         self.call_hook('before_run')
 
         # initialize the model weights
         self._init_model_weights()
+
+        # try to enable efficient_conv_bn_eval feature
+        modules = self.cfg.get('efficient_conv_bn_eval', None)
+        if modules is not None:
+            self.logger.info(f'Enabling the "efficient_conv_bn_eval" feature'
+                             f' for sub-modules: {modules}')
+            turn_on_efficient_conv_bn_eval(ori_model, modules)
+
         # make sure checkpoint-related hooks are triggered after `before_run`
         self.load_or_resume()
 
         # Initiate inner count of `optim_wrapper`.
         self.optim_wrapper.initialize_count_status(
             self.model,
             self._train_loop.iter,  # type: ignore
```

### Comparing `mmengine-0.8.2/mmengine/runner/utils.py` & `mmengine-0.8.3/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/structures/base_data_element.py` & `mmengine-0.8.3/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/structures/instance_data.py` & `mmengine-0.8.3/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/structures/label_data.py` & `mmengine-0.8.3/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/structures/pixel_data.py` & `mmengine-0.8.3/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/testing/__init__.py` & `mmengine-0.8.3/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/testing/_internal/distributed.py` & `mmengine-0.8.3/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/testing/compare.py` & `mmengine-0.8.3/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/testing/runner_test_case.py` & `mmengine-0.8.3/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/__init__.py` & `mmengine-0.8.3/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/hub.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/misc.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/trace.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.8.3/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/manager.py` & `mmengine-0.8.3/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/misc.py` & `mmengine-0.8.3/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/package_utils.py` & `mmengine-0.8.3/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/path.py` & `mmengine-0.8.3/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/progressbar.py` & `mmengine-0.8.3/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/timer.py` & `mmengine-0.8.3/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/utils/version_utils.py` & `mmengine-0.8.3/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/version.py` & `mmengine-0.8.3/mmengine/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.8.2/mmengine/visualization/utils.py` & `mmengine-0.8.3/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/visualization/vis_backend.py` & `mmengine-0.8.3/mmengine/visualization/vis_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.2/mmengine/visualization/visualizer.py` & `mmengine-0.8.3/mmengine/visualization/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 import os.path as osp
 import warnings
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple, Union
 
 if TYPE_CHECKING:
     from matplotlib.font_manager import FontProperties
 
-import logging
-
 import cv2
 import numpy as np
 import torch
 import torch.nn.functional as F
 
 from mmengine.config import Config
 from mmengine.dist import master_only
-from mmengine.logging import print_log
 from mmengine.registry import VISBACKENDS, VISUALIZERS
 from mmengine.structures import BaseDataElement
 from mmengine.utils import ManagerMixin
 from mmengine.visualization.utils import (check_type, check_type_and_length,
                                           color_str2rgb, color_val_matplotlib,
                                           convert_overlay_heatmap,
                                           img_from_canvas, tensor2ndarray,
@@ -161,25 +158,17 @@
         fig_save_cfg=dict(frameon=False),
         fig_show_cfg=dict(frameon=False)
     ) -> None:
         super().__init__(name)
         self._dataset_meta: Optional[dict] = None
         self._vis_backends: Union[Dict, Dict[str, 'BaseVisBackend']] = dict()
 
-        if save_dir is None:
-            print_log(
-                '`Visualizer` backend is not initialized '
-                'because save_dir is None.',
-                logger='current',
-                level=logging.WARNING)
-        elif vis_backends is not None:
+        if vis_backends is not None:
             assert len(vis_backends) > 0, 'empty list'
-            names = [
-                vis_backend.get('name', None) for vis_backend in vis_backends
-            ]
+            names = [vis_backend.get('name') for vis_backend in vis_backends]
             if None in names:
                 if len(set(names)) > 1:
                     raise RuntimeError(
                         'If one of them has a name attribute, '
                         'all backends must use the name attribute')
                 else:
                     type_names = [
@@ -190,16 +179,16 @@
                             'The same vis backend cannot exist in '
                             '`vis_backend` config. '
                             'Please specify the name field.')
 
             if None not in names and len(set(names)) != len(names):
                 raise RuntimeError('The name fields cannot be the same')
 
-            save_dir = osp.join(save_dir, 'vis_data')
-
+            if save_dir is not None:
+                save_dir = osp.join(save_dir, 'vis_data')
             for vis_backend in vis_backends:
                 name = vis_backend.pop('name', vis_backend['type'])
                 vis_backend.setdefault('save_dir', save_dir)
                 self._vis_backends[name] = VISBACKENDS.build(vis_backend)
 
         self.fig_save = None
         self.fig_save_cfg = fig_save_cfg
```

### Comparing `mmengine-0.8.2/mmengine.egg-info/PKG-INFO` & `mmengine-0.8.3/mmengine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.2
+Version: 0.8.3
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -62,33 +62,49 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.8.0 was released on 2023-06-30.
+        v0.8.3 was released on 2023-07-31.
         
         Highlights:
         
+        - Support enabling `efficient_conv_bn_eval` for efficient convolution and batch normalization. See [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#save-memory-on-gpu) for more details
+        
+        - Add an [example](./examples/llama2/) to finetune Llama2.
+        
         - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for more detailed usages.
         
         - Introduce the pure Python style configuration file:
         
           - Support navigating to base configuration file in IDE
           - Support navigating to base variable in IDE
           - Support navigating to source code of class in IDE
           - Support inheriting two configuration files containing the same field
           - Load the configuration file without other third-party requirements
         
           Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
         
           ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
         
-        Read [Changelog](./docs/en/notes/changelog.md#v080-06302023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v083-07312023) for more details.
+        
+        ## Table of Contents
+        
+        - [Introduction](#introduction)
+        - [Installation](#installation)
+        - [Get Started](#get-started)
+        - [Learn More](#learn-more)
+        - [Contributing](#contributing)
+        - [Citation](#citation)
+        - [License](#license)
+        - [Ecosystem](#ecosystem)
+        - [Projects in OpenMMLab](#projects-in-openmmlab)
         
         ## Introduction
         
         MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
         
         Major features:
         
@@ -104,14 +120,16 @@
         
         3. **Customizable training process**:
         
            - Defines the training process just like playing with Legos.
            - Provides rich components and strategies.
            - Complete controls on the training process with different levels of APIs.
         
+        ![mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/267db9cb-72e4-4af2-a58b-877b30091acc)
+        
         ## Installation
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
         
         ```bash
@@ -344,14 +362,18 @@
         }
         ```
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE).
         
+        ## Ecosystem
+        
+        - [APES: Attention-based Point Cloud Edge Sampling](https://github.com/JunweiZheng93/APES)
+        
         ## Projects in OpenMMLab
         
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
         - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
         - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.2 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.3 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
@@ -17,62 +17,71 @@
    badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
 mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
      ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## What's New v0.8.0 was released on 2023-06-30. Highlights: - Support training
-with [FSDP](https://pytorch.org/tutorials/intermediate/
-FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://
-www.deepspeed.ai/). Refer to the [Training Large Models](https://
-mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for
-more detailed usages. - Introduce the pure Python style configuration file: -
-Support navigating to base configuration file in IDE - Support navigating to
-base variable in IDE - Support navigating to source code of class in IDE -
-Support inheriting two configuration files containing the same field - Load the
-configuration file without other third-party requirements Refer to the
-[tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/
-config.html#a-pure-python-style-configuration-file-beta) for more detailed
-usages. ![new-config-en](https://github.com/open-mmlab/mmengine/assets/
-57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1) Read [Changelog](./docs/en/
-notes/changelog.md#v080-06302023) for more details. ## Introduction MMEngine is
-a foundational library for training deep learning models based on PyTorch. It
-provides a solid engineering foundation and frees developers from writing
-redundant codes on workflows. It serves as the training engine of all OpenMMLab
-codebases, which support hundreds of algorithms in various research areas.
-Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
-Major features: 1. **A universal and powerful runner**: - Supports training
-different tasks with a small amount of code, e.g., ImageNet can be trained with
-only 80 lines of code (400 lines of the original PyTorch example). - Easily
-compatible with models from popular algorithm libraries such as TIMM,
+## What's New v0.8.3 was released on 2023-07-31. Highlights: - Support enabling
+`efficient_conv_bn_eval` for efficient convolution and batch normalization. See
+[save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/
+save_gpu_memory.html#save-memory-on-gpu) for more details - Add an [example](./
+examples/llama2/) to finetune Llama2. - Support training with [FSDP](https://
+pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp)
+and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large
+Models](https://mmengine.readthedocs.io/en/latest/common_usage/
+large_model_training.html) for more detailed usages. - Introduce the pure
+Python style configuration file: - Support navigating to base configuration
+file in IDE - Support navigating to base variable in IDE - Support navigating
+to source code of class in IDE - Support inheriting two configuration files
+containing the same field - Load the configuration file without other third-
+party requirements Refer to the [tutorial](https://mmengine.readthedocs.io/en/
+latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
+beta) for more detailed usages. ![new-config-en](https://github.com/open-mmlab/
+mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1) Read [Changelog]
+(./docs/en/notes/changelog.md#v083-07312023) for more details. ## Table of
+Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
+Started](#get-started) - [Learn More](#learn-more) - [Contributing]
+(#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
+(#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
+MMEngine is a foundational library for training deep learning models based on
+PyTorch. It provides a solid engineering foundation and frees developers from
+writing redundant codes on workflows. It serves as the training engine of all
+OpenMMLab codebases, which support hundreds of algorithms in various research
+areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab
+projects. Major features: 1. **A universal and powerful runner**: - Supports
+training different tasks with a small amount of code, e.g., ImageNet can be
+trained with only 80 lines of code (400 lines of the original PyTorch example).
+- Easily compatible with models from popular algorithm libraries such as TIMM,
 TorchVision, and Detectron2. 2. **Open architecture with unified interfaces**:
 - Handles different algorithm tasks with unified APIs, e.g., implement a method
 and apply it to all compatible models. - Provides a unified abstraction for
 upper-level algorithm libraries, which supports various back-end devices such
 as Nvidia CUDA, Mac MPS, AMD, MLU, and more for model training. 3.
 **Customizable training process**: - Defines the training process just like
 playing with Legos. - Provides rich components and strategies. - Complete
-controls on the training process with different levels of APIs. ## Installation
-Before installing MMEngine, please ensure that PyTorch has been successfully
-installed following the [official guide](https://pytorch.org/get-started/
-locally/). Install MMEngine ```bash pip install -U openmim mim install mmengine
-``` Verify the installation ```bash python -c 'from mmengine.utils.dl_utils
-import collect_env;print(collect_env())' ``` ## Get Started Taking the training
-of a ResNet-50 model on the CIFAR-10 dataset as an example, we will use
-MMEngine to build a complete, configurable training and validation process in
-less than 80 lines of code.  Build Models First, we need to define a **model**
-which 1) inherits from `BaseModel` and 2) accepts an additional argument `mode`
-in the `forward` method, in addition to those arguments related to the dataset.
-- During training, the value of `mode` is "loss", and the `forward` method
-should return a `dict` containing the key "loss". - During validation, the
-value of `mode` is "predict", and the forward method should return results
-containing both predictions and labels. ```python import torch.nn.functional as
-F import torchvision from mmengine.model import BaseModel class MMResNet50
-(BaseModel): def __init__(self): super().__init__() self.resnet =
+controls on the training process with different levels of APIs. !
+[mmengine_dataflow](https://github.com/open-mmlab/mmengine/assets/58739961/
+267db9cb-72e4-4af2-a58b-877b30091acc) ## Installation Before installing
+MMEngine, please ensure that PyTorch has been successfully installed following
+the [official guide](https://pytorch.org/get-started/locally/). Install
+MMEngine ```bash pip install -U openmim mim install mmengine ``` Verify the
+installation ```bash python -c 'from mmengine.utils.dl_utils import
+collect_env;print(collect_env())' ``` ## Get Started Taking the training of a
+ResNet-50 model on the CIFAR-10 dataset as an example, we will use MMEngine to
+build a complete, configurable training and validation process in less than 80
+lines of code.  Build Models First, we need to define a **model** which 1)
+inherits from `BaseModel` and 2) accepts an additional argument `mode` in the
+`forward` method, in addition to those arguments related to the dataset. -
+During training, the value of `mode` is "loss", and the `forward` method should
+return a `dict` containing the key "loss". - During validation, the value of
+`mode` is "predict", and the forward method should return results containing
+both predictions and labels. ```python import torch.nn.functional as F import
+torchvision from mmengine.model import BaseModel class MMResNet50(BaseModel):
+def __init__(self): super().__init__() self.resnet =
 torchvision.models.resnet50() def forward(self, imgs, labels, mode): x =
 self.resnet(imgs) if mode == 'loss': return {'loss': F.cross_entropy(x,
 labels)} elif mode == 'predict': return x, labels ```   Build Datasets Next, we
 need to create **Dataset**s and **DataLoader**s for training and validation. In
 this case, we simply use built-in datasets supported in TorchVision. ```python
 import torchvision.transforms as transforms from torch.utils.data import
 DataLoader norm_cfg = dict(mean=[0.491, 0.482, 0.447], std=[0.202, 0.199,
@@ -154,46 +163,47 @@
 Contributing We appreciate all contributions to improve MMEngine. Please refer
 to [CONTRIBUTING.md](CONTRIBUTING.md) for the contributing guideline. ##
 Citation If you find this project useful in your research, please consider
 cite: ``` @article{mmengine2022, title = {{MMEngine}: OpenMMLab Foundational
 Library for Training Deep Learning Models}, author = {MMEngine Contributors},
 howpublished = {\url{https://github.com/open-mmlab/mmengine}}, year={2022} }
 ``` ## License This project is released under the [Apache 2.0 license]
-(LICENSE). ## Projects in OpenMMLab - [MIM](https://github.com/open-mmlab/mim):
-MIM installs OpenMMLab packages. - [MMCV](https://github.com/open-mmlab/mmcv):
-OpenMMLab foundational library for computer vision. - [MMEval](https://
-github.com/open-mmlab/mmeval): A unified evaluation library for multiple
-machine learning libraries. - [MMPreTrain](https://github.com/open-mmlab/
-mmpretrain): OpenMMLab pre-training toolbox and benchmark. - [MMagic](https://
-github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
-**I**ntelligent **C**reation toolbox. - [MMDetection](https://github.com/open-
-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark. - [MMYOLO]
-(https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and
-benchmark. - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d):
-OpenMMLab's next-generation platform for general 3D object detection. -
-[MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object
-detection toolbox and benchmark. - [MMTracking](https://github.com/open-mmlab/
-mmtracking): OpenMMLab video perception toolbox and benchmark. - [MMPose]
-(https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and
-benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
-OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR](https://
-github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and
-understanding toolbox. - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d):
-OpenMMLab 3D human parametric model toolbox and benchmark. - [MMSelfSup](https:
-//github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox
-and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
-OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
-github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
-understanding toolbox and benchmark. - [MMFlow](https://github.com/open-mmlab/
-mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework. -
-[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
-toolbox and benchmark. - [Playground](https://github.com/open-mmlab/
-playground): A central hub for gathering and showcasing amazing projects built
-upon OpenMMLab. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
+(LICENSE). ## Ecosystem - [APES: Attention-based Point Cloud Edge Sampling]
+(https://github.com/JunweiZheng93/APES) ## Projects in OpenMMLab - [MIM](https:
+//github.com/open-mmlab/mim): MIM installs OpenMMLab packages. - [MMCV](https:/
+/github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
+vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation
+library for multiple machine learning libraries. - [MMPreTrain](https://
+github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+benchmark. - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab
+**A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMYOLO](https://github.com/open-mmlab/mmyolo):
+OpenMMLab YOLO series toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
+general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
+mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video
+perception toolbox and benchmark. - [MMPose](https://github.com/open-mmlab/
+mmpose): OpenMMLab pose estimation toolbox and benchmark. - [MMSegmentation]
+(https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation
+toolbox and benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr):
+OpenMMLab text detection, recognition, and understanding toolbox. - [MMHuman3D]
+(https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model
+toolbox and benchmark. - [MMSelfSup](https://github.com/open-mmlab/mmselfsup):
+OpenMMLab self-supervised learning toolbox and benchmark. - [MMFewShot](https:/
+/github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and
+benchmark. - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's
+next-generation action understanding toolbox and benchmark. - [MMFlow](https://
+github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model
+compression toolbox and benchmark. - [Playground](https://github.com/open-
+mmlab/playground): A central hub for gathering and showcasing amazing projects
+built upon OpenMMLab. Platform: UNKNOWN Classifier: Development Status :: 4 -
+Beta Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Utilities Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests
```

### Comparing `mmengine-0.8.2/mmengine.egg-info/SOURCES.txt` & `mmengine-0.8.3/mmengine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 mmengine/logging/__init__.py
 mmengine/logging/history_buffer.py
 mmengine/logging/logger.py
 mmengine/logging/message_hub.py
 mmengine/model/__init__.py
 mmengine/model/averaged_model.py
 mmengine/model/base_module.py
+mmengine/model/efficient_conv_bn_eval.py
 mmengine/model/test_time_aug.py
 mmengine/model/utils.py
 mmengine/model/weight_init.py
 mmengine/model/base_model/__init__.py
 mmengine/model/base_model/base_model.py
 mmengine/model/base_model/data_preprocessor.py
 mmengine/model/wrappers/__init__.py
```

### Comparing `mmengine-0.8.2/setup.py` & `mmengine-0.8.3/setup.py`

 * *Files identical despite different names*

