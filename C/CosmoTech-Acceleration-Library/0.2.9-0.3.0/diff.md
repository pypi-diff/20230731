# Comparing `tmp/CosmoTech_Acceleration_Library-0.2.9.tar.gz` & `tmp/CosmoTech_Acceleration_Library-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech_Acceleration_Library-0.2.9.tar", last modified: Mon Apr 24 08:45:06 2023, max compression
+gzip compressed data, was "CosmoTech_Acceleration_Library-0.3.0.tar", last modified: Mon Jul 31 06:56:56 2023, max compression
```

## Comparing `CosmoTech_Acceleration_Library-0.2.9.tar` & `CosmoTech_Acceleration_Library-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataInterface/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataStorage/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:45:06.175603 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 08:45:06.000000 CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:45:06.179604 CosmoTech_Acceleration_Library-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-24 08:44:53.000000 CosmoTech_Acceleration_Library-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.337069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/download_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Core/DataInterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Core/DataStorage/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-31 06:56:56.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-31 06:56:56.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:56:56.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 06:56:56.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-31 06:56:56.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 06:56:56.000000 CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:56:56.341069 CosmoTech_Acceleration_Library-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 06:56:47.000000 CosmoTech_Acceleration_Library-0.3.0/setup.py
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/csm_engine.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # Copyright (c) Cosmo Tech corporation.
 # Licensed under the MIT license.
 import csv
 import io
 import json
+import multiprocessing
 import os
 import tempfile
 from typing import Union
 
+import cosmotech_api
 from azure.digitaltwins.core import DigitalTwinsClient
 from azure.identity import DefaultAzureCredential
-
-import cosmotech_api
 from cosmotech_api.api.dataset_api import DatasetApi
 from cosmotech_api.api.scenario_api import ScenarioApi
-from cosmotech_api.api.workspace_api import WorkspaceApi
 from cosmotech_api.api.twingraph_api import TwingraphApi
-from cosmotech_api.api.twingraph_api import TwinGraphQuery
-
+from cosmotech_api.api.workspace_api import WorkspaceApi
+from cosmotech_api.model.twin_graph_query import TwinGraphQuery
 from openpyxl import load_workbook
 
 from CosmoTech_Acceleration_Library.Accelerators.utils.multi_environment import MultiEnvironment
 
 env = MultiEnvironment()
 
 
 class ScenarioDownloader:
 
-    def __init__(self, workspace_id: str, organization_id: str):
+    def __init__(self, workspace_id: str, organization_id: str, read_files=True):
         self.credentials = DefaultAzureCredential()
         scope = env.api_scope
         token = self.credentials.get_token(scope)
 
         self.configuration = cosmotech_api.Configuration(
             host=env.api_host,
             discard_unknown_keys=True,
             access_token=token.token
         )
 
         self.workspace_id = workspace_id
         self.organization_id = organization_id
+        self.dataset_file_temp_path = dict()
+        self.read_files = read_files
 
     def get_scenario_data(self, scenario_id: str):
         with cosmotech_api.ApiClient(self.configuration) as api_client:
             api_instance = ScenarioApi(api_client)
             scenario_data = api_instance.find_scenario_by_id(organization_id=self.organization_id,
                                                              workspace_id=self.workspace_id,
                                                              scenario_id=scenario_id)
@@ -72,17 +73,19 @@
                     "type": "adt",
                     "content": self._read_twingraph_content(twin_cache_name),
                     "name": dataset["name"]
                 }
             else:
                 _file_name = parameters['AZURE_STORAGE_CONTAINER_BLOB_PREFIX'].replace(
                     '%WORKSPACE_FILE%/', '')
+                _content = self._download_file(_file_name)
+                self.dataset_file_temp_path[dataset_id] = self.dataset_file_temp_path[_file_name]
                 return {
                     "type": _file_name.split('.')[-1],
-                    "content": self._download_file(_file_name),
+                    "content": _content,
                     "name": dataset['name']
                 }
 
     def _read_twingraph_content(self, cache_name: str) -> dict:
         with cosmotech_api.ApiClient(self.configuration) as api_client:
             api_instance = TwingraphApi(api_client)
             _query_nodes = TwinGraphQuery(
@@ -127,14 +130,15 @@
                     **props
                 })
 
             return content
 
     def _download_file(self, file_name: str):
         tmp_dataset_dir = tempfile.mkdtemp()
