# Comparing `tmp/aliyun-python-sdk-dts-5.1.8.tar.gz` & `tmp/aliyun-python-sdk-dts-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dts-5.1.8.tar", last modified: Fri Jan 15 03:24:35 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dts-5.1.9.tar", last modified: Sat Jan 30 10:13:06 2021, max compression
```

## Comparing `aliyun-python-sdk-dts-5.1.8.tar` & `aliyun-python-sdk-dts-5.1.9.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/
--rw-r--r--   0 root         (0) root         (0)      575 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3762 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/
--rw-r--r--   0 root         (0) root         (0)       21 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3470 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/
--rw-r--r--   0 root         (0) root         (0)     2834 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureMigrationJobAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     9210 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureMigrationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2898 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     6126 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3138 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     2652 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobReplicatorCompareRequest.py
--rw-r--r--   0 root         (0) root         (0)     8952 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2530 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2134 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateMigrationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2668 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateSubscriptionInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3962 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateSynchronizationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2042 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1790 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteMigrationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1854 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteSubscriptionInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1838 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteSynchronizationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     7044 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeConnectionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2158 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1758 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeDTSIPRequest.py
--rw-r--r--   0 root         (0) root         (0)     1940 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeEndpointSwitchStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2160 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeInitializationStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1982 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     3234 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2520 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2046 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     1870 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2762 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2286 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     2310 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobReplicatorCompareRequest.py
--rw-r--r--   0 root         (0) root         (0)     2106 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2288 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2746 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1966 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationObjectModifyStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2306 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3004 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifyConsumerGroupPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2086 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifyConsumptionTimestampRequest.py
--rw-r--r--   0 root         (0) root         (0)     2176 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifyMigrationObjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifySubscriptionObjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2344 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifySynchronizationObjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2092 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ResetSynchronizationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ShieldPrecheckRequest.py
--rw-r--r--   0 root         (0) root         (0)     1788 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StartMigrationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1852 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StartSubscriptionInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2092 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StartSynchronizationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1964 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StopMigrationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1970 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/SuspendMigrationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2096 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/SuspendSynchronizationJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3568 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/SwitchSynchronizationEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2021-01-15 03:24:35.000000 aliyun-python-sdk-dts-5.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3699 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/
+-rw-r--r--   0 root         (0) root         (0)     2834 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureMigrationJobAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9210 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureMigrationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6126 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2652 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobReplicatorCompareRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8952 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateMigrationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateSubscriptionInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateSynchronizationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteMigrationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteSubscriptionInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteSynchronizationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7044 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeConnectionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeDTSIPRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeEndpointSwitchStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeInitializationStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobReplicatorCompareRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationObjectModifyStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifyConsumerGroupPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifyConsumptionTimestampRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifySubscriptionObjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifySynchronizationObjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ResetSynchronizationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ShieldPrecheckRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StartMigrationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StartSubscriptionInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StartSynchronizationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StopMigrationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/SuspendMigrationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/SuspendSynchronizationJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/SwitchSynchronizationEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-01-30 10:13:06.000000 aliyun-python-sdk-dts-5.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2021-01-30 10:13:05.000000 aliyun-python-sdk-dts-5.1.9/setup.py
```

### Comparing `aliyun-python-sdk-dts-5.1.8/LICENSE` & `aliyun-python-sdk-dts-5.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/PKG-INFO` & `aliyun-python-sdk-dts-5.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dts
-Version: 5.1.8
+Version: 5.1.9
 Summary: The dts module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dts
```

### Comparing `aliyun-python-sdk-dts-5.1.8/README.rst` & `aliyun-python-sdk-dts-5.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/PKG-INFO` & `aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dts
-Version: 5.1.8
+Version: 5.1.9
 Summary: The dts module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dts
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyun_python_sdk_dts.egg-info/SOURCES.txt` & `aliyun-python-sdk-dts-5.1.9/aliyun_python_sdk_dts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusListRequest.py
 aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusRequest.py
 aliyunsdkdts/request/v20200101/DescribeSynchronizationJobsRequest.py
 aliyunsdkdts/request/v20200101/DescribeSynchronizationObjectModifyStatusRequest.py
 aliyunsdkdts/request/v20200101/ListTagResourcesRequest.py
 aliyunsdkdts/request/v20200101/ModifyConsumerGroupPasswordRequest.py
 aliyunsdkdts/request/v20200101/ModifyConsumptionTimestampRequest.py
