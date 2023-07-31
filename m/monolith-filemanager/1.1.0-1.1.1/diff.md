# Comparing `tmp/monolith_filemanager-1.1.0.tar.gz` & `tmp/monolith_filemanager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monolith_filemanager-1.1.0.tar", last modified: Fri Dec 10 15:14:45 2021, max compression
+gzip compressed data, was "dist/monolith_filemanager-1.1.1.tar", last modified: Mon Jul 31 10:13:55 2023, max compression
```

## Comparing `monolith_filemanager-1.1.0.tar` & `monolith_filemanager-1.1.1.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      651 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)     8606 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    13756 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/local_file_processes.py
--rw-r--r--   0 runner    (1001) docker     (121)    18004 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/s3_processes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/adapters/version_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager/components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/components/path_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager/console_commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/console_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/console_commands/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/console_commands/install_boto.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/console_commands/install_flask.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/console_commands/install_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/gmsh_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/hdf5_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/joblib_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/json_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/keras_model_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/matlab.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/numpy_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     6548 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/pandas_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/protobuf_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/standard_pickle_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/vtk_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/file/yml_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager/s3storage/
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/s3storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/s3storage/bucket_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/s3storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6532 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/s3storage/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/monolith_filemanager/singleton.py
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-10 15:14:33.000000 monolith_filemanager-1.1.0/monolith_filemanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/monolith_filemanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/requirements_manager/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/requirements_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/requirements_manager/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/requirements_manager/operator_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/requirements_manager/requirements_manager_class.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2878 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22915 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/adapters/test_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    19428 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/adapters/test_s3_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/adapters/test_version_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/tests/components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/components/test_path_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/tests/file/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_joblib_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_json_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_keras_model_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_numpyfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_protobuf_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_standard_pickle_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/file/test_yml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/tests/requirements_manager/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/requirements_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/requirements_manager/test_requirements_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 15:14:45.000000 monolith_filemanager-1.1.0/tests/s3storage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/s3storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4262 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/s3storage/test_bucket_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/s3storage/test_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7634 2021-12-10 15:10:59.000000 monolith_filemanager-1.1.0/tests/s3storage/test_v1engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/local_file_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18004 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/s3_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/version_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/components/path_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/install_boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/install_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/install_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/gmsh_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/hdf5_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/joblib_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/json_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/keras_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/numpy_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/pandas_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/protobuf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/standard_pickle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/vtk_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/yml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/bucket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 10:13:45.000000 monolith_filemanager-1.1.1/monolith_filemanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/requirements_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/operator_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/requirements_manager_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22915 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/test_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/test_s3_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/test_version_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/components/test_path_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_joblib_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_json_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_keras_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_numpyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_protobuf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_standard_pickle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_yml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/requirements_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/requirements_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/requirements_manager/test_requirements_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/s3storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/test_bucket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/test_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/test_v1engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/test_path.py
```

### Comparing `monolith_filemanager-1.1.0/LICENSE` & `monolith_filemanager-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/PKG-INFO` & `monolith_filemanager-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: monolith_filemanager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package for reading and writing files
 Home-page: https://github.com/MonolithAILtd/monolith-filemanager
 Author: Maxwell Flitton
 Author-email: maxwell@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: flask
 Provides-Extra: 3d
@@ -240,9 +238,7 @@
 This repo is still fairly new so contributing will require some communication. 
 You can contact with ideas and outline for a feature at ```maxwell@monolithai.com```.
 
 Writing code is not the only way you can contribute. Merely using the module is a help, if you come across any issues 
 feel free to raise them in the issues section of the Github page as this enables us to make the module more stable.
 If there are any issues that you want to solve, your pull request has to have documentation, 100% unit test coverage 
 and functional testing. 
-
-
```

### Comparing `monolith_filemanager-1.1.0/README.md` & `monolith_filemanager-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/__init__.py` & `monolith_filemanager-1.1.1/monolith_filemanager/__init__.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/adapters/base.py` & `monolith_filemanager-1.1.1/monolith_filemanager/adapters/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from abc import ABC, abstractmethod
 from typing import Any, Tuple, List, Union, Optional
 
 from monolith_filemanager.file import FileMap
 from monolith_filemanager.path import FilePath
 
 
