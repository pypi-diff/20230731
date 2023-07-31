# Comparing `tmp/fiddler-client-2.0.0.dev7.tar.gz` & `tmp/fiddler-client-2.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-2.0.0.dev7.tar", last modified: Thu Jul 27 12:35:18 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev8.tar", last modified: Mon Jul 31 16:37:49 2023, max compression
```

## Comparing `fiddler-client-2.0.0.dev7.tar` & `fiddler-client-2.0.0.dev8.tar`

### file list

```diff
@@ -1,123 +1,115 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    16868 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)     1725 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1822 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   112950 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2490 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6439 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/libs/http_client.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/template_model.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/schemas/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1535 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1124 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1000) docker    (1001)      642 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1000) docker    (1001)      679 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1000) docker    (1001)      313 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/xai_params.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4399 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      782 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      189 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5493 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/pandas_helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16477 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4254 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9825 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1316 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/compatibility_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17012 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    22117 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15338 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9611 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/infer_schema_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4538 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8271 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4160 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    24244 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3210 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/project_mixin.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4630 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      490 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3048 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      882 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      504 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1107 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4230 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/compatibility_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3616 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2564 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1818 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1936 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/validators/dataset_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     3036 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1274 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/tests/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/tests/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1473 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/test_general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8079 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/test_pandas.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1800 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/tests_utils.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3252 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/test_infer_model_schema.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5346 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/test_object_inference.py
--rw-r--r--   0 runner    (1000) docker    (1001)      280 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/utils.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/tests/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1421 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1785 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3793 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_add_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)    32093 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)    10273 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)      912 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_check_version_decorator.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3028 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_custom_features.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6301 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_dataset_api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7654 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_events_api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2804 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15104 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_explainability_apis.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7556 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_file_upload.py
--rw-r--r--   0 runner    (1000) docker    (1001)      826 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4606 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_job.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7390 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6546 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_project.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2964 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13744 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_upload_dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      584 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    16868 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.860216 fiddler-client-2.0.0.dev8/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)     1476 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16916 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4187 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9813 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1313 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/compatibility_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16963 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    22076 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15332 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9792 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/generate_schema_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4722 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4496 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4118 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21054 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3198 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/project_mixin.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1822 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   112950 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2490 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/exceptions.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6439 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/libs/http_client.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/template_model.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4493 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      343 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      487 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3045 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      879 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      501 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1104 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      121 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      388 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler/schemas/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1535 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1124 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      642 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      679 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      313 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/xai_params.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4399 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4284 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/compatibility_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3613 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2561 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      189 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5493 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/pandas_helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1818 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15839 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/semver_version.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1933 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/validators/dataset_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2927 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      144 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1250 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/tests/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1418 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1785 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3787 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_add_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    36786 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    10277 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      906 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_check_version_decorator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3028 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_custom_features.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6307 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_dataset_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7718 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_events_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2801 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15111 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_explainability_apis.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7611 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_file_upload.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3256 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_generate_schema.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      820 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4608 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7397 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6548 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2958 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13719 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_upload_dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      581 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/tests/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1473 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8084 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_pandas.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1800 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/tests_utils.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5346 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/test_object_inference.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      280 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/utils.py
```

### Comparing `fiddler-client-2.0.0.dev7/PKG-INFO` & `fiddler-client-2.0.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev7
+Version: 2.0.0.dev8
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
```

### Comparing `fiddler-client-2.0.0.dev7/PUBLIC.md` & `fiddler-client-2.0.0.dev8/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/README.md` & `fiddler-client-2.0.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/__init__.py` & `fiddler-client-2.0.0.dev8/fiddler/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 A Python client for Fiddler service.
 
 TODO: Add Licence.
 """
 
 from fiddler import utils
 from fiddler._version import __version__
+from fiddler.api import FiddlerApi, FiddlerClient
 from fiddler.constants import CSV_EXTENSION
 from fiddler.core_objects import (
     ArtifactStatus,
     BaselineType,
     BatchPublishType,
     Column,
     DatasetInfo,
@@ -24,36 +25,21 @@
     ModelInfo,
     ModelInputType,
     ModelTask,
     WeightingParams,
     WindowSize,
 )
 from fiddler.packtools import gem
-from fiddler.schemas.custom_features import Multivariate, TextEmbedding
-from fiddler.utils import logger
+from fiddler.schemas.custom_features import Multivariate, TextEmbedding, ImageEmbedding
+from fiddler.utils import logger, ColorLogger
 from fiddler.utils.validator import (
     PackageValidator,
     ValidationChainSettings,
     ValidationModule,
 )
-from fiddler.v2.api.api import FiddlerApi, FiddlerClient
-from fiddler.v2.api.explainability_mixin import (
-    DatasetDataSource,
-    RowDataSource,
-    SqlSliceQueryDataSource,
-)
-from fiddler.v2.schema.alert import (
-    AlertCondition,
-    AlertType,
-    BinSize,
-    ComparePeriod,
-    CompareTo,
-    Metric,
-    Priority,
-)
 
 logger = logger.get_logger(__name__)
 
 SUPPORTED_API_VERSIONS = ['v2']
 
 
 __all__ = [
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev8/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/constants.py` & `fiddler-client-2.0.0.dev8/fiddler/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev8/fiddler/core_objects.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/exceptions.py` & `fiddler-client-2.0.0.dev8/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/libs/http_client.py` & `fiddler-client-2.0.0.dev8/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev8/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev8/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev8/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev8/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/schemas/custom_features.py` & `fiddler-client-2.0.0.dev8/fiddler/schemas/custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/schemas/model_schema.py` & `fiddler-client-2.0.0.dev8/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/schemas/model_spec.py` & `fiddler-client-2.0.0.dev8/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/schemas/model_task_params.py` & `fiddler-client-2.0.0.dev8/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/utils/pandas_helper.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/utils/validator.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/alert_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/alert_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,82 +1,84 @@
+from __future__ import annotations
+
 import json
 from datetime import datetime, timedelta
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import parse_obj_as
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils.logger import get_logger
-from fiddler.v2.schema.alert import (
+from fiddler.schema.alert import (
     AlertCondition,
     AlertRule,
     AlertRulePayload,
     AlertType,
     BinSize,
     ComparePeriod,
     CompareTo,
     Metric,
     Priority,
     TriggeredAlerts,
 )
-from fiddler.v2.utils.compatibility_helpers import project_id_compat, model_id_compat
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.helpers import match_semver
-from fiddler.v2.utils.response_handler import (
+from fiddler.utils.compatibility_helpers import project_id_compat, model_id_compat
+from fiddler.utils.decorators import handle_api_error_response
+from fiddler.utils.helpers import match_semver
+from fiddler.utils.logger import get_logger
+from fiddler.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = get_logger(__name__)
 
 
 class AlertMixin:
     FILTER_ALERT_RULES_API_VERSION = '>=23.1.0'
     GROUP_OF_COLUMNS_API_VERSION = '>=23.3.0'
+    RULE_V3_API_VERSION = '>=23.4.0'
 
     client: RequestClient
     organization_name: str
 
     @handle_api_error_response
     def add_alert_rule(
         self,
         name: str,
+        metric: Union[Metric, str],
+        compare_to: CompareTo,
+        priority: Priority,
+        critical_threshold: float,
+        condition: AlertCondition,
         project_id: str = None,
         model_id: str = None,
-        alert_type: AlertType = None,
-        metric: Metric = None,
-        compare_to: CompareTo = None,
-        priority: Priority = None,
-        critical_threshold: float = None,
-        condition: AlertCondition = None,
         bin_size: BinSize = BinSize.ONE_DAY,
+        alert_type: Optional[AlertType] = None,
         baseline_name: Optional[str] = None,
         compare_period: Optional[ComparePeriod] = None,
         columns: Optional[List[str]] = None,
         warning_threshold: Optional[float] = None,
         project_name: str = None,
         model_name: str = None,
         notifications_config: Optional[Dict[str, Any]] = None,
     ) -> AlertRule:
-        """
+        f"""
         To add an alert rule
 
         :param project_id: Unique project name for which the alert rule is created
         :param model_id: Unique model name for which the alert rule is created
         :param project_name: Unique project name for which the alert rule is created
         :param model_name: Unique model name for which the alert rule is created
         :param name: Name of the Alert rule
-        :param alert_type: Selects one of the four metric types:
-                1) AlertType.PERFORMANCE
-                2) AlertType.DATA_DRIFT
-                3) AlertType.DATA_INTEGRITY
-                4) AlertType.SERVICE_METRICS
-
-
-        :param metric: "metric":
+        :param alert_type: [DEPRECATED] Used only for older server versions. For {self.RULE_V3_API_VERSION} you can simply use 'metric'. 
+            Selects one of the four metric types:
+                    1) AlertType.PERFORMANCE
+                    2) AlertType.DATA_DRIFT
+                    3) AlertType.DATA_INTEGRITY
+                    4) AlertType.SERVICE_METRICS
+        :param metric: can be a string or MetricType enum.
                 For service_metrics:
                 1) MetricType.TRAFFIC
 
                 For performance:
                 1)  For binary_classfication:
                         a) MetricType.ACCURACY b) MetricType.TPR c) MetricType.FPR d) MetricType.PRECISION e) MetricType.RECALL
                         f) MetricType.F1_SCORE g) MetricType.ECE h) MetricType.AUC
@@ -120,27 +122,14 @@
                 2) AlertCondition.GREATER
         :param columns: List of column names on which alert rule is to be created. It can take ['__ANY__'] to check for all columns
         :param notifications_config: notifications config object created using helper method build_notifications_config()
         :param baseline_name: Name of the baselne, whose histogram is compared against the same derived from current data.
                             Used only when alert type is AlertType.DATA_DRIFT.
         :return: created alert rule object
         """
-        required_params = [
-            'alert_type',
-            'metric',
-            'compare_to',
-            'priority',
-            'critical_threshold',
-            'condition',
-        ]
-        if any(param is None for param in required_params):
-            raise TypeError(
-                f'Please make sure {", ".join(required_params)} params are passed'
-            )
-
         if columns and not match_semver(
             self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION
         ):
             raise ValueError(
                 f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}'
             )
 
@@ -168,23 +157,25 @@
         request_body = AlertRulePayload(
             organization_name=self.organization_name,
             project_name=project_name,
             model_name=model_name,
             name=name,
             alert_type=alert_type,
             metric=metric,
+            metric_id=metric,
             compare_to=compare_to,
             compare_period=compare_period,
             priority=priority,
             baseline_name=baseline_name,
             feature_names=columns,
             warning_threshold=warning_threshold,
             critical_threshold=critical_threshold,
             condition=condition,
-            time_bucket=bin_size,
+            time_bucket=bin_size.value[0],
+            bin_size=bin_size.value[1],
             notifications=notifications_config,
         ).dict()
         response = self.client.post(
             url='alert-configs',
             data=request_body,
         )
         response_data = APIResponseHandler(response)
@@ -209,38 +200,37 @@
 
     @handle_api_error_response
     def get_alert_rules(
         self,
         project_id: Optional[str] = None,
         model_id: Optional[str] = None,
         alert_type: Optional[AlertType] = None,
-        metric: Optional[Metric] = None,
+        metrics: Optional[List[Metric]] = None,
         columns: Optional[List[str]] = None,
         baseline_name: Optional[str] = None,
         ordering: Optional[List[str]] = None,
         offset: int = 0,
         limit: int = 20,
         project_name: Optional[str] = None,
         model_name: Optional[str] = None,
     ) -> List[AlertRule]:
-        """
+        f"""
         Get a list of alert rules with respect to the filtering parameters
 
         :param project_id: Unique project name for which the alert rule is created
         :param model_id: Unique model name for which the alert rule is created
         :param project_name: unique project name
         :param model_name: unique model name
-        :param alert_type: Selects one of the four metric types:
+        :param alert_type: [DEPRECATED] Used only for older server versions. For {self.RULE_V3_API_VERSION} you can simply use 'metrics'. 
+            Selects one of the four metric types:
                 1) AlertType.PERFORMANCE
                 2) AlertType.DATA_DRIFT
                 3) AlertType.DATA_INTEGRITY
                 4) AlertType.SERVICE_METRICS
-
-
-        :param metric: "metric":
+        :param metrics: can be a list of strings or MetricTypes that specify metrics you want to retrieve.:
                 For service_metrics:
                 1) MetricType.TRAFFIC
 
                 For performance:
                 1)  For binary_classfication:
                         a) MetricType.ACCURACY b) MetricType.TPR c) MetricType.FPR d) MetricType.PRECISION e) MetricType.RECALL
                         f) MetricType.F1_SCORE g) MetricType.ECE h) MetricType.AUC
@@ -303,23 +293,28 @@
                 )
 
             if model_name:
                 filter_by_rules.append(
                     {'field': 'model_name', 'operator': 'equal', 'value': model_name}
                 )
 
