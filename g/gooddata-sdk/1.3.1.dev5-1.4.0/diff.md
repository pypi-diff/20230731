# Comparing `tmp/gooddata-sdk-1.3.1.dev5.tar.gz` & `tmp/gooddata-sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-sdk-1.3.1.dev5.tar", last modified: Fri Jun 23 15:18:33 2023, max compression
+gzip compressed data, was "gooddata-sdk-1.4.0.tar", last modified: Mon Jul 31 09:28:11 2023, max compression
```

## Comparing `gooddata-sdk-1.3.1.dev5.tar` & `gooddata-sdk-1.4.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.318357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.318357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/catalog_service_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/sql_column.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/content_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/model_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    42925 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.318357 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-23 15:18:25.000000 gooddata-sdk-1.3.1.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/tests/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.484841 gooddata-sdk-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-07-31 09:27:55.000000 gooddata-sdk-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-31 09:28:11.484841 gooddata-sdk-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.468840 gooddata-sdk-1.4.0/gooddata_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/catalog_service_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/sql_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.472840 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/validation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/export/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/export/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/entity_model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.476841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/entity_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/entity_model/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/content_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.480841 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/model_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43496 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.484841 gooddata-sdk-1.4.0/gooddata_sdk/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.484841 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/compute/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/gooddata_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.468840 gooddata-sdk-1.4.0/gooddata_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-31 09:28:11.000000 gooddata-sdk-1.4.0/gooddata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-31 09:28:11.000000 gooddata-sdk-1.4.0/gooddata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:28:11.000000 gooddata-sdk-1.4.0/gooddata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 09:28:11.000000 gooddata-sdk-1.4.0/gooddata_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 09:28:11.000000 gooddata-sdk-1.4.0/gooddata_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:28:11.484841 gooddata-sdk-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:11.484841 gooddata-sdk-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-31 09:27:56.000000 gooddata-sdk-1.4.0/tests/test_type_converter.py
```

### Comparing `gooddata-sdk-1.3.1.dev5/LICENSE.txt` & `gooddata-sdk-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/PKG-INFO` & `gooddata-sdk-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.3.1.dev5
+Version: 1.4.0
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev5
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.4.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoodData Python SDK
 
 The `gooddata-sdk` package provides a clean and convenient Python API to interact with [GoodData](https://www.gooddata.com/).
 
@@ -34,15 +34,15 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.3) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.4.0) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
 -  Python 3.7 or newer
 
 ## Installation
```

### Comparing `gooddata-sdk-1.3.1.dev5/README.md` & `gooddata-sdk-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.3) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.4.0) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
 -  Python 3.7 or newer
 
 ## Installation
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/__init__.py` & `gooddata-sdk-1.4.0/gooddata_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/base.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/catalog_service_base.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/catalog_service_base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/data_source.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/data_source.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/entity_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/data_source.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/data_source/validation/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/entity.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/entity.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/request.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/export/request.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,28 +48,50 @@
     @staticmethod
     def client_class() -> Type[ApiSettings]:
         return ApiSettings
 
 
 @attr.s(auto_attribs=True, kw_only=True)
 class ExportRequest(Base):
+    """
+    ExportRequest class is used to create an export request in the desired format, filename, and settings.
+    Attributes:
+        format (str): The format of the output file (CSV, XLSX).
+        execution_result (str): Execution result id from backend.
+        file_name (str): The name of the output file.
+        settings (Optional[Dict[str, bool]]): Optional dictionary containing settings for the export request.
+        custom_override (Optional[Dict[str, Any]]): Optional dictionary containing custom settings.
+    """
+
     format: str
-    # execution result id from backend
     execution_result: str
     file_name: str
     settings: Optional[ExportSettings] = None
     custom_override: Optional[ExportCustomOverride] = None
 
     def __attrs_post_init__(self) -> None:
+        """
+        Validates that the provided format is supported and raises ValueError if not.
+        """
         supported_formats = ["CSV", "XLSX"]
         if self.format not in supported_formats:
             raise ValueError(
                 f"format '{self.format}' is not presented " f"in supported formats {','.join(supported_formats)}"
             )
 
     @staticmethod
     def client_class() -> Type[TabularExportRequest]:
+        """
+        Returns the appropriate client class for the tabular export request.
+        Returns:
+            Type[TabularExportRequest]: TabularExportRequest class
+        """
         return TabularExportRequest
 
     @property
     def file(self) -> str:
+        """
+        Generates the full filename with the format extension.
+        Returns:
+            str: Full filename with the format extension.
+        """
         return f"{self.file_name}.{self.format.lower()}"
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/identifier.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/identifier.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/organization.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/entity_model/organization.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/organization/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/permission.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/declarative_model/permission.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/permission/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,16 @@
             dashboard_id (str):
                 Dashboard identification string. e.g. "campaign"
         Returns:
             CatalogAvailableAssignees:
                 Object containing users and user groups
         """
         return CatalogAvailableAssignees.from_dict(
-            self._actions_api.available_assignes(workspace_id, dashboard_id, _check_return_type=False), camel_case=False
+            self._actions_api.available_assignees(workspace_id, dashboard_id, _check_return_type=False),
+            camel_case=False,
         )
 
     def list_dashboard_permissions(self, workspace_id: str, dashboard_id: str) -> CatalogDashboardPermissions:
         """Provide list of users and user groups with granted dashboard permissions for particular dashboard
 
         Args:
             workspace_id (str):
@@ -71,15 +72,16 @@
             dashboard_id (str):
                 Dashboard identification string. e.g. "campaign"
         Returns:
             CatalogDashboardPermissions:
                 Object containing users and user groups and granted dashboard permissions
         """
         return CatalogDashboardPermissions.from_dict(
-            self._actions_api.permissions(workspace_id, dashboard_id, _check_return_type=False), camel_case=False
+            self._actions_api.dashboard_permissions(workspace_id, dashboard_id, _check_return_type=False),
+            camel_case=False,
         )
 
     def manage_dashboard_permissions(
         self, workspace_id: str, dashboard_id: str, permissions_for_assignee: List[CatalogPermissionsForAssignee]
     ) -> None:
         """Provide managing dashboard permissions for user and user groups.
 
@@ -90,13 +92,13 @@
                 Dashboard identification string. e.g. "campaign"
             permissions_for_assignee ([CatalogPermissionsForAssignee]):
                 Object containing List of users and user group and desired dashboard permissions. Set empty list
                 permissions for user/user group means remove dashboard permissions.
         Returns:
             None
         """
-        self._actions_api.manage_permissions(
+        self._actions_api.manage_dashboard_permissions(
             workspace_id,
             dashboard_id,
             [permission.to_api() for permission in permissions_for_assignee],
             _check_return_type=False,
         )
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/setting.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_group.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/declarative_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/entity_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user_group.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/entity_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/user/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from gooddata_sdk.catalog.user.declarative_model.user_group import CatalogDeclarativeUserGroups
 from gooddata_sdk.catalog.user.entity_model.user import CatalogUser, CatalogUserDocument
 from gooddata_sdk.catalog.user.entity_model.user_group import CatalogUserGroup, CatalogUserGroupDocument
 from gooddata_sdk.utils import load_all_entities, load_all_entities_dict
 
 
 class CatalogUserService(CatalogServiceBase):
-
     # Entity methods for users
 
     def create_or_update_user(self, user: CatalogUser) -> None:
         """Creates a new user or overwrites an existing user.
 
 
         Args:
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/content_service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/content_service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 # (C) 2023 GoodData Corporation
 from __future__ import annotations
 
-from typing import Any
+from typing import Type, Union
 
 import attr
 
 from gooddata_api_client.model.json_api_organization_setting_in_attributes import JsonApiOrganizationSettingInAttributes
 from gooddata_api_client.model.json_api_workspace_setting_in import JsonApiWorkspaceSettingIn
 from gooddata_api_client.model.json_api_workspace_setting_in_document import JsonApiWorkspaceSettingInDocument
 from gooddata_api_client.model.json_api_workspace_setting_out import JsonApiWorkspaceSettingOut
