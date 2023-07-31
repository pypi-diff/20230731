# Comparing `tmp/nautobot_device_lifecycle_mgmt-1.3.0.tar.gz` & `tmp/nautobot_device_lifecycle_mgmt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.3.0.tar", max compression
+gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.3.1.tar", max compression
```

## Comparing `nautobot_device_lifecycle_mgmt-1.3.0.tar` & `nautobot_device_lifecycle_mgmt-1.3.1.tar`

### file list

```diff
@@ -1,82 +1,83 @@
--rw-r--r--   0        0        0      591 2023-06-17 20:01:15.064929 nautobot_device_lifecycle_mgmt-1.3.0/LICENSE
--rw-r--r--   0        0        0     5939 2023-06-17 20:01:15.064929 nautobot_device_lifecycle_mgmt-1.3.0/README.md
--rw-r--r--   0        0        0     1418 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/__init__.py
--rw-r--r--   0        0        0       65 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/__init__.py
--rw-r--r--   0        0        0     3052 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
--rw-r--r--   0        0        0    11452 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/serializers.py
--rw-r--r--   0        0        0     1234 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/urls.py
--rw-r--r--   0        0        0     4602 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/views.py
--rw-r--r--   0        0        0     2141 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/choices.py
--rw-r--r--   0        0        0     1188 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/const.py
--rw-r--r--   0        0        0    30000 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/filters.py
--rw-r--r--   0        0        0    40491 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/forms.py
--rw-r--r--   0        0        0      685 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/graphql/types.py
--rw-r--r--   0        0        0      327 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/__init__.py
--rw-r--r--   0        0        0     3191 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
--rw-r--r--   0        0        0     3287 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
--rw-r--r--   0        0        0     9475 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/metrics.py
--rw-r--r--   0        0        0     3449 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
--rw-r--r--   0        0        0     4319 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
--rw-r--r--   0        0        0     5580 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
--rw-r--r--   0        0        0     2378 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
--rw-r--r--   0        0        0     4405 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
--rw-r--r--   0        0        0     4794 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
--rw-r--r--   0        0        0     3131 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
--rw-r--r--   0        0        0     1123 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
--rw-r--r--   0        0        0      612 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
--rw-r--r--   0        0        0      463 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
--rw-r--r--   0        0        0      984 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
--rw-r--r--   0        0        0      902 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
--rw-r--r--   0        0        0        0 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/__init__.py
--rw-r--r--   0        0        0    31202 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/models.py
--rw-r--r--   0        0        0    14180 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/navigation.py
--rw-r--r--   0        0        0     5407 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/signals.py
--rw-r--r--   0        0        0     2995 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software.py
--rw-r--r--   0        0        0     8101 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software_filters.py
--rw-r--r--   0        0        0    20020 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tables.py
--rw-r--r--   0        0        0     4326 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/template_content.py
--rw-r--r--   0        0        0     2094 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
--rw-r--r--   0        0        0     5904 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
--rw-r--r--   0        0        0     2429 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
--rw-r--r--   0        0        0      492 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
--rw-r--r--   0        0        0     2613 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
--rw-r--r--   0        0        0      939 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
--rw-r--r--   0        0        0     1523 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
--rw-r--r--   0        0        0     5632 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
--rw-r--r--   0        0        0     2160 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
--rw-r--r--   0        0        0      513 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
--rw-r--r--   0        0        0     1113 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
--rw-r--r--   0        0        0      747 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
--rw-r--r--   0        0        0      365 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
--rw-r--r--   0        0        0      505 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
--rw-r--r--   0        0        0     3605 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
--rw-r--r--   0        0        0     5075 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
--rw-r--r--   0        0        0      263 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
--rw-r--r--   0        0        0     1971 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
--rw-r--r--   0        0        0       92 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
--rw-r--r--   0        0        0     3138 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
--rw-r--r--   0        0        0      251 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
--rw-r--r--   0        0        0       86 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
--rw-r--r--   0        0        0      392 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
--rw-r--r--   0        0        0     5784 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
--rw-r--r--   0        0        0     5885 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
--rw-r--r--   0        0        0     5686 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
--rw-r--r--   0        0        0      269 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
--rw-r--r--   0        0        0     1942 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
--rw-r--r--   0        0        0       96 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
--rw-r--r--   0        0        0     1599 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
--rw-r--r--   0        0        0      615 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
--rw-r--r--   0        0        0       67 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/__init__.py
--rw-r--r--   0        0        0     5247 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/conftest.py
--rw-r--r--   0        0        0    27988 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_api.py
--rw-r--r--   0        0        0     1535 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py
--rw-r--r--   0        0        0    30831 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py
--rw-r--r--   0        0        0    23393 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py
--rw-r--r--   0        0        0    30032 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_model.py
--rw-r--r--   0        0        0    11840 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
--rw-r--r--   0        0        0    16523 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_views.py
--rw-r--r--   0        0        0    11497 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/urls.py
--rw-r--r--   0        0        0      423 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/utils.py
--rw-r--r--   0        0        0    43490 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/views.py
--rw-r--r--   0        0        0     2771 2023-06-17 20:01:28.468865 nautobot_device_lifecycle_mgmt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-07-31 20:13:08.289233 nautobot_device_lifecycle_mgmt-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5939 2023-07-31 20:13:08.289233 nautobot_device_lifecycle_mgmt-1.3.1/README.md
+-rw-r--r--   0        0        0     1418 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/__init__.py
+-rw-r--r--   0        0        0     3052 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
+-rw-r--r--   0        0        0    11145 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/serializers.py
+-rw-r--r--   0        0        0     1234 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/urls.py
+-rw-r--r--   0        0        0     4602 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/views.py
+-rw-r--r--   0        0        0     2141 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/choices.py
+-rw-r--r--   0        0        0     1188 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/const.py
+-rw-r--r--   0        0        0    29610 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/filters.py
+-rw-r--r--   0        0        0    40734 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/forms.py
+-rw-r--r--   0        0        0      685 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/graphql/types.py
+-rw-r--r--   0        0        0      327 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/__init__.py
+-rw-r--r--   0        0        0     3191 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
+-rw-r--r--   0        0        0     3287 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
+-rw-r--r--   0        0        0     9475 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/metrics.py
+-rw-r--r--   0        0        0     3449 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
+-rw-r--r--   0        0        0     4319 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
+-rw-r--r--   0        0        0     5580 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
+-rw-r--r--   0        0        0     2378 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
+-rw-r--r--   0        0        0     4405 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
+-rw-r--r--   0        0        0     4794 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
+-rw-r--r--   0        0        0     3131 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
+-rw-r--r--   0        0        0     1123 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
+-rw-r--r--   0        0        0      612 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
+-rw-r--r--   0        0        0      463 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
+-rw-r--r--   0        0        0      984 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
+-rw-r--r--   0        0        0      902 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
+-rw-r--r--   0        0        0      568 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/__init__.py
+-rw-r--r--   0        0        0    31341 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/models.py
+-rw-r--r--   0        0        0    14180 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/navigation.py
+-rw-r--r--   0        0        0     5407 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/signals.py
+-rw-r--r--   0        0        0     2995 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software.py
+-rw-r--r--   0        0        0     8101 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software_filters.py
+-rw-r--r--   0        0        0    20020 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tables.py
+-rw-r--r--   0        0        0     5526 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/template_content.py
+-rw-r--r--   0        0        0     2094 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
+-rw-r--r--   0        0        0     5904 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
+-rw-r--r--   0        0        0     2429 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
+-rw-r--r--   0        0        0      492 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     2613 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
+-rw-r--r--   0        0        0      939 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
+-rw-r--r--   0        0        0     1523 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
+-rw-r--r--   0        0        0     5632 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
+-rw-r--r--   0        0        0     2160 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
+-rw-r--r--   0        0        0      513 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
+-rw-r--r--   0        0        0     1113 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
+-rw-r--r--   0        0        0      747 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
+-rw-r--r--   0        0        0      365 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
+-rw-r--r--   0        0        0      505 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     3605 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
+-rw-r--r--   0        0        0     5075 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
+-rw-r--r--   0        0        0      263 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
+-rw-r--r--   0        0        0     1971 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
+-rw-r--r--   0        0        0       92 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
+-rw-r--r--   0        0        0     3138 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
+-rw-r--r--   0        0        0      251 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
+-rw-r--r--   0        0        0       86 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
+-rw-r--r--   0        0        0      392 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
+-rw-r--r--   0        0        0     5784 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
+-rw-r--r--   0        0        0     5885 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
+-rw-r--r--   0        0        0     5686 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
+-rw-r--r--   0        0        0      269 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
+-rw-r--r--   0        0        0     1942 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
+-rw-r--r--   0        0        0       96 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
+-rw-r--r--   0        0        0     1599 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
+-rw-r--r--   0        0        0      615 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
+-rw-r--r--   0        0        0       67 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/__init__.py
+-rw-r--r--   0        0        0     5277 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/conftest.py
+-rw-r--r--   0        0        0    27988 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_api.py
+-rw-r--r--   0        0        0     1535 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_basic.py
+-rw-r--r--   0        0        0    30831 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_filters.py
+-rw-r--r--   0        0        0    23393 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_forms.py
+-rw-r--r--   0        0        0    32901 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_model.py
+-rw-r--r--   0        0        0    11840 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
+-rw-r--r--   0        0        0    16523 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_views.py
+-rw-r--r--   0        0        0    11497 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/urls.py
+-rw-r--r--   0        0        0      423 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/utils.py
+-rw-r--r--   0        0        0    43490 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/views.py
+-rw-r--r--   0        0        0     2771 2023-07-31 20:13:26.713583 nautobot_device_lifecycle_mgmt-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.3.1/PKG-INFO
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/LICENSE` & `nautobot_device_lifecycle_mgmt-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/README.md` & `nautobot_device_lifecycle_mgmt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/__init__.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/serializers.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,59 +3,48 @@
 from nautobot.dcim.api.nested_serializers import (
     NestedDeviceSerializer,
     NestedDeviceTypeSerializer,
     NestedInventoryItemSerializer,
     NestedPlatformSerializer,
 )
 from nautobot.extras.api.customfields import CustomFieldModelSerializer
