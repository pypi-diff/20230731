# Comparing `tmp/snowflake_cli_labs-1.0.0.tar.gz` & `tmp/snowflake_cli_labs-1.0.1.tar.gz`

## Comparing `snowflake_cli_labs-1.0.0.tar` & `snowflake_cli_labs-1.0.1.tar`

### file list

```diff
@@ -1,151 +1,169 @@
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/LEGAL.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/snowcli.spec
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tox.ini
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_5.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/config.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/connection_params.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/exception.py
--rw-r--r--   0        0        0    25360 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/snow_connector.py
--rw-r--r--   0        0        0    22751 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/utils.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/__init__.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/connection.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/loggers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/registry.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/render.py
--rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark_shared.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/sql.py
--rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/stage.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/streamlit.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/warehouse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/alias.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/flags.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/snow_cli_global_context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/main/__init__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/main/snow_cli_main_typer.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/__init__.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/cp.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/function.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/jobs.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/package.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/registry.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/services.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/clear.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/output/formats.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/output/printing.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/python_templates/environment.yml.jinja
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/python_templates/snowpark_coverage.py.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/call_procedure.sql
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_function.sql
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_procedure.sql
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_stage.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_streamlit.sql
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/describe_function.sql
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/describe_procedure.sql
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/describe_streamlit.sql
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_function.sql
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_procedure.sql
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_stage.sql
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_streamlit.sql
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/execute_function.sql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/get_stage.sql
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/get_streamlit_url.sql
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_functions.sql
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_procedures.sql
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_stage.sql
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_stages.sql
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_streamlits.sql
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/put_stage.sql
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/remove_from_stage.sql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/set_env.sql
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/set_procedure_comment.sql
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/share_streamlit.sql
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/show_warehouses.sql
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/create_compute_pool.sql
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/drop_compute_pool.sql
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/list_compute_pools.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/stop_compute_pools.sql
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/create_job.sql
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/desc_job.sql
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/drop_job.sql
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/logs_job.sql
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/status_job.sql
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/create_service.sql
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/desc_service.sql
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/drop_service.sql
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/list_service.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/logs_service.sql
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/status_service.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/.gitignore
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/app.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/.gitignore
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/app.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/config.toml
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/local_connection.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test.toml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_config.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_connection.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_main.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_render.py
--rw-r--r--   0        0        0    25290 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_snow_connector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_spec.yaml
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_sql.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_stage.py
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_utils.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/__snapshots__/test_connection.ambr
--rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/config/env_variables_config
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/output/test_printing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/test_data.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/conftest.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/snowflake_connector.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/test_warehouse.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/config/connection_configs.toml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/config/test.toml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/LICENSE
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/README.md
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/LEGAL.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/snowcli.spec
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tox.ini
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/docs/images/coverage_5.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/__main__.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/config.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/exception.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/pycharm_remote_debug.py
+-rw-r--r--   0        0        0    22983 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/snow_connector.py
+-rw-r--r--   0        0        0    22435 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/app.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/connection.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/loggers.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/render.py
+-rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark_shared.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/sql.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/stage.py
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/streamlit.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/warehouse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/common/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/common/alias.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/common/flags.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/common/snow_cli_global_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/main/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/main/snow_cli_main_typer.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/__init__.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/cp.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/function.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/jobs.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/package.py
+-rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/registry.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/services.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure_coverage/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure_coverage/clear.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure_coverage/report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/output/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/output/decorators.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/output/formats.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/output/printing.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/python_templates/environment.yml.jinja
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/python_templates/snowpark_coverage.py.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/call_procedure.sql
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/create_function.sql
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/create_procedure.sql
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/create_stage.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/create_streamlit.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/describe_function.sql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/describe_procedure.sql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/describe_streamlit.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/drop_function.sql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/drop_procedure.sql
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/drop_streamlit.sql
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/execute_function.sql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/get_stage.sql
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/get_streamlit_url.sql
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/list_functions.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/list_procedures.sql
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/list_streamlits.sql
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/put_stage.sql
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/remove_from_stage.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/set_env.sql
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/set_procedure_comment.sql
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/share_streamlit.sql
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/compute_pool/create_compute_pool.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/compute_pool/drop_compute_pool.sql
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/compute_pool/list_compute_pools.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/compute_pool/stop_compute_pools.sql
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/jobs/create_job.sql
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/jobs/desc_job.sql
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/jobs/drop_job.sql
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/jobs/logs_job.sql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/jobs/status_job.sql
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/services/create_service.sql
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/services/desc_service.sql
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/services/drop_service.sql
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/services/list_service.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/services/logs_service.sql
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/snowcli/sql/snowservices/services/status_service.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_function/.gitignore
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_function/app.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_function/config.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_function/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_procedure/.gitignore
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_procedure/app.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_procedure/config.toml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_procedure/local_connection.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/src/templates/default_procedure/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/empty_config.toml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test.toml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_config.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_connection.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_main.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_package.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_render.py
+-rw-r--r--   0        0        0    21151 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_snow_connector.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_sql.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_stage.py
+-rw-r--r--   0        0        0    17314 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_warehouse.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0     9504 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/__snapshots__/test_snow_connector.ambr
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/__snapshots__/test_warehouse.ambr
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/output/test_printing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/testing_utils/files_and_dirs.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/conftest.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_cp.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_package.py
+-rw-r--r--   0        0        0    15308 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_snowpark_function.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_sql.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_stage.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_streamlit.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_utils.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_warehouse.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/__snapshots__/test_snowpark_function.ambr
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_files/sql_multi_queries.sql
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/test_files/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/file_utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/naming_utils.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/sql_utils.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/working_directory_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/assertions/__init__.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/assertions/test_file_assertions.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/tests_integration/testing_utils/assertions/test_result_assertions.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/README.md
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8206 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.1/PKG-INFO
```

### Comparing `snowflake_cli_labs-1.0.0/.pre-commit-config.yaml` & `snowflake_cli_labs-1.0.1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.1.0
     hooks:
       - id: trailing-whitespace
-        exclude: tests/
+        exclude: '(^tests/|^tests_integration/)'
       - id: end-of-file-fixer
         exclude: license_header.txt
       - id: check-yaml
         exclude: .github/repo_meta.yaml
       - id: debug-statements
+        exclude: src/snowcli/pycharm_remote_debug.py
       - id: check-ast
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.217"
     hooks:
       - id: ruff
         args: [--fix, --exclude, "**/tests/", --line-length, "88", --select, "N"]
   - repo: https://github.com/psf/black