+        self.dataset_file_temp_path[file_name] = tmp_dataset_dir
         with cosmotech_api.ApiClient(self.configuration) as api_client:
             api_ws = WorkspaceApi(api_client)
 
             all_api_files = api_ws.find_all_workspace_files(
                 self.organization_id, self.workspace_id)
 
             existing_files = list(
@@ -148,14 +152,16 @@
                                                          workspace_id=self.workspace_id,
                                                          file_name=_file_name)
 
                 target_file = os.path.join(
                     tmp_dataset_dir, _file_name.split('/')[-1])
                 with open(target_file, "wb") as tmp_file:
                     tmp_file.write(dl_file.read())
+                if not self.read_files:
+                    return {}
                 if ".xls" in _file_name:
                     wb = load_workbook(target_file, data_only=True)
                     for sheet_name in wb.sheetnames:
                         sheet = wb[sheet_name]
                         content[sheet_name] = list()
                         headers = next(sheet.iter_rows(
                             max_row=1, values_only=True))
@@ -175,16 +181,15 @@
                                 if converted_value is not None:
                                     new_row[key] = converted_value
                             if new_row:
                                 content[sheet_name].append(new_row)
                 elif ".csv" in _file_name:
                     with open(target_file, "r") as file:
                         # Read every file in the input folder
-                        current_filename = os.path.basename(target_file)[
-                            :-len(".csv")]
+                        current_filename = os.path.basename(target_file)[:-len(".csv")]
                         content[current_filename] = list()
                         for row in csv.DictReader(file):
                             new_row = dict()
                             for key, value in row.items():
                                 try:
                                     # Try to convert any json row to dict object
                                     converted_value = json.load(
@@ -250,17 +255,77 @@
         return content
 
     def get_all_datasets(self, scenario_id: str) -> dict:
         scenario_data = self.get_scenario_data(scenario_id=scenario_id)
 
         datasets = scenario_data['dataset_list']
 
-        content = dict()
-        for dataset_id in datasets:
-            content[dataset_id] = self.download_dataset(dataset_id)
+        dataset_ids = datasets[:]
 
         for parameter in scenario_data['parameters_values']:
             if parameter['var_type'] == '%DATASETID%':
                 dataset_id = parameter['value']
-                content[dataset_id] = self.download_dataset(dataset_id)
+                dataset_ids.append(dataset_id)
+
+        def process(_dataset_id, _return_dict):
+            _c = self.download_dataset(_dataset_id)
+            if _dataset_id in self.dataset_file_temp_path:
+                _return_dict[_dataset_id] = (_c, self.dataset_file_temp_path[_dataset_id], dataset_id)
+            else:
+                _return_dict[_dataset_id] = _c
+
+        manager = multiprocessing.Manager()
+        return_dict = manager.dict()
+        processes = [multiprocessing.Process(target=process, args=(dataset_id, return_dict)) for dataset_id in
+                     dataset_ids]
+        [p.start() for p in processes]
+        [p.join() for p in processes]
+        content = dict()
+        for k, v in return_dict.items():
+            if isinstance(v, tuple):
+                content[k] = v[0]
+                self.dataset_file_temp_path[v[2]] = v[1]
+            else:
+                content[k] = v
 
         return content
+
+    def dataset_to_file(self, dataset_id, dataset_info):
+        type = dataset_info['type']
+        content = dataset_info['content']
+        name = dataset_info['name']
+        if type == "adt":
+            return self.adt_dataset(content, name, type)
+        return self.dataset_file_temp_path[dataset_id]
+
+    @staticmethod
+    def sheet_to_header(sheet_content):
+        fieldnames = []
+        has_src = False
+        has_id = False
+        for r in sheet_content:
+            for k in r.keys():
+                if k not in fieldnames:
+                    if k in ['source', 'target']:
+                        has_src = True
+                    elif k == "id":
+                        has_id = True
+                    else:
+                        fieldnames.append(k)
+        if has_src:
+            fieldnames = ['source', 'target'] + fieldnames
+        if has_id:
+            fieldnames = ['id', ] + fieldnames
+        return fieldnames
+
+    def adt_dataset(self, content, _name, _type):
+        tmp_dataset_dir = tempfile.mkdtemp()
+        for _filename, _filecontent in content.items():
+            with open(tmp_dataset_dir + "/" + _filename + ".csv", "w") as _file:
+                fieldnames = self.sheet_to_header(_filecontent)
+
+                _w = csv.DictWriter(_file, fieldnames=fieldnames, dialect="unix", quoting=csv.QUOTE_MINIMAL)
+                _w.writeheader()
+                # _w.writerows(_filecontent)
+                for r in _filecontent:
+                    _w.writerow({k: str(v).replace("'", "\"") for k, v in r.items()})
+        return tmp_dataset_dir
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/graph_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) Cosmo Tech corporation.
 # Licensed under the MIT license.
 import logging
