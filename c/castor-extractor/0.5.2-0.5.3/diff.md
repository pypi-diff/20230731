# Comparing `tmp/castor_extractor-0.5.2.tar.gz` & `tmp/castor_extractor-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castor_extractor-0.5.2.tar", max compression
+gzip compressed data, was "castor_extractor-0.5.3.tar", max compression
```

## Comparing `castor_extractor-0.5.2.tar` & `castor_extractor-0.5.3.tar`

### file list

```diff
@@ -1,277 +1,278 @@
--rw-r--r--   0        0        0     5356 2023-07-13 12:59:29.549320 castor_extractor-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     8254 2023-07-13 12:59:29.549320 castor_extractor-0.5.2/LICENCE
--rw-r--r--   0        0        0     3423 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/README.md
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.696321 castor_extractor-0.5.2/castor_extractor/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.696321 castor_extractor-0.5.2/castor_extractor/commands/__init__.py
--rw-r--r--   0        0        0     1252 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_bigquery.py
--rwxr-xr-x   0        0        0     1075 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_looker.py
--rwxr-xr-x   0        0        0      761 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_metabase_api.py
--rwxr-xr-x   0        0        0     1235 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_metabase_db.py
--rwxr-xr-x   0        0        0      919 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_mode.py
--rw-r--r--   0        0        0     1154 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_postgres.py
--rw-r--r--   0        0        0      850 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_powerbi.py
--rw-r--r--   0        0        0      989 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_qlik.py
--rwxr-xr-x   0        0        0     1155 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_redshift.py
--rw-r--r--   0        0        0      703 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_sigma.py
--rwxr-xr-x   0        0        0     1799 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_snowflake.py
--rwxr-xr-x   0        0        0     1390 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/extract_tableau.py
--rw-r--r--   0        0        0     2667 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/file_check.py
--rwxr-xr-x   0        0        0     1930 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/commands/upload.py
--rw-r--r--   0        0        0      119 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/file_checker/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/file_checker/column.py
--rw-r--r--   0        0        0     1935 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/file_checker/column_test.py
--rw-r--r--   0        0        0      289 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/file_checker/constants.py
--rw-r--r--   0        0        0      536 2023-07-13 12:59:29.550320 castor_extractor-0.5.2/castor_extractor/file_checker/enums.py
--rw-r--r--   0        0        0     6537 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/file_checker/file.py
--rw-r--r--   0        0        0     2082 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/file_checker/file_test.py
--rw-r--r--   0        0        0      547 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/file_checker/file_test_users.csv
--rw-r--r--   0        0        0      286 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/file_checker/file_test_users_valid.csv
--rw-r--r--   0        0        0       60 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/file_checker/templates/__init__.py
--rw-r--r--   0        0        0     2967 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/file_checker/templates/generic_warehouse.py
--rw-r--r--   0        0        0      886 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/logger.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.696321 castor_extractor-0.5.2/castor_extractor/transformation/__init__.py
--rw-r--r--   0        0        0       91 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/transformation/dbt/__init__.py
--rw-r--r--   0        0        0       94 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/transformation/dbt/assets.py
--rw-r--r--   0        0        0       86 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/transformation/dbt/client/__init__.py
--rw-r--r--   0        0        0     2938 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/transformation/dbt/client/client.py
--rw-r--r--   0        0        0      746 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/transformation/dbt/client/credentials.py
--rw-r--r--   0        0        0      170 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/types.py
--rw-r--r--   0        0        0       75 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/__init__.py
--rw-r--r--   0        0        0      718 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/constant.py
--rw-r--r--   0        0        0      878 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/env.py
--rw-r--r--   0        0        0      472 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/env_test.py
--rw-r--r--   0        0        0     3353 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/upload.py
--rw-r--r--   0        0        0      329 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/upload_test.py
--rw-r--r--   0        0        0      478 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/uploader/utils.py
--rw-r--r--   0        0        0      929 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/utils/__init__.py
--rw-r--r--   0        0        0      417 2023-07-13 12:59:29.551319 castor_extractor-0.5.2/castor_extractor/utils/collection.py
--rw-r--r--   0        0        0       39 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/constants.py
--rw-r--r--   0        0        0      818 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/deprecate.py
--rw-r--r--   0        0        0      608 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/env.py
--rw-r--r--   0        0        0     1545 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/files.py
--rw-r--r--   0        0        0     1514 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/files_test.py
--rw-r--r--   0        0        0     4616 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/formatter.py
--rw-r--r--   0        0        0     3802 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/formatter_test.csv
--rw-r--r--   0        0        0    12527 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/formatter_test.json
--rw-r--r--   0        0        0     1543 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/formatter_test.py
--rw-r--r--   0        0        0      265 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/load.py
--rw-r--r--   0        0        0     1987 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/object.py
--rw-r--r--   0        0        0     2487 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/object_test.py
--rw-r--r--   0        0        0     3894 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/pager.py
--rw-r--r--   0        0        0     3245 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/pager_test.py
--rw-r--r--   0        0        0     2664 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/retry.py
--rw-r--r--   0        0        0     1635 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/retry_test.py
--rw-r--r--   0        0        0     1966 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/safe.py
--rw-r--r--   0        0        0     2160 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/safe_test.py
--rw-r--r--   0        0        0     2092 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/store.py
--rw-r--r--   0        0        0     1961 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/string.py
--rw-r--r--   0        0        0     2206 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/string_test.py
--rw-r--r--   0        0        0      903 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/time.py
--rw-r--r--   0        0        0      313 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/type.py
--rw-r--r--   0        0        0      150 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/uri.py
--rw-r--r--   0        0        0      259 2023-07-13 12:59:29.552320 castor_extractor-0.5.2/castor_extractor/utils/uri_test.py
--rw-r--r--   0        0        0     1904 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/utils/validation.py
--rw-r--r--   0        0        0     1181 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/utils/validation_test.py
--rw-r--r--   0        0        0     2135 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/utils/write.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.698321 castor_extractor-0.5.2/castor_extractor/visualization/__init__.py
--rw-r--r--   0        0        0      191 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/__init__.py
--rw-r--r--   0        0        0      181 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/__init__.py
--rw-r--r--   0        0        0     8859 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/client.py
--rw-r--r--   0        0        0     1924 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/client_test.py
--rw-r--r--   0        0        0     4049 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/constants.py
--rw-r--r--   0        0        0     3526 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/sdk.py
--rw-r--r--   0        0        0     1742 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/sdk_test.py
--rw-r--r--   0        0        0     1320 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/api/utils.py
--rw-r--r--   0        0        0      400 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/assets.py
--rw-r--r--   0        0        0      467 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/constant.py
--rw-r--r--   0        0        0      864 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/env.py
--rw-r--r--   0        0        0     3685 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/extract.py
--rw-r--r--   0        0        0      636 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/fields.py
--rw-r--r--   0        0        0      782 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/fields_test.py
--rw-r--r--   0        0        0     1527 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/looker/parameters.py
--rw-r--r--   0        0        0      125 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/metabase/__init__.py
--rw-r--r--   0        0        0     2814 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/metabase/assets.py
--rw-r--r--   0        0        0       52 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/__init__.py
--rw-r--r--   0        0        0       30 2023-07-13 12:59:29.553320 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/api/__init__.py
--rw-r--r--   0        0        0     5609 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/api/client.py
--rw-r--r--   0        0        0     1334 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/api/credentials.py
--rw-r--r--   0        0        0       29 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/__init__.py
--rw-r--r--   0        0        0     4091 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/client.py
--rw-r--r--   0        0        0     1863 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/credentials.py
--rw-r--r--   0        0        0       76 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
--rw-r--r--   0        0        0       79 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
--rw-r--r--   0        0        0      419 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/card.sql
--rw-r--r--   0        0        0       42 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/collection.sql
--rw-r--r--   0        0        0      439 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
--rw-r--r--   0        0        0       52 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
--rw-r--r--   0        0        0       49 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/database.sql
--rw-r--r--   0        0        0       46 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/table.sql
--rw-r--r--   0        0        0       41 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/queries/user.sql
--rw-r--r--   0        0        0     1076 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/decryption.py
--rw-r--r--   0        0        0      591 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/decryption_test.py
--rw-r--r--   0        0        0      389 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/shared.py
--rw-r--r--   0        0        0     1006 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/errors.py
--rw-r--r--   0        0        0     1773 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/extract.py
--rw-r--r--   0        0        0       45 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/metabase/types.py
--rw-r--r--   0        0        0      117 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/mode/__init__.py
--rw-r--r--   0        0        0     1552 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/mode/assets.py
--rw-r--r--   0        0        0       27 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/mode/client/__init__.py
--rw-r--r--   0        0        0     7803 2023-07-13 12:59:29.554319 castor_extractor-0.5.2/castor_extractor/visualization/mode/client/client.py
--rw-r--r--   0        0        0     2087 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/mode/client/client_test.json
--rw-r--r--   0        0        0     1400 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/mode/client/client_test.py
--rw-r--r--   0        0        0      453 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/mode/client/constants.py
--rw-r--r--   0        0        0     1622 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/mode/client/credentials.py
--rw-r--r--   0        0        0     1495 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/mode/errors.py
--rw-r--r--   0        0        0     1559 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/mode/extract.py
--rw-r--r--   0        0        0      106 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/__init__.py
--rw-r--r--   0        0        0      449 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/assets.py
--rw-r--r--   0        0        0       62 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/__init__.py
--rw-r--r--   0        0        0     2142 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/constants.py
--rw-r--r--   0        0        0      501 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/credentials.py
--rw-r--r--   0        0        0      720 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/credentials_test.py
--rw-r--r--   0        0        0     7084 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/rest.py
--rw-r--r--   0        0        0     6142 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/rest_test.py
--rw-r--r--   0        0        0      541 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/utils.py
--rw-r--r--   0        0        0      719 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/utils_test.py
--rw-r--r--   0        0        0     1616 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/powerbi/extract.py
--rw-r--r--   0        0        0      143 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/assets.py
--rw-r--r--   0        0        0       94 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/__init__.py
--rw-r--r--   0        0        0      786 2023-07-13 12:59:29.555320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/constants.py
--rw-r--r--   0        0        0       36 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/__init__.py
--rw-r--r--   0        0        0     2512 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/client.py
--rw-r--r--   0        0        0      707 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/constants.py
--rw-r--r--   0        0        0     1229 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/error.py
--rw-r--r--   0        0        0     1005 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/error_test.py
--rw-r--r--   0        0        0     1386 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/json_rpc.py
--rw-r--r--   0        0        0     1305 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
--rw-r--r--   0        0        0     2032 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/websocket.py
--rw-r--r--   0        0        0     3209 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/master.py
--rw-r--r--   0        0        0     5966 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/rest.py
--rw-r--r--   0        0        0     1676 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/rest_test.py
--rw-r--r--   0        0        0       95 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/constants.py
--rw-r--r--   0        0        0     2397 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/qlik/extract.py
--rw-r--r--   0        0        0      130 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/__init__.py
--rw-r--r--   0        0        0      246 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/assets.py
--rw-r--r--   0        0        0       90 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/__init__.py
--rw-r--r--   0        0        0     6311 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/client.py
--rw-r--r--   0        0        0     1529 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/client_test.py
--rw-r--r--   0        0        0      769 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/credentials.py
--rw-r--r--   0        0        0     1157 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/endpoints.py
--rw-r--r--   0        0        0      667 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/pagination.py
--rw-r--r--   0        0        0      130 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/constants.py
--rw-r--r--   0        0        0     2661 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/sigma/extract.py
--rw-r--r--   0        0        0      114 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/__init__.py
--rw-r--r--   0        0        0      762 2023-07-13 12:59:29.556320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/assets.py
--rw-r--r--   0        0        0       78 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/__init__.py
--rw-r--r--   0        0        0     6824 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/client.py
--rw-r--r--   0        0        0     2077 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/client_utils.py
--rw-r--r--   0        0        0     3335 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/credentials.py
--rw-r--r--   0        0        0      803 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/project.py
--rw-r--r--   0        0        0     2036 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/safe_mode.py
--rw-r--r--   0        0        0      126 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/constants.py
--rw-r--r--   0        0        0       91 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/errors.py
--rw-r--r--   0        0        0     2873 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/extract.py
--rw-r--r--   0        0        0     4728 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/gql_fields.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.708321 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.708321 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/__init__.py
--rw-r--r--   0        0        0      446 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
--rw-r--r--   0        0        0      447 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
--rw-r--r--   0        0        0      450 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
--rw-r--r--   0        0        0     1018 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
--rw-r--r--   0        0        0      679 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
--rw-r--r--   0        0        0     1415 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
--rw-r--r--   0        0        0     1325 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.708321 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
--rw-r--r--   0        0        0     1917 2023-07-13 12:59:29.557320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.708321 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
--rw-r--r--   0        0        0      422 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
--rw-r--r--   0        0        0     1779 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
--rw-r--r--   0        0        0     1384 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
--rw-r--r--   0        0        0     1499 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
--rw-r--r--   0        0        0     1979 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
--rw-r--r--   0        0        0       26 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
--rw-r--r--   0        0        0      966 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/tsc_fields.py
--rw-r--r--   0        0        0      322 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/types.py
--rw-r--r--   0        0        0      427 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/visualization/tableau/usage.py
--rw-r--r--   0        0        0        0 2023-07-13 12:59:29.715322 castor_extractor-0.5.2/castor_extractor/warehouse/__init__.py
--rw-r--r--   0        0        0      386 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/asset.py
--rw-r--r--   0        0        0     1947 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/client.py
--rw-r--r--   0        0        0     2885 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/extract.py
--rw-r--r--   0        0        0     2640 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/query.py
--rw-r--r--   0        0        0      935 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/time_filter.py
--rw-r--r--   0        0        0      449 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/abstract/time_filter_test.py
--rw-r--r--   0        0        0      125 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/__init__.py
--rw-r--r--   0        0        0     3062 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/client.py
--rw-r--r--   0        0        0     1567 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/client_test.py
--rw-r--r--   0        0        0     2800 2023-07-13 12:59:29.558320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/extract.py
--rw-r--r--   0        0        0       30 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/.sqlfluff
--rw-r--r--   0        0        0     1815 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/column.sql
--rw-r--r--   0        0        0     1347 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
--rw-r--r--   0        0        0      207 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/database.sql
--rw-r--r--   0        0        0      660 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/query.sql
--rw-r--r--   0        0        0      284 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/schema.sql
--rw-r--r--   0        0        0     1508 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/table.sql
--rw-r--r--   0        0        0     2660 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
--rw-r--r--   0        0        0      189 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/user.sql
--rw-r--r--   0        0        0      326 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
--rw-r--r--   0        0        0     4147 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/query.py
--rw-r--r--   0        0        0      140 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/types.py
--rw-r--r--   0        0        0      125 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/__init__.py
--rw-r--r--   0        0        0      871 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/client.py
--rw-r--r--   0        0        0     2099 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/extract.py
--rw-r--r--   0        0        0       30 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/.sqlfluff
--rw-r--r--   0        0        0     1632 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/column.sql
--rw-r--r--   0        0        0      241 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/database.sql
--rw-r--r--   0        0        0      101 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/group.sql
--rw-r--r--   0        0        0      592 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/schema.sql
--rw-r--r--   0        0        0     1489 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/table.sql
--rw-r--r--   0        0        0      170 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/user.sql
--rw-r--r--   0        0        0      540 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/postgres/query.py
--rw-r--r--   0        0        0      125 2023-07-13 12:59:29.559320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/__init__.py
--rw-r--r--   0        0        0      764 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/client.py
--rw-r--r--   0        0        0     1028 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/client_test.py
--rw-r--r--   0        0        0     2238 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/extract.py
--rw-r--r--   0        0        0       30 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/.sqlfluff
--rw-r--r--   0        0        0     7044 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/column.sql
--rw-r--r--   0        0        0      299 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/database.sql
--rw-r--r--   0        0        0      101 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/group.sql
--rw-r--r--   0        0        0     3258 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/query.sql
--rw-r--r--   0        0        0      585 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/schema.sql
--rw-r--r--   0        0        0     2645 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/table.sql
--rw-r--r--   0        0        0      726 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/table_freshness.sql
--rw-r--r--   0        0        0      170 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/user.sql
--rw-r--r--   0        0        0      719 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/view_ddl.sql
--rw-r--r--   0        0        0      540 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/redshift/query.py
--rw-r--r--   0        0        0      128 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/__init__.py
--rw-r--r--   0        0        0     4128 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/client.py
--rw-r--r--   0        0        0     1434 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/client_test.py
--rw-r--r--   0        0        0     2443 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/extract.py
--rw-r--r--   0        0        0       31 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/.sqlfluff
--rw-r--r--   0        0        0     1130 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/column.sql
--rw-r--r--   0        0        0     1179 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
--rw-r--r--   0        0        0      483 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/database.sql
--rw-r--r--   0        0        0      272 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
--rw-r--r--   0        0        0      143 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
--rw-r--r--   0        0        0     1779 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/query.sql
--rw-r--r--   0        0        0       96 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/role.sql
--rw-r--r--   0        0        0      730 2023-07-13 12:59:29.560320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/schema.sql
--rw-r--r--   0        0        0     1378 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/table.sql
--rw-r--r--   0        0        0      570 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/user.sql
--rw-r--r--   0        0        0      673 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
--rw-r--r--   0        0        0     1769 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/query.py
--rw-r--r--   0        0        0       36 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/__init__.py
--rw-r--r--   0        0        0      517 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/extract.py
--rw-r--r--   0        0        0       26 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/.sqlfluff
--rw-r--r--   0        0        0     1392 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/column.sql
--rw-r--r--   0        0        0      138 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/database.sql
--rw-r--r--   0        0        0     1110 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/query.sql
--rw-r--r--   0        0        0      250 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/schema.sql
--rw-r--r--   0        0        0     1049 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/table.sql
--rw-r--r--   0        0        0       67 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/user.sql
--rw-r--r--   0        0        0      249 2023-07-13 12:59:29.561320 castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/view_ddl.sql
--rw-r--r--   0        0        0     5603 2023-07-13 12:59:29.562320 castor_extractor-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 castor_extractor-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     5425 2023-07-31 08:50:07.950733 castor_extractor-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     8254 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/LICENCE
+-rw-r--r--   0        0        0     3423 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.092731 castor_extractor-0.5.3/castor_extractor/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.092731 castor_extractor-0.5.3/castor_extractor/commands/__init__.py
+-rw-r--r--   0        0        0     1252 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_bigquery.py
+-rwxr-xr-x   0        0        0     1075 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_looker.py
+-rwxr-xr-x   0        0        0      761 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_metabase_api.py
+-rwxr-xr-x   0        0        0     1235 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_metabase_db.py
+-rwxr-xr-x   0        0        0      919 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_mode.py
+-rw-r--r--   0        0        0     1154 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_postgres.py
+-rw-r--r--   0        0        0      850 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_powerbi.py
+-rw-r--r--   0        0        0      989 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_qlik.py
+-rwxr-xr-x   0        0        0     1155 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_redshift.py
+-rw-r--r--   0        0        0      703 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_sigma.py
+-rwxr-xr-x   0        0        0     1799 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_snowflake.py
+-rwxr-xr-x   0        0        0     1390 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/extract_tableau.py
+-rw-r--r--   0        0        0     2667 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/file_check.py
+-rwxr-xr-x   0        0        0     1930 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/commands/upload.py
+-rw-r--r--   0        0        0      119 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/file_checker/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/file_checker/column.py
+-rw-r--r--   0        0        0     1935 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/file_checker/column_test.py
+-rw-r--r--   0        0        0      289 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/file_checker/constants.py
+-rw-r--r--   0        0        0      536 2023-07-31 08:50:07.951733 castor_extractor-0.5.3/castor_extractor/file_checker/enums.py
+-rw-r--r--   0        0        0     6537 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/file_checker/file.py
+-rw-r--r--   0        0        0     2082 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/file_checker/file_test.py
+-rw-r--r--   0        0        0      547 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/file_checker/file_test_users.csv
+-rw-r--r--   0        0        0      286 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/file_checker/file_test_users_valid.csv
+-rw-r--r--   0        0        0       60 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/file_checker/templates/__init__.py
+-rw-r--r--   0        0        0     2967 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/file_checker/templates/generic_warehouse.py
+-rw-r--r--   0        0        0      886 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/logger.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.093731 castor_extractor-0.5.3/castor_extractor/transformation/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/transformation/dbt/__init__.py
+-rw-r--r--   0        0        0       94 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/transformation/dbt/assets.py
+-rw-r--r--   0        0        0       86 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/transformation/dbt/client/__init__.py
+-rw-r--r--   0        0        0     2938 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/transformation/dbt/client/client.py
+-rw-r--r--   0        0        0      746 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/transformation/dbt/client/credentials.py
+-rw-r--r--   0        0        0      170 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/types.py
+-rw-r--r--   0        0        0       75 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/__init__.py
+-rw-r--r--   0        0        0      718 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/constant.py
+-rw-r--r--   0        0        0      878 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/env.py
+-rw-r--r--   0        0        0      472 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/env_test.py
+-rw-r--r--   0        0        0     3353 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/upload.py
+-rw-r--r--   0        0        0      329 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/upload_test.py
+-rw-r--r--   0        0        0      478 2023-07-31 08:50:07.952733 castor_extractor-0.5.3/castor_extractor/uploader/utils.py
+-rw-r--r--   0        0        0      967 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/collection.py
+-rw-r--r--   0        0        0       39 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/constants.py
+-rw-r--r--   0        0        0      818 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/deprecate.py
+-rw-r--r--   0        0        0      608 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/env.py
+-rw-r--r--   0        0        0     1545 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/files.py
+-rw-r--r--   0        0        0     1514 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/files_test.py
+-rw-r--r--   0        0        0     4616 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/formatter.py
+-rw-r--r--   0        0        0     3802 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/formatter_test.csv
+-rw-r--r--   0        0        0    12527 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/formatter_test.json
+-rw-r--r--   0        0        0     1543 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/formatter_test.py
+-rw-r--r--   0        0        0      265 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/load.py
+-rw-r--r--   0        0        0     1987 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/object.py
+-rw-r--r--   0        0        0     2487 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/object_test.py
+-rw-r--r--   0        0        0     3894 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/pager.py
+-rw-r--r--   0        0        0     3245 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/pager_test.py
+-rw-r--r--   0        0        0     2664 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/retry.py
+-rw-r--r--   0        0        0     1635 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/retry_test.py
+-rw-r--r--   0        0        0     1966 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/safe.py
+-rw-r--r--   0        0        0     2160 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/safe_test.py
+-rw-r--r--   0        0        0     2092 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/store.py
+-rw-r--r--   0        0        0     1961 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/string.py
+-rw-r--r--   0        0        0     2206 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/string_test.py
+-rw-r--r--   0        0        0     1062 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/time.py
+-rw-r--r--   0        0        0      211 2023-07-31 08:50:07.953733 castor_extractor-0.5.3/castor_extractor/utils/time_test.py
+-rw-r--r--   0        0        0      313 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/utils/type.py
+-rw-r--r--   0        0        0      150 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/utils/uri.py
+-rw-r--r--   0        0        0      259 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/utils/uri_test.py
+-rw-r--r--   0        0        0     1904 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/utils/validation.py
+-rw-r--r--   0        0        0     1181 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/utils/validation_test.py
+-rw-r--r--   0        0        0     2135 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/utils/write.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.095731 castor_extractor-0.5.3/castor_extractor/visualization/__init__.py
+-rw-r--r--   0        0        0      191 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/__init__.py
+-rw-r--r--   0        0        0     8859 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/client.py
+-rw-r--r--   0        0        0     1924 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/client_test.py
+-rw-r--r--   0        0        0     4049 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/constants.py
+-rw-r--r--   0        0        0     3526 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/sdk.py
+-rw-r--r--   0        0        0     1742 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/sdk_test.py
+-rw-r--r--   0        0        0     1320 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/api/utils.py
+-rw-r--r--   0        0        0      400 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/assets.py
+-rw-r--r--   0        0        0      467 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/constant.py
+-rw-r--r--   0        0        0      864 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/env.py
+-rw-r--r--   0        0        0     3685 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/extract.py
+-rw-r--r--   0        0        0      636 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/fields.py
+-rw-r--r--   0        0        0      782 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/fields_test.py
+-rw-r--r--   0        0        0     1527 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/looker/parameters.py
+-rw-r--r--   0        0        0      125 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/__init__.py
+-rw-r--r--   0        0        0     2814 2023-07-31 08:50:07.954733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/assets.py
+-rw-r--r--   0        0        0       52 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/api/__init__.py
+-rw-r--r--   0        0        0     5609 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/api/client.py
+-rw-r--r--   0        0        0     1334 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/api/credentials.py
+-rw-r--r--   0        0        0       29 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/__init__.py
+-rw-r--r--   0        0        0     4091 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/client.py
+-rw-r--r--   0        0        0     1863 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/credentials.py
+-rw-r--r--   0        0        0       76 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
+-rw-r--r--   0        0        0       79 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
+-rw-r--r--   0        0        0      419 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/card.sql
+-rw-r--r--   0        0        0       42 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/collection.sql
+-rw-r--r--   0        0        0      439 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
+-rw-r--r--   0        0        0       52 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
+-rw-r--r--   0        0        0       49 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/database.sql
+-rw-r--r--   0        0        0       46 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/table.sql
+-rw-r--r--   0        0        0       41 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/queries/user.sql
+-rw-r--r--   0        0        0     1076 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/decryption.py
+-rw-r--r--   0        0        0      591 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/decryption_test.py
+-rw-r--r--   0        0        0      389 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/shared.py
+-rw-r--r--   0        0        0     1006 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/errors.py
+-rw-r--r--   0        0        0     1773 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/extract.py
+-rw-r--r--   0        0        0       45 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/metabase/types.py
+-rw-r--r--   0        0        0      117 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/mode/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/mode/assets.py
+-rw-r--r--   0        0        0       27 2023-07-31 08:50:07.955733 castor_extractor-0.5.3/castor_extractor/visualization/mode/client/__init__.py
+-rw-r--r--   0        0        0     7803 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/client/client.py
+-rw-r--r--   0        0        0     2087 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/client/client_test.json
+-rw-r--r--   0        0        0     1400 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/client/client_test.py
+-rw-r--r--   0        0        0      453 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/client/constants.py
+-rw-r--r--   0        0        0     1622 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/client/credentials.py
+-rw-r--r--   0        0        0     1495 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/errors.py
+-rw-r--r--   0        0        0     1559 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/mode/extract.py
+-rw-r--r--   0        0        0      106 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/__init__.py
+-rw-r--r--   0        0        0      504 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/assets.py
+-rw-r--r--   0        0        0       62 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/__init__.py
+-rw-r--r--   0        0        0     2342 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/constants.py
+-rw-r--r--   0        0        0      501 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/credentials.py
+-rw-r--r--   0        0        0      720 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/credentials_test.py
+-rw-r--r--   0        0        0     9383 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/rest.py
+-rw-r--r--   0        0        0     7098 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/rest_test.py
+-rw-r--r--   0        0        0      541 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/utils.py
+-rw-r--r--   0        0        0      719 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/utils_test.py
+-rw-r--r--   0        0        0     1305 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/powerbi/extract.py
+-rw-r--r--   0        0        0      143 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-31 08:50:07.956733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/assets.py
+-rw-r--r--   0        0        0       94 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/__init__.py
+-rw-r--r--   0        0        0      786 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/constants.py
+-rw-r--r--   0        0        0       36 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/__init__.py
+-rw-r--r--   0        0        0     2512 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/client.py
+-rw-r--r--   0        0        0      707 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/constants.py
+-rw-r--r--   0        0        0     1229 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/error.py
+-rw-r--r--   0        0        0     1005 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/error_test.py
+-rw-r--r--   0        0        0     1386 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/json_rpc.py
+-rw-r--r--   0        0        0     1305 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
+-rw-r--r--   0        0        0     2032 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/websocket.py
+-rw-r--r--   0        0        0     3209 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/master.py
+-rw-r--r--   0        0        0     5966 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/rest.py
+-rw-r--r--   0        0        0     1676 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/rest_test.py
+-rw-r--r--   0        0        0       95 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/constants.py
+-rw-r--r--   0        0        0     2397 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/qlik/extract.py
+-rw-r--r--   0        0        0      130 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/assets.py
+-rw-r--r--   0        0        0       90 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/__init__.py
+-rw-r--r--   0        0        0     6311 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/client.py
+-rw-r--r--   0        0        0     1529 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/client_test.py
+-rw-r--r--   0        0        0      769 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/credentials.py
+-rw-r--r--   0        0        0     1157 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/endpoints.py
+-rw-r--r--   0        0        0      667 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/pagination.py
+-rw-r--r--   0        0        0      130 2023-07-31 08:50:07.957733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/constants.py
+-rw-r--r--   0        0        0     2661 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/sigma/extract.py
+-rw-r--r--   0        0        0      114 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/__init__.py
+-rw-r--r--   0        0        0      762 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/assets.py
+-rw-r--r--   0        0        0       78 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/__init__.py
+-rw-r--r--   0        0        0     6824 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/client.py
+-rw-r--r--   0        0        0     2077 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/client_utils.py
+-rw-r--r--   0        0        0     3335 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/credentials.py
+-rw-r--r--   0        0        0      803 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/project.py
+-rw-r--r--   0        0        0     2036 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/safe_mode.py
+-rw-r--r--   0        0        0      126 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/constants.py
+-rw-r--r--   0        0        0       91 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/errors.py
+-rw-r--r--   0        0        0     2873 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/extract.py
+-rw-r--r--   0        0        0     4728 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/gql_fields.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.099731 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.099731 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/__init__.py
+-rw-r--r--   0        0        0      446 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
+-rw-r--r--   0        0        0      447 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
+-rw-r--r--   0        0        0      450 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
+-rw-r--r--   0        0        0     1018 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
+-rw-r--r--   0        0        0      679 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
+-rw-r--r--   0        0        0     1415 2023-07-31 08:50:07.958733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
+-rw-r--r--   0        0        0     1325 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.100731 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
+-rw-r--r--   0        0        0     1917 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.100731 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
+-rw-r--r--   0        0        0      422 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
+-rw-r--r--   0        0        0     1779 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
+-rw-r--r--   0        0        0     1384 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
+-rw-r--r--   0        0        0     1499 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
+-rw-r--r--   0        0        0     1979 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
+-rw-r--r--   0        0        0       26 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
+-rw-r--r--   0        0        0      966 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/tsc_fields.py
+-rw-r--r--   0        0        0      322 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/types.py
+-rw-r--r--   0        0        0      427 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/visualization/tableau/usage.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:50:08.100731 castor_extractor-0.5.3/castor_extractor/warehouse/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/asset.py
+-rw-r--r--   0        0        0     1947 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/client.py
+-rw-r--r--   0        0        0     2885 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/extract.py
+-rw-r--r--   0        0        0     2640 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/query.py
+-rw-r--r--   0        0        0      935 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/time_filter.py
+-rw-r--r--   0        0        0      449 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/abstract/time_filter_test.py
+-rw-r--r--   0        0        0      125 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/__init__.py
+-rw-r--r--   0        0        0     3062 2023-07-31 08:50:07.959733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/client.py
+-rw-r--r--   0        0        0     1567 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/client_test.py
+-rw-r--r--   0        0        0     2800 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/extract.py
+-rw-r--r--   0        0        0       30 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/.sqlfluff
+-rw-r--r--   0        0        0     1815 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/column.sql
+-rw-r--r--   0        0        0     1347 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
+-rw-r--r--   0        0        0      207 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/database.sql
+-rw-r--r--   0        0        0      660 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/query.sql
+-rw-r--r--   0        0        0      284 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/schema.sql
+-rw-r--r--   0        0        0     1508 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/table.sql
+-rw-r--r--   0        0        0     2660 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
+-rw-r--r--   0        0        0      189 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/user.sql
+-rw-r--r--   0        0        0      326 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
+-rw-r--r--   0        0        0     4147 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/query.py
+-rw-r--r--   0        0        0      140 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/types.py
+-rw-r--r--   0        0        0      125 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/__init__.py
+-rw-r--r--   0        0        0      871 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/client.py
+-rw-r--r--   0        0        0     2099 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/extract.py
+-rw-r--r--   0        0        0       30 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/.sqlfluff
+-rw-r--r--   0        0        0     1632 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/column.sql
+-rw-r--r--   0        0        0      241 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/group.sql
+-rw-r--r--   0        0        0      592 2023-07-31 08:50:07.960733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/schema.sql
+-rw-r--r--   0        0        0     1489 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/table.sql
+-rw-r--r--   0        0        0      170 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/user.sql
+-rw-r--r--   0        0        0      540 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/postgres/query.py
+-rw-r--r--   0        0        0      125 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/__init__.py
+-rw-r--r--   0        0        0      764 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/client.py
+-rw-r--r--   0        0        0     1028 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/client_test.py
+-rw-r--r--   0        0        0     2238 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/extract.py
+-rw-r--r--   0        0        0       30 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/.sqlfluff
+-rw-r--r--   0        0        0     7044 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/column.sql
+-rw-r--r--   0        0        0      299 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/group.sql
+-rw-r--r--   0        0        0     3258 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/query.sql
+-rw-r--r--   0        0        0      585 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/schema.sql
+-rw-r--r--   0        0        0     2645 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/table.sql
+-rw-r--r--   0        0        0      726 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/table_freshness.sql
+-rw-r--r--   0        0        0      170 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/user.sql
+-rw-r--r--   0        0        0      719 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/view_ddl.sql
+-rw-r--r--   0        0        0      540 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/redshift/query.py
+-rw-r--r--   0        0        0      128 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/__init__.py
+-rw-r--r--   0        0        0     4128 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/client.py
+-rw-r--r--   0        0        0     1434 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/client_test.py
+-rw-r--r--   0        0        0     2443 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/extract.py
+-rw-r--r--   0        0        0       31 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/.sqlfluff
+-rw-r--r--   0        0        0     1130 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/column.sql
+-rw-r--r--   0        0        0     1179 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
+-rw-r--r--   0        0        0      483 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/database.sql
+-rw-r--r--   0        0        0      272 2023-07-31 08:50:07.961733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
+-rw-r--r--   0        0        0      143 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
+-rw-r--r--   0        0        0     1779 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/query.sql
+-rw-r--r--   0        0        0       96 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/role.sql
+-rw-r--r--   0        0        0      730 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/schema.sql
+-rw-r--r--   0        0        0     1378 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/table.sql
+-rw-r--r--   0        0        0      570 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/user.sql
+-rw-r--r--   0        0        0      673 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
+-rw-r--r--   0        0        0     1769 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/query.py
+-rw-r--r--   0        0        0       36 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/extract.py
+-rw-r--r--   0        0        0       26 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/.sqlfluff
+-rw-r--r--   0        0        0     1392 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/column.sql
+-rw-r--r--   0        0        0      138 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/database.sql
+-rw-r--r--   0        0        0     1110 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/query.sql
+-rw-r--r--   0        0        0      250 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/schema.sql
+-rw-r--r--   0        0        0     1049 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/table.sql
+-rw-r--r--   0        0        0       67 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/user.sql
+-rw-r--r--   0        0        0      249 2023-07-31 08:50:07.962733 castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/view_ddl.sql
+-rw-r--r--   0        0        0     5603 2023-07-31 08:50:07.963733 castor_extractor-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 castor_extractor-0.5.3/PKG-INFO
```

### Comparing `castor_extractor-0.5.2/CHANGELOG.md` & `castor_extractor-0.5.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## 0.5.3 - 2023-07-27
+* Add support for PowerBI's `Activity Events`
+
 ## 0.5.2 - 2023-07-12
 * Fix Metabase DbClient url
 
 ## 0.5.1 - 2023-07-03
 * Add support for Looker's `ContentViews`
 
 ## 0.5.0 - 2023-06-28
