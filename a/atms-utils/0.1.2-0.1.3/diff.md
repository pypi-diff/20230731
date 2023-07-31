# Comparing `tmp/atms_utils-0.1.2.tar.gz` & `tmp/atms_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atms_utils-0.1.2.tar", max compression
+gzip compressed data, was "atms_utils-0.1.3.tar", max compression
```

## Comparing `atms_utils-0.1.2.tar` & `atms_utils-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.268222 atms_utils-0.1.2/LICENSE
--rw-r--r--   0        0        0      592 2023-07-31 06:50:46.592036 atms_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1659 2023-07-04 10:19:51.268222 atms_utils-0.1.2/README.md
--rw-r--r--   0        0        0       47 2023-07-04 10:19:51.299233 atms_utils-0.1.2/src/atmsutils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.300232 atms_utils-0.1.2/src/atmsutils/aws/__init__.py
--rw-r--r--   0        0        0    22569 2023-07-04 10:19:51.300232 atms_utils-0.1.2/src/atmsutils/aws/aws_utils.py
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.301740 atms_utils-0.1.2/src/atmsutils/bamboo/__init__.py
--rw-r--r--   0        0        0     2705 2023-07-04 10:19:51.302749 atms_utils-0.1.2/src/atmsutils/bamboo/bamboo_utils.py
--rw-r--r--   0        0        0     4893 2023-07-04 10:19:51.302749 atms_utils-0.1.2/src/atmsutils/bamboo/log_bamboo_builds.py
--rw-r--r--   0        0        0      550 2023-07-04 10:19:51.303752 atms_utils-0.1.2/src/atmsutils/bamboo/log_bamboo_test.py
--rw-r--r--   0        0        0     3382 2023-07-04 10:19:51.304752 atms_utils-0.1.2/src/atmsutils/bamboo/mapping/report_mapping.json
--rw-r--r--   0        0        0      597 2023-07-04 10:19:51.305750 atms_utils-0.1.2/src/atmsutils/bamboo/sql/bamboo_builds.ddl
--rw-r--r--   0        0        0      100 2023-07-04 10:19:51.305750 atms_utils-0.1.2/src/atmsutils/bamboo/sql/max_completed_at.sql
--rw-r--r--   0        0        0     7096 2023-07-04 10:19:51.305750 atms_utils-0.1.2/src/atmsutils/functions.py
--rw-r--r--   0        0        0      297 2023-07-31 05:21:19.739203 atms_utils-0.1.2/src/atmsutils/geo_utils/__init__.py
--rw-r--r--   0        0        0     5831 2023-07-31 05:21:19.740192 atms_utils-0.1.2/src/atmsutils/geo_utils/geo_analysis.py
--rw-r--r--   0        0        0     4496 2023-07-31 05:21:19.741182 atms_utils-0.1.2/src/atmsutils/geo_utils/geo_data_handler.py
--rw-r--r--   0        0        0     7708 2023-07-31 05:21:19.742192 atms_utils-0.1.2/src/atmsutils/geo_utils/geo_processor.py
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.306750 atms_utils-0.1.2/src/atmsutils/odbc/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-04 10:19:51.307749 atms_utils-0.1.2/src/atmsutils/odbc/odbc_utils.py
--rw-r--r--   0        0        0      179 2023-07-04 15:28:12.178883 atms_utils-0.1.2/src/atmsutils/test_submodul
--rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 atms_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.268222 atms_utils-0.1.3/LICENSE
+-rw-r--r--   0        0        0      592 2023-07-31 06:59:04.449173 atms_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1314 2023-07-31 06:58:31.040741 atms_utils-0.1.3/README.md
+-rw-r--r--   0        0        0       47 2023-07-04 10:19:51.299233 atms_utils-0.1.3/src/atmsutils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.300232 atms_utils-0.1.3/src/atmsutils/aws/__init__.py
+-rw-r--r--   0        0        0    22569 2023-07-04 10:19:51.300232 atms_utils-0.1.3/src/atmsutils/aws/aws_utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.301740 atms_utils-0.1.3/src/atmsutils/bamboo/__init__.py
+-rw-r--r--   0        0        0     2705 2023-07-04 10:19:51.302749 atms_utils-0.1.3/src/atmsutils/bamboo/bamboo_utils.py
+-rw-r--r--   0        0        0     4893 2023-07-04 10:19:51.302749 atms_utils-0.1.3/src/atmsutils/bamboo/log_bamboo_builds.py
+-rw-r--r--   0        0        0      550 2023-07-04 10:19:51.303752 atms_utils-0.1.3/src/atmsutils/bamboo/log_bamboo_test.py
+-rw-r--r--   0        0        0     3382 2023-07-04 10:19:51.304752 atms_utils-0.1.3/src/atmsutils/bamboo/mapping/report_mapping.json
+-rw-r--r--   0        0        0      597 2023-07-04 10:19:51.305750 atms_utils-0.1.3/src/atmsutils/bamboo/sql/bamboo_builds.ddl
+-rw-r--r--   0        0        0      100 2023-07-04 10:19:51.305750 atms_utils-0.1.3/src/atmsutils/bamboo/sql/max_completed_at.sql
+-rw-r--r--   0        0        0     7096 2023-07-04 10:19:51.305750 atms_utils-0.1.3/src/atmsutils/functions.py
+-rw-r--r--   0        0        0      297 2023-07-31 05:21:19.739203 atms_utils-0.1.3/src/atmsutils/geo_utils/__init__.py
+-rw-r--r--   0        0        0     5831 2023-07-31 05:21:19.740192 atms_utils-0.1.3/src/atmsutils/geo_utils/geo_analysis.py
+-rw-r--r--   0        0        0     4496 2023-07-31 05:21:19.741182 atms_utils-0.1.3/src/atmsutils/geo_utils/geo_data_handler.py
+-rw-r--r--   0        0        0     7708 2023-07-31 05:21:19.742192 atms_utils-0.1.3/src/atmsutils/geo_utils/geo_processor.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.306750 atms_utils-0.1.3/src/atmsutils/odbc/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-04 10:19:51.307749 atms_utils-0.1.3/src/atmsutils/odbc/odbc_utils.py
+-rw-r--r--   0        0        0      179 2023-07-04 15:28:12.178883 atms_utils-0.1.3/src/atmsutils/test_submodul
+-rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 atms_utils-0.1.3/PKG-INFO
```

### Comparing `atms_utils-0.1.2/pyproject.toml` & `atms_utils-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atms-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["jakub.sulek <jakub.sulek@atmstechnology.com>"]
 readme = "README.md"
 packages = [{include = "atmsutils", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `atms_utils-0.1.2/src/atmsutils/aws/aws_utils.py` & `atms_utils-0.1.3/src/atmsutils/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/bamboo/bamboo_utils.py` & `atms_utils-0.1.3/src/atmsutils/bamboo/bamboo_utils.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/bamboo/log_bamboo_builds.py` & `atms_utils-0.1.3/src/atmsutils/bamboo/log_bamboo_builds.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/bamboo/log_bamboo_test.py` & `atms_utils-0.1.3/src/atmsutils/bamboo/log_bamboo_test.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/bamboo/mapping/report_mapping.json` & `atms_utils-0.1.3/src/atmsutils/bamboo/mapping/report_mapping.json`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/bamboo/sql/bamboo_builds.ddl` & `atms_utils-0.1.3/src/atmsutils/bamboo/sql/bamboo_builds.ddl`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/functions.py` & `atms_utils-0.1.3/src/atmsutils/functions.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/geo_utils/geo_analysis.py` & `atms_utils-0.1.3/src/atmsutils/geo_utils/geo_analysis.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/geo_utils/geo_data_handler.py` & `atms_utils-0.1.3/src/atmsutils/geo_utils/geo_data_handler.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/geo_utils/geo_processor.py` & `atms_utils-0.1.3/src/atmsutils/geo_utils/geo_processor.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/src/atmsutils/odbc/odbc_utils.py` & `atms_utils-0.1.3/src/atmsutils/odbc/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.2/PKG-INFO` & `atms_utils-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atms-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: jakub.sulek
 Author-email: jakub.sulek@atmstechnology.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -40,30 +40,15 @@
 - change directory to the `atms-utils`  
 - Run `pip install .`  
 
 Prerequisites
 ==============================
 - Add `config.ini` file with your credentials to the root folder of your project
 - Example for Redshift and MySQL:
-```
-[redshift]
-Host = redshift-itrack-analytics.ckf2lv5nbsbo.eu-west-1.redshift.amazonaws.com
-Database = itrack_analytics
-Port = 5439
-User = <your_username>
-Password = <your_password>
-
-[mysql-rep]
-Host = itrack-db-reporting.atmstechnology.com
-Database = itrack_beta
-Port = 3306
-User = <your_username>
-Password = <your_password>
-```
-
+- 
 Supported Python versions
 ===============
 Default python version is 3.8
 
 Examples
 ===============
 - run `python examples/mysql_connection.py` which will load the dataframe from MySQL for one customer
```