-from pathlib import Path
 
 from CosmoTech_Acceleration_Library.Modelops.core.common.redis_handler import RedisHandler
 from CosmoTech_Acceleration_Library.Modelops.core.io.model_metadata import ModelMetadata
 from CosmoTech_Acceleration_Library.Modelops.core.utils.model_util import ModelUtil
 
 logger = logging.getLogger(__name__)
 
@@ -15,99 +14,91 @@
     Class that handle Graph Redis information
     """
 
     def __init__(self, host: str, port: int, name: str, password: str = None, source_url: str = "", graph_rotation: int = 3):
         super().__init__(host=host, port=port, name=name, password=password)
         logger.debug("GraphHandler init")
         self.graph = self.r.graph(name)
+        self.name = name
         self.m_metadata = ModelMetadata(host=host, port=port, name=name, password=password)
         current_metadata = self.m_metadata.get_metadata()
         if not current_metadata:
+            if graph_rotation is None:
+                graph_rotation = 3
             logger.debug("Create metadata key")
             self.m_metadata.set_metadata(last_graph_version=0, graph_source_url=source_url,
                                          graph_rotation=graph_rotation)
 
 
 class VersionedGraphHandler(GraphHandler):
     """
     Class that handle Versioned Graph Redis information
     """
 
-    def __init__(self, host: str, port: int, name: str, version: int, password: str = None, source_url: str = "",
-                 graph_rotation: int = 3):
+    def __init__(self, host: str, port: int, name: str, version: int = None, password: str = None, source_url: str = "",
+                 graph_rotation: int = None):
         super().__init__(host=host, port=port, name=name, password=password, source_url=source_url,
                          graph_rotation=graph_rotation)
         logger.debug("VersionedGraphHandler init")
-        self.version = None
-        self.versioned_name = None
-        self.fill_versioned_graph_data(name, version)
-
-    def fill_versioned_graph_data(self, graph_name: str, version: int):
-        """
-        Fill data about version and create new graph
-        :param graph_name: the graph name
-        :param version: the version
-        """
-        versioned_name = ModelUtil.build_graph_version_name(graph_name, version)
-        self.versioned_name = versioned_name
         self.version = version
-        self.graph = self.r.graph(versioned_name)
-        self.m_metadata.set_last_graph_version(version)
+        if version is None:
+            self.version = self.m_metadata.get_last_graph_version()
+        self.versioned_name = ModelUtil.build_graph_version_name(self.name, self.version)
+        self.graph = self.r.graph(self.versioned_name)
 
 
 class RotatedGraphHandler(VersionedGraphHandler):
     """
     Class that handle Rotated Graph Redis information
     """
 
-    def __init__(self, host: str, port: int, name: str, password: str = None, version: int = -1, source_url: str = "",
-                 graph_rotation: int = 3):
+    def __init__(self, host: str, port: int, name: str, password: str = None, version: int = None, source_url: str = "",
+                 graph_rotation: int = None):
         super().__init__(host=host, port=port, name=name, password=password, source_url=source_url, version=version,
                          graph_rotation=graph_rotation)
         logger.debug("RotatedGraphHandler init")
-        self.graph_rotation = graph_rotation
-        new_version = version
-        if version == -1:
-            logger.debug("Handle Rotation Graph")
-            new_version = self.handle_graph_rotation(name, graph_rotation)
-        self.fill_versioned_graph_data(name, new_version)
+        self.graph_rotation = self.m_metadata.get_graph_rotation()
+
+    def get_all_versions(self):
+        matching_graph_keys = self.r.keys(ModelUtil.build_graph_key_pattern(self.name))
+        versions = []
+        for graph_key in matching_graph_keys:
+            versions.append(graph_key.split(":")[-1])
+        return versions
 
-    def handle_graph_rotation(self, graph_name: str, graph_rotation: int) -> int:
+    def handle_graph_rotation(func):
         """