```

### Comparing `castor_extractor-0.5.2/LICENCE` & `castor_extractor-0.5.3/LICENCE`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/README.md` & `castor_extractor-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_bigquery.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_bigquery.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_looker.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_looker.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_metabase_api.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_metabase_api.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_metabase_db.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_metabase_db.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_mode.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_postgres.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_postgres.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_powerbi.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_powerbi.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_qlik.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_qlik.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_redshift.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_redshift.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_sigma.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_sigma.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_snowflake.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_snowflake.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/extract_tableau.py` & `castor_extractor-0.5.3/castor_extractor/commands/extract_tableau.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/file_check.py` & `castor_extractor-0.5.3/castor_extractor/commands/file_check.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/commands/upload.py` & `castor_extractor-0.5.3/castor_extractor/commands/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/column.py` & `castor_extractor-0.5.3/castor_extractor/file_checker/column.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/column_test.py` & `castor_extractor-0.5.3/castor_extractor/file_checker/column_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/enums.py` & `castor_extractor-0.5.3/castor_extractor/file_checker/enums.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/file.py` & `castor_extractor-0.5.3/castor_extractor/file_checker/file.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/file_test.py` & `castor_extractor-0.5.3/castor_extractor/file_checker/file_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/file_test_users.csv` & `castor_extractor-0.5.3/castor_extractor/file_checker/file_test_users.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/file_checker/templates/generic_warehouse.py` & `castor_extractor-0.5.3/castor_extractor/file_checker/templates/generic_warehouse.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/logger.py` & `castor_extractor-0.5.3/castor_extractor/logger.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/transformation/dbt/client/client.py` & `castor_extractor-0.5.3/castor_extractor/transformation/dbt/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/transformation/dbt/client/credentials.py` & `castor_extractor-0.5.3/castor_extractor/transformation/dbt/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/uploader/constant.py` & `castor_extractor-0.5.3/castor_extractor/uploader/constant.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/uploader/env.py` & `castor_extractor-0.5.3/castor_extractor/uploader/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/uploader/upload.py` & `castor_extractor-0.5.3/castor_extractor/uploader/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/__init__.py` & `castor_extractor-0.5.3/castor_extractor/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     PagerOnIdLogger,
     PagerStopStrategy,
 )
 from .retry import RetryStrategy, retry
 from .safe import SafeMode, safe_mode
 from .store import AbstractStorage, LocalStorage
 from .string import string_to_tuple
-from .time import current_date, current_datetime, current_timestamp, past_date
+from .time import (
+    at_midnight,
+    current_date,
+    current_datetime,
+    current_timestamp,
+    past_date,
+)
 from .type import Callback, Getter, JsonType, SerializedAsset
 from .uri import uri_encode
 from .validation import validate_baseurl
 from .write import (
     get_output_filename,
     get_summary_filename,
     get_summary_payload,
```

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/deprecate.py` & `castor_extractor-0.5.3/castor_extractor/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/env.py` & `castor_extractor-0.5.3/castor_extractor/utils/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/files.py` & `castor_extractor-0.5.3/castor_extractor/utils/files.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/files_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/formatter.py` & `castor_extractor-0.5.3/castor_extractor/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/formatter_test.csv` & `castor_extractor-0.5.3/castor_extractor/utils/formatter_test.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/formatter_test.json` & `castor_extractor-0.5.3/castor_extractor/utils/formatter_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/formatter_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/formatter_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/object.py` & `castor_extractor-0.5.3/castor_extractor/utils/object.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/object_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/pager.py` & `castor_extractor-0.5.3/castor_extractor/utils/pager.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/pager_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/pager_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/retry.py` & `castor_extractor-0.5.3/castor_extractor/utils/retry.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/retry_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/retry_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/safe.py` & `castor_extractor-0.5.3/castor_extractor/utils/safe.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/safe_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/safe_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/store.py` & `castor_extractor-0.5.3/castor_extractor/utils/store.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/string.py` & `castor_extractor-0.5.3/castor_extractor/utils/string.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/string_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/string_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/time.py` & `castor_extractor-0.5.3/castor_extractor/utils/time.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,7 +32,12 @@
     ts = datetime.utcnow()
     return _set_uct_timezone(ts) if tz else ts
 
 
 def past_date(past_days: int) -> date:
     """returns a date in the past"""
     return now().date() - timedelta(past_days)
