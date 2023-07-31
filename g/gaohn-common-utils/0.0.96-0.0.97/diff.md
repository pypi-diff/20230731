# Comparing `tmp/gaohn-common-utils-0.0.96.tar.gz` & `tmp/gaohn-common-utils-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.96.tar", last modified: Wed Jul 26 11:38:36 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.97.tar", last modified: Mon Jul 31 04:48:39 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.96.tar` & `gaohn-common-utils-0.0.97.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/decorators/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/orchestrator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/orchestrator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/common_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/tests/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.364656 gaohn-common-utils-0.0.96/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-26 11:38:36.000000 gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-26 11:38:36.000000 gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:38:36.000000 gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-26 11:38:36.000000 gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 11:38:36.000000 gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-26 11:38:18.000000 gaohn-common-utils-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:38:36.368656 gaohn-common-utils-0.0.96/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.696689 gaohn-common-utils-0.0.97/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.696689 gaohn-common-utils-0.0.97/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.692689 gaohn-common-utils-0.0.97/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.696689 gaohn-common-utils-0.0.97/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.696689 gaohn-common-utils-0.0.97/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.696689 gaohn-common-utils-0.0.97/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.696689 gaohn-common-utils-0.0.97/common_utils/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/decorators/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.692689 gaohn-common-utils-0.0.97/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/orchestrator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/orchestrator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/common_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/tests/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.692689 gaohn-common-utils-0.0.97/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-31 04:48:39.000000 gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-31 04:48:39.000000 gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:48:39.000000 gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-31 04:48:39.000000 gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 04:48:39.000000 gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-31 04:48:22.000000 gaohn-common-utils-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 04:48:39.700690 gaohn-common-utils-0.0.97/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.96/LICENSE` & `gaohn-common-utils-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/PKG-INFO` & `gaohn-common-utils-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.96
+Version: 0.0.97
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.96/README.md` & `gaohn-common-utils-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.97/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.97/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.97/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/core/base.py` & `gaohn-common-utils-0.0.97/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/core/common.py` & `gaohn-common-utils-0.0.97/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/core/decorators/decorators.py` & `gaohn-common-utils-0.0.97/common_utils/core/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/core/decorators/timer.py` & `gaohn-common-utils-0.0.97/common_utils/core/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.97/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/core/logger.py` & `gaohn-common-utils-0.0.97/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.97/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.97/common_utils/experiment_tracking/promoter/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.97/common_utils/experiment_tracking/promoter/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/orchestrator/core.py` & `gaohn-common-utils-0.0.97/common_utils/orchestrator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/tests/core.py` & `gaohn-common-utils-0.0.97/common_utils/tests/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.97/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.97/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.96
+Version: 0.0.97
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.96/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.97/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.96/pyproject.toml` & `gaohn-common-utils-0.0.97/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.96"
+version = "0.0.97"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

