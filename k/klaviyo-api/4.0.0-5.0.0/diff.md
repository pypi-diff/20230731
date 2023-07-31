# Comparing `tmp/klaviyo-api-4.0.0.tar.gz` & `tmp/klaviyo-api-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jenkins/build/workspace/dev-team/DevX/generateSDKs/pip/dist/tmppzbz8yyq/klaviyo-api-4.0.0.tar", last modified: Mon Jul 17 17:51:14 2023, max compression
+gzip compressed data, was "klaviyo-api-5.0.0.tar", last modified: Mon Jul 31 06:56:06 2023, max compression
```

## Comparing `klaviyo-api-4.0.0.tar` & `klaviyo-api-5.0.0.tar`

### file list

```diff
@@ -1,308 +1,290 @@
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)      801 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/setup.cfg
--rw-r--r--   0 jenkins    (500) jenkins    (500)      103 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/pyproject.toml
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    57655 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/README.md
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    58208 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/PKG-INFO
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api.egg-info/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    20113 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (500) jenkins    (500)      119 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (500) jenkins    (500)        1 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    58208 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (500) jenkins    (500)       27 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/openapi_client/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    17158 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/configuration.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    14324 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/rest.py
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/openapi_client/api/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    73091 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/lists_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)     7228 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/data_privacy_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)   149966 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/tags_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)   153787 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/campaigns_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    21844 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/metrics_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    85077 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/profiles_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    42433 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/templates_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    15356 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/accounts_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    50615 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/segments_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)   109573 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/flows_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)   356584 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/catalogs_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    55796 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/api/events_api.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)      219 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/api/__init__.py
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/openapi_client/apis/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)     1086 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/apis/__init__.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)     5120 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/exceptions.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    39434 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/api_client.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    82630 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/model_utils.py
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/openapi_client/models/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    30958 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/models/__init__.py
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/openapi_client/model/
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11991 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_create_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12786 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11999 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12023 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_create_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11831 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_members_add_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11930 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_partial_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11851 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_category_op.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12080 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11985 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/event_create_query_v2_resource_object_attributes_profile.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11890 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_partial_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11304 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_location_longitude.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13115 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/send_strategy_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13136 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11775 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12366 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11819 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/flow_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12603 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12296 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11762 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12012 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    21095 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12213 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_relationships_item.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12586 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/segment_partial_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13219 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/email_tracking_options_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12671 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12068 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_delete_job_create_query_resource_object_attributes_profiles.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12225 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12264 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query_resource_object_relationships_variant.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11965 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11921 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12026 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_suppression_bulk_delete_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_render_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13066 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13362 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12172 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11803 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_meta.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12093 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_create_query_resource_object_relationships_tag_group.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_delete_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11750 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11991 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11819 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12364 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_render_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11663 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11890 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11768 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12023 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes_profile.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12744 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12200 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_channels.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12683 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_identifier_dto_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12068 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes_profiles.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12654 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12485 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11849 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12334 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/event_create_query_v2_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11668 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12022 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12364 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_profile_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13362 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12010 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes_items.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11840 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_members_delete_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11991 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    17148 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12568 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    14140 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes_send_options.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11860 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12845 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12651 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_delete_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11645 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12654 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12671 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    16063 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11869 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_aggregate_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11764 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/flow_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12049 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes_variants.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_delete_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13857 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12026 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11760 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_segment_op.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11618 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12845 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/render_options_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11926 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_flow_op_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11821 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/onsite_profile_meta.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12608 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12410 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11301 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_location_latitude.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11730 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_flow_op.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12839 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_meta_patch_properties.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12022 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_delete_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11558 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12458 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_suppression_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11879 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_deletion_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11685 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_suppression_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12625 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11633 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12002 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12667 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12583 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_render_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13274 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11703 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    15169 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_create_query_resource_object_attributes_content.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12256 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11959 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_segment_op_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12702 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/static_schedule_options.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12671 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12065 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes_categories.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12818 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_subscription_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11999 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_subscription_delete_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12011 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_assign_template_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11999 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11809 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13736 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12187 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12170 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query_resource_object_relationships_variant_data.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11750 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_aggregate_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12848 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11966 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12065 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes_categories.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11689 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_suppression_delete_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11588 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/event_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12225 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12837 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    14788 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12347 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12364 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11325 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_meta_patch_properties_unset.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11998 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query_resource_object_attributes_profile.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12151 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12137 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12134 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13298 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11627 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/email_send_options_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12432 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/email_content_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11930 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12219 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11921 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12362 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/sms_tracking_options_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13112 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12302 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12012 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12049 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes_variants.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    15708 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes_tracking_options.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12256 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12049 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes_variants.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12256 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11521 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/sms_content_sub_object_create.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12058 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_category_op_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12458 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_suppression_delete_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12487 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12235 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11850 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    15281 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11750 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12816 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12330 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12073 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query_resource_object_relationships_list_data.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11547 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/sto_schedule_options.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12714 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_profile_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12354 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_clone_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11858 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13961 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_location.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12834 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_identifier_dto_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11966 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    15156 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12160 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12570 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11860 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12071 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_create_query_resource_object_relationships_tag_group_data.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/segment_partial_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11921 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11850 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/event_create_query_v2.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12041 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13039 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_partial_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11930 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12468 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_subscription_delete_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11573 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12228 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11632 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12959 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/server_bis_subscription_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12022 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12806 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_subscription_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12065 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes_categories.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12012 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_update_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12354 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_clone_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12041 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_subscription_bulk_delete_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12294 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_relationships_template.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12603 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12010 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes_items.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11890 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11916 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_clone_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12538 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/flow_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12078 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query_resource_object_attributes_profiles.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11970 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_campaign_op_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11633 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12302 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11966 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12603 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11932 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/event_create_query_v2_resource_object_attributes_metric.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    16135 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/event_create_query_v2_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13040 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    19026 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12035 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes_campaign_messages.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11894 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/back_in_stock_subscription_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11954 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12010 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes_items.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12422 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_delete_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12102 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11980 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_members_add_query_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12225 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_delete_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12172 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11845 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/utm_params_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11735 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12625 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/list_partial_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12122 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13074 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/onsite_profile_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13632 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    15428 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_partial_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12424 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_aggregate_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12374 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_delete_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12172 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11926 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_list_op_data_inner.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12002 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_partial_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_create_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11690 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12234 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_delete_job_create_query_resource_object_relationships_list.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11834 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/audiences_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11730 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_list_op.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12001 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_partial_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11809 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12651 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12123 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_relationships_template_data.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12302 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12078 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes_profiles.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12572 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11618 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/segment_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/profile_partial_update_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11849 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/template_clone_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12184 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/throttled_schedule_options.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11881 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11770 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_campaign_op.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12654 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11603 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/metric_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11675 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12469 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_update_query_resource_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12082 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11849 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_clone_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13240 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_message_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11625 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/tag_update_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    13243 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11931 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/campaign_send_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_update_job_create_query.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    17029 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)      348 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/model/__init__.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11621 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/sms_send_options_sub_object.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    12114 2023-07-17 17:51:06.000000 klaviyo-api-4.0.0/src/openapi_client/model/catalog_category_item_op.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    11573 2023-07-17 17:51:07.000000 klaviyo-api-4.0.0/src/openapi_client/model/flow_enum.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)      788 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/openapi_client/__init__.py
-drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-07-17 17:51:14.000000 klaviyo-api-4.0.0/src/klaviyo_api/
--rw-r--r--   0 jenkins    (500) jenkins    (500)      501 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/klaviyo_api/custom_retry.py
--rw-rw-r--   0 jenkins    (500) jenkins    (500)    26919 2023-07-17 17:51:08.000000 klaviyo-api-4.0.0/src/klaviyo_api/wrapper.py
--rw-r--r--   0 jenkins    (500) jenkins    (500)      130 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/src/klaviyo_api/__init__.py
--rw-r--r--   0 jenkins    (500) jenkins    (500)     1063 2023-07-17 17:51:09.000000 klaviyo-api-4.0.0/LICENSE
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:06.028173 klaviyo-api-5.0.0/
+-rw-r--r--   0 local      (503) staff       (20)     1063 2023-07-31 06:55:56.000000 klaviyo-api-5.0.0/LICENSE
+-rw-r--r--   0 local      (503) staff       (20)    58762 2023-07-31 06:56:06.028626 klaviyo-api-5.0.0/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    58245 2023-07-31 06:55:56.000000 klaviyo-api-5.0.0/README.md
+-rw-r--r--   0 local      (503) staff       (20)      103 2023-07-31 06:55:56.000000 klaviyo-api-5.0.0/pyproject.toml
+-rw-r--r--   0 local      (503) staff       (20)      789 2023-07-31 06:56:06.030836 klaviyo-api-5.0.0/setup.cfg
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:05.654603 klaviyo-api-5.0.0/src/
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:05.659500 klaviyo-api-5.0.0/src/klaviyo_api/
+-rw-r--r--   0 local      (503) staff       (20)      130 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/klaviyo_api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)      501 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/klaviyo_api/custom_retry.py
+-rw-r--r--   0 local      (503) staff       (20)    26919 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/klaviyo_api/wrapper.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:05.662721 klaviyo-api-5.0.0/src/klaviyo_api.egg-info/
+-rw-r--r--   0 local      (503) staff       (20)    58762 2023-07-31 06:56:05.000000 klaviyo-api-5.0.0/src/klaviyo_api.egg-info/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    19358 2023-07-31 06:56:05.000000 klaviyo-api-5.0.0/src/klaviyo_api.egg-info/SOURCES.txt
+-rw-r--r--   0 local      (503) staff       (20)        1 2023-07-31 06:56:05.000000 klaviyo-api-5.0.0/src/klaviyo_api.egg-info/dependency_links.txt
+-rw-r--r--   0 local      (503) staff       (20)      108 2023-07-31 06:56:05.000000 klaviyo-api-5.0.0/src/klaviyo_api.egg-info/requires.txt
+-rw-r--r--   0 local      (503) staff       (20)       27 2023-07-31 06:56:05.000000 klaviyo-api-5.0.0/src/klaviyo_api.egg-info/top_level.txt
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:05.666036 klaviyo-api-5.0.0/src/openapi_client/
+-rw-r--r--   0 local      (503) staff       (20)    30943 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/__init__.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:05.675123 klaviyo-api-5.0.0/src/openapi_client/api/
+-rw-r--r--   0 local      (503) staff       (20)      705 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    16394 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/accounts_api.py
+-rw-r--r--   0 local      (503) staff       (20)   191270 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/campaigns_api.py
+-rw-r--r--   0 local      (503) staff       (20)   477516 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/catalogs_api.py
+-rw-r--r--   0 local      (503) staff       (20)     9254 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/data_privacy_api.py
+-rw-r--r--   0 local      (503) staff       (20)    62961 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/events_api.py
+-rw-r--r--   0 local      (503) staff       (20)   145037 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/flows_api.py
+-rw-r--r--   0 local      (503) staff       (20)    94658 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/lists_api.py
+-rw-r--r--   0 local      (503) staff       (20)    31568 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/metrics_api.py
+-rw-r--r--   0 local      (503) staff       (20)   106307 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/profiles_api.py
+-rw-r--r--   0 local      (503) staff       (20)    65868 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/segments_api.py
+-rw-r--r--   0 local      (503) staff       (20)   192610 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/tags_api.py
+-rw-r--r--   0 local      (503) staff       (20)    55679 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/api/templates_api.py
+-rw-r--r--   0 local      (503) staff       (20)    30340 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/api_client.py
+-rw-r--r--   0 local      (503) staff       (20)      844 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/api_response.py
+-rw-r--r--   0 local      (503) staff       (20)    15354 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/configuration.py
+-rw-r--r--   0 local      (503) staff       (20)     5182 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/exceptions.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-07-31 06:56:06.027581 klaviyo-api-5.0.0/src/openapi_client/models/
+-rw-r--r--   0 local      (503) staff       (20)    29742 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/models/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)     2219 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/audiences_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)      879 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/back_in_stock_subscription_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2283 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_clone_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2632 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_clone_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2749 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_clone_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2295 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2644 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     4399 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2830 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_create_query_resource_object_attributes_campaign_messages.py
+-rw-r--r--   0 local      (503) staff       (20)      750 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2477 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_assign_template_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3522 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_assign_template_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2513 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_assign_template_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2839 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_assign_template_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2860 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_assign_template_query_resource_object_relationships_template.py
+-rw-r--r--   0 local      (503) staff       (20)     2503 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_assign_template_query_resource_object_relationships_template_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2751 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3554 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      807 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2465 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2963 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3219 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_message_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2380 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2857 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3766 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2562 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_recipient_estimation_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2980 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_recipient_estimation_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2591 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      928 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_recipient_estimation_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2381 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2753 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2447 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      815 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2466 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2995 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2590 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/campaign_send_job_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      922 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      922 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      922 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2490 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2903 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2818 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2895 2023-07-31 06:55:52.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_job_create_query_resource_object_attributes_categories.py
+-rw-r--r--   0 local      (503) staff       (20)     2380 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3392 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     4195 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2703 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2921 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_create_query_resource_object_relationships_items.py
+-rw-r--r--   0 local      (503) staff       (20)     2490 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2903 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2818 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2895 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_delete_job_create_query_resource_object_attributes_categories.py
+-rw-r--r--   0 local      (503) staff       (20)     2492 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)      807 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2625 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_item_op.py
+-rw-r--r--   0 local      (503) staff       (20)     2490 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2903 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2818 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2895 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_job_create_query_resource_object_attributes_categories.py
+-rw-r--r--   0 local      (503) staff       (20)     2380 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3704 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2467 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_category_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      894 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      894 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      894 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2658 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_category_op.py
+-rw-r--r--   0 local      (503) staff       (20)     2442 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2843 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2705 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2811 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_job_create_query_resource_object_attributes_items.py
+-rw-r--r--   0 local      (503) staff       (20)     2332 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3316 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     7046 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2720 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2962 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_query_resource_object_relationships_categories.py
+-rw-r--r--   0 local      (503) staff       (20)     2485 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2442 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2843 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2705 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2811 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_delete_job_create_query_resource_object_attributes_items.py
+-rw-r--r--   0 local      (503) staff       (20)     2444 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)      779 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2442 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2843 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2705 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2811 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_job_create_query_resource_object_attributes_items.py
+-rw-r--r--   0 local      (503) staff       (20)     2332 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3624 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     5278 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_item_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      915 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      915 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      915 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2478 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2888 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2780 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2868 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_job_create_query_resource_object_attributes_variants.py
+-rw-r--r--   0 local      (503) staff       (20)     2368 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3373 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     8501 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2678 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2703 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_query_resource_object_relationships_item.py
+-rw-r--r--   0 local      (503) staff       (20)     2409 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_create_query_resource_object_relationships_item_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2478 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2888 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2780 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2868 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_delete_job_create_query_resource_object_attributes_variants.py
+-rw-r--r--   0 local      (503) staff       (20)     2480 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)      800 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2478 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2888 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2780 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2868 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_job_create_query_resource_object_attributes_variants.py
+-rw-r--r--   0 local      (503) staff       (20)     2368 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3047 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     6759 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/catalog_variant_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2466 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_create_deletion_job_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2860 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_create_deletion_job_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2755 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_create_deletion_job_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2672 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_create_deletion_job_query_resource_object_attributes_profile.py
+-rw-r--r--   0 local      (503) staff       (20)      872 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_deletion_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2897 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_profile_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2849 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/data_privacy_profile_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2284 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/event_create_query_v2.py
+-rw-r--r--   0 local      (503) staff       (20)     2624 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/event_create_query_v2_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     5268 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/event_create_query_v2_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2519 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/event_create_query_v2_resource_object_attributes_metric.py
+-rw-r--r--   0 local      (503) staff       (20)     2556 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/event_create_query_v2_resource_object_attributes_profile.py
+-rw-r--r--   0 local      (503) staff       (20)      729 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/event_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      722 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/flow_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2247 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/flow_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2717 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/flow_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2430 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/flow_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2540 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/get_accounts4_xx_response.py
+-rw-r--r--   0 local      (503) staff       (20)     2809 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/get_accounts4_xx_response_errors_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2235 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/get_accounts4_xx_response_errors_inner_source.py
+-rw-r--r--   0 local      (503) staff       (20)     2247 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2584 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2377 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      722 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2478 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_members_add_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2140 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_members_add_query_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2502 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_members_delete_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2332 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2806 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/list_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)      807 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_aggregate_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2307 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_aggregate_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2678 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_aggregate_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    10037 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_aggregate_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2614 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2832 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      736 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/metric_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     3294 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/onsite_profile_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     6244 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/onsite_profile_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2382 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/onsite_profile_meta.py
+-rw-r--r--   0 local      (503) staff       (20)     2283 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2629 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     5855 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      743 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2860 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_identifier_dto_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3702 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_identifier_dto_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     3294 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_location.py
+-rw-r--r--   0 local      (503) staff       (20)     2334 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_meta.py
+-rw-r--r--   0 local      (503) staff       (20)     2476 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_meta_patch_properties.py
+-rw-r--r--   0 local      (503) staff       (20)     2368 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3266 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)      950 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_subscription_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      950 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_subscription_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2998 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_subscription_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3544 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_subscription_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2774 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_subscription_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2903 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_subscription_delete_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      943 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_suppression_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)      943 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_suppression_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2762 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_suppression_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2503 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_suppression_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2762 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_suppression_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2505 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/profile_suppression_delete_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2563 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/render_options_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)      743 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/segment_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2368 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/segment_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2795 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/segment_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2409 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/segment_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     3591 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/send_strategy_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2453 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3516 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3425 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2651 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query_resource_object_attributes_profile.py
+-rw-r--r--   0 local      (503) staff       (20)     2802 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2824 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query_resource_object_relationships_variant.py
+-rw-r--r--   0 local      (503) staff       (20)     2498 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/server_bis_subscription_create_query_resource_object_relationships_variant_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2679 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/static_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)     1994 2023-07-31 06:55:53.000000 klaviyo-api-5.0.0/src/openapi_client/models/sto_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)     2970 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_channels.py
+-rw-r--r--   0 local      (503) staff       (20)     2453 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3544 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3230 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2865 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query_resource_object_attributes_profiles.py
+-rw-r--r--   0 local      (503) staff       (20)     2763 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2788 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query_resource_object_relationships_list.py
+-rw-r--r--   0 local      (503) staff       (20)     2443 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_create_job_create_query_resource_object_relationships_list_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2453 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3544 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2755 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2867 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/subscription_delete_job_create_query_resource_object_attributes_profiles.py
+-rw-r--r--   0 local      (503) staff       (20)     2441 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2863 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2743 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2869 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_create_job_create_query_resource_object_attributes_profiles.py
+-rw-r--r--   0 local      (503) staff       (20)     2441 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2863 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2743 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2869 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/suppression_delete_job_create_query_resource_object_attributes_profiles.py
+-rw-r--r--   0 local      (503) staff       (20)     2405 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_campaign_op.py
+-rw-r--r--   0 local      (503) staff       (20)     2095 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_campaign_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2235 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     3161 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2349 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2640 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)     2619 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_create_query_resource_object_relationships_tag_group.py
+-rw-r--r--   0 local      (503) staff       (20)     2344 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_create_query_resource_object_relationships_tag_group_data.py
+-rw-r--r--   0 local      (503) staff       (20)      715 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2357 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_flow_op.py
+-rw-r--r--   0 local      (503) staff       (20)     2051 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_flow_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2296 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2646 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2510 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      758 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2296 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2759 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2537 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_group_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2357 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_list_op.py
+-rw-r--r--   0 local      (503) staff       (20)     2051 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_list_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2393 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_segment_op.py
+-rw-r--r--   0 local      (503) staff       (20)     2084 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_segment_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2235 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2676 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/tag_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2283 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_clone_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2632 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_clone_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2708 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_clone_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2295 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2644 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3444 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)      750 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_enum.py
+-rw-r--r--   0 local      (503) staff       (20)     2295 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_render_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2644 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_render_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     2707 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_render_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2295 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)     2759 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)     3055 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/template_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)     2312 2023-07-31 06:55:54.000000 klaviyo-api-5.0.0/src/openapi_client/models/throttled_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    12828 2023-07-31 06:55:55.000000 klaviyo-api-5.0.0/src/openapi_client/rest.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `klaviyo-api-4.0.0/setup.cfg` & `klaviyo-api-5.0.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = klaviyo-api
-version = 4.0.0
+version = 5.0.0
 author = Klaviyo Developers
 author_email = developers@klaviyo.com
 description = Klaviyo Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klaviyo/klaviyo-api-python
 project_urls = 
@@ -16,21 +16,20 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	certifi >= 14.05.14
-	six >= 1.10
 	python_dateutil >= 2.5.3
 	setuptools >= 21.0.0
-	urllib3 >= 1.15.1
+	urllib3 >= 1.25.3
+	pydantic >= 1.10.5, < 2
+	aenum >= 3.1.11
 	tenacity >= 8.0.0
-	requests >= 2.26.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `klaviyo-api-4.0.0/README.md` & `klaviyo-api-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+Metadata-Version: 2.1
+Name: klaviyo-api
+Version: 5.0.0
+Summary: Klaviyo Python SDK
+Home-page: https://github.com/klaviyo/klaviyo-api-python
+Author: Klaviyo Developers
+Author-email: developers@klaviyo.com
+Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Klaviyo Python SDK
 