-            if alert_type:
-                filter_by_rules.append(
-                    {'field': 'alert_type', 'operator': 'equal', 'value': alert_type}
-                )
+            if metrics:
+                if match_semver(self.server_info.server_version, self.RULE_V3_API_VERSION):
+                    filter_by_rules.append(
+                        {'field': 'metric_id', 'operator': 'contains', 'value': metrics}
+                    )
+                else:
+                    if alert_type:
+                        filter_by_rules.append(
+                            {'field': 'alert_type', 'operator': 'equal', 'value': alert_type}
+                        )
+                    filter_by_rules.append(
+                        {'field': 'metric', 'operator': 'equal', 'value': metrics[0]}
+                    )
 
-            if metric:
-                filter_by_rules.append(
-                    {'field': 'metric', 'operator': 'equal', 'value': metric}
-                )
 
             if columns:
                 filter_by_rules.append(
                     {'field': 'feature_names', 'operator': 'contains', 'value': columns}
                 )
 
             if baseline_name:
@@ -339,15 +334,15 @@
             )
         else:
             alert_params.update(
                 {
                     'project_name': project_name,
                     'model_name': model_name,
                     'alert_type': alert_type,
-                    'metric': metric,
+                    'metric': metrics[0] if metrics else None,
                     'baseline_name': baseline_name,
                     'ordering': ordering,
                 }
             )
 
         response = self.client.get(
             url='alert-configs',
@@ -404,17 +399,17 @@
         To get the notifications value to be set for alert rule
         :param emails: Comma separated emails list
         :param pagerduty_services: Comma separated pagerduty services list
         :param pagerduty severity: Severity for the alerts triggered by pagerduty
         :param webhooks: List of webhook uuids, on which we need notification
         :return: dict with emails and pagerduty dict. If left unused, will store empty string for these values
         """
-        webhooks_dict: list[dict[str, str]] = []
-        for webhook_uuid in webhooks:
-            webhooks_dict.append({'uuid': webhook_uuid})
+        webhooks_dict: list[dict[str, str]] = [
+            {'uuid': webhook_uuid} for webhook_uuid in webhooks
+        ]
 
         return {
             'emails': {
                 'email': emails,
             },
             'pagerduty': {
                 'service': pagerduty_services,
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/api.py` & `fiddler-client-2.0.0.dev8/fiddler/api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import warnings
 from typing import Optional
 from urllib.parse import urljoin
 
 from fiddler._version import __version__
+from fiddler.api.alert_mixin import AlertMixin
+from fiddler.api.baseline_mixin import BaselineMixin
+# @todo: This is v1 implementation needs to have a proper v2 approach
+from fiddler.api.compatibility_mixin import CompatibilityMixin
+from fiddler.api.dataset_mixin import DatasetMixin
+from fiddler.api.events_mixin import EventsMixin
+from fiddler.api.explainability_mixin import ExplainabilityMixin
+from fiddler.api.generate_schema_mixin import GenerateSchemaMixin
+from fiddler.api.job_mixin import JobMixin
+from fiddler.api.model_deployment_mixin import ModelDeploymentMixin
+from fiddler.api.model_mixin import ModelMixin
+from fiddler.api.project_mixin import ProjectMixin
 from fiddler.constants import (
     CURRENT_API_VERSION,
     FIDDLER_CLIENT_VERSION_HEADER,
     MIN_SERVER_VERSION,
 )
 from fiddler.libs.http_client import RequestClient
+from fiddler.schema.server_info import ServerInfo
+from fiddler.utils.decorators import handle_api_error_response
+from fiddler.utils.helpers import match_semver, raise_not_supported
 from fiddler.utils.logger import get_logger
-from fiddler.v2.api.alert_mixin import AlertMixin
-from fiddler.v2.api.baseline_mixin import BaselineMixin
-# @todo: This is v1 implementation needs to have a proper v2 approach
-from fiddler.v2.api.compatibility_mixin import CompatibilityMixin
-from fiddler.v2.api.dataset_mixin import DatasetMixin
-from fiddler.v2.api.events_mixin import EventsMixin
-from fiddler.v2.api.explainability_mixin import ExplainabilityMixin
-from fiddler.v2.api.infer_schema_mixin import InferModelSchemaMixin
-from fiddler.v2.api.job_mixin import JobMixin
-from fiddler.v2.api.model_deployment_mixin import ModelDeploymentMixin
-from fiddler.v2.api.model_mixin import ModelMixin
-from fiddler.v2.api.project_mixin import ProjectMixin
-from fiddler.v2.schema.server_info import ServerInfo
-from fiddler.v2.utils.helpers import match_semver, raise_not_supported
-from fiddler.v2.utils.decorators import handle_api_error_response
 
 logger = get_logger(__name__)
 
 
 class FiddlerClient(
     ModelMixin,
     CompatibilityMixin,
@@ -36,15 +36,15 @@
     ProjectMixin,
     EventsMixin,
     JobMixin,
     BaselineMixin,
     AlertMixin,
     ExplainabilityMixin,
     ModelDeploymentMixin,
-    InferModelSchemaMixin,
+    GenerateSchemaMixin,
 ):
     def __init__(
         self,
         url: Optional[str] = None,
         org_id: Optional[str] = None,
         auth_token: Optional[str] = None,
         proxies: Optional[dict] = None,
@@ -72,24 +72,24 @@
         if all(value is not None for value in duplicated_params):
             raise ValueError('Pass either org_id or organization_name')
         if all(value is None for value in duplicated_params):
             raise ValueError('Pass either org_id or organization_name')
         self.organization_name = organization_name
         if org_id:
             warnings.warn(
-                f'WARNING: org_id is deprecated and will be removed from future \
-                        versions. Please use organization_name',
+                'WARNING: org_id is deprecated and will be removed from future '
+                'versions. Please use organization_name',
                 FutureWarning,
             )
 
             self.organization_name = org_id
 
         self.server_info: ServerInfo = self._get_server_info()
         self._check_server_version()
-        
+
         # Checks client's version compatibility with server
         self._check_version_compatibility()
 
     def _get_server_info(self) -> ServerInfo:
         response = self.client.get(
             url='server-info',
             params={'organization_name': self.organization_name},
@@ -103,15 +103,15 @@
             'client_version': __version__,
             'client_name': 'python-sdk',
         }
         self.client.get(
             url='version-compatibility',
             params=params,
         )
-        
+
     def _check_server_version(self) -> None:
         if match_semver(self.server_info.server_version, f'>={MIN_SERVER_VERSION}'):
             return
 
         raise_not_supported(
             compatible_client_version='1.8',
             client_version=__version__,
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/baseline_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/baseline_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from http import HTTPStatus
 from typing import List
 
 from pydantic import parse_obj_as
 
 from fiddler.core_objects import BaselineType, WindowSize
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils.logger import get_logger
-from fiddler.v2.schema.baseline import Baseline
-from fiddler.v2.utils.compatibility_helpers import (
+from fiddler.schema.baseline import Baseline
+from fiddler.utils.compatibility_helpers import (
     project_id_compat,
     model_id_compat,
     baseline_id_compat,
 )
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.response_handler import (
+from fiddler.utils.decorators import handle_api_error_response
+from fiddler.utils.logger import get_logger
+from fiddler.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = get_logger(__name__)
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/compatibility_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/compatibility_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from deprecated import deprecated
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.v2.schema.project import Project
+from fiddler.schema.project import Project
 
 
 class CompatibilityMixin:
     client: RequestClient
     organization_name: str
 
     @deprecated(
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/dataset_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/dataset_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 from http import HTTPStatus
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
 import yaml
 
+from fiddler.api.helpers import multipart_upload
 from fiddler.constants import FileType, UploadType
 from fiddler.core_objects import DatasetInfo
 from fiddler.exceptions import HttpException
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils.logger import get_logger
-from fiddler.v2.api.helpers import multipart_upload
-from fiddler.v2.schema.dataset import Dataset, DatasetIngest
-from fiddler.v2.utils.compatibility_helpers import (
+from fiddler.schema.dataset import Dataset, DatasetIngest
+from fiddler.utils.compatibility_helpers import (
     project_id_compat,
     dataset_id_compat,
     dataset_compat,
 )
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.helpers import map_extension_to_file_type, match_semver
-from fiddler.v2.utils.response_handler import (
+from fiddler.utils.decorators import handle_api_error_response
+from fiddler.utils.helpers import match_semver
+from fiddler.utils.logger import get_logger
+from fiddler.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
-from fiddler.v2.validators.dataset_validator import (
+from fiddler.validators.dataset_validator import (
     validate_dataset_columns,
     validate_dataset_info,
     validate_dataset_shape,
 )
 
 DEFAULT_NROWS_PER_CHUNK = 100000
 DEFAULT_SAMPLE_SIZE = 20000
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/events_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/events_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 from http import HTTPStatus
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import pandas as pd
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
+from fiddler.api.helpers import multipart_upload
 from fiddler.constants import FiddlerTimestamp, FileType, UploadType
 from fiddler.core_objects import BatchPublishType
 from fiddler.exceptions import HttpException
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import get_logger
-from fiddler.utils import logger
-from fiddler.v2.api.helpers import multipart_upload
-from fiddler.v2.schema.events import EventIngest, EventsIngest
-from fiddler.v2.utils.compatibility_helpers import (
+from fiddler.schema.events import EventIngest, EventsIngest
+from fiddler.utils.compatibility_helpers import (
     project_id_compat,
     model_id_compat,
     update_event_compat,
 )
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.response_handler import APIResponseHandler
+from fiddler.utils.decorators import handle_api_error_response
+from fiddler.utils.logger import get_logger
+from fiddler.utils.response_handler import APIResponseHandler
 
 logger = get_logger(__name__)
 
 
 class EventsMixin:
     client: RequestClient
     organization_name: str
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/explainability_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections import namedtuple
 from typing import Dict, List, NamedTuple, Optional, Union
 
 import pandas as pd
 from pydantic import BaseModel
 
 from fiddler.libs.http_client import RequestClient
+from fiddler.utils.decorators import handle_api_error_response
 from fiddler.utils.logger import get_logger
 from fiddler.utils.pandas_helper import try_series_retype
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.response_handler import APIResponseHandler
+from fiddler.utils.response_handler import APIResponseHandler
 
 logger = get_logger(__name__)
 
 
 class DatasetDataSource(BaseModel):
     source_type = 'DATASET'
     dataset_name: str
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/helpers.py` & `fiddler-client-2.0.0.dev8/fiddler/api/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     CONTENT_TYPE_OCTET_STREAM_HEADER,
     MULTI_PART_CHUNK_SIZE,
     MULTI_PART_UPLOAD_SIZE_THRESHOLD,
     UploadType,
 )
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils.logger import get_logger
-from fiddler.v2.utils.response_handler import APIResponseHandler
+from fiddler.utils.response_handler import APIResponseHandler
 
 logger = get_logger(__name__)
 
 UPLOAD_ID_KEY = 'upload_id'
 UPLOAD_TYPE_KEY = 'upload_type'
 RESOURCE_IDENT_KEY = 'resource_identifier'
 FILE_NAME_KEY = 'file_name'
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/infer_schema_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/generate_schema_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,53 +3,53 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from pyarrow.parquet import ParquetFile
 
-from fiddler import DataType
+from fiddler.core_objects import DataType
 from fiddler.libs.http_client import RequestClient
 from fiddler.schemas.model_schema import Column, ModelSchema
-from fiddler.v2.utils.decorators import check_version, handle_api_error_response
-from fiddler.v2.utils.response_handler import APIResponseHandler
+from fiddler.utils.decorators import check_version, handle_api_error_response
+from fiddler.utils.response_handler import APIResponseHandler
 
 
-class InferModelSchemaMixin:
+class GenerateSchemaMixin:
     client: RequestClient
     organization_name: str
 
     @check_version(version_expr='>=23.4.0')
     @handle_api_error_response
-    def generate_model_schema(
+    def generate_schema(
         self,
         source: Union[pd.DataFrame, Path, List[Dict[str, Any]], str],
         max_cardinality: Optional[int] = None,
         sample_size: Optional[int] = None,
         enrich: bool = True,
     ) -> ModelSchema:
         """
         Generate model schema from the given data
         :param source: Data source - Dataframe or path to csv or parquet file.
         :param max_cardinality: Max cardinality to detect categorical columns
-        :param sample_size: No. if samples to use for inferring schema
+        :param sample_size: No. of samples to use for generating schema
         :param enrich: Enrich the model schema client side by scanning all data
         :return: Generated ModelSchema object
         """
-        schema_generator = InferSchemaFactory.create(
+        schema_generator = SchemaGeneratorFactory.create(
             source=source,
             max_cardinality=max_cardinality,
             sample_size=sample_size,
             enrich=enrich,
         )
 
-        return schema_generator.infer_schema(client=self.client)
+        return schema_generator.generate(client=self.client)
 
 
-class BaseInferSchema(ABC):
+class BaseSchemaGenerator(ABC):
     SAMPLE_SIZE = 10_000
     CHUNK_SIZE = 10_000
     BIN_SIZE = 10
     MAX_CARDINALITY = 1_000
 
     def __init__(
         self,
@@ -89,27 +89,27 @@
     @property
     def sample_size_per_chunk(self) -> int:
         """Number of samples per chunk"""
         return math.ceil(self.sample_size / self.num_chunks)
 
     @abstractmethod
     def sample_rows(self) -> pd.DataFrame:
-        """Data sample which will be used for inferring schema"""
+        """Data sample which will be used for generating schema"""
 
-    def infer_schema(self, client: RequestClient) -> ModelSchema:
-        """Call backend for inferring model schema"""
+    def generate(self, client: RequestClient) -> ModelSchema:
+        """Call backend for generating model schema"""
         request_body = {
             'rows': self.sample_rows(),
         }
 
         if self.max_cardinality is not None:
             request_body['max_cardinality'] = self.max_cardinality
 
         response = client.post(
-            url='infer-model-schema',
+            url='generate-schema',
             data=request_body,
         )
 
         data = APIResponseHandler(response).get_data()
 
         schema = ModelSchema(**data)
 
@@ -179,40 +179,40 @@
                 schema.columns[index] = self._enrich_categorical_column(
                     series=series, column=column
                 )
 
         return schema
 
 
-class CSVInferSchema(BaseInferSchema):
+class CSVSchemaGenerator(BaseSchemaGenerator):
     def __init__(self, source: Path, *args: Any, **kwargs: Any) -> None:
         super().__init__(source, *args, **kwargs)
 
     def _get_num_rows(self) -> int:
         # Num of rows excluding header
         return sum(1 for _ in open(self.source)) - 1
 
     def sample_rows(self) -> List[Dict]:
         df = pd.concat(
             [
                 chunk.sample(self.sample_size_per_chunk)
                 for chunk in pd.read_csv(
-                    self.source, chunksize=self.CHUNK_SIZE, dtype='object'
+                    self.source, chunksize=self.CHUNK_SIZE, dtype='str'
                 )
             ]
         )
 
         return df.to_dict(orient='records')
 
     def get_series(self, col_name: str) -> pd.Series:
         df = pd.read_csv(self.source, usecols=[col_name])
         return df[col_name]
 
 
-class ParquetInferSchema(BaseInferSchema):
+class ParquetSchemaGenerator(BaseSchemaGenerator):
     def __init__(self, source: Path, *args: Any, **kwargs: Any) -> None:
         super().__init__(source, *args, **kwargs)
 
         self.parquet_file = ParquetFile(self.source)
 
     def _get_num_rows(self) -> int:
         return self.parquet_file.scan_contents(batch_size=self.CHUNK_SIZE)
@@ -220,36 +220,38 @@
     def sample_rows(self) -> List[Dict]:
         df = pd.concat(
             [
                 batch.to_pandas().sample(self.sample_size_per_chunk)
                 for batch in self.parquet_file.iter_batches()
             ]
         )
-        return df.to_dict(orient='records')
+        return df.astype('str').to_dict(orient='records')
 
     def get_series(self, col_name: str) -> pd.Series:
         df = pd.read_parquet(self.source, columns=[col_name])
         return df[col_name]
 
 
-class DataframeInferSchema(BaseInferSchema):
+class DataframeSchemaGenerator(BaseSchemaGenerator):
     def __init__(self, source: pd.DataFrame, *args: Any, **kwargs: Any) -> None:
         super().__init__(source, *args, **kwargs)
 
     def _get_num_rows(self) -> int:
         return self.source.shape[0]
 
     def sample_rows(self) -> List[Dict]:
-        return self.source.sample(self.sample_size).to_dict(orient='records')
+        return (
+            self.source.sample(self.sample_size).astype('str').to_dict(orient='records')
+        )
 
     def get_series(self, col_name: str) -> pd.Series:
         return self.source[col_name]
 
 
-class ListInferSchema(BaseInferSchema):
+class ListSchemaGenerator(BaseSchemaGenerator):
     def __init__(self, source: List[Dict[str, Any]], *args: Any, **kwargs: Any) -> None:
         super().__init__(source, *args, **kwargs)
 
     def _get_num_rows(self) -> int:
         return len(self.source)
 
     def sample_rows(self) -> List[Dict]:
@@ -261,39 +263,39 @@
     ) -> ModelSchema:
         return schema
 
     def get_series(self, col_name: str) -> pd.Series:
         raise NotImplementedError
 
 
-class InferSchemaFactory:
+class SchemaGeneratorFactory:
     @staticmethod
     def create(
         source: Union[pd.DataFrame, Path, List[Dict[str, Any]], str],
         max_cardinality: Optional[int] = None,
         sample_size: Optional[int] = None,
         enrich: bool = False,
-    ) -> BaseInferSchema:
-        infer_class = None
+    ) -> BaseSchemaGenerator:
+        schema_generator_class = None
         if isinstance(source, pd.DataFrame):
-            infer_class = DataframeInferSchema
+            schema_generator_class = DataframeSchemaGenerator
         elif isinstance(source, (Path, str)):
             source = Path(source) if isinstance(source, str) else source
             if source.name.endswith('.csv'):
-                infer_class = CSVInferSchema
+                schema_generator_class = CSVSchemaGenerator
             elif source.name.endswith('.parquet'):
-                infer_class = ParquetInferSchema
+                schema_generator_class = ParquetSchemaGenerator
         elif isinstance(source, list):
-            infer_class = ListInferSchema
+            schema_generator_class = ListSchemaGenerator
 
-        if not infer_class:
+        if not schema_generator_class:
             raise ValueError(
                 'Invalid source. Pass dataframe, path to csv/parquet file or list of '
                 'rows instead'
             )
 
-        return infer_class(
+        return schema_generator_class(
             source=source,
             max_cardinality=max_cardinality,
             sample_size=sample_size,
             enrich=enrich,
         )
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/job_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/job_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 from http import HTTPStatus
 from typing import Iterator, List, Optional
 
 from requests.exceptions import ConnectionError
 
 from fiddler.exceptions import AsyncJobFailed
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logger
+from fiddler.schema.job import JobStatus
+from fiddler.utils.decorators import handle_api_error_response
 from fiddler.utils.logger import get_logger
-from fiddler.v2.schema.job import JobStatus
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.response_handler import JobResponseHandler
+from fiddler.utils.response_handler import JobResponseHandler
 
 logger = get_logger(__name__)
 
 
 class JobMixin:
     DEFAULT_POLL_INTERVAL = 3  # In seconds
     DEFAULT_TIMEOUT = 1800  # 30 minutes in seconds
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev8/fiddler/api/model_artifact_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Callable, Dict, List, Optional
 
 from fiddler.constants import CONTENT_TYPE_OCTET_STREAM_HEADER, \
     MULTI_PART_CHUNK_SIZE
 from fiddler.libs.http_client import RequestClient
+from fiddler.schema.model_deployment import DeploymentParams
 from fiddler.utils.logger import get_logger
-from fiddler.v2.schema.model_deployment import DeploymentParams
-from fiddler.v2.utils.response_handler import APIResponseHandler
+from fiddler.utils.response_handler import APIResponseHandler
 
 logger = get_logger(__name__)
 
 
 class _AbstractModelDeployer(ABC):
     """Abstract class for deploying model artifact"""
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/model_deployment_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Optional
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logger
-from fiddler.utils.logger import get_logger
-from fiddler.v2.schema.model_deployment import ModelDeployment
-from fiddler.v2.utils.compatibility_helpers import (
+from fiddler.schema.model_deployment import ModelDeployment
+from fiddler.utils.compatibility_helpers import (
     project_id_compat,
     model_id_compat,
     is_sync_id_compat,
 )
-from fiddler.v2.utils.decorators import check_version, handle_api_error_response
+from fiddler.utils.decorators import check_version, handle_api_error_response
+from fiddler.utils.logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class ModelDeploymentMixin:
     """Model deployment api handler"""
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/model_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/model_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,41 @@
 import os
 import shutil
 import tempfile
-import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from pydantic import parse_obj_as
 
-from fiddler import ModelInfo
-from fiddler.constants import MULTI_PART_CHUNK_SIZE
-from fiddler.core_objects import ModelInputType, ModelTask
-from fiddler.libs.http_client import RequestClient
-from fiddler.schemas.model_schema import ModelSchema
-from fiddler.schemas.model_spec import ModelSpec
-from fiddler.schemas.model_task_params import ModelTaskParams
-from fiddler.schemas.xai_params import XaiParams
-from fiddler.utils.logger import get_logger
-from fiddler.v2.api.model_artifact_deploy import (
+from fiddler.api.model_artifact_deploy import (
     ModelArtifactDeployer,
     MultiPartModelArtifactDeployer,
 )
-from fiddler.v2.schema.model import Model
-from fiddler.v2.schema.model_deployment import ArtifactType, DeploymentParams
-from fiddler.v2.utils.compatibility_helpers import (
-    project_id_compat,
-    model_id_compat,
+from fiddler.constants import MULTI_PART_CHUNK_SIZE
+from fiddler.core_objects import ModelInfo
+from fiddler.libs.http_client import RequestClient
+from fiddler.schema.model import Model
+from fiddler.schema.model_deployment import ArtifactType, DeploymentParams
+from fiddler.utils.compatibility_helpers import (
     dataset_id_compat,
     is_sync_id_compat,
     model_dir_compat,
+    model_id_compat,
+    project_id_compat,
 )
-from fiddler.v2.utils.decorators import check_version, handle_api_error_response
-from fiddler.v2.utils.helpers import get_model_artifact_info, read_model_yaml
-from fiddler.v2.utils.response_handler import (
-    APIResponseHandler,
-    PaginatedResponseHandler,
-)
-from fiddler.v2.utils.validations import validate_artifact_dir
+from fiddler.utils.decorators import check_version, handle_api_error_response
+from fiddler.utils.helpers import get_model_artifact_info, read_model_yaml
+from fiddler.utils.logger import get_logger
+from fiddler.utils.response_handler import APIResponseHandler, PaginatedResponseHandler
+from fiddler.utils.validations import validate_artifact_dir
 
 logger = get_logger(__name__)
 
 
 class ModelMixin:
-    ADD_SURROGATE_MODEL_API_VERSION = '>=22.12.0'
-    ADD_MODEL_ARTIFACT_API_VERSION = '>=22.12.0'
-    DELETE_MODEL_API_VERSION = '>=22.12.0'
 
     client: RequestClient
     organization_name: str
 
     @handle_api_error_response
     def get_models(self, project_name: str) -> List[Model]:
         """
@@ -121,57 +109,31 @@
 
     @handle_api_error_response
     def add_model(  # noqa: C901
         self,
         project_id: str = None,
         model_id: str = None,
         dataset_id: str = None,
-        model_info: Optional[ModelInfo] = None,
-        is_sync: Optional[bool] = True,
-        task: Optional[ModelTask] = None,
-        input_type: Optional[ModelInputType] = None,
-        schema: Optional[ModelSchema] = None,
-        spec: Optional[ModelSpec] = None,
-        task_params: Optional[ModelTaskParams] = None,
-        xai_params: Optional[XaiParams] = None,
-        display_name: Optional[str] = None,
-        description: Optional[str] = None,
-        algorithm: Optional[str] = None,
-        framework: Optional[str] = None,
-        event_id_col: Optional[str] = None,
-        event_ts_col: Optional[str] = None,
-        event_ts_format: Optional[str] = None,
-        wait: bool = True,
+        model_info: ModelInfo = None,
+        is_sync: bool = True,
         project_name: str = None,
         model_name: str = None,
-        dataset_name: Optional[str] = None,
+        dataset_name: str = None,
+        wait: bool = True,
     ) -> Model:
         """
         Onboard model to Fiddler Platform
         :params project_id: The project to which the model belongs to
         :params model_id: The model name of which you need the details
         :param dataset_id: name of the dataset
         :param is_sync: Wait for job to complete or return after submitting
         :param project_name: project name where the model will be added
         :param model_name: name of the model
         :param dataset_name: name of the dataset
         :param model_info: (Deprecated) model related information from user
-        :param task: Task the model is designed to address
-        :param input_type: Whether the model is in the tabular or text
-        :param schema: ModelSchema object
-        :param spec: ModelSpec object
-        :param task_params: ModelTaskParams object
-        :param xai_params: XaiParams object
-        :param display_name: Display name for the model
-        :param description: Description for the model
-        :param algorithm: Algorithm used for this model
-        :param framework: Framework used for this model
-        :param event_id_col: Column name to use as event id
-        :param event_ts_col: Column name to use as event timestamp
-        :param event_ts_format: Format of the event timestamp specified in event_ts_col
         :param wait: Whether to wait for job to complete or return after submitting
             the job
         """
 
         project_name = project_id_compat(
             project_id=project_id, project_name=project_name
         )
@@ -182,63 +144,28 @@
         )
 
         dataset_name = dataset_id_compat(
             dataset_id=dataset_id,
             dataset_name=dataset_name,
         )
 
