# Comparing `tmp/lightdash_client_python-0.651.2.tar.gz` & `tmp/lightdash_client_python-0.692.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.651.2.tar", last modified: Tue Jul 11 01:36:57 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.692.1.tar", last modified: Mon Jul 31 06:06:31 2023, max compression
```

## Comparing `lightdash_client_python-0.651.2.tar` & `lightdash_client_python-0.692.1.tar`

### file list

```diff
@@ -1,1199 +1,1267 @@
--rw-r--r--   0        0        0     1040 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/.openapi-generator-ignore
--rw-r--r--   0        0        0        8 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/.python-version
--rw-r--r--   0        0        0    11357 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/LICENSE
--rw-r--r--   0        0        0     3258 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/README.md
--rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/charts/__init__.py
--rw-r--r--   0        0        0     4749 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/charts/post_chart_results.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/content/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/content/get_pinned_items.py
--rw-r--r--   0        0        0     5871 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/content/update_pinned_items_order.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exploring/__init__.py
--rw-r--r--   0        0        0     5223 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_query.py
--rw-r--r--   0        0        0     5659 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_underlying_data_query.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exports/__init__.py
--rw-r--r--   0        0        0     3852 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exports/get_csv_url.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/__init__.py
--rw-r--r--   0        0        0     4545 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4511 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4956 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     3655 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_slack_channels.py
--rw-r--r--   0        0        0     4543 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/__init__.py
--rw-r--r--   0        0        0     4215 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/create_email_one_time_passcode.py
--rw-r--r--   0        0        0     3518 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/delete_me.py
--rw-r--r--   0        0        0     4750 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/get_email_verification_status.py
--rw-r--r--   0        0        0     4914 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/join_organization.py
--rw-r--r--   0        0        0     4375 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/list_my_available_organizations.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/__init__.py
--rw-r--r--   0        0        0     4823 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_group_in_organization.py
--rw-r--r--   0        0        0     5097 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_organization.py
--rw-r--r--   0        0        0     4439 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_my_organization.py
--rw-r--r--   0        0        0     4292 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_organization_member.py
--rw-r--r--   0        0        0     3725 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/get_my_organization.py
--rw-r--r--   0        0        0     3909 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_groups_in_organization.py
--rw-r--r--   0        0        0     4022 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_email_domains.py
--rw-r--r--   0        0        0     3898 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_members.py
--rw-r--r--   0        0        0     3902 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_projects.py
--rw-r--r--   0        0        0     4654 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_my_organization.py
--rw-r--r--   0        0        0     5049 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_organization_email_domains.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/__init__.py
--rw-r--r--   0        0        0     4743 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/delete_validation_dismiss.py
--rw-r--r--   0        0        0     5908 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/get_latest_validation_results.py
--rw-r--r--   0        0        0     4077 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/get_project.py
--rw-r--r--   0        0        0     4191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/list_charts_in_project.py
--rw-r--r--   0        0        0     4191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/list_spaces_in_project.py
--rw-r--r--   0        0        0     6431 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/validate_project.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/__init__.py
--rw-r--r--   0        0        0     5295 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/add_space_share_to_user.py
--rw-r--r--   0        0        0     4946 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/create_space_in_project.py
--rw-r--r--   0        0        0     4941 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/get_project_access_list.py
--rw-r--r--   0        0        0     5041 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
--rw-r--r--   0        0        0     4688 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
--rw-r--r--   0        0        0     5031 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
--rw-r--r--   0        0        0     5256 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_organization_member.py
--rw-r--r--   0        0        0     5467 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py
--rw-r--r--   0        0        0     5071 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_space.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/__init__.py
--rw-r--r--   0        0        0     4140 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/delete_scheduler.py
--rw-r--r--   0        0        0     4151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduled_jobs.py
--rw-r--r--   0        0        0     4081 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler.py
--rw-r--r--   0        0        0     4332 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_job_status.py
--rw-r--r--   0        0        0     4111 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_logs.py
--rw-r--r--   0        0        0     4615 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/update_scheduler.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/share_links/__init__.py
--rw-r--r--   0        0        0     4687 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/share_links/create_share_url.py
--rw-r--r--   0        0        0     4004 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/share_links/get_share_url.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/spaces/__init__.py
--rw-r--r--   0        0        0     4485 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/spaces/delete_space.py
--rw-r--r--   0        0        0     4463 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/spaces/get_space.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/ssh_keypairs/__init__.py
--rw-r--r--   0        0        0     3585 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
--rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/__init__.py
--rw-r--r--   0        0        0     4462 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/add_user_to_group.py
--rw-r--r--   0        0        0     3983 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/delete_group.py
--rw-r--r--   0        0        0     3953 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group.py
--rw-r--r--   0        0        0     4077 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group_members.py
--rw-r--r--   0        0        0     4510 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/remove_user_from_group.py
--rw-r--r--   0        0        0     4885 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/update_group.py
--rw-r--r--   0        0        0     2888 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/errors.py
--rw-r--r--   0        0        0   177550 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     1415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share.py
--rw-r--r--   0        0        0     1497 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_json_body.py
--rw-r--r--   0        0        0     2003 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_response_200.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_response_200_status.py
--rw-r--r--   0        0        0     1949 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_user_to_group_response_200.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_user_to_group_response_200_status.py
--rw-r--r--   0        0        0     6478 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric.py
--rw-r--r--   0        0        0      241 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_compact_type_0.py
--rw-r--r--   0        0        0      281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_compact_type_1.py
--rw-r--r--   0        0        0     2365 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item.py
--rw-r--r--   0        0        0      650 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_operator.py
--rw-r--r--   0        0        0     1521 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_target.py
--rw-r--r--   0        0        0      393 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_type.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domain_projects_role_type_0.py
--rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domain_projects_role_type_1.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domain_projects_role_type_2.py
--rw-r--r--   0        0        0     4988 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains.py
--rw-r--r--   0        0        0     3595 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item.py
--rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item_role_type_0.py
--rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item_role_type_1.py
--rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item_role_type_2.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_0.py
--rw-r--r--   0        0        0      179 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_1.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_2.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_3.py
--rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response.py
--rw-r--r--   0        0        0     4038 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_results_item.py
--rw-r--r--   0        0        0      246 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_results_item_chart_type.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_status.py
--rw-r--r--   0        0        0     2016 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response.py
--rw-r--r--   0        0        0     1580 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response_results.py
--rw-r--r--   0        0        0      142 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response_status.py
--rw-r--r--   0        0        0     2776 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     1737 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings_results.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings_status.py
--rw-r--r--   0        0        0     2122 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     2325 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results.py
--rw-r--r--   0        0        0     2526 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py
--rw-r--r--   0        0        0      143 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_status.py
--rw-r--r--   0        0        0     2019 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
--rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
--rw-r--r--   0        0        0     2224 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response.py
--rw-r--r--   0        0        0     2709 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results.py
--rw-r--r--   0        0        0     2813 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results_otp.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_status.py
--rw-r--r--   0        0        0     2049 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload.py
--rw-r--r--   0        0        0     2277 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload_error.py
--rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload_status.py
--rw-r--r--   0        0        0     2429 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response.py
--rw-r--r--   0        0        0     2320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response_results_item.py
--rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response_status.py
--rw-r--r--   0        0        0     2480 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response.py
--rw-r--r--   0        0        0     2218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response_results_item.py
--rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response_status.py
--rw-r--r--   0        0        0     1993 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_response.py
--rw-r--r--   0        0        0     2274 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_response_results.py
--rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_response_status.py
--rw-r--r--   0        0        0     2160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response.py
--rw-r--r--   0        0        0     1476 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response_results.py
--rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response_status.py
--rw-r--r--   0        0        0     2067 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response.py
--rw-r--r--   0        0        0     1463 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response_results.py
--rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response_status.py
--rw-r--r--   0        0        0     2003 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization.py
--rw-r--r--   0        0        0     2362 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains.py
--rw-r--r--   0        0        0     5921 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results.py
--rw-r--r--   0        0        0     4175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py
--rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_0.py
--rw-r--r--   0        0        0      213 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_1.py
--rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_2.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_0.py
--rw-r--r--   0        0        0      201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_1.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_2.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_3.py
--rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_status.py
--rw-r--r--   0        0        0     2305 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile.py
--rw-r--r--   0        0        0     3624 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_results.py
--rw-r--r--   0        0        0      304 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_results_role.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_status.py
--rw-r--r--   0        0        0     2591 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles.py
--rw-r--r--   0        0        0     3678 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_results_item.py
--rw-r--r--   0        0        0      309 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_results_item_role.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_status.py
--rw-r--r--   0        0        0     2519 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects.py
--rw-r--r--   0        0        0     2151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_results_item.py
--rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_results_item_type.py
--rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_status.py
--rw-r--r--   0        0        0     3203 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_results.py
--rw-r--r--   0        0        0      140 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_status.py
--rw-r--r--   0        0        0     4640 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items.py
--rw-r--r--   0        0        0     2288 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0.py
--rw-r--r--   0        0        0     7025 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data.py
--rw-r--r--   0        0        0     1271 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_type.py
--rw-r--r--   0        0        0     2288 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1.py
--rw-r--r--   0        0        0     7876 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data.py
--rw-r--r--   0        0        0      366 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1271 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_type.py
--rw-r--r--   0        0        0     2225 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2.py
--rw-r--r--   0        0        0     3849 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2_data.py
--rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2_type.py
--rw-r--r--   0        0        0      139 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_status.py
--rw-r--r--   0        0        0     2580 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response.py
--rw-r--r--   0        0        0     2719 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_results_item.py
--rw-r--r--   0        0        0      286 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_results_item_role.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_status.py
--rw-r--r--   0        0        0     2027 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response.py
--rw-r--r--   0        0        0    20745 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results.py
--rw-r--r--   0        0        0     3377 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py
--rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py
--rw-r--r--   0        0        0      168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0_type.py
--rw-r--r--   0        0        0     2541 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py
--rw-r--r--   0        0        0      188 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_1_type.py
--rw-r--r--   0        0        0     4004 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py
--rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py
--rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2_type.py
--rw-r--r--   0        0        0     4186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py
--rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py
--rw-r--r--   0        0        0      180 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3_type.py
--rw-r--r--   0        0        0     4004 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py
--rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py
--rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4_type.py
--rw-r--r--   0        0        0     4097 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py
--rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py
--rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5_type.py
--rw-r--r--   0        0        0     3152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py
--rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6_type.py
--rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_type.py
--rw-r--r--   0        0        0     5577 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py
--rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py
--rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_type.py
--rw-r--r--   0        0        0     6883 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py
--rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_type.py
--rw-r--r--   0        0        0     7128 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py
--rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_type.py
--rw-r--r--   0        0        0     6150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py
--rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_priority.py
--rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_type.py
--rw-r--r--   0        0        0     4260 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py
--rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py
--rw-r--r--   0        0        0      188 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_type.py
--rw-r--r--   0        0        0     4197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py
--rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py
--rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_type.py
--rw-r--r--   0        0        0      143 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_status.py
--rw-r--r--   0        0        0     2050 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response.py
--rw-r--r--   0        0        0     2119 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results.py
--rw-r--r--   0        0        0     6314 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query.py
--rw-r--r--   0        0        0     8094 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      283 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      323 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3077 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      692 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1779 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      435 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     8170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters.py
--rw-r--r--   0        0        0     1767 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1777 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1752 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1762 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1792 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5063 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      284 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      342 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      269 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_status.py
--rw-r--r--   0        0        0     2497 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response.py
--rw-r--r--   0        0        0     1711 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response_results_item.py
--rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response_status.py
--rw-r--r--   0        0        0     2294 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response.py
--rw-r--r--   0        0        0     4066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results.py
--rw-r--r--   0        0        0     2779 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py
--rw-r--r--   0        0        0     2799 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_status.py
--rw-r--r--   0        0        0     2177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response.py
--rw-r--r--   0        0        0     5791 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results.py
--rw-r--r--   0        0        0     1777 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py
--rw-r--r--   0        0        0     1779 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py
--rw-r--r--   0        0        0     5858 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py
--rw-r--r--   0        0        0     1392 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py
--rw-r--r--   0        0        0      250 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_status.py
--rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_target_type.py
--rw-r--r--   0        0        0      470 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_task.py
--rw-r--r--   0        0        0     4266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py
--rw-r--r--   0        0        0     2822 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py
--rw-r--r--   0        0        0     2842 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py
--rw-r--r--   0        0        0     1952 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_users_item.py
--rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_status.py
--rw-r--r--   0        0        0     2148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_share_response.py
--rw-r--r--   0        0        0     3477 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_share_response_results.py
--rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_share_response_status.py
--rw-r--r--   0        0        0     2497 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response.py
--rw-r--r--   0        0        0     1608 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response_results_item.py
--rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response_status.py
--rw-r--r--   0        0        0     1993 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response.py
--rw-r--r--   0        0        0     5415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results.py
--rw-r--r--   0        0        0     2283 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_access_item.py
--rw-r--r--   0        0        0      280 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_access_item_role.py
--rw-r--r--   0        0        0     7498 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item.py
--rw-r--r--   0        0        0     1279 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2216 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7797 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item.py
--rw-r--r--   0        0        0      366 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_status.py
--rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response.py
--rw-r--r--   0        0        0     2535 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response_results_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response_status.py
--rw-r--r--   0        0        0     2178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response.py
--rw-r--r--   0        0        0     1572 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response_results.py
--rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response_status.py
--rw-r--r--   0        0        0     1828 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_success_empty.py
--rw-r--r--   0        0        0      140 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_success_empty_status.py
--rw-r--r--   0        0        0     2699 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response.py
--rw-r--r--   0        0        0     2048 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response_results_item.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response_status.py
--rw-r--r--   0        0        0     4920 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response.py
--rw-r--r--   0        0        0     6933 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0.py
--rw-r--r--   0        0        0      367 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0_chart_type.py
--rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0_error_type.py
--rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0_source.py
--rw-r--r--   0        0        0     6161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1.py
--rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1_error_type.py
--rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1_source.py
--rw-r--r--   0        0        0     4038 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2.py
--rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2_error_type.py
--rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2_source.py
--rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_status.py
--rw-r--r--   0        0        0     1674 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validation_dismiss_response.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validation_dismiss_response_status.py
--rw-r--r--   0        0        0     5370 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_priority.py
--rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_type.py
--rw-r--r--   0        0        0      332 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_kind.py
--rw-r--r--   0        0        0     4853 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_format.py
--rw-r--r--   0        0        0     2484 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_0.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_1.py
--rw-r--r--   0        0        0     3723 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_summary.py
--rw-r--r--   0        0        0      220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_summary_chart_type.py
--rw-r--r--   0        0        0      208 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_type.py
--rw-r--r--   0        0        0      220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/compact.py
--rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/compact_or_alias_type_0.py
--rw-r--r--   0        0        0      272 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/compact_or_alias_type_1.py
--rw-r--r--   0        0        0      634 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/conditional_operator.py
--rw-r--r--   0        0        0     2523 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200.py
--rw-r--r--   0        0        0     2919 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results.py
--rw-r--r--   0        0        0     2897 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_status.py
--rw-r--r--   0        0        0     1528 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_json_body.py
--rw-r--r--   0        0        0     2402 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200.py
--rw-r--r--   0        0        0     2383 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200_results.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200_status.py
--rw-r--r--   0        0        0     1481 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization.py
--rw-r--r--   0        0        0     1494 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization_json_body.py
--rw-r--r--   0        0        0     1981 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization_response_200.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization_response_200_status.py
--rw-r--r--   0        0        0     1896 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_project_member.py
--rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_project_member_role.py
--rw-r--r--   0        0        0     1624 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url.py
--rw-r--r--   0        0        0     1652 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_json_body.py
--rw-r--r--   0        0        0     2364 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201.py
--rw-r--r--   0        0        0     3528 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201_results.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201_status.py
--rw-r--r--   0        0        0     2601 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space.py
--rw-r--r--   0        0        0     2146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_access_item.py
--rw-r--r--   0        0        0      268 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_access_item_role.py
--rw-r--r--   0        0        0     2867 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body.py
--rw-r--r--   0        0        0     2341 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body_access_item.py
--rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body_access_item_role.py
--rw-r--r--   0        0        0     2317 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200.py
--rw-r--r--   0        0        0     5832 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results.py
--rw-r--r--   0        0        0     2445 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_access_item.py
--rw-r--r--   0        0        0      295 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_access_item_role.py
--rw-r--r--   0        0        0     7875 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     1345 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2300 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     8225 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py
--rw-r--r--   0        0        0      381 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1333 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_status.py
--rw-r--r--   0        0        0     2312 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201.py
--rw-r--r--   0        0        0     1605 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201_results.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201_status.py
--rw-r--r--   0        0        0     7127 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details.py
--rw-r--r--   0        0        0     1209 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_updated_by_user.py
--rw-r--r--   0        0        0     2127 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_validation_errors_item.py
--rw-r--r--   0        0        0     5078 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler.py
--rw-r--r--   0        0        0      165 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_format.py
--rw-r--r--   0        0        0     2536 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_0.py
--rw-r--r--   0        0        0      181 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_1.py
--rw-r--r--   0        0        0     3711 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials.py
--rw-r--r--   0        0        0     1261 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials_type.py
--rw-r--r--   0        0        0     3801 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config.py
--rw-r--r--   0        0        0     1669 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config_type.py
--rw-r--r--   0        0        0     3844 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config_type.py
--rw-r--r--   0        0        0     2352 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_ide_project_config.py
--rw-r--r--   0        0        0      169 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_ide_project_config_type.py
--rw-r--r--   0        0        0     1638 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_integration.py
--rw-r--r--   0        0        0     2397 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
--rw-r--r--   0        0        0     2556 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py
--rw-r--r--   0        0        0     2404 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metric.py
--rw-r--r--   0        0        0     3609 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config.py
--rw-r--r--   0        0        0     1638 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config_environment_item.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config_type.py
--rw-r--r--   0        0        0     3609 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config.py
--rw-r--r--   0        0        0     1638 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config_environment_item.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config_type.py
--rw-r--r--   0        0        0     2966 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config.py
--rw-r--r--   0        0        0     1633 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config_environment_item.py
--rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config_type.py
--rw-r--r--   0        0        0     2725 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config.py
--rw-r--r--   0        0        0     1628 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config_environment_item.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config_type.py
--rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_0_environment_item.py
--rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_0_type.py
--rw-r--r--   0        0        0     2325 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_1.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_1_type.py
--rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_2_environment_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_2_type.py
--rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_3_environment_item.py
--rw-r--r--   0        0        0      158 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_3_type.py
--rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_4_environment_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_4_type.py
--rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_5_environment_item.py
--rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_5_type.py
--rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_6_environment_item.py
--rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_6_type.py
--rw-r--r--   0        0        0     1592 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_environment_variable.py
--rw-r--r--   0        0        0      295 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type.py
--rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_azuredevops.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_bitbucket.py
--rw-r--r--   0        0        0      138 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_dbt.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_dbtcloudide.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_github.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_gitlab.py
--rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_none.py
--rw-r--r--   0        0        0     2143 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py
--rw-r--r--   0        0        0      169 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200_status.py
--rw-r--r--   0        0        0     1902 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_group_response_200.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_group_response_200_status.py
--rw-r--r--   0        0        0     1872 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_me_response_200.py
--rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_me_response_200_status.py
--rw-r--r--   0        0        0     2005 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_my_organization_response_200.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_my_organization_response_200_status.py
--rw-r--r--   0        0        0     2045 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_organization_member_response_200.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_organization_member_response_200_status.py
--rw-r--r--   0        0        0     1951 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_scheduler_response_201.py
--rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_scheduler_response_201_status.py
--rw-r--r--   0        0        0     1902 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_space_response_204.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_space_response_204_status.py
--rw-r--r--   0        0        0     1738 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_validation_dismiss_response_200.py
--rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_validation_dismiss_response_200_status.py
--rw-r--r--   0        0        0     1931 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password.py
--rw-r--r--   0        0        0     2677 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password_expiring.py
--rw-r--r--   0        0        0     2281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status.py
--rw-r--r--   0        0        0     2527 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring.py
--rw-r--r--   0        0        0     2757 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring_otp.py
--rw-r--r--   0        0        0     1898 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status_otp.py
--rw-r--r--   0        0        0     1574 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_0.py
--rw-r--r--   0        0        0     1584 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_1.py
--rw-r--r--   0        0        0     5812 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters.py
--rw-r--r--   0        0        0     1561 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1571 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1546 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_0.py
--rw-r--r--   0        0        0     1556 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_1.py
--rw-r--r--   0        0        0     2098 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200.py
--rw-r--r--   0        0        0     1598 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200_results.py
--rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200_status.py
--rw-r--r--   0        0        0     2986 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py
--rw-r--r--   0        0        0     1798 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_status.py
--rw-r--r--   0        0        0     2372 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200.py
--rw-r--r--   0        0        0     2467 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py
--rw-r--r--   0        0        0     2587 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_status.py
--rw-r--r--   0        0        0     2517 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200.py
--rw-r--r--   0        0        0     2914 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results.py
--rw-r--r--   0        0        0     2894 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results_otp.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_status.py
--rw-r--r--   0        0        0     2546 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200.py
--rw-r--r--   0        0        0     2236 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200_results_item.py
--rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200_status.py
--rw-r--r--   0        0        0     2050 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200.py
--rw-r--r--   0        0        0     2292 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200_results.py
--rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200_status.py
--rw-r--r--   0        0        0     5697 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200.py
--rw-r--r--   0        0        0     7347 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py
--rw-r--r--   0        0        0      385 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_chart_type.py
--rw-r--r--   0        0        0      303 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_error_type.py
--rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_source.py
--rw-r--r--   0        0        0     6464 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py
--rw-r--r--   0        0        0      303 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_error_type.py
--rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_source.py
--rw-r--r--   0        0        0     4341 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py
--rw-r--r--   0        0        0      303 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_error_type.py
--rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_source.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_status.py
--rw-r--r--   0        0        0     2293 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200.py
--rw-r--r--   0        0        0     3277 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200_results.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200_status.py
--rw-r--r--   0        0        0     5193 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200.py
--rw-r--r--   0        0        0     2499 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py
--rw-r--r--   0        0        0     7259 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py
--rw-r--r--   0        0        0     1319 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2268 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_type.py
--rw-r--r--   0        0        0     2499 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py
--rw-r--r--   0        0        0     8178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py
--rw-r--r--   0        0        0      377 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1319 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2268 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_type.py
--rw-r--r--   0        0        0     2424 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py
--rw-r--r--   0        0        0     3910 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_type.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_status.py
--rw-r--r--   0        0        0     2637 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200.py
--rw-r--r--   0        0        0     2753 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_results_item.py
--rw-r--r--   0        0        0      289 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_results_item_role.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_status.py
--rw-r--r--   0        0        0     2109 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200.py
--rw-r--r--   0        0        0    21254 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results.py
--rw-r--r--   0        0        0     3430 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py
--rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py
--rw-r--r--   0        0        0      171 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_type.py
--rw-r--r--   0        0        0     2571 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py
--rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1_type.py
--rw-r--r--   0        0        0     4057 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py
--rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_type.py
--rw-r--r--   0        0        0     4239 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py
--rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py
--rw-r--r--   0        0        0      183 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_type.py
--rw-r--r--   0        0        0     4057 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py
--rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_type.py
--rw-r--r--   0        0        0     4150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py
--rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py
--rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_type.py
--rw-r--r--   0        0        0     3205 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py
--rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py
--rw-r--r--   0        0        0      173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_type.py
--rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_type.py
--rw-r--r--   0        0        0     5637 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py
--rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py
--rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_type.py
--rw-r--r--   0        0        0     6943 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py
--rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py
--rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_type.py
--rw-r--r--   0        0        0     7188 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py
--rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py
--rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_type.py
--rw-r--r--   0        0        0     6229 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py
--rw-r--r--   0        0        0      217 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_priority.py
--rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py
--rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_type.py
--rw-r--r--   0        0        0     4320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py
--rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py
--rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_type.py
--rw-r--r--   0        0        0     4257 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py
--rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py
--rw-r--r--   0        0        0      181 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_type.py
--rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_status.py
--rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200.py
--rw-r--r--   0        0        0     1729 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200_status.py
--rw-r--r--   0        0        0     2334 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200.py
--rw-r--r--   0        0        0     1529 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200_results.py
--rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200_status.py
--rw-r--r--   0        0        0     2243 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200.py
--rw-r--r--   0        0        0     5924 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results.py
--rw-r--r--   0        0        0     1795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py
--rw-r--r--   0        0        0     1797 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     5953 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py
--rw-r--r--   0        0        0     1410 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py
--rw-r--r--   0        0        0      253 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_status.py
--rw-r--r--   0        0        0      197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_target_type.py
--rw-r--r--   0        0        0      473 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_task.py
--rw-r--r--   0        0        0     4392 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py
--rw-r--r--   0        0        0     2840 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py
--rw-r--r--   0        0        0     2860 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py
--rw-r--r--   0        0        0     1970 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_status.py
--rw-r--r--   0        0        0     2160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200.py
--rw-r--r--   0        0        0     3838 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results.py
--rw-r--r--   0        0        0     2741 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py
--rw-r--r--   0        0        0     2761 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py
--rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_status.py
--rw-r--r--   0        0        0     2304 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200.py
--rw-r--r--   0        0        0     3513 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200_results.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200_status.py
--rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200.py
--rw-r--r--   0        0        0     1626 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200_results_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200_status.py
--rw-r--r--   0        0        0     2050 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200.py
--rw-r--r--   0        0        0     5502 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results.py
--rw-r--r--   0        0        0     2317 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_access_item.py
--rw-r--r--   0        0        0      283 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_access_item_role.py
--rw-r--r--   0        0        0     7565 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     1293 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7883 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item.py
--rw-r--r--   0        0        0      369 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2219 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_status.py
--rw-r--r--   0        0        0     2051 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_json_body.py
--rw-r--r--   0        0        0      279 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_json_body_role.py
--rw-r--r--   0        0        0     2053 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_response_200.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_response_200_status.py
--rw-r--r--   0        0        0     2175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/group.py
--rw-r--r--   0        0        0     2091 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/group_member.py
--rw-r--r--   0        0        0     1961 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/join_organization_response_200.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/join_organization_response_200_status.py
--rw-r--r--   0        0        0     2620 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200.py
--rw-r--r--   0        0        0     4075 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_results_item.py
--rw-r--r--   0        0        0      249 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_results_item_chart_type.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_status.py
--rw-r--r--   0        0        0     2705 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200.py
--rw-r--r--   0        0        0     2401 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200_results_item.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200_status.py
--rw-r--r--   0        0        0     2773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200.py
--rw-r--r--   0        0        0     2071 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200_results_item.py
--rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200_status.py
--rw-r--r--   0        0        0     2453 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200.py
--rw-r--r--   0        0        0     6137 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results.py
--rw-r--r--   0        0        0     4306 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py
--rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_0.py
--rw-r--r--   0        0        0      218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_1.py
--rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_2.py
--rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_0.py
--rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_1.py
--rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_2.py
--rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_3.py
--rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_status.py
--rw-r--r--   0        0        0     2682 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200.py
--rw-r--r--   0        0        0     3732 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_results_item.py
--rw-r--r--   0        0        0      314 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_results_item_role.py
--rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_status.py
--rw-r--r--   0        0        0     2744 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200.py
--rw-r--r--   0        0        0     2279 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_results_item.py
--rw-r--r--   0        0        0      203 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_results_item_type.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_status.py
--rw-r--r--   0        0        0     2620 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200.py
--rw-r--r--   0        0        0     2553 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200_results_item.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200_status.py
--rw-r--r--   0        0        0     2133 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule.py
--rw-r--r--   0        0        0      639 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_operator.py
--rw-r--r--   0        0        0     1463 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_target.py
--rw-r--r--   0        0        0     5557 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response.py
--rw-r--r--   0        0        0     7432 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item.py
--rw-r--r--   0        0        0      265 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      305 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     2769 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      674 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1653 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      417 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_type.py
--rw-r--r--   0        0        0     7034 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters.py
--rw-r--r--   0        0        0     1665 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1675 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1650 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1660 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1690 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_sorts_item.py
--rw-r--r--   0        0        0     3183 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item.py
--rw-r--r--   0        0        0     4643 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format.py
--rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      324 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      383 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_type.py
--rw-r--r--   0        0        0      284 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/number_separator.py
--rw-r--r--   0        0        0     5630 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     4125 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py
--rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
--rw-r--r--   0        0        0      211 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
--rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
--rw-r--r--   0        0        0      175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_0.py
--rw-r--r--   0        0        0      199 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_1.py
--rw-r--r--   0        0        0      175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_2.py
--rw-r--r--   0        0        0      175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_3.py
--rw-r--r--   0        0        0     6420 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0      224 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
--rw-r--r--   0        0        0     1469 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     4520 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1479 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      200 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     7338 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1469 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     7093 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1469 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     5805 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1474 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     4353 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1454 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     3794 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name.py
--rw-r--r--   0        0        0      280 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name_error_type.py
--rw-r--r--   0        0        0      209 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name_source.py
--rw-r--r--   0        0        0     3147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization.py
--rw-r--r--   0        0        0     3507 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile.py
--rw-r--r--   0        0        0      294 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_role.py
--rw-r--r--   0        0        0     1674 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_update.py
--rw-r--r--   0        0        0      300 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_update_role.py
--rw-r--r--   0        0        0      287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_editor.py
--rw-r--r--   0        0        0      190 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_interactiveviewer.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_member.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_viewer.py
--rw-r--r--   0        0        0     1980 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_project.py
--rw-r--r--   0        0        0      176 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_project_type.py
--rw-r--r--   0        0        0     2713 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
--rw-r--r--   0        0        0     6971 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     5108 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py
--rw-r--r--   0        0        0      218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
--rw-r--r--   0        0        0      242 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
--rw-r--r--   0        0        0      218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
--rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_0.py
--rw-r--r--   0        0        0      230 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_1.py
--rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_2.py
--rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_3.py
--rw-r--r--   0        0        0     7661 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0      267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
--rw-r--r--   0        0        0     1728 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     5374 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1748 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      245 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     1769 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
--rw-r--r--   0        0        0     1493 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_group_name.py
--rw-r--r--   0        0        0     8285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1728 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     8036 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1728 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     6654 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1738 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      235 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     5124 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1693 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      219 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     9895 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py
--rw-r--r--   0        0        0     1834 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
--rw-r--r--   0        0        0     2946 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
--rw-r--r--   0        0        0     7951 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1840 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
--rw-r--r--   0        0        0     1460 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_group_name.py
--rw-r--r--   0        0        0     1494 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_organization_name.py
--rw-r--r--   0        0        0     1926 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     3654 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
--rw-r--r--   0        0        0     5491 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1610 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
--rw-r--r--   0        0        0     1685 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_share_url_path_or_params.py
--rw-r--r--   0        0        0     2537 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
--rw-r--r--   0        0        0     3330 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
--rw-r--r--   0        0        0    11635 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py
--rw-r--r--   0        0        0      496 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_chart_type.py
--rw-r--r--   0        0        0     1838 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
--rw-r--r--   0        0        0     2952 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
--rw-r--r--   0        0        0     1547 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_ssh_key_pair_public_key.py
--rw-r--r--   0        0        0     4356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
--rw-r--r--   0        0        0      314 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_error_type.py
--rw-r--r--   0        0        0      243 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_source.py
--rw-r--r--   0        0        0     2194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
--rw-r--r--   0        0        0     1227 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_type.py
--rw-r--r--   0        0        0      356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1227 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_type.py
--rw-r--r--   0        0        0     3793 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_2_data.py
--rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_2_type.py
--rw-r--r--   0        0        0     2212 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body.py
--rw-r--r--   0        0        0     7343 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters.py
--rw-r--r--   0        0        0     1696 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1706 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1681 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1691 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py
--rw-r--r--   0        0        0     2243 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200.py
--rw-r--r--   0        0        0     2220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results.py
--rw-r--r--   0        0        0     6589 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query.py
--rw-r--r--   0        0        0     8425 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      291 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      331 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3254 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      700 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1822 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      443 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     8643 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py
--rw-r--r--   0        0        0     1810 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1820 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1805 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1835 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3546 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5245 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      292 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      350 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      277 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_status.py
--rw-r--r--   0        0        0     5967 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body.py
--rw-r--r--   0        0        0     7477 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py
--rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      306 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     2795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      675 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1664 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      418 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_type.py
--rw-r--r--   0        0        0     1855 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_filters.py
--rw-r--r--   0        0        0     1701 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_sorts_item.py
--rw-r--r--   0        0        0     3206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item.py
--rw-r--r--   0        0        0     4677 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py
--rw-r--r--   0        0        0      267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      325 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      252 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_type.py
--rw-r--r--   0        0        0     2166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200.py
--rw-r--r--   0        0        0     2172 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results.py
--rw-r--r--   0        0        0     6457 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query.py
--rw-r--r--   0        0        0     8263 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      327 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      696 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1802 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      439 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     8417 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py
--rw-r--r--   0        0        0     1790 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1800 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1775 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1785 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1815 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3494 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      288 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      346 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_status.py
--rw-r--r--   0        0        0     6528 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body.py
--rw-r--r--   0        0        0     8001 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py
--rw-r--r--   0        0        0      280 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3029 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      689 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1740 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      432 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_type.py
--rw-r--r--   0        0        0     1931 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py
--rw-r--r--   0        0        0     1777 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py
--rw-r--r--   0        0        0     3398 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py
--rw-r--r--   0        0        0     4997 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py
--rw-r--r--   0        0        0      281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      339 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_type.py
--rw-r--r--   0        0        0     2425 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200.py
--rw-r--r--   0        0        0     2350 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results.py
--rw-r--r--   0        0        0     7047 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py
--rw-r--r--   0        0        0     8971 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      301 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      341 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3456 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      710 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1934 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      453 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     9367 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py
--rw-r--r--   0        0        0     1890 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1900 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1875 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1885 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1891 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3740 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5635 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      302 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      360 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_status.py
--rw-r--r--   0        0        0     6543 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials.py
--rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials_type.py
--rw-r--r--   0        0        0    17362 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project.py
--rw-r--r--   0        0        0     3035 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0_environment_item.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0_type.py
--rw-r--r--   0        0        0     2361 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_1.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_1_type.py
--rw-r--r--   0        0        0     3662 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2_environment_item.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2_type.py
--rw-r--r--   0        0        0     3844 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3_environment_item.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3_type.py
--rw-r--r--   0        0        0     3662 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4_environment_item.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4_type.py
--rw-r--r--   0        0        0     3755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5_environment_item.py
--rw-r--r--   0        0        0      168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5_type.py
--rw-r--r--   0        0        0     2810 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6.py
--rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6_environment_item.py
--rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6_type.py
--rw-r--r--   0        0        0     2504 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_profile.py
--rw-r--r--   0        0        0      267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_profile_role.py
--rw-r--r--   0        0        0      260 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role_editor.py
--rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role_interactiveviewer.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role_viewer.py
--rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_type.py
--rw-r--r--   0        0        0     5235 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0.py
--rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py
--rw-r--r--   0        0        0      168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0_type.py
--rw-r--r--   0        0        0     6541 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1.py
--rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1_type.py
--rw-r--r--   0        0        0     6786 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2.py
--rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2_type.py
--rw-r--r--   0        0        0     5697 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3.py
--rw-r--r--   0        0        0      196 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_priority.py
--rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_type.py
--rw-r--r--   0        0        0     3918 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4.py
--rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4_type.py
--rw-r--r--   0        0        0     3855 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5.py
--rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5_type.py
--rw-r--r--   0        0        0     1222 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/record_string_any.py
--rw-r--r--   0        0        0     6298 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials.py
--rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials_type.py
--rw-r--r--   0        0        0     1999 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/remove_user_from_group_response_200.py
--rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/remove_user_from_group_response_200_status.py
--rw-r--r--   0        0        0     2066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item.py
--rw-r--r--   0        0        0     7618 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data.py
--rw-r--r--   0        0        0      357 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_chart_type.py
--rw-r--r--   0        0        0     1229 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py
--rw-r--r--   0        0        0     2153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_type.py
--rw-r--r--   0        0        0     2159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item.py
--rw-r--r--   0        0        0     6904 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data.py
--rw-r--r--   0        0        0     1245 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py
--rw-r--r--   0        0        0     2173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_type.py
--rw-r--r--   0        0        0      193 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type_chart.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type_dashboard.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type_space.py
--rw-r--r--   0        0        0     2003 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item.py
--rw-r--r--   0        0        0     3795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item_data.py
--rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item_type.py
--rw-r--r--   0        0        0     2073 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_project_access_for_user_response_200.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_project_access_for_user_response_200_status.py
--rw-r--r--   0        0        0     2053 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_space_access_for_user_response_200.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_space_access_for_user_response_200_status.py
--rw-r--r--   0        0        0     5680 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request.py
--rw-r--r--   0        0        0     7266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item.py
--rw-r--r--   0        0        0      261 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      301 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     2705 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      670 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1633 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      413 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_type.py
--rw-r--r--   0        0        0     1824 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_filters.py
--rw-r--r--   0        0        0     1670 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_sorts_item.py
--rw-r--r--   0        0        0     3131 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item.py
--rw-r--r--   0        0        0     4555 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format.py
--rw-r--r--   0        0        0      262 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      247 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format_type.py
--rw-r--r--   0        0        0     1589 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduled_jobs.py
--rw-r--r--   0        0        0     3502 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets.py
--rw-r--r--   0        0        0     2680 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py
--rw-r--r--   0        0        0     2700 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py
--rw-r--r--   0        0        0     4849 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_format.py
--rw-r--r--   0        0        0     2471 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_0.py
--rw-r--r--   0        0        0      176 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1226 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_1.py
--rw-r--r--   0        0        0     2376 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_csv_options.py
--rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_csv_options_limit_type_1.py
--rw-r--r--   0        0        0     2613 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_email_target.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_format.py
--rw-r--r--   0        0        0     1200 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_image_options.py
--rw-r--r--   0        0        0      223 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_job_status.py
--rw-r--r--   0        0        0     4954 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log.py
--rw-r--r--   0        0        0     1242 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_details.py
--rw-r--r--   0        0        0      223 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_status.py
--rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_target_type.py
--rw-r--r--   0        0        0      443 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_task.py
--rw-r--r--   0        0        0     2415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_0.py
--rw-r--r--   0        0        0      172 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1203 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_1.py
--rw-r--r--   0        0        0     2593 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_slack_target.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_format.py
--rw-r--r--   0        0        0     2488 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_0.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_1.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_format.py
--rw-r--r--   0        0        0     2488 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_0.py
--rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_1.py
--rw-r--r--   0        0        0     5079 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs.py
--rw-r--r--   0        0        0     1701 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_charts_item.py
--rw-r--r--   0        0        0     1703 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_dashboards_item.py
--rw-r--r--   0        0        0     5415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item.py
--rw-r--r--   0        0        0     1316 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_details.py
--rw-r--r--   0        0        0      236 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_status.py
--rw-r--r--   0        0        0      180 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_target_type.py
--rw-r--r--   0        0        0      456 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_task.py
--rw-r--r--   0        0        0     3862 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item.py
--rw-r--r--   0        0        0     2746 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py
--rw-r--r--   0        0        0     2766 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py
--rw-r--r--   0        0        0     1876 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_users_item.py
--rw-r--r--   0        0        0     3396 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/share_url.py
--rw-r--r--   0        0        0     1481 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/slack_channel.py
--rw-r--r--   0        0        0     5010 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials.py
--rw-r--r--   0        0        0     1256 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials_start_of_week.py
--rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials_type.py
--rw-r--r--   0        0        0     1586 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/sort_field.py
--rw-r--r--   0        0        0     4794 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space.py
--rw-r--r--   0        0        0     2082 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_access_item.py
--rw-r--r--   0        0        0      262 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_access_item_role.py
--rw-r--r--   0        0        0     6938 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard.py
--rw-r--r--   0        0        0     1179 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_updated_by_user.py
--rw-r--r--   0        0        0     2089 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_validation_errors_item.py
--rw-r--r--   0        0        0     7087 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item.py
--rw-r--r--   0        0        0     1201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2117 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item.py
--rw-r--r--   0        0        0      348 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_chart_type.py
--rw-r--r--   0        0        0     1189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2102 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0     7060 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query.py
--rw-r--r--   0        0        0      342 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query_chart_type.py
--rw-r--r--   0        0        0     1163 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query_updated_by_user.py
--rw-r--r--   0        0        0     2069 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query_validation_errors_item.py
--rw-r--r--   0        0        0     2028 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_share.py
--rw-r--r--   0        0        0      257 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_share_role.py
--rw-r--r--   0        0        0     2390 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_summary.py
--rw-r--r--   0        0        0      242 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/table_calculation_format_compact.py
--rw-r--r--   0        0        0      300 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/table_calculation_format_separator.py
--rw-r--r--   0        0        0      227 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/table_calculation_format_type.py
--rw-r--r--   0        0        0     3516 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials.py
--rw-r--r--   0        0        0     1236 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials_start_of_week.py
--rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials_type.py
--rw-r--r--   0        0        0     5066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains.py
--rw-r--r--   0        0        0     3751 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item.py
--rw-r--r--   0        0        0      173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_0.py
--rw-r--r--   0        0        0      197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_1.py
--rw-r--r--   0        0        0      173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_2.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_0.py
--rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_1.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_2.py
--rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_3.py
--rw-r--r--   0        0        0     3040 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py
--rw-r--r--   0        0        0     1813 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py
--rw-r--r--   0        0        0      169 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_status.py
--rw-r--r--   0        0        0     1447 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group.py
--rw-r--r--   0        0        0     1493 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_json_body.py
--rw-r--r--   0        0        0     2126 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200.py
--rw-r--r--   0        0        0     2307 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200_results.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200_status.py
--rw-r--r--   0        0        0     2575 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_json_body.py
--rw-r--r--   0        0        0     2005 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_response_200.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_response_200_status.py
--rw-r--r--   0        0        0     2520 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization.py
--rw-r--r--   0        0        0     5551 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body.py
--rw-r--r--   0        0        0     4100 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py
--rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_0.py
--rw-r--r--   0        0        0      210 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_1.py
--rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_2.py
--rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_0.py
--rw-r--r--   0        0        0      198 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_1.py
--rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_2.py
--rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_3.py
--rw-r--r--   0        0        0     2487 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200.py
--rw-r--r--   0        0        0     6215 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results.py
--rw-r--r--   0        0        0     4356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py
--rw-r--r--   0        0        0      196 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_0.py
--rw-r--r--   0        0        0      220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_1.py
--rw-r--r--   0        0        0      196 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_2.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_0.py
--rw-r--r--   0        0        0      208 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_1.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_2.py
--rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_3.py
--rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_status.py
--rw-r--r--   0        0        0     1715 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_json_body.py
--rw-r--r--   0        0        0      301 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_json_body_role.py
--rw-r--r--   0        0        0     2430 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200.py
--rw-r--r--   0        0        0     3698 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_results.py
--rw-r--r--   0        0        0      311 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_results_role.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_status.py
--rw-r--r--   0        0        0     2066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order.py
--rw-r--r--   0        0        0     1798 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order_data.py
--rw-r--r--   0        0        0      198 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order_type.py
--rw-r--r--   0        0        0     2356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item.py
--rw-r--r--   0        0        0     1872 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item_data.py
--rw-r--r--   0        0        0      211 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item_type.py
--rw-r--r--   0        0        0     5525 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200.py
--rw-r--r--   0        0        0     2641 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py
--rw-r--r--   0        0        0     7522 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py
--rw-r--r--   0        0        0     1353 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2311 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_type.py
--rw-r--r--   0        0        0     2641 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py
--rw-r--r--   0        0        0     8490 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py
--rw-r--r--   0        0        0      385 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1353 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2311 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_type.py
--rw-r--r--   0        0        0     2566 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py
--rw-r--r--   0        0        0     3953 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py
--rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_type.py
--rw-r--r--   0        0        0      158 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_status.py
--rw-r--r--   0        0        0     1716 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_json_body.py
--rw-r--r--   0        0        0      281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_json_body_role.py
--rw-r--r--   0        0        0     2073 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_response_200.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_response_200_status.py
--rw-r--r--   0        0        0     1541 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_member.py
--rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_member_role.py
--rw-r--r--   0        0        0     2220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201.py
--rw-r--r--   0        0        0     3910 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results.py
--rw-r--r--   0        0        0     2756 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py
--rw-r--r--   0        0        0     2776 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py
--rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_status.py
--rw-r--r--   0        0        0     1556 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space.py
--rw-r--r--   0        0        0     1602 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_json_body.py
--rw-r--r--   0        0        0     2126 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200.py
--rw-r--r--   0        0        0     5580 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results.py
--rw-r--r--   0        0        0     2347 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_access_item.py
--rw-r--r--   0        0        0      286 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_access_item_role.py
--rw-r--r--   0        0        0     7625 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     1305 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2249 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7961 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item.py
--rw-r--r--   0        0        0      372 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1293 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_status.py
--rw-r--r--   0        0        0     1119 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0     1921 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/user_allowed_organization.py
--rw-r--r--   0        0        0     1837 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_json_body.py
--rw-r--r--   0        0        0     2220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200.py
--rw-r--r--   0        0        0     1491 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200_results.py
--rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200_status.py
--rw-r--r--   0        0        0     6761 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response.py
--rw-r--r--   0        0        0      360 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response_chart_type.py
--rw-r--r--   0        0        0      278 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response_error_type.py
--rw-r--r--   0        0        0      207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response_source.py
--rw-r--r--   0        0        0     6098 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response.py
--rw-r--r--   0        0        0      282 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response_error_type.py
--rw-r--r--   0        0        0      211 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response_source.py
--rw-r--r--   0        0        0     3911 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response.py
--rw-r--r--   0        0        0      278 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response_error_type.py
--rw-r--r--   0        0        0      207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response_source.py
--rw-r--r--   0        0        0      260 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_type.py
--rw-r--r--   0        0        0     3711 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base.py
--rw-r--r--   0        0        0      272 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base_error_type.py
--rw-r--r--   0        0        0      201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base_source.py
--rw-r--r--   0        0        0     6642 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0.py
--rw-r--r--   0        0        0      355 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0_chart_type.py
--rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0_error_type.py
--rw-r--r--   0        0        0      202 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0_source.py
--rw-r--r--   0        0        0     5945 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1.py
--rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1_error_type.py
--rw-r--r--   0        0        0      202 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1_source.py
--rw-r--r--   0        0        0     3822 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2.py
--rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2_error_type.py
--rw-r--r--   0        0        0      202 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2_source.py
--rw-r--r--   0        0        0      193 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_source_type.py
--rw-r--r--   0        0        0     1995 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_summary.py
--rw-r--r--   0        0        0     2525 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/view_statistics.py
--rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py
--rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_0_type.py
--rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_1_type.py
--rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_2_type.py
--rw-r--r--   0        0        0      190 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_priority.py
--rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_type.py
--rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py
--rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_4_type.py
--rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_5_type.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_bigquery.py
--rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_databricks.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_postgres.py
--rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_redshift.py
--rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_snowflake.py
--rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_trino.py
--rw-r--r--   0        0        0      225 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/week_day.py
--rw-r--r--   0        0        0       26 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/py.typed
--rw-r--r--   0        0        0      993 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/types.py
--rw-r--r--   0        0        0     1862 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/pyproject.toml
--rw-r--r--   0        0        0      830 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/setup.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.651.2/PKG-INFO
+-rw-r--r--   0        0        0     1040 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/.openapi-generator-ignore
+-rw-r--r--   0        0        0        8 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/.python-version
+-rw-r--r--   0        0        0    11357 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/LICENSE
+-rw-r--r--   0        0        0     3258 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/README.md
+-rw-r--r--   0        0        0      182 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4749 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4592 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5871 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5659 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0     5271 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/exploring/run_metric_query.py
+-rw-r--r--   0        0        0     4897 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/exploring/run_sql_query.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3852 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4545 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4511 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4956 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3655 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     4543 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     4215 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3518 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     4750 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4914 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4375 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     4823 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     5097 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/create_organization.py
+-rw-r--r--   0        0        0     4439 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4292 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3725 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     4767 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/get_organization_member_by_uuid.py
+-rw-r--r--   0        0        0     3909 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     4022 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3898 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0     3902 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_organization_projects.py
+-rw-r--r--   0        0        0     4654 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/update_my_organization.py
+-rw-r--r--   0        0        0     5049 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/organizations/update_organization_email_domains.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     4743 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/delete_validation_dismiss.py
+-rw-r--r--   0        0        0     5908 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     4077 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     4191 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4191 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6431 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     5295 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/add_space_share_to_user.py
+-rw-r--r--   0        0        0     4946 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4941 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     5041 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4688 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     5031 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
+-rw-r--r--   0        0        0     5256 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/update_organization_member.py
+-rw-r--r--   0        0        0     5467 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0     5071 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/update_space.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4140 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     4081 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4332 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     4111 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     4615 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     4687 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/share_links/create_share_url.py
+-rw-r--r--   0        0        0     4004 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4485 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     4463 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3585 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_attributes/__init__.py
+-rw-r--r--   0        0        0     4579 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_attributes/create_user_attribute.py
+-rw-r--r--   0        0        0     3688 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_attributes/get_user_attributes.py
+-rw-r--r--   0        0        0     4310 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_attributes/remove_user_attribute.py
+-rw-r--r--   0        0        0     5119 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_attributes/update_user_attribute.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4462 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     3983 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3953 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4077 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4510 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     4885 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/api/user_groups/update_group.py
+-rw-r--r--   0        0        0     2888 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/errors.py
+-rw-r--r--   0        0        0   186666 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/add_space_share.py
+-rw-r--r--   0        0        0     1497 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/add_space_share_to_user_json_body.py
+-rw-r--r--   0        0        0     2003 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/add_space_share_to_user_response_200.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/add_space_share_to_user_response_200_status.py
+-rw-r--r--   0        0        0     1949 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/add_user_to_group_response_200.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/add_user_to_group_response_200_status.py
+-rw-r--r--   0        0        0     6879 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0      241 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_compact_type_0.py
+-rw-r--r--   0        0        0      281 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_compact_type_1.py
+-rw-r--r--   0        0        0     2365 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_filters_item.py
+-rw-r--r--   0        0        0      650 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_filters_item_operator.py
+-rw-r--r--   0        0        0     1521 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_filters_item_target.py
+-rw-r--r--   0        0        0      241 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_format.py
+-rw-r--r--   0        0        0      393 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_type.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domain_projects_role_type_0.py
+-rw-r--r--   0        0        0      186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domain_projects_role_type_1.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domain_projects_role_type_2.py
+-rw-r--r--   0        0        0     4988 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0     3595 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_projects_item.py
+-rw-r--r--   0        0        0      167 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      191 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      167 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_role_type_0.py
+-rw-r--r--   0        0        0      179 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_role_type_1.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_role_type_2.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_role_type_3.py
+-rw-r--r--   0        0        0     2563 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0     4038 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_chart_summary_list_response_results_item.py
+-rw-r--r--   0        0        0      246 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_chart_summary_list_response_results_item_chart_type.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2294 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_create_user_attribute_response.py
+-rw-r--r--   0        0        0     3462 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_create_user_attribute_response_results.py
+-rw-r--r--   0        0        0     1899 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_create_user_attribute_response_results_users_item.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_create_user_attribute_response_status.py
+-rw-r--r--   0        0        0     2016 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1580 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2776 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     1737 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_integration_settings_results.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_integration_settings_status.py
+-rw-r--r--   0        0        0     2122 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     2325 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics_results.py
+-rw-r--r--   0        0        0     2526 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py
+-rw-r--r--   0        0        0      143 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2019 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0     2224 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response.py
+-rw-r--r--   0        0        0     2709 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response_results.py
+-rw-r--r--   0        0        0     2813 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response_results_otp.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2049 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2277 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2429 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0     2320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_list_response_results_item.py
+-rw-r--r--   0        0        0      145 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2480 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0     2218 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_members_response_results_item.py
+-rw-r--r--   0        0        0      148 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     1993 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0     2274 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_response_results.py
+-rw-r--r--   0        0        0      141 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1476 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2067 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1463 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2003 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2362 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0     5921 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results.py
+-rw-r--r--   0        0        0     4175 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py
+-rw-r--r--   0        0        0      189 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      213 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      189 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_0.py
+-rw-r--r--   0        0        0      201 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_1.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_2.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_3.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2305 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0     3624 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profile_results.py
+-rw-r--r--   0        0        0      304 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profile_results_role.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2591 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0     3678 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profiles_results_item.py
+-rw-r--r--   0        0        0      309 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profiles_results_item_role.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0     2519 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_projects.py
+-rw-r--r--   0        0        0     2151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_projects_results_item.py
+-rw-r--r--   0        0        0      191 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_projects_results_item_type.py
+-rw-r--r--   0        0        0      148 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_projects_status.py
+-rw-r--r--   0        0        0     3203 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_results.py
+-rw-r--r--   0        0        0      140 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4640 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0     2288 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0.py
+-rw-r--r--   0        0        0     7025 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1271 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2207 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      167 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2288 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1.py
+-rw-r--r--   0        0        0     7876 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data.py
+-rw-r--r--   0        0        0      366 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1271 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2207 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2225 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_2.py
+-rw-r--r--   0        0        0     3849 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_2_data.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_2_type.py
+-rw-r--r--   0        0        0      139 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2580 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0     2719 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_access_list_response_results_item.py
+-rw-r--r--   0        0        0      286 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_access_list_response_results_item_role.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0     2027 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response.py
+-rw-r--r--   0        0        0    20745 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results.py
+-rw-r--r--   0        0        0     3377 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      168 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2541 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      188 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     4004 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      174 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     4186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      180 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     4004 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      174 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     4097 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     3152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0      182 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_type.py
+-rw-r--r--   0        0        0     5577 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1419 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6883 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1419 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     7128 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1419 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     6150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      214 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1419 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4260 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1419 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      188 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     4197 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1419 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      178 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0      143 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_status.py
+-rw-r--r--   0        0        0     2050 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2119 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0     6314 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query.py
+-rw-r--r--   0        0        0     8764 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      283 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      323 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3077 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      692 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1779 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      283 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      435 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1767 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1777 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1752 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1762 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1792 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5063 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      284 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      342 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      269 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2497 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0     1711 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduled_jobs_response_results_item.py
+-rw-r--r--   0        0        0      149 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0     2294 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response.py
+-rw-r--r--   0        0        0     4066 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_results.py
+-rw-r--r--   0        0        0     2779 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2799 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0     2177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response.py
+-rw-r--r--   0        0        0     5791 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results.py
+-rw-r--r--   0        0        0     1777 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py
+-rw-r--r--   0        0        0     1779 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py
+-rw-r--r--   0        0        0     5858 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py
+-rw-r--r--   0        0        0     1392 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py
+-rw-r--r--   0        0        0      250 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_status.py
+-rw-r--r--   0        0        0      194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_target_type.py
+-rw-r--r--   0        0        0      470 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_task.py
+-rw-r--r--   0        0        0     4266 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py
+-rw-r--r--   0        0        0     2822 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2842 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1952 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_users_item.py
+-rw-r--r--   0        0        0      149 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2148 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0     3477 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_share_response_results.py
+-rw-r--r--   0        0        0      141 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2497 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0     1608 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_slack_channels_response_results_item.py
+-rw-r--r--   0        0        0      149 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0     1993 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response.py
+-rw-r--r--   0        0        0     5415 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results.py
+-rw-r--r--   0        0        0     2283 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_access_item.py
+-rw-r--r--   0        0        0      280 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_access_item_role.py
+-rw-r--r--   0        0        0     7498 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_dashboards_item.py
+-rw-r--r--   0        0        0     1279 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2216 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7797 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item.py
+-rw-r--r--   0        0        0      366 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1267 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2201 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      141 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2563 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0     3584 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_summary_list_response_results_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2422 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_sql_query_results.py
+-rw-r--r--   0        0        0     1273 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_sql_query_results_fields.py
+-rw-r--r--   0        0        0     1286 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_sql_query_results_rows_item.py
+-rw-r--r--   0        0        0     2178 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0     1572 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_ssh_key_pair_response_results.py
+-rw-r--r--   0        0        0      146 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1828 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2699 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0     2048 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_allowed_organizations_response_results_item.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     2514 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_attributes_response.py
+-rw-r--r--   0        0        0     3450 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_attributes_response_results_item.py
+-rw-r--r--   0        0        0     1894 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_attributes_response_results_item_users_item.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_user_attributes_response_status.py
+-rw-r--r--   0        0        0     4920 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0     6933 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_0.py
+-rw-r--r--   0        0        0      367 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_0_chart_type.py
+-rw-r--r--   0        0        0      285 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_0_error_type.py
+-rw-r--r--   0        0        0      214 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_0_source.py
+-rw-r--r--   0        0        0     6161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_1.py
+-rw-r--r--   0        0        0      285 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_1_error_type.py
+-rw-r--r--   0        0        0      214 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_1_source.py
+-rw-r--r--   0        0        0     4038 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_2.py
+-rw-r--r--   0        0        0      285 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_2_error_type.py
+-rw-r--r--   0        0        0      214 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_2_source.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1674 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0     5370 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/bigquery_credentials.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/bigquery_credentials_priority.py
+-rw-r--r--   0        0        0     1251 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/bigquery_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/bigquery_credentials_type.py
+-rw-r--r--   0        0        0      332 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     4853 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler_format.py
+-rw-r--r--   0        0        0     2484 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1231 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler_options_type_1.py
+-rw-r--r--   0        0        0     3723 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      220 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_summary_chart_type.py
+-rw-r--r--   0        0        0      208 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      232 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/compact_or_alias_type_0.py
+-rw-r--r--   0        0        0      272 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0      634 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/conditional_operator.py
+-rw-r--r--   0        0        0     2523 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200.py
+-rw-r--r--   0        0        0     2919 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200_results.py
+-rw-r--r--   0        0        0     2897 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200_status.py
+-rw-r--r--   0        0        0     1528 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_json_body.py
+-rw-r--r--   0        0        0     2402 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_response_200.py
+-rw-r--r--   0        0        0     2383 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_response_200_results.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_response_200_status.py
+-rw-r--r--   0        0        0     1481 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_organization.py
+-rw-r--r--   0        0        0     1494 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_organization_json_body.py
+-rw-r--r--   0        0        0     1981 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_organization_response_200.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_organization_response_200_status.py
+-rw-r--r--   0        0        0     1896 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0      266 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_project_member_role.py
+-rw-r--r--   0        0        0     1624 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_share_url.py
+-rw-r--r--   0        0        0     1652 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_json_body.py
+-rw-r--r--   0        0        0     2364 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_response_201.py
+-rw-r--r--   0        0        0     3528 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_response_201_results.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_response_201_status.py
+-rw-r--r--   0        0        0     2601 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     2146 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_access_item.py
+-rw-r--r--   0        0        0      268 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_access_item_role.py
+-rw-r--r--   0        0        0     2867 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_json_body.py
+-rw-r--r--   0        0        0     2341 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_json_body_access_item.py
+-rw-r--r--   0        0        0      285 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_json_body_access_item_role.py
+-rw-r--r--   0        0        0     2317 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200.py
+-rw-r--r--   0        0        0     5832 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results.py
+-rw-r--r--   0        0        0     2445 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_access_item.py
+-rw-r--r--   0        0        0      295 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7875 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1345 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2300 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     8225 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      381 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1333 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2285 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2312 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_ssh_key_pair_response_201.py
+-rw-r--r--   0        0        0     1605 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_ssh_key_pair_response_201_results.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_ssh_key_pair_response_201_status.py
+-rw-r--r--   0        0        0     2498 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute.py
+-rw-r--r--   0        0        0     2650 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_json_body.py
+-rw-r--r--   0        0        0     1764 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_json_body_users_item.py
+-rw-r--r--   0        0        0     2294 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_response_200.py
+-rw-r--r--   0        0        0     3462 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_response_200_results.py
+-rw-r--r--   0        0        0     1899 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_response_200_results_users_item.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_response_200_status.py
+-rw-r--r--   0        0        0     1718 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_users_item.py
+-rw-r--r--   0        0        0     1695 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_value.py
+-rw-r--r--   0        0        0     7127 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_basic_details.py
+-rw-r--r--   0        0        0     1209 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_basic_details_updated_by_user.py
+-rw-r--r--   0        0        0     2127 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_basic_details_validation_errors_item.py
+-rw-r--r--   0        0        0     5078 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler.py
+-rw-r--r--   0        0        0      165 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler_format.py
+-rw-r--r--   0        0        0     2536 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler_options_type_0.py
+-rw-r--r--   0        0        0      181 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1251 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler_options_type_1.py
+-rw-r--r--   0        0        0     3711 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/databricks_credentials.py
+-rw-r--r--   0        0        0     1261 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/databricks_credentials_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/databricks_credentials_type.py
+-rw-r--r--   0        0        0     3801 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py
+-rw-r--r--   0        0        0     1669 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_azure_dev_ops_project_config_type.py
+-rw-r--r--   0        0        0     3844 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_bit_bucket_project_config.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_bit_bucket_project_config_type.py
+-rw-r--r--   0        0        0     2352 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_ide_project_config.py
+-rw-r--r--   0        0        0      169 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_ide_project_config_type.py
+-rw-r--r--   0        0        0     1638 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_integration.py
+-rw-r--r--   0        0        0     2397 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2556 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py
+-rw-r--r--   0        0        0     2404 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     3609 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_github_project_config.py
+-rw-r--r--   0        0        0     1638 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_github_project_config_environment_item.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_github_project_config_type.py
+-rw-r--r--   0        0        0     3609 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_gitlab_project_config.py
+-rw-r--r--   0        0        0     1638 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_gitlab_project_config_environment_item.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_gitlab_project_config_type.py
+-rw-r--r--   0        0        0     2966 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_local_project_config.py
+-rw-r--r--   0        0        0     1633 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_local_project_config_environment_item.py
+-rw-r--r--   0        0        0      146 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_local_project_config_type.py
+-rw-r--r--   0        0        0     2725 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_none_project_config.py
+-rw-r--r--   0        0        0     1628 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_none_project_config_environment_item.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_none_project_config_type.py
+-rw-r--r--   0        0        0     1636 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_0_environment_item.py
+-rw-r--r--   0        0        0      146 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_0_type.py
+-rw-r--r--   0        0        0     2325 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_1.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_1_type.py
+-rw-r--r--   0        0        0     1636 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_2_environment_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_2_type.py
+-rw-r--r--   0        0        0     1636 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_3_environment_item.py
+-rw-r--r--   0        0        0      158 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_3_type.py
+-rw-r--r--   0        0        0     1636 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_4_environment_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_4_type.py
+-rw-r--r--   0        0        0     1636 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_5_environment_item.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_5_type.py
+-rw-r--r--   0        0        0     1636 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_6_environment_item.py
+-rw-r--r--   0        0        0      148 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_6_type.py
+-rw-r--r--   0        0        0     1592 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_environment_variable.py
+-rw-r--r--   0        0        0      295 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_azuredevops.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_bitbucket.py
+-rw-r--r--   0        0        0      138 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_dbt.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_dbtcloudide.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_github.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_gitlab.py
+-rw-r--r--   0        0        0      141 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_type_none.py
+-rw-r--r--   0        0        0     2143 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0      169 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     1902 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_group_response_200.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_group_response_200_status.py
+-rw-r--r--   0        0        0     1872 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_me_response_200.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_me_response_200_status.py
+-rw-r--r--   0        0        0     2005 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_my_organization_response_200.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2045 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_organization_member_response_200.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_organization_member_response_200_status.py
+-rw-r--r--   0        0        0     1951 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     1902 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_space_response_204.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_space_response_204_status.py
+-rw-r--r--   0        0        0     1738 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_validation_dismiss_response_200.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/delete_validation_dismiss_response_200_status.py
+-rw-r--r--   0        0        0     1931 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2677 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2281 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     2527 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/email_status_expiring.py
+-rw-r--r--   0        0        0     2757 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/email_status_expiring_otp.py
+-rw-r--r--   0        0        0     1898 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/email_status_otp.py
+-rw-r--r--   0        0        0     1574 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1584 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     5812 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     1561 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1571 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1546 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1556 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/filters_metrics_type_1.py
+-rw-r--r--   0        0        0      225 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/format_.py
+-rw-r--r--   0        0        0     2098 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_csv_url_response_200.py
+-rw-r--r--   0        0        0     1598 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_csv_url_response_200_results.py
+-rw-r--r--   0        0        0      145 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_csv_url_response_200_status.py
+-rw-r--r--   0        0        0     2986 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0     1798 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     2372 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200.py
+-rw-r--r--   0        0        0     2467 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py
+-rw-r--r--   0        0        0     2587 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_status.py
+-rw-r--r--   0        0        0     2517 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200.py
+-rw-r--r--   0        0        0     2914 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200_results.py
+-rw-r--r--   0        0        0     2894 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200_results_otp.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200_status.py
+-rw-r--r--   0        0        0     2546 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_group_members_response_200.py
+-rw-r--r--   0        0        0     2236 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_group_members_response_200_results_item.py
+-rw-r--r--   0        0        0      151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_group_members_response_200_status.py
+-rw-r--r--   0        0        0     2050 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_group_response_200.py
+-rw-r--r--   0        0        0     2292 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_group_response_200_results.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_group_response_200_status.py
+-rw-r--r--   0        0        0     5697 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200.py
+-rw-r--r--   0        0        0     7347 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0      385 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_chart_type.py
+-rw-r--r--   0        0        0      303 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_error_type.py
+-rw-r--r--   0        0        0      232 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_source.py
+-rw-r--r--   0        0        0     6464 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0      303 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_error_type.py
+-rw-r--r--   0        0        0      232 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_source.py
+-rw-r--r--   0        0        0     4341 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0      303 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_error_type.py
+-rw-r--r--   0        0        0      232 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_source.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_status.py
+-rw-r--r--   0        0        0     2293 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_my_organization_response_200.py
+-rw-r--r--   0        0        0     3277 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_my_organization_response_200_results.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2493 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_organization_member_by_uuid_response_200.py
+-rw-r--r--   0        0        0     3736 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_organization_member_by_uuid_response_200_results.py
+-rw-r--r--   0        0        0      314 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_organization_member_by_uuid_response_200_results_role.py
+-rw-r--r--   0        0        0      163 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_organization_member_by_uuid_response_200_status.py
+-rw-r--r--   0        0        0     5193 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200.py
+-rw-r--r--   0        0        0     2499 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0     7259 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1319 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2268 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      178 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2499 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0     8178 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py
+-rw-r--r--   0        0        0      377 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1319 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2268 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2424 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0     3910 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_type.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_status.py
+-rw-r--r--   0        0        0     2637 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_access_list_response_200.py
+-rw-r--r--   0        0        0     2753 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_access_list_response_200_results_item.py
+-rw-r--r--   0        0        0      289 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_access_list_response_200_results_item_role.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_access_list_response_200_status.py
+-rw-r--r--   0        0        0     2109 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200.py
+-rw-r--r--   0        0        0    21254 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results.py
+-rw-r--r--   0        0        0     3430 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      171 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2571 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      191 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     4057 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     4239 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      183 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     4057 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     4150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      189 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     3205 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      173 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0      185 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_type.py
+-rw-r--r--   0        0        0     5637 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      189 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6943 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     7188 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     6229 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      217 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      191 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     4257 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1437 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      181 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0      146 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_status.py
+-rw-r--r--   0        0        0     2563 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduled_jobs_response_200.py
+-rw-r--r--   0        0        0     1729 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduled_jobs_response_200_status.py
+-rw-r--r--   0        0        0     2334 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_job_status_response_200.py
+-rw-r--r--   0        0        0     1529 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_job_status_response_200_results.py
+-rw-r--r--   0        0        0      157 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_job_status_response_200_status.py
+-rw-r--r--   0        0        0     2243 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200.py
+-rw-r--r--   0        0        0     5924 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results.py
+-rw-r--r--   0        0        0     1795 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py
+-rw-r--r--   0        0        0     1797 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     5953 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py
+-rw-r--r--   0        0        0     1410 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py
+-rw-r--r--   0        0        0      253 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_status.py
+-rw-r--r--   0        0        0      197 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_target_type.py
+-rw-r--r--   0        0        0      473 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_task.py
+-rw-r--r--   0        0        0     4392 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py
+-rw-r--r--   0        0        0     2840 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2860 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1970 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_status.py
+-rw-r--r--   0        0        0     2160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200.py
+-rw-r--r--   0        0        0     3838 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_results.py
+-rw-r--r--   0        0        0     2741 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2761 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      148 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_status.py
+-rw-r--r--   0        0        0     2304 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_share_url_response_200.py
+-rw-r--r--   0        0        0     3513 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_share_url_response_200_results.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_share_url_response_200_status.py
+-rw-r--r--   0        0        0     2563 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_slack_channels_response_200.py
+-rw-r--r--   0        0        0     1626 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_slack_channels_response_200_results_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_slack_channels_response_200_status.py
+-rw-r--r--   0        0        0     2050 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200.py
+-rw-r--r--   0        0        0     5502 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results.py
+-rw-r--r--   0        0        0     2317 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_access_item.py
+-rw-r--r--   0        0        0      283 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7565 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1293 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2234 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7883 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      369 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1281 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2219 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_status.py
+-rw-r--r--   0        0        0     2580 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_user_attributes_response_200.py
+-rw-r--r--   0        0        0     3491 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_user_attributes_response_200_results_item.py
+-rw-r--r--   0        0        0     1912 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_user_attributes_response_200_results_item_users_item.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/get_user_attributes_response_200_status.py
+-rw-r--r--   0        0        0     2051 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/grant_project_access_to_user_json_body.py
+-rw-r--r--   0        0        0      279 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/grant_project_access_to_user_json_body_role.py
+-rw-r--r--   0        0        0     2053 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/grant_project_access_to_user_response_200.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/grant_project_access_to_user_response_200_status.py
+-rw-r--r--   0        0        0     2175 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2091 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     1961 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/join_organization_response_200.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/join_organization_response_200_status.py
+-rw-r--r--   0        0        0     2620 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_charts_in_project_response_200.py
+-rw-r--r--   0        0        0     4075 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_charts_in_project_response_200_results_item.py
+-rw-r--r--   0        0        0      249 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_charts_in_project_response_200_results_item_chart_type.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_charts_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2705 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_groups_in_organization_response_200.py
+-rw-r--r--   0        0        0     2401 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_groups_in_organization_response_200_results_item.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_groups_in_organization_response_200_status.py
+-rw-r--r--   0        0        0     2773 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_my_available_organizations_response_200.py
+-rw-r--r--   0        0        0     2071 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_my_available_organizations_response_200_results_item.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_my_available_organizations_response_200_status.py
+-rw-r--r--   0        0        0     2453 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200.py
+-rw-r--r--   0        0        0     6137 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results.py
+-rw-r--r--   0        0        0     4306 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py
+-rw-r--r--   0        0        0      194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      218 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      182 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_0.py
+-rw-r--r--   0        0        0      206 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_1.py
+-rw-r--r--   0        0        0      182 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_2.py
+-rw-r--r--   0        0        0      182 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_3.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_status.py
+-rw-r--r--   0        0        0     2682 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_members_response_200.py
+-rw-r--r--   0        0        0     3732 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_members_response_200_results_item.py
+-rw-r--r--   0        0        0      314 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_members_response_200_results_item_role.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_members_response_200_status.py
+-rw-r--r--   0        0        0     2744 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_projects_response_200.py
+-rw-r--r--   0        0        0     2279 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_projects_response_200_results_item.py
+-rw-r--r--   0        0        0      203 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_projects_response_200_results_item_type.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_organization_projects_response_200_status.py
+-rw-r--r--   0        0        0     2620 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_spaces_in_project_response_200.py
+-rw-r--r--   0        0        0     3602 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_spaces_in_project_response_200_results_item.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/list_spaces_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2133 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_filter_rule.py
+-rw-r--r--   0        0        0      639 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_filter_rule_operator.py
+-rw-r--r--   0        0        0     1463 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_filter_rule_target.py
+-rw-r--r--   0        0        0     5557 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0     7990 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item.py
+-rw-r--r--   0        0        0      265 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      305 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     2769 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      674 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1653 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      265 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      417 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     7034 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters.py
+-rw-r--r--   0        0        0     1665 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1675 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1650 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1660 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1690 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_sorts_item.py
+-rw-r--r--   0        0        0     3183 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item.py
+-rw-r--r--   0        0        0     4643 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item_format.py
+-rw-r--r--   0        0        0      266 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      324 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      251 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      383 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0      284 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/number_separator.py
+-rw-r--r--   0        0        0     5630 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     4125 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py
+-rw-r--r--   0        0        0      187 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      211 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      187 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      175 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_0.py
+-rw-r--r--   0        0        0      199 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_1.py
+-rw-r--r--   0        0        0      175 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_2.py
+-rw-r--r--   0        0        0      175 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_3.py
+-rw-r--r--   0        0        0     6420 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      224 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     1469 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     4520 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1479 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      200 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     7338 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1469 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     7093 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1469 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5805 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1474 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      197 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     4353 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1454 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      185 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     2025 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_user_attribute_uuid_or_created_at_or_organization_uuid_or_users.py
+-rw-r--r--   0        0        0     1713 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_user_attribute_value_email.py
+-rw-r--r--   0        0        0     3794 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_validation_response_base_name.py
+-rw-r--r--   0        0        0      280 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_validation_response_base_name_error_type.py
+-rw-r--r--   0        0        0      209 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/omit_validation_response_base_name_source.py
+-rw-r--r--   0        0        0     3147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3507 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0      294 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_profile_role.py
+-rw-r--r--   0        0        0     1674 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_profile_update.py
+-rw-r--r--   0        0        0      300 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_profile_update_role.py
+-rw-r--r--   0        0        0      287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_role_editor.py
+-rw-r--r--   0        0        0      190 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_role_interactiveviewer.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_role_member.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_member_role_viewer.py
+-rw-r--r--   0        0        0     1980 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_project.py
+-rw-r--r--   0        0        0      176 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/organization_project_type.py
+-rw-r--r--   0        0        0     2713 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     6971 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     5108 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py
+-rw-r--r--   0        0        0      218 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      242 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      218 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      206 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_0.py
+-rw-r--r--   0        0        0      230 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_1.py
+-rw-r--r--   0        0        0      206 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_2.py
+-rw-r--r--   0        0        0      206 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_3.py
+-rw-r--r--   0        0        0     7661 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      267 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     1728 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5374 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1748 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      245 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     1769 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1493 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     8285 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1728 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     8036 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1728 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     6654 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1738 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      235 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5124 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1693 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      219 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     9895 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py
+-rw-r--r--   0        0        0     1834 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
+-rw-r--r--   0        0        0     2946 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
+-rw-r--r--   0        0        0     7951 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1840 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
+-rw-r--r--   0        0        0     1460 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1494 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     1926 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3654 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     5491 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1610 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
+-rw-r--r--   0        0        0     1685 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     3330 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3330 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0    11635 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py
+-rw-r--r--   0        0        0      496 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_chart_type.py
+-rw-r--r--   0        0        0     1838 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
+-rw-r--r--   0        0        0     2952 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
+-rw-r--r--   0        0        0     1547 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     2179 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_user_attribute_exclude_keyof_user_attribute_uuid_or_created_at_or_organization_uuid_or_users.py
+-rw-r--r--   0        0        0     1871 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_user_attribute_value_exclude_keyof_user_attribute_value_email.py
+-rw-r--r--   0        0        0     4356 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0      314 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_error_type.py
+-rw-r--r--   0        0        0      243 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_source.py
+-rw-r--r--   0        0        0     2194 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     1227 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      157 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_0_type.py
+-rw-r--r--   0        0        0      356 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1227 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      149 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_1_type.py
+-rw-r--r--   0        0        0     3793 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_2_data.py
+-rw-r--r--   0        0        0      149 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_2_type.py
+-rw-r--r--   0        0        0     2212 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     7343 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters.py
+-rw-r--r--   0        0        0     1696 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1706 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1681 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1691 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     2243 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200.py
+-rw-r--r--   0        0        0     2220 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results.py
+-rw-r--r--   0        0        0     6589 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     9144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      291 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      331 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3254 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      700 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1822 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      291 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      443 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8643 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1810 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1820 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1795 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1805 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1835 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3546 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5245 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      292 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      350 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      277 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_status.py
+-rw-r--r--   0        0        0     6528 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body.py
+-rw-r--r--   0        0        0     8653 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py
+-rw-r--r--   0        0        0      280 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3029 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      689 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1740 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      280 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      432 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1931 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py
+-rw-r--r--   0        0        0     1777 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py
+-rw-r--r--   0        0        0     3398 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py
+-rw-r--r--   0        0        0     4997 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py
+-rw-r--r--   0        0        0      281 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      339 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      266 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     2425 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200.py
+-rw-r--r--   0        0        0     2350 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results.py
+-rw-r--r--   0        0        0     7047 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     9752 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      301 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      341 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3456 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      710 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1934 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      301 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      453 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     9367 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1890 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1900 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1875 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1885 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1891 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3740 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5635 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      302 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      360 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_status.py
+-rw-r--r--   0        0        0     6543 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/postgres_credentials.py
+-rw-r--r--   0        0        0     1251 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/postgres_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/postgres_credentials_type.py
+-rw-r--r--   0        0        0    17362 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project.py
+-rw-r--r--   0        0        0     3035 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2361 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     3662 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     3844 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     3662 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     3755 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      168 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     2810 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1656 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      152 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0     2504 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      267 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_member_profile_role.py
+-rw-r--r--   0        0        0      260 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_member_role_editor.py
+-rw-r--r--   0        0        0      185 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_member_role_interactiveviewer.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_member_role_viewer.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_type.py
+-rw-r--r--   0        0        0     5235 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      168 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6541 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     6786 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     5697 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      196 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     3918 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     3855 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0     1222 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0     1298 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/record_string_type_dimension_type.py
+-rw-r--r--   0        0        0     1242 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/record_string_unknown.py
+-rw-r--r--   0        0        0     6298 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/redshift_credentials.py
+-rw-r--r--   0        0        0     1251 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/redshift_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/redshift_credentials_type.py
+-rw-r--r--   0        0        0     1995 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/remove_user_attribute_response_200.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/remove_user_attribute_response_200_status.py
+-rw-r--r--   0        0        0     1999 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/remove_user_from_group_response_200.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/remove_user_from_group_response_200_status.py
+-rw-r--r--   0        0        0     2066 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item.py
+-rw-r--r--   0        0        0     7618 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data.py
+-rw-r--r--   0        0        0      357 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data_chart_type.py
+-rw-r--r--   0        0        0     1229 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py
+-rw-r--r--   0        0        0     2153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_type.py
+-rw-r--r--   0        0        0     2159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item.py
+-rw-r--r--   0        0        0     6904 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_data.py
+-rw-r--r--   0        0        0     1245 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py
+-rw-r--r--   0        0        0     2173 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_type.py
+-rw-r--r--   0        0        0      193 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2003 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3795 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/resource_view_space_item_type.py
+-rw-r--r--   0        0        0     2073 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/revoke_project_access_for_user_response_200.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/revoke_project_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     2053 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/revoke_space_access_for_user_response_200.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/revoke_space_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     6110 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body.py
+-rw-r--r--   0        0        0     8117 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item.py
+-rw-r--r--   0        0        0      268 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      308 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     2827 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      677 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1674 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      268 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      420 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1865 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_filters.py
+-rw-r--r--   0        0        0     1711 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_sorts_item.py
+-rw-r--r--   0        0        0     3232 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_table_calculations_item.py
+-rw-r--r--   0        0        0     4721 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_table_calculations_item_format.py
+-rw-r--r--   0        0        0      269 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      327 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      254 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     2209 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200.py
+-rw-r--r--   0        0        0     2196 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results.py
+-rw-r--r--   0        0        0     6523 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     9070 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      289 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      329 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3222 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      698 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1812 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      289 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      441 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8549 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1800 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1810 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1785 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1795 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1825 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3520 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5201 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      290 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      348 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      275 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      150 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_status.py
+-rw-r--r--   0        0        0     5680 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     7800 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item.py
+-rw-r--r--   0        0        0      261 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      301 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     2705 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      670 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1633 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      261 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_format.py
+-rw-r--r--   0        0        0      413 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1824 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1670 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_sorts_item.py
+-rw-r--r--   0        0        0     3131 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item.py
+-rw-r--r--   0        0        0     4555 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item_format.py
+-rw-r--r--   0        0        0      262 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      320 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      247 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     1410 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_json_body.py
+-rw-r--r--   0        0        0     2149 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_response_200.py
+-rw-r--r--   0        0        0     2729 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_response_200_results.py
+-rw-r--r--   0        0        0     1334 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_response_200_results_fields.py
+-rw-r--r--   0        0        0     1347 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_response_200_results_rows_item.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_response_200_status.py
+-rw-r--r--   0        0        0     1589 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     3502 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_and_targets.py
+-rw-r--r--   0        0        0     2680 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py
+-rw-r--r--   0        0        0     2700 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py
+-rw-r--r--   0        0        0     4849 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base_format.py
+-rw-r--r--   0        0        0     2471 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base_options_type_0.py
+-rw-r--r--   0        0        0      176 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1226 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base_options_type_1.py
+-rw-r--r--   0        0        0     2376 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2613 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1200 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     4954 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0     1242 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log_details.py
+-rw-r--r--   0        0        0      223 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log_status.py
+-rw-r--r--   0        0        0      167 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2415 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_options_type_0.py
+-rw-r--r--   0        0        0      172 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1203 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_options_type_1.py
+-rw-r--r--   0        0        0     2593 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_0_format.py
+-rw-r--r--   0        0        0     2488 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_0_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_0_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1234 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_0_options_type_1.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_1_format.py
+-rw-r--r--   0        0        0     2488 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_1_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_1_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1234 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_1_options_type_1.py
+-rw-r--r--   0        0        0     5079 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs.py
+-rw-r--r--   0        0        0     1701 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_charts_item.py
+-rw-r--r--   0        0        0     1703 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_dashboards_item.py
+-rw-r--r--   0        0        0     5415 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item.py
+-rw-r--r--   0        0        0     1316 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item_details.py
+-rw-r--r--   0        0        0      236 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item_status.py
+-rw-r--r--   0        0        0      180 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item_target_type.py
+-rw-r--r--   0        0        0      456 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item_task.py
+-rw-r--r--   0        0        0     3862 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_schedulers_item.py
+-rw-r--r--   0        0        0     2746 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2766 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1876 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_users_item.py
+-rw-r--r--   0        0        0     3396 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1481 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     5010 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/snowflake_credentials.py
+-rw-r--r--   0        0        0     1256 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/snowflake_credentials_start_of_week.py
+-rw-r--r--   0        0        0      157 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/snowflake_credentials_type.py
+-rw-r--r--   0        0        0     1586 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     4794 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space.py
+-rw-r--r--   0        0        0     2082 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_access_item.py
+-rw-r--r--   0        0        0      262 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_access_item_role.py
+-rw-r--r--   0        0        0     6938 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_dashboard.py
+-rw-r--r--   0        0        0     1179 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_dashboard_updated_by_user.py
+-rw-r--r--   0        0        0     2089 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_dashboard_validation_errors_item.py
+-rw-r--r--   0        0        0     7087 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_dashboards_item.py
+-rw-r--r--   0        0        0     1201 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2117 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7266 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item.py
+-rw-r--r--   0        0        0      348 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1189 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2102 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7060 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_query.py
+-rw-r--r--   0        0        0      342 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_query_chart_type.py
+-rw-r--r--   0        0        0     1163 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_query_updated_by_user.py
+-rw-r--r--   0        0        0     2069 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_query_validation_errors_item.py
+-rw-r--r--   0        0        0     2028 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0      257 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_share_role.py
+-rw-r--r--   0        0        0     3439 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0      242 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/table_calculation_format_compact.py
+-rw-r--r--   0        0        0      300 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/table_calculation_format_separator.py
+-rw-r--r--   0        0        0      227 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/table_calculation_format_type.py
+-rw-r--r--   0        0        0     3516 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/trino_credentials.py
+-rw-r--r--   0        0        0     1236 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/trino_credentials_start_of_week.py
+-rw-r--r--   0        0        0      145 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/trino_credentials_type.py
+-rw-r--r--   0        0        0     5066 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains.py
+-rw-r--r--   0        0        0     3751 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_projects_item.py
+-rw-r--r--   0        0        0      173 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      197 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      173 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_role_type_0.py
+-rw-r--r--   0        0        0      185 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_role_type_1.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_role_type_2.py
+-rw-r--r--   0        0        0      161 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_role_type_3.py
+-rw-r--r--   0        0        0     3040 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0     1813 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py
+-rw-r--r--   0        0        0      169 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     1447 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_group.py
+-rw-r--r--   0        0        0     1493 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_group_json_body.py
+-rw-r--r--   0        0        0     2126 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_group_response_200.py
+-rw-r--r--   0        0        0     2307 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_group_response_200_results.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_group_response_200_status.py
+-rw-r--r--   0        0        0     2575 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_my_organization_json_body.py
+-rw-r--r--   0        0        0     2005 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_my_organization_response_200.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2520 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization.py
+-rw-r--r--   0        0        0     5551 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body.py
+-rw-r--r--   0        0        0     4100 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py
+-rw-r--r--   0        0        0      186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      210 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      174 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_0.py
+-rw-r--r--   0        0        0      198 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_1.py
+-rw-r--r--   0        0        0      174 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_2.py
+-rw-r--r--   0        0        0      174 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_3.py
+-rw-r--r--   0        0        0     2487 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200.py
+-rw-r--r--   0        0        0     6215 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results.py
+-rw-r--r--   0        0        0     4356 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py
+-rw-r--r--   0        0        0      196 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      220 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      196 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_0.py
+-rw-r--r--   0        0        0      208 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_1.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_2.py
+-rw-r--r--   0        0        0      184 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_3.py
+-rw-r--r--   0        0        0      166 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_status.py
+-rw-r--r--   0        0        0     1715 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_json_body.py
+-rw-r--r--   0        0        0      301 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_json_body_role.py
+-rw-r--r--   0        0        0     2430 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_response_200.py
+-rw-r--r--   0        0        0     3698 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_response_200_results.py
+-rw-r--r--   0        0        0      311 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_response_200_results_role.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_response_200_status.py
+-rw-r--r--   0        0        0     2066 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1798 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_item_order_data.py
+-rw-r--r--   0        0        0      198 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_item_order_type.py
+-rw-r--r--   0        0        0     2356 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_json_body_item.py
+-rw-r--r--   0        0        0     1872 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_json_body_item_data.py
+-rw-r--r--   0        0        0      211 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_json_body_item_type.py
+-rw-r--r--   0        0        0     5525 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200.py
+-rw-r--r--   0        0        0     2641 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0     7522 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1353 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2311 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      186 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2641 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0     8490 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py
+-rw-r--r--   0        0        0      385 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1353 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2311 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      178 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2566 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0     3953 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py
+-rw-r--r--   0        0        0      178 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_type.py
+-rw-r--r--   0        0        0      158 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_status.py
+-rw-r--r--   0        0        0     1716 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_project_access_for_user_json_body.py
+-rw-r--r--   0        0        0      281 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_project_access_for_user_json_body_role.py
+-rw-r--r--   0        0        0     2073 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_project_access_for_user_response_200.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_project_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     1541 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0      266 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_project_member_role.py
+-rw-r--r--   0        0        0     2220 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201.py
+-rw-r--r--   0        0        0     3910 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_results.py
+-rw-r--r--   0        0        0     2756 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2776 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     1556 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space.py
+-rw-r--r--   0        0        0     1602 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_json_body.py
+-rw-r--r--   0        0        0     2126 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200.py
+-rw-r--r--   0        0        0     5580 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results.py
+-rw-r--r--   0        0        0     2347 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_access_item.py
+-rw-r--r--   0        0        0      286 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7625 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1305 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2249 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7961 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      372 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1293 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2234 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      147 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_status.py
+-rw-r--r--   0        0        0     2650 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_user_attribute_json_body.py
+-rw-r--r--   0        0        0     1764 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_user_attribute_json_body_users_item.py
+-rw-r--r--   0        0        0     2294 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_user_attribute_response_200.py
+-rw-r--r--   0        0        0     3462 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_user_attribute_response_200_results.py
+-rw-r--r--   0        0        0     1899 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_user_attribute_response_200_results_users_item.py
+-rw-r--r--   0        0        0      155 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/update_user_attribute_response_200_status.py
+-rw-r--r--   0        0        0     1119 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1921 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     3112 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/user_attribute.py
+-rw-r--r--   0        0        0     1767 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/user_attribute_users_item.py
+-rw-r--r--   0        0        0     1744 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/user_attribute_value.py
+-rw-r--r--   0        0        0     1837 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     2220 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validate_project_response_200.py
+-rw-r--r--   0        0        0     1491 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validate_project_response_200_results.py
+-rw-r--r--   0        0        0      151 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validate_project_response_200_status.py
+-rw-r--r--   0        0        0     6761 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0      360 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_chart_response_chart_type.py
+-rw-r--r--   0        0        0      278 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_chart_response_error_type.py
+-rw-r--r--   0        0        0      207 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_chart_response_source.py
+-rw-r--r--   0        0        0     6098 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      282 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_dashboard_response_error_type.py
+-rw-r--r--   0        0        0      211 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_dashboard_response_source.py
+-rw-r--r--   0        0        0     3911 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_table_response.py
+-rw-r--r--   0        0        0      278 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_table_response_error_type.py
+-rw-r--r--   0        0        0      207 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_table_response_source.py
+-rw-r--r--   0        0        0      260 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3711 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      272 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_base_error_type.py
+-rw-r--r--   0        0        0      201 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_base_source.py
+-rw-r--r--   0        0        0     6642 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_0.py
+-rw-r--r--   0        0        0      355 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_0_chart_type.py
+-rw-r--r--   0        0        0      273 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_0_error_type.py
+-rw-r--r--   0        0        0      202 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_0_source.py
+-rw-r--r--   0        0        0     5945 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_1.py
+-rw-r--r--   0        0        0      273 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_1_error_type.py
+-rw-r--r--   0        0        0      202 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_1_source.py
+-rw-r--r--   0        0        0     3822 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_2.py
+-rw-r--r--   0        0        0      273 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_2_error_type.py
+-rw-r--r--   0        0        0      202 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_2_source.py
+-rw-r--r--   0        0        0      193 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     1995 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/validation_summary.py
+-rw-r--r--   0        0        0     2525 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0     1287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py
+-rw-r--r--   0        0        0      162 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_0_type.py
+-rw-r--r--   0        0        0     1287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_1_type.py
+-rw-r--r--   0        0        0     1287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_2_type.py
+-rw-r--r--   0        0        0      190 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_3_priority.py
+-rw-r--r--   0        0        0     1287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_3_type.py
+-rw-r--r--   0        0        0     1287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py
+-rw-r--r--   0        0        0      164 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_4_type.py
+-rw-r--r--   0        0        0     1287 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_5_type.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_types_bigquery.py
+-rw-r--r--   0        0        0      159 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_types_databricks.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_types_postgres.py
+-rw-r--r--   0        0        0      153 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_types_redshift.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_types_snowflake.py
+-rw-r--r--   0        0        0      144 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/warehouse_types_trino.py
+-rw-r--r--   0        0        0      225 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/models/week_day.py
+-rw-r--r--   0        0        0       26 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/py.typed
+-rw-r--r--   0        0        0      993 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/lightdash_client/types.py
+-rw-r--r--   0        0        0     1862 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-07-31 06:06:31.000000 lightdash_client_python-0.692.1/setup.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.692.1/PKG-INFO
```

### Comparing `lightdash_client_python-0.651.2/.openapi-generator-ignore` & `lightdash_client_python-0.692.1/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/LICENSE` & `lightdash_client_python-0.692.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/README.md` & `lightdash_client_python-0.692.1/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/charts/post_chart_results.py` & `lightdash_client_python-0.692.1/lightdash_client/api/charts/post_chart_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/content/get_pinned_items.py` & `lightdash_client_python-0.692.1/lightdash_client/api/content/get_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/content/update_pinned_items_order.py` & `lightdash_client_python-0.692.1/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_query.py` & `lightdash_client_python-0.692.1/lightdash_client/api/exploring/run_metric_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.post_run_query_json_body import PostRunQueryJsonBody
-from ...models.post_run_query_response_200 import PostRunQueryResponse200
+from ...models.run_metric_query_json_body import RunMetricQueryJsonBody
+from ...models.run_metric_query_response_200 import RunMetricQueryResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     explore_id: str,
     *,
     client: Client,
