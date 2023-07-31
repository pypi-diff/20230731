# Comparing `tmp/mypy-boto3-inspector2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-inspector2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:16 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
```

## Comparing `mypy-boto3-inspector2-1.28.15.post1.tar` & `mypy-boto3-inspector2-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.681174 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36019 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35957 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75649 2023-07-29 09:47:22.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75568 2023-07-29 09:47:21.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:47:17.000000 mypy-boto3-inspector2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.242207 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36576 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36513 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    77088 2023-07-31 19:32:17.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77007 2023-07-31 19:32:16.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/setup.py
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/LICENSE` & `mypy-boto3-inspector2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15.post1/PKG-INFO` & `mypy-boto3-inspector2-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -349,14 +349,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -435,14 +436,16 @@
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
+    BatchGetFindingDetailsRequestRequestTypeDef,
+    FindingDetailsErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
@@ -475,14 +478,15 @@
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
+    EvidenceTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
@@ -563,14 +567,15 @@
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
+    FindingDetailTypeDef,
     VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
     ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
@@ -596,14 +601,15 @@
     ListCoverageRequestListCoveragePaginateTypeDef,
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
     GetSbomExportResponseTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/README.md` & `mypy-boto3-inspector2-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -317,14 +317,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -403,14 +404,16 @@
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
+    BatchGetFindingDetailsRequestRequestTypeDef,
+    FindingDetailsErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
@@ -443,14 +446,15 @@
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
+    EvidenceTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
@@ -531,14 +535,15 @@
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
+    FindingDetailTypeDef,
     VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
     ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
@@ -564,14 +569,15 @@
     ListCoverageRequestListCoveragePaginateTypeDef,
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
     GetSbomExportResponseTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AutoEnableTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     CancelFindingsReportResponseTypeDef,
     CancelSbomExportResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CreateFilterResponseTypeDef,
@@ -97,38 +98,34 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Inspector2Client",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class Inspector2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/)
     """
 
     meta: ClientMeta
@@ -137,110 +134,108 @@
     def exceptions(self) -> Exceptions:
         """
         Inspector2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#exceptions)
         """
-
     def associate_member(self, *, accountId: str) -> AssociateMemberResponseTypeDef:
         """
         Associates an Amazon Web Services account with an Amazon Inspector delegated
         administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.associate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#associate_member)
         """
-
     def batch_get_account_status(
         self, *, accountIds: Sequence[str] = ...
     ) -> BatchGetAccountStatusResponseTypeDef:
         """
         Retrieves the Amazon Inspector status of multiple Amazon Web Services accounts
         within your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_account_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_account_status)
         """
-
     def batch_get_code_snippet(
         self, *, findingArns: Sequence[str]
     ) -> BatchGetCodeSnippetResponseTypeDef:
         """
         Retrieves code snippets from findings that Amazon Inspector detected code
         vulnerabilities in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_code_snippet)
         """
+    def batch_get_finding_details(
+        self, *, findingArns: Sequence[str]
+    ) -> BatchGetFindingDetailsResponseTypeDef:
+        """
+        Gets vulnerability details for findings.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_finding_details)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_finding_details)
+        """
     def batch_get_free_trial_info(
         self, *, accountIds: Sequence[str]
     ) -> BatchGetFreeTrialInfoResponseTypeDef:
         """
         Gets free trial status for multiple Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_free_trial_info)
         """
-
     def batch_get_member_ec2_deep_inspection_status(
         self, *, accountIds: Sequence[str] = ...
     ) -> BatchGetMemberEc2DeepInspectionStatusResponseTypeDef:
         """
         Retrieves Amazon Inspector deep inspection activation status of multiple member
         accounts within your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_member_ec2_deep_inspection_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_member_ec2_deep_inspection_status)
         """
-
     def batch_update_member_ec2_deep_inspection_status(
         self, *, accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef]
     ) -> BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef:
         """
         Activates or deactivates Amazon Inspector deep inspection for the provided
         member accounts in your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_update_member_ec2_deep_inspection_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_update_member_ec2_deep_inspection_status)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#can_paginate)
         """
-
     def cancel_findings_report(self, *, reportId: str) -> CancelFindingsReportResponseTypeDef:
         """
         Cancels the given findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_findings_report)
         """
-
     def cancel_sbom_export(self, *, reportId: str) -> CancelSbomExportResponseTypeDef:
         """
         Cancels a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_sbom_export)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