-- SDK version: 4.0.0
+- SDK version: 5.0.0
 - API revision: 2023-07-15
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-07-15/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-07-15/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
@@ -94,15 +109,15 @@
 * The SDK retries on resolvable errors, namely: rate limits (common) and server errors (rare).
 * The keyword arguments define some advanced settings; the example is populated with the default values.
 * `max_delay` denotes total delay (in seconds) across all attempts.
 
 ```python
 from klaviyo_api import KlaviyoAPI
 
-klaviyo = KlaviyoAPI("YOUR API KEY HERE", max_delay=60, max_retries=3, test_host=None)
+klaviyo = KlaviyoAPI("YOUR_API_KEY_HERE", max_delay=60, max_retries=3, test_host=None)
 ```
 
 ### Example request
 
 ```python
 klaviyo.Metrics.get_metrics() 
 ```
@@ -202,15 +217,15 @@
 ## Important Notes
 
 - The main difference between this SDK and the language-agnostic API Docs that the below endpoints link to is that this SDK automatically adds the `revision` header corresponding to the SDK version.
 - Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-07-15/reference/get_events).
 - For example values / data types, as well as whether parameters are required/optional, please reference the corresponding API Reference link.
 - Some keyword args may potentially be required for the API call to succeed, the linked API docs are the source of truth regarding which keyword params are required.
 - JSON payloads should be passed in as native python dictionaries.
-- You can override the client private key by passing in an optional `api_key` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
+- You can override the client private key by passing in an optional `_request_auth` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
 
 # Comprehensive list of Operations & Parameters
 
 
 
 
 
@@ -221,29 +236,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_account | [str]
+# fields_account | List[str]
 
 klaviyo.Accounts.get_account(id, fields_account=fields_account)
 ```
 
 
 
 
 #### [Get Accounts](https://developers.klaviyo.com/en/v2023-07-15/reference/get_accounts)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_account | [str]
+# fields_account | List[str]
 
 klaviyo.Accounts.get_accounts(fields_account=fields_account)
 ```
 
 
 
 
@@ -334,18 +349,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -354,18 +369,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_template | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_template | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign_campaign_messages(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_template=fields_template, include=include)
 ```
 
 
 
 
@@ -374,18 +389,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_template | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_template | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign_message(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_template=fields_template, include=include)
 ```
 
 
 
 
