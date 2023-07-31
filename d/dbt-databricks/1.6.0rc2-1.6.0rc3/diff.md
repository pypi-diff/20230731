# Comparing `tmp/dbt-databricks-1.6.0rc2.tar.gz` & `tmp/dbt-databricks-1.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.6.0rc2.tar", last modified: Thu Jul 20 16:44:11 2023, max compression
+gzip compressed data, was "dbt-databricks-1.6.0rc3.tar", last modified: Thu Jul 27 19:21:05 2023, max compression
```

## Comparing `dbt-databricks-1.6.0rc2.tar` & `dbt-databricks-1.6.0rc3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.781909 dbt-databricks-1.6.0rc2/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       46 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/MANIFEST.in
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-20 16:44:11.781711 dbt-databricks-1.6.0rc2/PKG-INFO
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     4624 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/README.md
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.764076 dbt-databricks-1.6.0rc2/dbt/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.763801 dbt-databricks-1.6.0rc2/dbt/adapters/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.770055 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      626 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       26 2023-07-19 23:16:23.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2708 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/auth.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      586 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/column.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    35924 2023-07-19 22:57:01.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/connections.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    21146 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/impl.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    17743 2023-07-19 17:29:22.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     3564 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/relation.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2117 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.764236 dbt-databricks-1.6.0rc2/dbt/include/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.771047 dbt-databricks-1.6.0rc2/dbt/include/databricks/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       52 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/__init__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       77 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.772360 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    18808 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      592 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2409 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.773309 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.774470 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     4331 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     3910 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2066 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/validate.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.775701 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1682 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      279 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/refresh_materialized_view.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.776360 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2451 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2476 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/seeds.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5397 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/snapshot.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.777288 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      636 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1698 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1616 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1316 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      648 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.778720 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/utils/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      338 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      535 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.781374 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1959 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-06-15 16:25:03.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       91 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        4 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       38 2023-07-20 16:44:11.781963 dbt-databricks-1.6.0rc2/setup.cfg
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2502 2023-07-19 22:21:58.000000 dbt-databricks-1.6.0rc2/setup.py
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.368743 dbt-databricks-1.6.0rc3/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       46 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/MANIFEST.in
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-27 19:21:05.368539 dbt-databricks-1.6.0rc3/PKG-INFO
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     4624 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/README.md
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.352894 dbt-databricks-1.6.0rc3/dbt/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.352716 dbt-databricks-1.6.0rc3/dbt/adapters/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.359133 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      626 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       26 2023-07-27 19:20:54.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2708 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      586 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/column.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    35924 2023-07-19 22:57:01.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    21196 2023-07-27 19:15:21.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    17743 2023-07-19 17:29:22.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     3564 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2117 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.353007 dbt-databricks-1.6.0rc3/dbt/include/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.360233 dbt-databricks-1.6.0rc3/dbt/include/databricks/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       52 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/__init__.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       77 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.361666 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    18808 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      592 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2409 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.362839 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.363594 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     4331 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     3910 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2066 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/validate.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.364584 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1682 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      279 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/refresh_materialized_view.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.365110 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2451 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2476 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/seeds.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     5397 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/snapshot.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.365691 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      636 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1698 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1616 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1316 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      648 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.366401 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      338 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      535 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.368235 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1959 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-06-15 16:25:03.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       91 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)        4 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       38 2023-07-27 19:21:05.368800 dbt-databricks-1.6.0rc3/setup.cfg
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2502 2023-07-19 22:21:58.000000 dbt-databricks-1.6.0rc3/setup.py
```

### Comparing `dbt-databricks-1.6.0rc2/PKG-INFO` & `dbt-databricks-1.6.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.6.0rc2
+Version: 1.6.0rc3
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.6.0rc2/README.md` & `dbt-databricks-1.6.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/column.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,19 +120,20 @@
         return schema.lower() in set(s.lower() for s in self.list_schemas(database=database))
 
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
+        limit: Optional[int] = None,
         *,
         staging_table: Optional[BaseRelation] = None,
     ) -> Tuple[AdapterResponse, Table]:
         try:
-            return super().execute(sql=sql, auto_begin=auto_begin, fetch=fetch)
+            return super().execute(sql=sql, auto_begin=auto_begin, fetch=fetch, limit=limit)
         finally:
             if staging_table is not None:
                 self.drop_relation(staging_table)
 
     def list_relations_without_caching(  # type: ignore[override]
         self, schema_relation: DatabricksRelation
     ) -> List[DatabricksRelation]:
```

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/helpers.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/seeds.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/view.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.6.0rc3/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.6.0rc2
+Version: 1.6.0rc3
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc2/setup.py` & `dbt-databricks-1.6.0rc3/setup.py`

 * *Files identical despite different names*