```

### Comparing `snowflake_cli_labs-1.0.0/snowcli.spec` & `snowflake_cli_labs-1.0.1/snowcli.spec`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/docs/images/coverage_1.png` & `snowflake_cli_labs-1.0.1/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/docs/images/coverage_2.png` & `snowflake_cli_labs-1.0.1/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/docs/images/coverage_3.png` & `snowflake_cli_labs-1.0.1/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/docs/images/coverage_4.png` & `snowflake_cli_labs-1.0.1/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/docs/images/coverage_5.png` & `snowflake_cli_labs-1.0.1/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/config.py` & `snowflake_cli_labs-1.0.1/src/snowcli/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,127 +1,151 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
-from typing import Optional, Any
+from typing import Optional, Any, Dict, Union
 
 import tomlkit
 from tomlkit import dump, table, TOMLDocument
 from tomlkit.exceptions import NonExistentKey
+from tomlkit.items import Table
+from tomlkit.container import Container
 import logging
 
-from snowcli.exception import MissingConfiguration
-from snowcli.snow_connector import SnowflakeConnector
+from snowcli.exception import MissingConfiguration, UnsupportedConfigSectionTypeError
 from snowflake.connector.constants import CONFIG_FILE
 from snowflake.connector.config_manager import ConfigManager
 
-
 log = logging.getLogger(__name__)
-snowflake_connection: SnowflakeConnector
 
 
 class CliConfigManager(ConfigManager):
     def __init__(self, file_path: Path = CONFIG_FILE):
         super().__init__(name="SNOWCLI_PARSER", file_path=file_path)
         self._add_options()
 
     def from_context(self, config_path_override: Optional[Path]):
         if config_path_override:
             self.file_path = config_path_override
         if not self.file_path.exists():
             self._initialise_config()
         self.read_config()
 
+    def get_section(self, *path) -> dict:
+        section = self._find_section(*path)
+        if type(section) is Container:
+            return {
+                s: self._merge_section_with_env(section[s], *path, s) for s in section
+            }
+        elif type(section) is Table:
+            return self._merge_section_with_env(section, *path)
+        raise UnsupportedConfigSectionTypeError(type(section))
+
+    def section_exists(self, *path) -> bool:
+        try:
+            self._find_section(*path)
+            return True
+        except NonExistentKey:
+            return False
+
+    def get(self, *path, key: str, default: Optional[Any] = None) -> Any:
+        """Looks for given key under nested path in toml file."""
+        env_variable = self._get_env_value(*path, key=key)
+        if env_variable:
+            return env_variable
+        try:
+            return self.get_section(*path)[key]
+        except NonExistentKey:
+            if default:
+                return default
+            raise
+
+    def get_connection(self, connection_name: str) -> dict:
+        try:
+            return self.get_section("connections", connection_name)
+        except NonExistentKey:
+            raise MissingConfiguration(
+                f"Connection {connection_name} is not configured"
+            )
+
+    def add_connection(self, name: str, parameters: dict):
+        if not self.section_exists("connections"):
+            self._initialize_connection_section()
+        self._find_section("connections").add(name, parameters)
+        self._dump_config()
+
     def _add_options(self):
         self.add_option(
             name="options",
             parse_str=tomlkit.parse,
         )
         self.add_option(
             name="connections",
             parse_str=tomlkit.parse,
         )
 
-    def get_section(self, *path) -> TOMLDocument:
+    def _find_section(self, *path) -> TOMLDocument:
         section = self
         idx = 0
         while idx < len(path):
             section = section[path[idx]]
             idx += 1
         return section
 
-    def section_exists(self, *path) -> bool:
-        try:
-            self.get_section(*path)
-            return True
-        except NonExistentKey:
-            return False
+    def _merge_section_with_env(
+        self, section: Union[Table, Any], *path
+    ) -> Dict[str, str]:
+        if isinstance(section, Table):
+            env_variables = self._get_envs_for_path(*path)
+            section_copy = section.copy()
+            section_copy.update(env_variables)
+            return section_copy
+        # It's a atomic value
+        return section
 
-    def _get_from_env(self, *path, key: str):
+    def _get_env_value(self, *path, key: str):
         env_variable_name = (
             "SNOWFLAKE_" + "_".join(p.upper() for p in path) + f"_{key.upper()}"
         )
         return os.environ.get(env_variable_name)
 
-    def get(self, *path, key: str, default: Optional[Any] = None) -> Any:
-        """Looks for given key under nested path in toml file."""
-        env_variable = self._get_from_env(*path, key=key)
-        if env_variable:
-            return env_variable
-        try:
-            return self.get_section(*path)[key]
-        except NonExistentKey:
-            if default:
-                return default
-            raise
+    def _get_envs_for_path(self, *path) -> dict:
+        env_variables_prefix = "SNOWFLAKE_" + "_".join(p.upper() for p in path)
+        return {
+            k.replace(f"{env_variables_prefix}_", "").lower(): os.environ[k]
+            for k in os.environ.keys()
+            if k.startswith(env_variables_prefix)
+        }
 
-    def initialize_connection_section(self):
+    def _initialize_connection_section(self):
         self.conf_file_cache = TOMLDocument()
         self.conf_file_cache.append("connections", table())
 
     def _initialise_config(self):
         os.makedirs(os.path.dirname(self.file_path), exist_ok=True)
-        self.initialize_connection_section()
+        self._initialize_connection_section()
         self._dump_config()
         log.info(f"Created Snowflake configuration file at {cli_config.file_path}")
 
-    def get_connection(self, connection_name: str) -> dict:
-        try:
-            return self.get("connections", key=connection_name)
-        except NonExistentKey:
-            raise MissingConfiguration(
-                f"Connection {connection_name} is not configured"
-            )
-
-    def add_connection(self, name: str, parameters: dict):
-        if not self.section_exists("connections"):
-            self.initialize_connection_section()
-        self.get_section("connections").add(name, parameters)
-        self._dump_config()
-
     def _dump_config(self):
         with open(self.file_path, "w+") as fh:
             dump(self.conf_file_cache, fh)
 
 
 def config_init(config_file: Path):
     """
     Initializes the app configuration. Config provided via cli flag takes precedence.
     If config file does not exist we create an empty one.
     """
     cli_config.from_context(config_path_override=config_file)
 
 
-def connect_to_snowflake(connection_name: Optional[str] = None, **overrides):  # type: ignore
-    connection_name = connection_name if connection_name is not None else "dev"
-    return SnowflakeConnector(
-        connection_parameters=cli_config.get_connection(connection_name),
-        overrides=overrides,
-    )
+cli_config: CliConfigManager = CliConfigManager()  # type: ignore
 
 
-def is_auth():
-    # To be removed. Added to simplify refactor
-    return True
+_DEFAULT_CONNECTION = "dev"
 
 
-cli_config: CliConfigManager = CliConfigManager()  # type: ignore
+def get_default_connection():
+    return cli_config.get(
+        "options", key="default_connection", default=_DEFAULT_CONNECTION
+    )
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/snow_connector.py` & `snowflake_cli_labs-1.0.1/src/snowcli/snow_connector.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 
 import os
 
 import click
 import logging
 import hashlib
 from io import StringIO
+
 from jinja2 import Environment, FileSystemLoader
 from pathlib import Path
 from typing import Optional
 
 import snowflake.connector
 from snowflake.connector.cursor import SnowflakeCursor
+from snowflake.connector.errors import ForbiddenError, DatabaseError
+
+from snowcli.config import cli_config, get_default_connection
+from snowcli.exception import SnowflakeConnectionError, InvalidConnectionConfiguration
 
 log = logging.getLogger(__name__)
 TEMPLATES_PATH = Path(__file__).parent / "sql"
 
 
 def get_standard_stage_name(name: str) -> str:
     # Handle embedded stages
@@ -276,79 +281,14 @@
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
                 "like": like,
             },
         )
 
-    def list_stages(
-        self,
-        database,
-        schema,
-        role,
-        warehouse,
-        like="%%",
-    ) -> SnowflakeCursor:
-        return self.run_sql(
-            "list_stages",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "like": like,
-            },
-        )
-
-    def list_stage(
-        self,
-        database,
-        schema,
-        role,
-        warehouse,
-        name,
-        like="%%",
-    ) -> SnowflakeCursor:
-        name = get_standard_stage_name(name)
-
-        return self.run_sql(
-            "list_stage",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "name": name,
-                "like": like,
-            },
-        )
-
-    def get_stage(
-        self,
-        database,
-        schema,
-        role,
-        warehouse,
-        name,
-        path,
-    ) -> SnowflakeCursor:
-        name = get_standard_stage_name(name)
-
-        return self.run_sql(
-            "get_stage",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "name": name,
-                "path": path,
-            },
-        )
-
     def set_procedure_comment(
         self,
         database,
         schema,
         role,
         warehouse,
         signature=None,
@@ -368,96 +308,14 @@
                 "warehouse": warehouse,
                 "signature": signature,
                 "comment": comment,
             },
             show_exceptions,
         )
 
-    def put_stage(
-        self,
-        database,
-        schema,
-        warehouse,
-        role,
-        name,
-        path,
-        overwrite: bool = False,
-        parallel: int = 4,
-    ) -> SnowflakeCursor:
-        name = get_standard_stage_name(name)
-
-        return self.run_sql(
-            "put_stage",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "name": name,
-                "path": path,
-                "overwrite": overwrite,
-                "parallel": parallel,
-            },
-        )
-
-    def remove_from_stage(
-        self, database, schema, role, warehouse, name, path
-    ) -> SnowflakeCursor:
-        name = get_standard_stage_name(name)
-
-        return self.run_sql(
-            "remove_from_stage",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "name": name,
-                "path": path,
-            },
-        )
-
-    def create_stage(
-        self,
-        database,
-        schema,
-        role,
-        warehouse,
-        name,
-    ) -> SnowflakeCursor:
-        return self.run_sql(
-            "create_stage",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "name": name,
-            },
-        )
-
-    def drop_stage(
-        self,
-        database,
-        schema,
-        role,
-        warehouse,
-        name,
-    ) -> SnowflakeCursor:
-        return self.run_sql(
-            "drop_stage",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-                "name": name,
-            },
-        )
-
     def list_procedures(
         self,
         database,
         schema,
         role,
         warehouse,
         like="%%",
@@ -524,32 +382,14 @@
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
             },
         )
 
-    def show_warehouses(
-        self,
-        database="",
-        schema="",
-        role="",
-        warehouse="",
-        like="%%",
-    ) -> SnowflakeCursor:
-        return self.run_sql(
-            "show_warehouses",
-            {
-                "database": database,
-                "schema": schema,
-                "role": role,
-                "warehouse": warehouse,
-            },
-        )
-
     def create_streamlit(
         self,
         database="",
         schema="",
         role="",
         warehouse="",
         name="",
@@ -957,7 +797,40 @@
             raise e
 
     @staticmethod
     def generate_signature_from_params(params: str) -> str:
         if params == "()":
             return "()"
         return "(" + " ".join(params.split()[1::2])
+
+
+def connect_to_snowflake(connection_name: Optional[str] = None, **overrides) -> SnowflakeConnector:  # type: ignore
+    connection_name = (
+        connection_name if connection_name is not None else get_default_connection()
+    )
+    try:
+        return SnowflakeConnector(
+            connection_parameters=cli_config.get_connection(connection_name),
+            overrides=overrides,
+        )
+    except ForbiddenError as err:
+        raise SnowflakeConnectionError(err)
+    except DatabaseError as err:
+        raise InvalidConnectionConfiguration(err.msg)
+
+
+class SqlExecutionMixin:
+    def __init__(self, connection: SnowflakeConnector):
+        self._conn = connection
+
+    @classmethod
+    def from_connection(cls, connection_name: str):
+        conn = connect_to_snowflake(connection_name=connection_name)
+        return cls(connection=conn)
+
+    def _execute_template(self, template_name: str, payload: dict):
+        return self._conn.run_sql(template_name, payload)
+
+    def _execute_query(self, query: str):
+        results = self._conn.ctx.execute_string(query)
+        *_, last_result = results
+        return last_result
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/utils.py` & `snowflake_cli_labs-1.0.1/src/snowcli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations
 from dataclasses import dataclass
 
 import glob
 import json
 import logging
 import os
-import pathlib
 import re
 import shutil
 import subprocess
 import warnings
-import zipfile
-from pathlib import Path
 from typing import Dict, List, Literal, Optional
+from pathlib import Path
+from zipfile import ZipFile, ZIP_DEFLATED
 
 import click
 import requests
 import requirements
 from requirements.requirement import Requirement
 import typer
 from jinja2 import Environment, FileSystemLoader
 
-from snowcli.config import cli_config
+from snowcli.config import cli_config, get_default_connection
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 YesNoAskOptions = ["yes", "no", "ask"]
 YesNoAskOptionsType = Literal["yes", "no", "ask"]
 
 PIP_PATH = os.environ.get("SNOWCLI_PIP_PATH", "pip")
@@ -342,15 +341,15 @@
 def add_file_to_existing_zip(zip_file: str, other_file: str):
     """Adds another file to an existing zip file
 
     Args:
         zip_file (str): The existing zip file
         other_file (str): The new file to add
     """
-    with zipfile.ZipFile(zip_file, mode="a") as myzip:
+    with ZipFile(zip_file, mode="a") as myzip:
         myzip.write(other_file, os.path.basename(other_file))
 
 
 def install_packages(
     file_name: str | None,
     perform_anaconda_check: bool = True,
     package_native_libraries: YesNoAskOptionsType = "ask",
@@ -474,74 +473,73 @@
             return False, second_chance_results
     else:
         log.info("No non-supported native libraries found in packages (Good news!)...")
         return True, second_chance_results
 
 
 def recursive_zip_packages_dir(pack_dir: str, dest_zip: str) -> bool:
-    # TODO:
-    # 1. why this is -> bool
-    # 2. Reformat it to with open...
-    # 3. Reformat it to get list od dirs and then iterate through it, adding files to zip
-    # create a zip file object
-    zipf = zipfile.ZipFile(dest_zip, "w", zipfile.ZIP_DEFLATED, allowZip64=True)
-
-    # for every file in the relative path pack_dir, add it to the zip file
-    for file in pathlib.Path(pack_dir).glob("**/*"):
-        zipf.write(file, arcname=os.path.relpath(file, pack_dir))
-
-    # zip all files in the current directory except the ones that start with "." or are in the pack_dir
-    for file in pathlib.Path(".").glob("**/*"):
-        if (
-            not str(file).startswith(".")
-            and not file.match(f"{pack_dir}/*")
-            and not file.match(dest_zip)
-        ):
-            zipf.write(os.path.relpath(file))
-
-    if os.getenv("SNOWCLI_INCLUDE_PATHS") is not None:
-        for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
-            directory = pathlib.Path(dir_path)
-            if directory.is_dir():
-                for file in pathlib.Path(directory).glob("**/*"):
-                    if (
-                        not str(file).startswith(".")
-                        and not file.match("*.pyc")
-                        and not file.match("*__pycache__*")
-                    ):
-                        zipf.write(file, arcname=os.path.relpath(file, directory))
-
-    # close the zip file object
-    zipf.close()
+    files_to_pack = get_list_of_files_to_pack(pack_dir, True)
+    add_files_to_zip(dest_zip, files_to_pack)
     return True
 
 
 def standard_zip_dir(dest_zip: str) -> bool:
-    zipf = zipfile.ZipFile(dest_zip, "w", zipfile.ZIP_DEFLATED, allowZip64=True)
-    for file in pathlib.Path(".").glob("*"):
-        if not file.match(".*"):
-            zipf.write(os.path.relpath(file))
-
-    if os.getenv("SNOWCLI_INCLUDE_PATHS") is not None:
-        for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
-            directory = pathlib.Path(dir_path)
-            if directory.is_dir():
-                for file in pathlib.Path(directory).glob("**/*"):
-                    if (
-                        not str(file).startswith(".")
-                        and not file.match("*.pyc")
-                        and not file.match("*__pycache__*")
-                    ):
-                        zipf.write(file, arcname=os.path.relpath(file, directory))
-
-    # close the zip file object
-    zipf.close()
+    files_to_pack = get_list_of_files_to_pack(None, False)
+    add_files_to_zip(dest_zip, files_to_pack)
     return True
 
 
+def add_files_to_zip(dest_zip: str, files_to_pack: List[File]) -> None:
+    with ZipFile(dest_zip, "w", ZIP_DEFLATED, allowZip64=True) as package_zip:
+        for file in files_to_pack:
+            package_zip.write(
+                file.name, arcname=os.path.relpath(file.name, file.relpath)
+            )
+
+
+def get_list_of_files_to_pack(
+    pack_dir: Optional[str], is_recursive: bool
+) -> List[File]:
+
+    files: List[File] = []
+
+    def filenames_filter(filepath: Path) -> bool:
+        return (
+            not filepath.name.startswith(".")
+            and not str(filepath).startswith(".")
+            and not filepath.match("*.pyc")
+            and not filepath.match("*__pycache__*")
+            and filepath not in [file.name for file in files]
+        )
+
+    files += [
+        File(filepath.absolute(), None)
+        if filenames_filter(filepath)
+        else File(Path(), None)
+        for filepath in Path(".").glob("**/*")
+    ]
+    for include_dir in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
+        files += [
+            File(filepath.absolute(), include_dir)
+            if (os.path.isdir(include_dir) and filenames_filter(filepath))
+            else File(Path(), None)
+            for filepath in Path(include_dir).glob("**/*")
+        ]
+
+    if is_recursive:
+        files += [
+            File(filepath.absolute(), pack_dir)
+            if filenames_filter(filepath)
+            else File(Path(), None)
+            for filepath in Path(str(pack_dir)).glob("**/*")
+        ]
+
+    return list(filter(lambda x: os.path.isfile(x.name), files))
+
+
 def get_snowflake_packages() -> list[str]:
     if os.path.exists("requirements.snowflake.txt"):
         with open("requirements.snowflake.txt", encoding="utf-8") as f:
             return [line.strip() for line in f]
     else:
         return []
 
@@ -570,19 +568,27 @@
             )
         else:
             function_dict[function[0]] = function[1]
     return function_dict
 
 
 def check_for_connection(connection_name: str):
+    if not connection_name:
+        connection_name = get_default_connection()
     cli_config.get_connection(connection_name=connection_name)
     return connection_name
 
 
 def generate_deploy_stage_name(name: str, input_parameters: str) -> str:
     return name + input_parameters.replace("(", "",).replace(")", "",).replace(
         " ",
         "_",
     ).replace(
         ",",
         "",
     )
+
+
+@dataclass()
+class File:
+    name: Path
+    relpath: Optional[str] = None
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/loggers.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/loggers.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,7 +25,8 @@
         log_format = DEFAULT_LOG_FORMAT
         log_level = logging.ERROR
 
     console = logging.StreamHandler()
     console.setFormatter(logging.Formatter(log_format, "%Y-%m-%d %H:%M:%S"))
     logger.addHandler(console)
     logger.setLevel(log_level)
+    logging.getLogger("snowflake").setLevel(log_level)
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/render.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Optional
 
 import jinja2
 import typer
 
 from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS
 
-app = typer.Typer(context_settings=DEFAULT_CONTEXT_SETTINGS, hidden=True)
+app = typer.Typer(context_settings=DEFAULT_CONTEXT_SETTINGS, hidden=True, name="render")
 
 
 def read_file_content(file_name: str):
     return Path(file_name).read_text()
 
 
 @jinja2.pass_environment  # type: ignore
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark_shared.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark_shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import tempfile
 from pathlib import Path
 
 import click
 import logging
 import typer
 
-from snowcli import config, utils
-from snowcli.config import connect_to_snowflake
+from snowcli import utils
+from snowcli.snow_connector import connect_to_snowflake
 from snowcli.output.printing import print_db_cursor
 from snowcli.utils import (
     YesNoAskOptionsType,
     generate_deploy_stage_name,
     yes_no_ask_callback,
 )
 
@@ -52,85 +52,84 @@
     if type == "function" and install_coverage_wrapper:
         log.error(
             "You cannot install a code coverage wrapper on a function, only a procedure."
         )
         raise typer.Abort()
 
     conn = connect_to_snowflake(connection_name=environment)
-    if config.is_auth():
-        deploy_dict = utils.get_deploy_names(
-            conn.ctx.database,
-            conn.ctx.schema,
-            generate_deploy_stage_name(
-                name,
-                input_parameters,
-            ),
-        )
-        log.info("Uploading deployment file to stage...")
+    deploy_dict = utils.get_deploy_names(
+        conn.ctx.database,
+        conn.ctx.schema,
+        generate_deploy_stage_name(
+            name,
+            input_parameters,
+        ),
+    )
+    log.info("Uploading deployment file to stage...")
 
-        with tempfile.TemporaryDirectory() as temp_dir:
-            temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
-            if install_coverage_wrapper:
-                handler = replace_handler_in_zip(
-                    proc_name=name,
-                    proc_signature=input_parameters,
-                    handler=handler,
-                    coverage_reports_stage=deploy_dict["stage"],
-                    coverage_reports_stage_path=deploy_dict["directory"] + "/coverage",
-                    temp_dir=temp_dir,
-                    zip_file_path=temp_app_zip_path,
-                )
-            conn.upload_file_to_stage(
-                file_path=temp_app_zip_path,
-                destination_stage=deploy_dict["stage"],
-                path=deploy_dict["directory"],
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                overwrite=overwrite,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        packages = utils.get_snowflake_packages()
+    with tempfile.TemporaryDirectory() as temp_dir:
+        temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
         if install_coverage_wrapper:
-            # if we're installing a coverage wrapper, ensure the coverage package included as a dependency
-            if "coverage" not in packages:
-                packages.append("coverage")
-        log.info(f"Creating {type}...")
-        if type == "function":
-            results = conn.create_function(
-                name=name,
-                input_parameters=input_parameters,
-                return_type=return_type,
+            handler = replace_handler_in_zip(
+                proc_name=name,
+                proc_signature=input_parameters,
                 handler=handler,
-                imports=deploy_dict["full_path"],
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-                overwrite=overwrite,
-                packages=packages,
-            )
-        elif type == "procedure":
-            results = conn.create_procedure(
-                name=name,
-                input_parameters=input_parameters,
-                return_type=return_type,
-                handler=handler,
-                imports=deploy_dict["full_path"],
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-                overwrite=overwrite,
-                packages=packages,
-                execute_as_caller=execute_as_caller,
-            )
-        else:
-            raise typer.Abort()
-        print_db_cursor(results)
+                coverage_reports_stage=deploy_dict["stage"],
+                coverage_reports_stage_path=deploy_dict["directory"] + "/coverage",
+                temp_dir=temp_dir,
+                zip_file_path=temp_app_zip_path,
+            )
+        conn.upload_file_to_stage(
+            file_path=temp_app_zip_path,
+            destination_stage=deploy_dict["stage"],
+            path=deploy_dict["directory"],
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            overwrite=overwrite,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    packages = utils.get_snowflake_packages()
+    if install_coverage_wrapper:
+        # if we're installing a coverage wrapper, ensure the coverage package included as a dependency
+        if "coverage" not in packages:
+            packages.append("coverage")
+    log.info(f"Creating {type}...")
+    if type == "function":
+        results = conn.create_function(
+            name=name,
+            input_parameters=input_parameters,
+            return_type=return_type,
+            handler=handler,
+            imports=deploy_dict["full_path"],
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            overwrite=overwrite,
+            packages=packages,
+        )
+    elif type == "procedure":
+        results = conn.create_procedure(
+            name=name,
+            input_parameters=input_parameters,
+            return_type=return_type,
+            handler=handler,
+            imports=deploy_dict["full_path"],
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            overwrite=overwrite,
+            packages=packages,
+            execute_as_caller=execute_as_caller,
+        )
+    else:
+        raise typer.Abort()
+    print_db_cursor(results)
 
 
 def validate_configuration(env_conf, environment):
     if env_conf is None:
         log.error(
             f"The {environment} environment is not configured in app.toml "
             "yet, please run `snow configure -e {environment}` first before "
@@ -147,151 +146,150 @@
     handler: str,
     input_parameters: str,
     return_type: str,
     replace: bool,
     execute_as_caller: bool = False,
     install_coverage_wrapper: bool = False,
 ) -> None:
-    conn = connect_to_snowflake(connection_name=environment)
+
     if type == "function" and install_coverage_wrapper:
         log.error(
             "You cannot install a code coverage wrapper on a function, only a procedure."
         )
         raise typer.Abort()
-    if config.is_auth():
-        updated_package_list = []
-        try:
-            log.info(f"Updating {type} {name}...")
+
+    conn = connect_to_snowflake(connection_name=environment)
+    updated_package_list = []
+    try:
+        log.info(f"Updating {type} {name}...")
+        if type == "function":
+            resource_details = conn.describe_function(
+                name=name,
+                input_parameters=input_parameters,
+                database=conn.ctx.database,
+                schema=conn.ctx.schema,
+                role=conn.ctx.role,
+                warehouse=conn.ctx.warehouse,
+                show_exceptions=False,
+            )
+        elif type == "procedure":
+            resource_details = conn.describe_procedure(
+                name=name,
+                input_parameters=input_parameters,
+                database=conn.ctx.database,
+                schema=conn.ctx.schema,
+                role=conn.ctx.role,
+                warehouse=conn.ctx.warehouse,
+                show_exceptions=False,
+            )
+        log.info("Checking if any new packages to update...")
+        resource_json = utils.convert_resource_details_to_dict(
+            resource_details,
+        )  # type: ignore
+        anaconda_packages = resource_json["packages"]
+        log.info(
+            f"Found {len(anaconda_packages)} defined Anaconda "
+            "packages in deployed {type}..."
+        )
+        log.info(
+            "Checking if any packages defined or missing from "
+            "requirements.snowflake.txt..."
+        )
+        updated_package_list = utils.get_snowflake_packages_delta(
+            anaconda_packages,
+        )
+        if install_coverage_wrapper:
+            # if we're installing a coverage wrapper, ensure the coverage package included as a dependency
+            if (
+                "coverage" not in anaconda_packages
+                and "coverage" not in updated_package_list
+            ):
+                updated_package_list.append("coverage")
+        log.info("Checking if app configuration has changed...")
+        if (
+            resource_json["handler"].lower() != handler.lower()
+            or resource_json["returns"].lower() != return_type.lower()
+        ):
+            log.info(
+                "Return type or handler types do not match. Replacing"
+                "function configuration..."
+            )
+            replace = True
+    except Exception:
+        log.info(f"Existing {type} not found, creating new {type}...")
+        replace = True
+
+    finally:
+        deploy_dict = utils.get_deploy_names(
+            conn.ctx.database,
+            conn.ctx.schema,
+            generate_deploy_stage_name(name, input_parameters),
+        )
+        with tempfile.TemporaryDirectory() as temp_dir:
+            temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
+            stage_path = deploy_dict["directory"] + "/coverage"
+            if install_coverage_wrapper:
+                handler = replace_handler_in_zip(
+                    proc_name=name,
+                    proc_signature=input_parameters,
+                    handler=handler,
+                    coverage_reports_stage=deploy_dict["stage"],
+                    coverage_reports_stage_path=stage_path,
+                    temp_dir=temp_dir,
+                    zip_file_path=temp_app_zip_path,
+                )
+            deploy_response = conn.upload_file_to_stage(
+                file_path=temp_app_zip_path,
+                destination_stage=deploy_dict["stage"],
+                path=deploy_dict["directory"],
+                database=conn.ctx.database,
+                schema=conn.ctx.schema,
+                overwrite=True,
+                role=conn.ctx.role,
+                warehouse=conn.ctx.warehouse,
+            )
+        log.info(f"{file.name} uploaded to stage {deploy_dict['full_path']}")
+
+        if updated_package_list or replace:
+            log.info(f"Replacing {type} with updated values...")
             if type == "function":
-                resource_details = conn.describe_function(
+                conn.create_function(
                     name=name,
                     input_parameters=input_parameters,
+                    return_type=return_type,
+                    handler=handler,
+                    imports=deploy_dict["full_path"],
                     database=conn.ctx.database,
                     schema=conn.ctx.schema,
                     role=conn.ctx.role,
                     warehouse=conn.ctx.warehouse,
-                    show_exceptions=False,
+                    overwrite=True,
+                    packages=utils.get_snowflake_packages(),
                 )
             elif type == "procedure":
-                resource_details = conn.describe_procedure(
+                conn.create_procedure(
                     name=name,
                     input_parameters=input_parameters,
+                    return_type=return_type,
+                    handler=handler,
+                    imports=deploy_dict["full_path"],
                     database=conn.ctx.database,
                     schema=conn.ctx.schema,
                     role=conn.ctx.role,
                     warehouse=conn.ctx.warehouse,
-                    show_exceptions=False,
-                )
-            log.info("Checking if any new packages to update...")
-            resource_json = utils.convert_resource_details_to_dict(
-                resource_details,
-            )  # type: ignore
-            anaconda_packages = resource_json["packages"]
-            log.info(
-                f"Found {len(anaconda_packages)} defined Anaconda "
-                "packages in deployed {type}..."
-            )
-            log.info(
-                "Checking if any packages defined or missing from "
-                "requirements.snowflake.txt..."
-            )
-            updated_package_list = utils.get_snowflake_packages_delta(
-                anaconda_packages,
-            )
-            if install_coverage_wrapper:
-                # if we're installing a coverage wrapper, ensure the coverage package included as a dependency
-                if (
-                    "coverage" not in anaconda_packages
-                    and "coverage" not in updated_package_list
-                ):
-                    updated_package_list.append("coverage")
-            log.info("Checking if app configuration has changed...")
-            if (
-                resource_json["handler"].lower() != handler.lower()
-                or resource_json["returns"].lower() != return_type.lower()
-            ):
-                log.info(
-                    "Return type or handler types do not match. Replacing"
-                    "function configuration..."
-                )
-                replace = True
-        except Exception:
-            log.info(f"Existing {type} not found, creating new {type}...")
-            replace = True
-
-        finally:
-            deploy_dict = utils.get_deploy_names(
-                conn.ctx.database,
-                conn.ctx.schema,
-                generate_deploy_stage_name(name, input_parameters),
-            )
-            with tempfile.TemporaryDirectory() as temp_dir:
-                temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
-                stage_path = deploy_dict["directory"] + "/coverage"
-                if install_coverage_wrapper:
-                    handler = replace_handler_in_zip(
-                        proc_name=name,
-                        proc_signature=input_parameters,
-                        handler=handler,
-                        coverage_reports_stage=deploy_dict["stage"],
-                        coverage_reports_stage_path=stage_path,
-                        temp_dir=temp_dir,
-                        zip_file_path=temp_app_zip_path,
-                    )
-                deploy_response = conn.upload_file_to_stage(
-                    file_path=temp_app_zip_path,
-                    destination_stage=deploy_dict["stage"],
-                    path=deploy_dict["directory"],
-                    database=conn.ctx.database,
-                    schema=conn.ctx.schema,
                     overwrite=True,
-                    role=conn.ctx.role,
-                    warehouse=conn.ctx.warehouse,
+                    packages=utils.get_snowflake_packages(),
+                    execute_as_caller=execute_as_caller,
                 )
             log.info(
-                f"{deploy_response[0]} uploaded to stage " f"{deploy_dict['full_path']}"
+                f"{type.capitalize()} {name} updated with new packages. "
+                "Deployment complete!"
             )
-
-            if updated_package_list or replace:
-                log.info(f"Replacing {type} with updated values...")
-                if type == "function":
-                    conn.create_function(
-                        name=name,
-                        input_parameters=input_parameters,
-                        return_type=return_type,
-                        handler=handler,
-                        imports=deploy_dict["full_path"],
-                        database=conn.ctx.database,
-                        schema=conn.ctx.schema,
-                        role=conn.ctx.role,
-                        warehouse=conn.ctx.warehouse,
-                        overwrite=True,
-                        packages=utils.get_snowflake_packages(),
-                    )
-                elif type == "procedure":
-                    conn.create_procedure(
-                        name=name,
-                        input_parameters=input_parameters,
-                        return_type=return_type,
-                        handler=handler,
-                        imports=deploy_dict["full_path"],
-                        database=conn.ctx.database,
-                        schema=conn.ctx.schema,
-                        role=conn.ctx.role,
-                        warehouse=conn.ctx.warehouse,
-                        overwrite=True,
-                        packages=utils.get_snowflake_packages(),
-                        execute_as_caller=execute_as_caller,
-                    )
-                log.info(
-                    f"{type.capitalize()} {name} updated with new packages. "
-                    "Deployment complete!"
-                )
-            else:
-                log.info("No packages to update. Deployment complete!")
+        else:
+            log.info("No packages to update. Deployment complete!")
 
 
 def replace_handler_in_zip(
     proc_name: str,
     proc_signature: str,
     handler: str,
     temp_dir: str,
@@ -386,131 +384,127 @@
     else:
         utils.standard_zip_dir("app.zip")
     log.info("Deployment package now ready: app.zip")
 
 
 def snowpark_execute(type: str, environment: str, select: str):
     conn = connect_to_snowflake(connection_name=environment)
-    if config.is_auth():
-        if type == "function":
-            results = conn.execute_function(
-                function=select,
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        elif type == "procedure":
-            results = conn.execute_procedure(
-                procedure=select,
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        else:
-            raise typer.Abort()
-        print_db_cursor(results)
+    if type == "function":
+        results = conn.execute_function(
+            function=select,
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    elif type == "procedure":
+        results = conn.execute_procedure(
+            procedure=select,
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    else:
+        raise typer.Abort()
+    print_db_cursor(results)
 
 
 def snowpark_describe(
     type: str,
     environment: str,
     name: str,
     input_parameters: str,
     signature: str,
 ):
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        if signature == "":
-            if name == "" and input_parameters == "":
-                typer.BadParameter(
-                    "Please provide either a function name and input "
-                    "parameters or a function signature",
-                )
-            signature = name + conn.generate_signature_from_params(
-                input_parameters,
+    if signature == "":
+        if name == "" and input_parameters == "":
+            typer.BadParameter(
+                "Please provide either a function name and input "
+                "parameters or a function signature",
             )
-        if type == "function":
-            results = conn.describe_function(
-                signature=signature,
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        elif type == "procedure":
-            results = conn.describe_procedure(
-                signature=signature,
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        else:
-            raise typer.Abort()
-        print_db_cursor(results)
+        signature = name + conn.generate_signature_from_params(
+            input_parameters,
+        )
+    if type == "function":
+        results = conn.describe_function(
+            signature=signature,
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    elif type == "procedure":
+        results = conn.describe_procedure(
+            signature=signature,
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    else:
+        raise typer.Abort()
+    print_db_cursor(results)
 
 
 def snowpark_list(type, environment, like):
     conn = connect_to_snowflake(connection_name=environment)
-    if config.is_auth():
-        if type == "function":
-            results = conn.list_functions(
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-                like=like,
-            )
-        elif type == "procedure":
-            results = conn.list_procedures(
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-                like=like,
-            )
-        else:
-            raise typer.Abort()
-        print_db_cursor(results)
+    if type == "function":
+        results = conn.list_functions(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            like=like,
+        )
+    elif type == "procedure":
+        results = conn.list_procedures(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            like=like,
+        )
+    else:
+        raise typer.Abort()
+    print_db_cursor(results)
 
 
 def snowpark_drop(
     type: str,
     environment: str,
     name: str,
     input_parameters: str,
     signature: str,
 ):
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        if signature == "":
-            if name == "" and input_parameters == "":
-                typer.BadParameter(
-                    "Please provide either a function name and input "
-                    "parameters or a function signature",
-                )
-            signature = name + conn.generate_signature_from_params(
-                input_parameters,
-            )
-        if type == "function":
-            results = conn.drop_function(
-                signature=signature,
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
+    if signature == "":
+        if name == "" and input_parameters == "":
+            typer.BadParameter(
+                "Please provide either a function name and input "
+                "parameters or a function signature",
             )
-        elif type == "procedure":
-            results = conn.drop_procedure(
-                signature=signature,
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        else:
-            raise typer.Abort()
-        print_db_cursor(results)
+        signature = name + conn.generate_signature_from_params(
+            input_parameters,
+        )
+    if type == "function":
+        results = conn.drop_function(
+            signature=signature,
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    elif type == "procedure":
+        results = conn.drop_procedure(
+            signature=signature,
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    else:
+        raise typer.Abort()
+    print_db_cursor(results)
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/stage.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,179 @@
-from __future__ import annotations
-
-from pathlib import Path
+import sys
 
 import typer
+from typing import TextIO
+from typing_extensions import Annotated
 
-from snowcli import config
-from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
-from snowcli.config import connect_to_snowflake
+from snowcli.cli.common.flags import ConnectionOption, DEFAULT_CONTEXT_SETTINGS
+from snowcli.snow_connector import connect_to_snowflake
 from snowcli.output.printing import print_db_cursor
 
 app = typer.Typer(
-    name="stage",
-    context_settings=DEFAULT_CONTEXT_SETTINGS,
-    help="Manage stages",
+    context_settings=DEFAULT_CONTEXT_SETTINGS, name="services", help="Manage services"
 )
 
+if not sys.stdout.closed and sys.stdout.isatty():
+    GREEN = "\033[32m"
+    BLUE = "\033[34m"
+    ORANGE = "\033[38:2:238:76:44m"
+    GRAY = "\033[2m"
+    ENDC = "\033[0m"
+else:
+    GREEN = ""
+    ORANGE = ""
+    BLUE = ""
+    GRAY = ""
+    ENDC = ""
+
 
-@app.command("list")
-def stage_list(
+@app.command()
+def create(
     environment: str = ConnectionOption,
-    name=typer.Argument(None, help="Name of stage"),
+    name: str = typer.Option(..., "--name", "-n", help="Job Name"),
+    compute_pool: str = typer.Option(..., "--compute_pool", "-c", help="Compute Pool"),
+    spec_path: str = typer.Option(..., "--spec_path", "-s", help="Spec Path"),
+    num_instances: Annotated[
+        int, typer.Option("--num_instances", "-num", help="Number of instances")
+    ] = 1,
+    stage: str = typer.Option("SOURCE_STAGE", "--stage", "-l", help="Stage name"),
 ):
     """
-    List stage contents
+    Create service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        if name:
-            results = conn.list_stage(
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-                name=name,
-            )
-            print_db_cursor(results)
-        else:
-            results = conn.list_stages(
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-            print_db_cursor(results)
+    results = conn.create_service(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+        compute_pool=compute_pool,
+        num_instances=num_instances,
+        spec_path=spec_path,
+        stage=stage,
+    )
+    print_db_cursor(results)
 
 
-@app.command("get")
-def stage_get(
+@app.command()
+def desc(
     environment: str = ConnectionOption,
-    name: str = typer.Argument(..., help="Stage name"),
-    path: Path = typer.Argument(
-        Path.cwd(),
-        exists=False,
-        file_okay=True,
-        dir_okay=True,
-        writable=True,
-        resolve_path=True,
-        help="Directory location to store downloaded files",
-    ),
+    name: str = typer.Argument(..., help="Service Name"),
 ):
     """
-    Download files from a stage to a local client
+    Desc Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.get_stage(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-            path=str(path),
-        )
-        print_db_cursor(results)
+    results = conn.desc_service(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+    )
+    print_db_cursor(results)
+
+
+def _prefix_line(prefix: str, line: str) -> str:
+    """
+    _prefix_line ensure the prefix is still present even when dealing with return characters
+    """
+    if "\r" in line:
+        line = line.replace("\r", f"\r{prefix}")
+    if "\n" in line[:-1]:
+        line = line[:-1].replace("\n", f"\n{prefix}") + line[-1:]
+    if not line.startswith("\r"):
+        line = f"{prefix}{line}"
+    return line
+
+
+def print_log_lines(file: TextIO, name, id, logs):
+    prefix = f"{GREEN}{name}/{id}{ENDC} "
+    logs = logs[0:-1]
+    for log in logs:
+        print(_prefix_line(prefix, log + "\n"), file=file, end="", flush=True)
 
 
-@app.command("put")
-def stage_put(
+@app.command()
+def logs(
     environment: str = ConnectionOption,
-    path: Path = typer.Argument(
-        ...,
-        exists=True,
-        file_okay=True,
-        dir_okay=True,
-        writable=True,
-        resolve_path=True,
-        help="File or directory to upload to stage",
-    ),
-    name: str = typer.Argument(..., help="Stage name"),
-    overwrite: bool = typer.Option(
-        False,
-        help="Overwrite existing files in stage",
-    ),
-    parallel: int = typer.Option(
-        4,
-        help="Number of parallel threads to use for upload",
+    name: str = typer.Argument(..., help="Service Name"),
+    container_name: str = typer.Option(
+        ..., "--container_name", "-c", help="Container Name"
     ),
 ):
     """
-    Upload files to a stage from a local client
+    Logs Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        filepath = str(path)
-        if path.is_dir():
-            filepath = str(path) + "/*"
-
-        results = conn.put_stage(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-            path=str(filepath),
-            overwrite=overwrite,
-            parallel=parallel,
-        )
-        print_db_cursor(results)
+    results = conn.logs_service(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+        instance_id="0",
+        container_name=container_name,
+    )
+    cursor = results.fetchone()
+    logs = next(iter(cursor)).split("\n")
+    print_log_lines(sys.stdout, name, "0", logs)
 
 
-@app.command("create")
-def stage_create(
+@app.command()
+def status(
     environment: str = ConnectionOption,
-    name: str = typer.Argument(..., help="Stage name"),
+    name: str = typer.Argument(..., help="Service Name"),
 ):
     """
-    Create stage if not exists
+    Logs Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.create_stage(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-        )
-        print_db_cursor(results)
+    results = conn.status_service(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+    )
+    print_db_cursor(results)
 
 
-@app.command("drop")
-def stage_drop(
-    environment: str = ConnectionOption,
-    name: str = typer.Argument(..., help="Stage name"),
-):
+@app.command()
+def list(environment: str = ConnectionOption):
     """
-    Drop stage
+    List Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.drop_stage(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-        )
-        print_db_cursor(results)
+    results = conn.list_service(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+    )
+    print_db_cursor(results)
 
 
-@app.command("remove")
-def stage_remove(
+@app.command()
+def drop(
     environment: str = ConnectionOption,
-    stage_name: str = typer.Argument(..., help="Stage name"),
-    file_name: str = typer.Argument(..., help="File name"),
+    name: str = typer.Argument(..., help="Service Name"),
 ):
     """
-    Remove file from stage
+    Drop Service
     """
-
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        config.connect_to_snowflake()
-        results = conn.remove_from_stage(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=stage_name,
-            path=file_name,
-        )
-        print_db_cursor(results)
+    results = conn.drop_service(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+    )
+    print_db_cursor(results)
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/streamlit.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/streamlit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 import logging
 import typer
 from pathlib import Path
 from typing import List, Optional
 
-from snowcli import config
 from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
-from snowcli.config import connect_to_snowflake
+from snowcli.snow_connector import connect_to_snowflake
 from snowcli.output.printing import print_db_cursor
 from snowcli.utils import (
     generate_streamlit_environment_file,
     generate_streamlit_package_wrapper,
 )
 from snowcli.cli.snowpark_shared import (
     CheckAnacondaForPyPiDependancies,
     PackageNativeLibrariesOption,
     PyPiDownloadOption,
     snowpark_package,
 )
 
 app = typer.Typer(
     context_settings=DEFAULT_CONTEXT_SETTINGS,
+    name="streamlit",
     help="Manage Streamlit in Snowflake",
 )
 log = logging.getLogger(__name__)
 
 
 def get_standard_stage_name(name: str) -> str:
     # Handle embedded stages
@@ -41,48 +41,46 @@
     only_cols: List[str] = typer.Option(list, help="Only show these columns"),
 ):
     """
     List streamlit apps.
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.list_streamlits(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-        )
-
-        print_db_cursor(
-            results,
-            columns=only_cols,
-        )
+    results = conn.list_streamlits(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+    )
+
+    print_db_cursor(
+        results,
+        columns=only_cols,
+    )
 
 
 @app.command("describe")
 def streamlit_describe(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deployed."),
 ):
     """
     Describe a streamlit app.
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        description, url = conn.describe_streamlit(
-            name,
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-        )
-        print_db_cursor(description)
-        print_db_cursor(url)
+    description, url = conn.describe_streamlit(
+        name,
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+    )
+    print_db_cursor(description)
+    print_db_cursor(url)
 
 
 @app.command("create")
 def streamlit_create(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be created."),
     file: Path = typer.Option(
@@ -99,85 +97,82 @@
     use_packaging_workaround: bool = typer.Option(
         False,
         help="Set this flag to package all code and dependencies into a zip file. "
         + "This should be considered a temporary workaround until native support is available.",
     ),
 ):
     """
-    Create a streamlit app named NAME.
+    Create a streamlit app.
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        if from_stage:
-            if "." in from_stage:
-                full_stage_name = from_stage
-            else:
-                full_stage_name = f"{conn.ctx.database}.{conn.ctx.schema}.{from_stage}"
-            standard_page_name = get_standard_stage_name(full_stage_name)
-            from_stage_command = f"FROM {standard_page_name}"
+    if from_stage:
+        if "." in from_stage:
+            full_stage_name = from_stage
         else:
-            from_stage_command = ""
-
-        results = conn.create_streamlit(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-            file="streamlit_app_launcher.py" if use_packaging_workaround else file.name,
-            from_stage_command=from_stage_command,
-        )
-        print_db_cursor(results)
+            full_stage_name = f"{conn.ctx.database}.{conn.ctx.schema}.{from_stage}"
+        standard_page_name = get_standard_stage_name(full_stage_name)
+        from_stage_command = f"FROM {standard_page_name}"
+    else:
+        from_stage_command = ""
+
+    results = conn.create_streamlit(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+        file="streamlit_app_launcher.py" if use_packaging_workaround else file.name,
+        from_stage_command=from_stage_command,
+    )
+    print_db_cursor(results)
 
 
 @app.command("share")
 def streamlit_share(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be shared."),
     to_role: str = typer.Argument(
         ..., help="Role that streamlit should be shared with."
     ),
 ):
     """
-    Create a streamlit app named NAME.
+    Share a streamlit app with a role.
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.share_streamlit(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-            to_role=to_role,
-        )
-        print_db_cursor(results)
+    results = conn.share_streamlit(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+        to_role=to_role,
+    )
+    print_db_cursor(results)
 
 
 @app.command("drop")
 def streamlit_drop(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deleted."),
 ):
     """
-    Create a streamlit app named NAME.
+    Drop a streamlit app.
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.drop_streamlit(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-        )
-        print_db_cursor(results)
+    results = conn.drop_streamlit(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+    )
+    print_db_cursor(results)
 
 
 @app.command("deploy")
 def streamlit_deploy(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deployed."),
     file: Path = typer.Option(
@@ -211,116 +206,115 @@
         None,
         help="Sometimes Streamlit fails to import an Anaconda package at runtime. "
         + "Provide a comma-separated list of package names to exclude them from "
         + "environment.yml (noting the risk of runtime errors).",
     ),
 ):
     """
-    Deploy streamlit with NAME.
+    Deploy a streamlit app.
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        schema = conn.ctx.schema
-        role = conn.ctx.role
-        database = conn.ctx.database
-        warehouse = conn.ctx.warehouse
-        # THIS WORKAROUND HAS NOT BEEN TESTETD WITH THE NEW STREAMLIT SYNTAX
-        if use_packaging_workaround:
-            # package an app.zip file, same as the other snowpark_containers_cmds package commands
-            snowpark_package(
-                pypi_download,  # type: ignore[arg-type]
-                check_anaconda_for_pypi_deps,
-                package_native_libraries,  # type: ignore[arg-type]
-            )
-            # upload the resulting app.zip file
-            conn.upload_file_to_stage(
-                "app.zip",
-                f"{name}_stage",
-                "/",
-                role=role,
-                database=database,
-                schema=schema,
-                warehouse=warehouse,
-                overwrite=True,
-                create_stage=False,
-            )
-            main_module = str(file).replace(".py", "")
-            file = generate_streamlit_package_wrapper(
-                stage_name=f"{name}_stage",
-                main_module=main_module,
-                extract_zip=packaging_workaround_includes_content,
-            )
-            # upload the wrapper file
+    schema = conn.ctx.schema
+    role = conn.ctx.role
+    database = conn.ctx.database
+    warehouse = conn.ctx.warehouse
+    # THIS WORKAROUND HAS NOT BEEN TESTETD WITH THE NEW STREAMLIT SYNTAX
+    if use_packaging_workaround:
+        # package an app.zip file, same as the other snowpark_containers_cmds package commands
+        snowpark_package(
+            pypi_download,  # type: ignore[arg-type]
+            check_anaconda_for_pypi_deps,
+            package_native_libraries,  # type: ignore[arg-type]
+        )
+        # upload the resulting app.zip file
+        conn.upload_file_to_stage(
+            "app.zip",
+            f"{name}_stage",
+            "/",
+            role=role,
+            database=database,
+            schema=schema,
+            warehouse=warehouse,
+            overwrite=True,
+            create_stage=False,
+        )
+        main_module = str(file).replace(".py", "")
+        file = generate_streamlit_package_wrapper(
+            stage_name=f"{name}_stage",
+            main_module=main_module,
+            extract_zip=packaging_workaround_includes_content,
+        )
+        # upload the wrapper file
+        conn.upload_file_to_stage(
+            str(file),
+            f"{name}_stage",
+            "/",
+            role=role,
+            database=database,
+            schema=schema,
+            warehouse=warehouse,
+            overwrite=True,
+            create_stage=False,
+        )
+        # if the packaging process generated an environment.snowflake.txt
+        # file, convert it into an environment.yml file
+        excluded_anaconda_deps_list: Optional[List[str]] = None
+        if excluded_anaconda_deps is not None:
+            excluded_anaconda_deps_list = excluded_anaconda_deps.split(",")
+        env_file = generate_streamlit_environment_file(excluded_anaconda_deps_list)
+        if env_file:
             conn.upload_file_to_stage(
-                str(file),
+                str(env_file),
                 f"{name}_stage",
                 "/",
                 role=role,
                 database=database,
                 schema=schema,
                 warehouse=warehouse,
                 overwrite=True,
                 create_stage=False,
             )
-            # if the packaging process generated an environment.snowflake.txt
-            # file, convert it into an environment.yml file
-            excluded_anaconda_deps_list: Optional[List[str]] = None
-            if excluded_anaconda_deps is not None:
-                excluded_anaconda_deps_list = excluded_anaconda_deps.split(",")
-            env_file = generate_streamlit_environment_file(excluded_anaconda_deps_list)
-            if env_file:
-                conn.upload_file_to_stage(
-                    str(env_file),
-                    f"{name}_stage",
-                    "/",
-                    role=role,
-                    database=database,
-                    schema=schema,
-                    warehouse=warehouse,
-                    overwrite=True,
-                    create_stage=False,
-                )
-
-        base_url = conn.deploy_streamlit(
-            name=name,
-            file_path=str(file),
-            stage_path="/",
-            role=role,
-            database=database,
-            schema=schema,
-            warehouse=warehouse,
-            overwrite=True,
-        )
 
-        def get_url() -> str:
-            try:
-                host = conn.ctx.host
-            except KeyError:
-                return base_url
-
-            host_parts = host.split(".")
-
-            if len(host_parts) != 6:
-                log.error(
-                    f"The connection host ({host}) was missing or not in "
-                    "the expected format "
-                    "(<account>.<deployment>.snowflakecomputing.com)"
-                )
-                raise typer.Exit()
-            else:
-                account_name = host_parts[0]
-                deployment = ".".join(host_parts[1:4])
-
-            snowflake_host = conn.ctx.host or "app.snowflake.com"
-            uppercased_dsn = f"{database}.{schema}.{name}".upper()
-            return (
-                f"https://{snowflake_host}/{deployment}/{account_name}/"
-                f"#/streamlit-apps/{uppercased_dsn}"
+    base_url = conn.deploy_streamlit(
+        name=name,
+        file_path=str(file),
+        stage_path="/",
+        role=role,
+        database=database,
+        schema=schema,
+        warehouse=warehouse,
+        overwrite=True,
+    )
+
+    def get_url() -> str:
+        try:
+            host = conn.ctx.host
+        except KeyError:
+            return base_url
+
+        host_parts = host.split(".")
+
+        if len(host_parts) != 6:
+            log.error(
+                f"The connection host ({host}) was missing or not in "
+                "the expected format "
+                "(<account>.<deployment>.snowflakecomputing.com)"
             )
+            raise typer.Exit()
+        else:
+            account_name = host_parts[0]
+            deployment = ".".join(host_parts[1:4])
 
-        url = get_url()
+        snowflake_host = conn.ctx.host or "app.snowflake.com"
+        uppercased_dsn = f"{database}.{schema}.{name}".upper()
+        return (
+            f"https://{snowflake_host}/{deployment}/{account_name}/"
+            f"#/streamlit-apps/{uppercased_dsn}"
+        )
 
-        if open_:
-            typer.launch(url)
-        else:
-            log.info(url)
+    url = get_url()
+
+    if open_:
+        typer.launch(url)
+    else:
+        log.info(url)
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/common/flags.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/common/flags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import typer
+
 from snowcli.utils import check_for_connection
 
-DEFAULT_CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
+DEFAULT_CONTEXT_SETTINGS = {"help_option_names": ["--help", "-h"]}
 
 
 ConnectionOption = typer.Option(
-    "dev",
+    None,
     "-c",
     "--connection",
     "--environment",
-    help="Connection / environment name",
+    help=f"Connection / environment name. If not provided then default connection will be used.",
     callback=check_for_connection,
-    is_eager=True,
 )
 
 AccountOption = typer.Option(
     None,
     "-a",
     "--accountname",
     "--account",
@@ -32,15 +32,15 @@
     help="Username to connect to Snowflake.",
 )
 
 PasswordOption = typer.Option(
     None,
     "-p",
     "--password",
-    help="Snowflake password",
+    help="Snowflake password.",
     hide_input=True,
 )
 
 DatabaseOption = typer.Option(
     None,
     "-d",
     "--dbname",
@@ -52,10 +52,10 @@
     None,
     "-s",
     "--schemaname",
     "--schema",
     help=" Schema in the database to use.",
 )
 
-RoleOption = typer.Option(None, "-r", "--rolename", "--role", help="Role to be used")
+RoleOption = typer.Option(None, "-r", "--rolename", "--role", help="Role to be used.")
 
 WarehouseOption = typer.Option(None, "-w", "--warehouse", help="Warehouse to use.")
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/common/snow_cli_global_context.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/common/snow_cli_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/main/snow_cli_main_typer.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/main/snow_cli_main_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/__init__.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/cp.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/cp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import typer
-from snowcli import config
-from snowcli.cli import DEFAULT_CONTEXT_SETTINGS
+
 from snowcli.cli.common.alias import build_alias
-from snowcli.cli.common.flags import ConnectionOption
-from snowcli.config import connect_to_snowflake
+from snowcli.cli.common.flags import ConnectionOption, DEFAULT_CONTEXT_SETTINGS
+from snowcli.snow_connector import connect_to_snowflake
 from snowcli.output.printing import print_db_cursor
 
 app = typer.Typer(
     context_settings=DEFAULT_CONTEXT_SETTINGS,
     name="compute-pool",
     help="Manage compute pools. You can also use cp as alias for this command",
 )
@@ -21,84 +20,80 @@
     instance_family: str = typer.Option(..., "--family", "-f", help="Instance family"),
 ):
     """
     Create compute pool
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.create_compute_pool(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-            num_instances=num_instances,
-            instance_family=instance_family,
-        )
-        print_db_cursor(results)
+    results = conn.create_compute_pool(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+        num_instances=num_instances,
+        instance_family=instance_family,
+    )
+    print_db_cursor(results)
 
 
 @app.command()
 def list(environment: str = ConnectionOption):
     """
     List compute pools
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.list_compute_pools(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-        )
-        print_db_cursor(results)
+    results = conn.list_compute_pools(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+    )
+    print_db_cursor(results)
 
 
 @app.command()
 def drop(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Compute Pool Name"),
 ):
     """
     Drop compute pool
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.drop_compute_pool(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-        )
-        print_db_cursor(results)
+    results = conn.drop_compute_pool(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+    )
+    print_db_cursor(results)
 
 
 @app.command()
 def stop(
     environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Compute Pool Name"),
 ):
     """
     Stop and delete all services running on Compute Pool
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.stop_compute_pool(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=name,
-        )
-        print_db_cursor(results)
+    results = conn.stop_compute_pool(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        name=name,
+    )
+    print_db_cursor(results)
 
 
 app_cp = build_alias(
     app,
     name="cp",
     help_str="Manage compute pools. This is alias for compute-pool command",
 )
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/function.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/function.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/jobs.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
 import typer
-from snowcli import config
 from typing import TextIO
 
-from snowcli.cli import DEFAULT_CONTEXT_SETTINGS
-from snowcli.cli.common.flags import ConnectionOption
-from snowcli.config import connect_to_snowflake
-from snowcli.output.printing import print_db_cursor, print_data
+
+from snowcli.cli.common.flags import ConnectionOption, DEFAULT_CONTEXT_SETTINGS
+from snowcli.snow_connector import connect_to_snowflake
+from snowcli.output.printing import print_db_cursor
 
 app = typer.Typer(
     context_settings=DEFAULT_CONTEXT_SETTINGS, name="jobs", help="Manage jobs"
 )
 
 if not sys.stdout.closed and sys.stdout.isatty():
     GREEN = "\033[32m"
@@ -34,46 +33,44 @@
     stage: str = typer.Option("SOURCE_STAGE", "--stage", "-l", help="Stage name"),
 ):
     """
     Create Job
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.create_job(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            compute_pool=compute_pool,
-            spec_path=spec_path,
-            stage=stage,
-        )
-        print_db_cursor(results)
+    results = conn.create_job(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        compute_pool=compute_pool,
+        spec_path=spec_path,
+        stage=stage,
+    )
+    print_db_cursor(results)
 
 
 @app.command()
 def desc(
     environment: str = ConnectionOption,
     id: str = typer.Argument(..., help="Job id"),
 ):
     """
     Desc Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.desc_job(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            id=id,
-        )
-        print_db_cursor(results)
+    results = conn.desc_job(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        id=id,
+    )
+    print_db_cursor(results)
 
 
 def _prefix_line(prefix: str, line: str) -> str:
     """
     _prefix_line ensure the prefix is still present even when dealing with return characters
     """
     if "\r" in line:
@@ -101,61 +98,58 @@
     ),
 ):
     """
     Logs Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.logs_job(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            id=id,
-            container_name=container_name,
-        )
-        cursor = results.fetchone()
-        logs = next(iter(cursor)).split("\n")
-        print_log_lines(sys.stdout, id, "0", logs)
+    results = conn.logs_job(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        id=id,
+        container_name=container_name,
+    )
+    cursor = results.fetchone()
+    logs = next(iter(cursor)).split("\n")
+    print_log_lines(sys.stdout, id, "0", logs)
 
 
 @app.command()
 def status(
     environment: str = ConnectionOption,
     id: str = typer.Argument(..., help="Job id"),
 ):
     """
     Logs Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.status_job(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            id=id,
-        )
-        print_db_cursor(results)
+    results = conn.status_job(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        id=id,
+    )
+    print_db_cursor(results)
 
 
 @app.command()
 def drop(
     environment: str = ConnectionOption,
     id: str = typer.Argument(..., help="Job id"),
 ):
     """
     Drop Service
     """
     conn = connect_to_snowflake(connection_name=environment)
 
-    if config.is_auth():
-        results = conn.drop_job(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            id=id,
-        )
-        print_db_cursor(results)
+    results = conn.drop_job(
+        database=conn.ctx.database,
+        schema=conn.ctx.schema,
+        role=conn.ctx.role,
+        warehouse=conn.ctx.warehouse,
+        id=id,
+    )
+    print_db_cursor(results)
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/package.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import click
 import logging
 import typer
 from requirements.requirement import Requirement
 
 from snowcli import config, utils
 from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
-from snowcli.config import connect_to_snowflake
+from snowcli.snow_connector import connect_to_snowflake
 
 app = typer.Typer(
     name="package",
     context_settings=DEFAULT_CONTEXT_SETTINGS,
     help="Manage custom Python packages for Snowpark",
 )
 log = logging.getLogger(__name__)
@@ -56,15 +56,15 @@
             )
         if install_packages:
             packages_string = None
             status, results = utils.install_packages(
                 perform_anaconda_check=True, package_name=name, file_name=None
             )
             if status and results is not None and len(results.snowflake) > 0:
-                packages_string = f"The package {name} is supported, but does depend on the following Snowflake supported native libraries you should include the following in your packages: {results.snowflake}"
+                packages_string = f"The package {name} is supported, but does depend on the following Snowflake supported native libraries. You should include the following in your packages: {results.snowflake}"
             # if .packages subfolder exists, delete it
             if not _run_nested and os.path.exists(".packages"):
                 rmtree(".packages")
             if packages_string is not None:
                 log.info(packages_string)
             if _run_nested and packages_string is not None:
                 return packages_string
@@ -120,26 +120,27 @@
     ),
     environment: str = ConnectionOption,
 ):
     """
     Upload a python package zip file to a Snowflake stage so it can be referenced in the imports of a procedure or function.
     """
     conn = connect_to_snowflake(connection_name=environment)
-    if config.is_auth():
-        click.echo(f"Uploading {file} to Snowflake @{stage}/{file}...")
-        with tempfile.TemporaryDirectory() as temp_dir:
-            temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
-            deploy_response = conn.upload_file_to_stage(
-                file_path=temp_app_zip_path,
-                destination_stage=stage,
-                path="/",
-                database=conn.ctx.database,
-                schema=conn.ctx.schema,
-                overwrite=overwrite,
-                role=conn.ctx.role,
-                warehouse=conn.ctx.warehouse,
-            )
-        log.info(f"Package {file} {deploy_response[6]} to Snowflake @{stage}/{file}.")
-        if deploy_response[6] == "SKIPPED":
-            log.info(
-                "Package already exists on stage. Consider using --overwrite to overwrite the file."
-            )
+    log.info(f"Uploading {file} to Snowflake @{stage}/{file}...")
+    with tempfile.TemporaryDirectory() as temp_dir:
+        temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
+        deploy_response = conn.upload_file_to_stage(
+            file_path=temp_app_zip_path,
+            destination_stage=stage,
+            path="/",
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            overwrite=overwrite,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+        )
+    log.info(
+        f"Package {file} {deploy_response.description[6]} to Snowflake @{stage}/{file}."
+    )
+    if deploy_response.description[6] == "SKIPPED":
+        log.info(
+            "Package already exists on stage. Consider using --overwrite to overwrite the file."
+        )
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         "--return-type",
         "-r",
         help="Return type",
     ),
     replace: bool = typer.Option(
         False,
         "--replace-always",
-        "-r",
         help="Replace procedure, even if no detected changes to metadata",
     ),
     execute_as_caller: bool = typer.Option(
         False,
         "--execute-as-caller",
         help="Execute as caller",
     ),
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/registry.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from __future__ import annotations
 
 import json
 import sys
 
 import typer
-from rich import print
-from snowcli import config
-from snowcli.cli import DEFAULT_CONTEXT_SETTINGS
-from snowcli.cli.common.flags import ConnectionOption
-from snowcli.config import connect_to_snowflake
+from snowcli.cli.common.flags import ConnectionOption, DEFAULT_CONTEXT_SETTINGS
+from snowcli.snow_connector import connect_to_snowflake
 
 app = typer.Typer(
     context_settings=DEFAULT_CONTEXT_SETTINGS, name="registry", help="Manage registry"
 )
 
 
 @app.command("token")
@@ -23,19 +20,18 @@
     Get token to authenticate with registry.
     """
     conn = connect_to_snowflake(
         connection_name=environment,
         # to support registry login
         session_parameters={"PYTHON_CONNECTOR_QUERY_RESULT_FORMAT": "json"},
     )
-    if config.is_auth():
-        # disable session deletion
-        conn.ctx._all_async_queries_finished = lambda: False
-        if conn.ctx._rest is None:
-            raise Exception("error in connection object")
-        # obtain and create the token
-        token_data = conn.ctx._rest._token_request("ISSUE")
-        token = {
-            "token": token_data["data"]["sessionToken"],
-            "expires_in": token_data["data"]["validityInSecondsST"],
-        }
-        sys.stdout.write(json.dumps(token))
+    # disable session deletion
+    conn.ctx._all_async_queries_finished = lambda: False
+    if conn.ctx._rest is None:
+        raise Exception("error in connection object")
+    # obtain and create the token
+    token_data = conn.ctx._rest._token_request("ISSUE")
+    token = {
+        "token": token_data["data"]["sessionToken"],
+        "expires_in": token_data["data"]["validityInSecondsST"],
+    }
+    sys.stdout.write(json.dumps(token))
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/clear.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure_coverage/clear.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import typer
 
 from snowcli import config, utils
-from snowcli.config import connect_to_snowflake
+from snowcli.cli.stage import StageManager
+from snowcli.snow_connector import connect_to_snowflake
 from snowcli.utils import generate_deploy_stage_name
 from snowcli.output.printing import print_db_cursor
 
 from snowcli.cli.snowpark.procedure_coverage import app
 from snowcli.cli.common.flags import ConnectionOption
 
 log = logging.getLogger(__name__)
@@ -30,27 +31,21 @@
         ...,
         "--input-parameters",
         "-i",
         help="Input parameters - such as (message string, count int). Must exactly match those provided when creating the procedure.",
     ),
 ):
     conn = connect_to_snowflake(connection_name=environment)
-    if config.is_auth():
-        deploy_dict = utils.get_deploy_names(
-            conn.ctx.database,
-            conn.ctx.schema,
-            generate_deploy_stage_name(
-                name,
-                input_parameters,
-            ),
-        )
-        coverage_path = f"""{deploy_dict["directory"]}/coverage"""
-        results = conn.remove_from_stage(
-            database=conn.ctx.database,
-            schema=conn.ctx.schema,
-            role=conn.ctx.role,
-            warehouse=conn.ctx.warehouse,
-            name=deploy_dict["stage"],
-            path=coverage_path,
-        )
-        log.info("Deleted the following coverage results from the stage:")
-        print_db_cursor(results)
+    deploy_dict = utils.get_deploy_names(
+        conn.ctx.database,
+        conn.ctx.schema,
+        generate_deploy_stage_name(
+            name,
+            input_parameters,
+        ),
+    )
+    coverage_path = f"""{deploy_dict["directory"]}/coverage"""
+    results = StageManager(connection=conn).remove(
+        stage_name=deploy_dict["stage"], path=coverage_path
+    )
+    log.info("Deleted the following coverage results from the stage:")
+    print_db_cursor(results)
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/report.py` & `snowflake_cli_labs-1.0.1/src/snowcli/cli/snowpark/procedure_coverage/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from enum import Enum
 
 import coverage
 import snowflake.connector
 import typer
 
 from snowcli import config, utils
-from snowcli.config import connect_to_snowflake
+from snowcli.cli.stage import StageManager
+from snowcli.snow_connector import connect_to_snowflake
 from snowcli.utils import generate_deploy_stage_name
 
 from snowcli.cli.snowpark.procedure_coverage import app
 from snowcli.cli.common.flags import ConnectionOption
 
 log = logging.getLogger(__name__)
 
@@ -50,69 +51,65 @@
     store_as_comment: bool = typer.Option(
         False,
         "--store-as-comment",
         help="In addition to the local report, saves the percentage coverage (a decimal value) as a comment on the stored procedure so that a coverage threshold can be easily checked for a number of procedures.",
     ),
 ):
     conn = connect_to_snowflake(connection_name=environment)
-    if config.is_auth():
-        deploy_dict = utils.get_deploy_names(
-            conn.ctx.database,
-            conn.ctx.schema,
-            generate_deploy_stage_name(
-                name,
-                input_parameters,
-            ),
-        )
-        coverage_file = ".coverage"
-        # the coverage databases will include paths like "/home/udf/132735964617982/app.zip/app.py", where they ran on Snowflake
-        # we need to strip out the prefix up to and including "app.zip/" so that it reads them from the local folder
-        # tried to do this by modifying the report data, but couldn't seem to figure it out
-        # instead we'll monkey-patch the source code reader and strip it out
-        orig_get_python_source = coverage.python.get_python_source
-
-        def new_get_python_source(filename: str):
-            new_filename = filename[filename.index("app.zip/") + len("app.zip/") :]
-            return orig_get_python_source(new_filename)
-
-        coverage.python.get_python_source = new_get_python_source
-
-        combined_coverage = coverage.Coverage(data_file=coverage_file)
-        with tempfile.TemporaryDirectory() as temp_dir:
-            stage_name = deploy_dict["stage"]
-            stage_path = deploy_dict["directory"]
-            report_files = f"{stage_name}{stage_path}/coverage/"
-            try:
-                results = conn.get_stage(
-                    database=conn.ctx.database,
-                    schema=conn.ctx.schema,
-                    role=conn.ctx.role,
-                    warehouse=conn.ctx.warehouse,
-                    name=report_files,
-                    path=str(temp_dir),
-                ).fetchall()
-            except snowflake.connector.errors.DatabaseError as database_error:
-                if database_error.errno == 253006:
-                    results = []
-            if len(results) == 0:
-                log.error(
-                    "No code coverage reports were found on the stage. "
-                    "Please ensure that you've invoked the procedure at least once "
-                    "and that you provided the correct inputs"
-                )
-                raise typer.Abort()
-            else:
-                log.info(f"Combining data from {len(results)} reports")
-            combined_coverage.combine(
-                # the tuple contains the columns: | file ┃ size ┃ status ┃ message |
-                data_paths=[
-                    os.path.join(temp_dir, os.path.basename(result[0]))
-                    for result in results
-                ]
+    deploy_dict = utils.get_deploy_names(
+        conn.ctx.database,
+        conn.ctx.schema,
+        generate_deploy_stage_name(
+            name,
+            input_parameters,
+        ),
+    )
+    coverage_file = ".coverage"
+    # the coverage databases will include paths like "/home/udf/132735964617982/app.zip/app.py", where they ran on Snowflake
+    # we need to strip out the prefix up to and including "app.zip/" so that it reads them from the local folder
+    # tried to do this by modifying the report data, but couldn't seem to figure it out
+    # instead we'll monkey-patch the source code reader and strip it out
+    orig_get_python_source = coverage.python.get_python_source
+
+    def new_get_python_source(filename: str):
+        new_filename = filename[filename.index("app.zip/") + len("app.zip/") :]
+        return orig_get_python_source(new_filename)
+
+    coverage.python.get_python_source = new_get_python_source
+
+    combined_coverage = coverage.Coverage(data_file=coverage_file)
+    with tempfile.TemporaryDirectory() as temp_dir:
+        stage_name = deploy_dict["stage"]
+        stage_path = deploy_dict["directory"]
+        report_files = f"{stage_name}{stage_path}/coverage/"
+        try:
+            results = (
+                StageManager(connection=conn)
+                .get(stage_name=report_files, dest_path=str(temp_dir))
+                .fetchall()
+            )
+        except snowflake.connector.errors.DatabaseError as database_error:
+            if database_error.errno == 253006:
+                results = []
+        if len(results) == 0:
+            log.error(
+                "No code coverage reports were found on the stage. "
+                "Please ensure that you've invoked the procedure at least once "
+                "and that you provided the correct inputs"
             )
+            raise typer.Abort()
+        else:
+            log.info(f"Combining data from {len(results)} reports")
+        combined_coverage.combine(
+            # the tuple contains the columns: | file ┃ size ┃ status ┃ message |
+            data_paths=[
+                os.path.join(temp_dir, os.path.basename(result[0]))
+                for result in results
+            ]
+        )
         if output_format == ReportOutputOptions.html:
             coverage_percentage = combined_coverage.html_report()
             log.info(
                 "Your HTML code coverage report is now available under the 'htmlcov' folder (htmlcov/index.html)."
             )
         elif output_format == ReportOutputOptions.json:
             coverage_percentage = combined_coverage.json_report()
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/output/printing.py` & `snowflake_cli_labs-1.0.1/src/snowcli/output/printing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from datetime import datetime
 from json import JSONEncoder
+from pathlib import Path
 from typing import List, Optional, Dict
 
 from rich import box, print, print_json
 import click
 from snowflake.connector.cursor import SnowflakeCursor
 
 from snowcli.output.formats import OutputFormat
@@ -13,14 +14,16 @@
 
 class CustomJSONEncoder(JSONEncoder):
     """Custom JSON encoder handling serialization of non-standard types"""
 
     def default(self, o):
         if isinstance(o, datetime):
             return o.isoformat()
+        if isinstance(o, Path):
+            return str(o)
         return super().default(o)
 
 
 def print_db_cursor(
     cursor: SnowflakeCursor,
     columns: Optional[List[str]] = None,
 ) -> None:
@@ -40,17 +43,24 @@
         {k: v for k, v in zip(column_names, row) if k in columns_to_include}
         for row in result
     ]
 
     _print_formatted(data, columns_to_include)
 
 
-def _print_formatted(data: List[Dict], columns: Optional[List[str]] = None):
+def _get_format_type():
     context = click.get_current_context()
-    output_format = OutputFormat(context.find_root().params.get("output_format"))
+    format_from_ctx = context.find_root().params.get("output_format")
+    if format_from_ctx:
+        return OutputFormat(format_from_ctx)
+    return OutputFormat.TABLE
+
+
+def _print_formatted(data: List[Dict], columns: Optional[List[str]] = None):
+    output_format = _get_format_type()
     if output_format == OutputFormat.TABLE:
         _print_table(data, columns)
     elif output_format == OutputFormat.JSON:
         import json
 
         print_json(json.dumps(data, cls=CustomJSONEncoder))
     else:
```

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/python_templates/snowpark_coverage.py.jinja` & `snowflake_cli_labs-1.0.1/src/snowcli/python_templates/snowpark_coverage.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/snowcli/python_templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-1.0.1/src/snowcli/python_templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/src/templates/default_procedure/app.py` & `snowflake_cli_labs-1.0.1/src/templates/default_procedure/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # For local debugging. Be aware you may need to type-convert arguments if
 # you add input parameters
 if __name__ == "__main__":
     from snowcli.config import cli_config
 
     session = Session.builder.configs(**cli_config.get_connection("dev")).create()
     if len(sys.argv) > 1:
-        print(hello(session, *sys.argv[1:]))  # type: ignore
+        print(hello(*sys.argv[1:]))  # type: ignore
     else:
-        print(hello(session))  # type: ignore
+        print(hello())  # type: ignore
     session.close()
```

### Comparing `snowflake_cli_labs-1.0.0/src/templates/default_procedure/local_connection.py` & `snowflake_cli_labs-1.0.1/src/templates/default_procedure/local_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/conftest.py` & `snowflake_cli_labs-1.0.1/tests_integration/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 from __future__ import annotations
 
 import functools
-from pathlib import Path
-from tempfile import NamedTemporaryFile
-
 import pytest
 
+from pathlib import Path
+from snowcli.cli.app import app
+from tempfile import NamedTemporaryFile
 from typer import Typer
 from typer.testing import CliRunner
 
 TEST_DIR = Path(__file__).parent
 
 
 @pytest.fixture(scope="session")
 def test_snowcli_config():
-    test_config = TEST_DIR / "test.toml"
+    test_config = TEST_DIR / "config/connection_configs.toml"
     with NamedTemporaryFile(suffix=".toml", mode="w+") as fh:
         fh.write(test_config.read_text())
         fh.flush()
-        yield Path(fh.name)
+        yield fh.name
+
+
+@pytest.fixture(scope="session")
+def test_root_path():
+    return TEST_DIR
 
 
 class SnowCLIRunner(CliRunner):
     def __init__(self, app: Typer, test_snowcli_config: str):
         super().__init__()
         self.app = app
         self.test_snowcli_config = test_snowcli_config
 
     @functools.wraps(CliRunner.invoke)
     def invoke(self, *a, **kw):
         return super().invoke(self.app, *a, **kw)
 
     def invoke_with_config(self, *args, **kwargs):
         return self.invoke(
-            ["--config-file", self.test_snowcli_config, *args[0]], **kwargs
+            ["--config-file", self.test_snowcli_config, *args[0]],
+            **kwargs,
+        )
+
+    def invoke_with_config_and_integration_connection(self, *args, **kwargs):
+        return self.invoke(
+            ["--config-file", self.test_snowcli_config, *args[0], "-c", "integration"],
+            **kwargs,
         )
 
 