@@ -394,15 +409,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
+# fields_campaign_message | List[str]
 
 klaviyo.Campaigns.get_campaign_message_campaign(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
@@ -437,15 +452,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
+# fields_campaign_message | List[str]
 
 klaviyo.Campaigns.get_campaign_message_template(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
@@ -454,15 +469,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_recipient_estimation | [str]
+# fields_campaign_recipient_estimation | List[str]
 
 klaviyo.Campaigns.get_campaign_recipient_estimation(id, fields_campaign_recipient_estimation=fields_campaign_recipient_estimation)
 ```
 
 
 
 
@@ -471,15 +486,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_recipient_estimation_job | [str]
+# fields_campaign_recipient_estimation_job | List[str]
 
 klaviyo.Campaigns.get_campaign_recipient_estimation_job(id, fields_campaign_recipient_estimation_job=fields_campaign_recipient_estimation_job)
 ```
 
 
 
 
@@ -514,15 +529,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_send_job | [str]
+# fields_campaign_send_job | List[str]
 
 klaviyo.Campaigns.get_campaign_send_job(id, fields_campaign_send_job=fields_campaign_send_job)
 ```
 
 
 
 
@@ -531,15 +546,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Campaigns.get_campaign_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
@@ -548,18 +563,18 @@
 ```python
 ## Positional Arguments
 
 # filter | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_tag | List[str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Campaigns.get_campaigns(filter, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -760,15 +775,15 @@
 
 #### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_categories)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_categories(fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -780,15 +795,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 
 klaviyo.Catalogs.get_catalog_category(id, fields_catalog_category=fields_catalog_category)
 ```
 
 
 
 
@@ -797,18 +812,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_category_items(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -836,17 +851,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_catalog_item(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
@@ -855,15 +870,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_item_categories(id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -892,15 +907,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_item_variants(id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -909,18 +924,18 @@
 
 #### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_items)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_items(fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -931,29 +946,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 
 klaviyo.Catalogs.get_catalog_variant(id, fields_catalog_variant=fields_catalog_variant)
 ```
 
 
 
 
 #### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_variants)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_variants(fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -965,31 +980,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_create_job | [str]
-# fields_catalog_category | [str]
-# include | [str]
+# fields_catalog_category_bulk_create_job | List[str]
+# fields_catalog_category | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_categories_job(job_id, fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
 #### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_create_job | [str]
+# fields_catalog_category_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_categories_jobs(fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1000,31 +1015,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_create_job | [str]
-# fields_catalog_item | [str]
-# include | [str]
+# fields_catalog_item_bulk_create_job | List[str]
+# fields_catalog_item | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_items_job(job_id, fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
 #### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_create_job | [str]
+# fields_catalog_item_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_items_jobs(fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1035,31 +1050,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_create_job | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_variant_bulk_create_job | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_variants_job(job_id, fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
 #### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_create_job | [str]
+# fields_catalog_variant_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_variants_jobs(fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1070,29 +1085,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_delete_job | [str]
+# fields_catalog_category_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_categories_job(job_id, fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_delete_job | [str]
+# fields_catalog_category_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_categories_jobs(fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1103,29 +1118,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_delete_job | [str]
+# fields_catalog_item_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_items_job(job_id, fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_delete_job | [str]
+# fields_catalog_item_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_items_jobs(fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1136,29 +1151,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_delete_job | [str]
+# fields_catalog_variant_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_variants_job(job_id, fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_delete_job | [str]
+# fields_catalog_variant_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_variants_jobs(fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1169,31 +1184,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_update_job | [str]
-# fields_catalog_category | [str]
-# include | [str]
+# fields_catalog_category_bulk_update_job | List[str]
+# fields_catalog_category | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_categories_job(job_id, fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
 #### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_update_job | [str]
+# fields_catalog_category_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_categories_jobs(fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1204,31 +1219,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_update_job | [str]
-# fields_catalog_item | [str]
-# include | [str]
+# fields_catalog_item_bulk_update_job | List[str]
+# fields_catalog_item | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_items_job(job_id, fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
 #### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_update_job | [str]
+# fields_catalog_item_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_items_jobs(fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1239,31 +1254,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_update_job | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_variant_bulk_update_job | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_variants_job(job_id, fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
 #### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_update_job | [str]
+# fields_catalog_variant_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_variants_jobs(fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1495,18 +1510,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_event | [str]
-# fields_metric | [str]
-# fields_profile | [str]
-# include | [str]
+# fields_event | List[str]
+# fields_metric | List[str]
+# fields_profile | List[str]
+# include | List[str]
 
 klaviyo.Events.get_event(id, fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, include=include)
 ```
 
 
 
 
@@ -1515,15 +1530,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 
 klaviyo.Events.get_event_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
@@ -1532,16 +1547,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 
 klaviyo.Events.get_event_profile(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile)
 ```
 
 
 
 
@@ -1573,19 +1588,19 @@
 
 #### [Get Events](https://developers.klaviyo.com/en/v2023-07-15/reference/get_events)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_event | [str]
-# fields_metric | [str]
-# fields_profile | [str]
+# fields_event | List[str]
+# fields_metric | List[str]
+# fields_profile | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Events.get_events(fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -1600,18 +1615,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow(id, fields_flow_action=fields_flow_action, fields_flow=fields_flow, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -1620,18 +1635,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow_message | [str]
-# fields_flow | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow_message | List[str]
+# fields_flow | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow_action(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
@@ -1640,15 +1655,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow | [str]
+# fields_flow | List[str]
 
 klaviyo.Flows.get_flow_action_flow(id, fields_flow=fields_flow)
 ```
 
 
 
 
@@ -1657,15 +1672,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_message | [str]
+# fields_flow_message | List[str]
 # filter | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flow_action_messages(id, fields_flow_message=fields_flow_message, filter=filter, page_size=page_size, sort=sort)
 ```
 
@@ -1710,15 +1725,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
+# fields_flow_action | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flow_flow_actions(id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
@@ -1731,17 +1746,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow_message | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow_message | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow_message(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, include=include)
 ```
 
 
 
 
@@ -1750,15 +1765,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
+# fields_flow_action | List[str]
 
 klaviyo.Flows.get_flow_message_action(id, fields_flow_action=fields_flow_action)
 ```
 
 
 
 
@@ -1812,33 +1827,33 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Flows.get_flow_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Flows](https://developers.klaviyo.com/en/v2023-07-15/reference/get_flows)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow | [str]
-# fields_tag | [str]
+# fields_flow_action | List[str]
+# fields_flow | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
@@ -1922,18 +1937,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_list | [str]
-# fields_list | [str]
-# fields_tag | [str]
-# include | [str]
+# additional_fields_list | List[str]
+# fields_list | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Lists.get_list(id, additional_fields_list=additional_fields_list, fields_list=fields_list, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -1942,16 +1957,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
 klaviyo.Lists.get_list_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
@@ -1993,32 +2008,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Lists.get_list_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Lists](https://developers.klaviyo.com/en/v2023-07-15/reference/get_lists)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_list | [str]
-# fields_tag | [str]
+# fields_list | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 
 klaviyo.Lists.get_lists(fields_list=fields_list, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor)
 ```
 
 
 
@@ -2046,29 +2061,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 
 klaviyo.Metrics.get_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
 #### [Get Metrics](https://developers.klaviyo.com/en/v2023-07-15/reference/get_metrics)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Metrics.get_metrics(fields_metric=fields_metric, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -2109,19 +2124,19 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_list | [str]
-# fields_profile | [str]
-# fields_segment | [str]
-# include | [str]
+# additional_fields_profile | List[str]
+# fields_list | List[str]
+# fields_profile | List[str]
+# fields_segment | List[str]
+# include | List[str]
 
 klaviyo.Profiles.get_profile(id, additional_fields_profile=additional_fields_profile, fields_list=fields_list, fields_profile=fields_profile, fields_segment=fields_segment, include=include)
 ```
 
 
 
 
@@ -2130,15 +2145,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_list | [str]
+# fields_list | List[str]
 
 klaviyo.Profiles.get_profile_lists(id, fields_list=fields_list)
 ```
 
 
 
 
@@ -2173,30 +2188,30 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_segment | [str]
+# fields_segment | List[str]
 
 klaviyo.Profiles.get_profile_segments(id, fields_segment=fields_segment)
 ```
 
 
 
 
 #### [Get Profiles](https://developers.klaviyo.com/en/v2023-07-15/reference/get_profiles)
 
 ```python
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
@@ -2279,18 +2294,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_segment | [str]
-# fields_segment | [str]
-# fields_tag | [str]
-# include | [str]
+# additional_fields_segment | List[str]
+# fields_segment | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Segments.get_segment(id, additional_fields_segment=additional_fields_segment, fields_segment=fields_segment, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -2299,16 +2314,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
 klaviyo.Segments.get_segment_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
@@ -2350,32 +2365,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Segments.get_segment_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Segments](https://developers.klaviyo.com/en/v2023-07-15/reference/get_segments)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_segment | [str]
-# fields_tag | [str]
+# fields_segment | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 
 klaviyo.Segments.get_segments(fields_segment=fields_segment, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor)
 ```
 
 
 
@@ -2567,17 +2582,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_tag_group | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Tags.get_tag(id, fields_tag_group=fields_tag_group, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -2586,15 +2601,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 
 klaviyo.Tags.get_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
@@ -2616,29 +2631,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Tags.get_tag_group_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-07-15/reference/get_tag_groups)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Tags.get_tag_groups(fields_tag_group=fields_tag_group, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -2715,32 +2730,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 
 klaviyo.Tags.get_tag_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
 #### [Get Tags](https://developers.klaviyo.com/en/v2023-07-15/reference/get_tags)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
-# fields_tag | [str]
+# fields_tag_group | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Tags.get_tags(fields_tag_group=fields_tag_group, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -2835,29 +2850,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_template | [str]
+# fields_template | List[str]
 
 klaviyo.Templates.get_template(id, fields_template=fields_template)
 ```
 
 
 
 
 #### [Get Templates](https://developers.klaviyo.com/en/v2023-07-15/reference/get_templates)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_template | [str]
+# fields_template | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Templates.get_templates(fields_template=fields_template, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -2881,15 +2896,15 @@
 # Appendix
 
 ## Global Keyword Args
 
 NOTE: These are arguments that you can apply to any endpoint call, and which are unique to the SDK
 
 We currently support the following global keyword args:
-- `api_key` : use this to override the client-level api_key which you define upon client instantiation
+- `_request_auth` : use this to override the client-level api_key which you define upon client instantiation
 
 ## Refresher on catching exceptions:
 
 ```python
 try:
     YOUR_CALL
 except Exception as e:
@@ -2905,15 +2920,15 @@
 
 We stick to the following convention for parameters/arguments
 
 1. All parameters are passed as function args.
 2. All query and path params that are tagged as `required` in the docs are passed as positional args.
 3. All optional query params are passed as keyword args.
 4. Where applicable, the `body` param is passed in as a positional arg, and is expected to be a native python dictionary. Within that dictionary, refer to the API docs to see which fields are required/optional, along with valid values.
-4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `api_key` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
+4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `_request_auth` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
-- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
+- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
```

### Comparing `klaviyo-api-4.0.0/PKG-INFO` & `klaviyo-api-5.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-Metadata-Version: 2.1
-Name: klaviyo-api
-Version: 4.0.0
-Summary: Klaviyo Python SDK
-Home-page: https://github.com/klaviyo/klaviyo-api-python
-Author: Klaviyo Developers
-Author-email: developers@klaviyo.com
-License: UNKNOWN
-Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Klaviyo Python SDK
 
-- SDK version: 4.0.0
+- SDK version: 5.0.0
 - API revision: 2023-07-15
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-07-15/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-07-15/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
@@ -111,15 +94,15 @@
 * The SDK retries on resolvable errors, namely: rate limits (common) and server errors (rare).
 * The keyword arguments define some advanced settings; the example is populated with the default values.
 * `max_delay` denotes total delay (in seconds) across all attempts.
 
 ```python
 from klaviyo_api import KlaviyoAPI
 
-klaviyo = KlaviyoAPI("YOUR API KEY HERE", max_delay=60, max_retries=3, test_host=None)
+klaviyo = KlaviyoAPI("YOUR_API_KEY_HERE", max_delay=60, max_retries=3, test_host=None)
 ```
 
 ### Example request
 
 ```python
 klaviyo.Metrics.get_metrics() 
 ```
@@ -219,15 +202,15 @@
 ## Important Notes
 
 - The main difference between this SDK and the language-agnostic API Docs that the below endpoints link to is that this SDK automatically adds the `revision` header corresponding to the SDK version.
 - Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-07-15/reference/get_events).
 - For example values / data types, as well as whether parameters are required/optional, please reference the corresponding API Reference link.
 - Some keyword args may potentially be required for the API call to succeed, the linked API docs are the source of truth regarding which keyword params are required.
 - JSON payloads should be passed in as native python dictionaries.
-- You can override the client private key by passing in an optional `api_key` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
+- You can override the client private key by passing in an optional `_request_auth` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
 
 # Comprehensive list of Operations & Parameters
 
 
 
 
 
@@ -238,29 +221,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_account | [str]
+# fields_account | List[str]
 
 klaviyo.Accounts.get_account(id, fields_account=fields_account)
 ```
 
 
 
 
 #### [Get Accounts](https://developers.klaviyo.com/en/v2023-07-15/reference/get_accounts)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_account | [str]
+# fields_account | List[str]
 
 klaviyo.Accounts.get_accounts(fields_account=fields_account)
 ```
 
 
 
 
@@ -351,18 +334,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -371,18 +354,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_template | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_template | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign_campaign_messages(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_template=fields_template, include=include)
 ```
 
 
 
 
@@ -391,18 +374,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_template | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_template | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign_message(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_template=fields_template, include=include)
 ```
 
 
 
 
@@ -411,15 +394,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
+# fields_campaign_message | List[str]
 
 klaviyo.Campaigns.get_campaign_message_campaign(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
@@ -454,15 +437,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
+# fields_campaign_message | List[str]
 
 klaviyo.Campaigns.get_campaign_message_template(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
@@ -471,15 +454,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_recipient_estimation | [str]
+# fields_campaign_recipient_estimation | List[str]
 
 klaviyo.Campaigns.get_campaign_recipient_estimation(id, fields_campaign_recipient_estimation=fields_campaign_recipient_estimation)
 ```
 
 
 
 
@@ -488,15 +471,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_recipient_estimation_job | [str]
+# fields_campaign_recipient_estimation_job | List[str]
 
 klaviyo.Campaigns.get_campaign_recipient_estimation_job(id, fields_campaign_recipient_estimation_job=fields_campaign_recipient_estimation_job)
 ```
 
 
 
 
@@ -531,15 +514,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_send_job | [str]
+# fields_campaign_send_job | List[str]
 
 klaviyo.Campaigns.get_campaign_send_job(id, fields_campaign_send_job=fields_campaign_send_job)
 ```
 
 
 
 
@@ -548,15 +531,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Campaigns.get_campaign_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
@@ -565,18 +548,18 @@
 ```python
 ## Positional Arguments
 
 # filter | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_tag | List[str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Campaigns.get_campaigns(filter, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -777,15 +760,15 @@
 
 #### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_categories)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_categories(fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -797,15 +780,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 
 klaviyo.Catalogs.get_catalog_category(id, fields_catalog_category=fields_catalog_category)
 ```
 
 
 
 
@@ -814,18 +797,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_category_items(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -853,17 +836,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_catalog_item(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
@@ -872,15 +855,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_item_categories(id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -909,15 +892,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_item_variants(id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -926,18 +909,18 @@
 
 #### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_items)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_items(fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -948,29 +931,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 
 klaviyo.Catalogs.get_catalog_variant(id, fields_catalog_variant=fields_catalog_variant)
 ```
 
 
 
 
 #### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_variants)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_variants(fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -982,31 +965,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_create_job | [str]
-# fields_catalog_category | [str]
-# include | [str]
+# fields_catalog_category_bulk_create_job | List[str]
+# fields_catalog_category | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_categories_job(job_id, fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
 #### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_create_job | [str]
+# fields_catalog_category_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_categories_jobs(fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1017,31 +1000,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_create_job | [str]
-# fields_catalog_item | [str]
-# include | [str]
+# fields_catalog_item_bulk_create_job | List[str]
+# fields_catalog_item | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_items_job(job_id, fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
 #### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_create_job | [str]
+# fields_catalog_item_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_items_jobs(fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1052,31 +1035,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_create_job | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_variant_bulk_create_job | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_variants_job(job_id, fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
 #### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_create_job | [str]
+# fields_catalog_variant_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_variants_jobs(fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1087,29 +1070,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_delete_job | [str]
+# fields_catalog_category_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_categories_job(job_id, fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_delete_job | [str]
+# fields_catalog_category_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_categories_jobs(fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1120,29 +1103,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_delete_job | [str]
+# fields_catalog_item_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_items_job(job_id, fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_delete_job | [str]
+# fields_catalog_item_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_items_jobs(fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1153,29 +1136,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_delete_job | [str]
+# fields_catalog_variant_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_variants_job(job_id, fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_delete_job | [str]
+# fields_catalog_variant_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_variants_jobs(fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1186,31 +1169,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_update_job | [str]
-# fields_catalog_category | [str]
-# include | [str]
+# fields_catalog_category_bulk_update_job | List[str]
+# fields_catalog_category | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_categories_job(job_id, fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
 #### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_update_job | [str]
+# fields_catalog_category_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_categories_jobs(fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1221,31 +1204,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_update_job | [str]
-# fields_catalog_item | [str]
-# include | [str]
+# fields_catalog_item_bulk_update_job | List[str]
+# fields_catalog_item | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_items_job(job_id, fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
 #### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_update_job | [str]
+# fields_catalog_item_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_items_jobs(fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1256,31 +1239,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_update_job | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_variant_bulk_update_job | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_variants_job(job_id, fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
 #### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_update_job | [str]
+# fields_catalog_variant_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_variants_jobs(fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1512,18 +1495,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_event | [str]
-# fields_metric | [str]
-# fields_profile | [str]
-# include | [str]
+# fields_event | List[str]
+# fields_metric | List[str]
+# fields_profile | List[str]
+# include | List[str]
 
 klaviyo.Events.get_event(id, fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, include=include)
 ```
 
 
 
 
@@ -1532,15 +1515,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 
 klaviyo.Events.get_event_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
@@ -1549,16 +1532,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 
 klaviyo.Events.get_event_profile(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile)
 ```
 
 
 
 
@@ -1590,19 +1573,19 @@
 
 #### [Get Events](https://developers.klaviyo.com/en/v2023-07-15/reference/get_events)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_event | [str]
-# fields_metric | [str]
-# fields_profile | [str]
+# fields_event | List[str]
+# fields_metric | List[str]
+# fields_profile | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Events.get_events(fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -1617,18 +1600,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow(id, fields_flow_action=fields_flow_action, fields_flow=fields_flow, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -1637,18 +1620,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow_message | [str]
-# fields_flow | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow_message | List[str]
+# fields_flow | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow_action(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
@@ -1657,15 +1640,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow | [str]
+# fields_flow | List[str]
 
 klaviyo.Flows.get_flow_action_flow(id, fields_flow=fields_flow)
 ```
 
 
 
 
@@ -1674,15 +1657,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_message | [str]
+# fields_flow_message | List[str]
 # filter | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flow_action_messages(id, fields_flow_message=fields_flow_message, filter=filter, page_size=page_size, sort=sort)
 ```
 
@@ -1727,15 +1710,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
+# fields_flow_action | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flow_flow_actions(id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
@@ -1748,17 +1731,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow_message | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow_message | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow_message(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, include=include)
 ```
 
 
 
 
@@ -1767,15 +1750,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
+# fields_flow_action | List[str]
 
 klaviyo.Flows.get_flow_message_action(id, fields_flow_action=fields_flow_action)
 ```
 
 
 
 
@@ -1829,33 +1812,33 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Flows.get_flow_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Flows](https://developers.klaviyo.com/en/v2023-07-15/reference/get_flows)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow | [str]
-# fields_tag | [str]
+# fields_flow_action | List[str]
+# fields_flow | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
@@ -1939,18 +1922,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_list | [str]
-# fields_list | [str]
-# fields_tag | [str]
-# include | [str]
+# additional_fields_list | List[str]
+# fields_list | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Lists.get_list(id, additional_fields_list=additional_fields_list, fields_list=fields_list, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -1959,16 +1942,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
 klaviyo.Lists.get_list_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
@@ -2010,32 +1993,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Lists.get_list_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Lists](https://developers.klaviyo.com/en/v2023-07-15/reference/get_lists)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_list | [str]
-# fields_tag | [str]
+# fields_list | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 
 klaviyo.Lists.get_lists(fields_list=fields_list, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor)
 ```
 
 
 
@@ -2063,29 +2046,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 
 klaviyo.Metrics.get_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
 #### [Get Metrics](https://developers.klaviyo.com/en/v2023-07-15/reference/get_metrics)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Metrics.get_metrics(fields_metric=fields_metric, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -2126,19 +2109,19 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_list | [str]
-# fields_profile | [str]
-# fields_segment | [str]
-# include | [str]
+# additional_fields_profile | List[str]
+# fields_list | List[str]
+# fields_profile | List[str]
+# fields_segment | List[str]
+# include | List[str]
 
 klaviyo.Profiles.get_profile(id, additional_fields_profile=additional_fields_profile, fields_list=fields_list, fields_profile=fields_profile, fields_segment=fields_segment, include=include)
 ```
 
 
 
 
@@ -2147,15 +2130,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_list | [str]
+# fields_list | List[str]
 
 klaviyo.Profiles.get_profile_lists(id, fields_list=fields_list)
 ```
 
 
 
 
@@ -2190,30 +2173,30 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_segment | [str]
+# fields_segment | List[str]
 
 klaviyo.Profiles.get_profile_segments(id, fields_segment=fields_segment)
 ```
 
 
 
 
 #### [Get Profiles](https://developers.klaviyo.com/en/v2023-07-15/reference/get_profiles)
 
 ```python
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
@@ -2296,18 +2279,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_segment | [str]
-# fields_segment | [str]
-# fields_tag | [str]
-# include | [str]
+# additional_fields_segment | List[str]
+# fields_segment | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Segments.get_segment(id, additional_fields_segment=additional_fields_segment, fields_segment=fields_segment, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -2316,16 +2299,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
 klaviyo.Segments.get_segment_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
@@ -2367,32 +2350,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Segments.get_segment_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Segments](https://developers.klaviyo.com/en/v2023-07-15/reference/get_segments)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_segment | [str]
-# fields_tag | [str]
+# fields_segment | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 
 klaviyo.Segments.get_segments(fields_segment=fields_segment, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor)
 ```
 
 
 
@@ -2584,17 +2567,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_tag_group | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Tags.get_tag(id, fields_tag_group=fields_tag_group, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -2603,15 +2586,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 
 klaviyo.Tags.get_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
@@ -2633,29 +2616,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Tags.get_tag_group_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-07-15/reference/get_tag_groups)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Tags.get_tag_groups(fields_tag_group=fields_tag_group, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -2732,32 +2715,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 
 klaviyo.Tags.get_tag_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
 #### [Get Tags](https://developers.klaviyo.com/en/v2023-07-15/reference/get_tags)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
-# fields_tag | [str]
+# fields_tag_group | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Tags.get_tags(fields_tag_group=fields_tag_group, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -2852,29 +2835,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_template | [str]
+# fields_template | List[str]
 
 klaviyo.Templates.get_template(id, fields_template=fields_template)
 ```
 
 
 
 
 #### [Get Templates](https://developers.klaviyo.com/en/v2023-07-15/reference/get_templates)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_template | [str]
+# fields_template | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Templates.get_templates(fields_template=fields_template, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -2898,15 +2881,15 @@
 # Appendix
 
 ## Global Keyword Args
 
 NOTE: These are arguments that you can apply to any endpoint call, and which are unique to the SDK
 
 We currently support the following global keyword args:
-- `api_key` : use this to override the client-level api_key which you define upon client instantiation
+- `_request_auth` : use this to override the client-level api_key which you define upon client instantiation
 
 ## Refresher on catching exceptions:
 
 ```python
 try:
     YOUR_CALL
 except Exception as e:
@@ -2922,16 +2905,15 @@
 
 We stick to the following convention for parameters/arguments
 
 1. All parameters are passed as function args.
 2. All query and path params that are tagged as `required` in the docs are passed as positional args.
 3. All optional query params are passed as keyword args.
 4. Where applicable, the `body` param is passed in as a positional arg, and is expected to be a native python dictionary. Within that dictionary, refer to the API docs to see which fields are required/optional, along with valid values.
-4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `api_key` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
+4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `_request_auth` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
-- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
-
+- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
```

### Comparing `klaviyo-api-4.0.0/src/klaviyo_api.egg-info/SOURCES.txt` & `klaviyo-api-5.0.0/src/klaviyo_api.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,291 +8,275 @@
 src/klaviyo_api.egg-info/PKG-INFO
 src/klaviyo_api.egg-info/SOURCES.txt
 src/klaviyo_api.egg-info/dependency_links.txt
 src/klaviyo_api.egg-info/requires.txt
 src/klaviyo_api.egg-info/top_level.txt
 src/openapi_client/__init__.py
 src/openapi_client/api_client.py
+src/openapi_client/api_response.py
 src/openapi_client/configuration.py
 src/openapi_client/exceptions.py
-src/openapi_client/model_utils.py
 src/openapi_client/rest.py
 src/openapi_client/api/__init__.py
 src/openapi_client/api/accounts_api.py
 src/openapi_client/api/campaigns_api.py
 src/openapi_client/api/catalogs_api.py
 src/openapi_client/api/data_privacy_api.py
 src/openapi_client/api/events_api.py
 src/openapi_client/api/flows_api.py
 src/openapi_client/api/lists_api.py
 src/openapi_client/api/metrics_api.py
 src/openapi_client/api/profiles_api.py
 src/openapi_client/api/segments_api.py
 src/openapi_client/api/tags_api.py
 src/openapi_client/api/templates_api.py
-src/openapi_client/apis/__init__.py
-src/openapi_client/model/__init__.py
-src/openapi_client/model/audiences_sub_object.py
-src/openapi_client/model/back_in_stock_subscription_enum.py
-src/openapi_client/model/campaign_clone_query.py
-src/openapi_client/model/campaign_clone_query_resource_object.py
-src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
-src/openapi_client/model/campaign_create_query.py
-src/openapi_client/model/campaign_create_query_resource_object.py
-src/openapi_client/model/campaign_create_query_resource_object_attributes.py
-src/openapi_client/model/campaign_create_query_resource_object_attributes_campaign_messages.py
-src/openapi_client/model/campaign_create_query_resource_object_attributes_send_options.py
-src/openapi_client/model/campaign_create_query_resource_object_attributes_tracking_options.py
-src/openapi_client/model/campaign_enum.py
-src/openapi_client/model/campaign_message_assign_template_query.py
-src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
-src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
-src/openapi_client/model/campaign_message_assign_template_query_resource_object_relationships.py
-src/openapi_client/model/campaign_message_assign_template_query_resource_object_relationships_template.py
-src/openapi_client/model/campaign_message_assign_template_query_resource_object_relationships_template_data.py
-src/openapi_client/model/campaign_message_create_query_resource_object.py
-src/openapi_client/model/campaign_message_create_query_resource_object_attributes.py
-src/openapi_client/model/campaign_message_create_query_resource_object_attributes_content.py
-src/openapi_client/model/campaign_message_enum.py
-src/openapi_client/model/campaign_message_partial_update_query.py
-src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
-src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/campaign_partial_update_query.py
-src/openapi_client/model/campaign_partial_update_query_resource_object.py
-src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
-src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
-src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
-src/openapi_client/model/campaign_recipient_estimation_job_enum.py
-src/openapi_client/model/campaign_send_job_create_query.py
-src/openapi_client/model/campaign_send_job_create_query_resource_object.py
-src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
-src/openapi_client/model/campaign_send_job_enum.py
-src/openapi_client/model/campaign_send_job_partial_update_query.py
-src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
-src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/catalog_category_bulk_create_job_enum.py
-src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
-src/openapi_client/model/catalog_category_bulk_update_job_enum.py
-src/openapi_client/model/catalog_category_create_job_create_query.py
-src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
-src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes_categories.py
-src/openapi_client/model/catalog_category_create_query.py
-src/openapi_client/model/catalog_category_create_query_resource_object.py
-src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_category_delete_job_create_query.py
-src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
-src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes_categories.py
-src/openapi_client/model/catalog_category_delete_query_resource_object.py
-src/openapi_client/model/catalog_category_enum.py
-src/openapi_client/model/catalog_category_item_op.py
-src/openapi_client/model/catalog_category_update_job_create_query.py
-src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
-src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes_categories.py
-src/openapi_client/model/catalog_category_update_query.py
-src/openapi_client/model/catalog_category_update_query_resource_object.py
-src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
-src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
-src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
-src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
-src/openapi_client/model/catalog_item_bulk_create_job_enum.py
-src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
-src/openapi_client/model/catalog_item_bulk_update_job_enum.py
-src/openapi_client/model/catalog_item_category_op.py
-src/openapi_client/model/catalog_item_category_op_data_inner.py
-src/openapi_client/model/catalog_item_create_job_create_query.py
-src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
-src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes_items.py
-src/openapi_client/model/catalog_item_create_query.py
-src/openapi_client/model/catalog_item_create_query_resource_object.py
-src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
-src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
-src/openapi_client/model/catalog_item_delete_job_create_query.py
-src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
-src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes_items.py
-src/openapi_client/model/catalog_item_delete_query_resource_object.py
-src/openapi_client/model/catalog_item_enum.py
-src/openapi_client/model/catalog_item_update_job_create_query.py
-src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
-src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes_items.py
-src/openapi_client/model/catalog_item_update_query.py
-src/openapi_client/model/catalog_item_update_query_resource_object.py
-src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
-src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
-src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
-src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
-src/openapi_client/model/catalog_variant_create_job_create_query.py
-src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
-src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes_variants.py
-src/openapi_client/model/catalog_variant_create_query.py
-src/openapi_client/model/catalog_variant_create_query_resource_object.py
-src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_variant_create_query_resource_object_relationships.py
-src/openapi_client/model/catalog_variant_create_query_resource_object_relationships_item.py
-src/openapi_client/model/catalog_variant_delete_job_create_query.py
-src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
-src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes_variants.py
-src/openapi_client/model/catalog_variant_delete_query_resource_object.py
-src/openapi_client/model/catalog_variant_enum.py
-src/openapi_client/model/catalog_variant_update_job_create_query.py
-src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
-src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
-src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes_variants.py
-src/openapi_client/model/catalog_variant_update_query.py
-src/openapi_client/model/catalog_variant_update_query_resource_object.py
-src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
-src/openapi_client/model/data_privacy_create_deletion_job_query.py
-src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
-src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
-src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes_profile.py
-src/openapi_client/model/data_privacy_deletion_job_enum.py
-src/openapi_client/model/data_privacy_profile_query_resource_object.py
-src/openapi_client/model/data_privacy_profile_query_resource_object_attributes.py
-src/openapi_client/model/email_content_sub_object.py
-src/openapi_client/model/email_send_options_sub_object.py
-src/openapi_client/model/email_tracking_options_sub_object.py
-src/openapi_client/model/event_create_query_v2.py
-src/openapi_client/model/event_create_query_v2_resource_object.py
-src/openapi_client/model/event_create_query_v2_resource_object_attributes.py
-src/openapi_client/model/event_create_query_v2_resource_object_attributes_metric.py
-src/openapi_client/model/event_create_query_v2_resource_object_attributes_profile.py
-src/openapi_client/model/event_enum.py
-src/openapi_client/model/flow_enum.py
-src/openapi_client/model/flow_update_query.py
-src/openapi_client/model/flow_update_query_resource_object.py
-src/openapi_client/model/flow_update_query_resource_object_attributes.py
-src/openapi_client/model/get_create_variants_jobs5_xx_response.py
-src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
-src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
-src/openapi_client/model/list_create_query.py
-src/openapi_client/model/list_create_query_resource_object.py
-src/openapi_client/model/list_create_query_resource_object_attributes.py
-src/openapi_client/model/list_enum.py
-src/openapi_client/model/list_members_add_query.py
-src/openapi_client/model/list_members_add_query_data_inner.py
-src/openapi_client/model/list_members_delete_query.py
-src/openapi_client/model/list_partial_update_query.py
-src/openapi_client/model/list_partial_update_query_resource_object.py
-src/openapi_client/model/metric_aggregate_enum.py
-src/openapi_client/model/metric_aggregate_query.py
-src/openapi_client/model/metric_aggregate_query_resource_object.py
-src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
-src/openapi_client/model/metric_create_query_resource_object.py
-src/openapi_client/model/metric_create_query_resource_object_attributes.py
-src/openapi_client/model/metric_enum.py
-src/openapi_client/model/onsite_profile_create_query_resource_object.py
-src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
-src/openapi_client/model/onsite_profile_meta.py
-src/openapi_client/model/profile_create_query.py
-src/openapi_client/model/profile_create_query_resource_object.py
-src/openapi_client/model/profile_create_query_resource_object_attributes.py
-src/openapi_client/model/profile_enum.py
-src/openapi_client/model/profile_identifier_dto_resource_object.py
-src/openapi_client/model/profile_identifier_dto_resource_object_attributes.py
-src/openapi_client/model/profile_location.py
-src/openapi_client/model/profile_location_latitude.py
-src/openapi_client/model/profile_location_longitude.py
-src/openapi_client/model/profile_meta.py
-src/openapi_client/model/profile_meta_patch_properties.py
-src/openapi_client/model/profile_meta_patch_properties_unset.py
-src/openapi_client/model/profile_partial_update_query.py
-src/openapi_client/model/profile_partial_update_query_resource_object.py
-src/openapi_client/model/profile_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
-src/openapi_client/model/profile_subscription_bulk_delete_job_enum.py
-src/openapi_client/model/profile_subscription_create_query_resource_object.py
-src/openapi_client/model/profile_subscription_create_query_resource_object_attributes.py
-src/openapi_client/model/profile_subscription_delete_query_resource_object.py
-src/openapi_client/model/profile_subscription_delete_query_resource_object_attributes.py
-src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
-src/openapi_client/model/profile_suppression_bulk_delete_job_enum.py
-src/openapi_client/model/profile_suppression_create_query_resource_object.py
-src/openapi_client/model/profile_suppression_create_query_resource_object_attributes.py
-src/openapi_client/model/profile_suppression_delete_query_resource_object.py
-src/openapi_client/model/profile_suppression_delete_query_resource_object_attributes.py
-src/openapi_client/model/render_options_sub_object.py
-src/openapi_client/model/segment_enum.py
-src/openapi_client/model/segment_partial_update_query.py
-src/openapi_client/model/segment_partial_update_query_resource_object.py
-src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/send_strategy_sub_object.py
-src/openapi_client/model/server_bis_subscription_create_query.py
-src/openapi_client/model/server_bis_subscription_create_query_resource_object.py
-src/openapi_client/model/server_bis_subscription_create_query_resource_object_attributes.py
-src/openapi_client/model/server_bis_subscription_create_query_resource_object_attributes_profile.py
-src/openapi_client/model/server_bis_subscription_create_query_resource_object_relationships.py
-src/openapi_client/model/server_bis_subscription_create_query_resource_object_relationships_variant.py
-src/openapi_client/model/server_bis_subscription_create_query_resource_object_relationships_variant_data.py
-src/openapi_client/model/sms_content_sub_object_create.py
-src/openapi_client/model/sms_send_options_sub_object.py
-src/openapi_client/model/sms_tracking_options_sub_object.py
-src/openapi_client/model/static_schedule_options.py
-src/openapi_client/model/sto_schedule_options.py
-src/openapi_client/model/subscription_channels.py
-src/openapi_client/model/subscription_create_job_create_query.py
-src/openapi_client/model/subscription_create_job_create_query_resource_object.py
-src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes_profiles.py
-src/openapi_client/model/subscription_delete_job_create_query.py
-src/openapi_client/model/subscription_delete_job_create_query_resource_object.py
-src/openapi_client/model/subscription_delete_job_create_query_resource_object_attributes.py
-src/openapi_client/model/subscription_delete_job_create_query_resource_object_attributes_profiles.py
-src/openapi_client/model/subscription_delete_job_create_query_resource_object_relationships.py
-src/openapi_client/model/subscription_delete_job_create_query_resource_object_relationships_list.py
-src/openapi_client/model/subscription_delete_job_create_query_resource_object_relationships_list_data.py
-src/openapi_client/model/suppression_create_job_create_query.py
-src/openapi_client/model/suppression_create_job_create_query_resource_object.py
-src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes_profiles.py
-src/openapi_client/model/suppression_delete_job_create_query.py
-src/openapi_client/model/suppression_delete_job_create_query_resource_object.py
-src/openapi_client/model/suppression_delete_job_create_query_resource_object_attributes.py
-src/openapi_client/model/suppression_delete_job_create_query_resource_object_attributes_profiles.py
-src/openapi_client/model/tag_campaign_op.py
-src/openapi_client/model/tag_campaign_op_data_inner.py
-src/openapi_client/model/tag_create_query.py
-src/openapi_client/model/tag_create_query_resource_object.py
-src/openapi_client/model/tag_create_query_resource_object_relationships.py
-src/openapi_client/model/tag_create_query_resource_object_relationships_tag_group.py
-src/openapi_client/model/tag_create_query_resource_object_relationships_tag_group_data.py
-src/openapi_client/model/tag_enum.py
-src/openapi_client/model/tag_flow_op.py
-src/openapi_client/model/tag_flow_op_data_inner.py
-src/openapi_client/model/tag_group_create_query.py
-src/openapi_client/model/tag_group_create_query_resource_object.py
-src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
-src/openapi_client/model/tag_group_enum.py
-src/openapi_client/model/tag_group_update_query.py
-src/openapi_client/model/tag_group_update_query_resource_object.py
-src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
-src/openapi_client/model/tag_list_op.py
-src/openapi_client/model/tag_list_op_data_inner.py
-src/openapi_client/model/tag_segment_op.py
-src/openapi_client/model/tag_segment_op_data_inner.py
-src/openapi_client/model/tag_update_query.py
-src/openapi_client/model/tag_update_query_resource_object.py
-src/openapi_client/model/tag_update_query_resource_object_attributes.py
-src/openapi_client/model/template_clone_query.py
-src/openapi_client/model/template_clone_query_resource_object.py
-src/openapi_client/model/template_clone_query_resource_object_attributes.py
-src/openapi_client/model/template_create_query.py
-src/openapi_client/model/template_create_query_resource_object.py
-src/openapi_client/model/template_create_query_resource_object_attributes.py
-src/openapi_client/model/template_enum.py
-src/openapi_client/model/template_render_query.py
-src/openapi_client/model/template_render_query_resource_object.py
-src/openapi_client/model/template_render_query_resource_object_attributes.py
-src/openapi_client/model/template_update_query.py
-src/openapi_client/model/template_update_query_resource_object.py
-src/openapi_client/model/template_update_query_resource_object_attributes.py
-src/openapi_client/model/throttled_schedule_options.py
-src/openapi_client/model/utm_params_sub_object.py
-src/openapi_client/models/__init__.py
+src/openapi_client/models/__init__.py
+src/openapi_client/models/audiences_sub_object.py
+src/openapi_client/models/back_in_stock_subscription_enum.py
+src/openapi_client/models/campaign_clone_query.py
+src/openapi_client/models/campaign_clone_query_resource_object.py
+src/openapi_client/models/campaign_clone_query_resource_object_attributes.py
+src/openapi_client/models/campaign_create_query.py
+src/openapi_client/models/campaign_create_query_resource_object.py
+src/openapi_client/models/campaign_create_query_resource_object_attributes.py
+src/openapi_client/models/campaign_create_query_resource_object_attributes_campaign_messages.py
+src/openapi_client/models/campaign_enum.py
+src/openapi_client/models/campaign_message_assign_template_query.py
+src/openapi_client/models/campaign_message_assign_template_query_resource_object.py
+src/openapi_client/models/campaign_message_assign_template_query_resource_object_attributes.py
+src/openapi_client/models/campaign_message_assign_template_query_resource_object_relationships.py
+src/openapi_client/models/campaign_message_assign_template_query_resource_object_relationships_template.py
+src/openapi_client/models/campaign_message_assign_template_query_resource_object_relationships_template_data.py
+src/openapi_client/models/campaign_message_create_query_resource_object.py
+src/openapi_client/models/campaign_message_create_query_resource_object_attributes.py
+src/openapi_client/models/campaign_message_enum.py
+src/openapi_client/models/campaign_message_partial_update_query.py
+src/openapi_client/models/campaign_message_partial_update_query_resource_object.py
+src/openapi_client/models/campaign_message_partial_update_query_resource_object_attributes.py
+src/openapi_client/models/campaign_partial_update_query.py
+src/openapi_client/models/campaign_partial_update_query_resource_object.py
+src/openapi_client/models/campaign_partial_update_query_resource_object_attributes.py
+src/openapi_client/models/campaign_recipient_estimation_job_create_query.py
+src/openapi_client/models/campaign_recipient_estimation_job_create_query_resource_object.py
+src/openapi_client/models/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
+src/openapi_client/models/campaign_recipient_estimation_job_enum.py
+src/openapi_client/models/campaign_send_job_create_query.py
+src/openapi_client/models/campaign_send_job_create_query_resource_object.py
+src/openapi_client/models/campaign_send_job_create_query_resource_object_attributes.py
+src/openapi_client/models/campaign_send_job_enum.py
+src/openapi_client/models/campaign_send_job_partial_update_query.py
+src/openapi_client/models/campaign_send_job_partial_update_query_resource_object.py
+src/openapi_client/models/campaign_send_job_partial_update_query_resource_object_attributes.py
+src/openapi_client/models/catalog_category_bulk_create_job_enum.py
+src/openapi_client/models/catalog_category_bulk_delete_job_enum.py
+src/openapi_client/models/catalog_category_bulk_update_job_enum.py
+src/openapi_client/models/catalog_category_create_job_create_query.py
+src/openapi_client/models/catalog_category_create_job_create_query_resource_object.py
+src/openapi_client/models/catalog_category_create_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_category_create_job_create_query_resource_object_attributes_categories.py
+src/openapi_client/models/catalog_category_create_query.py
+src/openapi_client/models/catalog_category_create_query_resource_object.py
+src/openapi_client/models/catalog_category_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_category_create_query_resource_object_relationships.py
+src/openapi_client/models/catalog_category_create_query_resource_object_relationships_items.py
+src/openapi_client/models/catalog_category_delete_job_create_query.py
+src/openapi_client/models/catalog_category_delete_job_create_query_resource_object.py
+src/openapi_client/models/catalog_category_delete_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_category_delete_job_create_query_resource_object_attributes_categories.py
+src/openapi_client/models/catalog_category_delete_query_resource_object.py
+src/openapi_client/models/catalog_category_enum.py
+src/openapi_client/models/catalog_category_item_op.py
+src/openapi_client/models/catalog_category_update_job_create_query.py
+src/openapi_client/models/catalog_category_update_job_create_query_resource_object.py
+src/openapi_client/models/catalog_category_update_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_category_update_job_create_query_resource_object_attributes_categories.py
+src/openapi_client/models/catalog_category_update_query.py
+src/openapi_client/models/catalog_category_update_query_resource_object.py
+src/openapi_client/models/catalog_category_update_query_resource_object_attributes.py
+src/openapi_client/models/catalog_item_bulk_create_job_enum.py
+src/openapi_client/models/catalog_item_bulk_delete_job_enum.py
+src/openapi_client/models/catalog_item_bulk_update_job_enum.py
+src/openapi_client/models/catalog_item_category_op.py
+src/openapi_client/models/catalog_item_create_job_create_query.py
+src/openapi_client/models/catalog_item_create_job_create_query_resource_object.py
+src/openapi_client/models/catalog_item_create_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_item_create_job_create_query_resource_object_attributes_items.py
+src/openapi_client/models/catalog_item_create_query.py
+src/openapi_client/models/catalog_item_create_query_resource_object.py
+src/openapi_client/models/catalog_item_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_item_create_query_resource_object_relationships.py
+src/openapi_client/models/catalog_item_create_query_resource_object_relationships_categories.py
+src/openapi_client/models/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
+src/openapi_client/models/catalog_item_delete_job_create_query.py
+src/openapi_client/models/catalog_item_delete_job_create_query_resource_object.py
+src/openapi_client/models/catalog_item_delete_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_item_delete_job_create_query_resource_object_attributes_items.py
+src/openapi_client/models/catalog_item_delete_query_resource_object.py
+src/openapi_client/models/catalog_item_enum.py
+src/openapi_client/models/catalog_item_update_job_create_query.py
+src/openapi_client/models/catalog_item_update_job_create_query_resource_object.py
+src/openapi_client/models/catalog_item_update_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_item_update_job_create_query_resource_object_attributes_items.py
+src/openapi_client/models/catalog_item_update_query.py
+src/openapi_client/models/catalog_item_update_query_resource_object.py
+src/openapi_client/models/catalog_item_update_query_resource_object_attributes.py
+src/openapi_client/models/catalog_variant_bulk_create_job_enum.py
+src/openapi_client/models/catalog_variant_bulk_delete_job_enum.py
+src/openapi_client/models/catalog_variant_bulk_update_job_enum.py
+src/openapi_client/models/catalog_variant_create_job_create_query.py
+src/openapi_client/models/catalog_variant_create_job_create_query_resource_object.py
+src/openapi_client/models/catalog_variant_create_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_variant_create_job_create_query_resource_object_attributes_variants.py
+src/openapi_client/models/catalog_variant_create_query.py
+src/openapi_client/models/catalog_variant_create_query_resource_object.py
+src/openapi_client/models/catalog_variant_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_variant_create_query_resource_object_relationships.py
+src/openapi_client/models/catalog_variant_create_query_resource_object_relationships_item.py
+src/openapi_client/models/catalog_variant_create_query_resource_object_relationships_item_data.py
+src/openapi_client/models/catalog_variant_delete_job_create_query.py
+src/openapi_client/models/catalog_variant_delete_job_create_query_resource_object.py
+src/openapi_client/models/catalog_variant_delete_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_variant_delete_job_create_query_resource_object_attributes_variants.py
+src/openapi_client/models/catalog_variant_delete_query_resource_object.py
+src/openapi_client/models/catalog_variant_enum.py
+src/openapi_client/models/catalog_variant_update_job_create_query.py
+src/openapi_client/models/catalog_variant_update_job_create_query_resource_object.py
+src/openapi_client/models/catalog_variant_update_job_create_query_resource_object_attributes.py
+src/openapi_client/models/catalog_variant_update_job_create_query_resource_object_attributes_variants.py
+src/openapi_client/models/catalog_variant_update_query.py
+src/openapi_client/models/catalog_variant_update_query_resource_object.py
+src/openapi_client/models/catalog_variant_update_query_resource_object_attributes.py
+src/openapi_client/models/data_privacy_create_deletion_job_query.py
+src/openapi_client/models/data_privacy_create_deletion_job_query_resource_object.py
+src/openapi_client/models/data_privacy_create_deletion_job_query_resource_object_attributes.py
+src/openapi_client/models/data_privacy_create_deletion_job_query_resource_object_attributes_profile.py
+src/openapi_client/models/data_privacy_deletion_job_enum.py
+src/openapi_client/models/data_privacy_profile_query_resource_object.py
+src/openapi_client/models/data_privacy_profile_query_resource_object_attributes.py
+src/openapi_client/models/event_create_query_v2.py
+src/openapi_client/models/event_create_query_v2_resource_object.py
+src/openapi_client/models/event_create_query_v2_resource_object_attributes.py
+src/openapi_client/models/event_create_query_v2_resource_object_attributes_metric.py
+src/openapi_client/models/event_create_query_v2_resource_object_attributes_profile.py
+src/openapi_client/models/event_enum.py
+src/openapi_client/models/flow_enum.py
+src/openapi_client/models/flow_update_query.py
+src/openapi_client/models/flow_update_query_resource_object.py
+src/openapi_client/models/flow_update_query_resource_object_attributes.py
+src/openapi_client/models/get_accounts4_xx_response.py
+src/openapi_client/models/get_accounts4_xx_response_errors_inner.py
+src/openapi_client/models/get_accounts4_xx_response_errors_inner_source.py
+src/openapi_client/models/list_create_query.py
+src/openapi_client/models/list_create_query_resource_object.py
+src/openapi_client/models/list_create_query_resource_object_attributes.py
+src/openapi_client/models/list_enum.py
+src/openapi_client/models/list_members_add_query.py
+src/openapi_client/models/list_members_add_query_data_inner.py
+src/openapi_client/models/list_members_delete_query.py
+src/openapi_client/models/list_partial_update_query.py
+src/openapi_client/models/list_partial_update_query_resource_object.py
+src/openapi_client/models/metric_aggregate_enum.py
+src/openapi_client/models/metric_aggregate_query.py
+src/openapi_client/models/metric_aggregate_query_resource_object.py
+src/openapi_client/models/metric_aggregate_query_resource_object_attributes.py
+src/openapi_client/models/metric_create_query_resource_object.py
+src/openapi_client/models/metric_create_query_resource_object_attributes.py
+src/openapi_client/models/metric_enum.py
+src/openapi_client/models/onsite_profile_create_query_resource_object.py
+src/openapi_client/models/onsite_profile_create_query_resource_object_attributes.py
+src/openapi_client/models/onsite_profile_meta.py
+src/openapi_client/models/profile_create_query.py
+src/openapi_client/models/profile_create_query_resource_object.py
+src/openapi_client/models/profile_create_query_resource_object_attributes.py
+src/openapi_client/models/profile_enum.py
+src/openapi_client/models/profile_identifier_dto_resource_object.py
+src/openapi_client/models/profile_identifier_dto_resource_object_attributes.py
+src/openapi_client/models/profile_location.py
+src/openapi_client/models/profile_meta.py
+src/openapi_client/models/profile_meta_patch_properties.py
+src/openapi_client/models/profile_partial_update_query.py
+src/openapi_client/models/profile_partial_update_query_resource_object.py
+src/openapi_client/models/profile_subscription_bulk_create_job_enum.py
+src/openapi_client/models/profile_subscription_bulk_delete_job_enum.py
+src/openapi_client/models/profile_subscription_create_query_resource_object.py
+src/openapi_client/models/profile_subscription_create_query_resource_object_attributes.py
+src/openapi_client/models/profile_subscription_delete_query_resource_object.py
+src/openapi_client/models/profile_subscription_delete_query_resource_object_attributes.py
+src/openapi_client/models/profile_suppression_bulk_create_job_enum.py
+src/openapi_client/models/profile_suppression_bulk_delete_job_enum.py
+src/openapi_client/models/profile_suppression_create_query_resource_object.py
+src/openapi_client/models/profile_suppression_create_query_resource_object_attributes.py
+src/openapi_client/models/profile_suppression_delete_query_resource_object.py
+src/openapi_client/models/profile_suppression_delete_query_resource_object_attributes.py
+src/openapi_client/models/render_options_sub_object.py
+src/openapi_client/models/segment_enum.py
+src/openapi_client/models/segment_partial_update_query.py
+src/openapi_client/models/segment_partial_update_query_resource_object.py
+src/openapi_client/models/segment_partial_update_query_resource_object_attributes.py
+src/openapi_client/models/send_strategy_sub_object.py
+src/openapi_client/models/server_bis_subscription_create_query.py
+src/openapi_client/models/server_bis_subscription_create_query_resource_object.py
+src/openapi_client/models/server_bis_subscription_create_query_resource_object_attributes.py
+src/openapi_client/models/server_bis_subscription_create_query_resource_object_attributes_profile.py
+src/openapi_client/models/server_bis_subscription_create_query_resource_object_relationships.py
+src/openapi_client/models/server_bis_subscription_create_query_resource_object_relationships_variant.py
+src/openapi_client/models/server_bis_subscription_create_query_resource_object_relationships_variant_data.py
+src/openapi_client/models/static_schedule_options.py
+src/openapi_client/models/sto_schedule_options.py
+src/openapi_client/models/subscription_channels.py
+src/openapi_client/models/subscription_create_job_create_query.py
+src/openapi_client/models/subscription_create_job_create_query_resource_object.py
+src/openapi_client/models/subscription_create_job_create_query_resource_object_attributes.py
+src/openapi_client/models/subscription_create_job_create_query_resource_object_attributes_profiles.py
+src/openapi_client/models/subscription_create_job_create_query_resource_object_relationships.py
+src/openapi_client/models/subscription_create_job_create_query_resource_object_relationships_list.py
+src/openapi_client/models/subscription_create_job_create_query_resource_object_relationships_list_data.py
+src/openapi_client/models/subscription_delete_job_create_query.py
+src/openapi_client/models/subscription_delete_job_create_query_resource_object.py
+src/openapi_client/models/subscription_delete_job_create_query_resource_object_attributes.py
+src/openapi_client/models/subscription_delete_job_create_query_resource_object_attributes_profiles.py
+src/openapi_client/models/suppression_create_job_create_query.py
+src/openapi_client/models/suppression_create_job_create_query_resource_object.py
+src/openapi_client/models/suppression_create_job_create_query_resource_object_attributes.py
+src/openapi_client/models/suppression_create_job_create_query_resource_object_attributes_profiles.py
+src/openapi_client/models/suppression_delete_job_create_query.py
+src/openapi_client/models/suppression_delete_job_create_query_resource_object.py
+src/openapi_client/models/suppression_delete_job_create_query_resource_object_attributes.py
+src/openapi_client/models/suppression_delete_job_create_query_resource_object_attributes_profiles.py
+src/openapi_client/models/tag_campaign_op.py
+src/openapi_client/models/tag_campaign_op_data_inner.py
+src/openapi_client/models/tag_create_query.py
+src/openapi_client/models/tag_create_query_resource_object.py
+src/openapi_client/models/tag_create_query_resource_object_attributes.py
+src/openapi_client/models/tag_create_query_resource_object_relationships.py
+src/openapi_client/models/tag_create_query_resource_object_relationships_tag_group.py
+src/openapi_client/models/tag_create_query_resource_object_relationships_tag_group_data.py
+src/openapi_client/models/tag_enum.py
+src/openapi_client/models/tag_flow_op.py
+src/openapi_client/models/tag_flow_op_data_inner.py
+src/openapi_client/models/tag_group_create_query.py
+src/openapi_client/models/tag_group_create_query_resource_object.py
+src/openapi_client/models/tag_group_create_query_resource_object_attributes.py
+src/openapi_client/models/tag_group_enum.py
+src/openapi_client/models/tag_group_update_query.py
+src/openapi_client/models/tag_group_update_query_resource_object.py
+src/openapi_client/models/tag_group_update_query_resource_object_attributes.py
+src/openapi_client/models/tag_list_op.py
+src/openapi_client/models/tag_list_op_data_inner.py
+src/openapi_client/models/tag_segment_op.py
+src/openapi_client/models/tag_segment_op_data_inner.py
+src/openapi_client/models/tag_update_query.py
+src/openapi_client/models/tag_update_query_resource_object.py
+src/openapi_client/models/template_clone_query.py
+src/openapi_client/models/template_clone_query_resource_object.py
+src/openapi_client/models/template_clone_query_resource_object_attributes.py
+src/openapi_client/models/template_create_query.py
+src/openapi_client/models/template_create_query_resource_object.py
+src/openapi_client/models/template_create_query_resource_object_attributes.py
+src/openapi_client/models/template_enum.py
+src/openapi_client/models/template_render_query.py
+src/openapi_client/models/template_render_query_resource_object.py
+src/openapi_client/models/template_render_query_resource_object_attributes.py
+src/openapi_client/models/template_update_query.py
+src/openapi_client/models/template_update_query_resource_object.py
+src/openapi_client/models/template_update_query_resource_object_attributes.py
+src/openapi_client/models/throttled_schedule_options.py
```

### Comparing `klaviyo-api-4.0.0/src/klaviyo_api.egg-info/PKG-INFO` & `klaviyo-api-5.0.0/src/klaviyo_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: klaviyo-api
-Version: 4.0.0
+Version: 5.0.0
 Summary: Klaviyo Python SDK
 Home-page: https://github.com/klaviyo/klaviyo-api-python
 Author: Klaviyo Developers
 Author-email: developers@klaviyo.com
-License: UNKNOWN
 Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Klaviyo Python SDK
 
-- SDK version: 4.0.0
+- SDK version: 5.0.0
 - API revision: 2023-07-15
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-07-15/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-07-15/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
@@ -111,15 +109,15 @@
 * The SDK retries on resolvable errors, namely: rate limits (common) and server errors (rare).
 * The keyword arguments define some advanced settings; the example is populated with the default values.
 * `max_delay` denotes total delay (in seconds) across all attempts.
 
 ```python
 from klaviyo_api import KlaviyoAPI
 
-klaviyo = KlaviyoAPI("YOUR API KEY HERE", max_delay=60, max_retries=3, test_host=None)
+klaviyo = KlaviyoAPI("YOUR_API_KEY_HERE", max_delay=60, max_retries=3, test_host=None)
 ```
 
 ### Example request
 
 ```python
 klaviyo.Metrics.get_metrics() 
 ```
@@ -219,15 +217,15 @@
 ## Important Notes
 
 - The main difference between this SDK and the language-agnostic API Docs that the below endpoints link to is that this SDK automatically adds the `revision` header corresponding to the SDK version.
 - Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-07-15/reference/get_events).
 - For example values / data types, as well as whether parameters are required/optional, please reference the corresponding API Reference link.
 - Some keyword args may potentially be required for the API call to succeed, the linked API docs are the source of truth regarding which keyword params are required.
 - JSON payloads should be passed in as native python dictionaries.
-- You can override the client private key by passing in an optional `api_key` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
+- You can override the client private key by passing in an optional `_request_auth` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
 
 # Comprehensive list of Operations & Parameters
 
 
 
 
 
@@ -238,29 +236,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_account | [str]
+# fields_account | List[str]
 
 klaviyo.Accounts.get_account(id, fields_account=fields_account)
 ```
 
 
 
 
 #### [Get Accounts](https://developers.klaviyo.com/en/v2023-07-15/reference/get_accounts)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_account | [str]
+# fields_account | List[str]
 
 klaviyo.Accounts.get_accounts(fields_account=fields_account)
 ```
 
 
 
 
@@ -351,18 +349,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -371,18 +369,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_template | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_template | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign_campaign_messages(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_template=fields_template, include=include)
 ```
 
 
 
 
@@ -391,18 +389,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_template | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_template | List[str]
+# include | List[str]
 
 klaviyo.Campaigns.get_campaign_message(id, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_template=fields_template, include=include)
 ```
 
 
 
 
@@ -411,15 +409,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
+# fields_campaign_message | List[str]
 
 klaviyo.Campaigns.get_campaign_message_campaign(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
@@ -454,15 +452,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
+# fields_campaign_message | List[str]
 
 klaviyo.Campaigns.get_campaign_message_template(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
@@ -471,15 +469,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_recipient_estimation | [str]
+# fields_campaign_recipient_estimation | List[str]
 
 klaviyo.Campaigns.get_campaign_recipient_estimation(id, fields_campaign_recipient_estimation=fields_campaign_recipient_estimation)
 ```
 
 
 
 
@@ -488,15 +486,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_recipient_estimation_job | [str]
+# fields_campaign_recipient_estimation_job | List[str]
 
 klaviyo.Campaigns.get_campaign_recipient_estimation_job(id, fields_campaign_recipient_estimation_job=fields_campaign_recipient_estimation_job)
 ```
 
 
 
 
@@ -531,15 +529,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_campaign_send_job | [str]
+# fields_campaign_send_job | List[str]
 
 klaviyo.Campaigns.get_campaign_send_job(id, fields_campaign_send_job=fields_campaign_send_job)
 ```
 
 
 
 
@@ -548,15 +546,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Campaigns.get_campaign_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
@@ -565,18 +563,18 @@
 ```python
 ## Positional Arguments
 
 # filter | str
 
 ## Keyword Arguments
 
-# fields_campaign_message | [str]
-# fields_campaign | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_campaign_message | List[str]
+# fields_campaign | List[str]
+# fields_tag | List[str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Campaigns.get_campaigns(filter, fields_campaign_message=fields_campaign_message, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -777,15 +775,15 @@
 
 #### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_categories)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_categories(fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -797,15 +795,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 
 klaviyo.Catalogs.get_catalog_category(id, fields_catalog_category=fields_catalog_category)
 ```
 
 
 
 
@@ -814,18 +812,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_category_items(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -853,17 +851,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_catalog_item(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
@@ -872,15 +870,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category | [str]
+# fields_catalog_category | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_item_categories(id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -909,15 +907,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_item_variants(id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -926,18 +924,18 @@
 
 #### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_items)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item | [str]
-# fields_catalog_variant | [str]
+# fields_catalog_item | List[str]
+# fields_catalog_variant | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_items(fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -948,29 +946,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 
 klaviyo.Catalogs.get_catalog_variant(id, fields_catalog_variant=fields_catalog_variant)
 ```
 
 
 
 
 #### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-07-15/reference/get_catalog_variants)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant | [str]
+# fields_catalog_variant | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Catalogs.get_catalog_variants(fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -982,31 +980,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_create_job | [str]
-# fields_catalog_category | [str]
-# include | [str]
+# fields_catalog_category_bulk_create_job | List[str]
+# fields_catalog_category | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_categories_job(job_id, fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
 #### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_create_job | [str]
+# fields_catalog_category_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_categories_jobs(fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1017,31 +1015,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_create_job | [str]
-# fields_catalog_item | [str]
-# include | [str]
+# fields_catalog_item_bulk_create_job | List[str]
+# fields_catalog_item | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_items_job(job_id, fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
 #### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_create_job | [str]
+# fields_catalog_item_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_items_jobs(fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1052,31 +1050,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_create_job | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_variant_bulk_create_job | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_create_variants_job(job_id, fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
 #### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_create_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_create_job | [str]
+# fields_catalog_variant_bulk_create_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_create_variants_jobs(fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1087,29 +1085,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_delete_job | [str]
+# fields_catalog_category_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_categories_job(job_id, fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_delete_job | [str]
+# fields_catalog_category_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_categories_jobs(fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1120,29 +1118,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_delete_job | [str]
+# fields_catalog_item_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_items_job(job_id, fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_delete_job | [str]
+# fields_catalog_item_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_items_jobs(fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1153,29 +1151,29 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_delete_job | [str]
+# fields_catalog_variant_bulk_delete_job | List[str]
 
 klaviyo.Catalogs.get_delete_variants_job(job_id, fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job)
 ```
 
 
 
 
 #### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_delete_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_delete_job | [str]
+# fields_catalog_variant_bulk_delete_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_delete_variants_jobs(fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1186,31 +1184,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_update_job | [str]
-# fields_catalog_category | [str]
-# include | [str]
+# fields_catalog_category_bulk_update_job | List[str]
+# fields_catalog_category | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_categories_job(job_id, fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
 #### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_category_bulk_update_job | [str]
+# fields_catalog_category_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_categories_jobs(fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1221,31 +1219,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_update_job | [str]
-# fields_catalog_item | [str]
-# include | [str]
+# fields_catalog_item_bulk_update_job | List[str]
+# fields_catalog_item | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_items_job(job_id, fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
 #### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_item_bulk_update_job | [str]
+# fields_catalog_item_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_items_jobs(fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1256,31 +1254,31 @@
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_update_job | [str]
-# fields_catalog_variant | [str]
-# include | [str]
+# fields_catalog_variant_bulk_update_job | List[str]
+# fields_catalog_variant | List[str]
+# include | List[str]
 
 klaviyo.Catalogs.get_update_variants_job(job_id, fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
 #### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-07-15/reference/get_update_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_catalog_variant_bulk_update_job | [str]
+# fields_catalog_variant_bulk_update_job | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Catalogs.get_update_variants_jobs(fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -1512,18 +1510,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_event | [str]
-# fields_metric | [str]
-# fields_profile | [str]
-# include | [str]
+# fields_event | List[str]
+# fields_metric | List[str]
+# fields_profile | List[str]
+# include | List[str]
 
 klaviyo.Events.get_event(id, fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, include=include)
 ```
 
 
 
 
@@ -1532,15 +1530,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 
 klaviyo.Events.get_event_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
@@ -1549,16 +1547,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 
 klaviyo.Events.get_event_profile(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile)
 ```
 
 
 
 
@@ -1590,19 +1588,19 @@
 
 #### [Get Events](https://developers.klaviyo.com/en/v2023-07-15/reference/get_events)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_event | [str]
-# fields_metric | [str]
-# fields_profile | [str]
+# fields_event | List[str]
+# fields_metric | List[str]
+# fields_profile | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Events.get_events(fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -1617,18 +1615,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow(id, fields_flow_action=fields_flow_action, fields_flow=fields_flow, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -1637,18 +1635,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow_message | [str]
-# fields_flow | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow_message | List[str]
+# fields_flow | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow_action(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
@@ -1657,15 +1655,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow | [str]
+# fields_flow | List[str]
 
 klaviyo.Flows.get_flow_action_flow(id, fields_flow=fields_flow)
 ```
 
 
 
 
@@ -1674,15 +1672,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_message | [str]
+# fields_flow_message | List[str]
 # filter | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flow_action_messages(id, fields_flow_message=fields_flow_message, filter=filter, page_size=page_size, sort=sort)
 ```
 
@@ -1727,15 +1725,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
+# fields_flow_action | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flow_flow_actions(id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
@@ -1748,17 +1746,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow_message | [str]
-# include | [str]
+# fields_flow_action | List[str]
+# fields_flow_message | List[str]
+# include | List[str]
 
 klaviyo.Flows.get_flow_message(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, include=include)
 ```
 
 
 
 
@@ -1767,15 +1765,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
+# fields_flow_action | List[str]
 
 klaviyo.Flows.get_flow_message_action(id, fields_flow_action=fields_flow_action)
 ```
 
 
 
 
@@ -1829,33 +1827,33 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Flows.get_flow_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Flows](https://developers.klaviyo.com/en/v2023-07-15/reference/get_flows)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_flow_action | [str]
-# fields_flow | [str]
-# fields_tag | [str]
+# fields_flow_action | List[str]
+# fields_flow | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
@@ -1939,18 +1937,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_list | [str]
-# fields_list | [str]
-# fields_tag | [str]
-# include | [str]
+# additional_fields_list | List[str]
+# fields_list | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Lists.get_list(id, additional_fields_list=additional_fields_list, fields_list=fields_list, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -1959,16 +1957,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
 klaviyo.Lists.get_list_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
@@ -2010,32 +2008,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Lists.get_list_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Lists](https://developers.klaviyo.com/en/v2023-07-15/reference/get_lists)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_list | [str]
-# fields_tag | [str]
+# fields_list | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 
 klaviyo.Lists.get_lists(fields_list=fields_list, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor)
 ```
 
 
 
@@ -2063,29 +2061,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 
 klaviyo.Metrics.get_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
 #### [Get Metrics](https://developers.klaviyo.com/en/v2023-07-15/reference/get_metrics)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_metric | [str]
+# fields_metric | List[str]
 # filter | str
 # page_cursor | str
 
 klaviyo.Metrics.get_metrics(fields_metric=fields_metric, filter=filter, page_cursor=page_cursor)
 ```
 
 
@@ -2126,19 +2124,19 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_list | [str]
-# fields_profile | [str]
-# fields_segment | [str]
-# include | [str]
+# additional_fields_profile | List[str]
+# fields_list | List[str]
+# fields_profile | List[str]
+# fields_segment | List[str]
+# include | List[str]
 
 klaviyo.Profiles.get_profile(id, additional_fields_profile=additional_fields_profile, fields_list=fields_list, fields_profile=fields_profile, fields_segment=fields_segment, include=include)
 ```
 
 
 
 
@@ -2147,15 +2145,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_list | [str]
+# fields_list | List[str]
 
 klaviyo.Profiles.get_profile_lists(id, fields_list=fields_list)
 ```
 
 
 
 
@@ -2190,30 +2188,30 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_segment | [str]
+# fields_segment | List[str]
 
 klaviyo.Profiles.get_profile_segments(id, fields_segment=fields_segment)
 ```
 
 
 
 
 #### [Get Profiles](https://developers.klaviyo.com/en/v2023-07-15/reference/get_profiles)
 
 ```python
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
 klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
@@ -2296,18 +2294,18 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_segment | [str]
-# fields_segment | [str]
-# fields_tag | [str]
-# include | [str]
+# additional_fields_segment | List[str]
+# fields_segment | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Segments.get_segment(id, additional_fields_segment=additional_fields_segment, fields_segment=fields_segment, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -2316,16 +2314,16 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# additional_fields_profile | [str]
-# fields_profile | [str]
+# additional_fields_profile | List[str]
+# fields_profile | List[str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
 klaviyo.Segments.get_segment_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
@@ -2367,32 +2365,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Segments.get_segment_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Segments](https://developers.klaviyo.com/en/v2023-07-15/reference/get_segments)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_segment | [str]
-# fields_tag | [str]
+# fields_segment | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 
 klaviyo.Segments.get_segments(fields_segment=fields_segment, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor)
 ```
 
 
 
@@ -2584,17 +2582,17 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
-# fields_tag | [str]
-# include | [str]
+# fields_tag_group | List[str]
+# fields_tag | List[str]
+# include | List[str]
 
 klaviyo.Tags.get_tag(id, fields_tag_group=fields_tag_group, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
@@ -2603,15 +2601,15 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 
 klaviyo.Tags.get_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
@@ -2633,29 +2631,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag | [str]
+# fields_tag | List[str]
 
 klaviyo.Tags.get_tag_group_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
 #### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-07-15/reference/get_tag_groups)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Tags.get_tag_groups(fields_tag_group=fields_tag_group, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -2732,32 +2730,32 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
+# fields_tag_group | List[str]
 
 klaviyo.Tags.get_tag_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
 #### [Get Tags](https://developers.klaviyo.com/en/v2023-07-15/reference/get_tags)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_tag_group | [str]
-# fields_tag | [str]
+# fields_tag_group | List[str]
+# fields_tag | List[str]
 # filter | str
-# include | [str]
+# include | List[str]
 # page_cursor | str
 # sort | str
 
 klaviyo.Tags.get_tags(fields_tag_group=fields_tag_group, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
@@ -2852,29 +2850,29 @@
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
-# fields_template | [str]
+# fields_template | List[str]
 
 klaviyo.Templates.get_template(id, fields_template=fields_template)
 ```
 
 
 
 
 #### [Get Templates](https://developers.klaviyo.com/en/v2023-07-15/reference/get_templates)
 
 ```python
 
 ## Keyword Arguments
 
-# fields_template | [str]
+# fields_template | List[str]
 # filter | str
 # page_cursor | str
 # sort | str
 
 klaviyo.Templates.get_templates(fields_template=fields_template, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
@@ -2898,15 +2896,15 @@
 # Appendix
 
 ## Global Keyword Args
 
 NOTE: These are arguments that you can apply to any endpoint call, and which are unique to the SDK
 
 We currently support the following global keyword args:
-- `api_key` : use this to override the client-level api_key which you define upon client instantiation
+- `_request_auth` : use this to override the client-level api_key which you define upon client instantiation
 
 ## Refresher on catching exceptions:
 
 ```python
 try:
     YOUR_CALL
 except Exception as e:
@@ -2922,16 +2920,15 @@
 
 We stick to the following convention for parameters/arguments
 
 1. All parameters are passed as function args.
 2. All query and path params that are tagged as `required` in the docs are passed as positional args.
 3. All optional query params are passed as keyword args.
 4. Where applicable, the `body` param is passed in as a positional arg, and is expected to be a native python dictionary. Within that dictionary, refer to the API docs to see which fields are required/optional, along with valid values.
-4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `api_key` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
+4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `_request_auth` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
 - function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
-
```

### Comparing `klaviyo-api-4.0.0/src/openapi_client/configuration.py` & `klaviyo-api-5.0.0/src/openapi_client/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,62 @@
+# coding: utf-8
+
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
     The version of the OpenAPI document: 2023-07-15
     Contact: developers@klaviyo.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from openapi_client.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
+      in PEM format.
 
     :Example:
 
     API Key Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
@@ -99,18 +76,16 @@
        Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
-                 access_token=None,
                  username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
+                 access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
         self._base_path = "https://a.klaviyo.com" if host is None else host
@@ -124,15 +99,14 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
@@ -144,16 +118,17 @@
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("openapi_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -184,43 +159,53 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -230,46 +215,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -315,23 +303,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -406,15 +394,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2023-07-15\n"\
-               "SDK Package Version: 4.0.0".\
+               "SDK Package Version: 5.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `klaviyo-api-4.0.0/src/openapi_client/rest.py` & `klaviyo-api-5.0.0/src/openapi_client/rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+# coding: utf-8
+
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
     The version of the OpenAPI document: 2023-07-15
     Contact: developers@klaviyo.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
 
 import io
 import json
 import logging
 import re
 import ssl
-from urllib.parse import urlencode
-from urllib.parse import urlparse
-from urllib.request import proxy_bypass_environment
+
+from urllib.parse import urlencode, quote_plus
 import urllib3
-import ipaddress
 
 from openapi_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -32,19 +34,19 @@
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
+        return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
@@ -61,26 +63,29 @@
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.tls_server_name:
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
+
+
         if configuration.socket_options is not None:
             addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
-        if configuration.proxy and not should_bypass_proxies(
-                configuration.host, no_proxy=configuration.no_proxy or ''):
+        if configuration.proxy:
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
@@ -127,34 +132,33 @@
         if post_params and body:
             raise ApiValueError(
                 "body parameter cannot be used with post_params parameter."
             )
 
         post_params = post_params or {}
         headers = headers or {}
+        # url already contains the URL query string
+        # so reset query_params to empty dict
+        query_params = {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
+            if isinstance(_request_timeout, (int,float)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif (isinstance(_request_timeout, tuple) and
                   len(_request_timeout) == 2):
                 timeout = urllib3.Timeout(
                     connect=_request_timeout[0], read=_request_timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
-                if (method != 'DELETE') and ('Content-Type' not in headers):
-                    headers['Content-Type'] = 'application/json'
-                if query_params:
-                    url += '?' + urlencode(query_params)
-                if ('Content-Type' not in headers) or (re.search('json',
-                                                                 headers['Content-Type'], re.IGNORECASE)):
+
+                # no content type provided or payload is json
+                if not headers.get('Content-Type') or re.search('json', headers['Content-Type'], re.IGNORECASE):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
@@ -196,15 +200,15 @@
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
                 r = self.pool_manager.request(method, url,
-                                              fields=query_params,
+                                              fields={},
                                               preload_content=_preload_content,
                                               timeout=timeout,
                                               headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
@@ -227,127 +231,71 @@
             if 500 <= r.status <= 599:
                 raise ServiceException(http_resp=r)
 
             raise ApiException(http_resp=r)
 
         return r
 
-    def GET(self, url, headers=None, query_params=None, _preload_content=True,
+    def get_request(self, url, headers=None, query_params=None, _preload_content=True,
             _request_timeout=None):
         return self.request("GET", url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
-    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
+    def head_request(self, url, headers=None, query_params=None, _preload_content=True,
              _request_timeout=None):
         return self.request("HEAD", url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
-    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
+    def options_request(self, url, headers=None, query_params=None, post_params=None,
                 body=None, _preload_content=True, _request_timeout=None):
         return self.request("OPTIONS", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def DELETE(self, url, headers=None, query_params=None, body=None,
+    def delete_request(self, url, headers=None, query_params=None, body=None,
                _preload_content=True, _request_timeout=None):
         return self.request("DELETE", url,
                             headers=headers,
                             query_params=query_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def POST(self, url, headers=None, query_params=None, post_params=None,
+    def post_request(self, url, headers=None, query_params=None, post_params=None,
              body=None, _preload_content=True, _request_timeout=None):
         return self.request("POST", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def PUT(self, url, headers=None, query_params=None, post_params=None,
+    def put_request(self, url, headers=None, query_params=None, post_params=None,
             body=None, _preload_content=True, _request_timeout=None):
         return self.request("PUT", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def PATCH(self, url, headers=None, query_params=None, post_params=None,
+    def patch_request(self, url, headers=None, query_params=None, post_params=None,
               body=None, _preload_content=True, _request_timeout=None):
         return self.request("PATCH", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
-
-# end of class RESTClientObject
-
-
-def is_ipv4(target):
-    """ Test if IPv4 address or not
-    """
-    try:
-        chk = ipaddress.IPv4Address(target)
-        return True
-    except ipaddress.AddressValueError:
-        return False
-
-
-def in_ipv4net(target, net):
-    """ Test if target belongs to given IPv4 network
-    """
-    try:
-        nw = ipaddress.IPv4Network(net)
-        ip = ipaddress.IPv4Address(target)
-        if ip in nw:
-            return True
-        return False
-    except ipaddress.AddressValueError:
-        return False
-    except ipaddress.NetmaskValueError:
-        return False
-
-
-def should_bypass_proxies(url, no_proxy=None):
-    """ Yet another requests.should_bypass_proxies
-    Test if proxies should not be used for a particular url.
-    """
-
-    parsed = urlparse(url)
-
-    # special cases
-    if parsed.hostname in [None, '']:
-        return True
-
-    # special cases
-    if no_proxy in [None, '']:
-        return False
-    if no_proxy == '*':
-        return True
-
-    no_proxy = no_proxy.lower().replace(' ', '');
-    entries = (
-        host for host in no_proxy.split(',') if host
-    )
-
-    if is_ipv4(parsed.hostname):
-        for item in entries:
-            if in_ipv4net(parsed.hostname, item):
-                return True
-    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
```

### Comparing `klaviyo-api-4.0.0/src/openapi_client/api/data_privacy_api.py` & `klaviyo-api-5.0.0/src/openapi_client/api/data_privacy_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,175 +1,189 @@
+# coding: utf-8
+
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
     The version of the OpenAPI document: 2023-07-15
     Contact: developers@klaviyo.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
-import sys  # noqa: F401
+import io
+import warnings
+
+from pydantic import validate_arguments, ValidationError
+from typing_extensions import Annotated
+
+from enum import EnumMeta
+
+from openapi_client.models.data_privacy_create_deletion_job_query import DataPrivacyCreateDeletionJobQuery
 
-from openapi_client.api_client import ApiClient, Endpoint as _Endpoint
-from openapi_client.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
+from openapi_client.api_client import ApiClient
+from openapi_client.api_response import ApiResponse
+from openapi_client.exceptions import (  # noqa: F401
+    ApiTypeError,
+    ApiValueError
 )
-from openapi_client.model.data_privacy_create_deletion_job_query import DataPrivacyCreateDeletionJobQuery
-from openapi_client.model.get_create_variants_jobs5_xx_response import GetCreateVariantsJobs5XXResponse
 
 
 class DataPrivacyApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
-            api_client = ApiClient()
+            api_client = ApiClient.get_default()
         self.api_client = api_client
-        self.request_profile_deletion_endpoint = _Endpoint(
-            settings={
-                'response_type': None,
-                'auth': [
-                    'Klaviyo-API-Key'
-                ],
-                'endpoint_path': '/api/data-privacy-deletion-jobs/',
-                'operation_id': 'request_profile_deletion',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'data_privacy_create_deletion_job_query',
-                ],
-                'required': [
-                    'data_privacy_create_deletion_job_query',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'data_privacy_create_deletion_job_query':
-                        (DataPrivacyCreateDeletionJobQuery,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'data_privacy_create_deletion_job_query': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
 
-    def request_profile_deletion(
-        self,
-        data_privacy_create_deletion_job_query,
-        **kwargs
-    ):
+    @validate_arguments
+    def request_profile_deletion(self, data_privacy_create_deletion_job_query : DataPrivacyCreateDeletionJobQuery, **kwargs) -> None:  # noqa: E501
         """Request Profile Deletion  # noqa: E501
 
         Request a deletion for the profiles corresponding to one of the following identifiers: `email`, `phone_number`, or `id`. If multiple identifiers are provided, we will return an error. All profiles that match the provided identifier will be deleted.         The deletion occurs asynchronously; however, once it has completed, the deleted profile will appear on the [Deleted Profiles page](https://www.klaviyo.com/account/deleted).         For more information on the deletion process, please refer to our [Help Center docs on how to handle GDPR and CCPA deletion requests](https://help.klaviyo.com/hc/en-us/articles/360004217631-How-to-Handle-GDPR-Requests#record-gdpr-and-ccpa%20%20-deletion-requests2).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `data-privacy:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.request_profile_deletion(data_privacy_create_deletion_job_query, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            data_privacy_create_deletion_job_query (DataPrivacyCreateDeletionJobQuery):
+        :param data_privacy_create_deletion_job_query: (required)
+        :type data_privacy_create_deletion_job_query: DataPrivacyCreateDeletionJobQuery
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the request_profile_deletion_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.request_profile_deletion_with_http_info(data_privacy_create_deletion_job_query, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def request_profile_deletion_with_http_info(self, data_privacy_create_deletion_job_query : DataPrivacyCreateDeletionJobQuery, **kwargs) -> ApiResponse:  # noqa: E501
+        """Request Profile Deletion  # noqa: E501
+
+        Request a deletion for the profiles corresponding to one of the following identifiers: `email`, `phone_number`, or `id`. If multiple identifiers are provided, we will return an error. All profiles that match the provided identifier will be deleted.         The deletion occurs asynchronously; however, once it has completed, the deleted profile will appear on the [Deleted Profiles page](https://www.klaviyo.com/account/deleted).         For more information on the deletion process, please refer to our [Help Center docs on how to handle GDPR and CCPA deletion requests](https://help.klaviyo.com/hc/en-us/articles/360004217631-How-to-Handle-GDPR-Requests#record-gdpr-and-ccpa%20%20-deletion-requests2).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `data-privacy:write`  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.request_profile_deletion_with_http_info(data_privacy_create_deletion_job_query, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            None
-                If the method is called asynchronously, returns the request
-                thread.
+        :param data_privacy_create_deletion_job_query: (required)
+        :type data_privacy_create_deletion_job_query: DataPrivacyCreateDeletionJobQuery
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['data_privacy_create_deletion_job_query'] = \
-            data_privacy_create_deletion_job_query
-        return self.request_profile_deletion_endpoint.call_with_http_info(**kwargs)
 
+        _params = locals()
+
+        _all_params = [
+            'data_privacy_create_deletion_job_query'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method request_profile_deletion" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['data_privacy_create_deletion_job_query'] is not None:
+            _body_params = _params['data_privacy_create_deletion_job_query']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['Klaviyo-API-Key']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/data-privacy-deletion-jobs/', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
```

### Comparing `klaviyo-api-4.0.0/src/openapi_client/exceptions.py` & `klaviyo-api-5.0.0/src/openapi_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+# coding: utf-8
+
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
     The version of the OpenAPI document: 2023-07-15
     Contact: developers@klaviyo.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
@@ -108,15 +112,15 @@
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "Status Code: {0}\n"\
+        error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
                 self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
```

### Comparing `klaviyo-api-4.0.0/src/openapi_client/models/__init__.py` & `klaviyo-api-5.0.0/src/openapi_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,275 +1,295 @@
+# coding: utf-8
+
 # flake8: noqa
 
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from from openapi_client.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
+"""
+    Klaviyo API
+
+    The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
+
+    The version of the OpenAPI document: 2023-07-15
+    Contact: developers@klaviyo.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""
+
+
+__version__ = "5.0.0"
+
+# import apis into sdk package
+from openapi_client.api.accounts_api import AccountsApi
+from openapi_client.api.campaigns_api import CampaignsApi
+from openapi_client.api.catalogs_api import CatalogsApi
+from openapi_client.api.data_privacy_api import DataPrivacyApi
+from openapi_client.api.events_api import EventsApi
+from openapi_client.api.flows_api import FlowsApi
+from openapi_client.api.lists_api import ListsApi
+from openapi_client.api.metrics_api import MetricsApi
+from openapi_client.api.profiles_api import ProfilesApi
+from openapi_client.api.segments_api import SegmentsApi
+from openapi_client.api.tags_api import TagsApi
+from openapi_client.api.templates_api import TemplatesApi
+
+# import ApiClient
+from openapi_client.api_response import ApiResponse
+from openapi_client.api_client import ApiClient
+from openapi_client.configuration import Configuration
+from openapi_client.exceptions import OpenApiException
+from openapi_client.exceptions import ApiTypeError
+from openapi_client.exceptions import ApiValueError
+from openapi_client.exceptions import ApiKeyError
+from openapi_client.exceptions import ApiAttributeError
+from openapi_client.exceptions import ApiException
 
-from openapi_client.model.audiences_sub_object import AudiencesSubObject
-from openapi_client.model.back_in_stock_subscription_enum import BackInStockSubscriptionEnum
-from openapi_client.model.campaign_clone_query import CampaignCloneQuery
-from openapi_client.model.campaign_clone_query_resource_object import CampaignCloneQueryResourceObject
-from openapi_client.model.campaign_clone_query_resource_object_attributes import CampaignCloneQueryResourceObjectAttributes
-from openapi_client.model.campaign_create_query import CampaignCreateQuery
-from openapi_client.model.campaign_create_query_resource_object import CampaignCreateQueryResourceObject
-from openapi_client.model.campaign_create_query_resource_object_attributes import CampaignCreateQueryResourceObjectAttributes
-from openapi_client.model.campaign_create_query_resource_object_attributes_campaign_messages import CampaignCreateQueryResourceObjectAttributesCampaignMessages
-from openapi_client.model.campaign_create_query_resource_object_attributes_send_options import CampaignCreateQueryResourceObjectAttributesSendOptions
-from openapi_client.model.campaign_create_query_resource_object_attributes_tracking_options import CampaignCreateQueryResourceObjectAttributesTrackingOptions
-from openapi_client.model.campaign_enum import CampaignEnum
-from openapi_client.model.campaign_message_assign_template_query import CampaignMessageAssignTemplateQuery
-from openapi_client.model.campaign_message_assign_template_query_resource_object import CampaignMessageAssignTemplateQueryResourceObject
-from openapi_client.model.campaign_message_assign_template_query_resource_object_attributes import CampaignMessageAssignTemplateQueryResourceObjectAttributes
-from openapi_client.model.campaign_message_assign_template_query_resource_object_relationships import CampaignMessageAssignTemplateQueryResourceObjectRelationships
-from openapi_client.model.campaign_message_assign_template_query_resource_object_relationships_template import CampaignMessageAssignTemplateQueryResourceObjectRelationshipsTemplate
-from openapi_client.model.campaign_message_assign_template_query_resource_object_relationships_template_data import CampaignMessageAssignTemplateQueryResourceObjectRelationshipsTemplateData
-from openapi_client.model.campaign_message_create_query_resource_object import CampaignMessageCreateQueryResourceObject
-from openapi_client.model.campaign_message_create_query_resource_object_attributes import CampaignMessageCreateQueryResourceObjectAttributes
-from openapi_client.model.campaign_message_create_query_resource_object_attributes_content import CampaignMessageCreateQueryResourceObjectAttributesContent
-from openapi_client.model.campaign_message_enum import CampaignMessageEnum
-from openapi_client.model.campaign_message_partial_update_query import CampaignMessagePartialUpdateQuery
-from openapi_client.model.campaign_message_partial_update_query_resource_object import CampaignMessagePartialUpdateQueryResourceObject
-from openapi_client.model.campaign_message_partial_update_query_resource_object_attributes import CampaignMessagePartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.campaign_partial_update_query import CampaignPartialUpdateQuery
-from openapi_client.model.campaign_partial_update_query_resource_object import CampaignPartialUpdateQueryResourceObject
-from openapi_client.model.campaign_partial_update_query_resource_object_attributes import CampaignPartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.campaign_recipient_estimation_job_create_query import CampaignRecipientEstimationJobCreateQuery
-from openapi_client.model.campaign_recipient_estimation_job_create_query_resource_object import CampaignRecipientEstimationJobCreateQueryResourceObject
-from openapi_client.model.campaign_recipient_estimation_job_create_query_resource_object_attributes import CampaignRecipientEstimationJobCreateQueryResourceObjectAttributes
-from openapi_client.model.campaign_recipient_estimation_job_enum import CampaignRecipientEstimationJobEnum
-from openapi_client.model.campaign_send_job_create_query import CampaignSendJobCreateQuery
-from openapi_client.model.campaign_send_job_create_query_resource_object import CampaignSendJobCreateQueryResourceObject
-from openapi_client.model.campaign_send_job_create_query_resource_object_attributes import CampaignSendJobCreateQueryResourceObjectAttributes
-from openapi_client.model.campaign_send_job_enum import CampaignSendJobEnum
-from openapi_client.model.campaign_send_job_partial_update_query import CampaignSendJobPartialUpdateQuery
-from openapi_client.model.campaign_send_job_partial_update_query_resource_object import CampaignSendJobPartialUpdateQueryResourceObject
-from openapi_client.model.campaign_send_job_partial_update_query_resource_object_attributes import CampaignSendJobPartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.catalog_category_bulk_create_job_enum import CatalogCategoryBulkCreateJobEnum
-from openapi_client.model.catalog_category_bulk_delete_job_enum import CatalogCategoryBulkDeleteJobEnum
-from openapi_client.model.catalog_category_bulk_update_job_enum import CatalogCategoryBulkUpdateJobEnum
-from openapi_client.model.catalog_category_create_job_create_query import CatalogCategoryCreateJobCreateQuery
-from openapi_client.model.catalog_category_create_job_create_query_resource_object import CatalogCategoryCreateJobCreateQueryResourceObject
-from openapi_client.model.catalog_category_create_job_create_query_resource_object_attributes import CatalogCategoryCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_category_create_job_create_query_resource_object_attributes_categories import CatalogCategoryCreateJobCreateQueryResourceObjectAttributesCategories
-from openapi_client.model.catalog_category_create_query import CatalogCategoryCreateQuery
-from openapi_client.model.catalog_category_create_query_resource_object import CatalogCategoryCreateQueryResourceObject
-from openapi_client.model.catalog_category_create_query_resource_object_attributes import CatalogCategoryCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_category_delete_job_create_query import CatalogCategoryDeleteJobCreateQuery
-from openapi_client.model.catalog_category_delete_job_create_query_resource_object import CatalogCategoryDeleteJobCreateQueryResourceObject
-from openapi_client.model.catalog_category_delete_job_create_query_resource_object_attributes import CatalogCategoryDeleteJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_category_delete_job_create_query_resource_object_attributes_categories import CatalogCategoryDeleteJobCreateQueryResourceObjectAttributesCategories
-from openapi_client.model.catalog_category_delete_query_resource_object import CatalogCategoryDeleteQueryResourceObject
-from openapi_client.model.catalog_category_enum import CatalogCategoryEnum
-from openapi_client.model.catalog_category_item_op import CatalogCategoryItemOp
-from openapi_client.model.catalog_category_update_job_create_query import CatalogCategoryUpdateJobCreateQuery
-from openapi_client.model.catalog_category_update_job_create_query_resource_object import CatalogCategoryUpdateJobCreateQueryResourceObject
-from openapi_client.model.catalog_category_update_job_create_query_resource_object_attributes import CatalogCategoryUpdateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_category_update_job_create_query_resource_object_attributes_categories import CatalogCategoryUpdateJobCreateQueryResourceObjectAttributesCategories
-from openapi_client.model.catalog_category_update_query import CatalogCategoryUpdateQuery
-from openapi_client.model.catalog_category_update_query_resource_object import CatalogCategoryUpdateQueryResourceObject
-from openapi_client.model.catalog_category_update_query_resource_object_attributes import CatalogCategoryUpdateQueryResourceObjectAttributes
-from openapi_client.model.catalog_category_update_query_resource_object_relationships import CatalogCategoryUpdateQueryResourceObjectRelationships
-from openapi_client.model.catalog_category_update_query_resource_object_relationships_items import CatalogCategoryUpdateQueryResourceObjectRelationshipsItems
-from openapi_client.model.catalog_category_update_query_resource_object_relationships_items_data_inner import CatalogCategoryUpdateQueryResourceObjectRelationshipsItemsDataInner
-from openapi_client.model.catalog_item_bulk_create_job_enum import CatalogItemBulkCreateJobEnum
-from openapi_client.model.catalog_item_bulk_delete_job_enum import CatalogItemBulkDeleteJobEnum
-from openapi_client.model.catalog_item_bulk_update_job_enum import CatalogItemBulkUpdateJobEnum
-from openapi_client.model.catalog_item_category_op import CatalogItemCategoryOp
-from openapi_client.model.catalog_item_category_op_data_inner import CatalogItemCategoryOpDataInner
-from openapi_client.model.catalog_item_create_job_create_query import CatalogItemCreateJobCreateQuery
-from openapi_client.model.catalog_item_create_job_create_query_resource_object import CatalogItemCreateJobCreateQueryResourceObject
-from openapi_client.model.catalog_item_create_job_create_query_resource_object_attributes import CatalogItemCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_item_create_job_create_query_resource_object_attributes_items import CatalogItemCreateJobCreateQueryResourceObjectAttributesItems
-from openapi_client.model.catalog_item_create_query import CatalogItemCreateQuery
-from openapi_client.model.catalog_item_create_query_resource_object import CatalogItemCreateQueryResourceObject
-from openapi_client.model.catalog_item_create_query_resource_object_attributes import CatalogItemCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_item_create_query_resource_object_relationships import CatalogItemCreateQueryResourceObjectRelationships
-from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories import CatalogItemCreateQueryResourceObjectRelationshipsCategories
-from openapi_client.model.catalog_item_delete_job_create_query import CatalogItemDeleteJobCreateQuery
-from openapi_client.model.catalog_item_delete_job_create_query_resource_object import CatalogItemDeleteJobCreateQueryResourceObject
-from openapi_client.model.catalog_item_delete_job_create_query_resource_object_attributes import CatalogItemDeleteJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_item_delete_job_create_query_resource_object_attributes_items import CatalogItemDeleteJobCreateQueryResourceObjectAttributesItems
-from openapi_client.model.catalog_item_delete_query_resource_object import CatalogItemDeleteQueryResourceObject
-from openapi_client.model.catalog_item_enum import CatalogItemEnum
-from openapi_client.model.catalog_item_update_job_create_query import CatalogItemUpdateJobCreateQuery
-from openapi_client.model.catalog_item_update_job_create_query_resource_object import CatalogItemUpdateJobCreateQueryResourceObject
-from openapi_client.model.catalog_item_update_job_create_query_resource_object_attributes import CatalogItemUpdateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_item_update_job_create_query_resource_object_attributes_items import CatalogItemUpdateJobCreateQueryResourceObjectAttributesItems
-from openapi_client.model.catalog_item_update_query import CatalogItemUpdateQuery
-from openapi_client.model.catalog_item_update_query_resource_object import CatalogItemUpdateQueryResourceObject
-from openapi_client.model.catalog_item_update_query_resource_object_attributes import CatalogItemUpdateQueryResourceObjectAttributes
-from openapi_client.model.catalog_variant_bulk_create_job_enum import CatalogVariantBulkCreateJobEnum
-from openapi_client.model.catalog_variant_bulk_delete_job_enum import CatalogVariantBulkDeleteJobEnum
-from openapi_client.model.catalog_variant_bulk_update_job_enum import CatalogVariantBulkUpdateJobEnum
-from openapi_client.model.catalog_variant_create_job_create_query import CatalogVariantCreateJobCreateQuery
-from openapi_client.model.catalog_variant_create_job_create_query_resource_object import CatalogVariantCreateJobCreateQueryResourceObject
-from openapi_client.model.catalog_variant_create_job_create_query_resource_object_attributes import CatalogVariantCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_variant_create_job_create_query_resource_object_attributes_variants import CatalogVariantCreateJobCreateQueryResourceObjectAttributesVariants
-from openapi_client.model.catalog_variant_create_query import CatalogVariantCreateQuery
-from openapi_client.model.catalog_variant_create_query_resource_object import CatalogVariantCreateQueryResourceObject
-from openapi_client.model.catalog_variant_create_query_resource_object_attributes import CatalogVariantCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_variant_create_query_resource_object_relationships import CatalogVariantCreateQueryResourceObjectRelationships
-from openapi_client.model.catalog_variant_create_query_resource_object_relationships_item import CatalogVariantCreateQueryResourceObjectRelationshipsItem
-from openapi_client.model.catalog_variant_delete_job_create_query import CatalogVariantDeleteJobCreateQuery
-from openapi_client.model.catalog_variant_delete_job_create_query_resource_object import CatalogVariantDeleteJobCreateQueryResourceObject
-from openapi_client.model.catalog_variant_delete_job_create_query_resource_object_attributes import CatalogVariantDeleteJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_variant_delete_job_create_query_resource_object_attributes_variants import CatalogVariantDeleteJobCreateQueryResourceObjectAttributesVariants
-from openapi_client.model.catalog_variant_delete_query_resource_object import CatalogVariantDeleteQueryResourceObject
-from openapi_client.model.catalog_variant_enum import CatalogVariantEnum
-from openapi_client.model.catalog_variant_update_job_create_query import CatalogVariantUpdateJobCreateQuery
-from openapi_client.model.catalog_variant_update_job_create_query_resource_object import CatalogVariantUpdateJobCreateQueryResourceObject
-from openapi_client.model.catalog_variant_update_job_create_query_resource_object_attributes import CatalogVariantUpdateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.catalog_variant_update_job_create_query_resource_object_attributes_variants import CatalogVariantUpdateJobCreateQueryResourceObjectAttributesVariants
-from openapi_client.model.catalog_variant_update_query import CatalogVariantUpdateQuery
-from openapi_client.model.catalog_variant_update_query_resource_object import CatalogVariantUpdateQueryResourceObject
-from openapi_client.model.catalog_variant_update_query_resource_object_attributes import CatalogVariantUpdateQueryResourceObjectAttributes
-from openapi_client.model.data_privacy_create_deletion_job_query import DataPrivacyCreateDeletionJobQuery
-from openapi_client.model.data_privacy_create_deletion_job_query_resource_object import DataPrivacyCreateDeletionJobQueryResourceObject
-from openapi_client.model.data_privacy_create_deletion_job_query_resource_object_attributes import DataPrivacyCreateDeletionJobQueryResourceObjectAttributes
-from openapi_client.model.data_privacy_create_deletion_job_query_resource_object_attributes_profile import DataPrivacyCreateDeletionJobQueryResourceObjectAttributesProfile
-from openapi_client.model.data_privacy_deletion_job_enum import DataPrivacyDeletionJobEnum
-from openapi_client.model.data_privacy_profile_query_resource_object import DataPrivacyProfileQueryResourceObject
-from openapi_client.model.data_privacy_profile_query_resource_object_attributes import DataPrivacyProfileQueryResourceObjectAttributes
-from openapi_client.model.email_content_sub_object import EmailContentSubObject
-from openapi_client.model.email_send_options_sub_object import EmailSendOptionsSubObject
-from openapi_client.model.email_tracking_options_sub_object import EmailTrackingOptionsSubObject
-from openapi_client.model.event_create_query_v2 import EventCreateQueryV2
-from openapi_client.model.event_create_query_v2_resource_object import EventCreateQueryV2ResourceObject
-from openapi_client.model.event_create_query_v2_resource_object_attributes import EventCreateQueryV2ResourceObjectAttributes
-from openapi_client.model.event_create_query_v2_resource_object_attributes_metric import EventCreateQueryV2ResourceObjectAttributesMetric
-from openapi_client.model.event_create_query_v2_resource_object_attributes_profile import EventCreateQueryV2ResourceObjectAttributesProfile
-from openapi_client.model.event_enum import EventEnum
-from openapi_client.model.flow_enum import FlowEnum
-from openapi_client.model.flow_update_query import FlowUpdateQuery
-from openapi_client.model.flow_update_query_resource_object import FlowUpdateQueryResourceObject
-from openapi_client.model.flow_update_query_resource_object_attributes import FlowUpdateQueryResourceObjectAttributes
-from openapi_client.model.get_create_variants_jobs5_xx_response import GetCreateVariantsJobs5XXResponse
-from openapi_client.model.get_create_variants_jobs5_xx_response_errors_inner import GetCreateVariantsJobs5XXResponseErrorsInner
-from openapi_client.model.get_create_variants_jobs5_xx_response_errors_inner_source import GetCreateVariantsJobs5XXResponseErrorsInnerSource
-from openapi_client.model.list_create_query import ListCreateQuery
-from openapi_client.model.list_create_query_resource_object import ListCreateQueryResourceObject
-from openapi_client.model.list_create_query_resource_object_attributes import ListCreateQueryResourceObjectAttributes
-from openapi_client.model.list_enum import ListEnum
-from openapi_client.model.list_members_add_query import ListMembersAddQuery
-from openapi_client.model.list_members_add_query_data_inner import ListMembersAddQueryDataInner
-from openapi_client.model.list_members_delete_query import ListMembersDeleteQuery
-from openapi_client.model.list_partial_update_query import ListPartialUpdateQuery
-from openapi_client.model.list_partial_update_query_resource_object import ListPartialUpdateQueryResourceObject
-from openapi_client.model.metric_aggregate_enum import MetricAggregateEnum
-from openapi_client.model.metric_aggregate_query import MetricAggregateQuery
-from openapi_client.model.metric_aggregate_query_resource_object import MetricAggregateQueryResourceObject
-from openapi_client.model.metric_aggregate_query_resource_object_attributes import MetricAggregateQueryResourceObjectAttributes
-from openapi_client.model.metric_create_query_resource_object import MetricCreateQueryResourceObject
-from openapi_client.model.metric_create_query_resource_object_attributes import MetricCreateQueryResourceObjectAttributes
-from openapi_client.model.metric_enum import MetricEnum
-from openapi_client.model.onsite_profile_create_query_resource_object import OnsiteProfileCreateQueryResourceObject
-from openapi_client.model.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
-from openapi_client.model.onsite_profile_meta import OnsiteProfileMeta
-from openapi_client.model.profile_create_query import ProfileCreateQuery
-from openapi_client.model.profile_create_query_resource_object import ProfileCreateQueryResourceObject
-from openapi_client.model.profile_create_query_resource_object_attributes import ProfileCreateQueryResourceObjectAttributes
-from openapi_client.model.profile_enum import ProfileEnum
-from openapi_client.model.profile_identifier_dto_resource_object import ProfileIdentifierDTOResourceObject
-from openapi_client.model.profile_identifier_dto_resource_object_attributes import ProfileIdentifierDTOResourceObjectAttributes
-from openapi_client.model.profile_location import ProfileLocation
-from openapi_client.model.profile_location_latitude import ProfileLocationLatitude
-from openapi_client.model.profile_location_longitude import ProfileLocationLongitude
-from openapi_client.model.profile_meta import ProfileMeta
-from openapi_client.model.profile_meta_patch_properties import ProfileMetaPatchProperties
-from openapi_client.model.profile_meta_patch_properties_unset import ProfileMetaPatchPropertiesUnset
-from openapi_client.model.profile_partial_update_query import ProfilePartialUpdateQuery
-from openapi_client.model.profile_partial_update_query_resource_object import ProfilePartialUpdateQueryResourceObject
-from openapi_client.model.profile_partial_update_query_resource_object_attributes import ProfilePartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.profile_subscription_bulk_create_job_enum import ProfileSubscriptionBulkCreateJobEnum
-from openapi_client.model.profile_subscription_bulk_delete_job_enum import ProfileSubscriptionBulkDeleteJobEnum
-from openapi_client.model.profile_subscription_create_query_resource_object import ProfileSubscriptionCreateQueryResourceObject
-from openapi_client.model.profile_subscription_create_query_resource_object_attributes import ProfileSubscriptionCreateQueryResourceObjectAttributes
-from openapi_client.model.profile_subscription_delete_query_resource_object import ProfileSubscriptionDeleteQueryResourceObject
-from openapi_client.model.profile_subscription_delete_query_resource_object_attributes import ProfileSubscriptionDeleteQueryResourceObjectAttributes
-from openapi_client.model.profile_suppression_bulk_create_job_enum import ProfileSuppressionBulkCreateJobEnum
-from openapi_client.model.profile_suppression_bulk_delete_job_enum import ProfileSuppressionBulkDeleteJobEnum
-from openapi_client.model.profile_suppression_create_query_resource_object import ProfileSuppressionCreateQueryResourceObject
-from openapi_client.model.profile_suppression_create_query_resource_object_attributes import ProfileSuppressionCreateQueryResourceObjectAttributes
-from openapi_client.model.profile_suppression_delete_query_resource_object import ProfileSuppressionDeleteQueryResourceObject
-from openapi_client.model.profile_suppression_delete_query_resource_object_attributes import ProfileSuppressionDeleteQueryResourceObjectAttributes
-from openapi_client.model.render_options_sub_object import RenderOptionsSubObject
-from openapi_client.model.sms_content_sub_object_create import SMSContentSubObjectCreate
-from openapi_client.model.sms_send_options_sub_object import SMSSendOptionsSubObject
-from openapi_client.model.sms_tracking_options_sub_object import SMSTrackingOptionsSubObject
-from openapi_client.model.sto_schedule_options import STOScheduleOptions
-from openapi_client.model.segment_enum import SegmentEnum
-from openapi_client.model.segment_partial_update_query import SegmentPartialUpdateQuery
-from openapi_client.model.segment_partial_update_query_resource_object import SegmentPartialUpdateQueryResourceObject
-from openapi_client.model.segment_partial_update_query_resource_object_attributes import SegmentPartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.send_strategy_sub_object import SendStrategySubObject
-from openapi_client.model.server_bis_subscription_create_query import ServerBISSubscriptionCreateQuery
-from openapi_client.model.server_bis_subscription_create_query_resource_object import ServerBISSubscriptionCreateQueryResourceObject
-from openapi_client.model.server_bis_subscription_create_query_resource_object_attributes import ServerBISSubscriptionCreateQueryResourceObjectAttributes
-from openapi_client.model.server_bis_subscription_create_query_resource_object_attributes_profile import ServerBISSubscriptionCreateQueryResourceObjectAttributesProfile
-from openapi_client.model.server_bis_subscription_create_query_resource_object_relationships import ServerBISSubscriptionCreateQueryResourceObjectRelationships
-from openapi_client.model.server_bis_subscription_create_query_resource_object_relationships_variant import ServerBISSubscriptionCreateQueryResourceObjectRelationshipsVariant
-from openapi_client.model.server_bis_subscription_create_query_resource_object_relationships_variant_data import ServerBISSubscriptionCreateQueryResourceObjectRelationshipsVariantData
-from openapi_client.model.static_schedule_options import StaticScheduleOptions
-from openapi_client.model.subscription_channels import SubscriptionChannels
-from openapi_client.model.subscription_create_job_create_query import SubscriptionCreateJobCreateQuery
-from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
-from openapi_client.model.subscription_create_job_create_query_resource_object_attributes import SubscriptionCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.subscription_create_job_create_query_resource_object_attributes_profiles import SubscriptionCreateJobCreateQueryResourceObjectAttributesProfiles
-from openapi_client.model.subscription_delete_job_create_query import SubscriptionDeleteJobCreateQuery
-from openapi_client.model.subscription_delete_job_create_query_resource_object import SubscriptionDeleteJobCreateQueryResourceObject
-from openapi_client.model.subscription_delete_job_create_query_resource_object_attributes import SubscriptionDeleteJobCreateQueryResourceObjectAttributes
-from openapi_client.model.subscription_delete_job_create_query_resource_object_attributes_profiles import SubscriptionDeleteJobCreateQueryResourceObjectAttributesProfiles
-from openapi_client.model.subscription_delete_job_create_query_resource_object_relationships import SubscriptionDeleteJobCreateQueryResourceObjectRelationships
-from openapi_client.model.subscription_delete_job_create_query_resource_object_relationships_list import SubscriptionDeleteJobCreateQueryResourceObjectRelationshipsList
-from openapi_client.model.subscription_delete_job_create_query_resource_object_relationships_list_data import SubscriptionDeleteJobCreateQueryResourceObjectRelationshipsListData
-from openapi_client.model.suppression_create_job_create_query import SuppressionCreateJobCreateQuery
-from openapi_client.model.suppression_create_job_create_query_resource_object import SuppressionCreateJobCreateQueryResourceObject
-from openapi_client.model.suppression_create_job_create_query_resource_object_attributes import SuppressionCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.suppression_create_job_create_query_resource_object_attributes_profiles import SuppressionCreateJobCreateQueryResourceObjectAttributesProfiles
-from openapi_client.model.suppression_delete_job_create_query import SuppressionDeleteJobCreateQuery
-from openapi_client.model.suppression_delete_job_create_query_resource_object import SuppressionDeleteJobCreateQueryResourceObject
-from openapi_client.model.suppression_delete_job_create_query_resource_object_attributes import SuppressionDeleteJobCreateQueryResourceObjectAttributes
-from openapi_client.model.suppression_delete_job_create_query_resource_object_attributes_profiles import SuppressionDeleteJobCreateQueryResourceObjectAttributesProfiles
-from openapi_client.model.tag_campaign_op import TagCampaignOp
-from openapi_client.model.tag_campaign_op_data_inner import TagCampaignOpDataInner
-from openapi_client.model.tag_create_query import TagCreateQuery
-from openapi_client.model.tag_create_query_resource_object import TagCreateQueryResourceObject
-from openapi_client.model.tag_create_query_resource_object_relationships import TagCreateQueryResourceObjectRelationships
-from openapi_client.model.tag_create_query_resource_object_relationships_tag_group import TagCreateQueryResourceObjectRelationshipsTagGroup
-from openapi_client.model.tag_create_query_resource_object_relationships_tag_group_data import TagCreateQueryResourceObjectRelationshipsTagGroupData
-from openapi_client.model.tag_enum import TagEnum
-from openapi_client.model.tag_flow_op import TagFlowOp
-from openapi_client.model.tag_flow_op_data_inner import TagFlowOpDataInner
-from openapi_client.model.tag_group_create_query import TagGroupCreateQuery
-from openapi_client.model.tag_group_create_query_resource_object import TagGroupCreateQueryResourceObject
-from openapi_client.model.tag_group_create_query_resource_object_attributes import TagGroupCreateQueryResourceObjectAttributes
-from openapi_client.model.tag_group_enum import TagGroupEnum
-from openapi_client.model.tag_group_update_query import TagGroupUpdateQuery
-from openapi_client.model.tag_group_update_query_resource_object import TagGroupUpdateQueryResourceObject
-from openapi_client.model.tag_group_update_query_resource_object_attributes import TagGroupUpdateQueryResourceObjectAttributes
-from openapi_client.model.tag_list_op import TagListOp
-from openapi_client.model.tag_list_op_data_inner import TagListOpDataInner
-from openapi_client.model.tag_segment_op import TagSegmentOp
-from openapi_client.model.tag_segment_op_data_inner import TagSegmentOpDataInner
-from openapi_client.model.tag_update_query import TagUpdateQuery
-from openapi_client.model.tag_update_query_resource_object import TagUpdateQueryResourceObject
-from openapi_client.model.tag_update_query_resource_object_attributes import TagUpdateQueryResourceObjectAttributes
-from openapi_client.model.template_clone_query import TemplateCloneQuery
-from openapi_client.model.template_clone_query_resource_object import TemplateCloneQueryResourceObject
-from openapi_client.model.template_clone_query_resource_object_attributes import TemplateCloneQueryResourceObjectAttributes
-from openapi_client.model.template_create_query import TemplateCreateQuery
-from openapi_client.model.template_create_query_resource_object import TemplateCreateQueryResourceObject
-from openapi_client.model.template_create_query_resource_object_attributes import TemplateCreateQueryResourceObjectAttributes
-from openapi_client.model.template_enum import TemplateEnum
-from openapi_client.model.template_render_query import TemplateRenderQuery
-from openapi_client.model.template_render_query_resource_object import TemplateRenderQueryResourceObject
-from openapi_client.model.template_render_query_resource_object_attributes import TemplateRenderQueryResourceObjectAttributes
-from openapi_client.model.template_update_query import TemplateUpdateQuery
-from openapi_client.model.template_update_query_resource_object import TemplateUpdateQueryResourceObject
-from openapi_client.model.template_update_query_resource_object_attributes import TemplateUpdateQueryResourceObjectAttributes
-from openapi_client.model.throttled_schedule_options import ThrottledScheduleOptions
-from openapi_client.model.utm_params_sub_object import UTMParamsSubObject
+# import models into sdk package
+from openapi_client.models.audiences_sub_object import AudiencesSubObject
+from openapi_client.models.back_in_stock_subscription_enum import BackInStockSubscriptionEnum
+from openapi_client.models.campaign_clone_query import CampaignCloneQuery
+from openapi_client.models.campaign_clone_query_resource_object import CampaignCloneQueryResourceObject
+from openapi_client.models.campaign_clone_query_resource_object_attributes import CampaignCloneQueryResourceObjectAttributes
+from openapi_client.models.campaign_create_query import CampaignCreateQuery
+from openapi_client.models.campaign_create_query_resource_object import CampaignCreateQueryResourceObject
+from openapi_client.models.campaign_create_query_resource_object_attributes import CampaignCreateQueryResourceObjectAttributes
+from openapi_client.models.campaign_create_query_resource_object_attributes_campaign_messages import CampaignCreateQueryResourceObjectAttributesCampaignMessages
+from openapi_client.models.campaign_enum import CampaignEnum
+from openapi_client.models.campaign_message_assign_template_query import CampaignMessageAssignTemplateQuery
+from openapi_client.models.campaign_message_assign_template_query_resource_object import CampaignMessageAssignTemplateQueryResourceObject
+from openapi_client.models.campaign_message_assign_template_query_resource_object_attributes import CampaignMessageAssignTemplateQueryResourceObjectAttributes
+from openapi_client.models.campaign_message_assign_template_query_resource_object_relationships import CampaignMessageAssignTemplateQueryResourceObjectRelationships
+from openapi_client.models.campaign_message_assign_template_query_resource_object_relationships_template import CampaignMessageAssignTemplateQueryResourceObjectRelationshipsTemplate
+from openapi_client.models.campaign_message_assign_template_query_resource_object_relationships_template_data import CampaignMessageAssignTemplateQueryResourceObjectRelationshipsTemplateData
+from openapi_client.models.campaign_message_create_query_resource_object import CampaignMessageCreateQueryResourceObject
+from openapi_client.models.campaign_message_create_query_resource_object_attributes import CampaignMessageCreateQueryResourceObjectAttributes
+from openapi_client.models.campaign_message_enum import CampaignMessageEnum
+from openapi_client.models.campaign_message_partial_update_query import CampaignMessagePartialUpdateQuery
+from openapi_client.models.campaign_message_partial_update_query_resource_object import CampaignMessagePartialUpdateQueryResourceObject
+from openapi_client.models.campaign_message_partial_update_query_resource_object_attributes import CampaignMessagePartialUpdateQueryResourceObjectAttributes
+from openapi_client.models.campaign_partial_update_query import CampaignPartialUpdateQuery
+from openapi_client.models.campaign_partial_update_query_resource_object import CampaignPartialUpdateQueryResourceObject
+from openapi_client.models.campaign_partial_update_query_resource_object_attributes import CampaignPartialUpdateQueryResourceObjectAttributes
+from openapi_client.models.campaign_recipient_estimation_job_create_query import CampaignRecipientEstimationJobCreateQuery
+from openapi_client.models.campaign_recipient_estimation_job_create_query_resource_object import CampaignRecipientEstimationJobCreateQueryResourceObject
+from openapi_client.models.campaign_recipient_estimation_job_create_query_resource_object_attributes import CampaignRecipientEstimationJobCreateQueryResourceObjectAttributes
+from openapi_client.models.campaign_recipient_estimation_job_enum import CampaignRecipientEstimationJobEnum
+from openapi_client.models.campaign_send_job_create_query import CampaignSendJobCreateQuery
+from openapi_client.models.campaign_send_job_create_query_resource_object import CampaignSendJobCreateQueryResourceObject
+from openapi_client.models.campaign_send_job_create_query_resource_object_attributes import CampaignSendJobCreateQueryResourceObjectAttributes
+from openapi_client.models.campaign_send_job_enum import CampaignSendJobEnum
+from openapi_client.models.campaign_send_job_partial_update_query import CampaignSendJobPartialUpdateQuery
+from openapi_client.models.campaign_send_job_partial_update_query_resource_object import CampaignSendJobPartialUpdateQueryResourceObject
+from openapi_client.models.campaign_send_job_partial_update_query_resource_object_attributes import CampaignSendJobPartialUpdateQueryResourceObjectAttributes
+from openapi_client.models.catalog_category_bulk_create_job_enum import CatalogCategoryBulkCreateJobEnum
+from openapi_client.models.catalog_category_bulk_delete_job_enum import CatalogCategoryBulkDeleteJobEnum
+from openapi_client.models.catalog_category_bulk_update_job_enum import CatalogCategoryBulkUpdateJobEnum
+from openapi_client.models.catalog_category_create_job_create_query import CatalogCategoryCreateJobCreateQuery
+from openapi_client.models.catalog_category_create_job_create_query_resource_object import CatalogCategoryCreateJobCreateQueryResourceObject
+from openapi_client.models.catalog_category_create_job_create_query_resource_object_attributes import CatalogCategoryCreateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_category_create_job_create_query_resource_object_attributes_categories import CatalogCategoryCreateJobCreateQueryResourceObjectAttributesCategories
+from openapi_client.models.catalog_category_create_query import CatalogCategoryCreateQuery
+from openapi_client.models.catalog_category_create_query_resource_object import CatalogCategoryCreateQueryResourceObject
+from openapi_client.models.catalog_category_create_query_resource_object_attributes import CatalogCategoryCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_category_create_query_resource_object_relationships import CatalogCategoryCreateQueryResourceObjectRelationships
+from openapi_client.models.catalog_category_create_query_resource_object_relationships_items import CatalogCategoryCreateQueryResourceObjectRelationshipsItems
+from openapi_client.models.catalog_category_delete_job_create_query import CatalogCategoryDeleteJobCreateQuery
+from openapi_client.models.catalog_category_delete_job_create_query_resource_object import CatalogCategoryDeleteJobCreateQueryResourceObject
+from openapi_client.models.catalog_category_delete_job_create_query_resource_object_attributes import CatalogCategoryDeleteJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_category_delete_job_create_query_resource_object_attributes_categories import CatalogCategoryDeleteJobCreateQueryResourceObjectAttributesCategories
+from openapi_client.models.catalog_category_delete_query_resource_object import CatalogCategoryDeleteQueryResourceObject
+from openapi_client.models.catalog_category_enum import CatalogCategoryEnum
+from openapi_client.models.catalog_category_item_op import CatalogCategoryItemOp
+from openapi_client.models.catalog_category_update_job_create_query import CatalogCategoryUpdateJobCreateQuery
+from openapi_client.models.catalog_category_update_job_create_query_resource_object import CatalogCategoryUpdateJobCreateQueryResourceObject
+from openapi_client.models.catalog_category_update_job_create_query_resource_object_attributes import CatalogCategoryUpdateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_category_update_job_create_query_resource_object_attributes_categories import CatalogCategoryUpdateJobCreateQueryResourceObjectAttributesCategories
+from openapi_client.models.catalog_category_update_query import CatalogCategoryUpdateQuery
+from openapi_client.models.catalog_category_update_query_resource_object import CatalogCategoryUpdateQueryResourceObject
+from openapi_client.models.catalog_category_update_query_resource_object_attributes import CatalogCategoryUpdateQueryResourceObjectAttributes
+from openapi_client.models.catalog_item_bulk_create_job_enum import CatalogItemBulkCreateJobEnum
+from openapi_client.models.catalog_item_bulk_delete_job_enum import CatalogItemBulkDeleteJobEnum
+from openapi_client.models.catalog_item_bulk_update_job_enum import CatalogItemBulkUpdateJobEnum
+from openapi_client.models.catalog_item_category_op import CatalogItemCategoryOp
+from openapi_client.models.catalog_item_create_job_create_query import CatalogItemCreateJobCreateQuery
+from openapi_client.models.catalog_item_create_job_create_query_resource_object import CatalogItemCreateJobCreateQueryResourceObject
+from openapi_client.models.catalog_item_create_job_create_query_resource_object_attributes import CatalogItemCreateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_item_create_job_create_query_resource_object_attributes_items import CatalogItemCreateJobCreateQueryResourceObjectAttributesItems
+from openapi_client.models.catalog_item_create_query import CatalogItemCreateQuery
+from openapi_client.models.catalog_item_create_query_resource_object import CatalogItemCreateQueryResourceObject
+from openapi_client.models.catalog_item_create_query_resource_object_attributes import CatalogItemCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_item_create_query_resource_object_relationships import CatalogItemCreateQueryResourceObjectRelationships
+from openapi_client.models.catalog_item_create_query_resource_object_relationships_categories import CatalogItemCreateQueryResourceObjectRelationshipsCategories
+from openapi_client.models.catalog_item_create_query_resource_object_relationships_categories_data_inner import CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner
+from openapi_client.models.catalog_item_delete_job_create_query import CatalogItemDeleteJobCreateQuery
+from openapi_client.models.catalog_item_delete_job_create_query_resource_object import CatalogItemDeleteJobCreateQueryResourceObject
+from openapi_client.models.catalog_item_delete_job_create_query_resource_object_attributes import CatalogItemDeleteJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_item_delete_job_create_query_resource_object_attributes_items import CatalogItemDeleteJobCreateQueryResourceObjectAttributesItems
+from openapi_client.models.catalog_item_delete_query_resource_object import CatalogItemDeleteQueryResourceObject
+from openapi_client.models.catalog_item_enum import CatalogItemEnum
+from openapi_client.models.catalog_item_update_job_create_query import CatalogItemUpdateJobCreateQuery
+from openapi_client.models.catalog_item_update_job_create_query_resource_object import CatalogItemUpdateJobCreateQueryResourceObject
+from openapi_client.models.catalog_item_update_job_create_query_resource_object_attributes import CatalogItemUpdateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_item_update_job_create_query_resource_object_attributes_items import CatalogItemUpdateJobCreateQueryResourceObjectAttributesItems
+from openapi_client.models.catalog_item_update_query import CatalogItemUpdateQuery
+from openapi_client.models.catalog_item_update_query_resource_object import CatalogItemUpdateQueryResourceObject
+from openapi_client.models.catalog_item_update_query_resource_object_attributes import CatalogItemUpdateQueryResourceObjectAttributes
+from openapi_client.models.catalog_variant_bulk_create_job_enum import CatalogVariantBulkCreateJobEnum
+from openapi_client.models.catalog_variant_bulk_delete_job_enum import CatalogVariantBulkDeleteJobEnum
+from openapi_client.models.catalog_variant_bulk_update_job_enum import CatalogVariantBulkUpdateJobEnum
+from openapi_client.models.catalog_variant_create_job_create_query import CatalogVariantCreateJobCreateQuery
+from openapi_client.models.catalog_variant_create_job_create_query_resource_object import CatalogVariantCreateJobCreateQueryResourceObject
+from openapi_client.models.catalog_variant_create_job_create_query_resource_object_attributes import CatalogVariantCreateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_variant_create_job_create_query_resource_object_attributes_variants import CatalogVariantCreateJobCreateQueryResourceObjectAttributesVariants
+from openapi_client.models.catalog_variant_create_query import CatalogVariantCreateQuery
+from openapi_client.models.catalog_variant_create_query_resource_object import CatalogVariantCreateQueryResourceObject
+from openapi_client.models.catalog_variant_create_query_resource_object_attributes import CatalogVariantCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_variant_create_query_resource_object_relationships import CatalogVariantCreateQueryResourceObjectRelationships
+from openapi_client.models.catalog_variant_create_query_resource_object_relationships_item import CatalogVariantCreateQueryResourceObjectRelationshipsItem
+from openapi_client.models.catalog_variant_create_query_resource_object_relationships_item_data import CatalogVariantCreateQueryResourceObjectRelationshipsItemData
+from openapi_client.models.catalog_variant_delete_job_create_query import CatalogVariantDeleteJobCreateQuery
+from openapi_client.models.catalog_variant_delete_job_create_query_resource_object import CatalogVariantDeleteJobCreateQueryResourceObject
+from openapi_client.models.catalog_variant_delete_job_create_query_resource_object_attributes import CatalogVariantDeleteJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_variant_delete_job_create_query_resource_object_attributes_variants import CatalogVariantDeleteJobCreateQueryResourceObjectAttributesVariants
+from openapi_client.models.catalog_variant_delete_query_resource_object import CatalogVariantDeleteQueryResourceObject
+from openapi_client.models.catalog_variant_enum import CatalogVariantEnum
+from openapi_client.models.catalog_variant_update_job_create_query import CatalogVariantUpdateJobCreateQuery
+from openapi_client.models.catalog_variant_update_job_create_query_resource_object import CatalogVariantUpdateJobCreateQueryResourceObject
+from openapi_client.models.catalog_variant_update_job_create_query_resource_object_attributes import CatalogVariantUpdateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.catalog_variant_update_job_create_query_resource_object_attributes_variants import CatalogVariantUpdateJobCreateQueryResourceObjectAttributesVariants
+from openapi_client.models.catalog_variant_update_query import CatalogVariantUpdateQuery
+from openapi_client.models.catalog_variant_update_query_resource_object import CatalogVariantUpdateQueryResourceObject
+from openapi_client.models.catalog_variant_update_query_resource_object_attributes import CatalogVariantUpdateQueryResourceObjectAttributes
+from openapi_client.models.data_privacy_create_deletion_job_query import DataPrivacyCreateDeletionJobQuery
+from openapi_client.models.data_privacy_create_deletion_job_query_resource_object import DataPrivacyCreateDeletionJobQueryResourceObject
+from openapi_client.models.data_privacy_create_deletion_job_query_resource_object_attributes import DataPrivacyCreateDeletionJobQueryResourceObjectAttributes
+from openapi_client.models.data_privacy_create_deletion_job_query_resource_object_attributes_profile import DataPrivacyCreateDeletionJobQueryResourceObjectAttributesProfile
+from openapi_client.models.data_privacy_deletion_job_enum import DataPrivacyDeletionJobEnum
+from openapi_client.models.data_privacy_profile_query_resource_object import DataPrivacyProfileQueryResourceObject
+from openapi_client.models.data_privacy_profile_query_resource_object_attributes import DataPrivacyProfileQueryResourceObjectAttributes
+from openapi_client.models.event_create_query_v2 import EventCreateQueryV2
+from openapi_client.models.event_create_query_v2_resource_object import EventCreateQueryV2ResourceObject
+from openapi_client.models.event_create_query_v2_resource_object_attributes import EventCreateQueryV2ResourceObjectAttributes
+from openapi_client.models.event_create_query_v2_resource_object_attributes_metric import EventCreateQueryV2ResourceObjectAttributesMetric
+from openapi_client.models.event_create_query_v2_resource_object_attributes_profile import EventCreateQueryV2ResourceObjectAttributesProfile
+from openapi_client.models.event_enum import EventEnum
+from openapi_client.models.flow_enum import FlowEnum
+from openapi_client.models.flow_update_query import FlowUpdateQuery
+from openapi_client.models.flow_update_query_resource_object import FlowUpdateQueryResourceObject
+from openapi_client.models.flow_update_query_resource_object_attributes import FlowUpdateQueryResourceObjectAttributes
+from openapi_client.models.get_accounts4_xx_response import GetAccounts4XXResponse
+from openapi_client.models.get_accounts4_xx_response_errors_inner import GetAccounts4XXResponseErrorsInner
+from openapi_client.models.get_accounts4_xx_response_errors_inner_source import GetAccounts4XXResponseErrorsInnerSource
+from openapi_client.models.list_create_query import ListCreateQuery
+from openapi_client.models.list_create_query_resource_object import ListCreateQueryResourceObject
+from openapi_client.models.list_create_query_resource_object_attributes import ListCreateQueryResourceObjectAttributes
+from openapi_client.models.list_enum import ListEnum
+from openapi_client.models.list_members_add_query import ListMembersAddQuery
+from openapi_client.models.list_members_add_query_data_inner import ListMembersAddQueryDataInner
+from openapi_client.models.list_members_delete_query import ListMembersDeleteQuery
+from openapi_client.models.list_partial_update_query import ListPartialUpdateQuery
+from openapi_client.models.list_partial_update_query_resource_object import ListPartialUpdateQueryResourceObject
+from openapi_client.models.metric_aggregate_enum import MetricAggregateEnum
+from openapi_client.models.metric_aggregate_query import MetricAggregateQuery
+from openapi_client.models.metric_aggregate_query_resource_object import MetricAggregateQueryResourceObject
+from openapi_client.models.metric_aggregate_query_resource_object_attributes import MetricAggregateQueryResourceObjectAttributes
+from openapi_client.models.metric_create_query_resource_object import MetricCreateQueryResourceObject
+from openapi_client.models.metric_create_query_resource_object_attributes import MetricCreateQueryResourceObjectAttributes
+from openapi_client.models.metric_enum import MetricEnum
+from openapi_client.models.onsite_profile_create_query_resource_object import OnsiteProfileCreateQueryResourceObject
+from openapi_client.models.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
+from openapi_client.models.onsite_profile_meta import OnsiteProfileMeta
+from openapi_client.models.profile_create_query import ProfileCreateQuery
+from openapi_client.models.profile_create_query_resource_object import ProfileCreateQueryResourceObject
+from openapi_client.models.profile_create_query_resource_object_attributes import ProfileCreateQueryResourceObjectAttributes
+from openapi_client.models.profile_enum import ProfileEnum
+from openapi_client.models.profile_identifier_dto_resource_object import ProfileIdentifierDTOResourceObject
+from openapi_client.models.profile_identifier_dto_resource_object_attributes import ProfileIdentifierDTOResourceObjectAttributes
+from openapi_client.models.profile_location import ProfileLocation
+from openapi_client.models.profile_meta import ProfileMeta
+from openapi_client.models.profile_meta_patch_properties import ProfileMetaPatchProperties
+from openapi_client.models.profile_partial_update_query import ProfilePartialUpdateQuery
+from openapi_client.models.profile_partial_update_query_resource_object import ProfilePartialUpdateQueryResourceObject
+from openapi_client.models.profile_subscription_bulk_create_job_enum import ProfileSubscriptionBulkCreateJobEnum
+from openapi_client.models.profile_subscription_bulk_delete_job_enum import ProfileSubscriptionBulkDeleteJobEnum
+from openapi_client.models.profile_subscription_create_query_resource_object import ProfileSubscriptionCreateQueryResourceObject
+from openapi_client.models.profile_subscription_create_query_resource_object_attributes import ProfileSubscriptionCreateQueryResourceObjectAttributes
+from openapi_client.models.profile_subscription_delete_query_resource_object import ProfileSubscriptionDeleteQueryResourceObject
+from openapi_client.models.profile_subscription_delete_query_resource_object_attributes import ProfileSubscriptionDeleteQueryResourceObjectAttributes
+from openapi_client.models.profile_suppression_bulk_create_job_enum import ProfileSuppressionBulkCreateJobEnum
+from openapi_client.models.profile_suppression_bulk_delete_job_enum import ProfileSuppressionBulkDeleteJobEnum
+from openapi_client.models.profile_suppression_create_query_resource_object import ProfileSuppressionCreateQueryResourceObject
+from openapi_client.models.profile_suppression_create_query_resource_object_attributes import ProfileSuppressionCreateQueryResourceObjectAttributes
+from openapi_client.models.profile_suppression_delete_query_resource_object import ProfileSuppressionDeleteQueryResourceObject
+from openapi_client.models.profile_suppression_delete_query_resource_object_attributes import ProfileSuppressionDeleteQueryResourceObjectAttributes
+from openapi_client.models.render_options_sub_object import RenderOptionsSubObject
+from openapi_client.models.sto_schedule_options import STOScheduleOptions
+from openapi_client.models.segment_enum import SegmentEnum
+from openapi_client.models.segment_partial_update_query import SegmentPartialUpdateQuery
+from openapi_client.models.segment_partial_update_query_resource_object import SegmentPartialUpdateQueryResourceObject
+from openapi_client.models.segment_partial_update_query_resource_object_attributes import SegmentPartialUpdateQueryResourceObjectAttributes
+from openapi_client.models.send_strategy_sub_object import SendStrategySubObject
+from openapi_client.models.server_bis_subscription_create_query import ServerBISSubscriptionCreateQuery
+from openapi_client.models.server_bis_subscription_create_query_resource_object import ServerBISSubscriptionCreateQueryResourceObject
+from openapi_client.models.server_bis_subscription_create_query_resource_object_attributes import ServerBISSubscriptionCreateQueryResourceObjectAttributes
+from openapi_client.models.server_bis_subscription_create_query_resource_object_attributes_profile import ServerBISSubscriptionCreateQueryResourceObjectAttributesProfile
+from openapi_client.models.server_bis_subscription_create_query_resource_object_relationships import ServerBISSubscriptionCreateQueryResourceObjectRelationships
+from openapi_client.models.server_bis_subscription_create_query_resource_object_relationships_variant import ServerBISSubscriptionCreateQueryResourceObjectRelationshipsVariant
+from openapi_client.models.server_bis_subscription_create_query_resource_object_relationships_variant_data import ServerBISSubscriptionCreateQueryResourceObjectRelationshipsVariantData
+from openapi_client.models.static_schedule_options import StaticScheduleOptions
+from openapi_client.models.subscription_channels import SubscriptionChannels
+from openapi_client.models.subscription_create_job_create_query import SubscriptionCreateJobCreateQuery
+from openapi_client.models.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
+from openapi_client.models.subscription_create_job_create_query_resource_object_attributes import SubscriptionCreateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.subscription_create_job_create_query_resource_object_attributes_profiles import SubscriptionCreateJobCreateQueryResourceObjectAttributesProfiles
+from openapi_client.models.subscription_create_job_create_query_resource_object_relationships import SubscriptionCreateJobCreateQueryResourceObjectRelationships
+from openapi_client.models.subscription_create_job_create_query_resource_object_relationships_list import SubscriptionCreateJobCreateQueryResourceObjectRelationshipsList
+from openapi_client.models.subscription_create_job_create_query_resource_object_relationships_list_data import SubscriptionCreateJobCreateQueryResourceObjectRelationshipsListData
+from openapi_client.models.subscription_delete_job_create_query import SubscriptionDeleteJobCreateQuery
+from openapi_client.models.subscription_delete_job_create_query_resource_object import SubscriptionDeleteJobCreateQueryResourceObject
+from openapi_client.models.subscription_delete_job_create_query_resource_object_attributes import SubscriptionDeleteJobCreateQueryResourceObjectAttributes
+from openapi_client.models.subscription_delete_job_create_query_resource_object_attributes_profiles import SubscriptionDeleteJobCreateQueryResourceObjectAttributesProfiles
+from openapi_client.models.suppression_create_job_create_query import SuppressionCreateJobCreateQuery
+from openapi_client.models.suppression_create_job_create_query_resource_object import SuppressionCreateJobCreateQueryResourceObject
+from openapi_client.models.suppression_create_job_create_query_resource_object_attributes import SuppressionCreateJobCreateQueryResourceObjectAttributes
+from openapi_client.models.suppression_create_job_create_query_resource_object_attributes_profiles import SuppressionCreateJobCreateQueryResourceObjectAttributesProfiles
+from openapi_client.models.suppression_delete_job_create_query import SuppressionDeleteJobCreateQuery
+from openapi_client.models.suppression_delete_job_create_query_resource_object import SuppressionDeleteJobCreateQueryResourceObject
+from openapi_client.models.suppression_delete_job_create_query_resource_object_attributes import SuppressionDeleteJobCreateQueryResourceObjectAttributes
+from openapi_client.models.suppression_delete_job_create_query_resource_object_attributes_profiles import SuppressionDeleteJobCreateQueryResourceObjectAttributesProfiles
+from openapi_client.models.tag_campaign_op import TagCampaignOp
+from openapi_client.models.tag_campaign_op_data_inner import TagCampaignOpDataInner
+from openapi_client.models.tag_create_query import TagCreateQuery
+from openapi_client.models.tag_create_query_resource_object import TagCreateQueryResourceObject
+from openapi_client.models.tag_create_query_resource_object_attributes import TagCreateQueryResourceObjectAttributes
+from openapi_client.models.tag_create_query_resource_object_relationships import TagCreateQueryResourceObjectRelationships
+from openapi_client.models.tag_create_query_resource_object_relationships_tag_group import TagCreateQueryResourceObjectRelationshipsTagGroup
+from openapi_client.models.tag_create_query_resource_object_relationships_tag_group_data import TagCreateQueryResourceObjectRelationshipsTagGroupData
+from openapi_client.models.tag_enum import TagEnum
+from openapi_client.models.tag_flow_op import TagFlowOp
+from openapi_client.models.tag_flow_op_data_inner import TagFlowOpDataInner
+from openapi_client.models.tag_group_create_query import TagGroupCreateQuery
+from openapi_client.models.tag_group_create_query_resource_object import TagGroupCreateQueryResourceObject
+from openapi_client.models.tag_group_create_query_resource_object_attributes import TagGroupCreateQueryResourceObjectAttributes
+from openapi_client.models.tag_group_enum import TagGroupEnum
+from openapi_client.models.tag_group_update_query import TagGroupUpdateQuery
+from openapi_client.models.tag_group_update_query_resource_object import TagGroupUpdateQueryResourceObject
+from openapi_client.models.tag_group_update_query_resource_object_attributes import TagGroupUpdateQueryResourceObjectAttributes
+from openapi_client.models.tag_list_op import TagListOp
+from openapi_client.models.tag_list_op_data_inner import TagListOpDataInner
+from openapi_client.models.tag_segment_op import TagSegmentOp
+from openapi_client.models.tag_segment_op_data_inner import TagSegmentOpDataInner
+from openapi_client.models.tag_update_query import TagUpdateQuery
+from openapi_client.models.tag_update_query_resource_object import TagUpdateQueryResourceObject
+from openapi_client.models.template_clone_query import TemplateCloneQuery
+from openapi_client.models.template_clone_query_resource_object import TemplateCloneQueryResourceObject
+from openapi_client.models.template_clone_query_resource_object_attributes import TemplateCloneQueryResourceObjectAttributes
+from openapi_client.models.template_create_query import TemplateCreateQuery
+from openapi_client.models.template_create_query_resource_object import TemplateCreateQueryResourceObject
+from openapi_client.models.template_create_query_resource_object_attributes import TemplateCreateQueryResourceObjectAttributes
+from openapi_client.models.template_enum import TemplateEnum
+from openapi_client.models.template_render_query import TemplateRenderQuery
+from openapi_client.models.template_render_query_resource_object import TemplateRenderQueryResourceObject
+from openapi_client.models.template_render_query_resource_object_attributes import TemplateRenderQueryResourceObjectAttributes
+from openapi_client.models.template_update_query import TemplateUpdateQuery
+from openapi_client.models.template_update_query_resource_object import TemplateUpdateQueryResourceObject
+from openapi_client.models.template_update_query_resource_object_attributes import TemplateUpdateQueryResourceObjectAttributes
+from openapi_client.models.throttled_schedule_options import ThrottledScheduleOptions
```

### Comparing `klaviyo-api-4.0.0/src/klaviyo_api/wrapper.py` & `klaviyo-api-5.0.0/src/klaviyo_api/wrapper.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-4.0.0/LICENSE` & `klaviyo-api-5.0.0/LICENSE`

 * *Files identical despite different names*