-        Handle graph rotation (delete the oldest graph if the amount of graph is greater than graph rotation)
-        :param graph_name: the graph name
-        :param graph_rotation: the amount of graph to keep
-        :return: the graph version to create
+        Decorator to do stuff then handle graph rotation (delete the oldest graph if the amount of graph is greater than graph rotation)
         """
-        matching_graph_keys = self.r.keys(ModelUtil.build_graph_key_pattern(graph_name))
-        graph_versions = []
-        for graph_key in matching_graph_keys:
-            graph_versions.append(graph_key.split(":")[-1])
 
-        min_version = 0
-        max_version = 0
-        if len(graph_versions) > 0:
-            min_version = min([int(x) for x in graph_versions if x.isnumeric()])
-            max_version = max([int(x) for x in graph_versions if x.isnumeric()])
-        logger.debug(f"{graph_name} minimal version is: {min_version}")
-        logger.debug(f"{graph_name} maximal version is: {max_version}")
-
-        if len(matching_graph_keys) >= graph_rotation:
-            oldest_graph_version_to_delete = ModelUtil.build_graph_version_name(graph_name, min_version)
-            self.r.delete(oldest_graph_version_to_delete)
-            logger.debug(f"Graph {oldest_graph_version_to_delete} deleted")
-        return max_version + 1
-
-
-class ExportableGraphHandler(VersionedGraphHandler):
-    """
-    Class that handle Exportable Versioned Graph Redis information
-    """
-
-    def __init__(self, host: str, port: int, name: str, version: int, password: str = None, source_url: str = "", export_dir: str = "/"):
-        super().__init__(host=host, port=port, name=name, version=version, password=password, source_url=source_url)
-        logger.debug("ExportableGraphHandler init")
-        if export_dir != "":
-            Path(export_dir).mkdir(parents=True, exist_ok=True)
-            self.export_dir = export_dir
-        else:
-            self.export_dir = self.default_export_dir
+        def handle(self, *args, **kwargs):
+            graph_versions = self.get_all_versions()
+
+            if len(graph_versions) > 0:
+                max_version = max([int(x) for x in graph_versions if x.isnumeric()])
+            else:
+                max_version = 0
+            # upgrade current graph to max_version+1
+            self.version = max_version + 1
+            self.version_name = ModelUtil.build_graph_version_name(self.name, self.version)
+            self.graph = self.r.graph(self.version_name)
+            logger.debug(f'Using graph updated version {self.version_name}')
+
+            # do function on new graph
+            func(self, *args, **kwargs)
+
+            # get max version to manage case func not using (hence creating) graph
+            graph_versions = [int(v) for v in self.get_all_versions()]
+            graph_versions.sort()
+            graph_versions.reverse()
+            to_remove = graph_versions[int(self.graph_rotation):]
+
+            # remove all older versions
+            for v in to_remove:
+                oldest_graph_version_to_delete = ModelUtil.build_graph_version_name(self.name, v)
+                self.r.delete(oldest_graph_version_to_delete)
+                logger.debug(f"Graph {oldest_graph_version_to_delete} deleted")
+
+            # upgrade metadata last version to +1 after function execution
+            self.m_metadata.set_last_graph_version(self.version)
+
+        return handle
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/redis_handler.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/common/writer/CsvWriter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Copyright (c) Cosmo Tech corporation.
 # Licensed under the MIT license.
 import csv
 import logging
+import json
+import ast
+import os
 
 from redis.commands.graph.query_result import QueryResult
 
 from CosmoTech_Acceleration_Library.Modelops.core.utils.model_util import ModelUtil
 
 logger = logging.getLogger(__name__)
 
@@ -15,16 +18,23 @@
     Csv Writer class
     """
 
     @staticmethod
     def _to_csv_format(val: any) -> str:
         if isinstance(val, bool):
             return str(val).lower()
