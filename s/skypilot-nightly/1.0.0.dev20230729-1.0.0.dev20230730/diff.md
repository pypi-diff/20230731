# Comparing `tmp/skypilot-nightly-1.0.0.dev20230729.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230730.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230729.tar", last modified: Sat Jul 29 10:40:49 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230730.tar", last modified: Sun Jul 30 10:41:05 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230729.tar` & `skypilot-nightly-1.0.0.dev20230730.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.510635 skypilot-nightly-1.0.0.dev20230729/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-29 10:40:49.510635 skypilot-nightly-1.0.0.dev20230729/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:40:49.510635 skypilot-nightly-1.0.0.dev20230729/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-29 10:40:41.000000 skypilot-nightly-1.0.0.dev20230729/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.486635 skypilot-nightly-1.0.0.dev20230729/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-29 10:40:41.000000 skypilot-nightly-1.0.0.dev20230729/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.486635 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.490635 skypilot-nightly-1.0.0.dev20230729/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   114556 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   202355 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.490635 skypilot-nightly-1.0.0.dev20230729/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.490635 skypilot-nightly-1.0.0.dev20230729/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   168663 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.490635 skypilot-nightly-1.0.0.dev20230729/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    46013 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    90575 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.494635 skypilot-nightly-1.0.0.dev20230729/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-29 10:40:41.000000 skypilot-nightly-1.0.0.dev20230729/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.498635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.482635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.498635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.498635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.498635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.498635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.498635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.502635 skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.506635 skypilot-nightly-1.0.0.dev20230729/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.506635 skypilot-nightly-1.0.0.dev20230729/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.506635 skypilot-nightly-1.0.0.dev20230729/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.506635 skypilot-nightly-1.0.0.dev20230729/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.510635 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-29 10:40:49.000000 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-29 10:40:49.000000 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:40:49.000000 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 10:40:49.000000 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-29 10:40:49.000000 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-29 10:40:49.000000 skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:40:49.510635 skypilot-nightly-1.0.0.dev20230729/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   135092 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:40:36.000000 skypilot-nightly-1.0.0.dev20230729/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.012346 skypilot-nightly-1.0.0.dev20230730/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-30 10:41:05.012346 skypilot-nightly-1.0.0.dev20230730/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 10:41:05.012346 skypilot-nightly-1.0.0.dev20230730/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-30 10:40:56.000000 skypilot-nightly-1.0.0.dev20230730/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.984346 skypilot-nightly-1.0.0.dev20230730/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-30 10:40:56.000000 skypilot-nightly-1.0.0.dev20230730/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.984346 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.988346 skypilot-nightly-1.0.0.dev20230730/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114556 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202355 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.988346 skypilot-nightly-1.0.0.dev20230730/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.988346 skypilot-nightly-1.0.0.dev20230730/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168663 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.988346 skypilot-nightly-1.0.0.dev20230730/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46013 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.992346 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.992346 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.992346 skypilot-nightly-1.0.0.dev20230730/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90575 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.992346 skypilot-nightly-1.0.0.dev20230730/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.992346 skypilot-nightly-1.0.0.dev20230730/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.992346 skypilot-nightly-1.0.0.dev20230730/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.996346 skypilot-nightly-1.0.0.dev20230730/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-30 10:40:56.000000 skypilot-nightly-1.0.0.dev20230730/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.996346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.980346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.996346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.996346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:04.996346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.000346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.000346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.000346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.000346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.000346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.004346 skypilot-nightly-1.0.0.dev20230730/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.008346 skypilot-nightly-1.0.0.dev20230730/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.008346 skypilot-nightly-1.0.0.dev20230730/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.008346 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-30 10:41:04.000000 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-30 10:41:04.000000 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:41:04.000000 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 10:41:04.000000 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-30 10:41:04.000000 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-30 10:41:04.000000 skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:41:05.012346 skypilot-nightly-1.0.0.dev20230730/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135092 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 10:40:53.000000 skypilot-nightly-1.0.0.dev20230730/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230729/LICENSE` & `skypilot-nightly-1.0.0.dev20230730/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230730/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230730/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230729
+Version: 1.0.0.dev20230730
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230729
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230730
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230729/README.md` & `skypilot-nightly-1.0.0.dev20230730/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230730/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/setup.py` & `skypilot-nightly-1.0.0.dev20230730/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230730/sky/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
 __commit__ = 'b1569519e06778e28b3d8803b37ff439d44afd71'
-__version__ = '1.0.0-dev20230729'
+__version__ = '1.0.0-dev20230730'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230730/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230730/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230730/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/check.py` & `skypilot-nightly-1.0.0.dev20230730/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230730/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230730/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230730/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/core.py` & `skypilot-nightly-1.0.0.dev20230730/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230730/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230730/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230730/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230730/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230730/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230730/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230730/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230730/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230730/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230730/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230730/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230730/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230730/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230730/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230730/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230730/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/task.py` & `skypilot-nightly-1.0.0.dev20230730/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230730/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230730/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230730/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230730/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230729
+Version: 1.0.0.dev20230730
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230729
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230730
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230730/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230729/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230730/tests/test_wheels.py`

 * *Files identical despite different names*