-        if model_info:
-            warnings.warn(
-                'model_info is deprecated from 2.0.0. Use schema and spec instead',
-                DeprecationWarning,
-            )
-            if dataset_name:
-                model_info.datasets = [dataset_name]
-        elif not (schema and spec and input_type and task):
-            raise ValueError(
-                'Model requires either model_info or input_type, task, schema and spec'
-            )
+        wait = is_sync_id_compat(is_sync=is_sync, wait=wait)
+
+        if not model_info:
+            raise ValueError('Please pass a valid ModelInfo object')
+
+        model_info.datasets = [dataset_name]
 
         request_body = {
             'name': model_name,
             'project_name': project_name,
             'organization_name': self.organization_name,
+            'info': model_info.to_dict(),
         }
 
-        if model_info:
-            request_body['info'] = model_info.to_dict()
-        if dataset_name:
-            request_body['dataset_name'] = dataset_name
-        if input_type:
-            request_body['input_type'] = input_type.value
-        if task:
-            request_body['task'] = task.value
-        if schema:
-            request_body['schema'] = schema.dict()
-        if spec:
-            request_body['spec'] = spec.dict()
-        if task_params:
-            request_body['task_params'] = task_params.dict()
-        if xai_params:
-            request_body['xai_params'] = xai_params.dict()
-        if description:
-            request_body['description'] = description
-        if algorithm:
-            request_body['algorithm'] = algorithm
-        if framework:
-            request_body['framework'] = framework
-        if display_name:
-            request_body['display_name'] = display_name
-        if event_id_col:
-            request_body['event_id_col'] = event_id_col
-        if event_ts_col:
-            request_body['event_ts_col'] = event_ts_col
-        if event_ts_format:
-            request_body['event_ts_format'] = event_ts_format
-
         response = self.client.post(
             url='models',
             data=request_body,
         )
 
         logger.info('Model %s added to %s project', model_name, project_name)
 