-from nautobot.extras.api.serializers import (
-    StatusModelSerializerMixin,
-    StatusSerializerField,
-    TaggedObjectSerializer,
-)
-from rest_framework import serializers
-
-# Nautobot 1.4 introduced RelationshipModelSerializerMixin
-# TODO: Remove this once plugin drops support for Nautobot < 1.4
-try:
-    from nautobot.extras.api.relationships import RelationshipModelSerializerMixin  # pylint: disable=ungrouped-imports
-
-    serializer_base_classes = [
-        RelationshipModelSerializerMixin,
-        TaggedObjectSerializer,
-        CustomFieldModelSerializer,
-    ]  # pylint: disable=invalid-name
-except ImportError:
-    serializer_base_classes = [TaggedObjectSerializer, CustomFieldModelSerializer]  # pylint: disable=invalid-name
-
+from nautobot.extras.api.relationships import RelationshipModelSerializerMixin  # pylint: disable=ungrouped-imports
+from nautobot.extras.api.serializers import StatusModelSerializerMixin, StatusSerializerField, TaggedObjectSerializer
 from nautobot.extras.models import Status
+from rest_framework import serializers
 
 from nautobot_device_lifecycle_mgmt import choices
 from nautobot_device_lifecycle_mgmt.models import (
     CVELCM,
     ContactLCM,
     ContractLCM,
+    DeviceSoftwareValidationResult,
     HardwareLCM,
+    InventoryItemSoftwareValidationResult,
     ProviderLCM,
     SoftwareImageLCM,
     SoftwareLCM,
     ValidatedSoftwareLCM,
     VulnerabilityLCM,
-    DeviceSoftwareValidationResult,
-    InventoryItemSoftwareValidationResult,
 )
 
 from .nested_serializers import (
     NestedContractLCMSerializer,
     NestedCVELCMSerializer,
     NestedProviderLCMSerializer,
     NestedSoftwareImageLCMSerializer,
     NestedSoftwareLCMSerializer,
 )
 