-
     def create_filter(
         self,
         *,
         action: FilterActionType,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef],
         name: str,
         description: str = ...,
@@ -249,29 +244,27 @@
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_filter)
         """
-
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
-
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
         resourceFilterCriteria: Union[
             ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
@@ -279,232 +272,211 @@
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
-
     def delete_filter(self, *, arn: str) -> DeleteFilterResponseTypeDef:
         """
         Deletes a filter resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.delete_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#delete_filter)
         """
-
     def describe_organization_configuration(
         self,
     ) -> DescribeOrganizationConfigurationResponseTypeDef:
         """
         Describe Amazon Inspector configuration settings for an Amazon Web Services
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.describe_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#describe_organization_configuration)
         """
-
     def disable(
         self,
         *,
         accountIds: Sequence[str] = ...,
         resourceTypes: Sequence[ResourceScanTypeType] = ...
     ) -> DisableResponseTypeDef:
         """
         Disables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable)
         """
-
     def disable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str
     ) -> DisableDelegatedAdminAccountResponseTypeDef:
         """
         Disables the Amazon Inspector delegated administrator for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable_delegated_admin_account)
         """
-
     def disassociate_member(self, *, accountId: str) -> DisassociateMemberResponseTypeDef:
         """
         Disassociates a member account from an Amazon Inspector delegated administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disassociate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disassociate_member)
         """
-
     def enable(
         self,
         *,
         resourceTypes: Sequence[ResourceScanTypeType],
         accountIds: Sequence[str] = ...,
         clientToken: str = ...
     ) -> EnableResponseTypeDef:
         """
         Enables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable)
         """
-
     def enable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str, clientToken: str = ...
     ) -> EnableDelegatedAdminAccountResponseTypeDef:
         """
         Enables the Amazon Inspector delegated administrator for your Organizations
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable_delegated_admin_account)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#generate_presigned_url)
         """
-
     def get_configuration(self) -> GetConfigurationResponseTypeDef:
         """
         Retrieves setting configurations for Inspector scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_configuration)
         """
-
     def get_delegated_admin_account(self) -> GetDelegatedAdminAccountResponseTypeDef:
         """
         Retrieves information about the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_delegated_admin_account)
         """
-
     def get_ec2_deep_inspection_configuration(
         self,
     ) -> GetEc2DeepInspectionConfigurationResponseTypeDef:
         """
         Retrieves the activation status of Amazon Inspector deep inspection and custom
         paths associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_ec2_deep_inspection_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_ec2_deep_inspection_configuration)
         """
-
     def get_encryption_key(
         self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
     ) -> GetEncryptionKeyResponseTypeDef:
         """
         Gets an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_encryption_key)
         """
-
     def get_findings_report_status(
         self, *, reportId: str = ...
     ) -> GetFindingsReportStatusResponseTypeDef:
         """
         Gets the status of a findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_findings_report_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_findings_report_status)
         """
-
     def get_member(self, *, accountId: str) -> GetMemberResponseTypeDef:
         """
         Gets member information for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_member)
         """
-
     def get_sbom_export(self, *, reportId: str) -> GetSbomExportResponseTypeDef:
         """
         Gets details of a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_sbom_export)
         """
-
     def list_account_permissions(
         self, *, maxResults: int = ..., nextToken: str = ..., service: ServiceType = ...
     ) -> ListAccountPermissionsResponseTypeDef:
         """
         Lists the permissions an account has to configure Amazon Inspector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_account_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_account_permissions)
         """
-
     def list_coverage(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for you environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage)
         """
-
     def list_coverage_statistics(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
         nextToken: str = ...
     ) -> ListCoverageStatisticsResponseTypeDef:
         """
         Lists Amazon Inspector coverage statistics for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage_statistics)
         """