@@ -505,15 +432,15 @@
                 model_name,
                 artifact_dir,
             )
             file_path = shutil.make_archive(
                 base_name=str(Path(tmp) / 'files'),
                 format='tar',
                 root_dir=str(artifact_dir),
-                base_dir='.',
+                base_dir='',
             )
 
             logger.info(
                 'Model[%s/%s] - Model artifact tar file created at %s',
                 project_name,
                 model_name,
                 file_path,
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/api/project_mixin.py` & `fiddler-client-2.0.0.dev8/fiddler/api/project_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from http import HTTPStatus
 from typing import List
 
 from pydantic import parse_obj_as
 
 from fiddler.libs.http_client import RequestClient
+from fiddler.schema.project import Project
+from fiddler.utils.compatibility_helpers import project_id_compat
+from fiddler.utils.decorators import handle_api_error_response
 from fiddler.utils.logger import get_logger
-from fiddler.v2.schema.project import Project
-from fiddler.v2.utils.compatibility_helpers import project_id_compat
-from fiddler.v2.utils.decorators import handle_api_error_response
-from fiddler.v2.utils.response_handler import (
+from fiddler.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = get_logger(__name__)
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/schema/alert.py` & `fiddler-client-2.0.0.dev8/fiddler/schema/alert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import Field, root_validator
 
-from fiddler.v2.schema.base import BaseDataSchema
+from fiddler.schema.base import BaseDataSchema
 
 
 @enum.unique
 class AlertType(str, enum.Enum):
     """Supported Alert types"""
 
     PERFORMANCE = 'performance'
@@ -25,17 +25,17 @@
     """Supported metrics for Alerts."""
 
     # Drift metrics
     JSD = 'jsd'
     PSI = 'psi'
 
     ## Data Integrity Metrics
-    MISSING_VALUE = 'missing_value'
-    RANGE_VIOLATION = 'range_violation'
-    TYPE_VIOLATION = 'type_violation'
+    MISSING_VALUE = 'is_nullable_violation'
+    RANGE_VIOLATION = 'is_range_violation'
+    TYPE_VIOLATION = 'is_type_violation'
 
     ## Performance metrics
     # Binary Classification
     ACCURACY = 'accuracy'
     RECALL = 'recall'
     FPR = 'fpr'
     PRECISION = 'precision'
@@ -65,21 +65,21 @@
     AVERAGE = 'average'
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}.{self.name}'
 
 
 @enum.unique
-class BinSize(enum.IntEnum):
+class BinSize(enum.Enum):
     """Bin Size values in millisecs Alerts can be set on"""
 
-    ONE_HOUR = 3600000
-    ONE_DAY = 86400000
-    SEVEN_DAYS = 604800000
-    ONE_MONTH = 2592000000
+    ONE_HOUR = (3600000, 'Hour')
+    ONE_DAY = (86400000, 'Day')
+    SEVEN_DAYS = (604800000, 'Week')
+    ONE_MONTH = (2592000000, 'Month')
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}.{self.name}'
 
     @classmethod
     def keys(cls) -> List[str]:
         return list(cls.__members__.values())
@@ -133,51 +133,49 @@
 
 
 class AlertRulePayload(BaseDataSchema):
     organization_name: str
     project_name: str
     model_name: str
     name: str
-    alert_type: AlertType
+    alert_type: Optional[AlertType]
     metric: Metric
+    metric_id: Union[Metric, str]
     feature_names: Optional[List[str]]
     priority: Priority
     compare_to: CompareTo
     baseline_name: Optional[str]
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
-    time_bucket: BinSize
+    time_bucket: int
+    bin_size: str
     notifications: Optional[Dict[str, Any]]
 
 
 class AlertRule(BaseDataSchema):
     alert_rule_uuid: str = Field(alias='uuid')
     organization_name: str
     project_name: str = Field(alias='project_name')
-    model_name: str = Field(alias='model_name')
+    model_name: str
     name: Optional[str]
-    alert_type: AlertType
-    metric: Metric
+    alert_type: Optional[AlertType]
+    metric: str
     columns: Optional[List[str]] = Field(alias='feature_names')
-    baseline_name: Optional[str] = Field(alias='baseline_name')
+    baseline_name: Optional[str]
     priority: Priority
     compare_to: CompareTo
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
-    bin_size: BinSize = Field(alias='time_bucket')
+    bin_size: Optional[str]
+    time_bucket: Optional[int]
 
-    @root_validator(pre=True)
-    def set_compare_period(cls, values) -> Optional[ComparePeriod]:
-        if values['compare_period'] == 0:
-            values['compare_period'] = None
-        return values
 
 
 class TriggeredAlerts(BaseDataSchema):
     id: int
     triggered_alert_id: str = Field(alias='uuid')
     alert_rule_uuid: str = Field(alias='alert_config_uuid')
     alert_run_start_time: int
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/schema/dataset.py` & `fiddler-client-2.0.0.dev8/fiddler/schema/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Optional
 
 from fiddler.constants import FileType, UploadType
 from fiddler.core_objects import DatasetInfo
 from fiddler.exceptions import HttpException