-    json_body: PostRunQueryJsonBody,
+    json_body: RunMetricQueryJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/projects/{projectUuid}/explores/{exploreId}/runQuery".format(
         client.base_url, projectUuid=project_uuid, exploreId=explore_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -33,54 +33,54 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PostRunQueryResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RunMetricQueryResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PostRunQueryResponse200.from_dict(response.json())
+        response_200 = RunMetricQueryResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[PostRunQueryResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[RunMetricQueryResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     explore_id: str,
     *,
     client: Client,
-    json_body: PostRunQueryJsonBody,
-) -> Response[PostRunQueryResponse200]:
+    json_body: RunMetricQueryJsonBody,
+) -> Response[RunMetricQueryResponse200]:
     """Run a query for explore
 
     Args:
         project_uuid (str):
         explore_id (str):
-        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
+        json_body (RunMetricQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PostRunQueryResponse200]
+        Response[RunMetricQueryResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         explore_id=explore_id,
         client=client,
         json_body=json_body,
@@ -95,29 +95,29 @@
 
 
 def sync(
     project_uuid: str,
     explore_id: str,
     *,
     client: Client,
-    json_body: PostRunQueryJsonBody,
-) -> Optional[PostRunQueryResponse200]:
+    json_body: RunMetricQueryJsonBody,
+) -> Optional[RunMetricQueryResponse200]:
     """Run a query for explore
 
     Args:
         project_uuid (str):
         explore_id (str):