+
+
+def at_midnight(date_: date) -> datetime:
+    """convert date into datetime at midnight: 00:00:00"""
+    return datetime.combine(date_, datetime.min.time())
```

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/validation.py` & `castor_extractor-0.5.3/castor_extractor/utils/validation.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/validation_test.py` & `castor_extractor-0.5.3/castor_extractor/utils/validation_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/utils/write.py` & `castor_extractor-0.5.3/castor_extractor/utils/write.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/api/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/api/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/api/client_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/api/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/api/constants.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/api/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/api/sdk.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/api/sdk.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/api/sdk_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/api/sdk_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/api/utils.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/api/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/env.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/fields.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/fields_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/fields_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/looker/parameters.py` & `castor_extractor-0.5.3/castor_extractor/visualization/looker/parameters.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/assets.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/api/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/api/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/api/credentials.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/api/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/db/credentials.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/db/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/decryption.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/decryption.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/client/decryption_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/client/decryption_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/errors.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/metabase/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/metabase/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/assets.py` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/client/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/client/client_test.json` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/client/client_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/client/client_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/client/credentials.py` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/errors.py` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/mode/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/mode/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/constants.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     """PowerBi's urls"""
 
     REST_API_BASE_PATH = "https://api.powerbi.com/v1.0/myorg"
     CLIENT_APP_BASE = "https://login.microsoftonline.com/"
     DEFAULT_SCOPE = "https://analysis.windows.net/powerbi/api/.default"
 
     # PBI rest API Routes
+    ACTIVITY_EVENTS = f"{REST_API_BASE_PATH}/admin/activityevents"
     DATASETS = f"{REST_API_BASE_PATH}/admin/datasets"
     DASHBOARD = f"{REST_API_BASE_PATH}/admin/dashboards"
     GROUPS = f"{REST_API_BASE_PATH}/admin/groups"
     METADATA_POST = f"{REST_API_BASE_PATH}/admin/workspaces/getInfo"
     METADATA_WAIT = f"{REST_API_BASE_PATH}/admin/workspaces/scanStatus"
     METADATA_GET = f"{REST_API_BASE_PATH}/admin/workspaces/scanResult"
     REPORTS = f"{REST_API_BASE_PATH}/admin/reports"
@@ -54,21 +55,24 @@
         "lineage": True,
     }
     ACTIVE_WORKSPACE_FILTER = "state eq 'Active' and type eq 'Workspace'"
 
 
 class Keys:
     ACCESS_TOKEN = "access_token"
-    VALUE = "value"
-    WORKSPACES = "workspaces"
+    ACTIVITY_EVENT_ENTITIES = "activityEventEntities"
+    CONTINUATION_URI = "continuationUri"
+    ID = "id"
     INACTIVE_WORKSPACES = "excludeInActiveWorkspaces"
-    PERSONAL_WORKSPACES = "excludePersonalWorkspaces"
+    LAST_RESULT_SET = "lastResultSet"
     MODIFIED_SINCE = "modifiedSince"
-    ID = "id"
+    PERSONAL_WORKSPACES = "excludePersonalWorkspaces"
     STATUS = "status"
+    VALUE = "value"
+    WORKSPACES = "workspaces"
 
 
 class Assertions:
     """Assertion's messages"""
 
     BATCH_TOO_BIG = f"Can not retrieve more than {Batches.METADATA} at the time"
     DATETIME_TOO_OLD = "Date must be within 30 days range"
```

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/credentials_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/credentials_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/rest.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/rest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
-from datetime import datetime
+from datetime import date, datetime, timedelta
 from time import sleep
