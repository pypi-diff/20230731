# Comparing `tmp/datarobot_early_access-3.3.0.2023.7.24.tar.gz` & `tmp/datarobot_early_access-3.3.0.2023.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.3.0.2023.7.24.tar", last modified: Mon Jul 24 16:46:36 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.3.0.2023.7.31.tar", last modified: Mon Jul 31 16:46:38 2023, max compression
```

## Comparing `datarobot_early_access-3.3.0.2023.7.24.tar` & `datarobot_early_access-3.3.0.2023.7.31.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   180164 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5712 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2332 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/data_matching.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/dataset.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2346 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4428 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/recipe_operations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8990 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/recipes.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21331 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26065 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4140 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19691 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    66977 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11096 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13004 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33397 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59836 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17013 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18064 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59131 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5688 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94652 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18187 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21166 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5106 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   281784 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215815 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5049 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10126 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7236 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6168 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24079 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12513 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5976 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1154 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-07-24 16:46:36.000000 datarobot_early_access-3.3.0.2023.7.24/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-07-24 16:46:14.000000 datarobot_early_access-3.3.0.2023.7.24/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   180594 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5712 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2332 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/dataset.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2346 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4428 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8990 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21331 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26065 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4140 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19691 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    66977 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11096 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13004 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33397 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59836 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17013 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18064 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59131 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5688 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94652 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18187 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21166 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5106 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   282375 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215815 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5049 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10126 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7236 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6168 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24079 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12513 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5976 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1154 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-07-31 16:46:38.000000 datarobot_early_access-3.3.0.2023.7.31/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-07-31 16:46:15.000000 datarobot_early_access-3.3.0.2023.7.31/setup_weekly.py
```

### Comparing `datarobot_early_access-3.3.0.2023.7.24/CHANGES.rst` & `datarobot_early_access-3.3.0.2023.7.31/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 - Fixed incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
 - Fixed a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 - Fixed an issue where failed authentication when invoking `datarobot.client.Client()` raises a misleading error about client-server compatibility.
 
 API Changes
 ***********
 - Added parameter ``unsupervised_type`` to the class :class:`DatetimePartitioning <datarobot.DatetimePartitioning>`.
+- The sliced insight API endpoint `GET: api/v2/insights/<insight_name>/` returns a paginated response. This means that it returns an empty response if no insights data is found, unlike `GET: api/v2/projects/<pid>/models/<lid>/<insight_name>/`, which returns 404 NOT FOUND in this case. To maintain backwards-compatibility, all methods that retrieve insights data raise 404 NOT FOUND if the insights API returns an empty response.
 
 Deprecation Summary
 *******************
 - ``Model.get_feature_fit_metadata`` has been removed.
   Use :meth:`Model.get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>` instead.
 - ``DatetimeModel.get_feature_fit_metadata`` has been removed.
   Use :meth:`DatetimeModel.get_feature_effect_metadata <datarobot.models.DatetimeModel.get_feature_effect_metadata>` instead.
```

### Comparing `datarobot_early_access-3.3.0.2023.7.24/LICENSE.txt` & `datarobot_early_access-3.3.0.2023.7.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/PKG-INFO` & `datarobot_early_access-3.3.0.2023.7.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.3.0.2023.7.24
+Version: 3.3.0.2023.7.31
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.3.0.2023.7.24/README.md` & `datarobot_early_access-3.3.0.2023.7.31/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/common_setup.py` & `datarobot_early_access-3.3.0.2023.7.31/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/__init__.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_compat.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/dataset.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/enums.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/notebooks.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/recipe_operations.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/recipe_operations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/recipes.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/recipes.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/analytics.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/client.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/context.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/enums.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/errors.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/__init__.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/__init__.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/api_object.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/application.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/batch_job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/blueprint.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/calendar_file.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/change_request.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/cluster.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/connector.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/credential.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_model.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_task.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_slice.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_source.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/data_store.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/dataset.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/driver.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/execution_environment.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_effect.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/feature_impact.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/featurelist.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/imported_model.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/lift_chart.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/missing_report.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/model.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,18 +1002,21 @@
         response = self._client.post(url, data=data)
         job_id = get_id_from_response(response)
         return PredictJob.from_id(self.project_id, job_id)
 
     def _raise_if_not_slice_forbidden_error(self, e: Exception) -> None:
         """If the user does not have the SLICED_INSIGHTS feature flag enabled, then all requests to
         the /insights/ endpoints will be rejected with 403 FORBIDDEN. Also, some project types
-        are currently not supported by the /insights/ endpoint. Use this method to check the
-        error for that case. For any other error, reraise.
+        are currently not supported by the /insights/ endpoint. In addition, datarobot version < 9.1
+        does not support `unslicedOnly` query parameter and returns 400 BAD REQUEST for such requests.
+        Use this method to check the error for that case. For any other error, reraise.
         """
-        if e.status_code not in [403, 422]:
+        if (e.status_code not in [403, 422]) and not (
+            e.json.get("message") == {"unslicedOnly": "unslicedOnly is not allowed key"}
+        ):
             raise e
 
     def _post_insights_url(self, insight_name: str) -> str:
         """Build URL for requests to POST /insights/.../ endpoints, used with sliced insights."""
         return self._base_insights_template.format(insight_name)
 
     def _get_insights_url(self, insight_name: str) -> str:
@@ -1131,14 +1134,19 @@
 
         insight_name = "featureImpact"
         params = self._data_slice_to_query_params(data_slice_filter)
 
         try:
             insights_fi_url = self._get_insights_url(insight_name)
             paginated_response = self._client.get(insights_fi_url, params=params).json()
+            # if the insights API returns an empty response, raise 404
+            # to maintain backwards-compatibility of this function
+            if not paginated_response["data"]:
+                error_msg = f"No feature impact data found for model {self.id}."
+                raise ClientError(exc_message=error_msg, status_code=404)
             data = paginated_response["data"][0]
             use_insights_format = True
         except ClientError as e:
             self._raise_if_not_slice_forbidden_error(e)
             data = self._client.get(self._get_feature_impact_url()).json()
             use_insights_format = False
```

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/modeljob.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/pareto_front.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/predict_job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prediction_server.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/predictions.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/prime_file.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/project.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/project_options.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/rating_table.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/recommended_model.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/residuals.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/roc_curve.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/ruleset.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/segmentation.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/shap_impact.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/sharing.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/status_check_job.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/trafarets.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/training_predictions.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/types.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/use_cases/use_case.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/validators.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/images.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/models/word_cloud.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/rest.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/__init__.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/deprecation.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/pagination.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/retry.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/source.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot/utils/waiters.py` & `datarobot_early_access-3.3.0.2023.7.31/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.3.0.2023.7.24
+Version: 3.3.0.2023.7.31
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.3.0.2023.7.31/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/pyproject.toml` & `datarobot_early_access-3.3.0.2023.7.31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/setup.py` & `datarobot_early_access-3.3.0.2023.7.31/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.3.0.2023.7.24/setup_weekly.py` & `datarobot_early_access-3.3.0.2023.7.31/setup_weekly.py`

 * *Files identical despite different names*

