# Comparing `tmp/atms_utils-0.1.0.tar.gz` & `tmp/atms_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atms_utils-0.1.0.tar", max compression
+gzip compressed data, was "atms_utils-0.1.1.tar", max compression
```

## Comparing `atms_utils-0.1.0.tar` & `atms_utils-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.268222 atms_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0      617 2023-07-31 05:46:52.759694 atms_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1659 2023-07-04 10:19:51.268222 atms_utils-0.1.0/README.md
--rw-r--r--   0        0        0       47 2023-07-04 10:19:51.299233 atms_utils-0.1.0/src/atmsutils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.300232 atms_utils-0.1.0/src/atmsutils/aws/__init__.py
--rw-r--r--   0        0        0    22569 2023-07-04 10:19:51.300232 atms_utils-0.1.0/src/atmsutils/aws/aws_utils.py
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.301740 atms_utils-0.1.0/src/atmsutils/bamboo/__init__.py
--rw-r--r--   0        0        0     2705 2023-07-04 10:19:51.302749 atms_utils-0.1.0/src/atmsutils/bamboo/bamboo_utils.py
--rw-r--r--   0        0        0     4893 2023-07-04 10:19:51.302749 atms_utils-0.1.0/src/atmsutils/bamboo/log_bamboo_builds.py
--rw-r--r--   0        0        0      550 2023-07-04 10:19:51.303752 atms_utils-0.1.0/src/atmsutils/bamboo/log_bamboo_test.py
--rw-r--r--   0        0        0     3382 2023-07-04 10:19:51.304752 atms_utils-0.1.0/src/atmsutils/bamboo/mapping/report_mapping.json
--rw-r--r--   0        0        0      597 2023-07-04 10:19:51.305750 atms_utils-0.1.0/src/atmsutils/bamboo/sql/bamboo_builds.ddl
--rw-r--r--   0        0        0      100 2023-07-04 10:19:51.305750 atms_utils-0.1.0/src/atmsutils/bamboo/sql/max_completed_at.sql
--rw-r--r--   0        0        0     7096 2023-07-04 10:19:51.305750 atms_utils-0.1.0/src/atmsutils/functions.py
--rw-r--r--   0        0        0      297 2023-07-31 05:21:19.739203 atms_utils-0.1.0/src/atmsutils/geo_utils/__init__.py
--rw-r--r--   0        0        0     5831 2023-07-31 05:21:19.740192 atms_utils-0.1.0/src/atmsutils/geo_utils/geo_analysis.py
--rw-r--r--   0        0        0     4496 2023-07-31 05:21:19.741182 atms_utils-0.1.0/src/atmsutils/geo_utils/geo_data_handler.py
--rw-r--r--   0        0        0     7708 2023-07-31 05:21:19.742192 atms_utils-0.1.0/src/atmsutils/geo_utils/geo_processor.py
--rw-r--r--   0        0        0        0 2023-07-04 10:19:51.306750 atms_utils-0.1.0/src/atmsutils/odbc/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-04 10:19:51.307749 atms_utils-0.1.0/src/atmsutils/odbc/odbc_utils.py
--rw-r--r--   0        0        0      179 2023-07-04 15:28:12.178883 atms_utils-0.1.0/src/atmsutils/test_submodul
--rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 atms_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.268222 atms_utils-0.1.1/LICENSE
+-rw-r--r--   0        0        0      614 2023-07-31 06:08:54.744552 atms_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1659 2023-07-04 10:19:51.268222 atms_utils-0.1.1/README.md
+-rw-r--r--   0        0        0       47 2023-07-04 10:19:51.299233 atms_utils-0.1.1/src/atmsutils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.300232 atms_utils-0.1.1/src/atmsutils/aws/__init__.py
+-rw-r--r--   0        0        0    22569 2023-07-04 10:19:51.300232 atms_utils-0.1.1/src/atmsutils/aws/aws_utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.301740 atms_utils-0.1.1/src/atmsutils/bamboo/__init__.py
+-rw-r--r--   0        0        0     2705 2023-07-04 10:19:51.302749 atms_utils-0.1.1/src/atmsutils/bamboo/bamboo_utils.py
+-rw-r--r--   0        0        0     4893 2023-07-04 10:19:51.302749 atms_utils-0.1.1/src/atmsutils/bamboo/log_bamboo_builds.py
+-rw-r--r--   0        0        0      550 2023-07-04 10:19:51.303752 atms_utils-0.1.1/src/atmsutils/bamboo/log_bamboo_test.py
+-rw-r--r--   0        0        0     3382 2023-07-04 10:19:51.304752 atms_utils-0.1.1/src/atmsutils/bamboo/mapping/report_mapping.json
+-rw-r--r--   0        0        0      597 2023-07-04 10:19:51.305750 atms_utils-0.1.1/src/atmsutils/bamboo/sql/bamboo_builds.ddl
+-rw-r--r--   0        0        0      100 2023-07-04 10:19:51.305750 atms_utils-0.1.1/src/atmsutils/bamboo/sql/max_completed_at.sql
+-rw-r--r--   0        0        0     7096 2023-07-04 10:19:51.305750 atms_utils-0.1.1/src/atmsutils/functions.py
+-rw-r--r--   0        0        0      297 2023-07-31 05:21:19.739203 atms_utils-0.1.1/src/atmsutils/geo_utils/__init__.py
+-rw-r--r--   0        0        0     5831 2023-07-31 05:21:19.740192 atms_utils-0.1.1/src/atmsutils/geo_utils/geo_analysis.py
+-rw-r--r--   0        0        0     4496 2023-07-31 05:21:19.741182 atms_utils-0.1.1/src/atmsutils/geo_utils/geo_data_handler.py
+-rw-r--r--   0        0        0     7708 2023-07-31 05:21:19.742192 atms_utils-0.1.1/src/atmsutils/geo_utils/geo_processor.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:19:51.306750 atms_utils-0.1.1/src/atmsutils/odbc/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-04 10:19:51.307749 atms_utils-0.1.1/src/atmsutils/odbc/odbc_utils.py
+-rw-r--r--   0        0        0      179 2023-07-04 15:28:12.178883 atms_utils-0.1.1/src/atmsutils/test_submodul
+-rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 atms_utils-0.1.1/PKG-INFO
```

### Comparing `atms_utils-0.1.0/pyproject.toml` & `atms_utils-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "atms-utils"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["jakub.sulek <jakub.sulek@atmstechnology.com>"]
 readme = "README.md"
 packages = [{include = "atmsutils", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-jinja2 = ">=3.0.1"
+jinja2 = "~2"
 numpy = ">=1.20.3"
 pandas = ">=1.3.1"
 pytest = ">=6.2.4"
 sqlalchemy = ">=1.4.22"
 psycopg2 = ">=2.9"
 pymysql = ">=1.0.0"
-boto3 = ">=1.18"
+boto3 = "^1.23.6"
 pyyaml = "^6.0"
 botocore = "^1.31.2"
-requests = "2.26.0"
+requests = "^2.27.1"
 beautifulsoup4 = "4.9.3"
 matplotlib = "3.5.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `atms_utils-0.1.0/README.md` & `atms_utils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/aws/aws_utils.py` & `atms_utils-0.1.1/src/atmsutils/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/bamboo/bamboo_utils.py` & `atms_utils-0.1.1/src/atmsutils/bamboo/bamboo_utils.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/bamboo/log_bamboo_builds.py` & `atms_utils-0.1.1/src/atmsutils/bamboo/log_bamboo_builds.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/bamboo/log_bamboo_test.py` & `atms_utils-0.1.1/src/atmsutils/bamboo/log_bamboo_test.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/bamboo/mapping/report_mapping.json` & `atms_utils-0.1.1/src/atmsutils/bamboo/mapping/report_mapping.json`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/bamboo/sql/bamboo_builds.ddl` & `atms_utils-0.1.1/src/atmsutils/bamboo/sql/bamboo_builds.ddl`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/functions.py` & `atms_utils-0.1.1/src/atmsutils/functions.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/geo_utils/geo_analysis.py` & `atms_utils-0.1.1/src/atmsutils/geo_utils/geo_analysis.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/geo_utils/geo_data_handler.py` & `atms_utils-0.1.1/src/atmsutils/geo_utils/geo_data_handler.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/geo_utils/geo_processor.py` & `atms_utils-0.1.1/src/atmsutils/geo_utils/geo_processor.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/src/atmsutils/odbc/odbc_utils.py` & `atms_utils-0.1.1/src/atmsutils/odbc/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `atms_utils-0.1.0/PKG-INFO` & `atms_utils-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: atms-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: jakub.sulek
 Author-email: jakub.sulek@atmstechnology.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (==4.9.3)
-Requires-Dist: boto3 (>=1.18)
+Requires-Dist: boto3 (>=1.23.6,<2.0.0)
 Requires-Dist: botocore (>=1.31.2,<2.0.0)
-Requires-Dist: jinja2 (>=3.0.1)
+Requires-Dist: jinja2 (>=2,<3)
 Requires-Dist: matplotlib (==3.5.2)
 Requires-Dist: numpy (>=1.20.3)
 Requires-Dist: pandas (>=1.3.1)
 Requires-Dist: psycopg2 (>=2.9)
 Requires-Dist: pymysql (>=1.0.0)
 Requires-Dist: pytest (>=6.2.4)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (==2.26.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4.22)
 Description-Content-Type: text/markdown
 
 ATMS Utils
 ==============================
 
 Python package atms_utils provides:
```