-aliyunsdkdts/request/v20200101/ModifyMigrationObjectRequest.py
 aliyunsdkdts/request/v20200101/ModifySubscriptionObjectRequest.py
 aliyunsdkdts/request/v20200101/ModifySynchronizationObjectRequest.py
 aliyunsdkdts/request/v20200101/ResetSynchronizationJobRequest.py
 aliyunsdkdts/request/v20200101/ShieldPrecheckRequest.py
 aliyunsdkdts/request/v20200101/StartMigrationJobRequest.py
 aliyunsdkdts/request/v20200101/StartSubscriptionInstanceRequest.py
 aliyunsdkdts/request/v20200101/StartSynchronizationJobRequest.py
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/endpoint.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureMigrationJobAlertRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureMigrationJobAlertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureMigrationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureMigrationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceAlertRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceAlertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSubscriptionInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobAlertRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobAlertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobReplicatorCompareRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobReplicatorCompareRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ConfigureSynchronizationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateConsumerGroupRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateConsumerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateMigrationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateMigrationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateSubscriptionInstanceRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateSubscriptionInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/CreateSynchronizationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/CreateSynchronizationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteConsumerGroupRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteConsumerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteMigrationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteMigrationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteSubscriptionInstanceRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteSubscriptionInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DeleteSynchronizationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DeleteSynchronizationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeConnectionStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeConnectionStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeConsumerGroupRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeConsumerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeDTSIPRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeDTSIPRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeEndpointSwitchStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeEndpointSwitchStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeInitializationStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeInitializationStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobAlertRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobAlertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobDetailRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeMigrationJobsRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeMigrationJobsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
 	def get_MigrationJobName(self):
 		return self.get_query_params().get('MigrationJobName')
 
 	def set_MigrationJobName(self,MigrationJobName):
 		self.add_query_param('MigrationJobName',MigrationJobName)
 
-	def get_Tag(self):
+	def get_Tags(self):
 		return self.get_query_params().get('Tag')
 