+        if isinstance(val, dict):
+            return json.dumps(val)
         if str(val) == 'True' or str(val) == 'False':
             return str(val).lower()
+        if str(val).startswith('{') and str(val).endswith('}'):
+            try:
+                return json.dumps(json.loads(val))
+            except json.decoder.JSONDecodeError:
+                return json.dumps(ast.literal_eval(str(val)))
         return str(val)
 
     @staticmethod
     def _to_cosmo_key(val: any) -> str:
         if str(val) == ModelUtil.dt_id_key:
             return ModelUtil.id_key
         return val
@@ -41,15 +51,15 @@
                 row.update({CsvWriter._to_cosmo_key(k): CsvWriter._to_csv_format(v) for k, v in raw_data[i].properties.items()})
             headers.update(row.keys())
             rows.append(row)
 
         output_file_name = f'{export_dir}/{file_name}.csv'
         logger.debug(f"Writing CSV file {output_file_name}")
         with open(output_file_name, 'w') as csvfile:
-            csv_writer = csv.DictWriter(csvfile, fieldnames=headers, delimiter=delimiter, quotechar=quote_char, quoting=csv.QUOTE_ALL)
+            csv_writer = csv.DictWriter(csvfile, fieldnames=headers, delimiter=delimiter, quotechar=quote_char, quoting=csv.QUOTE_MINIMAL)
             csv_writer.writeheader()
             csv_writer.writerows(rows)
         logger.debug(f"... CSV file {output_file_name} has been written")
 
     @staticmethod
     def write_relationship_data(export_dir: str, file_name: str, query_result: QueryResult, headers: list = [],
                                 delimiter: str = ',', quote_char: str = '\"') -> None:
@@ -60,11 +70,32 @@
             row.update({k: CsvWriter._to_csv_format(v) for k, v in raw_data[2].properties.items()})
             headers.update(row.keys())
             rows.append(row)
 
         output_file_name = export_dir + file_name + '.csv'
         logger.debug(f"Writing CSV file {output_file_name}")
         with open(output_file_name, 'w') as csvfile:
-            csv_writer = csv.DictWriter(csvfile, fieldnames=headers, delimiter=delimiter, quotechar=quote_char, quoting=csv.QUOTE_ALL)
+            csv_writer = csv.DictWriter(csvfile, fieldnames=headers, delimiter=delimiter, quotechar=quote_char, quoting=csv.QUOTE_MINIMAL)
             csv_writer.writeheader()
             csv_writer.writerows(rows)
         logger.debug(f"... CSV file {output_file_name} has been written")
+
+    @staticmethod
+    def write_data(export_dir: str, file_name: str, input_rows: dict, delimiter: str = ',', quote_char: str = '\"') -> None:
+        output_file_name = export_dir + file_name + '.csv'
+        write_header = False
+        if not os.path.exists(output_file_name):
+            write_header = True
+
+        headers = set()
+        output_rows = []
+        for row in input_rows:
+            output_rows.append({CsvWriter._to_cosmo_key(k): CsvWriter._to_csv_format(v) for k, v in row.items()})
+            headers.update(row.keys())
+
+        logger.info(f"Writing file {output_file_name} ...")
+        with open(output_file_name, 'a') as csvfile:
+            csv_writer = csv.DictWriter(csvfile, fieldnames=headers, delimiter=delimiter, quotechar=quote_char, quoting=csv.QUOTE_MINIMAL)
+            if write_header:
+                csv_writer.writeheader()
+            csv_writer.writerows(output_rows)
+        logger.debug(f"... file {output_file_name} has been written")
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/decorators/model_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Cosmo Tech corporation.
 # Licensed under the MIT license.
 import functools
 
-from CosmoTech_Acceleration_Library.Modelops.core.common.graph_handler import GraphHandler, ExportableGraphHandler
+from CosmoTech_Acceleration_Library.Modelops.core.common.graph_handler import GraphHandler, VersionedGraphHandler
 
 
 def update_last_version(function):
     """
     Function decorator that update metadata last version after calling the function annotated
     :param function: the function annotated
     """