-from typing import Any, Callable, Dict, Iterator, List, Optional, Union
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 import msal  # type: ignore
 import requests
 
+from ....utils import at_midnight, current_date
 from ..assets import PowerBiAsset
 from .constants import (
     DEFAULT_TIMEOUT_IN_SECS,
     GET,
     POST,
     SCAN_READY,
     Batches,
@@ -18,14 +19,46 @@
     Urls,
 )
 from .credentials import Credentials
 from .utils import batch_size_is_valid_or_assert, datetime_is_recent_or_assert
 
 logger = logging.getLogger(__name__)
 
+_FORMAT = "%Y-%m-%dT%H:%M:%S"
+
+
+def _format(timestamp: datetime) -> str:
+    return timestamp.strftime(_FORMAT)
+
+
+def _yesterday() -> date:
+    return current_date() - timedelta(days=1)
+
+
+def _time_filter(day: Optional[date]) -> Tuple[datetime, datetime]:
+    target_day = day or _yesterday()
+    start = at_midnight(target_day)
+    end = datetime.combine(target_day, datetime.max.time())
+    return start, end
+
+
+def _url(
+    day: Optional[date],
+    continuation_uri: Optional[str],
+) -> str:
+    if continuation_uri:
+        return continuation_uri
+
+    url = Urls.ACTIVITY_EVENTS
+    start, end = _time_filter(day)
+    url += "?$filter=Activity eq 'viewreport'"
+    url += f"&startDateTime='{_format(start)}'"
+    url += f"&endDateTime='{_format(end)}'"
+    return url
+
 
 class Client:
     """
     PowerBI rest admin api
     https://learn.microsoft.com/en-us/rest/api/power-bi/admin
     """
 