-
     def list_delegated_admin_accounts(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDelegatedAdminAccountsResponseTypeDef:
         """
         Lists information about the Amazon Inspector delegated administrator of your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_delegated_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_delegated_admin_accounts)
         """
-
     def list_filters(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFiltersResponseTypeDef:
         """
         Lists the filters associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_filters)
         """
-
     def list_finding_aggregations(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
         maxResults: int = ...,
@@ -512,124 +484,112 @@
     ) -> ListFindingAggregationsResponseTypeDef:
         """
         Lists aggregated finding data for your environment based on specific criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
-
     def list_findings(
         self,
         *,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_findings)
         """
-
     def list_members(
         self, *, maxResults: int = ..., nextToken: str = ..., onlyAssociated: bool = ...
     ) -> ListMembersResponseTypeDef:
         """
         List members associated with the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_members)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags attached to a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_tags_for_resource)
         """
-
     def list_usage_totals(
         self, *, accountIds: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListUsageTotalsResponseTypeDef:
         """
         Lists the Amazon Inspector usage totals over the last 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_usage_totals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_usage_totals)
         """
-
     def reset_encryption_key(
         self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
     ) -> Dict[str, Any]:
         """
         Resets an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.reset_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#reset_encryption_key)
         """
-
     def search_vulnerabilities(
         self, *, filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef, nextToken: str = ...
     ) -> SearchVulnerabilitiesResponseTypeDef:
         """
         Lists Amazon Inspector coverage details for a specific vulnerability.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.search_vulnerabilities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#search_vulnerabilities)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#untag_resource)
         """
-
     def update_configuration(self, *, ecrConfiguration: EcrConfigurationTypeDef) -> Dict[str, Any]:
         """
         Updates setting configurations for your Amazon Inspector account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_configuration)
         """
-
     def update_ec2_deep_inspection_configuration(
         self, *, activateDeepInspection: bool = ..., packagePaths: Sequence[str] = ...
     ) -> UpdateEc2DeepInspectionConfigurationResponseTypeDef:
         """
         Activates, deactivates Amazon Inspector deep inspection, or updates custom paths
         for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_ec2_deep_inspection_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_ec2_deep_inspection_configuration)
         """
-
     def update_encryption_key(
         self, *, kmsKeyId: str, resourceType: ResourceTypeType, scanType: ScanTypeType
     ) -> Dict[str, Any]:
         """
         Updates an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_encryption_key)
         """
-
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
@@ -639,108 +599,96 @@
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_filter)
         """
-
     def update_org_ec2_deep_inspection_configuration(
         self, *, orgPackagePaths: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Updates the Amazon Inspector deep inspection custom paths for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_org_ec2_deep_inspection_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_org_ec2_deep_inspection_configuration)
         """
-
     def update_organization_configuration(
         self, *, autoEnable: AutoEnableTypeDef
     ) -> UpdateOrganizationConfigurationResponseTypeDef:
         """
         Updates the configurations for your Amazon Inspector organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_organization_configuration)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_account_permissions"]
     ) -> ListAccountPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_coverage"]) -> ListCoveragePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_coverage_statistics"]
     ) -> ListCoverageStatisticsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_delegated_admin_accounts"]
     ) -> ListDelegatedAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_filters"]) -> ListFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_finding_aggregations"]
     ) -> ListFindingAggregationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_findings"]) -> ListFindingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_members"]) -> ListMembersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_usage_totals"]
     ) -> ListUsageTotalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["search_vulnerabilities"]
     ) -> SearchVulnerabilitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AutoEnableTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     CancelFindingsReportResponseTypeDef,
     CancelSbomExportResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CreateFilterResponseTypeDef,
@@ -97,34 +98,38 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("Inspector2Client",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class Inspector2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/)
     """
 
     meta: ClientMeta
@@ -133,99 +138,120 @@
     def exceptions(self) -> Exceptions:
         """
         Inspector2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#exceptions)
         """
+
     def associate_member(self, *, accountId: str) -> AssociateMemberResponseTypeDef:
         """
         Associates an Amazon Web Services account with an Amazon Inspector delegated
         administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.associate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#associate_member)
         """
+
     def batch_get_account_status(
         self, *, accountIds: Sequence[str] = ...
     ) -> BatchGetAccountStatusResponseTypeDef:
         """
         Retrieves the Amazon Inspector status of multiple Amazon Web Services accounts
         within your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_account_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_account_status)
         """
+
     def batch_get_code_snippet(
         self, *, findingArns: Sequence[str]
     ) -> BatchGetCodeSnippetResponseTypeDef:
         """
         Retrieves code snippets from findings that Amazon Inspector detected code
         vulnerabilities in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_code_snippet)
         """
+
+    def batch_get_finding_details(
+        self, *, findingArns: Sequence[str]
+    ) -> BatchGetFindingDetailsResponseTypeDef:
+        """
+        Gets vulnerability details for findings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_finding_details)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_finding_details)
+        """
+
     def batch_get_free_trial_info(
         self, *, accountIds: Sequence[str]
     ) -> BatchGetFreeTrialInfoResponseTypeDef:
         """
         Gets free trial status for multiple Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_free_trial_info)
         """
+
     def batch_get_member_ec2_deep_inspection_status(
         self, *, accountIds: Sequence[str] = ...
     ) -> BatchGetMemberEc2DeepInspectionStatusResponseTypeDef:
         """
         Retrieves Amazon Inspector deep inspection activation status of multiple member
         accounts within your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_member_ec2_deep_inspection_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_member_ec2_deep_inspection_status)
         """
+
     def batch_update_member_ec2_deep_inspection_status(
         self, *, accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef]
     ) -> BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef:
         """
         Activates or deactivates Amazon Inspector deep inspection for the provided
         member accounts in your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_update_member_ec2_deep_inspection_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_update_member_ec2_deep_inspection_status)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#can_paginate)
         """
+
     def cancel_findings_report(self, *, reportId: str) -> CancelFindingsReportResponseTypeDef:
         """
         Cancels the given findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_findings_report)
         """
+
     def cancel_sbom_export(self, *, reportId: str) -> CancelSbomExportResponseTypeDef:
         """
         Cancels a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_sbom_export)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
+
     def create_filter(
         self,
         *,
         action: FilterActionType,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef],
         name: str,
         description: str = ...,
@@ -234,27 +260,29 @@
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_filter)
         """
+
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
+
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
         resourceFilterCriteria: Union[
             ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
@@ -262,211 +290,232 @@
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
+
     def delete_filter(self, *, arn: str) -> DeleteFilterResponseTypeDef:
         """
         Deletes a filter resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.delete_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#delete_filter)
         """
+
     def describe_organization_configuration(
         self,
     ) -> DescribeOrganizationConfigurationResponseTypeDef:
         """
         Describe Amazon Inspector configuration settings for an Amazon Web Services
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.describe_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#describe_organization_configuration)
         """
+
     def disable(
         self,
         *,
         accountIds: Sequence[str] = ...,
         resourceTypes: Sequence[ResourceScanTypeType] = ...
     ) -> DisableResponseTypeDef:
         """
         Disables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable)
         """
+
     def disable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str
     ) -> DisableDelegatedAdminAccountResponseTypeDef:
         """
         Disables the Amazon Inspector delegated administrator for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable_delegated_admin_account)
         """
+
     def disassociate_member(self, *, accountId: str) -> DisassociateMemberResponseTypeDef:
         """
         Disassociates a member account from an Amazon Inspector delegated administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disassociate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disassociate_member)
         """
+
     def enable(
         self,
         *,
         resourceTypes: Sequence[ResourceScanTypeType],
         accountIds: Sequence[str] = ...,
         clientToken: str = ...
     ) -> EnableResponseTypeDef:
         """
         Enables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable)
         """
+
     def enable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str, clientToken: str = ...
     ) -> EnableDelegatedAdminAccountResponseTypeDef:
         """
         Enables the Amazon Inspector delegated administrator for your Organizations
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable_delegated_admin_account)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#generate_presigned_url)
         """