-from fiddler.v2.utils.response_handler import APIResponseHandler
+from fiddler.utils.response_handler import APIResponseHandler
 
 
 class Dataset:
     def __init__(
             self,
         id: int,
         name: str,
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/schema/events.py` & `fiddler-client-2.0.0.dev8/fiddler/schema/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional
 
 from fiddler.constants import FiddlerTimestamp, FileType, UploadType
-from fiddler.v2.schema.base import BaseDataSchema
+from fiddler.schema.base import BaseDataSchema
 
 
 class EventsIngest(BaseDataSchema):
     file_name: List[str]
     batch_id: Optional[str] = None
     events_schema: Optional[dict] = None
     id_field: Optional[str] = None
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/schema/model_deployment.py` & `fiddler-client-2.0.0.dev8/fiddler/schema/model_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from enum import Enum
 from typing import Optional
 from uuid import UUID
 
 from pydantic import BaseModel
 
-from fiddler.v2.schema.user import UserCompact
+from fiddler.schema.user import UserCompact
 
 
 class ArtifactType(str, Enum):
     SURROGATE = 'SURROGATE'
     PYTHON_PACKAGE = 'PYTHON_PACKAGE'
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/utils/compatibility_helpers.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/compatibility_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Dict
 
 import pandas as pd
 
-from fiddler.v2.utils.decorators import compat_warning
+from fiddler.utils.decorators import compat_warning
 
 
 @compat_warning
 def dataset_id_compat(dataset_id: str, dataset_name: str) -> str:
     """
     Check duplicate dataset related params for compatibility.
 
     :param dataset_id:   The dataset name of which you need the details
     :param dataset_name: The dataset name of which you need the details
     """
 
     if dataset_id is None and dataset_name is None:
         raise ValueError('Pass either dataset_id or dataset_name')
     if dataset_id is not None and dataset_name is not None:
-        raise ValueError('Pass either dataset_id or dataset_name')
+        raise ValueError('Pass either dataset_id or dataset_name, not both')
 
     return dataset_id or dataset_name
 
 
 @compat_warning
 def model_id_compat(model_id: str, model_name: str) -> str:
     """
@@ -29,71 +29,72 @@
 
     :param model_id:   The model name of which you need the details
     :param model_name: The model name of which you need the details
     """
     if model_id is None and model_name is None:
         raise ValueError('Pass either model_id or model_name')
     if model_id is not None and model_name is not None:
-        raise ValueError('Pass either model_id or model_name')
+        raise ValueError('Pass either model_id or model_name, not both')
     return model_id or model_name
 
 
 @compat_warning
 def project_id_compat(project_id: str, project_name: str) -> str:
     """
     Check duplicate project related params for compatibility.
 
     :param project_id:   The project to which the dataset belongs to
     :param project_name: The project to which the dataset belongs to
     """
     if project_id is None and project_name is None:
-        raise ValueError('Pass either project_id or project_id')
+        raise ValueError('Pass either project_id or project_name')
     if project_id is not None and project_name is not None:
-        raise ValueError('Pass either project_id or project_id')
+        raise ValueError('Pass either project_id or project_name, not both')
     return project_id or project_name
 
 
 @compat_warning
 def update_event_compat(update_event: bool, is_update: bool) -> bool:
     """
     Check duplicate project related params for compatibility.
 
     :param update_event: If publish event is of type update
     :param is_update:    If publish event is of type update
     """
     if update_event is not None and is_update is not None:
-        raise ValueError('Pass either update_event or is_update')
+        raise ValueError('Pass either update_event or is_update, not both')
     return update_event or is_update
 
 
 @compat_warning
 def is_sync_id_compat(is_sync: bool, wait: bool) -> bool:
     """
     Check duplicate baseline related params for compatibility.
 
     :param baseline_id:    unique identifier for the baseline
     :param baseline_name:  unique identifier for the baseline
     """
-    if is_sync is not None and wait is not None:
+    if is_sync is None and wait is None:
         raise ValueError('Pass either is_sync or wait')
+
     return is_sync or wait
 
 
 @compat_warning
 def model_dir_compat(model_dir: str, artifact_dir: str) -> str:
     """
     Check duplicate baseline related params for compatibility.
 
     :param baseline_id:    unique identifier for the baseline
     :param baseline_name:  unique identifier for the baseline
     """
     if model_dir is None and artifact_dir is None:
         raise ValueError('Pass either model_dir or artifact_dir')
     if model_dir is not None and artifact_dir is not None:
-        raise ValueError('Pass either model_dir or artifact_dir')
+        raise ValueError('Pass either model_dir or artifact_dir, not both')
     return model_dir or artifact_dir
 
 
 @compat_warning
 def dataset_compat(
     dataset: Dict[str, pd.DataFrame], datasets: Dict[str, pd.DataFrame]
 ) -> Dict[str, pd.DataFrame]:
@@ -111,9 +112,9 @@
 
     :param baseline_id:    unique identifier for the baseline
     :param baseline_name:  unique identifier for the baseline
     """
     if baseline_id is None and baseline_name is None:
         raise ValueError('Pass either baseline_id or baseline_name')
     if baseline_id is not None and baseline_name is not None:
-        raise ValueError('Pass either baseline_id or baseline_name')
+        raise ValueError('Pass either baseline_id or baseline_name, not both')
     return baseline_id or baseline_name
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/utils/decorators.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     BadRequest,
     Forbidden,
     Conflict,
     NotFound,
     InternalServerError,
 )
 from fiddler.utils import logger
-from fiddler.v2.utils.helpers import match_semver
+from fiddler.utils.helpers import match_semver
 
 logger = logger.get_logger(__name__)
 
 map_except_resp_code = {
     HTTPStatus.BAD_REQUEST: BadRequest,  # 400
     HTTPStatus.FORBIDDEN: Forbidden,  # 403
     HTTPStatus.NOT_FOUND: NotFound,  # 404
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/utils/helpers.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict, List, Optional
 
 import yaml
 
 from fiddler.constants import FileType
 from fiddler.core_objects import ModelInfo
 from fiddler.exceptions import NotSupported
-from fiddler.v2.schema.server_info import Version
+from fiddler.schema.server_info import Version
 
 
 def match_semver(version: Optional[Version], match_expr: str) -> bool:
     """
     Match the version with match_expr
     :param version: Server version
     :param match_expr: Version to match with. Read more at VersionInfo.match
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/utils/response_handler.py` & `fiddler-client-2.0.0.dev8/fiddler/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev8/fiddler/validators/dataset_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import Dict
 
 import pandas as pd
 
 from fiddler.constants import FileType
 from fiddler.core_objects import DatasetInfo
+from fiddler.utils.helpers import map_extension_to_file_type
 from fiddler.utils.logger import get_logger
-from fiddler.v2.utils.helpers import map_extension_to_file_type
 
 LOG = get_logger(__name__)
 
 NUM_ROWS = 1
 JUST_THE_HEADER = 0
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev8/fiddler_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev7
+Version: 2.0.0.dev8
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
```

### Comparing `fiddler-client-2.0.0.dev7/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev8/fiddler_client.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,99 @@
 MANIFEST.in
 PUBLIC.md
 README.md
 setup.py
 fiddler/__init__.py
 fiddler/_version.py
-fiddler/connection.py
 fiddler/constants.py
 fiddler/core_objects.py
 fiddler/exceptions.py
-fiddler/fiddler_api.py
+fiddler/api/__init__.py
+fiddler/api/alert_mixin.py
+fiddler/api/api.py
+fiddler/api/baseline_mixin.py
+fiddler/api/compatibility_mixin.py
+fiddler/api/dataset_mixin.py
+fiddler/api/events_mixin.py
+fiddler/api/explainability_mixin.py
+fiddler/api/generate_schema_mixin.py
+fiddler/api/helpers.py
+fiddler/api/job_mixin.py
+fiddler/api/model_artifact_deploy.py
+fiddler/api/model_deployment_mixin.py
+fiddler/api/model_mixin.py
+fiddler/api/project_mixin.py
 fiddler/assets/__init__.py
 fiddler/assets/pg_reserved_words.py
 fiddler/libs/__init__.py
 fiddler/libs/http_client.py
 fiddler/packtools/__init__.py
 fiddler/packtools/gem.py
 fiddler/packtools/keras_ig_helpers.py
 fiddler/packtools/project_attributions_helpers.py
 fiddler/packtools/template_model.py
+fiddler/schema/__init__.py
+fiddler/schema/alert.py
+fiddler/schema/base.py
+fiddler/schema/baseline.py
+fiddler/schema/dataset.py
+fiddler/schema/events.py
+fiddler/schema/job.py
+fiddler/schema/model.py
+fiddler/schema/model_deployment.py
+fiddler/schema/project.py
+fiddler/schema/server_info.py
+fiddler/schema/user.py
 fiddler/schemas/__init__.py
 fiddler/schemas/custom_features.py
 fiddler/schemas/model_schema.py
 fiddler/schemas/model_spec.py
 fiddler/schemas/model_task_params.py
 fiddler/schemas/xai_params.py
 fiddler/utils/__init__.py
+fiddler/utils/compatibility_helpers.py
+fiddler/utils/decorators.py
 fiddler/utils/exceptions.py
 fiddler/utils/formatting.py
 fiddler/utils/general_checks.py
-fiddler/utils/helper.py
+fiddler/utils/helpers.py
 fiddler/utils/logger.py
 fiddler/utils/pandas_helper.py
+fiddler/utils/response_handler.py
+fiddler/utils/semver_version.py
+fiddler/utils/validations.py
 fiddler/utils/validator.py
-fiddler/v2/__init__.py
-fiddler/v2/api/__init__.py
-fiddler/v2/api/alert_mixin.py
-fiddler/v2/api/api.py
-fiddler/v2/api/baseline_mixin.py
-fiddler/v2/api/compatibility_mixin.py
-fiddler/v2/api/dataset_mixin.py
-fiddler/v2/api/events_mixin.py
-fiddler/v2/api/explainability_mixin.py
-fiddler/v2/api/helpers.py
-fiddler/v2/api/infer_schema_mixin.py
-fiddler/v2/api/job_mixin.py
-fiddler/v2/api/model_artifact_deploy.py
-fiddler/v2/api/model_deployment_mixin.py
-fiddler/v2/api/model_mixin.py
-fiddler/v2/api/project_mixin.py
-fiddler/v2/schema/__init__.py
-fiddler/v2/schema/alert.py
-fiddler/v2/schema/base.py
-fiddler/v2/schema/baseline.py
-fiddler/v2/schema/dataset.py
-fiddler/v2/schema/events.py
-fiddler/v2/schema/job.py
-fiddler/v2/schema/model.py
-fiddler/v2/schema/model_deployment.py
-fiddler/v2/schema/project.py
-fiddler/v2/schema/server_info.py
-fiddler/v2/schema/user.py
-fiddler/v2/utils/__init__.py
-fiddler/v2/utils/compatibility_helpers.py
-fiddler/v2/utils/decorators.py
-fiddler/v2/utils/helpers.py
-fiddler/v2/utils/response_handler.py
-fiddler/v2/utils/validations.py
-fiddler/v2/validators/__init__.py
-fiddler/v2/validators/dataset_validator.py
+fiddler/validators/__init__.py
+fiddler/validators/dataset_validator.py
 fiddler_client.egg-info/PKG-INFO
 fiddler_client.egg-info/SOURCES.txt
 fiddler_client.egg-info/dependency_links.txt
 fiddler_client.egg-info/requires.txt
 fiddler_client.egg-info/top_level.txt
 tests/__init__.py
-tests/test_infer_model_schema.py
 tests/test_object_inference.py
 tests/utils.py
 tests/fiddler/__init__.py
+tests/fiddler/base.py
+tests/fiddler/helper.py
+tests/fiddler/test_add_model.py
+tests/fiddler/test_alert.py
+tests/fiddler/test_baseline.py
+tests/fiddler/test_check_version_decorator.py
+tests/fiddler/test_custom_features.py
+tests/fiddler/test_dataset_api.py
+tests/fiddler/test_events_api.py
+tests/fiddler/test_exceptions.py
+tests/fiddler/test_explainability_apis.py
+tests/fiddler/test_file_upload.py
+tests/fiddler/test_generate_schema.py
+tests/fiddler/test_helpers.py
+tests/fiddler/test_job.py
+tests/fiddler/test_model.py
+tests/fiddler/test_project.py
+tests/fiddler/test_response_handler.py
+tests/fiddler/test_upload_dataset.py
+tests/fiddler/test_validations.py
 tests/fiddler/utils/__init__.py
 tests/fiddler/utils/test_general_checks.py
 tests/fiddler/utils/test_pandas.py
-tests/fiddler/utils/tests_utils.py
-tests/v2/__init__.py
-tests/v2/base.py
-tests/v2/helper.py
-tests/v2/test_add_model.py
-tests/v2/test_alert.py
-tests/v2/test_baseline.py
-tests/v2/test_check_version_decorator.py
-tests/v2/test_custom_features.py
-tests/v2/test_dataset_api.py
-tests/v2/test_events_api.py
-tests/v2/test_exceptions.py
-tests/v2/test_explainability_apis.py
-tests/v2/test_file_upload.py
-tests/v2/test_helpers.py
-tests/v2/test_job.py
-tests/v2/test_model.py
-tests/v2/test_project.py
-tests/v2/test_response_handler.py
-tests/v2/test_upload_dataset.py
-tests/v2/test_validations.py
+tests/fiddler/utils/tests_utils.py
```

### Comparing `fiddler-client-2.0.0.dev7/setup.py` & `fiddler-client-2.0.0.dev8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     install_requires=[
         'pip>=21.0',
         'requests<3',
         'requests-toolbelt',
         'pandas>=1.2.5,<=1.5.3',
         'pydantic==1.9.0',
         'deprecated==1.2.13',
-        'semver>=2,<3',
         'tqdm==4.64.1',
         'simplejson>=3.17.0',
         'pyarrow>=12.0.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `fiddler-client-2.0.0.dev7/tests/fiddler/utils/test_general_checks.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/tests/fiddler/utils/test_pandas.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 import pandas.api.types as ptypes
 from pytz import timezone
 
 from fiddler import utils
-from tests.v2.base import BaseTestCase
+from tests.fiddler.base import BaseTestCase
 
 LOG = utils.logger.get_logger(__name__)
 
 
 class TestUtils(BaseTestCase):
     def test_cleaning_df_with_all_datetime_col_should_convert_to_string_col(self):
         all_data = pd.DataFrame(
```

### Comparing `fiddler-client-2.0.0.dev7/tests/fiddler/utils/tests_utils.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/utils/tests_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/tests/test_infer_model_schema.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_generate_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tempfile
 
 import pandas as pd
 import pytest
 from pytest_mock import MockerFixture
 
-from fiddler.v2.api.infer_schema_mixin import InferSchemaFactory
+from fiddler.api.generate_schema_mixin import SchemaGeneratorFactory
 from tests.utils import MockResponse
 
 test_df = df = pd.DataFrame(
     [
         {'col1': 1, 'col2': 'foo'},
         {'col1': 2, 'col2': 'bar'},
         {'col1': 3, 'col2': 'baz'},
@@ -54,60 +54,60 @@
 def mock_client(mocker: MockerFixture):
     mock_client = mocker.MagicMock()
     mock_client.post.return_value = MockResponse(test_api_response)
     yield mock_client
 
 
 def test_infer_schema_with_dataframe(mock_client) -> None:
-    schema_generator = InferSchemaFactory.create(
+    schema_generator = SchemaGeneratorFactory.create(
         source=test_df,
     )
 
-    schema_generator.infer_schema(client=mock_client)
+    schema_generator.generate(client=mock_client)
 
     assert len(mock_client.post.call_args.kwargs['data']['rows']) == test_df.shape[0]
     assert 'max_cardinality' not in mock_client.post.call_args.kwargs['data']
 
 
 def test_infer_schema_with_max_cardinality(mock_client) -> None:
-    schema_generator = InferSchemaFactory.create(source=test_df, max_cardinality=10)
+    schema_generator = SchemaGeneratorFactory.create(source=test_df, max_cardinality=10)
 
-    schema_generator.infer_schema(client=mock_client)
+    schema_generator.generate(client=mock_client)
 
     assert len(mock_client.post.call_args.kwargs['data']['rows']) == test_df.shape[0]
     assert mock_client.post.call_args.kwargs['data']['max_cardinality'] == 10
 
 
 def test_infer_schema_with_csv_file(mock_client) -> None:
     with tempfile.NamedTemporaryFile(suffix='.csv', mode='w') as temp_file:
         test_df.to_csv(temp_file.name, index=False)
 
-        schema_generator = InferSchemaFactory.create(
+        schema_generator = SchemaGeneratorFactory.create(
             source=temp_file.name,
         )
 
-        schema_generator.infer_schema(client=mock_client)
+        schema_generator.generate(client=mock_client)
 
     assert len(mock_client.post.call_args.kwargs['data']['rows']) == test_df.shape[0]
 
 
 def test_infer_schema_with_parquet_file(mock_client) -> None:
     with tempfile.NamedTemporaryFile(suffix='.parquet', mode='wb') as temp_file:
         test_df.to_parquet(temp_file.name, index=False)
 
-        schema_generator = InferSchemaFactory.create(
+        schema_generator = SchemaGeneratorFactory.create(
             source=temp_file.name,
         )
 
-        schema_generator.infer_schema(client=mock_client)
+        schema_generator.generate(client=mock_client)
 
     assert len(mock_client.post.call_args.kwargs['data']['rows']) == test_df.shape[0]
 
 
 def test_infer_schema_with_rows(mock_client) -> None:
-    schema_generator = InferSchemaFactory.create(
+    schema_generator = SchemaGeneratorFactory.create(
         source=test_df.to_dict(orient='records'),
     )
 
-    schema_generator.infer_schema(client=mock_client)
+    schema_generator.generate(client=mock_client)
 
     assert len(mock_client.post.call_args.kwargs['data']['rows']) == test_df.shape[0]
```

### Comparing `fiddler-client-2.0.0.dev7/tests/test_object_inference.py` & `fiddler-client-2.0.0.dev8/tests/test_object_inference.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/base.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import TestCase, mock
 from urllib.parse import urljoin
 
 from decouple import config
 from responses import RequestsMock
 
+from fiddler.api.api import FiddlerClient
 from fiddler.constants import CURRENT_API_VERSION
-from fiddler.v2.api.api import FiddlerClient
 
 
 class BaseTestCase(TestCase):
     def setUp(self) -> None:
         self.maxDiff = None
         _url = config('TEST_FIDDLER_API_SERVER', 'http://127.0.0.1:30001')
         self._url = (
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/helper.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_add_model.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_add_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import mock
 
 import pytest
 
 import fiddler as fdl
 from fiddler import FiddlerClient
 from fiddler.core_objects import DatasetInfo, ModelInfo
-from fiddler.v2.schema.dataset import Dataset
+from fiddler.schema.dataset import Dataset
 
 model_info_json = {
     'model': {
         'name': 'dummy_model',
         'input-type': fdl.ModelInputType.TABULAR,
         'model-task': fdl.ModelTask.BINARY_CLASSIFICATION,
         'inputs': [
@@ -84,15 +84,17 @@
 
 def test_add_model_invalid_model_info_v2_client():
     with pytest.raises(Exception):
         server_info_mock = mock.patch.object(FiddlerClient, '_get_server_info')
         server_info_mock.start()
         _check_semver_mock = mock.patch.object(FiddlerClient, '_check_server_version')
         _check_semver_mock.start()
-        _check_vc_mock = mock.patch.object(FiddlerClient, '_check_version_compatibility')
+        _check_vc_mock = mock.patch.object(
+            FiddlerClient, '_check_version_compatibility'
+        )
         _check_vc_mock.start()
         client = FiddlerClient('https://test_org.fiddler.ai', 'test_org', 'test_token')
         client.add_model(
             project_name='project1',
             model_name='model1',
             dataset_name='dataset_id_1',
             model_info='string_instead_of_model_info_object',
@@ -101,20 +103,20 @@
 
 def test_add_model_none_model_info_v2_client():
     with pytest.raises(ValueError) as cx:
         server_info_mock = mock.patch.object(FiddlerClient, '_get_server_info')
         server_info_mock.start()
         _check_semver_mock = mock.patch.object(FiddlerClient, '_check_server_version')
         _check_semver_mock.start()
-        _check_vc_mock = mock.patch.object(FiddlerClient, '_check_version_compatibility')
+        _check_vc_mock = mock.patch.object(
+            FiddlerClient, '_check_version_compatibility'
+        )
         _check_vc_mock.start()
         client = FiddlerClient('https://test_org.fiddler.ai', 'test_org', 'test_token')
         client.add_model(
             project_name='project1',
             model_name='model1',
             dataset_name='dataset_id_1',
             model_info=None,
         )
 
-    assert cx.match(
-        'Model requires either model_info or input_type, task, schema and spec'
-    )
+    assert cx.match('Please pass a valid ModelInfo object')
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_alert.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from http import HTTPStatus
 from typing import Optional
 from unittest import mock
 
 from responses import matchers
 
 from fiddler.exceptions import NotFound
-from fiddler.v2.schema.alert import (
+from fiddler.schema.alert import (
     AlertCondition,
     AlertRule,
     AlertType,
     BinSize,
     ComparePeriod,
     CompareTo,
     Metric,
     Priority,
     TriggeredAlerts,
 )
-from fiddler.v2.schema.server_info import ServerInfo
-from tests.v2.base import BaseTestCase
+from fiddler.schema.server_info import ServerInfo
+from tests.fiddler.base import BaseTestCase
 
 
 class TestAlert(BaseTestCase):
     def setUp(self):
         super(TestAlert, self).setUp()
         self._project_name = 'test_project'
         self._model_name = 'test_model'
@@ -103,53 +103,79 @@
                         'critical_threshold': 0.8,
                         'organization_name': self._org,
                         'id': 3,
                         'sub_metric': 'jsd',
                         'metric': 'jsd',
                         'condition': 'greater',
                         'time_bucket': 3600000,
-                        'compare_period': 0,
                         'model_name': self._model_name,
                         'name': 'alert_name_3',
                         'feature_names': ['probability_churned'],
                         'created_by': 'admin@fiddler.ai',
                         'alert_type': 'drift',
                         'uuid': '320060fa-abeb-4cae-9718-17d6f917b414',
                         'is_active': True,
                         'created_at': '2022-09-08T18:47:28.975000+00:00',
                         'project_name': self._project_name,
                         'warning_threshold': 0.4,
                         'compare_to': 'raw_value',
                         'alert_log_time': '2022-09-08T18:47:30.100808+00:00',
                         'priority': 'LOW',
                     },
+                    {
+                        'critical_threshold': 0.8,
+                        'organization_name': self._org,
+                        'id': 4,
+                        'metric': 'newmetricid',
+                        'condition': 'greater',
+                        'bin_size': 'Hour',
+                        'model_name': self._model_name,
+                        'version': 'rule_v3',
+                        'name': 'alert_name_4',
+                        'feature_names': ['probability_churned', 'age'],
+                        'created_by': 'admin@fiddler.ai',
+                        'uuid': '328860fa-abeb-4cae-9718-17d6f917b735',
+                        'is_active': True,
+                        'created_at': '2022-09-08T18:47:28.975000+00:00',
+                        'project_name': self._project_name,
+                        'warning_threshold': 0.4,
+                        'compare_to': 'raw_value',
+                        'alert_log_time': '2022-09-08T18:47:30.100808+00:00',
+                        'priority': 'LOW',
+                    },
                 ],
             },
             'api_version': '2.0',
             'kind': 'PAGINATED',
         }
 
         url = self._get_url()
 
-        query_params = {'organization_name': 'test_organization', 'offset': 0, 'limit': 20, 'ordering': 'alert_type,metric', 'filter': '{"condition": "AND", "rules": [{"field": "project_name", "operator": "equal", "value": "test_project"}, {"field": "model_name", "operator": "equal", "value": "test_model"}, {"field": "alert_type", "operator": "equal", "value": "drift"}, {"field": "metric", "operator": "equal", "value": "jsd"}, {"field": "baseline_name", "operator": "equal", "value": "test_baseline"}]}'}
+        query_params = {
+            'organization_name': 'test_organization',
+            'offset': 0,
+            'limit': 20,
+            'ordering': 'alert_type,metric',
+            'filter': '{"condition": "AND", "rules": [{"field": "project_name", "operator": "equal", "value": "test_project"}, {"field": "model_name", "operator": "equal", "value": "test_model"}, {"field": "alert_type", "operator": "equal", "value": "drift"}, {"field": "metric", "operator": "equal", "value": "jsd"}, {"field": "baseline_name", "operator": "equal", "value": "test_baseline"}]}',
+        }
 
         self.requests_mock.get(
             url, json=response, match=[matchers.query_param_matcher(query_params)]
         )
 
         server_info = ServerInfo(**{'feature_flags': {}, 'server_version': '23.3.0'})
 
         with mock.patch.object(
             self.client, 'server_info', server_info
         ) as mock_server_info:
             alert_rules = self.client.get_alert_rules(
                 project_name='test_project',
                 model_name='test_model',
                 alert_type='drift',
-                metric='jsd',
+                metrics=['jsd'],
                 baseline_name='test_baseline',
                 ordering=['alert_type', 'metric'],
             )
 
         self.assertIsInstance(alert_rules[0], AlertRule)
         self.assertEqual(alert_rules[0].alert_type, 'drift')
         self.assertEqual(alert_rules[0].critical_threshold, 0.5)
@@ -168,15 +194,29 @@
         self.assertEqual(alert_rules[2].project_name, self._project_name)
         self.assertEqual(alert_rules[2].model_name, self._model_name)
         self.assertEqual(alert_rules[2].model_name, self._model_name)
         self.assertEqual(
             alert_rules[2].alert_rule_uuid, '320060fa-abeb-4cae-9718-17d6f917b414'
         )
         self.assertIsNone(alert_rules[2].compare_period)
-        self.assertEqual(len(alert_rules), 3)
+
+        self.assertIsInstance(alert_rules[3], AlertRule)
+        self.assertEqual(alert_rules[3].metric, 'newmetricid')
+        self.assertEqual(alert_rules[3].critical_threshold, 0.8)
+        self.assertEqual(alert_rules[3].name, 'alert_name_4')
+        self.assertEqual(alert_rules[3].columns, ['probability_churned', 'age'])
+        self.assertEqual(alert_rules[3].bin_size, 'Hour')
+        self.assertEqual(alert_rules[3].project_name, self._project_name)
+        self.assertEqual(alert_rules[3].model_name, self._model_name)
+        self.assertEqual(alert_rules[3].model_name, self._model_name)
+        self.assertEqual(
+            alert_rules[3].alert_rule_uuid, '328860fa-abeb-4cae-9718-17d6f917b735'
+        )
+
+        self.assertEqual(len(alert_rules), 4)
 
         response_items = self.requests_mock.calls[0].response.json()['data']['items']
 
         self.assertEqual(response_items[0]['organization_name'], self._org)
         self.assertEqual(response_items[0]['model_name'], self._model_name)
         self.assertEqual(response_items[0]['project_name'], self._project_name)
         self.assertEqual(response_items[0]['alert_type'], 'drift')
@@ -245,15 +285,14 @@
                         'critical_threshold': 0.8,
                         'organization_name': self._org,
                         'id': 3,
                         'sub_metric': 'jsd',
                         'metric': 'jsd',
                         'condition': 'greater',
                         'time_bucket': 3600000,
-                        'compare_period': 0,
                         'model_name': self._model_name,
                         'name': 'alert_name_3',
                         'feature_names': ['probability_churned'],
                         'created_by': 'admin@fiddler.ai',
                         'alert_type': 'drift',
                         'uuid': '320060fa-abeb-4cae-9718-17d6f917b414',
                         'is_active': True,
@@ -315,15 +354,15 @@
         with mock.patch.object(
             self.client, 'server_info', server_info
         ) as mock_server_info:
             alert_rules = self.client.get_alert_rules(
                 project_name='test_project',
                 model_name='test_model',
                 alert_type='drift',
-                metric='jsd',
+                metrics=['jsd'],
                 columns=['test_column'],
                 baseline_name='test_baseline',
                 ordering=['alert_type', 'metric'],
             )
 
         self.assertIsInstance(alert_rules[0], AlertRule)
         self.assertEqual(alert_rules[0].alert_type, 'drift')
@@ -431,15 +470,15 @@
                 name='alert_name_com',
                 priority=Priority.LOW,
                 alert_type=AlertType.DATA_DRIFT,
                 metric=Metric.JSD,
                 columns=['probability_churned'],
                 baseline_name='baseline_name',
                 bin_size=BinSize.ONE_HOUR,
-                compare_period= ComparePeriod.ONE_MONTH,
+                compare_period=ComparePeriod.ONE_MONTH,
                 compare_to=CompareTo.RAW_VALUE,
                 warning_threshold=0.7,
                 critical_threshold=0.2,
                 condition=AlertCondition.LESSER,
                 notifications_config={
                     'emails': {'email': 'nikhil@fiddler.ai, admin@fiddler.ai'},
                     'pagerduty': {
@@ -457,15 +496,15 @@
         )
         self.assertEqual(alert_rule.project_name, self._project_name)
         self.assertEqual(alert_rule.model_name, self._model_name)
         self.assertEqual(alert_rule.alert_type, 'drift')
         self.assertEqual(alert_rule.critical_threshold, 0.2)
         self.assertEqual(alert_rule.name, 'alert_name_com')
         self.assertEqual(alert_rule.baseline_name, 'baseline_name')
-        self.assertEqual(alert_rule.bin_size, BinSize.ONE_HOUR)
+        self.assertEqual(alert_rule.time_bucket, BinSize.ONE_HOUR.value[0])
         self.assertEqual(alert_rule.columns, ['probability_churned'])
         self.assertEqual(alert_rule.compare_period, ComparePeriod.ONE_MONTH)
 
         request_body = json.loads(self.requests_mock.calls[0].request.body)
 
         self.assertEqual(len(self.requests_mock.calls), 1)
         self.assertEqual(request_body['model_name'], self._model_name)
@@ -478,15 +517,14 @@
 
     def test_create_alert_rule(self):
         response = {
             'data': {
                 'created_by': 'admin@fiddler.ai',
                 'priority': 'LOW',
                 'alert_type': 'performance',
-                'compare_period': 0,
                 'time_bucket': 2592000000,
                 'metric': 'r2',
                 'model_name': self._model_name,
                 'organization_name': self._org,
                 'baseline_name': 'baseline_name',
                 'created_at': '2022-09-15T18:10:38.286686+00:00',
                 'critical_threshold': 0.2,
@@ -547,27 +585,100 @@
         )
         self.assertEqual(alert_rule.project_name, self._project_name)
         self.assertEqual(alert_rule.model_name, self._model_name)
         self.assertEqual(alert_rule.alert_type, 'performance')
         self.assertEqual(alert_rule.critical_threshold, 0.2)
         self.assertEqual(alert_rule.name, 'new_name')
         self.assertEqual(alert_rule.baseline_name, 'baseline_name')
-        self.assertEqual(alert_rule.bin_size, BinSize.ONE_MONTH)
+        self.assertEqual(alert_rule.time_bucket, BinSize.ONE_MONTH.value[0])
         self.assertEqual(alert_rule.columns, ['age', 'gender'])
 
         request_body = json.loads(self.requests_mock.calls[0].request.body)
 
         self.assertEqual(len(self.requests_mock.calls), 1)
         self.assertEqual(request_body['model_name'], self._model_name)
         self.assertEqual(request_body['project_name'], self._project_name)
         self.assertEqual(request_body['organization_name'], self._org)
         self.assertEqual(request_body['name'], 'new_name')
         self.assertEqual(request_body['alert_type'], 'performance')
         self.assertEqual(request_body['time_bucket'], 2592000000)
 
+    def test_create_alert_rule_v3(self):
+        response = {
+            'data': {
+                'created_by': 'admin@fiddler.ai',
+                'priority': 'LOW',
+                'bin_size': 'Hour',
+                'metric': 'r2',
+                'model_name': self._model_name,
+                'organization_name': self._org,
+                'baseline_name': 'baseline_name',
+                'created_at': '2022-09-15T18:10:38.286686+00:00',
+                'critical_threshold': 0.2,
+                'feature_names': ['age', 'gender'],
+                'is_active': True,
+                'uuid': '9f8180d3-3fa0-40c4-8656-b9b1d2de1b69',
+                'compare_to': 'raw_value',
+                'warning_threshold': 0.7,
+                'condition': 'lesser',
+                'project_name': self._project_name,
+                'id': 86,
+                'name': 'new_name',
+            },
+            'api_version': '2.0',
+            'kind': 'NORMAL',
+        }
+
+        url = self._get_url()
+
+        self.requests_mock.post(
+            url,
+            json=response,
+        )
+
+        # columns parameter is supported from 23.3.0
+        server_info = ServerInfo(**{'feature_flags': {}, 'server_version': '23.3.0'})
+        with mock.patch.object(
+            self.client, 'server_info', server_info
+        ) as mock_server_info:
+            alert_rule = self.client.add_alert_rule(
+                project_name=self._project_name,
+                model_name=self._model_name,
+                name='new_name',
+                priority=Priority.HIGH,
+                metric='r2',
+                columns=['age', 'gender'],
+                baseline_name='baseline_name',
+                bin_size=BinSize.ONE_HOUR,
+                compare_to=CompareTo.RAW_VALUE,
+                warning_threshold=0.7,
+                critical_threshold=0.2,
+                condition=AlertCondition.LESSER,
+                notifications_config={
+                    'emails': {'email': 'nikhil@fiddler.ai, admin@fiddler.ai'},
+                    'pagerduty': {
+                        'service': 'pd_test_1, pd_test_2',
+                        'severity': 'critical',
+                    },
+                },
+            )
+
+        self.assertEqual(
+            alert_rule.alert_rule_uuid, '9f8180d3-3fa0-40c4-8656-b9b1d2de1b69'
+        )
+        self.assertEqual(alert_rule.project_name, self._project_name)
+        self.assertEqual(alert_rule.model_name, self._model_name)
+        self.assertEqual(alert_rule.metric, 'r2')
+        self.assertEqual(alert_rule.alert_type, None)
+        self.assertEqual(alert_rule.critical_threshold, 0.2)
+        self.assertEqual(alert_rule.name, 'new_name')
+        self.assertEqual(alert_rule.baseline_name, 'baseline_name')
+        self.assertEqual(alert_rule.bin_size, BinSize.ONE_HOUR.value[1])
+        self.assertEqual(alert_rule.columns, ['age', 'gender'])
+
     def test_create_alert_rule_time_period(self):
         response = {
             'data': {
                 'created_by': 'admin@fiddler.ai',
                 'priority': 'LOW',
                 'alert_type': 'drift',
                 'compare_period': 86400000,
@@ -659,43 +770,43 @@
                 'items': [
                     {
                         'id': 285,
                         'uuid': 'ea45ff98-96de-4015-817d-00e571b3fac7',
                         'alert_config_uuid': self._alert_rule_uuid,
                         'alert_run_start_time': 1658481873833,
                         'alert_time_bucket': 1657710000000,
-                        'alert_value': {'__DEFAULT__':0.789176795308359},
+                        'alert_value': {'__DEFAULT__': 0.789176795308359},
                         'baseline_time_bucket': None,
                         'baseline_value': None,
                         'is_alert': True,
                         'severity': None,
                         'failure_reason': 'NA',
                         'message': 'In project bank_churn and model  bank_churn, during the time period of one hour  starting |2022-07-13 11:00:00 (UTC time)|, the prediction drift score was 0.789,   greater than 0.1.',
                     },
                     {
                         'id': 287,
                         'uuid': '9cc8df42-73f4-4f5d-aea9-d8a5ab5b195e',
                         'alert_config_uuid': self._alert_rule_uuid,
                         'alert_run_start_time': 1658481873991,
                         'alert_time_bucket': 1657720800000,
-                        'alert_value': {'__DEFAULT__':0.789176795308359},
+                        'alert_value': {'__DEFAULT__': 0.789176795308359},
                         'baseline_time_bucket': None,
                         'baseline_value': None,
                         'is_alert': True,
                         'severity': None,
                         'failure_reason': 'NA',
                         'message': 'In project bank_churn and model  bank_churn, during the time period of one hour  starting |2022-07-13 14:00:00 (UTC time)|, the prediction drift score was 0.789,   greater than 0.1.',
                     },
                     {
                         'id': 288,
                         'uuid': '5d2868cf-0321-46cd-af36-b784710b2295',
                         'alert_config_uuid': self._alert_rule_uuid,
                         'alert_run_start_time': 1658481874167,
                         'alert_time_bucket': 1657724400000,
-                        'alert_value': {'__DEFAULT__':0.789176795308359},
+                        'alert_value': {'__DEFAULT__': 0.789176795308359},
                         'baseline_time_bucket': None,
                         'baseline_value': None,
                         'is_alert': True,
                         'severity': None,
                         'failure_reason': 'NA',
                         'message': 'In project bank_churn and model  bank_churn, during the time period of one hour  starting |2022-07-13 15:00:00 (UTC time)|, the prediction drift score was 0.789,   greater than 0.1.',
                     },
@@ -710,15 +821,17 @@
             alert_rule_uuid=self._alert_rule_uuid,
             start_time='2022-07-12',
             end_time='2022-07-14',
         )
 
         self.assertIsInstance(triggered_alerts[0], TriggeredAlerts)
         self.assertEqual(triggered_alerts[0].alert_rule_uuid, self._alert_rule_uuid)
-        self.assertEqual(triggered_alerts[0].alert_value, {'__DEFAULT__':0.789176795308359})
+        self.assertEqual(
+            triggered_alerts[0].alert_value, {'__DEFAULT__': 0.789176795308359}
+        )
         self.assertEqual(triggered_alerts[0].failure_reason, 'NA')
         self.assertEqual(triggered_alerts[0].is_alert, True)
 
         response_items = self.requests_mock.calls[0].response.json()['data']['items']
 
         self.assertEqual(response_items[0]['is_alert'], True)
         self.assertEqual(response_items[0]['id'], 285)
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_baseline.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_baseline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from unittest.mock import patch
 
 from fiddler.core_objects import BaselineType
 from fiddler.exceptions import (
     BadRequest,
     NotFound,
 )
-from fiddler.v2.schema.baseline import Baseline
-from tests.v2.base import BaseTestCase
-from tests.v2.helper import (
+from fiddler.schema.baseline import Baseline
+from tests.fiddler.base import BaseTestCase
+from tests.fiddler.helper import (
     get_404_error_response,
     get_base_api_response_body,
     get_base_paginated_api_response_body,
 )
 
 
 class TestBaseline(BaseTestCase):
@@ -112,15 +112,15 @@
 
         self.assertIsInstance(baseline, Baseline)
         self.assertEqual(baseline.id, id)
         self.assertEqual(baseline.name, self._baseline_name)
         self.assertEqual(baseline.type, BaselineType.PRE_PRODUCTION)
         self.assertEqual(baseline.dataset_name, self._dataset_name)
 
-    @patch('fiddler.v2.api.baseline_mixin.RequestClient.post')
+    @patch('fiddler.api.baseline_mixin.RequestClient.post')
     def test_baseline_construction_add_baseline(self, post_request):
         test_ds_id = self._dataset_name
         baseline = self.client.add_baseline(
             self._project_name,
             self._model_name,
             self._baseline_name,
             type=BaselineType.PRE_PRODUCTION,
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_check_version_decorator.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_check_version_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from pytest_mock import MockerFixture
 
 from fiddler.exceptions import NotSupported
-from fiddler.v2.schema.server_info import Version
-from fiddler.v2.utils.decorators import check_version
+from fiddler.schema.server_info import Version
+from fiddler.utils.decorators import check_version
 
 
 def test_with_supported_version(mocker: MockerFixture) -> None:
     @check_version(version_expr='>=23.2.0')
     def func(self):
         pass
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_custom_features.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_dataset_api.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_dataset_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest
 from http import HTTPStatus
 from typing import Dict, List, Tuple
 
-from fiddler.exceptions import NotFound
 from fiddler.core_objects import DatasetInfo as DatasetInfoObj
-from fiddler.v2.schema.dataset import Dataset, DatasetInfo, DatasetIngest
-from tests.v2.base import BaseTestCase
-from tests.v2.helper import (
+from fiddler.exceptions import NotFound
+from fiddler.schema.dataset import Dataset, DatasetInfo, DatasetIngest
+from tests.fiddler.base import BaseTestCase
+from tests.fiddler.helper import (
     get_404_error_response,
     get_base_api_response_body,
     get_base_paginated_api_response_body,
 )
 
 
 class TestDataset(BaseTestCase):
@@ -166,15 +166,14 @@
         url, _ = self._get_url_query_params(self._dataset_name)
         self.requests_mock.get(
             url, json=get_404_error_response(), status=HTTPStatus.NOT_FOUND
         )
         with self.assertRaises(NotFound) as e:  # noqa
             self.client.get_dataset(self._project_name, self._dataset_name)
 
-
     def test_DatasetIngest_creation(self):
         request_body = DatasetIngest(
             name=self._dataset_name,
             file_name=self._file_names,
             info=DatasetInfoObj.from_dict(self._example_info),
         ).to_dict()
         assert request_body['info']['columns'] ==  self._example_info['columns']
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_events_api.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from http import HTTPStatus
 from pathlib import Path
 from unittest import mock
 
 import pandas as pd
 from requests import Response
 
+from fiddler.api.api import FiddlerClient
 from fiddler.constants import FiddlerTimestamp, UploadType
 from fiddler.exceptions import HttpException
-from fiddler.v2.api.api import FiddlerClient
-from tests.v2.base import BaseTestCase
+from tests.fiddler.base import BaseTestCase
 
 
 class TestEventsAPI(BaseTestCase):
     def setUp(self) -> None:
         super(TestEventsAPI, self).setUp()
         self._project_name = 'test_project'
         self._model_name = 'test_model'
@@ -28,17 +28,19 @@
                 'progress': 100.0,
                 'error_message': None,
                 'extras': {},
             },
             'api_version': '2.0',
             'kind': 'NORMAL',
         }
-        self._events_path = Path(__file__).parent.joinpath('data', 'ingest_events.csv')
+        self._events_path = Path(__file__).parent.parent.joinpath(
+            'datasets', 'data', 'ingest_events.csv'
+        )
         self.multipart_upload_patcher = mock.patch(
-            'fiddler.v2.api.events_mixin.multipart_upload'
+            'fiddler.api.events_mixin.multipart_upload'
         ).start()
         self.multipart_upload_patcher.return_value = {
             'status': 'SUCCESS',
             'file_name': 'dataset.csv',
             'message': 'Successfully uploaded to blob',
         }
         self._ingest_url = f'{self._url}/events/{self._org}:{self._project_name}:{self._model_name}/ingest'
@@ -105,15 +107,15 @@
         id_field = None
         is_update = None
         timestamp_field = None
         timestamp_format = None
         group_by = None
         wait = True
         publish_events_patcher = mock.patch(
-            'fiddler.v2.api.events_mixin.EventsMixin.publish_events_batch',
+            'fiddler.api.events_mixin.EventsMixin.publish_events_batch',
         ).start()
         response = {
             'uuid': self._job_uuid,
             'name': 'Ingestion publish events',
             'status': 'SUCCESS',
             'progress': 100.0,
             'error_message': None,
@@ -147,15 +149,15 @@
 
         _, kwargs = publish_events_patcher.call_args
         events = kwargs.get('events_path')
         self.assertIsNotNone(events)
 
     def test_publish_event(self):
         self.requests_mock.stop()
-        client_mocker = mock.patch('fiddler.v2.api.api.RequestClient').start()
+        client_mocker = mock.patch('fiddler.api.api.RequestClient').start()
         client = FiddlerClient(self._url, self._org, 'ssds')
         response = Response()
         response.status_code = HTTPStatus.ACCEPTED
         fiddler_id = 'foo'
         response._content = json.dumps(
             {
                 'data': {
@@ -211,12 +213,14 @@
     def test_publish_event_exception(self):
         self.requests_mock.post(
             url=f'{self._url}/{self._single_event_url}',
             body='this is error',
             status=HTTPStatus.OK,
         )
         with self.assertRaises(HttpException):
-            self.client.publish_event(project_name=self._project_name, model_name=self._model_name, event={})
+            self.client.publish_event(
+                project_name=self._project_name, model_name=self._model_name, event={}
+            )
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_exceptions.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from requests import HTTPError
 
 from fiddler.exceptions import (
     ErrorResponseHandler,
     HttpException,
     BadRequest,
 )
-from fiddler.v2.utils.decorators import handle_api_error_response
+from fiddler.utils.decorators import handle_api_error_response
 
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_explainability_apis.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_explainability_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import unittest
 
 import pandas as pd
 
-from fiddler.v2.api.explainability_mixin import (
+from fiddler.api.explainability_mixin import (
     DatasetDataSource,
     RowDataSource,
     SqlSliceQueryDataSource,
 )
-from tests.v2.base import BaseTestCase
-from tests.v2.helper import get_base_api_response_body
+from tests.fiddler.base import BaseTestCase
+from tests.fiddler.helper import get_base_api_response_body
 
 
 class TestExplainabilityApis(BaseTestCase):
     def setUp(self):
         super().setUp()
         self._project_name = 'test_project'
         self._dataset_name = 'test_dataset'
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_file_upload.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_file_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from http import HTTPStatus
 from pathlib import Path
 from unittest import mock
 from urllib.parse import urljoin
 
 from requests import Response
 
-from fiddler.constants import CONTENT_TYPE_OCTET_STREAM_HEADER, UploadType
-from fiddler.v2.api.helpers import (
+from fiddler.api.helpers import (
     FILE_NAME_KEY,
     MULTIPART_UPLOAD_KEY,
     RESOURCE_IDENT_KEY,
     UPLOAD_ID_KEY,
     UPLOAD_TYPE_KEY,
-    multipart_upload, NUM_ROWS_KEY, NUM_COLS_KEY,
+    multipart_upload,
+    NUM_ROWS_KEY,
+    NUM_COLS_KEY,
 )
-from tests.v2.base import BaseTestCase
+from fiddler.constants import CONTENT_TYPE_OCTET_STREAM_HEADER, UploadType
+from tests.fiddler.base import BaseTestCase
 
 
 class TestFileUpload(BaseTestCase):
     def setUp(self) -> None:
         super(TestFileUpload, self).setUp()
         self.project_name = 'test_project'
         self.file_name = 'foo.csv'
@@ -68,15 +70,17 @@
 
         resp = multipart_upload(
             self.mock_client,
             self._org,
             self.project_name,
             dataset_name,
             upload_type,
-            Path(__file__).parent.joinpath('data', 'dataset_0.csv').as_posix(),
+            Path(__file__)
+            .parent.parent.joinpath('datasets', 'data', 'dataset_0.csv')
+            .as_posix(),
             self.file_name,
         )
 
         self.mock_client.put.assert_called_once()
         _, kwargs = self.mock_client.put.call_args
         self.assertEqual(self.upload_url, kwargs.get('url'))
         self.assertDictEqual(params, kwargs.get('params'))
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_helpers.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fiddler.v2.schema.server_info import Version
-from fiddler.v2.utils.helpers import match_semver
+from fiddler.schema.server_info import Version
+from fiddler.utils.helpers import match_semver
 
 
 def test_match_semvar_version():
     assert match_semver(None, '>=22.9.0') is False
     assert match_semver(Version.parse('22.9.0'), '>=22.10.0') is False
     assert match_semver(Version.parse('22.10.0'), '>=22.10.0') is True
     assert match_semver(Version.parse('22.10.0'), '>22.10.0') is False
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_job.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from typing import Optional
 
 from fiddler.exceptions import AsyncJobFailed
-from fiddler.v2.schema.job import JobStatus
-from tests.v2.base import BaseTestCase
+from fiddler.schema.job import JobStatus
+from tests.fiddler.base import BaseTestCase
 
 
 class TestJob(BaseTestCase):
     def setUp(self) -> None:
         super(TestJob, self).setUp()
         self._job_uuid = '3fa85f64-5717-4562-b3fc-2c963f66afa6'
         self._jobs_url = f'{self._url}/jobs/{self._job_uuid}'
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_model.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
 from typing import Dict, Tuple
 
 from responses import matchers
 
 from fiddler.exceptions import NotFound
-from fiddler.v2.schema.model import Model
-from tests.v2.base import BaseTestCase
-from tests.v2.helper import (
+from fiddler.schema.model import Model
+from tests.fiddler.base import BaseTestCase
+from tests.fiddler.helper import (
     get_404_error_response,
     get_base_api_response_body,
     get_base_paginated_api_response_body,
 )
 
 
 class TestModel(BaseTestCase):
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_project.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from responses import matchers
 
 from fiddler.exceptions import (
     BadRequest,
     Conflict,
     NotFound,
 )
-from fiddler.v2.schema.project import Project
-from tests.v2.base import BaseTestCase
+from fiddler.schema.project import Project
+from tests.fiddler.base import BaseTestCase
 
 
 class TestProject(BaseTestCase):
     def setUp(self):
         super(TestProject, self).setUp()
         self._project_name = 'test_project'
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_response_handler.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_response_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import unittest
 from unittest import mock
 
-from fiddler.v2.utils.response_handler import JobResponseHandler
+from fiddler.utils.response_handler import JobResponseHandler
 
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
 
 from fiddler.exceptions import HttpException
-from fiddler.v2.utils.response_handler import BaseResponseHandler
+from fiddler.utils.response_handler import BaseResponseHandler
 
 
 class TestBaseResponseHandler(unittest.TestCase):
     def setUp(self) -> None:
         self.response = mock.MagicMock()
 
     def test_get_data(self):
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_upload_dataset.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_upload_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from pathlib import Path
 from unittest import mock
 
 import pandas as pd
 
 from fiddler.constants import FileType, UploadType
 from fiddler.exceptions import HttpException
-from fiddler.v2.schema.dataset import DatasetInfo
-from fiddler.v2.schema.server_info import ServerInfo
-from tests.v2.base import BaseTestCase
+from fiddler.schema.dataset import DatasetInfo
+from fiddler.schema.server_info import ServerInfo
+from tests.fiddler.base import BaseTestCase
 
 
 class TestUploadDataset(BaseTestCase):
     def setUp(self) -> None:
         super(TestUploadDataset, self).setUp()
         self._project_name = 'test_project'
         self._dataset_name = 'test_dataset'
@@ -28,15 +28,16 @@
                 'progress': 100.0,
                 'error_message': None,
                 'extras': {},
             },
             'api_version': '2.0',
             'kind': 'NORMAL',
         }
-        self._data_path = Path(__file__).parent.joinpath('data', 'dataset_0.csv')
+        self._datasets_path = Path(__file__).parent.parent.joinpath('datasets', 'data')
+        self._data_path = self._datasets_path.joinpath('dataset_0.csv')
         self._info = DatasetInfo.from_dict(
             {
                 'name': 'some_name',
                 'columns': [
                     {
                         'column-name': 'col0',
                         'data-type': 'int',
@@ -71,15 +72,15 @@
                         ],
                         'is-nullable': False,
                     },
                 ],
             }
         )
         self.multipart_upload_patcher = mock.patch(
-            'fiddler.v2.api.dataset_mixin.multipart_upload'
+            'fiddler.api.dataset_mixin.multipart_upload'
         ).start()
         self.multipart_upload_patcher.return_value = {
             'status': 'SUCCESS',
             'file_name': 'dataset.csv',
             'message': 'Successfully uploaded to blob',
         }
         self._ingest_url = f'{self._url}/datasets/{self._org}:{self._project_name}:{self._dataset_name}/ingest'
@@ -181,15 +182,15 @@
             )
 
     def test_upload_dataset_df(self):
         self.requests_mock.get(
             url=self._get_project_url, json=self._get_project_resp, status=HTTPStatus.OK
         )
         upload_dataset_patcher = mock.patch(
-            'fiddler.v2.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
+            'fiddler.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
         ).start()
         response = {
             'uuid': self._job_uuid,
             'name': 'Ingestion dataset Upload',
             'status': 'SUCCESS',
             'progress': 100.0,
             'error_message': None,
@@ -220,15 +221,15 @@
         self.assertEqual(files['train'].name, 'train.csv')
 
     def test_upload_dataset_df_23_4(self):
         self.requests_mock.get(
             url=self._get_project_url, json=self._get_project_resp, status=HTTPStatus.OK
         )
         upload_dataset_patcher = mock.patch(
-            'fiddler.v2.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
+            'fiddler.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
         ).start()
         response = {
             'uuid': self._job_uuid,
             'name': 'Ingestion dataset Upload',
             'status': 'SUCCESS',
             'progress': 100.0,
             'error_message': None,
@@ -261,55 +262,55 @@
             url=self._ingest_url, json=self._ingest_resp, status=HTTPStatus.ACCEPTED
         )
 
         resp = self.client.upload_dataset_from_file(
             project_name=self._project_name,
             dataset_name=self._dataset_name,
             files={
-                'train': Path(__file__).parent.joinpath('data', 'dataset_0.csv'),
-                'test': Path(__file__).parent.joinpath('data', 'dataset_1.csv'),
+                'train': self._datasets_path.joinpath('dataset_0.csv'),
+                'test': self._datasets_path.joinpath('dataset_1.csv'),
             },
             info=self._info,
             wait=False,
         )
         self.assertDictEqual(self._ingest_resp.get('data'), resp)
 
     def test_upload_dataset_norows(self):
         with self.assertRaises(ValueError) as e:  # noqa
             self.client.upload_dataset_from_file(
                 self._project_name,
                 self._dataset_name,
                 files={
-                    'train': Path(__file__).parent.joinpath('data', 'dataset_2.csv'),
+                    'train': self._datasets_path.joinpath('dataset_2.csv'),
                 },
                 info=self._info,
             )
 
     def test_upload_dataset_nocols(self):
         with self.assertRaises(ValueError) as e:  # noqa
             self.client.upload_dataset_from_file(
                 self._project_name,
                 self._dataset_name,
                 files={
-                    'train': Path(__file__).parent.joinpath('data', 'dataset_4.csv'),
+                    'train': self._datasets_path.joinpath('dataset_4.csv'),
                 },
                 info=self._info,
             )
 
     def test_upload_dataset_df_empty(self):
         with self.assertRaises(ValueError) as e:  # noqa
             _ = self.client.upload_dataset(
                 project_name=self._project_name,
                 dataset_name=self._dataset_name,
                 datasets={},
             )
 
     def test_upload_dataset_csv(self):
         upload_dataset_patcher = mock.patch(
-            'fiddler.v2.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
+            'fiddler.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
         ).start()
         response = {
             'uuid': self._job_uuid,
             'name': 'Ingestion dataset Upload',
             'status': 'SUCCESS',
             'progress': 100.0,
             'error_message': None,
@@ -334,30 +335,29 @@
             info=self._info,
             file_type=FileType.CSV,
             file_schema=None,  # Since we don't support file_schema; file_schema = None
             wait=True,
         )
 
     def test_upload_dataset_from_dir(self):
-        dir_path = Path(__file__).parent.joinpath('data')
         upload_dataset_patcher = mock.patch(
-            'fiddler.v2.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
+            'fiddler.api.dataset_mixin.DatasetMixin.upload_dataset_from_file'
         ).start()
         response = {
             'uuid': self._job_uuid,
             'name': 'Ingestion dataset Upload',
             'status': 'SUCCESS',
             'progress': 100.0,
             'error_message': None,
         }
         upload_dataset_patcher.return_value = response
         output = self.client.upload_dataset_from_dir(
             project_name=self._project_name,
             dataset_name=self._dataset_name,
-            dataset_dir=dir_path,
+            dataset_dir=self._datasets_path,
             file_type=FileType.CSV,
             file_schema=None,
             wait=True,
         )
         self.assertDictEqual(output, response)
         all_args = upload_dataset_patcher.call_args.kwargs
         assert isinstance(all_args['project_name'], str)
```

### Comparing `fiddler-client-2.0.0.dev7/tests/v2/test_validations.py` & `fiddler-client-2.0.0.dev8/tests/fiddler/test_validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tempfile
 from pathlib import Path
 
 import pytest
 
-from fiddler.v2.utils.validations import validate_artifact_dir
+from fiddler.utils.validations import validate_artifact_dir
 
 
 def test_validate_artifact_dir() -> None:
     # No dir
     with pytest.raises(ValueError) as cx:
         validate_artifact_dir(Path('/foo/bar'))
```