@@ -65,14 +98,15 @@
         processor: Optional[Callable] = None,
     ) -> Any:
         """
         Make either a get or a post http request.Request, by default
         result.json is returned. Optionally you can provide a processor callback
         to transform the result.
         """
+        logger.debug(f"Calling {method} on {url}")
         result = requests.request(
             method, url, headers=self._header(), params=params, data=data
         )
         result.raise_for_status()
 
         if processor:
             return processor(result)
@@ -162,14 +196,41 @@
             sleep(sleep_seconds)
         return False
 
     def _get_scan(self, scan_id: int) -> List[dict]:
         url = f"{Urls.METADATA_GET}/{scan_id}"
         return self._get(url)[Keys.WORKSPACES]
 
+    def _activity_events(
+        self,
+        *,
+        day: Optional[date] = None,
+        continuation_uri: Optional[str] = None,
+    ) -> List[Dict]:
+        """
+        Returns a list of activity events for the organization.
+        https://learn.microsoft.com/en-us/power-bi/admin/service-admin-auditing#activityevents-rest-api
+        - when no day is specified, fallback is yesterday
+        - continuation_uri allows to fetch paginated data (internal usage)
+        """
+        url = _url(day, continuation_uri)
+        answer = self._get(url)
+        activity_events = answer[Keys.ACTIVITY_EVENT_ENTITIES]
+        is_last = answer[Keys.LAST_RESULT_SET]
+        assert isinstance(is_last, bool)
+        if is_last:
+            return activity_events
+
+        # there are more data to fetch
+        # https://learn.microsoft.com/en-us/rest/api/power-bi/admin/get-activity-events#get-the-next-set-of-audit-activity-events-by-sending-the-continuation-token-to-the-api-example
+        continuation_uri = answer[Keys.CONTINUATION_URI]
+        rest = self._activity_events(continuation_uri=continuation_uri)
+        activity_events.extend(rest)
+        return activity_events
+
     def _datasets(self) -> List[Dict]:
         """
         Returns a list of datasets for the organization.
         https://learn.microsoft.com/en-us/rest/api/power-bi/admin/datasets-get-datasets-as-admin
         """
         return self._get(Urls.DATASETS)[Keys.VALUE]
 