+from gooddata_api_client.model.json_api_workspace_setting_post_optional_id import JsonApiWorkspaceSettingPostOptionalId
+from gooddata_api_client.model.json_api_workspace_setting_post_optional_id_document import (
+    JsonApiWorkspaceSettingPostOptionalIdDocument,
+)
 from gooddata_sdk.catalog.entity import AttrCatalogEntity
 from gooddata_sdk.utils import safeget
 
 
 @attr.s(auto_attribs=True, kw_only=True)
 class CatalogWorkspaceSetting(AttrCatalogEntity):
+    id: str = attr.field(default=None)
+
     @staticmethod
-    def client_class() -> Any:
+    def client_class() -> Type[JsonApiWorkspaceSettingOut]:
         return JsonApiWorkspaceSettingOut
 
     content: dict = attr.field(
         repr=False,
         default=attr.Factory(lambda self: safeget(self.json_api_entity.attributes, ["content"]), takes_self=True),
     )
 
-    def to_api(self) -> JsonApiWorkspaceSettingInDocument:
-        return JsonApiWorkspaceSettingInDocument(
-            data=JsonApiWorkspaceSettingIn(
-                id=self.id,
-                attributes=JsonApiOrganizationSettingInAttributes(
-                    content=self.content,
-                ),
-            )
+    def _attributes(self) -> JsonApiOrganizationSettingInAttributes:
+        return JsonApiOrganizationSettingInAttributes(
+            content=self.content,
         )
+
+    def to_api(
+        self, post: bool = False
+    ) -> Union[JsonApiWorkspaceSettingInDocument, JsonApiWorkspaceSettingPostOptionalIdDocument]:
+        if not post and self.id is None:
+            raise ValueError(
+                f"The combination for {post=} and {self.id=} is not valid. Id can be None only for post=True."
+            )
+        if post:
+            return JsonApiWorkspaceSettingPostOptionalIdDocument(
+                data=JsonApiWorkspaceSettingPostOptionalId(id=self.id, attributes=self._attributes())
+            )
+        else:
+            return JsonApiWorkspaceSettingInDocument(
+                data=JsonApiWorkspaceSettingIn(id=self.id, attributes=self._attributes())
+            )
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/workspace.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/entity_model/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/model_container.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/model_container.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/catalog/workspace/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,23 +142,26 @@
                 ID of workspace where we create the setting
             workspace_setting (CatalogWorkspaceSetting):
                 Catalog Workspace Setting object to be created or updated.
 
         Returns:
             None
         """
-        try:
-            self.get_workspace_setting(workspace_id, workspace_setting.id)
-            self._entities_api.update_entity_workspace_settings(
-                workspace_id,
-                workspace_setting.id,
-                workspace_setting.to_api(),
-            )
-        except NotFoundException:
-            self._entities_api.create_entity_workspace_settings(workspace_id, workspace_setting.to_api())
+        if workspace_setting.id is None:
+            self._entities_api.create_entity_workspace_settings(workspace_id, workspace_setting.to_api(True))
+        else:
+            try:
+                self.get_workspace_setting(workspace_id, workspace_setting.id)
+                self._entities_api.update_entity_workspace_settings(
+                    workspace_id,
+                    workspace_setting.id,
+                    workspace_setting.to_api(),
+                )
+            except NotFoundException:
+                self._entities_api.create_entity_workspace_settings(workspace_id, workspace_setting.to_api(True))
 
     def delete_workspace_setting(self, workspace_id: str, workspace_setting_id: str) -> None:
         try:
             self._entities_api.delete_entity_workspace_settings(workspace_id, workspace_setting_id)
         except NotFoundException:
             pass
 
@@ -810,25 +813,32 @@
             user_data_filter (CatalogUserDataFilter):
                 UserDataFilter entity object.
 
         Returns:
             None
         """
         user_data_filter_document = CatalogUserDataFilterDocument(data=user_data_filter)
-        try:
-            self.get_user_data_filter(workspace_id=workspace_id, user_data_filter_id=user_data_filter.id)
-            self._entities_api.update_entity_user_data_filters(
-                workspace_id=workspace_id,
-                object_id=user_data_filter.id,
-                json_api_user_data_filter_in_document=user_data_filter_document.to_api(),
-            )
-        except NotFoundException:
+        if user_data_filter.id is None:
             self._entities_api.create_entity_user_data_filters(
-                workspace_id=workspace_id, json_api_user_data_filter_in_document=user_data_filter_document.to_api()
+                workspace_id=workspace_id,
+                json_api_user_data_filter_post_optional_id_document=user_data_filter_document.to_api(True),
             )
+        else:
+            try:
+                self.get_user_data_filter(workspace_id=workspace_id, user_data_filter_id=user_data_filter.id)
+                self._entities_api.update_entity_user_data_filters(
+                    workspace_id=workspace_id,
+                    object_id=user_data_filter.id,
+                    json_api_user_data_filter_in_document=user_data_filter_document.to_api(),
+                )
+            except NotFoundException:
+                self._entities_api.create_entity_user_data_filters(
+                    workspace_id=workspace_id,
+                    json_api_user_data_filter_post_optional_id_document=user_data_filter_document.to_api(True),
+                )
 
     def get_user_data_filter(self, workspace_id: str, user_data_filter_id: str) -> CatalogUserDataFilter:
         """Get user data filter by its id.
 
         Args:
             workspace_id (str):
                 String containing id of the workspace.
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/client.py` & `gooddata-sdk-1.4.0/gooddata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/attribute.py` & `gooddata-sdk-1.4.0/gooddata_sdk/compute/model/attribute.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/base.py` & `gooddata-sdk-1.4.0/gooddata_sdk/compute/model/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/execution.py` & `gooddata-sdk-1.4.0/gooddata_sdk/compute/model/execution.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/filter.py` & `gooddata-sdk-1.4.0/gooddata_sdk/compute/model/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/metric.py` & `gooddata-sdk-1.4.0/gooddata_sdk/compute/model/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/service.py` & `gooddata-sdk-1.4.0/gooddata_sdk/compute/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/insight.py` & `gooddata-sdk-1.4.0/gooddata_sdk/insight.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/sdk.py` & `gooddata-sdk-1.4.0/gooddata_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/support.py` & `gooddata-sdk-1.4.0/gooddata_sdk/support.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/table.py` & `gooddata-sdk-1.4.0/gooddata_sdk/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/type_converter.py` & `gooddata-sdk-1.4.0/gooddata_sdk/type_converter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk/utils.py` & `gooddata-sdk-1.4.0/gooddata_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/PKG-INFO` & `gooddata-sdk-1.4.0/gooddata_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.3.1.dev5
+Version: 1.4.0
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev5
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.4.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoodData Python SDK
 
 The `gooddata-sdk` package provides a clean and convenient Python API to interact with [GoodData](https://www.gooddata.com/).
 
@@ -34,15 +34,15 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.3) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.4.0) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
 -  Python 3.7 or newer
 
 ## Installation
```

### Comparing `gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/SOURCES.txt` & `gooddata-sdk-1.4.0/gooddata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev5/setup.py` & `gooddata-sdk-1.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,50 +3,48 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-api-client~=1.3.1.dev5",
-    'importlib-metadata >= 1.0 ; python_version >= "3.7"',
+    "gooddata-api-client~=1.4.0",
     "python-dateutil>=2.5.3",
     "pyyaml>=5.1",
     "attrs==21.4.0",
     "cattrs==22.1.0",
     "brotli==1.0.9",
 ]
 
-
 setup(
     name="gooddata-sdk",
     description="GoodData.CN Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.3.1.dev5",
+    version="1.4.0",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     project_urls={
-        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.3.1.dev5",
+        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.4.0",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Database",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
     keywords=[
         "gooddata",
```

### Comparing `gooddata-sdk-1.3.1.dev5/tests/test_type_converter.py` & `gooddata-sdk-1.4.0/tests/test_type_converter.py`

 * *Files identical despite different names*