+
     def get_configuration(self) -> GetConfigurationResponseTypeDef:
         """
         Retrieves setting configurations for Inspector scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_configuration)
         """
+
     def get_delegated_admin_account(self) -> GetDelegatedAdminAccountResponseTypeDef:
         """
         Retrieves information about the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_delegated_admin_account)
         """
+
     def get_ec2_deep_inspection_configuration(
         self,
     ) -> GetEc2DeepInspectionConfigurationResponseTypeDef:
         """
         Retrieves the activation status of Amazon Inspector deep inspection and custom
         paths associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_ec2_deep_inspection_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_ec2_deep_inspection_configuration)
         """
+
     def get_encryption_key(
         self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
     ) -> GetEncryptionKeyResponseTypeDef:
         """
         Gets an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_encryption_key)
         """
+
     def get_findings_report_status(
         self, *, reportId: str = ...
     ) -> GetFindingsReportStatusResponseTypeDef:
         """
         Gets the status of a findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_findings_report_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_findings_report_status)
         """
+
     def get_member(self, *, accountId: str) -> GetMemberResponseTypeDef:
         """
         Gets member information for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_member)
         """
+
     def get_sbom_export(self, *, reportId: str) -> GetSbomExportResponseTypeDef:
         """
         Gets details of a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_sbom_export)
         """