@@ -199,22 +260,30 @@
         for ix in range(0, len(ids), Batches.METADATA):
             batch_ids = [w_id for w_id in ids[ix : ix + Batches.METADATA]]
             scan_id = self._create_scan(batch_ids)
             self._wait_for_scan_result(scan_id)
             yield self._get_scan(scan_id)
 
     def fetch(
-        self, asset: PowerBiAsset, modified_since: Optional[datetime] = None
+        self,
+        asset: PowerBiAsset,
+        *,
+        modified_since: Optional[datetime] = None,
+        day: Optional[date] = None,
     ) -> List[Dict]:
         """
         Given a PowerBi asset, returns the corresponding data using the
         appropriate client.
         """
+        logger.info(f"Starting extraction of {asset}")
         asset = PowerBiAsset(asset)
 
+        if asset == PowerBiAsset.ACTIVITY_EVENTS:
+            return self._activity_events(day=day)
+
         if asset == PowerBiAsset.DATASETS:
             return self._datasets()
 
         if asset == PowerBiAsset.DASHBOARDS:
             return self._dashboards()
 
         if asset == PowerBiAsset.REPORTS:
```

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/rest_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/rest_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timedelta
-from unittest.mock import ANY, Mock, patch
+from unittest.mock import ANY, MagicMock, Mock, call, patch
 
 import pytest
 from requests import HTTPError
 
 from .constants import GET, POST, Assertions, Keys, QueryParams, Urls
 from .credentials import Credentials
 from .rest import Client, msal
@@ -188,7 +188,42 @@
     mocked_wait.return_value = True
     mocked_get_scan.return_value = [{"workspace_id": 1871}]
 
     client = _client()
     result = client._metadata()
 
     assert list(result) == [[{"workspace_id": 1871}], [{"workspace_id": 1871}]]
+
+
+_CALLS = [
+    {
+        Keys.ACTIVITY_EVENT_ENTITIES: ["foo", "bar"],
+        Keys.LAST_RESULT_SET: False,
+        Keys.CONTINUATION_URI: "https://next-call-1",
+    },
+    {
+        Keys.ACTIVITY_EVENT_ENTITIES: ["baz"],
+        Keys.LAST_RESULT_SET: False,
+        Keys.CONTINUATION_URI: "https://next-call-2",
+    },
+    {
+        Keys.ACTIVITY_EVENT_ENTITIES: ["biz"],
+        Keys.LAST_RESULT_SET: True,
+        Keys.CONTINUATION_URI: None,
+    },
+]
+
+
+@patch.object(Client, "_call")
+def test__activity_events(mocked):
+    client = _client()
+    mocked.side_effect = _CALLS
+
+    result = client._activity_events()
+    assert result == ["foo", "bar", "baz", "biz"]
+
+    expected_calls = [
+        call(ANY, GET, params=None, processor=None),
+        call("https://next-call-1", GET, params=None, processor=None),
+        call("https://next-call-2", GET, params=None, processor=None),
+    ]
+    mocked.assert_has_calls(expected_calls)
```

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/utils.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/client/utils_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/client/utils_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/powerbi/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/powerbi/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,32 @@
-import logging
 from typing import Iterable, List, Optional, Tuple, Union
 
 from ...utils import (
     OUTPUT_DIR,
     current_timestamp,
     deep_serialize,
     from_env,
     get_output_filename,
     write_json,
     write_summary,
 )