@@ -46,15 +46,15 @@
     :param function: the function annotated
     """
 
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
         self = args[0]
         version_graph_name = self.versioned_name
-        if isinstance(self, ExportableGraphHandler):
+        if isinstance(self, VersionedGraphHandler):
             key_count = self.r.exists(version_graph_name)
             if key_count != 0:
                 function(*args, **kwargs)
             else:
                 raise Exception(f"{version_graph_name} does not exist!")
         else:
             function(*args, **kwargs)
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 class ModelImporter(RotatedGraphHandler):
     """
     Model Exporter for cached data
     """
 
+    @RotatedGraphHandler.handle_graph_rotation
     def bulk_import(self, twin_file_paths: list = [], relationship_file_paths: list = [], enforce_schema: bool = False):
         """
         Import all csv data
         :param twin_file_paths: the file paths of all twin csv files
         :param relationship_file_paths: the file paths of all relationship csv files
         :param enforce_schema: True if the schema is defined within headers (default False)
         `Enforce_schema documentation <https://github.com/RedisGraph/redisgraph-bulk-loader#input-schemas>`_
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 
 from CosmoTech_Acceleration_Library.Modelops.core.common.redis_handler import RedisHandler
 from CosmoTech_Acceleration_Library.Modelops.core.utils.model_util import ModelUtil
 
 logger = logging.getLogger(__name__)
 
+
 class ModelMetadata(RedisHandler):
     """
     Model Metadata management class for cached data
     """
 
     last_modified_date_key = "lastModifiedDate"
     last_version_key = "lastVersion"
@@ -139,13 +140,13 @@
     def update_last_version(self):
         """
         Update the last version of the graph
         """
         current_metadata = self.get_metadata()
         if self.last_version_key in current_metadata:
             current_version = int(self.get_last_graph_version())
-            current_version += 1
-            self.set_last_graph_version(str(current_version))
+            new_version = current_version + 1
+            self.set_last_graph_version(str(new_version))
             self.update_last_modified_date()
         else:
             self.set_last_graph_version("0")
             self.update_last_modified_date()
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         Run specified query
         :param query: the query to run
         :param params: the parameters for the query if any
         :param timeout: a specific timeout
         :param read_only: executes a readonly query if set to True
         :return: the QueryResult corresponding to specified query
         """
-        logger.debug(f"Query : {query}")
+        logger.debug(f"Query : {query} with params : {params}")
         return self.graph.query(q=query, params=params, timeout=timeout, read_only=read_only)
 
     def exists(self, key) -> bool:
         """
         Check if a key exists in Redis
         :param key: the key
         :return: True if exists else False
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/io/model_writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Cosmo Tech corporation.
 # Licensed under the MIT license.
 import logging
 
-from CosmoTech_Acceleration_Library.Modelops.core.common.graph_handler import RotatedGraphHandler
+from CosmoTech_Acceleration_Library.Modelops.core.common.graph_handler import VersionedGraphHandler
 from CosmoTech_Acceleration_Library.Modelops.core.decorators.model_decorators import update_last_modified_date
 from CosmoTech_Acceleration_Library.Modelops.core.utils.model_util import ModelUtil
 
 logger = logging.getLogger(__name__)
 
-class ModelWriter(RotatedGraphHandler):
+
+class ModelWriter(VersionedGraphHandler):
     """
     Model Writer for cached data
     """
 
     @update_last_modified_date
     def create_twin(self, twin_type: str, properties: dict):
         """
@@ -30,9 +31,7 @@
         Create a relationship
         :param relationship_type: the relationship type
         :param properties: the relationship properties
         """
         create_rel = ModelUtil.create_relationship_query(relationship_type, properties)
         logger.debug(f"Query: {create_rel}")
         self.graph.query(create_rel)
-
-
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/model_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         cypher_list = []
         for key, value in parameters.items():
             formatted_value = stringify_param_value(value)
             if isinstance(value, str):
                 try:
                     json.loads(value)
                     formatted_value = json.dumps(value)