-        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
+        json_body (RunMetricQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PostRunQueryResponse200
+        RunMetricQueryResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         explore_id=explore_id,
         client=client,
         json_body=json_body,
@@ -125,29 +125,29 @@
 
 
 async def asyncio_detailed(
     project_uuid: str,
     explore_id: str,
     *,
     client: Client,
-    json_body: PostRunQueryJsonBody,
-) -> Response[PostRunQueryResponse200]:
+    json_body: RunMetricQueryJsonBody,
+) -> Response[RunMetricQueryResponse200]:
     """Run a query for explore
 
     Args:
         project_uuid (str):
         explore_id (str):
-        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
+        json_body (RunMetricQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PostRunQueryResponse200]
+        Response[RunMetricQueryResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         explore_id=explore_id,
         client=client,
         json_body=json_body,
@@ -160,29 +160,29 @@
 
 
 async def asyncio(
     project_uuid: str,
     explore_id: str,
     *,
     client: Client,
-    json_body: PostRunQueryJsonBody,
-) -> Optional[PostRunQueryResponse200]:
+    json_body: RunMetricQueryJsonBody,
+) -> Optional[RunMetricQueryResponse200]:
     """Run a query for explore
 
     Args:
         project_uuid (str):
         explore_id (str):
-        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
+        json_body (RunMetricQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PostRunQueryResponse200
+        RunMetricQueryResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             explore_id=explore_id,
             client=client,
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_underlying_data_query.py` & `lightdash_client_python-0.692.1/lightdash_client/api/exploring/post_run_underlying_data_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/exports/get_csv_url.py` & `lightdash_client_python-0.692.1/lightdash_client/api/exports/get_csv_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.692.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.692.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py` & `lightdash_client_python-0.692.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_slack_channels.py` & `lightdash_client_python-0.692.1/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.692.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/my_account/create_email_one_time_passcode.py` & `lightdash_client_python-0.692.1/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/my_account/delete_me.py` & `lightdash_client_python-0.692.1/lightdash_client/api/my_account/delete_me.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/my_account/get_email_verification_status.py` & `lightdash_client_python-0.692.1/lightdash_client/api/my_account/get_email_verification_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/my_account/join_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/my_account/join_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/my_account/list_my_available_organizations.py` & `lightdash_client_python-0.692.1/lightdash_client/api/my_account/list_my_available_organizations.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_group_in_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/create_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_my_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/delete_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_organization_member.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/delete_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/get_my_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/get_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_groups_in_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_email_domains.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_members.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_organization_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_projects.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/list_organization_projects.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_my_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/update_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_organization_email_domains.py` & `lightdash_client_python-0.692.1/lightdash_client/api/organizations/update_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/projects/delete_validation_dismiss.py` & `lightdash_client_python-0.692.1/lightdash_client/api/projects/delete_validation_dismiss.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/projects/get_latest_validation_results.py` & `lightdash_client_python-0.692.1/lightdash_client/api/projects/get_latest_validation_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/projects/get_project.py` & `lightdash_client_python-0.692.1/lightdash_client/api/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/projects/list_charts_in_project.py` & `lightdash_client_python-0.692.1/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/projects/list_spaces_in_project.py` & `lightdash_client_python-0.692.1/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/projects/validate_project.py` & `lightdash_client_python-0.692.1/lightdash_client/api/projects/validate_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/add_space_share_to_user.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/add_space_share_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/create_space_in_project.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/get_project_access_list.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/get_project_access_list.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_organization_member.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/update_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_space.py` & `lightdash_client_python-0.692.1/lightdash_client/api/roles_permissions/update_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/delete_scheduler.py` & `lightdash_client_python-0.692.1/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduled_jobs.py` & `lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler.py` & `lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_job_status.py` & `lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_logs.py` & `lightdash_client_python-0.692.1/lightdash_client/api/schedulers/get_scheduler_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/update_scheduler.py` & `lightdash_client_python-0.692.1/lightdash_client/api/schedulers/update_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/share_links/create_share_url.py` & `lightdash_client_python-0.692.1/lightdash_client/api/share_links/create_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/share_links/get_share_url.py` & `lightdash_client_python-0.692.1/lightdash_client/api/share_links/get_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/spaces/delete_space.py` & `lightdash_client_python-0.692.1/lightdash_client/api/spaces/delete_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/spaces/get_space.py` & `lightdash_client_python-0.692.1/lightdash_client/api/spaces/get_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py` & `lightdash_client_python-0.692.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/add_user_to_group.py` & `lightdash_client_python-0.692.1/lightdash_client/api/user_groups/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/delete_group.py` & `lightdash_client_python-0.692.1/lightdash_client/api/user_groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group.py` & `lightdash_client_python-0.692.1/lightdash_client/api/user_groups/get_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group_members.py` & `lightdash_client_python-0.692.1/lightdash_client/api/user_groups/get_group_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/remove_user_from_group.py` & `lightdash_client_python-0.692.1/lightdash_client/api/user_groups/remove_user_from_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/update_group.py` & `lightdash_client_python-0.692.1/lightdash_client/api/user_groups/update_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/client.py` & `lightdash_client_python-0.692.1/lightdash_client/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/__init__.py` & `lightdash_client_python-0.692.1/lightdash_client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .add_user_to_group_response_200_status import AddUserToGroupResponse200Status
 from .additional_metric import AdditionalMetric
 from .additional_metric_compact_type_0 import AdditionalMetricCompactType0
 from .additional_metric_compact_type_1 import AdditionalMetricCompactType1
 from .additional_metric_filters_item import AdditionalMetricFiltersItem
 from .additional_metric_filters_item_operator import AdditionalMetricFiltersItemOperator
 from .additional_metric_filters_item_target import AdditionalMetricFiltersItemTarget
+from .additional_metric_format import AdditionalMetricFormat
 from .additional_metric_type import AdditionalMetricType
 from .allowed_email_domain_projects_role_type_0 import (
     AllowedEmailDomainProjectsRoleType0,
 )
 from .allowed_email_domain_projects_role_type_1 import (
     AllowedEmailDomainProjectsRoleType1,
 )
@@ -43,14 +44,24 @@
 from .api_chart_summary_list_response_results_item import (
     ApiChartSummaryListResponseResultsItem,
 )
 from .api_chart_summary_list_response_results_item_chart_type import (
     ApiChartSummaryListResponseResultsItemChartType,
 )
 from .api_chart_summary_list_response_status import ApiChartSummaryListResponseStatus
+from .api_create_user_attribute_response import ApiCreateUserAttributeResponse
+from .api_create_user_attribute_response_results import (
+    ApiCreateUserAttributeResponseResults,
+)
+from .api_create_user_attribute_response_results_users_item import (
+    ApiCreateUserAttributeResponseResultsUsersItem,
+)
+from .api_create_user_attribute_response_status import (
+    ApiCreateUserAttributeResponseStatus,
+)
 from .api_csv_url_response import ApiCsvUrlResponse
 from .api_csv_url_response_results import ApiCsvUrlResponseResults
 from .api_csv_url_response_status import ApiCsvUrlResponseStatus
 from .api_dbt_cloud_integration_settings import ApiDbtCloudIntegrationSettings
 from .api_dbt_cloud_integration_settings_results import (
     ApiDbtCloudIntegrationSettingsResults,
 )
@@ -329,14 +340,17 @@
 )
 from .api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator import (
     ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItemOperator,
 )
 from .api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target import (
     ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
 )
