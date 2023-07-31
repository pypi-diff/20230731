# Comparing `tmp/mypy-boto3-scheduler-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-scheduler-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-scheduler-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:08 2023, max compression
+gzip compressed data, was "mypy-boto3-scheduler-1.28.16.tar", last modified: Mon Jul 31 19:32:48 2023, max compression
```

## Comparing `mypy-boto3-scheduler-1.28.15.post1.tar` & `mypy-boto3-scheduler-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-31 19:32:37.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-07-31 19:32:37.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-31 19:32:37.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-31 19:32:48.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/setup.py
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/LICENSE` & `mypy-boto3-scheduler-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15.post1/PKG-INFO` & `mypy-boto3-scheduler-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-scheduler)](https://pepy.tech/project/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -300,14 +300,15 @@
 ### Literals
 
 `mypy_boto3_scheduler.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_scheduler.literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     ListScheduleGroupsPaginatorName,
     ListSchedulesPaginatorName,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
@@ -318,15 +319,15 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AssignPublicIpType) -> bool:
+def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/README.md` & `mypy-boto3-scheduler-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-scheduler)](https://pepy.tech/project/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -268,14 +268,15 @@
 ### Literals
 
 `mypy_boto3_scheduler.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_scheduler.literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     ListScheduleGroupsPaginatorName,
     ListSchedulesPaginatorName,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
@@ -286,15 +287,15 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AssignPublicIpType) -> bool:
+def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.py` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.pyi` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__main__.py` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgeScheduler 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EventBridgeScheduler 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.py` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ScheduleStateType
+from .literals import ActionAfterCompletionType, ScheduleStateType
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 from .type_defs import (
     CreateScheduleGroupOutputTypeDef,
     CreateScheduleOutputTypeDef,
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
@@ -99,14 +99,15 @@
     def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
         Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
@@ -232,14 +233,15 @@
     def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
         Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.pyi` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ScheduleStateType
+from .literals import ActionAfterCompletionType, ScheduleStateType
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 from .type_defs import (
     CreateScheduleGroupOutputTypeDef,
     CreateScheduleOutputTypeDef,
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
@@ -92,14 +92,15 @@
     def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
         Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
@@ -213,14 +214,15 @@
     def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
         Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.py` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for scheduler service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_scheduler.literals import AssignPublicIpType
+    from mypy_boto3_scheduler.literals import ActionAfterCompletionType
 
-    data: AssignPublicIpType = "DISABLED"
+    data: ActionAfterCompletionType = "DELETE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ActionAfterCompletionType",
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
     "PlacementConstraintTypeType",
     "PlacementStrategyTypeType",
@@ -34,14 +35,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+ActionAfterCompletionType = Literal["DELETE", "NONE"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
 PlacementStrategyTypeType = Literal["binpack", "random", "spread"]
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.pyi` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 Type annotations for scheduler service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_scheduler.literals import AssignPublicIpType
+    from mypy_boto3_scheduler.literals import ActionAfterCompletionType
 
-    data: AssignPublicIpType = "DISABLED"
+    data: ActionAfterCompletionType = "DELETE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ActionAfterCompletionType",
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
     "PlacementConstraintTypeType",
     "PlacementStrategyTypeType",
@@ -32,14 +33,15 @@
     "EventBridgeSchedulerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+ActionAfterCompletionType = Literal["DELETE", "NONE"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
 PlacementStrategyTypeType = Literal["binpack", "random", "spread"]
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.py` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.pyi` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.py` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
     ScheduleGroupStateType,
     ScheduleStateType,
@@ -670,14 +671,15 @@
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
 
 GetScheduleOutputTypeDef = TypedDict(
     "GetScheduleOutputTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "Arn": str,
         "CreationDate": datetime,
         "Description": str,
         "EndDate": datetime,
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
@@ -700,14 +702,15 @@
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalCreateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalCreateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": Union[datetime, str],
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
@@ -731,14 +734,15 @@
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalUpdateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": Union[datetime, str],
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.pyi` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
     ScheduleGroupStateType,
     ScheduleStateType,
@@ -645,14 +646,15 @@
 
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
 GetScheduleOutputTypeDef = TypedDict(
     "GetScheduleOutputTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "Arn": str,
         "CreationDate": datetime,
         "Description": str,
         "EndDate": datetime,
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
@@ -675,14 +677,15 @@
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalCreateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalCreateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": Union[datetime, str],
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
@@ -704,14 +707,15 @@
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalUpdateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": Union[datetime, str],
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/PKG-INFO` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-scheduler)](https://pepy.tech/project/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -300,14 +300,15 @@
 ### Literals
 
 `mypy_boto3_scheduler.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_scheduler.literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     ListScheduleGroupsPaginatorName,
     ListSchedulesPaginatorName,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
@@ -318,15 +319,15 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AssignPublicIpType) -> bool:
+def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
```

### Comparing `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/SOURCES.txt` & `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15.post1/setup.py` & `mypy-boto3-scheduler-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-scheduler",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with"
+        "Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with"
         " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