+serializer_base_classes = [
+    RelationshipModelSerializerMixin,
+    TaggedObjectSerializer,
+    CustomFieldModelSerializer,
+]  # pylint: disable=invalid-name
+
 
 class HardwareLCMSerializer(*serializer_base_classes):  # pylint: disable=R0901,too-few-public-methods
     """API serializer."""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:nautobot_device_lifecycle_mgmt-api:hardwarelcm-detail"
     )
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/urls.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/views.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/choices.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/const.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/const.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/filters.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 """Filtering implementation for the Lifecycle Management plugin."""
 import datetime
 
 import django_filters
 from django.db.models import Q
-from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Platform, Region, Site, Manufacturer
-from nautobot.extras.filters import StatusFilter, StatusModelFilterSetMixin, TagFilter
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Manufacturer, Platform, Region, Site
+from nautobot.extras.filters import NautobotFilterSet, StatusFilter, StatusModelFilterSetMixin, TagFilter
 from nautobot.extras.models import Tag
 
-try:
-    from nautobot.extras.filters import NautobotFilterSet
-except ImportError:
-    # TODO: Remove once plugin no longer supports Nautobot < 1.4.0
-    from nautobot.extras.filters import CustomFieldModelFilterSet
-    from nautobot.utilities.filters import BaseFilterSet
-
-    class NautobotFilterSet(BaseFilterSet, CustomFieldModelFilterSet):
-        """Emulate NautobotFilterSet from Nautobot 1.4.0 ."""
-
-
 from nautobot_device_lifecycle_mgmt.models import (
     CVELCM,
     ContactLCM,
     ContractLCM,
     DeviceSoftwareValidationResult,
     HardwareLCM,
     InventoryItemSoftwareValidationResult,
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/forms.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 """Forms implementation for the Lifecycle Management plugin."""
 import logging
+
 from django import forms
 from django.db.models import Q
-
-from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Platform, Region, Site, Manufacturer
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Manufacturer, Platform, Region, Site
 from nautobot.extras.forms import (
+    CustomFieldModelBulkEditFormMixin,
     CustomFieldModelCSVForm,
-    CustomFieldModelForm,
-    CustomFieldFilterForm,
-    CustomFieldBulkEditForm,
-    RelationshipModelForm,
-    StatusBulkEditFormMixin,
+    CustomFieldModelFilterFormMixin,
+    CustomFieldModelFormMixin,
+    RelationshipModelFormMixin,
+    StatusModelBulkEditFormMixin,
     StatusModelCSVFormMixin,
-    StatusFilterFormMixin,
+    StatusModelFilterFormMixin,
 )
-from nautobot.extras.models import Tag, Status
+from nautobot.extras.models import Status, Tag
 from nautobot.utilities.forms import (
+    BOOLEAN_WITH_BLANK_CHOICES,
     BootstrapMixin,
     BulkEditForm,
+    CSVModelChoiceField,
     DatePicker,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     StaticSelect2,
-    BOOLEAN_WITH_BLANK_CHOICES,
-    add_blank_choice,
-    CSVModelChoiceField,
     TagFilterField,
+    add_blank_choice,
 )
+
 from nautobot_device_lifecycle_mgmt.choices import (
     ContractTypeChoices,
-    CurrencyChoices,
-    PoCTypeChoices,
     CountryCodes,
+    CurrencyChoices,
     CVESeverityChoices,
+    PoCTypeChoices,
 )
 from nautobot_device_lifecycle_mgmt.models import (
+    CVELCM,
+    ContactLCM,
+    ContractLCM,
+    DeviceSoftwareValidationResult,
     HardwareLCM,
     InventoryItemSoftwareValidationResult,
+    ProviderLCM,
+    SoftwareImageLCM,
     SoftwareLCM,
     ValidatedSoftwareLCM,
-    DeviceSoftwareValidationResult,
-    ContractLCM,
-    ProviderLCM,
-    ContactLCM,
-    CVELCM,
     VulnerabilityLCM,
-    SoftwareImageLCM,
 )
 
 logger = logging.getLogger("nautobot_device_lifecycle_mgmt")
 
 
 class CSVMultipleModelChoiceField(forms.ModelMultipleChoiceField):
     """Reference a list of PKs."""
@@ -59,15 +60,15 @@
         pk_list = []
         if isinstance(value, str):
             pk_list = [val.strip() for val in value.split(",") if val]
 
         return super().prepare_value(pk_list)
 
 
-class HardwareLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class HardwareLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """Hardware Device Lifecycle creation/edit form."""
 
     inventory_item = forms.ModelChoiceField(
         queryset=InventoryItem.objects.exclude(part_id__exact="")
         .distinct()
         .order_by("part_id")
         .values_list("part_id", flat=True),
@@ -181,15 +182,15 @@
     class Meta:
         """Meta attributes for the HardwareLCMCSVForm class."""
 
         model = HardwareLCM
         fields = HardwareLCM.csv_headers
 
 
-class SoftwareLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class SoftwareLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """SoftwareLCM creation/edit form."""
 
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
 
     class Meta:
         """Meta attributes."""
 
@@ -258,15 +259,15 @@
     class Meta:
         """Meta attributes for the SoftwareLCMCSVForm class."""
 
         model = SoftwareLCM
         fields = SoftwareLCM.csv_headers
 
 
-class SoftwareImageLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class SoftwareImageLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """SoftwareImageLCM creation/edit form."""
 
     software = DynamicModelChoiceField(queryset=SoftwareLCM.objects.all(), required=True)
     device_types = DynamicModelMultipleChoiceField(queryset=DeviceType.objects.all(), required=False)
     inventory_items = DynamicModelMultipleChoiceField(queryset=InventoryItem.objects.all(), required=False)
     object_tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
 
@@ -418,15 +419,15 @@
     class Meta:
         """Meta attributes for the SoftwareImageLCMCSVForm class."""
 
         model = SoftwareImageLCM
         fields = SoftwareImageLCM.csv_headers
 
 
-class ValidatedSoftwareLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class ValidatedSoftwareLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """ValidatedSoftwareLCM creation/edit form."""
 
     software = DynamicModelChoiceField(queryset=SoftwareLCM.objects.all(), required=True)
     devices = DynamicModelMultipleChoiceField(queryset=Device.objects.all(), required=False)
     device_types = DynamicModelMultipleChoiceField(queryset=DeviceType.objects.all(), required=False)
     device_roles = DynamicModelMultipleChoiceField(queryset=DeviceRole.objects.all(), required=False)
     inventory_items = DynamicModelMultipleChoiceField(queryset=InventoryItem.objects.all(), required=False)
@@ -467,15 +468,15 @@
         object_tags = self.cleaned_data.get("object_tags")
 
         if sum(obj.count() for obj in (devices, device_types, device_roles, inventory_items, object_tags)) == 0:
             msg = "You need to assign to at least one object."
             self.add_error(None, msg)
 
 
-class ValidatedSoftwareLCMFilterForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class ValidatedSoftwareLCMFilterForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """Filter form to filter searches for SoftwareLCM."""
 
     q = forms.CharField(
         required=False,
         label="Search",
         help_text="Search for start or end date of validity.",
     )
@@ -527,15 +528,15 @@
             "preferred",
             "valid",
             "start_before",
             "start_after",
         ]
 
 
-class DeviceSoftwareValidationResultFilterForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class DeviceSoftwareValidationResultFilterForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """Filter form to filter searches for DeviceSoftwareValidationResult."""
 
     q = forms.CharField(
         required=False,
         label="Search",
     )
     software = DynamicModelMultipleChoiceField(
@@ -604,15 +605,17 @@
             "device_type",
             "device_role",
             "exclude_sw_missing",
             "sw_missing_only",
         ]
 
 
-class InventoryItemSoftwareValidationResultFilterForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class InventoryItemSoftwareValidationResultFilterForm(
+    BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin
+):
     """Filter form to filter searches for InventoryItemSoftwareValidationResult."""
 
     q = forms.CharField(
         required=False,
         label="Search",
     )
     software = DynamicModelMultipleChoiceField(
@@ -736,15 +739,15 @@
     class Meta:
         """Meta attributes for the ValidatedSoftwareLCM class."""
 
         model = ValidatedSoftwareLCM
         fields = ValidatedSoftwareLCM.csv_headers
 
 
-class ContractLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class ContractLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """Device Lifecycle Contracts creation/edit form."""
 
     provider = forms.ModelChoiceField(
         queryset=ProviderLCM.objects.all(),
         label="Vendor",
         to_field_name="pk",
         required=True,
@@ -849,15 +852,15 @@
     class Meta:
         """Meta attributes for the ContractLCMCSVForm class."""
 
         model = ContractLCM
         fields = ContractLCM.csv_headers
 
 
-class ProviderLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class ProviderLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """Device Lifecycle Contract Providers creation/edit form."""
 
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
     country = forms.ChoiceField(
         widget=StaticSelect2,
         required=False,
         choices=add_blank_choice(CountryCodes.CHOICES),
@@ -939,15 +942,15 @@
     class Meta:
         """Meta attributes for the ProviderLCMCSVForm class."""
 
         model = ProviderLCM
         fields = ProviderLCM.csv_headers
 
 
-class ContactLCMForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class ContactLCMForm(BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """Device Lifecycle Contract Resources creation/edit form."""
 
     type = forms.ChoiceField(choices=PoCTypeChoices.CHOICES, required=False)
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
 
     class Meta:
         """Meta attributes for the ContactLCMForm class."""
@@ -1025,15 +1028,15 @@
     class Meta:
         """Meta attributes for the ContactLCMCSVForm class."""
 
         model = ContactLCM
         fields = ContactLCM.csv_headers
 
 
-class CVELCMForm(StatusBulkEditFormMixin, BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class CVELCMForm(StatusModelBulkEditFormMixin, BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin):
     """CVE Lifecycle Management creation/edit form."""
 
     published_date = forms.DateField(widget=DatePicker())
     severity = forms.ChoiceField(choices=CVESeverityChoices.CHOICES, label="Severity", required=False)
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
 
     model = CVELCM
@@ -1049,15 +1052,15 @@
         ]
 
         widgets = {
             "published_date": DatePicker(),
         }
 
 
-class CVELCMBulkEditForm(StatusBulkEditFormMixin, BootstrapMixin, CustomFieldBulkEditForm):
+class CVELCMBulkEditForm(StatusModelBulkEditFormMixin, BootstrapMixin, CustomFieldModelBulkEditFormMixin):
     """CVE Lifecycle Management bulk edit form."""
 
     model = CVELCM
     pk = forms.ModelMultipleChoiceField(queryset=CVELCM.objects.all(), widget=forms.MultipleHiddenInput)
     description = forms.CharField(required=False)
     comments = forms.CharField(required=False)
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
@@ -1069,15 +1072,15 @@
             "description",
             "comments",
             "status",
             "tags",
         ]
 
 
-class CVELCMFilterForm(BootstrapMixin, StatusFilterFormMixin, CustomFieldFilterForm):
+class CVELCMFilterForm(BootstrapMixin, StatusModelFilterFormMixin, CustomFieldModelFilterFormMixin):
     """Filter form to filter searches for CVELCM."""
 
     model = CVELCM
     q = forms.CharField(
         required=False,
         label="Search",
         help_text="Search for name or link.",
@@ -1131,15 +1134,17 @@
     class Meta:
         """Meta attributes for the CVELCMCSVForm class."""
 
         model = CVELCM
         fields = CVELCM.csv_headers
 
 
-class VulnerabilityLCMForm(StatusBulkEditFormMixin, BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
+class VulnerabilityLCMForm(
+    StatusModelBulkEditFormMixin, BootstrapMixin, CustomFieldModelFormMixin, RelationshipModelFormMixin
+):
     """Vulnerability Lifecycle Management creation/edit form."""
 
     model = VulnerabilityLCM
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
 
     class Meta:
         """Meta attributes for the VulnerabilityLCMForm class."""
@@ -1148,15 +1153,15 @@
 
         fields = [
             "status",
             "tags",
         ]
 
 
-class VulnerabilityLCMBulkEditForm(StatusBulkEditFormMixin, BootstrapMixin, CustomFieldBulkEditForm):
+class VulnerabilityLCMBulkEditForm(StatusModelBulkEditFormMixin, BootstrapMixin, CustomFieldModelBulkEditFormMixin):
     """Vulnerability Lifecycle Management bulk edit form."""
 
     model = VulnerabilityLCM
     pk = forms.ModelMultipleChoiceField(queryset=VulnerabilityLCM.objects.all(), widget=forms.MultipleHiddenInput)
     tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
 
     class Meta:
@@ -1164,15 +1169,15 @@
 
         nullable_fields = [
             "status",
             "tags",
         ]
 
 
-class VulnerabilityLCMFilterForm(BootstrapMixin, StatusFilterFormMixin, CustomFieldFilterForm):
+class VulnerabilityLCMFilterForm(BootstrapMixin, StatusModelFilterFormMixin, CustomFieldModelFilterFormMixin):
     """Filter form to filter searches for VulnerabilityLCM."""
 
     model = VulnerabilityLCM
     q = forms.CharField(
         required=False,
         label="Search",
         help_text="Search for name or link.",
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/graphql/types.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/graphql/types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/metrics.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/models.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.db import models
 from django.urls import reverse
 from django.core.exceptions import ValidationError
 from django.conf import settings
 from nautobot.extras.utils import extras_features
 from nautobot.extras.models.statuses import StatusField
 from nautobot.core.models.generics import PrimaryModel, OrganizationalModel
-from nautobot.dcim.models import Device, InventoryItem
+from nautobot.dcim.models import Device, DeviceType, InventoryItem
 from nautobot.utilities.querysets import RestrictedQuerySet
 
 from nautobot_device_lifecycle_mgmt import choices
 from nautobot_device_lifecycle_mgmt.software_filters import (
     DeviceValidatedSoftwareFilter,
     InventoryItemValidatedSoftwareFilter,
     DeviceSoftwareFilter,
@@ -267,15 +267,15 @@
 class SoftwareImageLCM(PrimaryModel):
     """SoftwareImageLCM model."""
 
     image_file_name = models.CharField(blank=False, max_length=100, verbose_name="Image File Name")
     software = models.ForeignKey(
         to="SoftwareLCM", on_delete=models.CASCADE, related_name="software_images", verbose_name="Software Version"
     )
-    device_types = models.ManyToManyField(to="dcim.DeviceType", related_name="+", blank=True)
+    device_types = models.ManyToManyField(to="dcim.DeviceType", related_name="software_images", blank=True)
     inventory_items = models.ManyToManyField(to="dcim.InventoryItem", related_name="+", blank=True)
     object_tags = models.ManyToManyField(to="extras.Tag", related_name="+", blank=True)
     download_url = models.URLField(blank=True, verbose_name="Download URL")
     image_file_checksum = models.CharField(blank=True, max_length=256, verbose_name="Image File Checksum")
     hashing_algorithm = models.CharField(default="", blank=True, max_length=32, verbose_name="Hashing Algorithm")
     default_image = models.BooleanField(verbose_name="Default Image", default=False)
 
@@ -331,14 +331,16 @@
         """Return all `ValidatedSoftwareLCM` assigned to the given object."""
         if not isinstance(obj, models.Model):
             raise TypeError(f"{obj} is not an instance of Django Model class")
         if isinstance(obj, Device):
             qs = DeviceValidatedSoftwareFilter(qs=self, item_obj=obj).filter_qs()
         elif isinstance(obj, InventoryItem):
             qs = InventoryItemValidatedSoftwareFilter(qs=self, item_obj=obj).filter_qs()
+        elif isinstance(obj, DeviceType):
+            qs = ValidatedSoftwareLCM.objects.filter(device_types=obj)
         else:
             qs = self
 
         return qs
 
 
 @extras_features(
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/navigation.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/signals.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tables.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/template_content.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/template_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Extended core templates for the Lifecycle Management plugin."""
 from abc import ABCMeta
 
 from django.db.models import Q
 
 from nautobot.extras.plugins import PluginTemplateExtension
 from nautobot.dcim.models import InventoryItem
-from .models import HardwareLCM
+from .models import HardwareLCM, ValidatedSoftwareLCM
 from .software import (
     DeviceSoftware,
     InventoryItemSoftware,
 )
+from .tables import ValidatedSoftwareLCMTable
 
 
 class DeviceTypeHWLCM(PluginTemplateExtension, metaclass=ABCMeta):
     """Class to add table for HardwareLCM related to device type."""
 
     model = "dcim.devicetype"
 
@@ -23,14 +24,47 @@
 
         return self.render(
             "nautobot_device_lifecycle_mgmt/inc/general_notice.html",
             extra_context={"hw_notices": HardwareLCM.objects.filter(device_type=devtype_obj.pk)},
         )
 
 
+class DeviceTypeValidatedSoftwareLCM(
+    PluginTemplateExtension,
+):  # pylint: disable=abstract-method
+    """Class to add table for ValidatedSoftwareLCM related to device type."""
+
+    model = "dcim.devicetype"
+
+    def __init__(self, context):
+        """Init setting up the DeviceTypeValidatedSoftwareLCM object."""
+        super().__init__(context)
+        self.device_type_validated_software = ValidatedSoftwareLCM.objects.get_for_object(self.context["object"])
+        self.validated_software_table = ValidatedSoftwareLCMTable(
+            list(self.device_type_validated_software),
+            orderable=False,
+            exclude=(
+                "software",
+                "start",
+                "actions",
+            ),
+        )
+
+    def right_page(self):
+        """Display table on right side of page."""
+        extra_context = {
+            "validsoft_table": self.validated_software_table,
+        }
+
+        return self.render(
+            "nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html",
+            extra_context=extra_context,
+        )
+
+
 class DeviceHWLCM(PluginTemplateExtension, metaclass=ABCMeta):
     """Class to add table for DeviceHWLCM related to device type."""
 
     model = "dcim.device"
 
     def right_page(self):
         """Display table on right side of page."""
@@ -116,12 +150,13 @@
             "nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html",
             extra_context=extra_context,
         )
 
 
 template_extensions = [
     DeviceTypeHWLCM,
+    DeviceTypeValidatedSoftwareLCM,
     DeviceHWLCM,
     InventoryItemHWLCM,
     DeviceSoftwareLCMAndValidatedSoftwareLCM,
     InventoryItemSoftwareLCMAndValidatedSoftwareLCM,
 ]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/conftest.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from nautobot_device_lifecycle_mgmt.models import CVELCM, SoftwareLCM, ValidatedSoftwareLCM
 
 
 def create_devices():
     """Create devices for tests."""
     device_platform, _ = Platform.objects.get_or_create(name="Cisco IOS", slug="cisco_ios")
     manufacturer, _ = Manufacturer.objects.get_or_create(slug="cisco")
-    device_type = DeviceType.objects.create(manufacturer=manufacturer, model="6509-E", slug="6509-e")
-    device_role = DeviceRole.objects.create(name="Core Switch", slug="core-switch")
-    site = Site.objects.create(name="Test 1", slug="test-1")
+    device_type, _ = DeviceType.objects.get_or_create(manufacturer=manufacturer, model="6509-E", slug="6509-e")
+    device_role, _ = DeviceRole.objects.get_or_create(name="Core Switch", slug="core-switch")
+    site, _ = Site.objects.get_or_create(name="Test 1", slug="test-1")
     status_active = Status.objects.get(slug="active")
 
     return (
         Device.objects.create(
             name="sw1",
             platform=device_platform,
             device_type=device_type,
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_api.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_model.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,29 +176,31 @@
             "https://www.cisco.com/c/en/us/support/ios-nx-os-software/ios-15-4m-t/series.html",
         )
         self.assertEqual(softwarelcm_full.long_term_support, False)
         self.assertEqual(softwarelcm_full.pre_release, True)
         self.assertEqual(str(softwarelcm_full), f"{self.device_platform.name} - {softwarelcm_full.version}")
 
 
-class ValidatedSoftwareLCMTestCase(TestCase):
+class ValidatedSoftwareLCMTestCase(TestCase):  # pylint: disable=too-many-instance-attributes
     """Tests for the ValidatedSoftwareLCM model."""
 
     def setUp(self):
         """Set up base objects."""
         device_platform = Platform.objects.create(name="Cisco IOS", slug="cisco_ios")
         self.software = SoftwareLCM.objects.create(
             device_platform=device_platform,
             version="17.3.3 MD",
             release_date=date(2019, 1, 10),
         )
         manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
         self.device_type_1 = DeviceType.objects.create(manufacturer=manufacturer, model="ASR-1000", slug="asr-1000")
         self.device_type_2 = DeviceType.objects.create(manufacturer=manufacturer, model="CAT-3750", slug="cat-3750")
         self.content_type_devicetype = ContentType.objects.get(app_label="dcim", model="devicetype")
+        self.device_1, self.device_2 = create_devices()[:2]
+        self.inventoryitem_1, self.inventoryitem_2 = create_inventory_items()[:2]
 
     def test_create_validatedsoftwarelcm_required_only(self):
         """Successfully create ValidatedSoftwareLCM with required fields only."""
 
         validatedsoftwarelcm = ValidatedSoftwareLCM(
             software=self.software,
             start=date(2019, 1, 10),
@@ -264,14 +266,71 @@
             self.assertEqual(validatedsoftwarelcm_start_only.valid, True)
             self.assertEqual(validatedsoftwarelcm_start_end.valid, False)
 
         with time_machine.travel(date_start_valid):
             self.assertEqual(validatedsoftwarelcm_start_only.valid, True)
             self.assertEqual(validatedsoftwarelcm_start_end.valid, True)
 
+    def test_get_for_object_device(self):
+        validatedsoftwarelcm_1 = ValidatedSoftwareLCM(
+            software=self.software,
+            start=date(2019, 1, 10),
+        )
+        validatedsoftwarelcm_1.devices.set([self.device_1])
+        validatedsoftwarelcm_1.save()
+
+        validatedsoftwarelcm_2 = ValidatedSoftwareLCM(
+            software=self.software,
+            start=date(2018, 1, 10),
+        )
+        validatedsoftwarelcm_2.devices.set([self.device_2])
+        validatedsoftwarelcm_2.save()
+
+        validated_software_for_device = ValidatedSoftwareLCM.objects.get_for_object(self.device_1)
+        self.assertEqual(validated_software_for_device.count(), 1)
+        self.assertTrue(self.device_1 in validated_software_for_device.first().devices.all())
+
+    def test_get_for_object_devicetype(self):
+        validatedsoftwarelcm_1 = ValidatedSoftwareLCM(
+            software=self.software,
+            start=date(2019, 1, 10),
+        )
+        validatedsoftwarelcm_1.device_types.set([self.device_type_1])
+        validatedsoftwarelcm_1.save()
+
+        validatedsoftwarelcm_2 = ValidatedSoftwareLCM(
+            software=self.software,
+            start=date(2018, 1, 10),
+        )
+        validatedsoftwarelcm_2.device_types.set([self.device_type_2])
+        validatedsoftwarelcm_2.save()
+
+        validated_software_for_device_type = ValidatedSoftwareLCM.objects.get_for_object(self.device_type_1)
+        self.assertEqual(validated_software_for_device_type.count(), 1)
+        self.assertTrue(self.device_type_1 in validated_software_for_device_type.first().device_types.all())
+
+    def test_get_for_object_inventoryitem(self):
+        validatedsoftwarelcm_1 = ValidatedSoftwareLCM(
+            software=self.software,
+            start=date(2019, 1, 10),
+        )
+        validatedsoftwarelcm_1.inventory_items.set([self.inventoryitem_1])
+        validatedsoftwarelcm_1.save()
+
+        validatedsoftwarelcm_2 = ValidatedSoftwareLCM(
+            software=self.software,
+            start=date(2018, 1, 10),
+        )
+        validatedsoftwarelcm_2.inventory_items.set([self.inventoryitem_2])
+        validatedsoftwarelcm_2.save()
+
+        validated_software_for_inventoryitem = ValidatedSoftwareLCM.objects.get_for_object(self.inventoryitem_1)
+        self.assertEqual(validated_software_for_inventoryitem.count(), 1)
+        self.assertTrue(self.inventoryitem_1 in validated_software_for_inventoryitem.first().inventory_items.all())
+
 
 class DeviceSoftwareValidationResultTestCase(TestCase):  # pylint: disable=too-many-instance-attributes
     """Tests for the DeviceSoftwareValidationResult model."""
 
     def setUp(self):
         """Set up test objects."""
         self.device = create_devices()[0]
@@ -555,23 +614,27 @@
         self.assertEqual(softwareimage.image_file_checksum, "441rfabd75b0512r7fde7a7a66faa596")
         self.assertEqual(softwareimage.default_image, True)
         self.assertEqual(list(softwareimage.device_types.all()), [self.device_type_1])
         self.assertEqual(list(softwareimage.inventory_items.all()), [self.inventory_item])
         self.assertEqual(list(softwareimage.object_tags.all()), [self.tag])
         self.assertEqual(str(softwareimage), f"{softwareimage.image_file_name}")
 
-    def test_validatedsoftwarelcm_valid_property(self):
-        """Test behavior of the 'valid' property."""
-        validatedsoftwarelcm_start_only = ValidatedSoftwareLCM(
+    def test_get_software_images_for_device_type(self):
+        """Test related reverse relationship from device type to software image"""
+        softwareimage = SoftwareImageLCM(
+            image_file_name="ios17.3.3md.img",
             software=self.software,
-            start=date(2020, 4, 15),
-            preferred=False,
+            download_url="ftp://images.local/cisco/ios17.3.3md.img",
+            image_file_checksum="441rfabd75b0512r7fde7a7a66faa596",
+            default_image=False,
         )
-        validatedsoftwarelcm_start_only.device_types.set([self.device_type_1])
-        validatedsoftwarelcm_start_only.save()
+        softwareimage.device_types.set([self.device_type_1])
+        softwareimage.save()
+
+        self.assertEqual(list(self.device_type_1.software_images.all()), [softwareimage])
 
 
 class ProviderLCMTestCase(TestCase):
     """Tests for the HardwareLCM models."""
 
     def test_provider_creation(self):
         provider = ProviderLCM.objects.create(
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_views.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/urls.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/views.py` & `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/pyproject.toml` & `nautobot_device_lifecycle_mgmt-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-device-lifecycle-mgmt"
-version = "v1.3.0"
+version = "v1.3.1"
 description = "Manages device lifecycles for platforms and software."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 repository = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.0/PKG-INFO` & `nautobot_device_lifecycle_mgmt-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-device-lifecycle-mgmt
-Version: 1.3.0
+Version: 1.3.1
 Summary: Manages device lifecycles for platforms and software.
 Home-page: https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 1.3.0
+Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 1.3.1
 Summary: Manages device lifecycles for platforms and software. Home-page:
 https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt License:
 Apache-2.0 Keywords: nautobot,nautobot-plugin Author: Network to Code, LLC
 Author-email: opensource@networktocode.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