+from .api_run_query_response_results_metric_query_additional_metrics_item_format import (
+    ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat,
+)
 from .api_run_query_response_results_metric_query_additional_metrics_item_type import (
     ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemType,
 )
 from .api_run_query_response_results_metric_query_filters import (
     ApiRunQueryResponseResultsMetricQueryFilters,
 )
 from .api_run_query_response_results_metric_query_filters_dimensions_type_0 import (
@@ -459,26 +473,37 @@
 )
 from .api_space_response_status import ApiSpaceResponseStatus
 from .api_space_summary_list_response import ApiSpaceSummaryListResponse
 from .api_space_summary_list_response_results_item import (
     ApiSpaceSummaryListResponseResultsItem,
 )
 from .api_space_summary_list_response_status import ApiSpaceSummaryListResponseStatus
+from .api_sql_query_results import ApiSqlQueryResults
+from .api_sql_query_results_fields import ApiSqlQueryResultsFields
+from .api_sql_query_results_rows_item import ApiSqlQueryResultsRowsItem
 from .api_ssh_key_pair_response import ApiSshKeyPairResponse
 from .api_ssh_key_pair_response_results import ApiSshKeyPairResponseResults
 from .api_ssh_key_pair_response_status import ApiSshKeyPairResponseStatus
 from .api_success_empty import ApiSuccessEmpty
 from .api_success_empty_status import ApiSuccessEmptyStatus
 from .api_user_allowed_organizations_response import ApiUserAllowedOrganizationsResponse
 from .api_user_allowed_organizations_response_results_item import (
     ApiUserAllowedOrganizationsResponseResultsItem,
 )
 from .api_user_allowed_organizations_response_status import (
     ApiUserAllowedOrganizationsResponseStatus,
 )
+from .api_user_attributes_response import ApiUserAttributesResponse
+from .api_user_attributes_response_results_item import (
+    ApiUserAttributesResponseResultsItem,
+)
+from .api_user_attributes_response_results_item_users_item import (
+    ApiUserAttributesResponseResultsItemUsersItem,
+)
+from .api_user_attributes_response_status import ApiUserAttributesResponseStatus
 from .api_validate_response import ApiValidateResponse
 from .api_validate_response_results_item_type_0 import (
     ApiValidateResponseResultsItemType0,
 )
 from .api_validate_response_results_item_type_0_chart_type import (
     ApiValidateResponseResultsItemType0ChartType,
 )
@@ -604,14 +629,31 @@
 )
 from .create_space_in_project_response_200_status import (
     CreateSpaceInProjectResponse200Status,
 )
 from .create_ssh_key_pair_response_201 import CreateSshKeyPairResponse201
 from .create_ssh_key_pair_response_201_results import CreateSshKeyPairResponse201Results
 from .create_ssh_key_pair_response_201_status import CreateSshKeyPairResponse201Status
+from .create_user_attribute import CreateUserAttribute
+from .create_user_attribute_json_body import CreateUserAttributeJsonBody
+from .create_user_attribute_json_body_users_item import (
+    CreateUserAttributeJsonBodyUsersItem,
+)
+from .create_user_attribute_response_200 import CreateUserAttributeResponse200
+from .create_user_attribute_response_200_results import (
+    CreateUserAttributeResponse200Results,
+)
+from .create_user_attribute_response_200_results_users_item import (
+    CreateUserAttributeResponse200ResultsUsersItem,
+)
+from .create_user_attribute_response_200_status import (
+    CreateUserAttributeResponse200Status,
+)
+from .create_user_attribute_users_item import CreateUserAttributeUsersItem
+from .create_user_attribute_value import CreateUserAttributeValue
 from .dashboard_basic_details import DashboardBasicDetails
 from .dashboard_basic_details_updated_by_user import DashboardBasicDetailsUpdatedByUser
 from .dashboard_basic_details_validation_errors_item import (
     DashboardBasicDetailsValidationErrorsItem,
 )
 from .dashboard_scheduler import DashboardScheduler
 from .dashboard_scheduler_format import DashboardSchedulerFormat
@@ -731,14 +773,15 @@
 from .filter_group_response_type_0 import FilterGroupResponseType0
 from .filter_group_response_type_1 import FilterGroupResponseType1
 from .filters import Filters
 from .filters_dimensions_type_0 import FiltersDimensionsType0
 from .filters_dimensions_type_1 import FiltersDimensionsType1
 from .filters_metrics_type_0 import FiltersMetricsType0
 from .filters_metrics_type_1 import FiltersMetricsType1
+from .format_ import Format
 from .get_csv_url_response_200 import GetCsvUrlResponse200
 from .get_csv_url_response_200_results import GetCsvUrlResponse200Results
 from .get_csv_url_response_200_status import GetCsvUrlResponse200Status
 from .get_dbt_cloud_integration_settings_response_200 import (
     GetDbtCloudIntegrationSettingsResponse200,
 )
 from .get_dbt_cloud_integration_settings_response_200_results import (
@@ -814,14 +857,26 @@
     GetLatestValidationResultsResponse200Status,
 )
 from .get_my_organization_response_200 import GetMyOrganizationResponse200
 from .get_my_organization_response_200_results import (
     GetMyOrganizationResponse200Results,
 )
 from .get_my_organization_response_200_status import GetMyOrganizationResponse200Status
+from .get_organization_member_by_uuid_response_200 import (
+    GetOrganizationMemberByUuidResponse200,
+)
+from .get_organization_member_by_uuid_response_200_results import (
+    GetOrganizationMemberByUuidResponse200Results,
+)
+from .get_organization_member_by_uuid_response_200_results_role import (
+    GetOrganizationMemberByUuidResponse200ResultsRole,
+)
+from .get_organization_member_by_uuid_response_200_status import (
+    GetOrganizationMemberByUuidResponse200Status,
+)
 from .get_pinned_items_response_200 import GetPinnedItemsResponse200
 from .get_pinned_items_response_200_results_item_type_0 import (
     GetPinnedItemsResponse200ResultsItemType0,
 )
 from .get_pinned_items_response_200_results_item_type_0_data import (
     GetPinnedItemsResponse200ResultsItemType0Data,
 )
@@ -1084,14 +1139,22 @@
 from .get_space_response_200_results_queries_item_updated_by_user import (
     GetSpaceResponse200ResultsQueriesItemUpdatedByUser,
 )
 from .get_space_response_200_results_queries_item_validation_errors_item import (
     GetSpaceResponse200ResultsQueriesItemValidationErrorsItem,
 )
 from .get_space_response_200_status import GetSpaceResponse200Status
+from .get_user_attributes_response_200 import GetUserAttributesResponse200
+from .get_user_attributes_response_200_results_item import (
+    GetUserAttributesResponse200ResultsItem,
+)
+from .get_user_attributes_response_200_results_item_users_item import (
+    GetUserAttributesResponse200ResultsItemUsersItem,
+)
+from .get_user_attributes_response_200_status import GetUserAttributesResponse200Status
 from .grant_project_access_to_user_json_body import GrantProjectAccessToUserJsonBody
 from .grant_project_access_to_user_json_body_role import (
     GrantProjectAccessToUserJsonBodyRole,
 )
 from .grant_project_access_to_user_response_200 import (
     GrantProjectAccessToUserResponse200,
 )
@@ -1208,14 +1271,17 @@
 )
 from .metric_query_response_additional_metrics_item_filters_item_operator import (
     MetricQueryResponseAdditionalMetricsItemFiltersItemOperator,
 )
 from .metric_query_response_additional_metrics_item_filters_item_target import (
     MetricQueryResponseAdditionalMetricsItemFiltersItemTarget,
 )
+from .metric_query_response_additional_metrics_item_format import (
+    MetricQueryResponseAdditionalMetricsItemFormat,
+)
 from .metric_query_response_additional_metrics_item_type import (
     MetricQueryResponseAdditionalMetricsItemType,
 )
 from .metric_query_response_filters import MetricQueryResponseFilters
 from .metric_query_response_filters_dimensions_type_0 import (
     MetricQueryResponseFiltersDimensionsType0,
 )
@@ -1326,14 +1392,18 @@
 )
 from .omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week import (
     OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
 )
 from .omit_create_trino_credentials_sensitive_credentials_field_names_type import (
     OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesType,
 )
+from .omit_user_attribute_uuid_or_created_at_or_organization_uuid_or_users import (
+    OmitUserAttributeUuidOrCreatedAtOrOrganizationUuidOrUsers,
+)
+from .omit_user_attribute_value_email import OmitUserAttributeValueEmail
 from .omit_validation_response_base_name import OmitValidationResponseBaseName
 from .omit_validation_response_base_name_error_type import (
     OmitValidationResponseBaseNameErrorType,
 )
 from .omit_validation_response_base_name_source import (
     OmitValidationResponseBaseNameSource,
 )
@@ -1468,16 +1538,16 @@
 from .pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order import (
     PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrder,
 )
 from .pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user import (
     PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrderUpdatedByUser,
 )
 from .pick_share_url_path_or_params import PickShareUrlPathOrParams
-from .pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private import (
-    PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivate,
+from .pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order import (
+    PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivateOrPinnedListUuidOrPinnedListOrder,
 )
 from .pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid import (
     PickSpaceProjectUuidOrUuidOrNameOrIsPrivateOrPinnedListUuidOrPinnedListOrderOrOrganizationUuid,
 )
 from .pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors import (
     PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrors,
 )
@@ -1487,14 +1557,20 @@
 from .pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user import (
     PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrorsUpdatedByUser,
 )
 from .pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item import (
     PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrorsValidationErrorsItem,
 )
 from .pick_ssh_key_pair_public_key import PickSshKeyPairPublicKey
+from .pick_user_attribute_exclude_keyof_user_attribute_uuid_or_created_at_or_organization_uuid_or_users import (
+    PickUserAttributeExcludeKeyofUserAttributeUuidOrCreatedAtOrOrganizationUuidOrUsers,
+)
+from .pick_user_attribute_value_exclude_keyof_user_attribute_value_email import (
+    PickUserAttributeValueExcludeKeyofUserAttributeValueEmail,
+)
 from .pick_validation_response_base_exclude_keyof_validation_response_base_name import (
     PickValidationResponseBaseExcludeKeyofValidationResponseBaseName,
 )
 from .pick_validation_response_base_exclude_keyof_validation_response_base_name_error_type import (
     PickValidationResponseBaseExcludeKeyofValidationResponseBaseNameErrorType,
 )
 from .pick_validation_response_base_exclude_keyof_validation_response_base_name_source import (
@@ -1553,14 +1629,17 @@
 )
 from .post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator import (
     PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator,
 )
 from .post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target import (
     PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
 )
+from .post_chart_results_response_200_results_metric_query_additional_metrics_item_format import (
+    PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat,
+)
 from .post_chart_results_response_200_results_metric_query_additional_metrics_item_type import (
     PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemType,
 )
 from .post_chart_results_response_200_results_metric_query_filters import (
     PostChartResultsResponse200ResultsMetricQueryFilters,
 )
 from .post_chart_results_response_200_results_metric_query_filters_dimensions_type_0 import (
@@ -1590,113 +1669,14 @@
 from .post_chart_results_response_200_results_metric_query_table_calculations_item_format_separator import (
     PostChartResultsResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator,
 )
 from .post_chart_results_response_200_results_metric_query_table_calculations_item_format_type import (
     PostChartResultsResponse200ResultsMetricQueryTableCalculationsItemFormatType,
 )
 from .post_chart_results_response_200_status import PostChartResultsResponse200Status
-from .post_run_query_json_body import PostRunQueryJsonBody
-from .post_run_query_json_body_additional_metrics_item import (
-    PostRunQueryJsonBodyAdditionalMetricsItem,
-)
-from .post_run_query_json_body_additional_metrics_item_compact_type_0 import (
-    PostRunQueryJsonBodyAdditionalMetricsItemCompactType0,
-)
-from .post_run_query_json_body_additional_metrics_item_compact_type_1 import (
-    PostRunQueryJsonBodyAdditionalMetricsItemCompactType1,
-)
-from .post_run_query_json_body_additional_metrics_item_filters_item import (
-    PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem,
-)
-from .post_run_query_json_body_additional_metrics_item_filters_item_operator import (
-    PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator,
-)
-from .post_run_query_json_body_additional_metrics_item_filters_item_target import (
-    PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
-)
-from .post_run_query_json_body_additional_metrics_item_type import (
-    PostRunQueryJsonBodyAdditionalMetricsItemType,
-)
-from .post_run_query_json_body_filters import PostRunQueryJsonBodyFilters
-from .post_run_query_json_body_sorts_item import PostRunQueryJsonBodySortsItem
-from .post_run_query_json_body_table_calculations_item import (
-    PostRunQueryJsonBodyTableCalculationsItem,
-)
-from .post_run_query_json_body_table_calculations_item_format import (
-    PostRunQueryJsonBodyTableCalculationsItemFormat,
-)
-from .post_run_query_json_body_table_calculations_item_format_compact import (
-    PostRunQueryJsonBodyTableCalculationsItemFormatCompact,
-)
-from .post_run_query_json_body_table_calculations_item_format_separator import (
-    PostRunQueryJsonBodyTableCalculationsItemFormatSeparator,
-)
-from .post_run_query_json_body_table_calculations_item_format_type import (
-    PostRunQueryJsonBodyTableCalculationsItemFormatType,
-)
-from .post_run_query_response_200 import PostRunQueryResponse200
-from .post_run_query_response_200_results import PostRunQueryResponse200Results
-from .post_run_query_response_200_results_metric_query import (
-    PostRunQueryResponse200ResultsMetricQuery,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_0 import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_1 import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
-)
-from .post_run_query_response_200_results_metric_query_additional_metrics_item_type import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemType,
-)
-from .post_run_query_response_200_results_metric_query_filters import (
-    PostRunQueryResponse200ResultsMetricQueryFilters,
-)
-from .post_run_query_response_200_results_metric_query_filters_dimensions_type_0 import (
-    PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
-)
-from .post_run_query_response_200_results_metric_query_filters_dimensions_type_1 import (
-    PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1,
-)
-from .post_run_query_response_200_results_metric_query_filters_metrics_type_0 import (
-    PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0,
-)
-from .post_run_query_response_200_results_metric_query_filters_metrics_type_1 import (
-    PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1,
-)
-from .post_run_query_response_200_results_metric_query_sorts_item import (
-    PostRunQueryResponse200ResultsMetricQuerySortsItem,
-)
-from .post_run_query_response_200_results_metric_query_table_calculations_item import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem,
-)
-from .post_run_query_response_200_results_metric_query_table_calculations_item_format import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat,
-)
-from .post_run_query_response_200_results_metric_query_table_calculations_item_format_compact import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact,
-)
-from .post_run_query_response_200_results_metric_query_table_calculations_item_format_separator import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator,
-)
-from .post_run_query_response_200_results_metric_query_table_calculations_item_format_type import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType,
-)
-from .post_run_query_response_200_status import PostRunQueryResponse200Status
 from .post_run_underlying_data_query_json_body import PostRunUnderlyingDataQueryJsonBody
 from .post_run_underlying_data_query_json_body_additional_metrics_item import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItem,
 )
 from .post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0 import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType0,
 )
@@ -1708,14 +1688,17 @@
 )
 from .post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemOperator,
 )
 from .post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
 )
+from .post_run_underlying_data_query_json_body_additional_metrics_item_format import (
+    PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat,
+)
 from .post_run_underlying_data_query_json_body_additional_metrics_item_type import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemType,
 )
 from .post_run_underlying_data_query_json_body_filters import (
     PostRunUnderlyingDataQueryJsonBodyFilters,
 )
 from .post_run_underlying_data_query_json_body_sorts_item import (
@@ -1759,14 +1742,17 @@
 )
 from .post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator import (
     PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator,
 )
 from .post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target import (
     PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
 )
+from .post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_format import (
+    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat,
+)
 from .post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type import (
     PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType,
 )
 from .post_run_underlying_data_query_response_200_results_metric_query_filters import (
     PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters,
 )
 from .post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0 import (
@@ -1887,17 +1873,23 @@
 from .project_warehouse_connection_type_5_start_of_week import (
     ProjectWarehouseConnectionType5StartOfWeek,
 )
 from .project_warehouse_connection_type_5_type import (
     ProjectWarehouseConnectionType5Type,
 )
 from .record_string_any import RecordStringAny
+from .record_string_type_dimension_type import RecordStringTypeDimensionType
+from .record_string_unknown import RecordStringUnknown
 from .redshift_credentials import RedshiftCredentials
 from .redshift_credentials_start_of_week import RedshiftCredentialsStartOfWeek
 from .redshift_credentials_type import RedshiftCredentialsType
+from .remove_user_attribute_response_200 import RemoveUserAttributeResponse200
+from .remove_user_attribute_response_200_status import (
+    RemoveUserAttributeResponse200Status,
+)
 from .remove_user_from_group_response_200 import RemoveUserFromGroupResponse200
 from .remove_user_from_group_response_200_status import (
     RemoveUserFromGroupResponse200Status,
 )
 from .resource_view_chart_item import ResourceViewChartItem
 from .resource_view_chart_item_data import ResourceViewChartItemData
 from .resource_view_chart_item_data_chart_type import ResourceViewChartItemDataChartType
@@ -1932,14 +1924,119 @@
 )
 from .revoke_space_access_for_user_response_200 import (
     RevokeSpaceAccessForUserResponse200,
 )
 from .revoke_space_access_for_user_response_200_status import (
     RevokeSpaceAccessForUserResponse200Status,
 )
+from .run_metric_query_json_body import RunMetricQueryJsonBody
+from .run_metric_query_json_body_additional_metrics_item import (
+    RunMetricQueryJsonBodyAdditionalMetricsItem,
+)
+from .run_metric_query_json_body_additional_metrics_item_compact_type_0 import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0,
+)
+from .run_metric_query_json_body_additional_metrics_item_compact_type_1 import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1,
+)
+from .run_metric_query_json_body_additional_metrics_item_filters_item import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem,
+)
+from .run_metric_query_json_body_additional_metrics_item_filters_item_operator import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator,
+)
+from .run_metric_query_json_body_additional_metrics_item_filters_item_target import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
+)
+from .run_metric_query_json_body_additional_metrics_item_format import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemFormat,
+)
+from .run_metric_query_json_body_additional_metrics_item_type import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemType,
+)
+from .run_metric_query_json_body_filters import RunMetricQueryJsonBodyFilters
+from .run_metric_query_json_body_sorts_item import RunMetricQueryJsonBodySortsItem
+from .run_metric_query_json_body_table_calculations_item import (
+    RunMetricQueryJsonBodyTableCalculationsItem,
+)
+from .run_metric_query_json_body_table_calculations_item_format import (
+    RunMetricQueryJsonBodyTableCalculationsItemFormat,
+)
+from .run_metric_query_json_body_table_calculations_item_format_compact import (
+    RunMetricQueryJsonBodyTableCalculationsItemFormatCompact,
+)
+from .run_metric_query_json_body_table_calculations_item_format_separator import (
+    RunMetricQueryJsonBodyTableCalculationsItemFormatSeparator,
+)
+from .run_metric_query_json_body_table_calculations_item_format_type import (
+    RunMetricQueryJsonBodyTableCalculationsItemFormatType,
+)
+from .run_metric_query_response_200 import RunMetricQueryResponse200
+from .run_metric_query_response_200_results import RunMetricQueryResponse200Results
+from .run_metric_query_response_200_results_metric_query import (
+    RunMetricQueryResponse200ResultsMetricQuery,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_compact_type_0 import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_compact_type_1 import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_target import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_format import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat,
+)
+from .run_metric_query_response_200_results_metric_query_additional_metrics_item_type import (
+    RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemType,
+)
+from .run_metric_query_response_200_results_metric_query_filters import (
+    RunMetricQueryResponse200ResultsMetricQueryFilters,
+)
+from .run_metric_query_response_200_results_metric_query_filters_dimensions_type_0 import (
+    RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
+)
+from .run_metric_query_response_200_results_metric_query_filters_dimensions_type_1 import (
+    RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1,
+)
+from .run_metric_query_response_200_results_metric_query_filters_metrics_type_0 import (
+    RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0,
+)
+from .run_metric_query_response_200_results_metric_query_filters_metrics_type_1 import (
+    RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1,
+)
+from .run_metric_query_response_200_results_metric_query_sorts_item import (
+    RunMetricQueryResponse200ResultsMetricQuerySortsItem,
+)
+from .run_metric_query_response_200_results_metric_query_table_calculations_item import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem,
+)
+from .run_metric_query_response_200_results_metric_query_table_calculations_item_format import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat,
+)
+from .run_metric_query_response_200_results_metric_query_table_calculations_item_format_compact import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact,
+)
+from .run_metric_query_response_200_results_metric_query_table_calculations_item_format_separator import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator,
+)
+from .run_metric_query_response_200_results_metric_query_table_calculations_item_format_type import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType,
+)
+from .run_metric_query_response_200_status import RunMetricQueryResponse200Status
 from .run_query_request import RunQueryRequest
 from .run_query_request_additional_metrics_item import (
     RunQueryRequestAdditionalMetricsItem,
 )
 from .run_query_request_additional_metrics_item_compact_type_0 import (
     RunQueryRequestAdditionalMetricsItemCompactType0,
 )