+
     def list_account_permissions(
         self, *, maxResults: int = ..., nextToken: str = ..., service: ServiceType = ...
     ) -> ListAccountPermissionsResponseTypeDef:
         """
         Lists the permissions an account has to configure Amazon Inspector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_account_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_account_permissions)
         """
+
     def list_coverage(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for you environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage)
         """
+
     def list_coverage_statistics(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
         nextToken: str = ...
     ) -> ListCoverageStatisticsResponseTypeDef:
         """
         Lists Amazon Inspector coverage statistics for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage_statistics)
         """
+
     def list_delegated_admin_accounts(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDelegatedAdminAccountsResponseTypeDef:
         """
         Lists information about the Amazon Inspector delegated administrator of your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_delegated_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_delegated_admin_accounts)
         """
+
     def list_filters(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFiltersResponseTypeDef:
         """
         Lists the filters associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_filters)
         """
+
     def list_finding_aggregations(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
         maxResults: int = ...,
@@ -474,112 +523,124 @@
     ) -> ListFindingAggregationsResponseTypeDef:
         """
         Lists aggregated finding data for your environment based on specific criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
+
     def list_findings(
         self,
         *,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_findings)
         """
+
     def list_members(
         self, *, maxResults: int = ..., nextToken: str = ..., onlyAssociated: bool = ...
     ) -> ListMembersResponseTypeDef:
         """
         List members associated with the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_members)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags attached to a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_tags_for_resource)
         """
+
     def list_usage_totals(
         self, *, accountIds: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListUsageTotalsResponseTypeDef:
         """
         Lists the Amazon Inspector usage totals over the last 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_usage_totals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_usage_totals)
         """
+
     def reset_encryption_key(
         self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
     ) -> Dict[str, Any]:
         """
         Resets an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.reset_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#reset_encryption_key)
         """
+
     def search_vulnerabilities(
         self, *, filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef, nextToken: str = ...
     ) -> SearchVulnerabilitiesResponseTypeDef:
         """
         Lists Amazon Inspector coverage details for a specific vulnerability.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.search_vulnerabilities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#search_vulnerabilities)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#untag_resource)
         """
+
     def update_configuration(self, *, ecrConfiguration: EcrConfigurationTypeDef) -> Dict[str, Any]:
         """
         Updates setting configurations for your Amazon Inspector account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_configuration)
         """
+
     def update_ec2_deep_inspection_configuration(
         self, *, activateDeepInspection: bool = ..., packagePaths: Sequence[str] = ...
     ) -> UpdateEc2DeepInspectionConfigurationResponseTypeDef:
         """
         Activates, deactivates Amazon Inspector deep inspection, or updates custom paths
         for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_ec2_deep_inspection_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_ec2_deep_inspection_configuration)
         """
+
     def update_encryption_key(
         self, *, kmsKeyId: str, resourceType: ResourceTypeType, scanType: ScanTypeType
     ) -> Dict[str, Any]:
         """
         Updates an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_encryption_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_encryption_key)
         """
+
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
         filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
@@ -589,96 +650,108 @@
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_filter)
         """
+
     def update_org_ec2_deep_inspection_configuration(
         self, *, orgPackagePaths: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Updates the Amazon Inspector deep inspection custom paths for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_org_ec2_deep_inspection_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_org_ec2_deep_inspection_configuration)
         """
+
     def update_organization_configuration(
         self, *, autoEnable: AutoEnableTypeDef
     ) -> UpdateOrganizationConfigurationResponseTypeDef:
         """
         Updates the configurations for your Amazon Inspector organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_organization_configuration)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_account_permissions"]
     ) -> ListAccountPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_coverage"]) -> ListCoveragePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_coverage_statistics"]
     ) -> ListCoverageStatisticsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_delegated_admin_accounts"]
     ) -> ListDelegatedAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_filters"]) -> ListFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_finding_aggregations"]
     ) -> ListFindingAggregationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_findings"]) -> ListFindingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_members"]) -> ListMembersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_usage_totals"]
     ) -> ListUsageTotalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["search_vulnerabilities"]
     ) -> SearchVulnerabilitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
     "ExternalReportStatusType",
     "FilterActionType",