-from . import PowerBiAsset
-from .assets import MetadataAsset
+from .assets import METADATA_ASSETS, PowerBiAsset
 from .client import Client, Credentials
-from .client.constants import Urls
-
-logger = logging.getLogger(__name__)
-
-
-def _fetch(client: Client, asset: PowerBiAsset) -> Union[List, dict]:
-    logger.info(f"Extracting {asset}")
-    return client.fetch(asset)
 
 
 def iterate_all_data(
     client: Client,
 ) -> Iterable[Tuple[PowerBiAsset, Union[List, dict]]]:
 
-    metadata_assets = [enum.value for enum in MetadataAsset]
-
     for asset in PowerBiAsset:
 
-        if asset.value in metadata_assets:
+        if asset in METADATA_ASSETS:
             continue
 
-        data = _fetch(client, asset)
+        data = client.fetch(asset)
         yield asset, deep_serialize(data)
 
 
 def extract_all(
     tenant_id: str,
     client_id: str,
     secret: str,
```

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/assets.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/constants.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/constants.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/error.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/error.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/error_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/error_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/json_rpc.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/json_rpc.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/engine/websocket.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/engine/websocket.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/master.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/master.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/rest.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/client/rest_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/qlik/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/qlik/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/client_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/credentials.py` & `castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/endpoints.py` & `castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/sigma/client/pagination.py` & `castor_extractor-0.5.3/castor_extractor/visualization/sigma/client/pagination.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/sigma/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/sigma/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/assets.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/client.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/client_utils.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/credentials.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/project.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/project.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/client/safe_mode.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/client/safe_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/extract.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/gql_fields.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/gql_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/visualization/tableau/tsc_fields.py` & `castor_extractor-0.5.3/castor_extractor/visualization/tableau/tsc_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/abstract/asset.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/abstract/asset.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/abstract/client.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/abstract/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/abstract/extract.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/abstract/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/abstract/query.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/abstract/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/abstract/time_filter.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/abstract/time_filter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/client.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/client_test.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/extract.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/column.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/query.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/table.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/bigquery/query.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/bigquery/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/postgres/client.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/postgres/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/postgres/extract.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/postgres/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/column.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/schema.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/postgres/queries/table.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/postgres/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/postgres/query.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/postgres/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/client.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/client_test.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/extract.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/column.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/query.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/schema.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/table.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/table_freshness.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/table_freshness.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/queries/view_ddl.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/redshift/query.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/redshift/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/client.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/client_test.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/extract.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/column.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/column_lineage.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/column_lineage.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/query.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/schema.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/table.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/user.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/user.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/queries/view_ddl.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/snowflake/query.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/snowflake/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/synapse/extract.py` & `castor_extractor-0.5.3/castor_extractor/warehouse/synapse/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/column.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/query.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/castor_extractor/warehouse/synapse/queries/table.sql` & `castor_extractor-0.5.3/castor_extractor/warehouse/synapse/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.5.2/pyproject.toml` & `castor_extractor-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 
 [tool.poetry]
 name = "castor-extractor"
-version = "0.5.2"
+version = "0.5.3"
 description = "Extract your metadata assets."
 authors = ["Castor <support@castordoc.com>"]
 license = "EULA"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
```

### Comparing `castor_extractor-0.5.2/PKG-INFO` & `castor_extractor-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castor-extractor
-Version: 0.5.2
+Version: 0.5.3
 Summary: Extract your metadata assets.
 Home-page: https://www.castordoc.com/
 License: EULA
 Author: Castor
 Author-email: support@castordoc.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