-	def set_Tag(self, Tags):
+	def set_Tags(self, Tags):
 		for depth1 in range(len(Tags)):
 			if Tags[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
 			if Tags[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceAlertRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceAlertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstanceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstancesRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSubscriptionInstancesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
 	def get_SubscriptionInstanceName(self):
 		return self.get_query_params().get('SubscriptionInstanceName')
 
 	def set_SubscriptionInstanceName(self,SubscriptionInstanceName):
 		self.add_query_param('SubscriptionInstanceName',SubscriptionInstanceName)
 
-	def get_Tag(self):
+	def get_Tags(self):
 		return self.get_query_params().get('Tag')
 
-	def set_Tag(self, Tags):
+	def set_Tags(self, Tags):
 		for depth1 in range(len(Tags)):
 			if Tags[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
 			if Tags[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobAlertRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobAlertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobReplicatorCompareRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobReplicatorCompareRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusListRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobsRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationJobsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
-	def get_Tag(self):
+	def get_Tags(self):
 		return self.get_query_params().get('Tag')
 
-	def set_Tag(self, Tags):
+	def set_Tags(self, Tags):
 		for depth1 in range(len(Tags)):
 			if Tags[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
 			if Tags[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/DescribeSynchronizationObjectModifyStatusRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/DescribeSynchronizationObjectModifyStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ListTagResourcesRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ListTagResourcesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,28 @@
 
 	def get_NextToken(self):
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self,NextToken):
 		self.add_query_param('NextToken',NextToken)
 
-	def get_Tag(self):
+	def get_Tags(self):
 		return self.get_query_params().get('Tag')
 
-	def set_Tag(self, Tags):
+	def set_Tags(self, Tags):
 		for depth1 in range(len(Tags)):
 			if Tags[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
 			if Tags[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
 
-	def get_ResourceId(self):
+	def get_ResourceIds(self):
 		return self.get_query_params().get('ResourceId')
 
-	def set_ResourceId(self, ResourceIds):
+	def set_ResourceIds(self, ResourceIds):
 		for depth1 in range(len(ResourceIds)):
 			if ResourceIds[depth1] is not None:
 				self.add_query_param('ResourceId.' + str(depth1 + 1) , ResourceIds[depth1])
 
 	def get_ResourceType(self):
 		return self.get_query_params().get('ResourceType')
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifyConsumerGroupPasswordRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifyConsumerGroupPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifyConsumptionTimestampRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifyConsumptionTimestampRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifyMigrationObjectRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/SuspendMigrationJobRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,31 +16,25 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdts.endpoint import endpoint_data
 
-class ModifyMigrationObjectRequest(RpcRequest):
+class SuspendMigrationJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dts', '2020-01-01', 'ModifyMigrationObject','dts')
+		RpcRequest.__init__(self, 'Dts', '2020-01-01', 'SuspendMigrationJob','dts')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_MigrationObject(self):
-		return self.get_query_params().get('MigrationObject')
-
-	def set_MigrationObject(self,MigrationObject):
-		self.add_query_param('MigrationObject',MigrationObject)
-
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
 	def get_MigrationJobId(self):
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifySubscriptionObjectRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifySubscriptionObjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ModifySynchronizationObjectRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ModifySynchronizationObjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ResetSynchronizationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ResetSynchronizationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/ShieldPrecheckRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/ShieldPrecheckRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StartMigrationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StartMigrationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StartSubscriptionInstanceRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StartSubscriptionInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StartSynchronizationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StartSynchronizationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/StopMigrationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/StopMigrationJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/SuspendMigrationJobRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/SuspendSynchronizationJobRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,41 +16,41 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdts.endpoint import endpoint_data
 
-class SuspendMigrationJobRequest(RpcRequest):
+class SuspendSynchronizationJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dts', '2020-01-01', 'SuspendMigrationJob','dts')
+		RpcRequest.__init__(self, 'Dts', '2020-01-01', 'SuspendSynchronizationJob','dts')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_ClientToken(self):
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self,ClientToken):
-		self.add_query_param('ClientToken',ClientToken)
-
-	def get_MigrationJobId(self):
-		return self.get_query_params().get('MigrationJobId')
-
-	def set_MigrationJobId(self,MigrationJobId):
-		self.add_query_param('MigrationJobId',MigrationJobId)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
+	def get_SynchronizationJobId(self):
+		return self.get_query_params().get('SynchronizationJobId')
+
+	def set_SynchronizationJobId(self,SynchronizationJobId):
+		self.add_query_param('SynchronizationJobId',SynchronizationJobId)
+
 	def get_AccountId(self):
 		return self.get_query_params().get('AccountId')
 
 	def set_AccountId(self,AccountId):
-		self.add_query_param('AccountId',AccountId)
+		self.add_query_param('AccountId',AccountId)
+
+	def get_SynchronizationDirection(self):
+		return self.get_query_params().get('SynchronizationDirection')
+
+	def set_SynchronizationDirection(self,SynchronizationDirection):
+		self.add_query_param('SynchronizationDirection',SynchronizationDirection)
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/SwitchSynchronizationEndpointRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/SwitchSynchronizationEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/TagResourcesRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/TagResourcesRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_Tag(self):
+	def get_Tags(self):
 		return self.get_query_params().get('Tag')
 
-	def set_Tag(self, Tags):
+	def set_Tags(self, Tags):
 		for depth1 in range(len(Tags)):
 			if Tags[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
 			if Tags[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
 
-	def get_ResourceId(self):
+	def get_ResourceIds(self):
 		return self.get_query_params().get('ResourceId')
 
-	def set_ResourceId(self, ResourceIds):
+	def set_ResourceIds(self, ResourceIds):
 		for depth1 in range(len(ResourceIds)):
 			if ResourceIds[depth1] is not None:
 				self.add_query_param('ResourceId.' + str(depth1 + 1) , ResourceIds[depth1])
 
 	def get_ResourceType(self):
 		return self.get_query_params().get('ResourceType')
```

### Comparing `aliyun-python-sdk-dts-5.1.8/aliyunsdkdts/request/v20200101/UntagResourcesRequest.py` & `aliyun-python-sdk-dts-5.1.9/aliyunsdkdts/request/v20200101/UntagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,28 +33,28 @@
 
 	def get_All(self):
 		return self.get_query_params().get('All')
 
 	def set_All(self,All):
 		self.add_query_param('All',All)
 
-	def get_ResourceId(self):
+	def get_ResourceIds(self):
 		return self.get_query_params().get('ResourceId')
 
-	def set_ResourceId(self, ResourceIds):
+	def set_ResourceIds(self, ResourceIds):
 		for depth1 in range(len(ResourceIds)):
 			if ResourceIds[depth1] is not None:
 				self.add_query_param('ResourceId.' + str(depth1 + 1) , ResourceIds[depth1])
 
 	def get_ResourceType(self):
 		return self.get_query_params().get('ResourceType')
 
 	def set_ResourceType(self,ResourceType):
 		self.add_query_param('ResourceType',ResourceType)
 
-	def get_TagKey(self):
+	def get_TagKeys(self):
 		return self.get_query_params().get('TagKey')
 
-	def set_TagKey(self, TagKeys):
+	def set_TagKeys(self, TagKeys):
 		for depth1 in range(len(TagKeys)):
 			if TagKeys[depth1] is not None:
 				self.add_query_param('TagKey.' + str(depth1 + 1) , TagKeys[depth1])
```

### Comparing `aliyun-python-sdk-dts-5.1.8/setup.py` & `aliyun-python-sdk-dts-5.1.9/setup.py`

 * *Files identical despite different names*