+    "FindingDetailsErrorCodeType",
     "FindingStatusType",
     "FindingTypeSortByType",
     "FindingTypeType",
     "FixAvailableType",
     "FreeTrialInfoErrorCodeType",
     "FreeTrialStatusType",
     "FreeTrialTypeType",
@@ -154,14 +155,17 @@
     "SSM_THROTTLED",
     "SSM_UNAVAILABLE",
     "SUSPEND_IN_PROGRESS",
 ]
 ExploitAvailableType = Literal["NO", "YES"]
 ExternalReportStatusType = Literal["CANCELLED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 FilterActionType = Literal["NONE", "SUPPRESS"]
+FindingDetailsErrorCodeType = Literal[
+    "ACCESS_DENIED", "FINDING_DETAILS_NOT_FOUND", "INTERNAL_ERROR", "INVALID_INPUT"
+]
 FindingStatusType = Literal["ACTIVE", "CLOSED", "SUPPRESSED"]
 FindingTypeSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 FindingTypeType = Literal["CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 FixAvailableType = Literal["NO", "PARTIAL", "YES"]
 FreeTrialInfoErrorCodeType = Literal["ACCESS_DENIED", "INTERNAL_ERROR"]
 FreeTrialStatusType = Literal["ACTIVE", "INACTIVE"]
 FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
     "ExternalReportStatusType",
     "FilterActionType",
+    "FindingDetailsErrorCodeType",
     "FindingStatusType",
     "FindingTypeSortByType",
     "FindingTypeType",
     "FixAvailableType",
     "FreeTrialInfoErrorCodeType",
     "FreeTrialStatusType",
     "FreeTrialTypeType",
@@ -152,14 +153,17 @@
     "SSM_THROTTLED",
     "SSM_UNAVAILABLE",
     "SUSPEND_IN_PROGRESS",
 ]
 ExploitAvailableType = Literal["NO", "YES"]
 ExternalReportStatusType = Literal["CANCELLED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 FilterActionType = Literal["NONE", "SUPPRESS"]
+FindingDetailsErrorCodeType = Literal[
+    "ACCESS_DENIED", "FINDING_DETAILS_NOT_FOUND", "INTERNAL_ERROR", "INVALID_INPUT"
+]
 FindingStatusType = Literal["ACTIVE", "CLOSED", "SUPPRESSED"]
 FindingTypeSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 FindingTypeType = Literal["CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 FixAvailableType = Literal["NO", "PARTIAL", "YES"]
 FreeTrialInfoErrorCodeType = Literal["ACCESS_DENIED", "INTERNAL_ERROR"]
 FreeTrialStatusType = Literal["ACTIVE", "INACTIVE"]
 FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -98,14 +99,16 @@
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    "FindingDetailsErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
@@ -138,14 +141,15 @@
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
+    "EvidenceTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
@@ -226,14 +230,15 @@
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
+    "FindingDetailTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
@@ -259,14 +264,15 @@
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
+    "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
     "GetSbomExportResponseTypeDef",
@@ -485,14 +491,30 @@
     {
         "errorCode": CodeSnippetErrorCodeType,
         "errorMessage": str,
         "findingArn": str,
     },
 )
 
+BatchGetFindingDetailsRequestRequestTypeDef = TypedDict(
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    {
+        "findingArns": Sequence[str],
+    },
+)
+
+FindingDetailsErrorTypeDef = TypedDict(
+    "FindingDetailsErrorTypeDef",
+    {
+        "errorCode": FindingDetailsErrorCodeType,
+        "errorMessage": str,
+        "findingArn": str,
+    },
+)
+
 BatchGetFreeTrialInfoRequestRequestTypeDef = TypedDict(
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 
@@ -916,14 +938,24 @@
     "EpssTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
+EvidenceTypeDef = TypedDict(
+    "EvidenceTypeDef",
+    {
+        "evidenceDetail": str,
+        "evidenceRule": str,
+        "severity": str,
+    },
+    total=False,
+)
+
 ExploitObservedTypeDef = TypedDict(
     "ExploitObservedTypeDef",
     {
         "firstSeen": datetime,
         "lastSeen": datetime,
     },
     total=False,
@@ -1972,14 +2004,31 @@
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
 )
 
+FindingDetailTypeDef = TypedDict(
+    "FindingDetailTypeDef",
+    {
+        "cisaData": CisaDataTypeDef,
+        "cwes": List[str],
+        "epssScore": float,
+        "evidences": List[EvidenceTypeDef],
+        "exploitObserved": ExploitObservedTypeDef,
+        "findingArn": str,
+        "referenceUrls": List[str],
+        "riskScore": int,
+        "tools": List[str],
+        "ttps": List[str],
+    },
+    total=False,
+)
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -2375,14 +2424,23 @@
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchGetFindingDetailsResponseTypeDef = TypedDict(
+    "BatchGetFindingDetailsResponseTypeDef",
+    {
+        "errors": List[FindingDetailsErrorTypeDef],
+        "findingDetails": List[FindingDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SearchVulnerabilitiesResponseTypeDef = TypedDict(
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -97,14 +98,16 @@
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    "FindingDetailsErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
@@ -137,14 +140,15 @@
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
+    "EvidenceTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
@@ -225,14 +229,15 @@
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
+    "FindingDetailTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
@@ -258,14 +263,15 @@
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
+    "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
     "GetSbomExportResponseTypeDef",
@@ -478,14 +484,30 @@
     {
         "errorCode": CodeSnippetErrorCodeType,
         "errorMessage": str,
         "findingArn": str,
     },
 )
 
+BatchGetFindingDetailsRequestRequestTypeDef = TypedDict(
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    {
+        "findingArns": Sequence[str],
+    },
+)
+
+FindingDetailsErrorTypeDef = TypedDict(
+    "FindingDetailsErrorTypeDef",
+    {
+        "errorCode": FindingDetailsErrorCodeType,
+        "errorMessage": str,
+        "findingArn": str,
+    },
+)
+
 BatchGetFreeTrialInfoRequestRequestTypeDef = TypedDict(
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 
@@ -895,14 +917,24 @@
     "EpssTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
+EvidenceTypeDef = TypedDict(
+    "EvidenceTypeDef",
+    {
+        "evidenceDetail": str,
+        "evidenceRule": str,
+        "severity": str,
+    },
+    total=False,
+)
+
 ExploitObservedTypeDef = TypedDict(
     "ExploitObservedTypeDef",
     {
         "firstSeen": datetime,
         "lastSeen": datetime,
     },
     total=False,
@@ -1919,14 +1951,31 @@
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
 )
 
+FindingDetailTypeDef = TypedDict(
+    "FindingDetailTypeDef",
+    {
+        "cisaData": CisaDataTypeDef,
+        "cwes": List[str],
+        "epssScore": float,
+        "evidences": List[EvidenceTypeDef],
+        "exploitObserved": ExploitObservedTypeDef,
+        "findingArn": str,
+        "referenceUrls": List[str],
+        "riskScore": int,
+        "tools": List[str],
+        "ttps": List[str],
+    },
+    total=False,
+)
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -2314,14 +2363,23 @@
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchGetFindingDetailsResponseTypeDef = TypedDict(
+    "BatchGetFindingDetailsResponseTypeDef",
+    {
+        "errors": List[FindingDetailsErrorTypeDef],
+        "findingDetails": List[FindingDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SearchVulnerabilitiesResponseTypeDef = TypedDict(
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -349,14 +349,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -435,14 +436,16 @@
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
+    BatchGetFindingDetailsRequestRequestTypeDef,
+    FindingDetailsErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
@@ -475,14 +478,15 @@
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
+    EvidenceTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
@@ -563,14 +567,15 @@
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
+    FindingDetailTypeDef,
     VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
     ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
@@ -596,14 +601,15 @@
     ListCoverageRequestListCoveragePaginateTypeDef,
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
     GetSbomExportResponseTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15.post1/setup.py` & `mypy-boto3-inspector2-1.28.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder"
         " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