-                except ValueError as e:
+                except ValueError:
                     logger.debug(f"{value} is not a jsonString, use the raw value")
             cypher_list.append(f"{key} : {formatted_value}")
         joined_list = ', '.join(cypher_list)
         return '{' + joined_list + '}'
 
     @staticmethod
     def create_index_query(entity_name: str, entity_property_name: str) -> str:
@@ -157,23 +157,7 @@
         :return: the versioned graph name
         """
         return graph_name + ":" + str(version)
 
     @staticmethod
     def build_graph_key_pattern(graph_name: str) -> str:
         return graph_name + ":*"
-
-    @staticmethod
-    def unjsonify(value: dict) -> dict:
-        """
-        Unjsonify transform json strings to python objects
-        :param value a dict
-        :return: a dict with unjsonify values
-        """
-        for k, v in value.items():
-            if isinstance(v, str):
-                try:
-                    value[k] = json.loads(v)
-                    logger.debug(f" new value => {value[k]}")
-                except ValueError as e:
-                    logger.debug(f"{v} is not a jsonString, use the raw value")
-        return value
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library/Modelops/core/utils/tests/model_util_test.py`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/PKG-INFO` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech-Acceleration-Library
-Version: 0.2.9
+Version: 0.3.0
 Summary: Acceleration libraries for CosmoTech cloud based solution development
 Home-page: https://github.com/Cosmo-Tech/CosmoTech-Acceleration-Library
 Author: afossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt` & `CosmoTech_Acceleration_Library-0.3.0/CosmoTech_Acceleration_Library.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 setup.py
 CosmoTech_Acceleration_Library/__init__.py
 CosmoTech_Acceleration_Library.egg-info/PKG-INFO
 CosmoTech_Acceleration_Library.egg-info/SOURCES.txt
 CosmoTech_Acceleration_Library.egg-info/dependency_links.txt
+CosmoTech_Acceleration_Library.egg-info/entry_points.txt
 CosmoTech_Acceleration_Library.egg-info/requires.txt
 CosmoTech_Acceleration_Library.egg-info/top_level.txt
 CosmoTech_Acceleration_Library/Accelerators/__init__.py
 CosmoTech_Acceleration_Library/Accelerators/adx_wrapper.py
 CosmoTech_Acceleration_Library/Accelerators/cosmo_api.py
 CosmoTech_Acceleration_Library/Accelerators/csm_engine.py
 CosmoTech_Acceleration_Library/Accelerators/scenario_download/__init__.py
 CosmoTech_Acceleration_Library/Accelerators/scenario_download/azure_function_main.py
+CosmoTech_Acceleration_Library/Accelerators/scenario_download/download_command.py
 CosmoTech_Acceleration_Library/Accelerators/scenario_download/scenario_downloader.py
 CosmoTech_Acceleration_Library/Accelerators/utils/__init__.py
 CosmoTech_Acceleration_Library/Accelerators/utils/multi_environment.py
 CosmoTech_Acceleration_Library/Core/__init__.py
 CosmoTech_Acceleration_Library/Core/DataInterface/__init__.py
 CosmoTech_Acceleration_Library/Core/DataStorage/__init__.py
 CosmoTech_Acceleration_Library/Modelops/__init__.py
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/LICENSE` & `CosmoTech_Acceleration_Library-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/PKG-INFO` & `CosmoTech_Acceleration_Library-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech_Acceleration_Library
-Version: 0.2.9
+Version: 0.3.0
 Summary: Acceleration libraries for CosmoTech cloud based solution development
 Home-page: https://github.com/Cosmo-Tech/CosmoTech-Acceleration-Library
 Author: afossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CosmoTech_Acceleration_Library-0.2.9/README.md` & `CosmoTech_Acceleration_Library-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech_Acceleration_Library-0.2.9/setup.py` & `CosmoTech_Acceleration_Library-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,13 @@
     license='MIT',
     author='afossart',
     author_email='alexis.fossart@cosmotech.com',
     description='Acceleration libraries for CosmoTech cloud based solution development',
     long_description=readme_text,
     long_description_content_type='text/markdown',
     install_requires=required,
+    entry_points={
+        'console_scripts': [
+            'cosmotech_scenario_downloader=CosmoTech_Acceleration_Library.Accelerators.scenario_download.download_command:main'
+        ]
+    },
 )
```