-@pytest.fixture(scope="function")
+@pytest.fixture
 def runner(test_snowcli_config):
-    from snowcli.cli import app
-
     return SnowCLIRunner(app, test_snowcli_config)
```

### Comparing `snowflake_cli_labs-1.0.0/tests/test_cli.py` & `snowflake_cli_labs-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_render.py` & `snowflake_cli_labs-1.0.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_snow_connector.py` & `snowflake_cli_labs-1.0.1/tests/test_snow_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import os
 import textwrap
-from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from snowcli.snow_connector import SnowflakeConnector
 
 
@@ -29,14 +29,15 @@
     ],
 )
 @mock.patch("snowcli.snow_connector.snowflake.connector.connect")
 def test_command_context_is_passed_to_snowflake_connection(
     mock_conn, runner, cmd, expected
 ):
     mock_conn.return_value.execute_stream.return_value = (mock.MagicMock(),)
+    mock_conn.return_value.execute_string.return_value = (mock.MagicMock(),)
     result = runner.invoke_with_config(cmd)
     assert result.exit_code == 0, result.output
     kwargs = mock_conn.call_args_list[-1][-1]
     assert "application" in kwargs
     assert kwargs["application"] == expected
 
 
@@ -169,66 +170,14 @@
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_list_stages(_, snapshot):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.list_stages(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        like="likeValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
-@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
-@mock.patch("snowflake.connector")
-def test_list_stage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.list_stage(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        name=stage_name,
-        like="likeValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
-@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
-@mock.patch("snowflake.connector")
-def test_get_stage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.get_stage(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        name=stage_name,
-        path="pathValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
-@mock.patch("snowflake.connector")
 def test_set_procedure_comment(_, snapshot):
     connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.set_procedure_comment(
         database="databaseValue",
         schema="schemaValue",
@@ -240,84 +189,14 @@
         show_exceptions="show_exceptionsValue",
         comment="commentValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
-@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
-@mock.patch("snowflake.connector")
-def test_put_stage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.put_stage(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        name=stage_name,
-        path="pathValue",
-        overwrite=True,
-        parallel=42,
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert textwrap.dedent(query.getvalue()) == snapshot
-
-
-@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
-@mock.patch("snowflake.connector")
-def test_remove_from_stage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.remove_from_stage(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        name=stage_name,
-        path="/pathValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
-@mock.patch("snowflake.connector")
-def test_create_stage(_, snapshot):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.create_stage(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        name="nameValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
-@mock.patch("snowflake.connector")
-def test_drop_stage(_, snapshot):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.drop_stage(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        name="nameValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
 @mock.patch("snowflake.connector")
 def test_list_procedures(_, snapshot):
     connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.list_procedures(
         database="databaseValue",
@@ -374,30 +253,14 @@
         warehouse="warehouseValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_show_warehouses(_, snapshot):
-    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
-    connector.ctx.execute_stream.return_value = (None, None)
-
-    connector.show_warehouses(
-        database="databaseValue",
-        schema="schemaValue",
-        role="roleValue",
-        warehouse="warehouseValue",
-        like="likeValue",
-    )
-    query, *_ = connector.ctx.execute_stream.call_args.args
-    assert query.getvalue() == snapshot
-
-
-@mock.patch("snowflake.connector")
 def test_create_streamlit(_, snapshot):
     connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.create_streamlit(
         database="databaseValue",
         schema="schemaValue",
@@ -783,7 +646,15 @@
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
+
+
+@mock.patch.dict(os.environ, {}, clear=True)
+def test_returns_nice_error_in_case_of_connectivity_error(runner):
+    result = runner.invoke_with_config(["sql", "-q", "select 1"])
+    assert result.exit_code == 1
+    assert "Invalid connection configuration" in result.output
+    assert "User is empty" in result.output
```

### Comparing `snowflake_cli_labs-1.0.0/tests/test_sql.py` & `snowflake_cli_labs-1.0.1/tests/test_sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from unittest import mock
 
 from tests.testing_utils.result_assertions import assert_that_result_is_usage_error
 
-MOCK_CONNECTION = "snowcli.cli.sql.config.connect_to_snowflake"
+MOCK_CONNECTION = "snowcli.cli.sql.connect_to_snowflake"
 
 
 @mock.patch(MOCK_CONNECTION)
 def test_sql_execute_query(mock_conn, runner):
     result = runner.invoke(["sql", "-q", "query"])
 
     assert result.exit_code == 0
     mock_conn.return_value.ctx.execute_string.assert_called_once_with(
-        sql_text="query", remove_comments=True, cursor_class=mock.ANY
+        sql_text="query", remove_comments=True
     )
 
 
 @mock.patch(MOCK_CONNECTION)
 def test_sql_execute_file(mock_conn, runner):
     with NamedTemporaryFile("r") as tmp_file:
         Path(tmp_file.name).write_text("query from file")
         result = runner.invoke(["sql", "-f", tmp_file.name])
 
     assert result.exit_code == 0
     mock_conn.return_value.ctx.execute_string.assert_called_once_with(
-        sql_text="query from file", remove_comments=True, cursor_class=mock.ANY
+        sql_text="query from file", remove_comments=True
     )
 
 
 @mock.patch(MOCK_CONNECTION)
 def test_sql_execute_from_stdin(mock_conn, runner):
     result = runner.invoke(["sql"], input="query from input")
 
     assert result.exit_code == 0
     mock_conn.return_value.ctx.execute_string.assert_called_once_with(
-        sql_text="query from input", remove_comments=True, cursor_class=mock.ANY
+        sql_text="query from input", remove_comments=True
     )
 
 
 def test_sql_fails_if_no_query_file_or_stdin(runner):
     result = runner.invoke(["sql"])
 
     assert_that_result_is_usage_error(
@@ -59,25 +59,18 @@
 def test_sql_fails_for_both_query_and_file(runner):
     with NamedTemporaryFile("r") as tmp_file:
         result = runner.invoke(["sql", "-f", tmp_file.name, "-q", "query"])
 
     assert_that_result_is_usage_error(result, "Both query and file provided")
 
 
-@mock.patch("snowcli.cli.sql.config.is_auth")
-def test_sql_fails_if_user_not_authenticated(mock_is_auth, runner):
-    mock_is_auth.return_value = False
-    result = runner.invoke(["sql", "-q", "select 1"])
-
-    assert_that_result_is_usage_error(result, "Not authenticated")
-
-
-@mock.patch("snowflake.connector.connect")
+@mock.patch(MOCK_CONNECTION)
 @mock.patch("snowcli.config.cli_config")
 def test_sql_overrides_connection_configuration(mock_config, mock_conn, runner):
+    mock_config.get.return_value = "dev"  # mock of get_default_connection
     mock_config.get_connection.return_value = {}
     result = runner.invoke(
         [
             "sql",
             "-q",
             "select 1",
             "--accountname",
@@ -91,17 +84,17 @@
             "--rolename",
             "rolenameValue",
             "--warehouse",
             "warehouseValue",
         ]
     )
 
-    assert result.exit_code == 0
+    assert result.exit_code == 0, result.output
     mock_conn.assert_called_once_with(
-        application="SNOWCLI.SQL",
+        connection_name="dev",
         account="accountnameValue",
         user="usernameValue",
         warehouse="warehouseValue",
         database="dbnameValue",
         schema="schemanameValue",
         role="rolenameValue",
     )
```

### Comparing `snowflake_cli_labs-1.0.0/tests/test_utils.py` & `snowflake_cli_labs-1.0.1/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from unittest import mock
 import tempfile
 import json
 
 from pathlib import Path, PosixPath
 from requirements.requirement import Requirement
-from shutil import rmtree
-from typing import Generator, List
+from typing import Generator
 from unittest.mock import MagicMock, patch
 from zipfile import ZipFile
 
 import os
 import pytest
 import typer
 
 from snowcli import utils
 import tests.test_data.test_data as test_data
+from tests.testing_utils.files_and_dirs import create_temp_file, create_named_file
 
 
 class TestUtils:
     APP_ZIP = "app.zip"
     CORRECT_METADATA = "correct_metadata.yaml"
     FILE_IN_A_SUBDIR = "file_in_a_subdir.txt"
     FILE_IN_SECOND_TEST_DIRECTORY = "very_important_file.txt"
@@ -57,33 +57,32 @@
             "full_path": "@snowhouse_test.test_schema.deployments/jdoe/app.zip",
             "directory": "/jdoe",
         }
 
     def test_prepare_app_zip(
         self,
         temp_test_directory: str,
-        correct_app_zip: str,
+        app_zip: str,
         temp_directory_for_app_zip: str,
     ):
-        result = utils.prepare_app_zip(correct_app_zip, temp_directory_for_app_zip)
-
-        assert result == temp_directory_for_app_zip + "/app.zip"
+        result = utils.prepare_app_zip(app_zip, temp_directory_for_app_zip)
+        assert result == os.path.join(temp_directory_for_app_zip, Path(app_zip).name)
 
     def test_prepare_app_zip_if_exception_is_raised_if_no_source(
         self, temp_directory_for_app_zip
     ):
         with pytest.raises(FileNotFoundError) as expected_error:
             utils.prepare_app_zip("/non/existent/path", temp_directory_for_app_zip)
 
         assert expected_error.value.errno == 2
         assert expected_error.type == FileNotFoundError
 
-    def test_prepare_app_zip_if_exception_is_raised_if_no_dst(self, correct_app_zip):
+    def test_prepare_app_zip_if_exception_is_raised_if_no_dst(self, app_zip):
         with pytest.raises(FileNotFoundError) as expected_error:
-            utils.prepare_app_zip(correct_app_zip, "/non/existent/path")
+            utils.prepare_app_zip(app_zip, "/non/existent/path")
 
         assert expected_error.value.errno == 2
         assert expected_error.type == FileNotFoundError
 
     def test_parse_requierements_with_correct_file(self, correct_requirements_txt: str):
         result = utils.parse_requirements(correct_requirements_txt)
 
@@ -131,36 +130,38 @@
         mock_response.json.return_value = {}
         mock_requests.get.return_value = mock_response
 
         with pytest.raises(typer.Abort) as abort:
             result = utils.parse_anaconda_packages(test_data.packages)
 
     def test_generate_streamlit_environment_file_with_no_requirements(self):
-        result = utils.generate_streamlit_environment_file([])
+        result = utils.generate_streamlit_environment_file(
+            [],
+        )
         assert result is None
 
     def test_generate_streamlit_file(
-        self, streamlit_requirements_txt, temp_test_directory: str
+        self, correct_requirements_txt: str, temp_test_directory_with_chdir: str
     ):
-        os.chdir(temp_test_directory)
-        result = utils.generate_streamlit_environment_file([])
-        os.chdir("..")
+        result = utils.generate_streamlit_environment_file([], correct_requirements_txt)
 
         assert result == PosixPath("environment.yml")
-        assert os.path.isfile(os.path.join(temp_test_directory, "environment.yml"))
+        assert os.path.isfile(
+            os.path.join(temp_test_directory_with_chdir, "environment.yml")
+        )
 
     def test_generate_streamlit_environment_file_with_excluded_dependencies(
-        self, streamlit_requirements_txt, temp_test_directory: str
+        self, correct_requirements_txt: str, temp_test_directory_with_chdir: str
     ):
-        os.chdir(temp_test_directory)
+
         result = utils.generate_streamlit_environment_file(
-            test_data.excluded_anaconda_deps
+            test_data.excluded_anaconda_deps, correct_requirements_txt
         )
-        os.chdir("..")
-        env_file = os.path.join(temp_test_directory, "environment.yml")
+
+        env_file = os.path.join(temp_test_directory_with_chdir, "environment.yml")
         assert result == PosixPath("environment.yml")
         assert os.path.isfile(env_file)
         with open(env_file, "r") as f:
             for dep in test_data.excluded_anaconda_deps:
                 assert dep not in f.read()
 
     def test_generate_streamlit_package_wrapper(self):
@@ -194,81 +195,107 @@
         assert os.path.isfile(path)
         with open(path) as coverage_file:
             assert (
                 "return awesomeModule.even_better_function(*args,**kwargs)"
                 in coverage_file.read()
             )
 
-    def test_add_file_to_existing_zip(
-        self, correct_app_zip: str, correct_requirements_txt: str
-    ):
-        utils.add_file_to_existing_zip(correct_app_zip, correct_requirements_txt)
-        zip_file = ZipFile(correct_app_zip)
+    def test_add_file_to_existing_zip(self, app_zip, correct_requirements_txt: str):
+        utils.add_file_to_existing_zip(app_zip, correct_requirements_txt)
+        zip_file = ZipFile(app_zip)
 
         assert os.path.basename(correct_requirements_txt) in zip_file.namelist()
 
     def test_recursive_zip_packages(
         self,
-        temp_test_directory: str,
-        file_in_a_subdir: str,
-        file_in_other_directory: str,
+        temp_test_directory_with_chdir: str,
+        txt_file_in_a_subdir: str,
+        temp_file_in_other_directory: str,
     ):
-        zip_file_path = os.path.join(temp_test_directory, "packed.zip")
+        zip_file_path = os.path.join(temp_test_directory_with_chdir, "packed.zip")
+
+        utils.recursive_zip_packages_dir(temp_test_directory_with_chdir, zip_file_path)
 
-        utils.recursive_zip_packages_dir(temp_test_directory, zip_file_path)
         zip_file = ZipFile(zip_file_path)
 
         assert os.path.isfile(zip_file_path)
         assert os.getenv("SNOWCLI_INCLUDE_PATHS") is None
-        assert (os.path.join(self.SUBDIR, self.FILE_IN_A_SUBDIR)) in zip_file.namelist()
         assert (
-            os.path.join(self.SECOND_TEST_DIRECTORY, self.FILE_IN_SECOND_TEST_DIRECTORY)
-            not in zip_file.namelist()
+            str(Path(txt_file_in_a_subdir).relative_to(temp_test_directory_with_chdir))
+            in zip_file.namelist()
         )
+        assert Path(temp_file_in_other_directory).name not in zip_file.namelist()
+        assert zip_file_path not in zip_file.namelist()
 
     def test_recursive_zip_packages_with_env_variable(
         self,
         temp_test_directory: str,
-        file_in_a_subdir: str,
+        txt_file_in_a_subdir: str,
         other_directory: str,
-        file_in_other_directory: str,
+        temp_file_in_other_directory,
         include_paths_env_variable,
     ):
         zip_file_path = os.path.join(temp_test_directory, "packed.zip")
 
         utils.recursive_zip_packages_dir(temp_test_directory, zip_file_path)
         zip_file = ZipFile(zip_file_path)
 
         assert os.path.isfile(zip_file_path)
-        assert (os.path.join(self.SUBDIR, self.FILE_IN_A_SUBDIR)) in zip_file.namelist()
-        assert os.path.join(self.FILE_IN_SECOND_TEST_DIRECTORY) in zip_file.namelist()
+        assert (
+            str(Path(txt_file_in_a_subdir).relative_to(temp_test_directory))
+            in zip_file.namelist()
+        )
+        assert str(Path(temp_file_in_other_directory).name) in zip_file.namelist()
 
-    def test_standard_zip_dir(self, temp_test_directory: str, file_in_a_subdir: str):
+    def test_standard_zip_dir(
+        self, temp_test_directory: str, txt_file_in_a_subdir: str
+    ):
         zip_file_path = os.path.join(temp_test_directory, "packed.zip")
         utils.standard_zip_dir(zip_file_path)
         zip_file = ZipFile(zip_file_path)
 
         assert os.path.isfile(zip_file_path)
         assert (
-            os.path.join("subdir", os.path.basename(file_in_a_subdir))
+            os.path.join(self.SUBDIR, os.path.basename(txt_file_in_a_subdir))
             not in zip_file.namelist()
         )
 
-    def test_get_snowflake_packages(self, streamlit_requirements_txt):
-        os.chdir(".tests")
+    def test_standard_zip_dir_with_env_variable(
+        self,
+        temp_test_directory: str,
+        txt_file_in_a_subdir: str,
+        include_paths_env_variable,
+        other_directory: str,
+        temp_file_in_other_directory,
+    ):
+        zip_file_path = os.path.join(temp_test_directory, "packed.zip")
+        utils.standard_zip_dir(zip_file_path)
+        zip_file = ZipFile(zip_file_path)
+
+        assert os.path.isfile(zip_file_path)
+        assert (
+            os.path.join("subdir", os.path.basename(txt_file_in_a_subdir))
+            not in zip_file.namelist()
+        )
+        assert Path(temp_file_in_other_directory).name in zip_file.namelist()
+
+    def test_get_snowflake_packages(
+        self, temp_test_directory_with_chdir, correct_requirements_txt
+    ):
+
         result = utils.get_snowflake_packages()
-        os.chdir("..")
 
         assert result == test_data.requirements
 
-    def test_get_snowflake_packages_delta(self, streamlit_requirements_txt):
+    def test_get_snowflake_packages_delta(
+        self, temp_test_directory_with_chdir, correct_requirements_txt
+    ):
         anaconda_package = test_data.requirements[-1]
-        os.chdir(".tests")
+
         result = utils.get_snowflake_packages_delta(anaconda_package)
-        os.chdir("..")
 
         assert result == test_data.requirements[:-1]
 
     def test_convert_resource_details_to_dict(self):
         resource_details = [
             ("packages", "{'name': 'my-awesome-package','version': '1.2.3'}"),
             ("handler", "handler_function"),
@@ -360,80 +387,58 @@
         assert sorted_packages[0].specs == [("==", "0.9.5")]
 
     # Setup functions
     # These functions are used to set up files and directories used in tests
     # and delete them, after the tests are performed
 
     @pytest.fixture
-    def temp_test_directory(self, tmp_path_factory) -> Generator:
-        path = os.path.join(os.getcwd(), self.TEMP_TEST_DIRECTORY)
-        os.mkdir(path)
-        yield path
-        rmtree(self.TEMP_TEST_DIRECTORY)  # We delete whole directory in teardown -
-        # so, no need to delete any of the files separately
+    def temp_test_directory(self) -> Generator:
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            yield tmp_dir
 
     @pytest.fixture
-    def temp_directory_for_app_zip(self, temp_test_directory: str) -> Generator:
-        path = os.path.join(temp_test_directory, self.TEMP_DIR_FOR_APP_ZIP)
-        os.mkdir(path)
-        yield path
+    def temp_test_directory_with_chdir(self, temp_test_directory) -> Generator:
+        initial_dir = os.getcwd()
+        os.chdir(temp_test_directory)
+        yield temp_test_directory
+        os.chdir(initial_dir)
 
     @pytest.fixture
-    def correct_app_zip(self, temp_test_directory: str) -> Generator:
-        path = os.path.join(temp_test_directory, self.APP_ZIP)
-        self.create_file(path, [])
-        yield path
+    def temp_directory_for_app_zip(self, temp_test_directory: str) -> Generator:
+        temp_dir = tempfile.TemporaryDirectory(dir=temp_test_directory)
+        yield temp_dir.name
 
     @pytest.fixture
-    def correct_requirements_txt(self, temp_test_directory: str) -> Generator:
-        path = os.path.join(temp_test_directory, self.REQUIREMENTS_TXT)
-        self.create_file(path, test_data.requirements)
-        yield path
+    def app_zip(self, temp_test_directory: str) -> Generator:
+        yield create_temp_file(".zip", temp_test_directory, [])
 
     @pytest.fixture
-    def streamlit_requirements_txt(self, temp_test_directory: str) -> Generator:
-        path = os.path.join(temp_test_directory, self.REQUIREMENTS_SNOWFLAKE)
-        self.create_file(path, test_data.requirements)
-        yield path
+    def correct_requirements_txt(self, temp_test_directory: str) -> Generator:
+        yield create_named_file(
+            self.REQUIREMENTS_SNOWFLAKE, temp_test_directory, test_data.requirements
+        )
 
     @pytest.fixture
     def correct_metadata_file(self, temp_test_directory: str) -> Generator:
-        path = os.path.join(temp_test_directory, self.CORRECT_METADATA)
-        self.create_file(path, test_data.correct_package_metadata)
-        yield path
+        yield create_temp_file(
+            ".yaml", temp_test_directory, test_data.correct_package_metadata
+        )
 
     @pytest.fixture
-    def file_in_a_subdir(self, temp_test_directory: str) -> Generator:
-        dir_path = os.path.join(temp_test_directory, self.SUBDIR)
-        os.mkdir(dir_path)
-
-        path = os.path.join(dir_path, self.FILE_IN_A_SUBDIR)
-        self.create_file(path, [])
-        yield path
+    def txt_file_in_a_subdir(self, temp_test_directory: str) -> Generator:
+        subdir = tempfile.TemporaryDirectory(dir=temp_test_directory)
+        yield create_temp_file(".txt", subdir.name, [])
 
     @pytest.fixture
     def other_directory(self) -> Generator:
-        current_path = Path(os.getcwd())
-        path = os.path.join(
-            current_path.parent.absolute(), self.SECOND_TEST_DIRECTORY
-        ).lower()
-        os.mkdir(path)
-        yield path
-        rmtree(path)
+        with tempfile.TemporaryDirectory() as tmp:
+            yield tmp
 
     @pytest.fixture
-    def file_in_other_directory(self, other_directory: str) -> Generator:
-        path = os.path.join(other_directory, self.FILE_IN_SECOND_TEST_DIRECTORY)
-        self.create_file(path, [])
-        yield path
+    def temp_file_in_other_directory(self, other_directory: str) -> Generator:
+        yield create_temp_file(".txt", other_directory, [])
 
     @pytest.fixture
     def include_paths_env_variable(self, other_directory: str) -> Generator:
         os.environ["SNOWCLI_INCLUDE_PATHS"] = other_directory
         yield os.environ["SNOWCLI_INCLUDE_PATHS"]
         os.environ.pop("SNOWCLI_INCLUDE_PATHS")
-
-    @staticmethod
-    def create_file(filepath: str, contents: List[str]) -> None:
-        with open(filepath, "w") as new_file:
-            for line in contents:
-                new_file.write(line + "\n")
```

### Comparing `snowflake_cli_labs-1.0.0/tests/__snapshots__/test_snow_connector.ambr` & `snowflake_cli_labs-1.0.1/tests/__snapshots__/test_snow_connector.ambr`

 * *Files 14% similar despite different names*

```diff
@@ -61,24 +61,14 @@
   CREATE SERVICE IF NOT EXISTS nameValue
     MIN_INSTANCES = 42
     MAX_INSTANCES = 42
     COMPUTE_POOL =  compute_poolValue
     spec=@stageValue/services/4231/test_spec.yaml;
   '''
 # ---
-# name: test_create_stage
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  create stage if not exists nameValue;
-  '''
-# ---
 # name: test_create_streamlit
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   create streamlit nameValue
@@ -211,31 +201,21 @@
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   DROP SERVICE nameValue;
   '''
 # ---
-# name: test_drop_stage
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  drop stage nameValue;
-  '''
-# ---
 # name: test_drop_streamlit
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
-  drop streamlit "nameValue";
+  drop streamlit nameValue;
   '''
 # ---
 # name: test_execute_function
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
@@ -248,34 +228,14 @@
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   call procedureValue;
   '''
 # ---
-# name: test_get_stage[namedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  get @namedStageValue file://pathValue/
-  '''
-# ---
-# name: test_get_stage[snow://embeddedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  get snow://embeddedStageValue file://pathValue/
-  '''
-# ---
 # name: test_job_service
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
@@ -324,41 +284,14 @@
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   show services;
   '''
 # ---
-# name: test_list_stage[namedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  ls @namedStageValue;
-  '''
-# ---
-# name: test_list_stage[snow://embeddedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  ls snow://embeddedStageValue;
-  '''
-# ---
-# name: test_list_stages
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  show stages;
-  '''
-# ---
 # name: test_list_streamlits
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show streamlits;
@@ -380,58 +313,14 @@
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   call SYSTEM$GET_SERVICE_LOGS('nameValue', '0', 'container_nameValue');
   '''
 # ---
-# name: test_put_stage[namedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  
-  
-  put file://pathValue @namedStageValue auto_compress=false parallel=42 overwrite=True;
-  '''
-# ---
-# name: test_put_stage[snow://embeddedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  
-  
-  put file://pathValue snow://embeddedStageValue auto_compress=false parallel=42 overwrite=True;
-  '''
-# ---
-# name: test_remove_from_stage[namedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  remove @namedStageValue/pathValue
-  '''
-# ---
-# name: test_remove_from_stage[snow://embeddedStageValue]
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  
-  remove snow://embeddedStageValue/pathValue
-  '''
-# ---
 # name: test_set_procedure_comment
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   alter PROCEDURE signatureValue SET COMMENT = $$commentValue$$;
@@ -443,23 +332,14 @@
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   grant usage on streamlit nameValue to role to_roleValue;
   '''
 # ---
-# name: test_show_warehouses
-  '''
-  use role roleValue;
-  use warehouse warehouseValue;
-  use database databaseValue;
-  use schema schemaValue;
-  show warehouses;
-  '''
-# ---
 # name: test_status_job
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
```

### Comparing `snowflake_cli_labs-1.0.0/tests/output/test_printing.py` & `snowflake_cli_labs-1.0.1/tests/output/test_printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/anaconda_channel_data.json` & `snowflake_cli_labs-1.0.1/tests/test_data/anaconda_channel_data.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/test_data.py` & `snowflake_cli_labs-1.0.1/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `snowflake_cli_labs-1.0.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/tests_integration/test_warehouse.py` & `snowflake_cli_labs-1.0.1/tests_integration/test_warehouse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 
 from unittest import mock
 from tests_integration.snowflake_connector import snowflake_session
 
 
 @pytest.mark.integration
-@mock.patch("snowcli.cli.warehouse.print_db_cursor")
+@mock.patch("snowcli.output.decorators.print_db_cursor")
 def test_warehouse_status_query(mock_print, runner, snowflake_session):
-    runner.invoke_with_config(["warehouse", "status"])
+    runner.invoke_with_config_and_integration_connection(["warehouse", "status"])
 
     expected_results = snowflake_session.execute_string("show warehouses")[-1]
     result_names = _get_name_values_from_cursor(mock_print.call_args.args[0])
     expected_names = _get_name_values_from_cursor(expected_results)
     assert result_names == expected_names
```

### Comparing `snowflake_cli_labs-1.0.0/LICENSE` & `snowflake_cli_labs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-1.0.0/README.md` & `snowflake_cli_labs-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Snowflake Developer CLI
 
-This is an open source and community supported tool. Support is provided on a best effort basis by project contributors.
-
 **Note**: Snowflake CLI is in Private Preview (PrPr). You must register for the PrPr to use Snowflake CLI by filling out the
 [Snowflake CLI  - PrPr Intake Form](https://forms.gle/HZNhPNbzn7oExjFu8). Also, if you want to access Snowflake Container
 Services through Snowflake CLI, you must register for its PrPr. For more information, you can contact a
 Snowflake sales representative.
 
 For complete installation and usage instructions, refer to the
 [Snowflake CLI Guide](https://docs.snowflake.com/LIMITEDACCESS/snowcli/snowcli-guide).
@@ -14,18 +12,14 @@
 
 Snowflake CLI is a command line interface for working with Snowflake. It lets you create, manage, update, and view apps running in Snowflake.
 
 This is an open source project and contributions are welcome (though the project is maintained on a best-effort basis).
 
 We plan to incorporate some patterns and features of this CLI into the Snowflake CLI (SnowSQL) in the future. We hope this project starts a conversation about what a delightful developer experience could look like, and we'd love your help in shaping that with us!
 
-### Tour and quickstart
-
-[![Snowflake CLI overview and quickstart demo](https://i.imgur.com/tqLVPWnm.png)](https://youtu.be/WDuBeAgbTt4)
-
 ## Benefits of Snowflake CLI
 
 Snowflake CLI lets you locally run and debug Snowflake apps, and has the following benefits:
 
 - Search, create, and upload python packages that may not be yet supported in Anaconda.
 - Has support for Snowpark Python **user defined functions** and **stored procedures**, **warehouses**, and **Streamlit** apps.
 - Define packages using `requirements.txt`, with dependencies automatically added via integration with Anaconda at deploy time.
@@ -209,8 +203,9 @@
 SNOWFLAKE_CONNECTIONS_MYCONNECTION_PASSWORD=pass1234
 ```
 
 In these two examples, Snowflake CLI uses the password "pass1234".
 
 ## Get involved
 
-Have a feature idea? Running into a bug? Want to contribute? We'd love to hear from you! Please open or review issues, open pull requests, or reach out to us on Twitter or LinkedIn [@jeffhollan](https://twitter.com/jeffhollan) and [@jroes](https://twitter.com/jroes).
+Have a feature idea? Running into a bug? Want to contribute? We'd love to hear from you!
+Please open or review issues, open pull requests, or reach out to us on developers@snowflake.com
```

### Comparing `snowflake_cli_labs-1.0.0/pyproject.toml` & `snowflake_cli_labs-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 requires-python = ">=3.8"
 description = "Snowflake CLI"
 readme = "README.md"
 dependencies = [
   "coverage==7.2.7",
   "jinja2==3.1.2",
   "rich==13.4.2",
-  "requests==2.28.1",
+  "requests==2.31.0",
   "requirements-parser==0.5.0",
 #  "snowflake-connector-python==3.0.4",
-  "snowflake-connector-python-nightly==2023.6.24",
+  "snowflake-connector-python-nightly[secure-local-storage]==2023.6.24",
   "tomlkit==0.11.8",
   "typer==0.9.0",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
@@ -32,26 +32,27 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: SQL",
   "Topic :: Database"
 ]
 
 [project.optional-dependencies]
 dev = [
+  "coverage==7.2.7",
   "pre-commit==3.3.3",
   "pytest==7.4.0",
-  "syrupy==4.0.4",
+  "syrupy==4.0.8",
   "tox==4.6.3",
 ]
 
 [project.urls]
 "Source code" = "https://github.com/Snowflake-Labs/snowcli"
 "Bug Tracker" = "https://github.com/Snowflake-Labs/snowcli/issues"
 
 [project.scripts]
-snow = "snowcli.cli:app"
+snow = "snowcli.__main__:main"
 
 [tool.hatch.version]
 path = "src/snowcli/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
```

### Comparing `snowflake_cli_labs-1.0.0/PKG-INFO` & `snowflake_cli_labs-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-cli-labs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Snowflake CLI
 Project-URL: Source code, https://github.com/Snowflake-Labs/snowcli
 Project-URL: Bug Tracker, https://github.com/Snowflake-Labs/snowcli/issues
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -14,31 +14,30 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Requires-Python: >=3.8
 Requires-Dist: coverage==7.2.7
 Requires-Dist: jinja2==3.1.2
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: requirements-parser==0.5.0
 Requires-Dist: rich==13.4.2
-Requires-Dist: snowflake-connector-python-nightly==2023.6.24
+Requires-Dist: snowflake-connector-python-nightly[secure-local-storage]==2023.6.24
 Requires-Dist: tomlkit==0.11.8
 Requires-Dist: typer==0.9.0
 Provides-Extra: dev
+Requires-Dist: coverage==7.2.7; extra == 'dev'
 Requires-Dist: pre-commit==3.3.3; extra == 'dev'
 Requires-Dist: pytest==7.4.0; extra == 'dev'
-Requires-Dist: syrupy==4.0.4; extra == 'dev'
+Requires-Dist: syrupy==4.0.8; extra == 'dev'
 Requires-Dist: tox==4.6.3; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Snowflake Developer CLI
 
-This is an open source and community supported tool. Support is provided on a best effort basis by project contributors.
-
 **Note**: Snowflake CLI is in Private Preview (PrPr). You must register for the PrPr to use Snowflake CLI by filling out the
 [Snowflake CLI  - PrPr Intake Form](https://forms.gle/HZNhPNbzn7oExjFu8). Also, if you want to access Snowflake Container
 Services through Snowflake CLI, you must register for its PrPr. For more information, you can contact a
 Snowflake sales representative.
 
 For complete installation and usage instructions, refer to the
 [Snowflake CLI Guide](https://docs.snowflake.com/LIMITEDACCESS/snowcli/snowcli-guide).
@@ -47,18 +46,14 @@
 
 Snowflake CLI is a command line interface for working with Snowflake. It lets you create, manage, update, and view apps running in Snowflake.
 
 This is an open source project and contributions are welcome (though the project is maintained on a best-effort basis).
 
 We plan to incorporate some patterns and features of this CLI into the Snowflake CLI (SnowSQL) in the future. We hope this project starts a conversation about what a delightful developer experience could look like, and we'd love your help in shaping that with us!
 
-### Tour and quickstart
-
-[![Snowflake CLI overview and quickstart demo](https://i.imgur.com/tqLVPWnm.png)](https://youtu.be/WDuBeAgbTt4)
-
 ## Benefits of Snowflake CLI
 
 Snowflake CLI lets you locally run and debug Snowflake apps, and has the following benefits:
 
 - Search, create, and upload python packages that may not be yet supported in Anaconda.
 - Has support for Snowpark Python **user defined functions** and **stored procedures**, **warehouses**, and **Streamlit** apps.
 - Define packages using `requirements.txt`, with dependencies automatically added via integration with Anaconda at deploy time.
@@ -242,8 +237,9 @@
 SNOWFLAKE_CONNECTIONS_MYCONNECTION_PASSWORD=pass1234
 ```
 
 In these two examples, Snowflake CLI uses the password "pass1234".
 
 ## Get involved
 
-Have a feature idea? Running into a bug? Want to contribute? We'd love to hear from you! Please open or review issues, open pull requests, or reach out to us on Twitter or LinkedIn [@jeffhollan](https://twitter.com/jeffhollan) and [@jroes](https://twitter.com/jroes).
+Have a feature idea? Running into a bug? Want to contribute? We'd love to hear from you!
+Please open or review issues, open pull requests, or reach out to us on developers@snowflake.com
```

