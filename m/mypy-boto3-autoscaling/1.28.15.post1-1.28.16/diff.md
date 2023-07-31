# Comparing `tmp/mypy-boto3-autoscaling-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.15.post1.tar` & `mypy-boto3-autoscaling-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.393021 mypy-boto3-autoscaling-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-07-29 10:02:34.385021 mypy-boto3-autoscaling-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.381021 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53486 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53403 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-29 09:38:49.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86078 2023-07-29 09:38:50.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.385021 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.393021 mypy-boto3-autoscaling-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:38:46.000000 mypy-boto3-autoscaling-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53486 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53403 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-31 19:32:06.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86691 2023-07-31 19:32:08.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86554 2023-07-31 19:32:07.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:32:46.000000 mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.238207 mypy-boto3-autoscaling-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-31 19:32:05.000000 mypy-boto3-autoscaling-1.28.16/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/LICENSE` & `mypy-boto3-autoscaling-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/PKG-INFO` & `mypy-boto3-autoscaling-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -397,14 +397,16 @@
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
+    AlarmSpecificationOutputTypeDef,
+    AlarmSpecificationTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
@@ -456,15 +458,14 @@
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
@@ -477,15 +478,14 @@
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
-    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
@@ -499,14 +499,16 @@
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
+    RefreshPreferencesOutputTypeDef,
+    RefreshPreferencesTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
     DescribeTagsTypeRequestTypeDef,
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/README.md` & `mypy-boto3-autoscaling-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -365,14 +365,16 @@
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
+    AlarmSpecificationOutputTypeDef,
+    AlarmSpecificationTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
@@ -424,15 +426,14 @@
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
@@ -445,15 +446,14 @@
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
-    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
@@ -467,14 +467,16 @@
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
+    RefreshPreferencesOutputTypeDef,
+    RefreshPreferencesTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
     DescribeTagsTypeRequestTypeDef,
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
+    "AlarmSpecificationOutputTypeDef",
+    "AlarmSpecificationTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
@@ -113,15 +115,14 @@
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
@@ -134,15 +135,14 @@
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
-    "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
@@ -156,14 +156,16 @@
     "DetachInstancesAnswerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
     "RollbackInstanceRefreshAnswerTypeDef",
     "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
+    "RefreshPreferencesOutputTypeDef",
+    "RefreshPreferencesTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
     "DescribeTagsTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
@@ -312,14 +314,30 @@
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
 
+AlarmSpecificationOutputTypeDef = TypedDict(
+    "AlarmSpecificationOutputTypeDef",
+    {
+        "Alarms": List[str],
+    },
+    total=False,
+)
+
+AlarmSpecificationTypeDef = TypedDict(
+    "AlarmSpecificationTypeDef",
+    {
+        "Alarms": Sequence[str],
+    },
+    total=False,
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmARN": str,
     },
     total=False,
@@ -1166,29 +1184,14 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesOutputTypeDef = TypedDict(
-    "RefreshPreferencesOutputTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": List[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1497,29 +1500,14 @@
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": Sequence[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -1734,14 +1722,46 @@
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesOutputTypeDef = TypedDict(
+    "RefreshPreferencesOutputTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": List[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
+        "AlarmSpecification": AlarmSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": Sequence[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
+        "AlarmSpecification": AlarmSpecificationTypeDef,
+    },
+    total=False,
+)
+
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
+    "AlarmSpecificationOutputTypeDef",
+    "AlarmSpecificationTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
@@ -112,15 +114,14 @@
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
@@ -133,15 +134,14 @@
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
-    "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
@@ -155,14 +155,16 @@
     "DetachInstancesAnswerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
     "RollbackInstanceRefreshAnswerTypeDef",
     "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
+    "RefreshPreferencesOutputTypeDef",
+    "RefreshPreferencesTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
     "DescribeTagsTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
@@ -309,14 +311,30 @@
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
 
+AlarmSpecificationOutputTypeDef = TypedDict(
+    "AlarmSpecificationOutputTypeDef",
+    {
+        "Alarms": List[str],
+    },
+    total=False,
+)
+
+AlarmSpecificationTypeDef = TypedDict(
+    "AlarmSpecificationTypeDef",
+    {
+        "Alarms": Sequence[str],
+    },
+    total=False,
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmARN": str,
     },
     total=False,
@@ -1119,29 +1137,14 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesOutputTypeDef = TypedDict(
-    "RefreshPreferencesOutputTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": List[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1430,29 +1433,14 @@
 
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": Sequence[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -1661,14 +1649,46 @@
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesOutputTypeDef = TypedDict(
+    "RefreshPreferencesOutputTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": List[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
+        "AlarmSpecification": AlarmSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": Sequence[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
+        "AlarmSpecification": AlarmSpecificationTypeDef,
+    },
+    total=False,
+)
+
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -397,14 +397,16 @@
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
+    AlarmSpecificationOutputTypeDef,
+    AlarmSpecificationTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
@@ -456,15 +458,14 @@
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
@@ -477,15 +478,14 @@
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
-    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
@@ -499,14 +499,16 @@
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
+    RefreshPreferencesOutputTypeDef,
+    RefreshPreferencesTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
     DescribeTagsTypeRequestTypeDef,
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
```

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.16/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15.post1/setup.py` & `mypy-boto3-autoscaling-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder"
         " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