@@ -1951,14 +2048,17 @@
 )
 from .run_query_request_additional_metrics_item_filters_item_operator import (
     RunQueryRequestAdditionalMetricsItemFiltersItemOperator,
 )
 from .run_query_request_additional_metrics_item_filters_item_target import (
     RunQueryRequestAdditionalMetricsItemFiltersItemTarget,
 )
+from .run_query_request_additional_metrics_item_format import (
+    RunQueryRequestAdditionalMetricsItemFormat,
+)
 from .run_query_request_additional_metrics_item_type import (
     RunQueryRequestAdditionalMetricsItemType,
 )
 from .run_query_request_filters import RunQueryRequestFilters
 from .run_query_request_sorts_item import RunQueryRequestSortsItem
 from .run_query_request_table_calculations_item import (
     RunQueryRequestTableCalculationsItem,
@@ -1971,14 +2071,24 @@
 )
 from .run_query_request_table_calculations_item_format_separator import (
     RunQueryRequestTableCalculationsItemFormatSeparator,
 )
 from .run_query_request_table_calculations_item_format_type import (
     RunQueryRequestTableCalculationsItemFormatType,
 )
+from .run_sql_query_json_body import RunSqlQueryJsonBody
+from .run_sql_query_response_200 import RunSqlQueryResponse200
+from .run_sql_query_response_200_results import RunSqlQueryResponse200Results
+from .run_sql_query_response_200_results_fields import (
+    RunSqlQueryResponse200ResultsFields,
+)
+from .run_sql_query_response_200_results_rows_item import (
+    RunSqlQueryResponse200ResultsRowsItem,
+)
+from .run_sql_query_response_200_status import RunSqlQueryResponse200Status
 from .scheduled_jobs import ScheduledJobs
 from .scheduler_and_targets import SchedulerAndTargets
 from .scheduler_and_targets_targets_item_type_0 import (
     SchedulerAndTargetsTargetsItemType0,
 )
 from .scheduler_and_targets_targets_item_type_1 import (
     SchedulerAndTargetsTargetsItemType1,
@@ -2287,16 +2397,33 @@
 from .update_space_response_200_results_queries_item_updated_by_user import (
     UpdateSpaceResponse200ResultsQueriesItemUpdatedByUser,
 )
 from .update_space_response_200_results_queries_item_validation_errors_item import (
     UpdateSpaceResponse200ResultsQueriesItemValidationErrorsItem,
 )
 from .update_space_response_200_status import UpdateSpaceResponse200Status
+from .update_user_attribute_json_body import UpdateUserAttributeJsonBody
+from .update_user_attribute_json_body_users_item import (
+    UpdateUserAttributeJsonBodyUsersItem,
+)
+from .update_user_attribute_response_200 import UpdateUserAttributeResponse200
+from .update_user_attribute_response_200_results import (
+    UpdateUserAttributeResponse200Results,
+)
+from .update_user_attribute_response_200_results_users_item import (
+    UpdateUserAttributeResponse200ResultsUsersItem,
+)
+from .update_user_attribute_response_200_status import (
+    UpdateUserAttributeResponse200Status,
+)
 from .updated_by_user import UpdatedByUser
 from .user_allowed_organization import UserAllowedOrganization
+from .user_attribute import UserAttribute
+from .user_attribute_users_item import UserAttributeUsersItem
+from .user_attribute_value import UserAttributeValue
 from .validate_project_json_body import ValidateProjectJsonBody
 from .validate_project_response_200 import ValidateProjectResponse200
 from .validate_project_response_200_results import ValidateProjectResponse200Results
 from .validate_project_response_200_status import ValidateProjectResponse200Status
 from .validation_error_chart_response import ValidationErrorChartResponse
 from .validation_error_chart_response_chart_type import (
     ValidationErrorChartResponseChartType,
@@ -2370,14 +2497,15 @@
 __all__ = (
     "AdditionalMetric",
     "AdditionalMetricCompactType0",
     "AdditionalMetricCompactType1",
     "AdditionalMetricFiltersItem",
     "AdditionalMetricFiltersItemOperator",
     "AdditionalMetricFiltersItemTarget",
+    "AdditionalMetricFormat",
     "AdditionalMetricType",
     "AddSpaceShare",
     "AddSpaceShareToUserJsonBody",
     "AddSpaceShareToUserResponse200",
     "AddSpaceShareToUserResponse200Status",
     "AddUserToGroupResponse200",
     "AddUserToGroupResponse200Status",
@@ -2393,14 +2521,18 @@
     "AllowedEmailDomainsRoleType1",
     "AllowedEmailDomainsRoleType2",
     "AllowedEmailDomainsRoleType3",
     "ApiChartSummaryListResponse",
     "ApiChartSummaryListResponseResultsItem",
     "ApiChartSummaryListResponseResultsItemChartType",
     "ApiChartSummaryListResponseStatus",
+    "ApiCreateUserAttributeResponse",
+    "ApiCreateUserAttributeResponseResults",
+    "ApiCreateUserAttributeResponseResultsUsersItem",
+    "ApiCreateUserAttributeResponseStatus",
     "ApiCsvUrlResponse",
     "ApiCsvUrlResponseResults",
     "ApiCsvUrlResponseStatus",
     "ApiDbtCloudIntegrationSettings",
     "ApiDbtCloudIntegrationSettingsResults",
     "ApiDbtCloudIntegrationSettingsStatus",
     "ApiDbtCloudMetrics",
@@ -2525,14 +2657,15 @@
     "ApiRunQueryResponseResultsMetricQuery",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItem",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType0",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType1",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItem",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItemOperator",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItemTarget",
+    "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat",
     "ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemType",
     "ApiRunQueryResponseResultsMetricQueryFilters",
     "ApiRunQueryResponseResultsMetricQueryFiltersDimensionsType0",
     "ApiRunQueryResponseResultsMetricQueryFiltersDimensionsType1",
     "ApiRunQueryResponseResultsMetricQueryFiltersMetricsType0",
     "ApiRunQueryResponseResultsMetricQueryFiltersMetricsType1",
     "ApiRunQueryResponseResultsMetricQuerySortsItem",
@@ -2581,22 +2714,29 @@
     "ApiSpaceResponseResultsQueriesItemChartType",
     "ApiSpaceResponseResultsQueriesItemUpdatedByUser",
     "ApiSpaceResponseResultsQueriesItemValidationErrorsItem",
     "ApiSpaceResponseStatus",
     "ApiSpaceSummaryListResponse",
     "ApiSpaceSummaryListResponseResultsItem",
     "ApiSpaceSummaryListResponseStatus",
+    "ApiSqlQueryResults",
+    "ApiSqlQueryResultsFields",
+    "ApiSqlQueryResultsRowsItem",
     "ApiSshKeyPairResponse",
     "ApiSshKeyPairResponseResults",
     "ApiSshKeyPairResponseStatus",
     "ApiSuccessEmpty",
     "ApiSuccessEmptyStatus",
     "ApiUserAllowedOrganizationsResponse",
     "ApiUserAllowedOrganizationsResponseResultsItem",
     "ApiUserAllowedOrganizationsResponseStatus",
+    "ApiUserAttributesResponse",
+    "ApiUserAttributesResponseResultsItem",
+    "ApiUserAttributesResponseResultsItemUsersItem",
+    "ApiUserAttributesResponseStatus",
     "ApiValidateResponse",
     "ApiValidateResponseResultsItemType0",
     "ApiValidateResponseResultsItemType0ChartType",
     "ApiValidateResponseResultsItemType0ErrorType",
     "ApiValidateResponseResultsItemType0Source",
     "ApiValidateResponseResultsItemType1",
     "ApiValidateResponseResultsItemType1ErrorType",
@@ -2660,14 +2800,23 @@
     "CreateSpaceInProjectResponse200ResultsQueriesItemChartType",
     "CreateSpaceInProjectResponse200ResultsQueriesItemUpdatedByUser",
     "CreateSpaceInProjectResponse200ResultsQueriesItemValidationErrorsItem",
     "CreateSpaceInProjectResponse200Status",
     "CreateSshKeyPairResponse201",
     "CreateSshKeyPairResponse201Results",
     "CreateSshKeyPairResponse201Status",
+    "CreateUserAttribute",
+    "CreateUserAttributeJsonBody",
+    "CreateUserAttributeJsonBodyUsersItem",
+    "CreateUserAttributeResponse200",
+    "CreateUserAttributeResponse200Results",
+    "CreateUserAttributeResponse200ResultsUsersItem",
+    "CreateUserAttributeResponse200Status",
+    "CreateUserAttributeUsersItem",
+    "CreateUserAttributeValue",
     "DashboardBasicDetails",
     "DashboardBasicDetailsUpdatedByUser",
     "DashboardBasicDetailsValidationErrorsItem",
     "DashboardScheduler",
     "DashboardSchedulerFormat",
     "DashboardSchedulerOptionsType0",
     "DashboardSchedulerOptionsType0LimitType1",
@@ -2747,14 +2896,15 @@
     "FilterGroupResponseType0",
     "FilterGroupResponseType1",
     "Filters",
     "FiltersDimensionsType0",
     "FiltersDimensionsType1",
     "FiltersMetricsType0",
     "FiltersMetricsType1",
+    "Format",
     "GetCsvUrlResponse200",
     "GetCsvUrlResponse200Results",
     "GetCsvUrlResponse200Status",
     "GetDbtCloudIntegrationSettingsResponse200",
     "GetDbtCloudIntegrationSettingsResponse200Results",
     "GetDbtCloudIntegrationSettingsResponse200Status",
     "GetDbtCloudMetricsResponse200",
@@ -2782,14 +2932,18 @@
     "GetLatestValidationResultsResponse200ResultsItemType2",
     "GetLatestValidationResultsResponse200ResultsItemType2ErrorType",
     "GetLatestValidationResultsResponse200ResultsItemType2Source",
     "GetLatestValidationResultsResponse200Status",
     "GetMyOrganizationResponse200",
     "GetMyOrganizationResponse200Results",
     "GetMyOrganizationResponse200Status",
+    "GetOrganizationMemberByUuidResponse200",
+    "GetOrganizationMemberByUuidResponse200Results",
+    "GetOrganizationMemberByUuidResponse200ResultsRole",
+    "GetOrganizationMemberByUuidResponse200Status",
     "GetPinnedItemsResponse200",
     "GetPinnedItemsResponse200ResultsItemType0",
     "GetPinnedItemsResponse200ResultsItemType0Data",
     "GetPinnedItemsResponse200ResultsItemType0DataUpdatedByUser",
     "GetPinnedItemsResponse200ResultsItemType0DataValidationErrorsItem",
     "GetPinnedItemsResponse200ResultsItemType0Type",
     "GetPinnedItemsResponse200ResultsItemType1",
@@ -2888,14 +3042,18 @@
     "GetSpaceResponse200ResultsDashboardsItemUpdatedByUser",
     "GetSpaceResponse200ResultsDashboardsItemValidationErrorsItem",
     "GetSpaceResponse200ResultsQueriesItem",
     "GetSpaceResponse200ResultsQueriesItemChartType",
     "GetSpaceResponse200ResultsQueriesItemUpdatedByUser",
     "GetSpaceResponse200ResultsQueriesItemValidationErrorsItem",
     "GetSpaceResponse200Status",
+    "GetUserAttributesResponse200",
+    "GetUserAttributesResponse200ResultsItem",
+    "GetUserAttributesResponse200ResultsItemUsersItem",
+    "GetUserAttributesResponse200Status",
     "GrantProjectAccessToUserJsonBody",
     "GrantProjectAccessToUserJsonBodyRole",
     "GrantProjectAccessToUserResponse200",
     "GrantProjectAccessToUserResponse200Status",
     "Group",
     "GroupMember",
     "JoinOrganizationResponse200",
@@ -2938,14 +3096,15 @@
     "MetricQueryResponse",
     "MetricQueryResponseAdditionalMetricsItem",
     "MetricQueryResponseAdditionalMetricsItemCompactType0",
     "MetricQueryResponseAdditionalMetricsItemCompactType1",
     "MetricQueryResponseAdditionalMetricsItemFiltersItem",
     "MetricQueryResponseAdditionalMetricsItemFiltersItemOperator",
     "MetricQueryResponseAdditionalMetricsItemFiltersItemTarget",
+    "MetricQueryResponseAdditionalMetricsItemFormat",
     "MetricQueryResponseAdditionalMetricsItemType",
     "MetricQueryResponseFilters",
     "MetricQueryResponseFiltersDimensionsType0",
     "MetricQueryResponseFiltersDimensionsType1",
     "MetricQueryResponseFiltersMetricsType0",
     "MetricQueryResponseFiltersMetricsType1",
     "MetricQueryResponseSortsItem",
@@ -2980,14 +3139,16 @@
     "OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesType",
     "OmitCreateSnowflakeCredentialsSensitiveCredentialsFieldNames",
     "OmitCreateSnowflakeCredentialsSensitiveCredentialsFieldNamesStartOfWeek",
     "OmitCreateSnowflakeCredentialsSensitiveCredentialsFieldNamesType",
     "OmitCreateTrinoCredentialsSensitiveCredentialsFieldNames",
     "OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek",
     "OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesType",
+    "OmitUserAttributeUuidOrCreatedAtOrOrganizationUuidOrUsers",
+    "OmitUserAttributeValueEmail",
     "OmitValidationResponseBaseName",
     "OmitValidationResponseBaseNameErrorType",
     "OmitValidationResponseBaseNameSource",
     "Organization",
     "OrganizationMemberProfile",
     "OrganizationMemberProfileRole",
     "OrganizationMemberProfileUpdate",
@@ -3038,21 +3199,23 @@
     "PickGroupName",
     "PickOrganizationName",
     "PickResourceViewItemAtDataUuidOrPinnedListOrder",
     "PickSavedChartUuidOrNameOrDescriptionOrSpaceNameOrSpaceUuidOrProjectUuidOrOrganizationUuidOrPinnedListUuid",
     "PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrder",
     "PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrderUpdatedByUser",
     "PickShareUrlPathOrParams",
-    "PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivate",
+    "PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivateOrPinnedListUuidOrPinnedListOrder",
     "PickSpaceProjectUuidOrUuidOrNameOrIsPrivateOrPinnedListUuidOrPinnedListOrderOrOrganizationUuid",
     "PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrors",
     "PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrorsChartType",
     "PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrorsUpdatedByUser",
     "PickSpaceQueryUuidOrNameOrChartTypeOrFirstViewedAtOrViewsOrPinnedListUuidOrPinnedListOrderOrSpaceUuidOrDescriptionOrUpdatedAtOrUpdatedByUserOrValidationErrorsValidationErrorsItem",
     "PickSshKeyPairPublicKey",
+    "PickUserAttributeExcludeKeyofUserAttributeUuidOrCreatedAtOrOrganizationUuidOrUsers",
+    "PickUserAttributeValueExcludeKeyofUserAttributeValueEmail",
     "PickValidationResponseBaseExcludeKeyofValidationResponseBaseName",
     "PickValidationResponseBaseExcludeKeyofValidationResponseBaseNameErrorType",
     "PickValidationResponseBaseExcludeKeyofValidationResponseBaseNameSource",
     "PickValidationResponseErrorOrCreatedAtOrValidationId",
     "PinnedItemsItemType0DataUpdatedByUser",
     "PinnedItemsItemType0DataValidationErrorsItem",
     "PinnedItemsItemType0Type",
@@ -3073,14 +3236,15 @@
     "PostChartResultsResponse200ResultsMetricQuery",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItem",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget",
+    "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat",
     "PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemType",
     "PostChartResultsResponse200ResultsMetricQueryFilters",
     "PostChartResultsResponse200ResultsMetricQueryFiltersDimensionsType0",
     "PostChartResultsResponse200ResultsMetricQueryFiltersDimensionsType1",
     "PostChartResultsResponse200ResultsMetricQueryFiltersMetricsType0",
     "PostChartResultsResponse200ResultsMetricQueryFiltersMetricsType1",
     "PostChartResultsResponse200ResultsMetricQuerySortsItem",
@@ -3089,58 +3253,22 @@
     "PostChartResultsResponse200ResultsMetricQueryTableCalculationsItemFormatCompact",
     "PostChartResultsResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator",
     "PostChartResultsResponse200ResultsMetricQueryTableCalculationsItemFormatType",
     "PostChartResultsResponse200Status",
     "PostgresCredentials",
     "PostgresCredentialsStartOfWeek",
     "PostgresCredentialsType",
-    "PostRunQueryJsonBody",
-    "PostRunQueryJsonBodyAdditionalMetricsItem",
-    "PostRunQueryJsonBodyAdditionalMetricsItemCompactType0",
-    "PostRunQueryJsonBodyAdditionalMetricsItemCompactType1",
-    "PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem",
-    "PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator",
-    "PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget",
-    "PostRunQueryJsonBodyAdditionalMetricsItemType",
-    "PostRunQueryJsonBodyFilters",
-    "PostRunQueryJsonBodySortsItem",
-    "PostRunQueryJsonBodyTableCalculationsItem",
-    "PostRunQueryJsonBodyTableCalculationsItemFormat",
-    "PostRunQueryJsonBodyTableCalculationsItemFormatCompact",
-    "PostRunQueryJsonBodyTableCalculationsItemFormatSeparator",
-    "PostRunQueryJsonBodyTableCalculationsItemFormatType",
-    "PostRunQueryResponse200",
-    "PostRunQueryResponse200Results",
-    "PostRunQueryResponse200ResultsMetricQuery",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget",
-    "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemType",
-    "PostRunQueryResponse200ResultsMetricQueryFilters",
-    "PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
-    "PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
-    "PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0",
-    "PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1",
-    "PostRunQueryResponse200ResultsMetricQuerySortsItem",
-    "PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem",
-    "PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat",
-    "PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact",
-    "PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator",
-    "PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType",
-    "PostRunQueryResponse200Status",
     "PostRunUnderlyingDataQueryJsonBody",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItem",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType0",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType1",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItem",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemOperator",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemTarget",
+    "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat",
     "PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemType",
     "PostRunUnderlyingDataQueryJsonBodyFilters",
     "PostRunUnderlyingDataQueryJsonBodySortsItem",
     "PostRunUnderlyingDataQueryJsonBodyTableCalculationsItem",
     "PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormat",
     "PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact",
     "PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator",
@@ -3150,14 +3278,15 @@
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQuery",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget",
+    "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersMetricsType0",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersMetricsType1",
     "PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem",
@@ -3211,17 +3340,21 @@
     "ProjectWarehouseConnectionType4",
     "ProjectWarehouseConnectionType4StartOfWeek",
     "ProjectWarehouseConnectionType4Type",
     "ProjectWarehouseConnectionType5",
     "ProjectWarehouseConnectionType5StartOfWeek",
     "ProjectWarehouseConnectionType5Type",
     "RecordStringAny",
+    "RecordStringTypeDimensionType",
+    "RecordStringUnknown",
     "RedshiftCredentials",
     "RedshiftCredentialsStartOfWeek",
     "RedshiftCredentialsType",
+    "RemoveUserAttributeResponse200",
+    "RemoveUserAttributeResponse200Status",
     "RemoveUserFromGroupResponse200",
     "RemoveUserFromGroupResponse200Status",
     "ResourceViewChartItem",
     "ResourceViewChartItemData",
     "ResourceViewChartItemDataChartType",
     "ResourceViewChartItemDataUpdatedByUser",
     "ResourceViewChartItemDataValidationErrorsItem",
@@ -3238,29 +3371,75 @@
     "ResourceViewSpaceItem",
     "ResourceViewSpaceItemData",
     "ResourceViewSpaceItemType",
     "RevokeProjectAccessForUserResponse200",
     "RevokeProjectAccessForUserResponse200Status",
     "RevokeSpaceAccessForUserResponse200",
     "RevokeSpaceAccessForUserResponse200Status",
+    "RunMetricQueryJsonBody",
+    "RunMetricQueryJsonBodyAdditionalMetricsItem",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemFormat",
+    "RunMetricQueryJsonBodyAdditionalMetricsItemType",
+    "RunMetricQueryJsonBodyFilters",
+    "RunMetricQueryJsonBodySortsItem",
+    "RunMetricQueryJsonBodyTableCalculationsItem",
+    "RunMetricQueryJsonBodyTableCalculationsItemFormat",
+    "RunMetricQueryJsonBodyTableCalculationsItemFormatCompact",
+    "RunMetricQueryJsonBodyTableCalculationsItemFormatSeparator",
+    "RunMetricQueryJsonBodyTableCalculationsItemFormatType",
+    "RunMetricQueryResponse200",
+    "RunMetricQueryResponse200Results",
+    "RunMetricQueryResponse200ResultsMetricQuery",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat",
+    "RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemType",
+    "RunMetricQueryResponse200ResultsMetricQueryFilters",
+    "RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
+    "RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
+    "RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0",
+    "RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1",
+    "RunMetricQueryResponse200ResultsMetricQuerySortsItem",
+    "RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem",
+    "RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat",
+    "RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact",
+    "RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator",
+    "RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType",
+    "RunMetricQueryResponse200Status",
     "RunQueryRequest",
     "RunQueryRequestAdditionalMetricsItem",
     "RunQueryRequestAdditionalMetricsItemCompactType0",
     "RunQueryRequestAdditionalMetricsItemCompactType1",
     "RunQueryRequestAdditionalMetricsItemFiltersItem",
     "RunQueryRequestAdditionalMetricsItemFiltersItemOperator",
     "RunQueryRequestAdditionalMetricsItemFiltersItemTarget",
+    "RunQueryRequestAdditionalMetricsItemFormat",
     "RunQueryRequestAdditionalMetricsItemType",
     "RunQueryRequestFilters",
     "RunQueryRequestSortsItem",
     "RunQueryRequestTableCalculationsItem",
     "RunQueryRequestTableCalculationsItemFormat",
     "RunQueryRequestTableCalculationsItemFormatCompact",
     "RunQueryRequestTableCalculationsItemFormatSeparator",
     "RunQueryRequestTableCalculationsItemFormatType",
+    "RunSqlQueryJsonBody",
+    "RunSqlQueryResponse200",
+    "RunSqlQueryResponse200Results",
+    "RunSqlQueryResponse200ResultsFields",
+    "RunSqlQueryResponse200ResultsRowsItem",
+    "RunSqlQueryResponse200Status",
     "ScheduledJobs",
     "SchedulerAndTargets",
     "SchedulerAndTargetsTargetsItemType0",
     "SchedulerAndTargetsTargetsItemType1",
     "SchedulerBase",
     "SchedulerBaseFormat",
     "SchedulerBaseOptionsType0",
@@ -3424,15 +3603,24 @@
     "UpdateSpaceResponse200ResultsDashboardsItemUpdatedByUser",
     "UpdateSpaceResponse200ResultsDashboardsItemValidationErrorsItem",
     "UpdateSpaceResponse200ResultsQueriesItem",
     "UpdateSpaceResponse200ResultsQueriesItemChartType",
     "UpdateSpaceResponse200ResultsQueriesItemUpdatedByUser",
     "UpdateSpaceResponse200ResultsQueriesItemValidationErrorsItem",
     "UpdateSpaceResponse200Status",
+    "UpdateUserAttributeJsonBody",
+    "UpdateUserAttributeJsonBodyUsersItem",
+    "UpdateUserAttributeResponse200",
+    "UpdateUserAttributeResponse200Results",
+    "UpdateUserAttributeResponse200ResultsUsersItem",
+    "UpdateUserAttributeResponse200Status",
     "UserAllowedOrganization",
+    "UserAttribute",
+    "UserAttributeUsersItem",
+    "UserAttributeValue",
     "ValidateProjectJsonBody",
     "ValidateProjectResponse200",
     "ValidateProjectResponse200Results",
     "ValidateProjectResponse200Status",
     "ValidationErrorChartResponse",
     "ValidationErrorChartResponseChartType",
     "ValidationErrorChartResponseErrorType",
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/add_space_share.py` & `lightdash_client_python-0.692.1/lightdash_client/models/add_space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/add_space_share_to_user_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/add_space_share_to_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/add_user_to_group_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/add_user_to_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric.py` & `lightdash_client_python-0.692.1/lightdash_client/models/additional_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.additional_metric_compact_type_0 import AdditionalMetricCompactType0
 from ..models.additional_metric_compact_type_1 import AdditionalMetricCompactType1
+from ..models.additional_metric_format import AdditionalMetricFormat
 from ..models.additional_metric_type import AdditionalMetricType
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.additional_metric_filters_item import AdditionalMetricFiltersItem
 
 
@@ -23,15 +24,15 @@
         table (str):
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
         compact (Union[AdditionalMetricCompactType0, AdditionalMetricCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        format_ (Union[Unset, AdditionalMetricFormat]):
         index (Union[Unset, float]):
         filters (Union[Unset, List['AdditionalMetricFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
     type: AdditionalMetricType
@@ -39,15 +40,15 @@
     table: str
     name: str
     label: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[AdditionalMetricCompactType0, AdditionalMetricCompactType1, Unset] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, AdditionalMetricFormat] = UNSET
     index: Union[Unset, float] = UNSET
     filters: Union[Unset, List["AdditionalMetricFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
@@ -69,15 +70,18 @@
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -164,15 +168,20 @@
             else:
                 compact_type_1 = AdditionalMetricCompactType1(_compact_type_1)
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, AdditionalMetricFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = AdditionalMetricFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
             filters_item = AdditionalMetricFiltersItem.from_dict(filters_item_data)
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_filters_item_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/additional_metric_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains.py` & `lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/allowed_email_domains_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_chart_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_chart_summary_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_csv_url_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_csv_url_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_integration_settings_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results_otp.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_email_status_response_results_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_error_payload.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload_error.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_error_payload_error.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_group_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_group_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_group_members_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_group_members_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_group_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_group_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_group_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_group_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_job_scheduled_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_job_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_job_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profile_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profiles.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_member_profiles_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_projects.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_projects_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_organization_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_pinned_items_results_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_access_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_access_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 from ..models.api_run_query_response_results_metric_query_additional_metrics_item_compact_type_0 import (
     ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType0,
 )
 from ..models.api_run_query_response_results_metric_query_additional_metrics_item_compact_type_1 import (
     ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType1,
 )
+from ..models.api_run_query_response_results_metric_query_additional_metrics_item_format import (
+    ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat,
+)
 from ..models.api_run_query_response_results_metric_query_additional_metrics_item_type import (
     ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.api_run_query_response_results_metric_query_additional_metrics_item_filters_item import (
@@ -32,15 +35,15 @@
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
         compact (Union[ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType0,
             ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        format_ (Union[Unset, ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
         filters (Union[Unset, List['ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
     type: ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemType
@@ -52,15 +55,15 @@
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
         ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType0,
         ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType1,
         Unset,
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
     filters: Union[Unset, List["ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
@@ -82,15 +85,18 @@
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -187,15 +193,20 @@
             else:
                 compact_type_1 = ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemCompactType1(_compact_type_1)
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
             filters_item = ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItem.from_dict(
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduled_jobs_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_users_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_scheduler_logs_response_results_users_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_share_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_share_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_share_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_share_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_slack_channels_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_slack_channels_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_space_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/user_allowed_organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,62 @@
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ApiSpaceSummaryListResponseResultsItem")
+T = TypeVar("T", bound="UserAllowedOrganization")
 
 
 @attr.s(auto_attribs=True)
-class ApiSpaceSummaryListResponseResultsItem:
+class UserAllowedOrganization:
     """
     Attributes:
+        members_count (float):
         name (str):
         organization_uuid (str):
-        uuid (str):
-        project_uuid (str):
-        is_private (bool):
-        access (List[str]):
     """
 
+    members_count: float
     name: str
     organization_uuid: str
-    uuid: str
-    project_uuid: str
-    is_private: bool
-    access: List[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        members_count = self.members_count
         name = self.name
         organization_uuid = self.organization_uuid
-        uuid = self.uuid
-        project_uuid = self.project_uuid
-        is_private = self.is_private
-        access = self.access
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "membersCount": members_count,
                 "name": name,
                 "organizationUuid": organization_uuid,
-                "uuid": uuid,
-                "projectUuid": project_uuid,
-                "isPrivate": is_private,
-                "access": access,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        members_count = d.pop("membersCount")
+
         name = d.pop("name")
 
         organization_uuid = d.pop("organizationUuid")
 
-        uuid = d.pop("uuid")
-
-        project_uuid = d.pop("projectUuid")
-
-        is_private = d.pop("isPrivate")
-
-        access = cast(List[str], d.pop("access"))
-
-        api_space_summary_list_response_results_item = cls(
+        user_allowed_organization = cls(
+            members_count=members_count,
             name=name,
             organization_uuid=organization_uuid,
-            uuid=uuid,
-            project_uuid=project_uuid,
-            is_private=is_private,
-            access=access,
         )
 
-        api_space_summary_list_response_results_item.additional_properties = d
-        return api_space_summary_list_response_results_item
+        user_allowed_organization.additional_properties = d
+        return user_allowed_organization
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_ssh_key_pair_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_success_empty.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_success_empty.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_user_allowed_organizations_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_validate_response_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/api_validation_dismiss_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials.py` & `lightdash_client_python-0.692.1/lightdash_client/models/bigquery_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/bigquery_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler.py` & `lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/chart_scheduler_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/chart_summary.py` & `lightdash_client_python-0.692.1/lightdash_client/models/chart_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/conditional_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/conditional_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_group_in_organization_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_organization_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_organization_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_project_member.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_share_url_response_201_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_json_body_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_ssh_key_pair_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_ssh_key_pair_response_201_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dashboard_basic_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dashboard_basic_details_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dashboard_basic_details_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dashboard_scheduler_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials.py` & `lightdash_client_python-0.692.1/lightdash_client/models/databricks_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/databricks_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_bit_bucket_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_ide_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_ide_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_integration.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_integration.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metric.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_cloud_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_github_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_github_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_gitlab_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_gitlab_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_local_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_local_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_none_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_none_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_0_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_2_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_3_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_4_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_5_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_6_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_config_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_environment_variable.py` & `lightdash_client_python-0.692.1/lightdash_client/models/dbt_project_environment_variable.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_group_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_me_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_me_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_my_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_my_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_organization_member_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_organization_member_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_scheduler_response_201.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_space_response_204.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_space_response_204.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/delete_validation_dismiss_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/delete_validation_dismiss_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password.py` & `lightdash_client_python-0.692.1/lightdash_client/models/email_one_time_password.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password_expiring.py` & `lightdash_client_python-0.692.1/lightdash_client/models/email_one_time_password_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/email_status.py` & `lightdash_client_python-0.692.1/lightdash_client/models/email_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring.py` & `lightdash_client_python-0.692.1/lightdash_client/models/email_status_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring_otp.py` & `lightdash_client_python-0.692.1/lightdash_client/models/email_status_expiring_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/email_status_otp.py` & `lightdash_client_python-0.692.1/lightdash_client/models/email_status_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filter_group_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filter_group_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_csv_url_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_csv_url_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results_otp.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_email_verification_status_response_200_results_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_group_members_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_group_members_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_group_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_my_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_my_organization_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_access_list_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_access_list_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduled_jobs_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_job_status_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_job_status_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_share_url_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_share_url_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_slack_channels_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_slack_channels_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/grant_project_access_to_user_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/grant_project_access_to_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/group.py` & `lightdash_client_python-0.692.1/lightdash_client/models/group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/group_member.py` & `lightdash_client_python-0.692.1/lightdash_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/join_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/join_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_charts_in_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_charts_in_project_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_groups_in_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_groups_in_organization_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_my_available_organizations_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_my_available_organizations_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_members_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_members_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_projects_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_organization_projects_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/list_spaces_in_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200_results_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_member_profile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,86 @@
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ListSpacesInProjectResponse200ResultsItem")
+from ..models.project_member_profile_role import ProjectMemberProfileRole
+
+T = TypeVar("T", bound="ProjectMemberProfile")
 
 
 @attr.s(auto_attribs=True)
-class ListSpacesInProjectResponse200ResultsItem:
+class ProjectMemberProfile:
     """
     Attributes:
-        name (str):
-        organization_uuid (str):
-        uuid (str):
+        last_name (str):
+        first_name (str):
+        email (str):
+        role (ProjectMemberProfileRole):
         project_uuid (str):
-        is_private (bool):
-        access (List[str]):
+        user_uuid (str):
     """
 
-    name: str
-    organization_uuid: str
-    uuid: str
+    last_name: str
+    first_name: str
+    email: str
+    role: ProjectMemberProfileRole
     project_uuid: str
-    is_private: bool
-    access: List[str]
+    user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        organization_uuid = self.organization_uuid
-        uuid = self.uuid
+        last_name = self.last_name
+        first_name = self.first_name
+        email = self.email
+        role = self.role.value
+
         project_uuid = self.project_uuid
-        is_private = self.is_private
-        access = self.access
+        user_uuid = self.user_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
-                "organizationUuid": organization_uuid,
-                "uuid": uuid,
+                "lastName": last_name,
+                "firstName": first_name,
+                "email": email,
+                "role": role,
                 "projectUuid": project_uuid,
-                "isPrivate": is_private,
-                "access": access,
+                "userUuid": user_uuid,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
+        last_name = d.pop("lastName")
 
-        organization_uuid = d.pop("organizationUuid")
+        first_name = d.pop("firstName")
 
-        uuid = d.pop("uuid")
+        email = d.pop("email")
 
-        project_uuid = d.pop("projectUuid")
+        role = ProjectMemberProfileRole(d.pop("role"))
 
-        is_private = d.pop("isPrivate")
+        project_uuid = d.pop("projectUuid")
 
-        access = cast(List[str], d.pop("access"))
+        user_uuid = d.pop("userUuid")
 
-        list_spaces_in_project_response_200_results_item = cls(
-            name=name,
-            organization_uuid=organization_uuid,
-            uuid=uuid,
+        project_member_profile = cls(
+            last_name=last_name,
+            first_name=first_name,
+            email=email,
+            role=role,
             project_uuid=project_uuid,
-            is_private=is_private,
-            access=access,
+            user_uuid=user_uuid,
         )
 
-        list_spaces_in_project_response_200_results_item.additional_properties = d
-        return list_spaces_in_project_response_200_results_item
+        project_member_profile.additional_properties = d
+        return project_member_profile
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_filter_rule.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_filter_rule_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_filter_rule_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 from ..models.metric_query_response_additional_metrics_item_compact_type_0 import (
     MetricQueryResponseAdditionalMetricsItemCompactType0,
 )
 from ..models.metric_query_response_additional_metrics_item_compact_type_1 import (
     MetricQueryResponseAdditionalMetricsItemCompactType1,
 )
+from ..models.metric_query_response_additional_metrics_item_format import (
+    MetricQueryResponseAdditionalMetricsItemFormat,
+)
 from ..models.metric_query_response_additional_metrics_item_type import (
     MetricQueryResponseAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.metric_query_response_additional_metrics_item_filters_item import (
@@ -32,15 +35,15 @@
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
         compact (Union[MetricQueryResponseAdditionalMetricsItemCompactType0,
             MetricQueryResponseAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        format_ (Union[Unset, MetricQueryResponseAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
         filters (Union[Unset, List['MetricQueryResponseAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
     type: MetricQueryResponseAdditionalMetricsItemType
@@ -52,15 +55,15 @@
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
         MetricQueryResponseAdditionalMetricsItemCompactType0,
         MetricQueryResponseAdditionalMetricsItemCompactType1,
         Unset,
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, MetricQueryResponseAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
     filters: Union[Unset, List["MetricQueryResponseAdditionalMetricsItemFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
@@ -82,15 +85,18 @@
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -185,15 +191,20 @@
             else:
                 compact_type_1 = MetricQueryResponseAdditionalMetricsItemCompactType1(_compact_type_1)
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, MetricQueryResponseAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = MetricQueryResponseAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
             filters_item = MetricQueryResponseAdditionalMetricsItemFiltersItem.from_dict(filters_item_data)
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/metric_query_response_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name.py` & `lightdash_client_python-0.692.1/lightdash_client/models/omit_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/organization.py` & `lightdash_client_python-0.692.1/lightdash_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile.py` & `lightdash_client_python-0.692.1/lightdash_client/models/organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_update.py` & `lightdash_client_python-0.692.1/lightdash_client/models/organization_member_profile_update.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/organization_project.py` & `lightdash_client_python-0.692.1/lightdash_client/models/organization_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py` & `lightdash_client_python-0.692.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_group_name.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_group_name.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_organization_name.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_organization_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_share_url_path_or_params.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,57 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivate")
+T = TypeVar("T", bound="PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivateOrPinnedListUuidOrPinnedListOrder")
 
 
 @attr.s(auto_attribs=True)
-class PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivate:
+class PickSpaceOrganizationUuidOrProjectUuidOrUuidOrNameOrIsPrivateOrPinnedListUuidOrPinnedListOrder:
     """From T, pick a set of properties whose keys are in the union K
 
     Attributes:
         name (str):
         organization_uuid (str):
         uuid (str):
         project_uuid (str):
         is_private (bool):
+        pinned_list_uuid (Optional[str]):
+        pinned_list_order (Optional[float]):
     """
 
     name: str
     organization_uuid: str
     uuid: str
     project_uuid: str
     is_private: bool
+    pinned_list_uuid: Optional[str]
+    pinned_list_order: Optional[float]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         organization_uuid = self.organization_uuid
         uuid = self.uuid
         project_uuid = self.project_uuid
         is_private = self.is_private
+        pinned_list_uuid = self.pinned_list_uuid
+        pinned_list_order = self.pinned_list_order
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
                 "organizationUuid": organization_uuid,
                 "uuid": uuid,
                 "projectUuid": project_uuid,
                 "isPrivate": is_private,
+                "pinnedListUuid": pinned_list_uuid,
+                "pinnedListOrder": pinned_list_order,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -54,24 +62,32 @@
 
         uuid = d.pop("uuid")
 
         project_uuid = d.pop("projectUuid")
 
         is_private = d.pop("isPrivate")
 
-        pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private = cls(
+        pinned_list_uuid = d.pop("pinnedListUuid")
+
+        pinned_list_order = d.pop("pinnedListOrder")
+
+        pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order = cls(
             name=name,
             organization_uuid=organization_uuid,
             uuid=uuid,
             project_uuid=project_uuid,
             is_private=is_private,
+            pinned_list_uuid=pinned_list_uuid,
+            pinned_list_order=pinned_list_order,
         )
 
-        pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.additional_properties = d
-        return pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private
+        pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order.additional_properties = (
+            d
+        )
+        return pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_ssh_key_pair_public_key.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_2_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/pinned_items_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 from ..models.post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_0 import (
     PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
 )
 from ..models.post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_1 import (
     PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
 )
+from ..models.post_chart_results_response_200_results_metric_query_additional_metrics_item_format import (
+    PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat,
+)
 from ..models.post_chart_results_response_200_results_metric_query_additional_metrics_item_type import (
     PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item import (
@@ -32,15 +35,15 @@
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
         compact (Union[PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
             PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        format_ (Union[Unset, PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
         filters (Union[Unset, List['PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
     type: PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemType
@@ -52,15 +55,15 @@
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
         PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
         PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
         Unset,
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
     filters: Union[Unset, List["PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
@@ -82,15 +85,18 @@
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -191,15 +197,20 @@
                     _compact_type_1
                 )
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
             filters_item = PostChartResultsResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem.from_dict(
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_json_body_additional_metrics_item import (
-        PostRunQueryJsonBodyAdditionalMetricsItem,
+    from ..models.run_query_request_additional_metrics_item import (
+        RunQueryRequestAdditionalMetricsItem,
     )
-    from ..models.post_run_query_json_body_filters import PostRunQueryJsonBodyFilters
-    from ..models.post_run_query_json_body_sorts_item import (
-        PostRunQueryJsonBodySortsItem,
-    )
-    from ..models.post_run_query_json_body_table_calculations_item import (
-        PostRunQueryJsonBodyTableCalculationsItem,
+    from ..models.run_query_request_filters import RunQueryRequestFilters
+    from ..models.run_query_request_sorts_item import RunQueryRequestSortsItem
+    from ..models.run_query_request_table_calculations_item import (
+        RunQueryRequestTableCalculationsItem,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryJsonBody")
+T = TypeVar("T", bound="RunQueryRequest")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBody:
-    """metricQuery for the chart to run
-
+class RunQueryRequest:
+    """
     Attributes:
-        table_calculations (List['PostRunQueryJsonBodyTableCalculationsItem']):
+        table_calculations (List['RunQueryRequestTableCalculationsItem']):
         limit (float):
-        sorts (List['PostRunQueryJsonBodySortsItem']):
-        filters (PostRunQueryJsonBodyFilters):
+        sorts (List['RunQueryRequestSortsItem']):
+        filters (RunQueryRequestFilters):
         metrics (List[str]):
         dimensions (List[str]):
         csv_limit (Union[Unset, float]):
-        additional_metrics (Union[Unset, List['PostRunQueryJsonBodyAdditionalMetricsItem']]):
+        additional_metrics (Union[Unset, List['RunQueryRequestAdditionalMetricsItem']]):
     """
 
-    table_calculations: List["PostRunQueryJsonBodyTableCalculationsItem"]
+    table_calculations: List["RunQueryRequestTableCalculationsItem"]
     limit: float
-    sorts: List["PostRunQueryJsonBodySortsItem"]
-    filters: "PostRunQueryJsonBodyFilters"
+    sorts: List["RunQueryRequestSortsItem"]
+    filters: "RunQueryRequestFilters"
     metrics: List[str]
     dimensions: List[str]
     csv_limit: Union[Unset, float] = UNSET
-    additional_metrics: Union[Unset, List["PostRunQueryJsonBodyAdditionalMetricsItem"]] = UNSET
+    additional_metrics: Union[Unset, List["RunQueryRequestAdditionalMetricsItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         table_calculations = []
         for table_calculations_item_data in self.table_calculations:
             table_calculations_item = table_calculations_item_data.to_dict()
 
@@ -91,72 +88,68 @@
         if additional_metrics is not UNSET:
             field_dict["additionalMetrics"] = additional_metrics
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_json_body_additional_metrics_item import (
-            PostRunQueryJsonBodyAdditionalMetricsItem,
-        )
-        from ..models.post_run_query_json_body_filters import (
-            PostRunQueryJsonBodyFilters,
-        )
-        from ..models.post_run_query_json_body_sorts_item import (
-            PostRunQueryJsonBodySortsItem,
+        from ..models.run_query_request_additional_metrics_item import (
+            RunQueryRequestAdditionalMetricsItem,
         )
-        from ..models.post_run_query_json_body_table_calculations_item import (
-            PostRunQueryJsonBodyTableCalculationsItem,
+        from ..models.run_query_request_filters import RunQueryRequestFilters
+        from ..models.run_query_request_sorts_item import RunQueryRequestSortsItem
+        from ..models.run_query_request_table_calculations_item import (
+            RunQueryRequestTableCalculationsItem,
         )
 
         d = src_dict.copy()
         table_calculations = []
         _table_calculations = d.pop("tableCalculations")
         for table_calculations_item_data in _table_calculations:
-            table_calculations_item = PostRunQueryJsonBodyTableCalculationsItem.from_dict(table_calculations_item_data)
+            table_calculations_item = RunQueryRequestTableCalculationsItem.from_dict(table_calculations_item_data)
 
             table_calculations.append(table_calculations_item)
 
         limit = d.pop("limit")
 
         sorts = []
         _sorts = d.pop("sorts")
         for sorts_item_data in _sorts:
-            sorts_item = PostRunQueryJsonBodySortsItem.from_dict(sorts_item_data)
+            sorts_item = RunQueryRequestSortsItem.from_dict(sorts_item_data)
 
             sorts.append(sorts_item)
 
-        filters = PostRunQueryJsonBodyFilters.from_dict(d.pop("filters"))
+        filters = RunQueryRequestFilters.from_dict(d.pop("filters"))
 
         metrics = cast(List[str], d.pop("metrics"))
 
         dimensions = cast(List[str], d.pop("dimensions"))
 
         csv_limit = d.pop("csvLimit", UNSET)
 
         additional_metrics = []
         _additional_metrics = d.pop("additionalMetrics", UNSET)
         for additional_metrics_item_data in _additional_metrics or []:
-            additional_metrics_item = PostRunQueryJsonBodyAdditionalMetricsItem.from_dict(additional_metrics_item_data)
+            additional_metrics_item = RunQueryRequestAdditionalMetricsItem.from_dict(additional_metrics_item_data)
 
             additional_metrics.append(additional_metrics_item)
 
-        post_run_query_json_body = cls(
+        run_query_request = cls(
             table_calculations=table_calculations,
             limit=limit,
             sorts=sorts,
             filters=filters,
             metrics=metrics,
             dimensions=dimensions,
             csv_limit=csv_limit,
             additional_metrics=additional_metrics,
         )
 
-        post_run_query_json_body.additional_properties = d
-        return post_run_query_json_body
+        run_query_request.additional_properties = d
+        return run_query_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.post_run_query_json_body_additional_metrics_item_compact_type_0 import (
-    PostRunQueryJsonBodyAdditionalMetricsItemCompactType0,
+from ..models.run_metric_query_json_body_additional_metrics_item_compact_type_0 import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0,
 )
-from ..models.post_run_query_json_body_additional_metrics_item_compact_type_1 import (
-    PostRunQueryJsonBodyAdditionalMetricsItemCompactType1,
+from ..models.run_metric_query_json_body_additional_metrics_item_compact_type_1 import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1,
 )
-from ..models.post_run_query_json_body_additional_metrics_item_type import (
-    PostRunQueryJsonBodyAdditionalMetricsItemType,
+from ..models.run_metric_query_json_body_additional_metrics_item_format import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemFormat,
+)
+from ..models.run_metric_query_json_body_additional_metrics_item_type import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_json_body_additional_metrics_item_filters_item import (
-        PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem,
+    from ..models.run_metric_query_json_body_additional_metrics_item_filters_item import (
+        RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryJsonBodyAdditionalMetricsItem")
+T = TypeVar("T", bound="RunMetricQueryJsonBodyAdditionalMetricsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodyAdditionalMetricsItem:
+class RunMetricQueryJsonBodyAdditionalMetricsItem:
     """
     Attributes:
-        type (PostRunQueryJsonBodyAdditionalMetricsItemType):
+        type (RunMetricQueryJsonBodyAdditionalMetricsItemType):
         sql (str):
         table (str):
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
-        compact (Union[PostRunQueryJsonBodyAdditionalMetricsItemCompactType0,
-            PostRunQueryJsonBodyAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        compact (Union[RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0,
+            RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1, Unset]):
+        format_ (Union[Unset, RunMetricQueryJsonBodyAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
-        filters (Union[Unset, List['PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem']]):
+        filters (Union[Unset, List['RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
-    type: PostRunQueryJsonBodyAdditionalMetricsItemType
+    type: RunMetricQueryJsonBodyAdditionalMetricsItemType
     sql: str
     table: str
     name: str
     label: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
-        PostRunQueryJsonBodyAdditionalMetricsItemCompactType0,
-        PostRunQueryJsonBodyAdditionalMetricsItemCompactType1,
+        RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0,
+        RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1,
         Unset,
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, RunMetricQueryJsonBodyAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
-    filters: Union[Unset, List["PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem"]] = UNSET
+    filters: Union[Unset, List["RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         sql = self.sql
@@ -72,25 +75,28 @@
         description = self.description
         hidden = self.hidden
         round_ = self.round_
         compact: Union[Unset, str]
         if isinstance(self.compact, Unset):
             compact = UNSET
 
-        elif isinstance(self.compact, PostRunQueryJsonBodyAdditionalMetricsItemCompactType0):
+        elif isinstance(self.compact, RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0):
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -129,20 +135,20 @@
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_json_body_additional_metrics_item_filters_item import (
-            PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem,
+        from ..models.run_metric_query_json_body_additional_metrics_item_filters_item import (
+            RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem,
         )
 
         d = src_dict.copy()
-        type = PostRunQueryJsonBodyAdditionalMetricsItemType(d.pop("type"))
+        type = RunMetricQueryJsonBodyAdditionalMetricsItemType(d.pop("type"))
 
         sql = d.pop("sql")
 
         table = d.pop("table")
 
         name = d.pop("name")
 
@@ -153,62 +159,67 @@
         hidden = d.pop("hidden", UNSET)
 
         round_ = d.pop("round", UNSET)
 
         def _parse_compact(
             data: object,
         ) -> Union[
-            PostRunQueryJsonBodyAdditionalMetricsItemCompactType0,
-            PostRunQueryJsonBodyAdditionalMetricsItemCompactType1,
+            RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0,
+            RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1,
             Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _compact_type_0 = data
-                compact_type_0: Union[Unset, PostRunQueryJsonBodyAdditionalMetricsItemCompactType0]
+                compact_type_0: Union[Unset, RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0]
                 if isinstance(_compact_type_0, Unset):
                     compact_type_0 = UNSET
                 else:
-                    compact_type_0 = PostRunQueryJsonBodyAdditionalMetricsItemCompactType0(_compact_type_0)
+                    compact_type_0 = RunMetricQueryJsonBodyAdditionalMetricsItemCompactType0(_compact_type_0)
 
                 return compact_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _compact_type_1 = data
-            compact_type_1: Union[Unset, PostRunQueryJsonBodyAdditionalMetricsItemCompactType1]
+            compact_type_1: Union[Unset, RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1]
             if isinstance(_compact_type_1, Unset):
                 compact_type_1 = UNSET
             else:
-                compact_type_1 = PostRunQueryJsonBodyAdditionalMetricsItemCompactType1(_compact_type_1)
+                compact_type_1 = RunMetricQueryJsonBodyAdditionalMetricsItemCompactType1(_compact_type_1)
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, RunMetricQueryJsonBodyAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = RunMetricQueryJsonBodyAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
-            filters_item = PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem.from_dict(filters_item_data)
+            filters_item = RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem.from_dict(filters_item_data)
 
             filters.append(filters_item)
 
         base_dimension_name = d.pop("baseDimensionName", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        post_run_query_json_body_additional_metrics_item = cls(
+        run_metric_query_json_body_additional_metrics_item = cls(
             type=type,
             sql=sql,
             table=table,
             name=name,
             label=label,
             description=description,
             hidden=hidden,
@@ -217,8 +228,8 @@
             format_=format_,
             index=index,
             filters=filters,
             base_dimension_name=base_dimension_name,
             uuid=uuid,
         )
 
-        return post_run_query_json_body_additional_metrics_item
+        return run_metric_query_json_body_additional_metrics_item
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_filters_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
-from ..models.post_run_query_json_body_additional_metrics_item_filters_item_operator import (
-    PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator,
+from ..models.run_metric_query_json_body_additional_metrics_item_filters_item_operator import (
+    RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_json_body_additional_metrics_item_filters_item_target import (
-        PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
+    from ..models.run_metric_query_json_body_additional_metrics_item_filters_item_target import (
+        RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem")
+T = TypeVar("T", bound="RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodyAdditionalMetricsItemFiltersItem:
+class RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItem:
     """
     Attributes:
-        operator (PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator):
+        operator (RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator):
         id (str):
-        target (PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget):
+        target (RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget):
         values (Union[Unset, List[Any]]):
         settings (Union[Unset, Any]):
     """
 
-    operator: PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator
+    operator: RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator
     id: str
-    target: "PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget"
+    target: "RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget"
     values: Union[Unset, List[Any]] = UNSET
     settings: Union[Unset, Any] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         operator = self.operator.value
 
         id = self.id
@@ -58,31 +58,31 @@
         if settings is not UNSET:
             field_dict["settings"] = settings
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_json_body_additional_metrics_item_filters_item_target import (
-            PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
+        from ..models.run_metric_query_json_body_additional_metrics_item_filters_item_target import (
+            RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget,
         )
 
         d = src_dict.copy()
-        operator = PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(d.pop("operator"))
+        operator = RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(d.pop("operator"))
 
         id = d.pop("id")
 
-        target = PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget.from_dict(d.pop("target"))
+        target = RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemTarget.from_dict(d.pop("target"))
 
         values = cast(List[Any], d.pop("values", UNSET))
 
         settings = d.pop("settings", UNSET)
 
-        post_run_query_json_body_additional_metrics_item_filters_item = cls(
+        run_metric_query_json_body_additional_metrics_item_filters_item = cls(
             operator=operator,
             id=id,
             target=target,
             values=values,
             settings=settings,
         )
 
-        return post_run_query_json_body_additional_metrics_item_filters_item
+        return run_metric_query_json_body_additional_metrics_item_filters_item
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 
-class PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget")
+T = TypeVar("T", bound="PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemTarget")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemTarget:
+class PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemTarget:
     """
     Attributes:
         field_ref (str):
     """
 
     field_ref: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -29,20 +29,20 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         field_ref = d.pop("fieldRef")
 
-        post_run_query_json_body_additional_metrics_item_filters_item_target = cls(
+        post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target = cls(
             field_ref=field_ref,
         )
 
-        post_run_query_json_body_additional_metrics_item_filters_item_target.additional_properties = d
-        return post_run_query_json_body_additional_metrics_item_filters_item_target
+        post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.additional_properties = d
+        return post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PostRunQueryJsonBodyFilters")
+T = TypeVar("T", bound="RunMetricQueryJsonBodyFilters")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodyFilters:
+class RunMetricQueryJsonBodyFilters:
     """
     Attributes:
         metrics (Union[Unset, Any]):
         dimensions (Union[Unset, Any]):
     """
 
     metrics: Union[Unset, Any] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         metrics = d.pop("metrics", UNSET)
 
         dimensions = d.pop("dimensions", UNSET)
 
-        post_run_query_json_body_filters = cls(
+        run_metric_query_json_body_filters = cls(
             metrics=metrics,
             dimensions=dimensions,
         )
 
-        post_run_query_json_body_filters.additional_properties = d
-        return post_run_query_json_body_filters
+        run_metric_query_json_body_filters.additional_properties = d
+        return run_metric_query_json_body_filters
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_sorts_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryJsonBodySortsItem")
+T = TypeVar("T", bound="RunQueryRequestSortsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodySortsItem:
+class RunQueryRequestSortsItem:
     """
     Attributes:
         descending (bool):
         field_id (str):
     """
 
     descending: bool
@@ -35,21 +35,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         descending = d.pop("descending")
 
         field_id = d.pop("fieldId")
 
-        post_run_query_json_body_sorts_item = cls(
+        run_query_request_sorts_item = cls(
             descending=descending,
             field_id=field_id,
         )
 
-        post_run_query_json_body_sorts_item.additional_properties = d
-        return post_run_query_json_body_sorts_item
+        run_query_request_sorts_item.additional_properties = d
+        return run_query_request_sorts_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_table_calculations_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_json_body_table_calculations_item_format import (
-        PostRunQueryJsonBodyTableCalculationsItemFormat,
+    from ..models.run_metric_query_json_body_table_calculations_item_format import (
+        RunMetricQueryJsonBodyTableCalculationsItemFormat,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryJsonBodyTableCalculationsItem")
+T = TypeVar("T", bound="RunMetricQueryJsonBodyTableCalculationsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodyTableCalculationsItem:
+class RunMetricQueryJsonBodyTableCalculationsItem:
     """
     Attributes:
         sql (str):
         display_name (str):
         name (str):
-        format_ (Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormat]):
+        format_ (Union[Unset, RunMetricQueryJsonBodyTableCalculationsItemFormat]):
         index (Union[Unset, float]):
     """
 
     sql: str
     display_name: str
     name: str
-    format_: Union[Unset, "PostRunQueryJsonBodyTableCalculationsItemFormat"] = UNSET
+    format_: Union[Unset, "RunMetricQueryJsonBodyTableCalculationsItemFormat"] = UNSET
     index: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         sql = self.sql
         display_name = self.display_name
         name = self.name
@@ -55,44 +55,44 @@
         if index is not UNSET:
             field_dict["index"] = index
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_json_body_table_calculations_item_format import (
-            PostRunQueryJsonBodyTableCalculationsItemFormat,
+        from ..models.run_metric_query_json_body_table_calculations_item_format import (
+            RunMetricQueryJsonBodyTableCalculationsItemFormat,
         )
 
         d = src_dict.copy()
         sql = d.pop("sql")
 
         display_name = d.pop("displayName")
 
         name = d.pop("name")
 
         _format_ = d.pop("format", UNSET)
-        format_: Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormat]
+        format_: Union[Unset, RunMetricQueryJsonBodyTableCalculationsItemFormat]
         if isinstance(_format_, Unset):
             format_ = UNSET
         else:
-            format_ = PostRunQueryJsonBodyTableCalculationsItemFormat.from_dict(_format_)
+            format_ = RunMetricQueryJsonBodyTableCalculationsItemFormat.from_dict(_format_)
 
         index = d.pop("index", UNSET)
 
-        post_run_query_json_body_table_calculations_item = cls(
+        run_metric_query_json_body_table_calculations_item = cls(
             sql=sql,
             display_name=display_name,
             name=name,
             format_=format_,
             index=index,
         )
 
-        post_run_query_json_body_table_calculations_item.additional_properties = d
-        return post_run_query_json_body_table_calculations_item
+        run_metric_query_json_body_table_calculations_item.additional_properties = d
+        return run_metric_query_json_body_table_calculations_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.post_run_query_json_body_table_calculations_item_format_compact import (
-    PostRunQueryJsonBodyTableCalculationsItemFormatCompact,
+from ..models.post_run_underlying_data_query_json_body_table_calculations_item_format_compact import (
+    PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact,
 )
-from ..models.post_run_query_json_body_table_calculations_item_format_separator import (
-    PostRunQueryJsonBodyTableCalculationsItemFormatSeparator,
+from ..models.post_run_underlying_data_query_json_body_table_calculations_item_format_separator import (
+    PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator,
 )
-from ..models.post_run_query_json_body_table_calculations_item_format_type import (
-    PostRunQueryJsonBodyTableCalculationsItemFormatType,
+from ..models.post_run_underlying_data_query_json_body_table_calculations_item_format_type import (
+    PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PostRunQueryJsonBodyTableCalculationsItemFormat")
+T = TypeVar("T", bound="PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormat")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryJsonBodyTableCalculationsItemFormat:
+class PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormat:
     """
     Attributes:
-        type (PostRunQueryJsonBodyTableCalculationsItemFormatType):
+        type (PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType):
         suffix (Union[Unset, str]):
         prefix (Union[Unset, str]):
-        compact (Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormatCompact]):
+        compact (Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact]):
         currency (Union[Unset, str]):
-        separator (Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormatSeparator]):
+        separator (Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator]):
         round_ (Union[Unset, float]):
     """
 
-    type: PostRunQueryJsonBodyTableCalculationsItemFormatType
+    type: PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType
     suffix: Union[Unset, str] = UNSET
     prefix: Union[Unset, str] = UNSET
-    compact: Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormatCompact] = UNSET
+    compact: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact] = UNSET
     currency: Union[Unset, str] = UNSET
-    separator: Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormatSeparator] = UNSET
+    separator: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator] = UNSET
     round_: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         suffix = self.suffix
@@ -75,50 +75,50 @@
             field_dict["round"] = round_
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = PostRunQueryJsonBodyTableCalculationsItemFormatType(d.pop("type"))
+        type = PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType(d.pop("type"))
 
         suffix = d.pop("suffix", UNSET)
 
         prefix = d.pop("prefix", UNSET)
 
         _compact = d.pop("compact", UNSET)
-        compact: Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormatCompact]
+        compact: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact]
         if isinstance(_compact, Unset):
             compact = UNSET
         else:
-            compact = PostRunQueryJsonBodyTableCalculationsItemFormatCompact(_compact)
+            compact = PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact(_compact)
 
         currency = d.pop("currency", UNSET)
 
         _separator = d.pop("separator", UNSET)
-        separator: Union[Unset, PostRunQueryJsonBodyTableCalculationsItemFormatSeparator]
+        separator: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator]
         if isinstance(_separator, Unset):
             separator = UNSET
         else:
-            separator = PostRunQueryJsonBodyTableCalculationsItemFormatSeparator(_separator)
+            separator = PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator(_separator)
 
         round_ = d.pop("round", UNSET)
 
-        post_run_query_json_body_table_calculations_item_format = cls(
+        post_run_underlying_data_query_json_body_table_calculations_item_format = cls(
             type=type,
             suffix=suffix,
             prefix=prefix,
             compact=compact,
             currency=currency,
             separator=separator,
             round_=round_,
         )
 
-        post_run_query_json_body_table_calculations_item_format.additional_properties = d
-        return post_run_query_json_body_table_calculations_item_format
+        post_run_underlying_data_query_json_body_table_calculations_item_format.additional_properties = d
+        return post_run_underlying_data_query_json_body_table_calculations_item_format
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/create_user_attribute_response_200.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.post_run_query_response_200_status import PostRunQueryResponse200Status
+from ..models.create_user_attribute_response_200_status import (
+    CreateUserAttributeResponse200Status,
+)
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results import (
-        PostRunQueryResponse200Results,
+    from ..models.create_user_attribute_response_200_results import (
+        CreateUserAttributeResponse200Results,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200")
+T = TypeVar("T", bound="CreateUserAttributeResponse200")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200:
+class CreateUserAttributeResponse200:
     """
     Attributes:
-        results (PostRunQueryResponse200Results):
-        status (PostRunQueryResponse200Status):
+        results (CreateUserAttributeResponse200Results):
+        status (CreateUserAttributeResponse200Status):
     """
 
-    results: "PostRunQueryResponse200Results"
-    status: PostRunQueryResponse200Status
+    results: "CreateUserAttributeResponse200Results"
+    status: CreateUserAttributeResponse200Status
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
 
@@ -39,30 +41,30 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results import (
-            PostRunQueryResponse200Results,
+        from ..models.create_user_attribute_response_200_results import (
+            CreateUserAttributeResponse200Results,
         )
 
         d = src_dict.copy()
-        results = PostRunQueryResponse200Results.from_dict(d.pop("results"))
+        results = CreateUserAttributeResponse200Results.from_dict(d.pop("results"))
 
-        status = PostRunQueryResponse200Status(d.pop("status"))
+        status = CreateUserAttributeResponse200Status(d.pop("status"))
 
-        post_run_query_response_200 = cls(
+        create_user_attribute_response_200 = cls(
             results=results,
             status=status,
         )
 
-        post_run_query_response_200.additional_properties = d
-        return post_run_query_response_200
+        create_user_attribute_response_200.additional_properties = d
+        return create_user_attribute_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results_metric_query import (
-        PostRunQueryResponse200ResultsMetricQuery,
+    from ..models.run_metric_query_response_200_results_metric_query import (
+        RunMetricQueryResponse200ResultsMetricQuery,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200Results")
+T = TypeVar("T", bound="RunMetricQueryResponse200Results")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200Results:
+class RunMetricQueryResponse200Results:
     """
     Attributes:
         rows (List[Any]):
-        metric_query (PostRunQueryResponse200ResultsMetricQuery):
+        metric_query (RunMetricQueryResponse200ResultsMetricQuery):
     """
 
     rows: List[Any]
-    metric_query: "PostRunQueryResponse200ResultsMetricQuery"
+    metric_query: "RunMetricQueryResponse200ResultsMetricQuery"
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         rows = self.rows
 
         metric_query = self.metric_query.to_dict()
 
@@ -37,30 +37,30 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results_metric_query import (
-            PostRunQueryResponse200ResultsMetricQuery,
+        from ..models.run_metric_query_response_200_results_metric_query import (
+            RunMetricQueryResponse200ResultsMetricQuery,
         )
 
         d = src_dict.copy()
         rows = cast(List[Any], d.pop("rows"))
 
-        metric_query = PostRunQueryResponse200ResultsMetricQuery.from_dict(d.pop("metricQuery"))
+        metric_query = RunMetricQueryResponse200ResultsMetricQuery.from_dict(d.pop("metricQuery"))
 
-        post_run_query_response_200_results = cls(
+        run_metric_query_response_200_results = cls(
             rows=rows,
             metric_query=metric_query,
         )
 
-        post_run_query_response_200_results.additional_properties = d
-        return post_run_query_response_200_results
+        run_metric_query_response_200_results.additional_properties = d
+        return run_metric_query_response_200_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item import (
-        PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
+    from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item import (
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
     )
-    from ..models.post_run_query_response_200_results_metric_query_filters import (
-        PostRunQueryResponse200ResultsMetricQueryFilters,
+    from ..models.post_run_underlying_data_query_response_200_results_metric_query_filters import (
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters,
     )
-    from ..models.post_run_query_response_200_results_metric_query_sorts_item import (
-        PostRunQueryResponse200ResultsMetricQuerySortsItem,
+    from ..models.post_run_underlying_data_query_response_200_results_metric_query_sorts_item import (
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem,
     )
-    from ..models.post_run_query_response_200_results_metric_query_table_calculations_item import (
-        PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem,
+    from ..models.post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item import (
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQuery")
+T = TypeVar("T", bound="PostRunUnderlyingDataQueryResponse200ResultsMetricQuery")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQuery:
+class PostRunUnderlyingDataQueryResponse200ResultsMetricQuery:
     """
     Attributes:
-        table_calculations (List['PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem']):
+        table_calculations (List['PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem']):
         limit (float):
-        sorts (List['PostRunQueryResponse200ResultsMetricQuerySortsItem']):
-        filters (PostRunQueryResponse200ResultsMetricQueryFilters):
+        sorts (List['PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem']):
+        filters (PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters):
         metrics (List[str]):
         dimensions (List[str]):
-        additional_metrics (Union[Unset, List['PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem']]):
+        additional_metrics (Union[Unset,
+            List['PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem']]):
     """
 
-    table_calculations: List["PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem"]
+    table_calculations: List["PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem"]
     limit: float
-    sorts: List["PostRunQueryResponse200ResultsMetricQuerySortsItem"]
-    filters: "PostRunQueryResponse200ResultsMetricQueryFilters"
+    sorts: List["PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem"]
+    filters: "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters"
     metrics: List[str]
     dimensions: List[str]
-    additional_metrics: Union[Unset, List["PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem"]] = UNSET
+    additional_metrics: Union[
+        Unset, List["PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem"]
+    ] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         table_calculations = []
         for table_calculations_item_data in self.table_calculations:
             table_calculations_item = table_calculations_item_data.to_dict()
 
@@ -87,73 +90,77 @@
         if additional_metrics is not UNSET:
             field_dict["additionalMetrics"] = additional_metrics
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item import (
-            PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
+        from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item import (
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
         )
-        from ..models.post_run_query_response_200_results_metric_query_filters import (
-            PostRunQueryResponse200ResultsMetricQueryFilters,
+        from ..models.post_run_underlying_data_query_response_200_results_metric_query_filters import (
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters,
         )
-        from ..models.post_run_query_response_200_results_metric_query_sorts_item import (
-            PostRunQueryResponse200ResultsMetricQuerySortsItem,
+        from ..models.post_run_underlying_data_query_response_200_results_metric_query_sorts_item import (
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem,
         )
-        from ..models.post_run_query_response_200_results_metric_query_table_calculations_item import (
-            PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem,
+        from ..models.post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item import (
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem,
         )
 
         d = src_dict.copy()
         table_calculations = []
         _table_calculations = d.pop("tableCalculations")
         for table_calculations_item_data in _table_calculations:
-            table_calculations_item = PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem.from_dict(
-                table_calculations_item_data
+            table_calculations_item = (
+                PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem.from_dict(
+                    table_calculations_item_data
+                )
             )
 
             table_calculations.append(table_calculations_item)
 
         limit = d.pop("limit")
 
         sorts = []
         _sorts = d.pop("sorts")
         for sorts_item_data in _sorts:
-            sorts_item = PostRunQueryResponse200ResultsMetricQuerySortsItem.from_dict(sorts_item_data)
+            sorts_item = PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem.from_dict(sorts_item_data)
 
             sorts.append(sorts_item)
 
-        filters = PostRunQueryResponse200ResultsMetricQueryFilters.from_dict(d.pop("filters"))
+        filters = PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters.from_dict(d.pop("filters"))
 
         metrics = cast(List[str], d.pop("metrics"))
 
         dimensions = cast(List[str], d.pop("dimensions"))
 
         additional_metrics = []
         _additional_metrics = d.pop("additionalMetrics", UNSET)
         for additional_metrics_item_data in _additional_metrics or []:
-            additional_metrics_item = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem.from_dict(
-                additional_metrics_item_data
+            additional_metrics_item = (
+                PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem.from_dict(
+                    additional_metrics_item_data
+                )
             )
 
             additional_metrics.append(additional_metrics_item)
 
-        post_run_query_response_200_results_metric_query = cls(
+        post_run_underlying_data_query_response_200_results_metric_query = cls(
             table_calculations=table_calculations,
             limit=limit,
             sorts=sorts,
             filters=filters,
             metrics=metrics,
             dimensions=dimensions,
             additional_metrics=additional_metrics,
         )
 
-        post_run_query_response_200_results_metric_query.additional_properties = d
-        return post_run_query_response_200_results_metric_query
+        post_run_underlying_data_query_response_200_results_metric_query.additional_properties = d
+        return post_run_underlying_data_query_response_200_results_metric_query
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_0 import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
+from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0 import (
+    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
 )
-from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_1 import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
+from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1 import (
+    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
 )
-from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_type import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemType,
+from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_format import (
+    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat,
+)
+from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type import (
+    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
-        PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
+    from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem")
+T = TypeVar("T", bound="PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItem:
+class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem:
     """
     Attributes:
-        type (PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemType):
+        type (PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType):
         sql (str):
         table (str):
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
-        compact (Union[PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-            PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        compact (Union[PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1, Unset]):
+        format_ (Union[Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
-        filters (Union[Unset, List['PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem']]):
+        filters (Union[Unset,
+            List['PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
-    type: PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemType
+    type: PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType
     sql: str
     table: str
     name: str
     label: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
-        PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-        PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
+        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
         Unset,
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
-    filters: Union[Unset, List["PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem"]] = UNSET
+    filters: Union[
+        Unset, List["PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem"]
+    ] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         sql = self.sql
@@ -72,25 +78,30 @@
         description = self.description
         hidden = self.hidden
         round_ = self.round_
         compact: Union[Unset, str]
         if isinstance(self.compact, Unset):
             compact = UNSET
 
-        elif isinstance(self.compact, PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0):
+        elif isinstance(
+            self.compact, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0
+        ):
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -129,20 +140,20 @@
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
-            PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
+        from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
         )
 
         d = src_dict.copy()
-        type = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemType(d.pop("type"))
+        type = PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType(d.pop("type"))
 
         sql = d.pop("sql")
 
         table = d.pop("table")
 
         name = d.pop("name")
 
@@ -153,68 +164,83 @@
         hidden = d.pop("hidden", UNSET)
 
         round_ = d.pop("round", UNSET)
 
         def _parse_compact(
             data: object,
         ) -> Union[
-            PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-            PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
+            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
             Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _compact_type_0 = data
-                compact_type_0: Union[Unset, PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0]
+                compact_type_0: Union[
+                    Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0
+                ]
                 if isinstance(_compact_type_0, Unset):
                     compact_type_0 = UNSET
                 else:
-                    compact_type_0 = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0(
-                        _compact_type_0
+                    compact_type_0 = (
+                        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0(
+                            _compact_type_0
+                        )
                     )
 
                 return compact_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _compact_type_1 = data
-            compact_type_1: Union[Unset, PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1]
+            compact_type_1: Union[
+                Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1
+            ]
             if isinstance(_compact_type_1, Unset):
                 compact_type_1 = UNSET
             else:
-                compact_type_1 = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1(
-                    _compact_type_1
+                compact_type_1 = (
+                    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1(
+                        _compact_type_1
+                    )
                 )
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
-            filters_item = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem.from_dict(
-                filters_item_data
+            filters_item = (
+                PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem.from_dict(
+                    filters_item_data
+                )
             )
 
             filters.append(filters_item)
 
         base_dimension_name = d.pop("baseDimensionName", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        post_run_query_response_200_results_metric_query_additional_metrics_item = cls(
+        post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item = cls(
             type=type,
             sql=sql,
             table=table,
             name=name,
             label=label,
             description=description,
             hidden=hidden,
@@ -223,8 +249,8 @@
             format_=format_,
             index=index,
             filters=filters,
             base_dimension_name=base_dimension_name,
             uuid=uuid,
         )
 
-        return post_run_query_response_200_results_metric_query_additional_metrics_item
+        return post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
-from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator import (
-    PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator,
+from ..models.run_query_request_additional_metrics_item_filters_item_operator import (
+    RunQueryRequestAdditionalMetricsItemFiltersItemOperator,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target import (
-        PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
+    from ..models.run_query_request_additional_metrics_item_filters_item_target import (
+        RunQueryRequestAdditionalMetricsItemFiltersItemTarget,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem")
+T = TypeVar("T", bound="RunQueryRequestAdditionalMetricsItemFiltersItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem:
+class RunQueryRequestAdditionalMetricsItemFiltersItem:
     """
     Attributes:
-        operator (PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator):
+        operator (RunQueryRequestAdditionalMetricsItemFiltersItemOperator):
         id (str):
-        target (PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget):
+        target (RunQueryRequestAdditionalMetricsItemFiltersItemTarget):
         values (Union[Unset, List[Any]]):
         settings (Union[Unset, Any]):
     """
 
-    operator: PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator
+    operator: RunQueryRequestAdditionalMetricsItemFiltersItemOperator
     id: str
-    target: "PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget"
+    target: "RunQueryRequestAdditionalMetricsItemFiltersItemTarget"
     values: Union[Unset, List[Any]] = UNSET
     settings: Union[Unset, Any] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         operator = self.operator.value
 
         id = self.id
@@ -58,33 +58,31 @@
         if settings is not UNSET:
             field_dict["settings"] = settings
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target import (
-            PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget,
+        from ..models.run_query_request_additional_metrics_item_filters_item_target import (
+            RunQueryRequestAdditionalMetricsItemFiltersItemTarget,
         )
 
         d = src_dict.copy()
-        operator = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(d.pop("operator"))
+        operator = RunQueryRequestAdditionalMetricsItemFiltersItemOperator(d.pop("operator"))
 
         id = d.pop("id")
 
-        target = PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget.from_dict(
-            d.pop("target")
-        )
+        target = RunQueryRequestAdditionalMetricsItemFiltersItemTarget.from_dict(d.pop("target"))
 
         values = cast(List[Any], d.pop("values", UNSET))
 
         settings = d.pop("settings", UNSET)
 
-        post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item = cls(
+        run_query_request_additional_metrics_item_filters_item = cls(
             operator=operator,
             id=id,
             target=target,
             values=values,
             settings=settings,
         )
 
-        return post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item
+        return run_query_request_additional_metrics_item_filters_item
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 
-class PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget:
+class RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemTarget:
     """
     Attributes:
         field_ref (str):
     """
 
     field_ref: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -29,22 +29,22 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         field_ref = d.pop("fieldRef")
 
-        post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target = cls(
+        run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_target = cls(
             field_ref=field_ref,
         )
 
-        post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.additional_properties = (
+        run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.additional_properties = (
             d
         )
-        return post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target
+        return run_metric_query_response_200_results_metric_query_additional_metrics_item_filters_item_target
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results_metric_query_filters_dimensions_type_0 import (
-        PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
+    from ..models.run_metric_query_response_200_results_metric_query_filters_dimensions_type_0 import (
+        RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
     )
-    from ..models.post_run_query_response_200_results_metric_query_filters_dimensions_type_1 import (
-        PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1,
+    from ..models.run_metric_query_response_200_results_metric_query_filters_dimensions_type_1 import (
+        RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1,
     )
-    from ..models.post_run_query_response_200_results_metric_query_filters_metrics_type_0 import (
-        PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0,
+    from ..models.run_metric_query_response_200_results_metric_query_filters_metrics_type_0 import (
+        RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0,
     )
-    from ..models.post_run_query_response_200_results_metric_query_filters_metrics_type_1 import (
-        PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1,
+    from ..models.run_metric_query_response_200_results_metric_query_filters_metrics_type_1 import (
+        RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryFilters")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryFilters")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryFilters:
+class RunMetricQueryResponse200ResultsMetricQueryFilters:
     """
     Attributes:
-        metrics (Union['PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0',
-            'PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1', Unset]):
-        dimensions (Union['PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0',
-            'PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1', Unset]):
+        metrics (Union['RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0',
+            'RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1', Unset]):
+        dimensions (Union['RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0',
+            'RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1', Unset]):
     """
 
     metrics: Union[
-        "PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0",
-        "PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1",
+        "RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0",
+        "RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1",
         Unset,
     ] = UNSET
     dimensions: Union[
-        "PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
-        "PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
+        "RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
+        "RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
         Unset,
     ] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.post_run_query_response_200_results_metric_query_filters_dimensions_type_0 import (
-            PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
+        from ..models.run_metric_query_response_200_results_metric_query_filters_dimensions_type_0 import (
+            RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
         )
-        from ..models.post_run_query_response_200_results_metric_query_filters_metrics_type_0 import (
-            PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0,
+        from ..models.run_metric_query_response_200_results_metric_query_filters_metrics_type_0 import (
+            RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0,
         )
 
         metrics: Union[Dict[str, Any], Unset]
         if isinstance(self.metrics, Unset):
             metrics = UNSET
 
-        elif isinstance(self.metrics, PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0):
+        elif isinstance(self.metrics, RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0):
             metrics = UNSET
             if not isinstance(self.metrics, Unset):
                 metrics = self.metrics.to_dict()
 
         else:
             metrics = UNSET
             if not isinstance(self.metrics, Unset):
                 metrics = self.metrics.to_dict()
 
         dimensions: Union[Dict[str, Any], Unset]
         if isinstance(self.dimensions, Unset):
             dimensions = UNSET
 
-        elif isinstance(self.dimensions, PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0):
+        elif isinstance(self.dimensions, RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0):
             dimensions = UNSET
             if not isinstance(self.dimensions, Unset):
                 dimensions = self.dimensions.to_dict()
 
         else:
             dimensions = UNSET
             if not isinstance(self.dimensions, Unset):
@@ -88,112 +88,114 @@
         if dimensions is not UNSET:
             field_dict["dimensions"] = dimensions
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results_metric_query_filters_dimensions_type_0 import (
-            PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
+        from ..models.run_metric_query_response_200_results_metric_query_filters_dimensions_type_0 import (
+            RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0,
         )
-        from ..models.post_run_query_response_200_results_metric_query_filters_dimensions_type_1 import (
-            PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1,
+        from ..models.run_metric_query_response_200_results_metric_query_filters_dimensions_type_1 import (
+            RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1,
         )
-        from ..models.post_run_query_response_200_results_metric_query_filters_metrics_type_0 import (
-            PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0,
+        from ..models.run_metric_query_response_200_results_metric_query_filters_metrics_type_0 import (
+            RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0,
         )
-        from ..models.post_run_query_response_200_results_metric_query_filters_metrics_type_1 import (
-            PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1,
+        from ..models.run_metric_query_response_200_results_metric_query_filters_metrics_type_1 import (
+            RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1,
         )
 
         d = src_dict.copy()
 
         def _parse_metrics(
             data: object,
         ) -> Union[
-            "PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0",
-            "PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1",
+            "RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0",
+            "RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1",
             Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _metrics_type_0 = data
-                metrics_type_0: Union[Unset, PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0]
+                metrics_type_0: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0]
                 if isinstance(_metrics_type_0, Unset):
                     metrics_type_0 = UNSET
                 else:
-                    metrics_type_0 = PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0.from_dict(
+                    metrics_type_0 = RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0.from_dict(
                         _metrics_type_0
                     )
 
                 return metrics_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _metrics_type_1 = data
-            metrics_type_1: Union[Unset, PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1]
+            metrics_type_1: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1]
             if isinstance(_metrics_type_1, Unset):
                 metrics_type_1 = UNSET
             else:
-                metrics_type_1 = PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1.from_dict(_metrics_type_1)
+                metrics_type_1 = RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1.from_dict(
+                    _metrics_type_1
+                )
 
             return metrics_type_1
 
         metrics = _parse_metrics(d.pop("metrics", UNSET))
 
         def _parse_dimensions(
             data: object,
         ) -> Union[
-            "PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
-            "PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
+            "RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0",
+            "RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1",
             Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _dimensions_type_0 = data
-                dimensions_type_0: Union[Unset, PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0]
+                dimensions_type_0: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0]
                 if isinstance(_dimensions_type_0, Unset):
                     dimensions_type_0 = UNSET
                 else:
-                    dimensions_type_0 = PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0.from_dict(
+                    dimensions_type_0 = RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0.from_dict(
                         _dimensions_type_0
                     )
 
                 return dimensions_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _dimensions_type_1 = data
-            dimensions_type_1: Union[Unset, PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1]
+            dimensions_type_1: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1]
             if isinstance(_dimensions_type_1, Unset):
                 dimensions_type_1 = UNSET
             else:
-                dimensions_type_1 = PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1.from_dict(
+                dimensions_type_1 = RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1.from_dict(
                     _dimensions_type_1
                 )
 
             return dimensions_type_1
 
         dimensions = _parse_dimensions(d.pop("dimensions", UNSET))
 
-        post_run_query_response_200_results_metric_query_filters = cls(
+        run_metric_query_response_200_results_metric_query_filters = cls(
             metrics=metrics,
             dimensions=dimensions,
         )
 
-        post_run_query_response_200_results_metric_query_filters.additional_properties = d
-        return post_run_query_response_200_results_metric_query_filters
+        run_metric_query_response_200_results_metric_query_filters.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_filters
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_dimensions_type_0.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType0:
+class RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType0:
     """
     Attributes:
         or_ (List[Any]):
         id (str):
     """
 
     or_: List[Any]
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         or_ = cast(List[Any], d.pop("or"))
 
         id = d.pop("id")
 
-        post_run_query_response_200_results_metric_query_filters_dimensions_type_0 = cls(
+        run_metric_query_response_200_results_metric_query_filters_dimensions_type_0 = cls(
             or_=or_,
             id=id,
         )
 
-        post_run_query_response_200_results_metric_query_filters_dimensions_type_0.additional_properties = d
-        return post_run_query_response_200_results_metric_query_filters_dimensions_type_0
+        run_metric_query_response_200_results_metric_query_filters_dimensions_type_0.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_filters_dimensions_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1:
+class RunMetricQueryResponse200ResultsMetricQueryFiltersDimensionsType1:
     """
     Attributes:
         and_ (List[Any]):
         id (str):
     """
 
     and_: List[Any]
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         and_ = cast(List[Any], d.pop("and"))
 
         id = d.pop("id")
 
-        post_run_query_response_200_results_metric_query_filters_dimensions_type_1 = cls(
+        run_metric_query_response_200_results_metric_query_filters_dimensions_type_1 = cls(
             and_=and_,
             id=id,
         )
 
-        post_run_query_response_200_results_metric_query_filters_dimensions_type_1.additional_properties = d
-        return post_run_query_response_200_results_metric_query_filters_dimensions_type_1
+        run_metric_query_response_200_results_metric_query_filters_dimensions_type_1.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_filters_dimensions_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0")
+T = TypeVar("T", bound="PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersMetricsType1")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType0:
+class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersMetricsType1:
     """
     Attributes:
-        or_ (List[Any]):
+        and_ (List[Any]):
         id (str):
     """
 
-    or_: List[Any]
+    and_: List[Any]
     id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        or_ = self.or_
+        and_ = self.and_
 
         id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "or": or_,
+                "and": and_,
                 "id": id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        or_ = cast(List[Any], d.pop("or"))
+        and_ = cast(List[Any], d.pop("and"))
 
         id = d.pop("id")
 
-        post_run_query_response_200_results_metric_query_filters_metrics_type_0 = cls(
-            or_=or_,
+        post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1 = cls(
+            and_=and_,
             id=id,
         )
 
-        post_run_query_response_200_results_metric_query_filters_metrics_type_0.additional_properties = d
-        return post_run_query_response_200_results_metric_query_filters_metrics_type_0
+        post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.additional_properties = (
+            d
+        )
+        return post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_metrics_type_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryFiltersMetricsType1:
+class RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType1:
     """
     Attributes:
         and_ (List[Any]):
         id (str):
     """
 
     and_: List[Any]
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         and_ = cast(List[Any], d.pop("and"))
 
         id = d.pop("id")
 
-        post_run_query_response_200_results_metric_query_filters_metrics_type_1 = cls(
+        run_metric_query_response_200_results_metric_query_filters_metrics_type_1 = cls(
             and_=and_,
             id=id,
         )
 
-        post_run_query_response_200_results_metric_query_filters_metrics_type_1.additional_properties = d
-        return post_run_query_response_200_results_metric_query_filters_metrics_type_1
+        run_metric_query_response_200_results_metric_query_filters_metrics_type_1.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_filters_metrics_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_sorts_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQuerySortsItem")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQuerySortsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQuerySortsItem:
+class RunMetricQueryResponse200ResultsMetricQuerySortsItem:
     """
     Attributes:
         descending (bool):
         field_id (str):
     """
 
     descending: bool
@@ -35,21 +35,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         descending = d.pop("descending")
 
         field_id = d.pop("fieldId")
 
-        post_run_query_response_200_results_metric_query_sorts_item = cls(
+        run_metric_query_response_200_results_metric_query_sorts_item = cls(
             descending=descending,
             field_id=field_id,
         )
 
-        post_run_query_response_200_results_metric_query_sorts_item.additional_properties = d
-        return post_run_query_response_200_results_metric_query_sorts_item
+        run_metric_query_response_200_results_metric_query_sorts_item.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_sorts_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_query_response_200_results_metric_query_table_calculations_item_format import (
-        PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat,
+    from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item_format import (
+        RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat,
     )
 
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryTableCalculationsItem:
+class RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem:
     """
     Attributes:
         sql (str):
         display_name (str):
         name (str):
-        format_ (Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat]):
+        format_ (Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat]):
         index (Union[Unset, float]):
     """
 
     sql: str
     display_name: str
     name: str
-    format_: Union[Unset, "PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat"] = UNSET
+    format_: Union[Unset, "RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat"] = UNSET
     index: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         sql = self.sql
         display_name = self.display_name
         name = self.name
@@ -55,44 +55,44 @@
         if index is not UNSET:
             field_dict["index"] = index
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_query_response_200_results_metric_query_table_calculations_item_format import (
-            PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat,
+        from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item_format import (
+            RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat,
         )
 
         d = src_dict.copy()
         sql = d.pop("sql")
 
         display_name = d.pop("displayName")
 
         name = d.pop("name")
 
         _format_ = d.pop("format", UNSET)
-        format_: Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat]
+        format_: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat]
         if isinstance(_format_, Unset):
             format_ = UNSET
         else:
-            format_ = PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat.from_dict(_format_)
+            format_ = RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat.from_dict(_format_)
 
         index = d.pop("index", UNSET)
 
-        post_run_query_response_200_results_metric_query_table_calculations_item = cls(
+        run_metric_query_response_200_results_metric_query_table_calculations_item = cls(
             sql=sql,
             display_name=display_name,
             name=name,
             format_=format_,
             index=index,
         )
 
-        post_run_query_response_200_results_metric_query_table_calculations_item.additional_properties = d
-        return post_run_query_response_200_results_metric_query_table_calculations_item
+        run_metric_query_response_200_results_metric_query_table_calculations_item.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_table_calculations_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_table_calculations_item_format.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.post_run_query_response_200_results_metric_query_table_calculations_item_format_compact import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact,
+from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item_format_compact import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact,
 )
-from ..models.post_run_query_response_200_results_metric_query_table_calculations_item_format_separator import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator,
+from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item_format_separator import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator,
 )
-from ..models.post_run_query_response_200_results_metric_query_table_calculations_item_format_type import (
-    PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType,
+from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item_format_type import (
+    RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat")
 
 
 @attr.s(auto_attribs=True)
-class PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormat:
+class RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormat:
     """
     Attributes:
-        type (PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType):
+        type (RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType):
         suffix (Union[Unset, str]):
         prefix (Union[Unset, str]):
-        compact (Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact]):
+        compact (Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact]):
         currency (Union[Unset, str]):
-        separator (Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator]):
+        separator (Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator]):
         round_ (Union[Unset, float]):
     """
 
-    type: PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType
+    type: RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType
     suffix: Union[Unset, str] = UNSET
     prefix: Union[Unset, str] = UNSET
-    compact: Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact] = UNSET
+    compact: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact] = UNSET
     currency: Union[Unset, str] = UNSET
-    separator: Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator] = UNSET
+    separator: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator] = UNSET
     round_: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         suffix = self.suffix
@@ -75,50 +75,50 @@
             field_dict["round"] = round_
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType(d.pop("type"))
+        type = RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatType(d.pop("type"))
 
         suffix = d.pop("suffix", UNSET)
 
         prefix = d.pop("prefix", UNSET)
 
         _compact = d.pop("compact", UNSET)
-        compact: Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact]
+        compact: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact]
         if isinstance(_compact, Unset):
             compact = UNSET
         else:
-            compact = PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact(_compact)
+            compact = RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatCompact(_compact)
 
         currency = d.pop("currency", UNSET)
 
         _separator = d.pop("separator", UNSET)
-        separator: Union[Unset, PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator]
+        separator: Union[Unset, RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator]
         if isinstance(_separator, Unset):
             separator = UNSET
         else:
-            separator = PostRunQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator(_separator)
+            separator = RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItemFormatSeparator(_separator)
 
         round_ = d.pop("round", UNSET)
 
-        post_run_query_response_200_results_metric_query_table_calculations_item_format = cls(
+        run_metric_query_response_200_results_metric_query_table_calculations_item_format = cls(
             type=type,
             suffix=suffix,
             prefix=prefix,
             compact=compact,
             currency=currency,
             separator=separator,
             round_=round_,
         )
 
-        post_run_query_response_200_results_metric_query_table_calculations_item_format.additional_properties = d
-        return post_run_query_response_200_results_metric_query_table_calculations_item_format
+        run_metric_query_response_200_results_metric_query_table_calculations_item_format.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_table_calculations_item_format
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 from ..models.post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0 import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType0,
 )
 from ..models.post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_1 import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType1,
 )
+from ..models.post_run_underlying_data_query_json_body_additional_metrics_item_format import (
+    PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat,
+)
 from ..models.post_run_underlying_data_query_json_body_additional_metrics_item_type import (
     PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.post_run_underlying_data_query_json_body_additional_metrics_item_filters_item import (
@@ -32,15 +35,15 @@
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
         compact (Union[PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType0,
             PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        format_ (Union[Unset, PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
         filters (Union[Unset, List['PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
     type: PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemType
@@ -52,15 +55,15 @@
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
         PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType0,
         PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType1,
         Unset,
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
     filters: Union[Unset, List["PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
@@ -82,15 +85,18 @@
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -187,15 +193,20 @@
             else:
                 compact_type_1 = PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemCompactType1(_compact_type_1)
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
             filters_item = PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItem.from_dict(
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_additional_metrics_item_filters_item_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 
-class PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class RunMetricQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_json_body_sorts_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemTarget")
+T = TypeVar("T", bound="RunMetricQueryJsonBodySortsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemTarget:
+class RunMetricQueryJsonBodySortsItem:
     """
     Attributes:
-        field_ref (str):
+        descending (bool):
+        field_id (str):
     """
 
-    field_ref: str
+    descending: bool
+    field_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        field_ref = self.field_ref
+        descending = self.descending
+        field_id = self.field_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "fieldRef": field_ref,
+                "descending": descending,
+                "fieldId": field_id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        field_ref = d.pop("fieldRef")
+        descending = d.pop("descending")
 
-        post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target = cls(
-            field_ref=field_ref,
+        field_id = d.pop("fieldId")
+
+        run_metric_query_json_body_sorts_item = cls(
+            descending=descending,
+            field_id=field_id,
         )
 
-        post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.additional_properties = d
-        return post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target
+        run_metric_query_json_body_sorts_item.additional_properties = d
+        return run_metric_query_json_body_sorts_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item_format.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.post_run_underlying_data_query_json_body_table_calculations_item_format_compact import (
-    PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact,
+from ..models.run_query_request_table_calculations_item_format_compact import (
+    RunQueryRequestTableCalculationsItemFormatCompact,
 )
-from ..models.post_run_underlying_data_query_json_body_table_calculations_item_format_separator import (
-    PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator,
+from ..models.run_query_request_table_calculations_item_format_separator import (
+    RunQueryRequestTableCalculationsItemFormatSeparator,
 )
-from ..models.post_run_underlying_data_query_json_body_table_calculations_item_format_type import (
-    PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType,
+from ..models.run_query_request_table_calculations_item_format_type import (
+    RunQueryRequestTableCalculationsItemFormatType,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormat")
+T = TypeVar("T", bound="RunQueryRequestTableCalculationsItemFormat")
 
 
 @attr.s(auto_attribs=True)
-class PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormat:
+class RunQueryRequestTableCalculationsItemFormat:
     """
     Attributes:
-        type (PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType):
+        type (RunQueryRequestTableCalculationsItemFormatType):
         suffix (Union[Unset, str]):
         prefix (Union[Unset, str]):
-        compact (Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact]):
+        compact (Union[Unset, RunQueryRequestTableCalculationsItemFormatCompact]):
         currency (Union[Unset, str]):
-        separator (Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator]):
+        separator (Union[Unset, RunQueryRequestTableCalculationsItemFormatSeparator]):
         round_ (Union[Unset, float]):
     """
 
-    type: PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType
+    type: RunQueryRequestTableCalculationsItemFormatType
     suffix: Union[Unset, str] = UNSET
     prefix: Union[Unset, str] = UNSET
-    compact: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact] = UNSET
+    compact: Union[Unset, RunQueryRequestTableCalculationsItemFormatCompact] = UNSET
     currency: Union[Unset, str] = UNSET
-    separator: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator] = UNSET
+    separator: Union[Unset, RunQueryRequestTableCalculationsItemFormatSeparator] = UNSET
     round_: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         suffix = self.suffix
@@ -75,50 +75,50 @@
             field_dict["round"] = round_
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatType(d.pop("type"))
+        type = RunQueryRequestTableCalculationsItemFormatType(d.pop("type"))
 
         suffix = d.pop("suffix", UNSET)
 
         prefix = d.pop("prefix", UNSET)
 
         _compact = d.pop("compact", UNSET)
-        compact: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact]
+        compact: Union[Unset, RunQueryRequestTableCalculationsItemFormatCompact]
         if isinstance(_compact, Unset):
             compact = UNSET
         else:
-            compact = PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatCompact(_compact)
+            compact = RunQueryRequestTableCalculationsItemFormatCompact(_compact)
 
         currency = d.pop("currency", UNSET)
 
         _separator = d.pop("separator", UNSET)
-        separator: Union[Unset, PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator]
+        separator: Union[Unset, RunQueryRequestTableCalculationsItemFormatSeparator]
         if isinstance(_separator, Unset):
             separator = UNSET
         else:
-            separator = PostRunUnderlyingDataQueryJsonBodyTableCalculationsItemFormatSeparator(_separator)
+            separator = RunQueryRequestTableCalculationsItemFormatSeparator(_separator)
 
         round_ = d.pop("round", UNSET)
 
-        post_run_underlying_data_query_json_body_table_calculations_item_format = cls(
+        run_query_request_table_calculations_item_format = cls(
             type=type,
             suffix=suffix,
             prefix=prefix,
             compact=compact,
             currency=currency,
             separator=separator,
             round_=round_,
         )
 
-        post_run_underlying_data_query_json_body_table_calculations_item_format.additional_properties = d
-        return post_run_underlying_data_query_json_body_table_calculations_item_format
+        run_query_request_table_calculations_item_format.additional_properties = d
+        return run_query_request_table_calculations_item_format
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item import (
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
+    from ..models.run_metric_query_response_200_results_metric_query_additional_metrics_item import (
+        RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
     )
-    from ..models.post_run_underlying_data_query_response_200_results_metric_query_filters import (
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters,
+    from ..models.run_metric_query_response_200_results_metric_query_filters import (
+        RunMetricQueryResponse200ResultsMetricQueryFilters,
     )
-    from ..models.post_run_underlying_data_query_response_200_results_metric_query_sorts_item import (
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem,
+    from ..models.run_metric_query_response_200_results_metric_query_sorts_item import (
+        RunMetricQueryResponse200ResultsMetricQuerySortsItem,
     )
-    from ..models.post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item import (
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem,
+    from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item import (
+        RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem,
     )
 
 
-T = TypeVar("T", bound="PostRunUnderlyingDataQueryResponse200ResultsMetricQuery")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQuery")
 
 
 @attr.s(auto_attribs=True)
-class PostRunUnderlyingDataQueryResponse200ResultsMetricQuery:
+class RunMetricQueryResponse200ResultsMetricQuery:
     """
     Attributes:
-        table_calculations (List['PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem']):
+        table_calculations (List['RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem']):
         limit (float):
-        sorts (List['PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem']):
-        filters (PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters):
+        sorts (List['RunMetricQueryResponse200ResultsMetricQuerySortsItem']):
+        filters (RunMetricQueryResponse200ResultsMetricQueryFilters):
         metrics (List[str]):
         dimensions (List[str]):
-        additional_metrics (Union[Unset,
-            List['PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem']]):
+        additional_metrics (Union[Unset, List['RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem']]):
     """
 
-    table_calculations: List["PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem"]
+    table_calculations: List["RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem"]
     limit: float
-    sorts: List["PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem"]
-    filters: "PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters"
+    sorts: List["RunMetricQueryResponse200ResultsMetricQuerySortsItem"]
+    filters: "RunMetricQueryResponse200ResultsMetricQueryFilters"
     metrics: List[str]
     dimensions: List[str]
-    additional_metrics: Union[
-        Unset, List["PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem"]
-    ] = UNSET
+    additional_metrics: Union[Unset, List["RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         table_calculations = []
         for table_calculations_item_data in self.table_calculations:
             table_calculations_item = table_calculations_item_data.to_dict()
 
@@ -90,77 +87,73 @@
         if additional_metrics is not UNSET:
             field_dict["additionalMetrics"] = additional_metrics
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item import (
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
+        from ..models.run_metric_query_response_200_results_metric_query_additional_metrics_item import (
+            RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem,
         )
-        from ..models.post_run_underlying_data_query_response_200_results_metric_query_filters import (
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters,
+        from ..models.run_metric_query_response_200_results_metric_query_filters import (
+            RunMetricQueryResponse200ResultsMetricQueryFilters,
         )
-        from ..models.post_run_underlying_data_query_response_200_results_metric_query_sorts_item import (
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem,
+        from ..models.run_metric_query_response_200_results_metric_query_sorts_item import (
+            RunMetricQueryResponse200ResultsMetricQuerySortsItem,
         )
-        from ..models.post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item import (
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem,
+        from ..models.run_metric_query_response_200_results_metric_query_table_calculations_item import (
+            RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem,
         )
 
         d = src_dict.copy()
         table_calculations = []
         _table_calculations = d.pop("tableCalculations")
         for table_calculations_item_data in _table_calculations:
-            table_calculations_item = (
-                PostRunUnderlyingDataQueryResponse200ResultsMetricQueryTableCalculationsItem.from_dict(
-                    table_calculations_item_data
-                )
+            table_calculations_item = RunMetricQueryResponse200ResultsMetricQueryTableCalculationsItem.from_dict(
+                table_calculations_item_data
             )
 
             table_calculations.append(table_calculations_item)
 
         limit = d.pop("limit")
 
         sorts = []
         _sorts = d.pop("sorts")
         for sorts_item_data in _sorts:
-            sorts_item = PostRunUnderlyingDataQueryResponse200ResultsMetricQuerySortsItem.from_dict(sorts_item_data)
+            sorts_item = RunMetricQueryResponse200ResultsMetricQuerySortsItem.from_dict(sorts_item_data)
 
             sorts.append(sorts_item)
 
-        filters = PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFilters.from_dict(d.pop("filters"))
+        filters = RunMetricQueryResponse200ResultsMetricQueryFilters.from_dict(d.pop("filters"))
 
         metrics = cast(List[str], d.pop("metrics"))
 
         dimensions = cast(List[str], d.pop("dimensions"))
 
         additional_metrics = []
         _additional_metrics = d.pop("additionalMetrics", UNSET)
         for additional_metrics_item_data in _additional_metrics or []:
-            additional_metrics_item = (
-                PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem.from_dict(
-                    additional_metrics_item_data
-                )
+            additional_metrics_item = RunMetricQueryResponse200ResultsMetricQueryAdditionalMetricsItem.from_dict(
+                additional_metrics_item_data
             )
 
             additional_metrics.append(additional_metrics_item)
 
-        post_run_underlying_data_query_response_200_results_metric_query = cls(
+        run_metric_query_response_200_results_metric_query = cls(
             table_calculations=table_calculations,
             limit=limit,
             sorts=sorts,
             filters=filters,
             metrics=metrics,
             dimensions=dimensions,
             additional_metrics=additional_metrics,
         )
 
-        post_run_underlying_data_query_response_200_results_metric_query.additional_properties = d
-        return post_run_underlying_data_query_response_200_results_metric_query
+        run_metric_query_response_200_results_metric_query.additional_properties = d
+        return run_metric_query_response_200_results_metric_query
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0 import (
-    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
+from ..models.run_query_request_additional_metrics_item_compact_type_0 import (
+    RunQueryRequestAdditionalMetricsItemCompactType0,
 )
-from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1 import (
-    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
+from ..models.run_query_request_additional_metrics_item_compact_type_1 import (
+    RunQueryRequestAdditionalMetricsItemCompactType1,
 )
-from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type import (
-    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType,
+from ..models.run_query_request_additional_metrics_item_format import (
+    RunQueryRequestAdditionalMetricsItemFormat,
+)
+from ..models.run_query_request_additional_metrics_item_type import (
+    RunQueryRequestAdditionalMetricsItemType,
 )
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
+    from ..models.run_query_request_additional_metrics_item_filters_item import (
+        RunQueryRequestAdditionalMetricsItemFiltersItem,
     )
 
 
-T = TypeVar("T", bound="PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem")
+T = TypeVar("T", bound="RunQueryRequestAdditionalMetricsItem")
 
 
 @attr.s(auto_attribs=True)
-class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItem:
+class RunQueryRequestAdditionalMetricsItem:
     """
     Attributes:
-        type (PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType):
+        type (RunQueryRequestAdditionalMetricsItemType):
         sql (str):
         table (str):
         name (str):
         label (Union[Unset, str]):
         description (Union[Unset, str]):
         hidden (Union[Unset, bool]):
         round_ (Union[Unset, float]):
-        compact (Union[PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1, Unset]):
-        format_ (Union[Unset, str]):
+        compact (Union[RunQueryRequestAdditionalMetricsItemCompactType0,
+            RunQueryRequestAdditionalMetricsItemCompactType1, Unset]):
+        format_ (Union[Unset, RunQueryRequestAdditionalMetricsItemFormat]):
         index (Union[Unset, float]):
-        filters (Union[Unset,
-            List['PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem']]):
+        filters (Union[Unset, List['RunQueryRequestAdditionalMetricsItemFiltersItem']]):
         base_dimension_name (Union[Unset, str]):
         uuid (Union[Unset, None, str]):
     """
 
-    type: PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType
+    type: RunQueryRequestAdditionalMetricsItemType
     sql: str
     table: str
     name: str
     label: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     hidden: Union[Unset, bool] = UNSET
     round_: Union[Unset, float] = UNSET
     compact: Union[
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
-        Unset,
+        RunQueryRequestAdditionalMetricsItemCompactType0, RunQueryRequestAdditionalMetricsItemCompactType1, Unset
     ] = UNSET
-    format_: Union[Unset, str] = UNSET
+    format_: Union[Unset, RunQueryRequestAdditionalMetricsItemFormat] = UNSET
     index: Union[Unset, float] = UNSET
-    filters: Union[
-        Unset, List["PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem"]
-    ] = UNSET
+    filters: Union[Unset, List["RunQueryRequestAdditionalMetricsItemFiltersItem"]] = UNSET
     base_dimension_name: Union[Unset, str] = UNSET
     uuid: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         sql = self.sql
@@ -75,27 +73,28 @@
         description = self.description
         hidden = self.hidden
         round_ = self.round_
         compact: Union[Unset, str]
         if isinstance(self.compact, Unset):
             compact = UNSET
 
-        elif isinstance(
-            self.compact, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0
-        ):
+        elif isinstance(self.compact, RunQueryRequestAdditionalMetricsItemCompactType0):
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
         else:
             compact = UNSET
             if not isinstance(self.compact, Unset):
                 compact = self.compact.value
 
-        format_ = self.format_
+        format_: Union[Unset, str] = UNSET
+        if not isinstance(self.format_, Unset):
+            format_ = self.format_.value
+
         index = self.index
         filters: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.filters, Unset):
             filters = []
             for filters_item_data in self.filters:
                 filters_item = filters_item_data.to_dict()
 
@@ -134,20 +133,20 @@
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item import (
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem,
+        from ..models.run_query_request_additional_metrics_item_filters_item import (
+            RunQueryRequestAdditionalMetricsItemFiltersItem,
         )
 
         d = src_dict.copy()
-        type = PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemType(d.pop("type"))
+        type = RunQueryRequestAdditionalMetricsItemType(d.pop("type"))
 
         sql = d.pop("sql")
 
         table = d.pop("table")
 
         name = d.pop("name")
 
@@ -158,78 +157,65 @@
         hidden = d.pop("hidden", UNSET)
 
         round_ = d.pop("round", UNSET)
 
         def _parse_compact(
             data: object,
         ) -> Union[
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0,
-            PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1,
-            Unset,
+            RunQueryRequestAdditionalMetricsItemCompactType0, RunQueryRequestAdditionalMetricsItemCompactType1, Unset
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _compact_type_0 = data
-                compact_type_0: Union[
-                    Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0
-                ]
+                compact_type_0: Union[Unset, RunQueryRequestAdditionalMetricsItemCompactType0]
                 if isinstance(_compact_type_0, Unset):
                     compact_type_0 = UNSET
                 else:
-                    compact_type_0 = (
-                        PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType0(
-                            _compact_type_0
-                        )
-                    )
+                    compact_type_0 = RunQueryRequestAdditionalMetricsItemCompactType0(_compact_type_0)
 
                 return compact_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _compact_type_1 = data
-            compact_type_1: Union[
-                Unset, PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1
-            ]
+            compact_type_1: Union[Unset, RunQueryRequestAdditionalMetricsItemCompactType1]
             if isinstance(_compact_type_1, Unset):
                 compact_type_1 = UNSET
             else:
-                compact_type_1 = (
-                    PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemCompactType1(
-                        _compact_type_1
-                    )
-                )
+                compact_type_1 = RunQueryRequestAdditionalMetricsItemCompactType1(_compact_type_1)
 
             return compact_type_1
 
         compact = _parse_compact(d.pop("compact", UNSET))
 
-        format_ = d.pop("format", UNSET)
+        _format_ = d.pop("format", UNSET)
+        format_: Union[Unset, RunQueryRequestAdditionalMetricsItemFormat]
+        if isinstance(_format_, Unset):
+            format_ = UNSET
+        else:
+            format_ = RunQueryRequestAdditionalMetricsItemFormat(_format_)
 
         index = d.pop("index", UNSET)
 
         filters = []
         _filters = d.pop("filters", UNSET)
         for filters_item_data in _filters or []:
-            filters_item = (
-                PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItem.from_dict(
-                    filters_item_data
-                )
-            )
+            filters_item = RunQueryRequestAdditionalMetricsItemFiltersItem.from_dict(filters_item_data)
 
             filters.append(filters_item)
 
         base_dimension_name = d.pop("baseDimensionName", UNSET)
 
         uuid = d.pop("uuid", UNSET)
 
-        post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item = cls(
+        run_query_request_additional_metrics_item = cls(
             type=type,
             sql=sql,
             table=table,
             name=name,
             label=label,
             description=description,
             hidden=hidden,
@@ -238,8 +224,8 @@
             format_=format_,
             index=index,
             filters=filters,
             base_dimension_name=base_dimension_name,
             uuid=uuid,
         )
 
-        return post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item
+        return run_query_request_additional_metrics_item
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_metric_query_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-T = TypeVar("T", bound="PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersMetricsType1")
+T = TypeVar("T", bound="RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0")
 
 
 @attr.s(auto_attribs=True)
-class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryFiltersMetricsType1:
+class RunMetricQueryResponse200ResultsMetricQueryFiltersMetricsType0:
     """
     Attributes:
-        and_ (List[Any]):
+        or_ (List[Any]):
         id (str):
     """
 
-    and_: List[Any]
+    or_: List[Any]
     id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        and_ = self.and_
+        or_ = self.or_
 
         id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "and": and_,
+                "or": or_,
                 "id": id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        and_ = cast(List[Any], d.pop("and"))
+        or_ = cast(List[Any], d.pop("or"))
 
         id = d.pop("id")
 
-        post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1 = cls(
-            and_=and_,
+        run_metric_query_response_200_results_metric_query_filters_metrics_type_0 = cls(
+            or_=or_,
             id=id,
         )
 
-        post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.additional_properties = (
-            d
-        )
-        return post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1
+        run_metric_query_response_200_results_metric_query_filters_metrics_type_0.additional_properties = d
+        return run_metric_query_response_200_results_metric_query_filters_metrics_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.692.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials.py` & `lightdash_client_python-0.692.1/lightdash_client/models/postgres_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/postgres_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_6.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6_environment_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_dbt_connection_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_member_profile.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_create_user_attribute_response_results_users_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,62 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.project_member_profile_role import ProjectMemberProfileRole
-
-T = TypeVar("T", bound="ProjectMemberProfile")
+T = TypeVar("T", bound="ApiCreateUserAttributeResponseResultsUsersItem")
 
 
 @attr.s(auto_attribs=True)
-class ProjectMemberProfile:
+class ApiCreateUserAttributeResponseResultsUsersItem:
     """
     Attributes:
-        last_name (str):
-        first_name (str):
+        value (str):
         email (str):
-        role (ProjectMemberProfileRole):
-        project_uuid (str):
         user_uuid (str):
     """
 
-    last_name: str
-    first_name: str
+    value: str
     email: str
-    role: ProjectMemberProfileRole
-    project_uuid: str
     user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        last_name = self.last_name
-        first_name = self.first_name
+        value = self.value
         email = self.email
-        role = self.role.value
-
-        project_uuid = self.project_uuid
         user_uuid = self.user_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "lastName": last_name,
-                "firstName": first_name,
+                "value": value,
                 "email": email,
-                "role": role,
-                "projectUuid": project_uuid,
                 "userUuid": user_uuid,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        last_name = d.pop("lastName")
-
-        first_name = d.pop("firstName")
+        value = d.pop("value")
 
         email = d.pop("email")
 
-        role = ProjectMemberProfileRole(d.pop("role"))
-
-        project_uuid = d.pop("projectUuid")
-
         user_uuid = d.pop("userUuid")
 
-        project_member_profile = cls(
-            last_name=last_name,
-            first_name=first_name,
+        api_create_user_attribute_response_results_users_item = cls(
+            value=value,
             email=email,
-            role=role,
-            project_uuid=project_uuid,
             user_uuid=user_uuid,
         )
 
-        project_member_profile.additional_properties = d
-        return project_member_profile
+        api_create_user_attribute_response_results_users_item.additional_properties = d
+        return api_create_user_attribute_response_results_users_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/record_string_any.py` & `lightdash_client_python-0.692.1/lightdash_client/models/record_string_any.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials.py` & `lightdash_client_python-0.692.1/lightdash_client/models/redshift_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/redshift_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/remove_user_from_group_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/remove_user_from_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_space_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/resource_view_space_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/revoke_project_access_for_user_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/revoke_project_access_for_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/revoke_space_access_for_user_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/revoke_space_access_for_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_filters.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_sorts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/sort_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="RunQueryRequestSortsItem")
+T = TypeVar("T", bound="SortField")
 
 
 @attr.s(auto_attribs=True)
-class RunQueryRequestSortsItem:
+class SortField:
     """
     Attributes:
         descending (bool):
         field_id (str):
     """
 
     descending: bool
@@ -35,21 +35,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         descending = d.pop("descending")
 
         field_id = d.pop("fieldId")
 
-        run_query_request_sorts_item = cls(
+        sort_field = cls(
             descending=descending,
             field_id=field_id,
         )
 
-        run_query_request_sorts_item.additional_properties = d
-        return run_query_request_sorts_item
+        sort_field.additional_properties = d
+        return sort_field
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_query_request_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduled_jobs.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_and_targets.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_base_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_csv_options.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_csv_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_email_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_email_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_image_options.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_image_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_details.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_log_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_slack_target.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_slack_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_0_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_0_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_1_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_type_1_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_charts_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_charts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_details.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_logs_item_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_schedulers_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_users_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/scheduler_with_logs_users_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/share_url.py` & `lightdash_client_python-0.692.1/lightdash_client/models/share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/slack_channel.py` & `lightdash_client_python-0.692.1/lightdash_client/models/slack_channel.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials.py` & `lightdash_client_python-0.692.1/lightdash_client/models/snowflake_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/snowflake_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/sort_field.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_sql_query_results_rows_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,34 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SortField")
+T = TypeVar("T", bound="ApiSqlQueryResultsRowsItem")
 
 
 @attr.s(auto_attribs=True)
-class SortField:
-    """
-    Attributes:
-        descending (bool):
-        field_id (str):
-    """
+class ApiSqlQueryResultsRowsItem:
+    """Construct a type with a set of properties K of type T"""
 
-    descending: bool
-    field_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        descending = self.descending
-        field_id = self.field_id
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "descending": descending,
-                "fieldId": field_id,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        descending = d.pop("descending")
-
-        field_id = d.pop("fieldId")
-
-        sort_field = cls(
-            descending=descending,
-            field_id=field_id,
-        )
+        api_sql_query_results_rows_item = cls()
 
-        sort_field.additional_properties = d
-        return sort_field
+        api_sql_query_results_rows_item.additional_properties = d
+        return api_sql_query_results_rows_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_dashboard.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_dashboard_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_dashboard_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_query.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_query_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_query_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_query_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_query_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_share.py` & `lightdash_client_python-0.692.1/lightdash_client/models/space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/space_summary.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,55 @@
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SpaceSummary")
+T = TypeVar("T", bound="UpdateSpace")
 
 
 @attr.s(auto_attribs=True)
-class SpaceSummary:
+class UpdateSpace:
     """
     Attributes:
-        name (str):
-        organization_uuid (str):
-        uuid (str):
-        project_uuid (str):
         is_private (bool):
-        access (List[str]):
+        name (str):
     """
 
-    name: str
-    organization_uuid: str
-    uuid: str
-    project_uuid: str
     is_private: bool
-    access: List[str]
+    name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        organization_uuid = self.organization_uuid
-        uuid = self.uuid
-        project_uuid = self.project_uuid
         is_private = self.is_private
-        access = self.access
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
-                "organizationUuid": organization_uuid,
-                "uuid": uuid,
-                "projectUuid": project_uuid,
                 "isPrivate": is_private,
-                "access": access,
+                "name": name,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        organization_uuid = d.pop("organizationUuid")
-
-        uuid = d.pop("uuid")
-
-        project_uuid = d.pop("projectUuid")
-
         is_private = d.pop("isPrivate")
 
-        access = cast(List[str], d.pop("access"))
+        name = d.pop("name")
 
-        space_summary = cls(
-            name=name,
-            organization_uuid=organization_uuid,
-            uuid=uuid,
-            project_uuid=project_uuid,
+        update_space = cls(
             is_private=is_private,
-            access=access,
+            name=name,
         )
 
-        space_summary.additional_properties = d
-        return space_summary
+        update_space.additional_properties = d
+        return update_space
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials.py` & `lightdash_client_python-0.692.1/lightdash_client/models/trino_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/trino_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_allowed_email_domains_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_group.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_group_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_group_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_my_organization_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_my_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_organization_member_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_item_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_item_order_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_json_body_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_json_body_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_project_access_for_user_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_project_access_for_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_project_member.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_json_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UpdateSpace")
+T = TypeVar("T", bound="UpdateSpaceJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateSpace:
+class UpdateSpaceJsonBody:
     """
     Attributes:
         is_private (bool):
         name (str):
     """
 
     is_private: bool
@@ -35,21 +35,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         is_private = d.pop("isPrivate")
 
         name = d.pop("name")
 
-        update_space = cls(
+        update_space_json_body = cls(
             is_private=is_private,
             name=name,
         )
 
-        update_space.additional_properties = d
-        return update_space
+        update_space_json_body.additional_properties = d
+        return update_space_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/run_sql_query_json_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UpdateSpaceJsonBody")
+T = TypeVar("T", bound="RunSqlQueryJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateSpaceJsonBody:
-    """
+class RunSqlQueryJsonBody:
+    """The query to run
+
     Attributes:
-        is_private (bool):
-        name (str):
+        sql (str):
     """
 
-    is_private: bool
-    name: str
+    sql: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        is_private = self.is_private
-        name = self.name
+        sql = self.sql
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "isPrivate": is_private,
-                "name": name,
+                "sql": sql,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        is_private = d.pop("isPrivate")
-
-        name = d.pop("name")
+        sql = d.pop("sql")
 
-        update_space_json_body = cls(
-            is_private=is_private,
-            name=name,
+        run_sql_query_json_body = cls(
+            sql=sql,
         )
 
-        update_space_json_body.additional_properties = d
-        return update_space_json_body
+        run_sql_query_json_body.additional_properties = d
+        return run_sql_query_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_access_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.692.1/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.692.1/lightdash_client/models/updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/user_allowed_organization.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validate_project_response_200_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UserAllowedOrganization")
+T = TypeVar("T", bound="ValidateProjectResponse200Results")
 
 
 @attr.s(auto_attribs=True)
-class UserAllowedOrganization:
+class ValidateProjectResponse200Results:
     """
     Attributes:
-        members_count (float):
-        name (str):
-        organization_uuid (str):
+        job_id (str):
     """
 
-    members_count: float
-    name: str
-    organization_uuid: str
+    job_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        members_count = self.members_count
-        name = self.name
-        organization_uuid = self.organization_uuid
+        job_id = self.job_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "membersCount": members_count,
-                "name": name,
-                "organizationUuid": organization_uuid,
+                "jobId": job_id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        members_count = d.pop("membersCount")
+        job_id = d.pop("jobId")
 
-        name = d.pop("name")
-
-        organization_uuid = d.pop("organizationUuid")
-
-        user_allowed_organization = cls(
-            members_count=members_count,
-            name=name,
-            organization_uuid=organization_uuid,
+        validate_project_response_200_results = cls(
+            job_id=job_id,
         )
 
-        user_allowed_organization.additional_properties = d
-        return user_allowed_organization
+        validate_project_response_200_results.additional_properties = d
+        return validate_project_response_200_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validate_project_json_body.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validate_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validate_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200_results.py` & `lightdash_client_python-0.692.1/lightdash_client/models/api_sql_query_results_fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ValidateProjectResponse200Results")
+T = TypeVar("T", bound="ApiSqlQueryResultsFields")
 
 
 @attr.s(auto_attribs=True)
-class ValidateProjectResponse200Results:
-    """
-    Attributes:
-        job_id (str):
-    """
+class ApiSqlQueryResultsFields:
+    """Construct a type with a set of properties K of type T"""
 
-    job_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        job_id = self.job_id
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "jobId": job_id,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        job_id = d.pop("jobId")
-
-        validate_project_response_200_results = cls(
-            job_id=job_id,
-        )
+        api_sql_query_results_fields = cls()
 
-        validate_project_response_200_results.additional_properties = d
-        return validate_project_response_200_results
+        api_sql_query_results_fields.additional_properties = d
+        return api_sql_query_results_fields
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_error_chart_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_error_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_error_table_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_response_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_response_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/validation_summary.py` & `lightdash_client_python-0.692.1/lightdash_client/models/validation_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/view_statistics.py` & `lightdash_client_python-0.692.1/lightdash_client/models/view_statistics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py` & `lightdash_client_python-0.692.1/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/lightdash_client/types.py` & `lightdash_client_python-0.692.1/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/pyproject.toml` & `lightdash_client_python-0.692.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/setup.py` & `lightdash_client_python-0.692.1/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.651.2/PKG-INFO` & `lightdash_client_python-0.692.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.651.2
+Version: 0.692.1
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