@@ -114,15 +115,24 @@
         Batch delete files or folders within the parent directory of self.path.
 
         :param paths: (List[str]) file/folder paths within self.path to be deleted
         :return: None
         """
         for path in paths:
             del_path = FilePath(f"{self.path}/{path}")
-            self.delete_file(path=del_path)
+            # Assume that any path with no extension represents a folder. We must do this in order
+            # to append a trailing slash to the path later to prevent spurious folder deletion as
+            # a result of the use of the Prefix filter in boto3. Without this logic, deleting folder
+            # DirA would also delete DirA* (DirAB, DirABC etc.).
+            _, ext = os.path.splitext(del_path)
+
+            if ext:
+                self.delete_file(path=del_path)
+
+            self.delete_folder(path=del_path)
 
     @abstractmethod
     def rename_file(self, new_name: str) -> None:
         pass
 
     @abstractmethod
     def rename_folder(self, new_name: str) -> None:
```

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/adapters/errors.py` & `monolith_filemanager-1.1.1/monolith_filemanager/adapters/errors.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/adapters/local_file_processes.py` & `monolith_filemanager-1.1.1/monolith_filemanager/adapters/local_file_processes.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/adapters/s3_processes.py` & `monolith_filemanager-1.1.1/monolith_filemanager/adapters/s3_processes.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/adapters/version_identifier.py` & `monolith_filemanager-1.1.1/monolith_filemanager/adapters/version_identifier.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/components/path_map.py` & `monolith_filemanager-1.1.1/monolith_filemanager/components/path_map.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/console_commands/hello.py` & `monolith_filemanager-1.1.1/monolith_filemanager/console_commands/hello.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/errors.py` & `monolith_filemanager-1.1.1/monolith_filemanager/errors.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/__init__.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/__init__.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/base.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/base.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/errors.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/errors.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/gmsh_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/gmsh_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/hdf5_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/hdf5_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/joblib_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/joblib_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/json_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/json_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/keras_model_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/keras_model_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/matlab.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/matlab.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/numpy_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/numpy_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/pandas_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/pandas_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/protobuf_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/protobuf_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/standard_pickle_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/standard_pickle_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/vtk_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/vtk_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/file/yml_file.py` & `monolith_filemanager-1.1.1/monolith_filemanager/file/yml_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/path.py` & `monolith_filemanager-1.1.1/monolith_filemanager/path.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/s3storage/__init__.py` & `monolith_filemanager-1.1.1/monolith_filemanager/s3storage/__init__.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/s3storage/bucket_manager.py` & `monolith_filemanager-1.1.1/monolith_filemanager/s3storage/bucket_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager/s3storage/file_manager.py` & `monolith_filemanager-1.1.1/monolith_filemanager/s3storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager.egg-info/PKG-INFO` & `monolith_filemanager-1.1.1/monolith_filemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: monolith-filemanager
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package for reading and writing files
 Home-page: https://github.com/MonolithAILtd/monolith-filemanager
 Author: Maxwell Flitton
 Author-email: maxwell@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: flask
 Provides-Extra: 3d
@@ -240,9 +238,7 @@
 This repo is still fairly new so contributing will require some communication. 
 You can contact with ideas and outline for a feature at ```maxwell@monolithai.com```.
 
 Writing code is not the only way you can contribute. Merely using the module is a help, if you come across any issues 
 feel free to raise them in the issues section of the Github page as this enables us to make the module more stable.
 If there are any issues that you want to solve, your pull request has to have documentation, 100% unit test coverage 
 and functional testing. 
-
-
```

### Comparing `monolith_filemanager-1.1.0/monolith_filemanager.egg-info/SOURCES.txt` & `monolith_filemanager-1.1.1/monolith_filemanager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 monolith_filemanager/s3storage/bucket_manager.py
 monolith_filemanager/s3storage/errors.py
 monolith_filemanager/s3storage/file_manager.py
 requirements_manager/__init__.py
 requirements_manager/errors.py
 requirements_manager/operator_enums.py
 requirements_manager/requirements_manager_class.py
+tests/test_path.py
 tests/adapters/__init__.py
 tests/adapters/test_local_adapter.py
 tests/adapters/test_s3_adapter.py
 tests/adapters/test_version_identifier.py
 tests/components/__init__.py
 tests/components/test_path_map.py
 tests/file/__init__.py
```

### Comparing `monolith_filemanager-1.1.0/requirements_manager/requirements_manager_class.py` & `monolith_filemanager-1.1.1/requirements_manager/requirements_manager_class.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/setup.py` & `monolith_filemanager-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/adapters/test_local_adapter.py` & `monolith_filemanager-1.1.1/tests/adapters/test_local_adapter.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/adapters/test_s3_adapter.py` & `monolith_filemanager-1.1.1/tests/adapters/test_s3_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,26 +243,28 @@
         test = S3ProcessesAdapter(file_path="test path")
         test._engine = MagicMock()
         test.path = MagicMock()
 
         test.ls()
         test._engine.ls.assert_called_once_with(storage_path=test.path.to_string.return_value)
 
+    @patch("monolith_filemanager.adapters.s3_processes.S3ProcessesAdapter.delete_folder")
     @patch("monolith_filemanager.adapters.s3_processes.S3ProcessesAdapter.delete_file")
     @patch("monolith_filemanager.adapters.s3_processes.S3ProcessesAdapter.__init__")
-    def test_batch_delete(self, mock_init, mock_delete_file):
+    def test_batch_delete(self, mock_init, mock_delete_file, mock_delete_folder):
         mock_init.return_value = None
         test = S3ProcessesAdapter(file_path="test/path")
         test.path = "test/path"
         test.path = "mock/folder/path"
-        mock_paths = ["mock_folder", "mock_file"]
+        mock_paths = ["mock_folder", "mock_file.file"]
         mock_delete_file.side_effect = [None, None]
+        mock_delete_folder.side_effect = [None, None]
         test.batch_delete(paths=mock_paths)
-        mock_delete_file.assert_has_calls = [call(path=test.path + mock_paths[0]),
-                                             call(path=test.path + mock_paths[1])]
+        mock_delete_folder.assert_has_calls = [call(path=test.path + mock_paths[0])]
+        mock_delete_file.assert_has_calls = [call(path=test.path + mock_paths[1])]
 
     def test_copy_file(self):
         mock_new_path = "mock/new/path"
         mock_engine = MagicMock()
         mock_engine._split_s3_path.side_effect = [("mock-bucket", "old/file.txt", None),
                                                   ("mock-bucket", "new/file.txt", None)]
         mockObject = MagicMock()
```

### Comparing `monolith_filemanager-1.1.0/tests/adapters/test_version_identifier.py` & `monolith_filemanager-1.1.1/tests/adapters/test_version_identifier.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/components/test_path_map.py` & `monolith_filemanager-1.1.1/tests/components/test_path_map.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_base.py` & `monolith_filemanager-1.1.1/tests/file/test_base.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_hdf5.py` & `monolith_filemanager-1.1.1/tests/file/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_joblib_file.py` & `monolith_filemanager-1.1.1/tests/file/test_joblib_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_json_file.py` & `monolith_filemanager-1.1.1/tests/file/test_json_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_keras_model_file.py` & `monolith_filemanager-1.1.1/tests/file/test_keras_model_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_map.py` & `monolith_filemanager-1.1.1/tests/file/test_map.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_numpyfile.py` & `monolith_filemanager-1.1.1/tests/file/test_numpyfile.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_pandas.py` & `monolith_filemanager-1.1.1/tests/file/test_pandas.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_protobuf_file.py` & `monolith_filemanager-1.1.1/tests/file/test_protobuf_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_standard_pickle_file.py` & `monolith_filemanager-1.1.1/tests/file/test_standard_pickle_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_vtk.py` & `monolith_filemanager-1.1.1/tests/file/test_vtk.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/file/test_yml.py` & `monolith_filemanager-1.1.1/tests/file/test_yml.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/requirements_manager/test_requirements_manager.py` & `monolith_filemanager-1.1.1/tests/requirements_manager/test_requirements_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from unittest import TestCase
 
 from requirements_manager import RequirementsManager, OperatorEnum
 from requirements_manager.errors import NoPackagesInPipfileError, PipfilePathDoesNotExistError
 
 
 extras_packages = {
-    "flask": ["flask", "tensorflow", "boto3"],
+    "flask": ["flask", "tensorflow", "boto3", "protobuf", "jinja2", "itsdangerous", "werkzeug",
+              "markupsafe"],
     "3d": ["pyvista", "gmsh"],
     "matlab": ["scipy"]
 }
 
-flask_packages = ["flask>=1.1.2", "tensorflow>=2.2.0", "boto3>=1.10.5"]
-three_d_packages = ["gmsh>=4.8.4", "pyvista>=0.24.2"]
+flask_packages = ["flask>=1.1.4", "tensorflow>=2.2.0", "boto3>=1.10.5", "protobuf>=3.19.6",
+                  "jinja2>=2.11.3", "itsdangerous>=1.1.0", "werkzeug>=1.0.1", "markupsafe>=2.0.1"]
+three_d_packages = ["gmsh>=4.9.0", "pyvista>=0.34.2"]
 matlab_packages = ["scipy>=1.4.1"]
 
 all_packages = ['globre>=0.1.5', 'h5py>=2.10.0', 'joblib>=0.15.0', 'numpy>=1.16.4', 'pandas>=0.25.1',
                 'distributed>=2021.1.1', 'dill>=0.2.9', 'pyyaml>=5.1.2', 'boto3>=1.10.5', 'botocore>=1.13.5',
                 'requests>=2.22.0', 'openpyxl>=3.0.7', 'pyarrow>=0.16.0', 'xlwt>=1.3.0', 'xlrd>=1.2.0',
                 'dask[complete]>=2020.12.0'] + flask_packages + three_d_packages + matlab_packages
```

### Comparing `monolith_filemanager-1.1.0/tests/s3storage/test_bucket_manager.py` & `monolith_filemanager-1.1.1/tests/s3storage/test_bucket_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/s3storage/test_file_manager.py` & `monolith_filemanager-1.1.1/tests/s3storage/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.0/tests/s3storage/test_v1engine.py` & `monolith_filemanager-1.1.1/tests/s3storage/test_v1engine.py`

 * *Files identical despite different names*

