# Comparing `tmp/cloudshell-orch-core-4.2.0.263.tar.gz` & `tmp/cloudshell-orch-core-4.3.0.282.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudshell-orch-core-4.2.0.263.tar", last modified: Mon Sep 19 08:54:07 2022, max compression
+gzip compressed data, was "dist\cloudshell-orch-core-4.3.0.282.tar", last modified: Mon Jul 31 12:22:36 2023, max compression
```

## Comparing `cloudshell-orch-core-4.2.0.263.tar` & `cloudshell-orch-core-4.3.0.282.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/helpers/
--rw-rw-rw-   0        0        0     2620 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/helpers/resource_helpers.py
--rw-rw-rw-   0        0        0     8596 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/helpers/sandbox_helpers.py
--rw-rw-rw-   0        0        0      102 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/
--rw-rw-rw-   0        0        0     1496 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/app.py
--rw-rw-rw-   0        0        0     3831 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/apps_configuration.py
--rw-rw-rw-   0        0        0     3304 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/components.py
--rw-rw-rw-   0        0        0    11021 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/sandbox.py
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/setup/
--rw-rw-rw-   0        0        0    28315 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/setup/default_setup_logic.py
--rw-rw-rw-   0        0        0     5303 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/setup/default_setup_orchestrator.py
--rw-rw-rw-   0        0        0       97 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/teardown/
--rw-rw-rw-   0        0        0     8487 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/teardown/default_teardown_logic.py
--rw-rw-rw-   0        0        0     1924 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/teardown/default_teardown_orchestrator.py
--rw-rw-rw-   0        0        0       99 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/teardown/__init__.py
--rw-rw-rw-   0        0        0     6032 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/workflow.py
--rw-rw-rw-   0        0        0       97 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/profiler/
--rw-rw-rw-   0        0        0     1207 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/profiler/env_profiler.py
--rw-rw-rw-   0        0        0      102 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/profiler/__init__.py
--rw-rw-rw-   0        0        0       97 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/workflow/__init__.py
--rw-rw-rw-   0        0        0       97 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/
--rw-rw-rw-   0        0        0        1 2022-09-19 08:54:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      538 2022-09-19 08:54:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      106 2022-09-19 08:54:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1273 2022-09-19 08:54:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2022-09-19 08:54:06.000000 cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       49 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/MANIFEST.in
--rw-rw-rw-   0        0        0      538 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/PKG-INFO
--rw-rw-rw-   0        0        0      109 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/setup.cfg
--rw-rw-rw-   0        0        0     1258 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-19 08:54:07.000000 cloudshell-orch-core-4.2.0.263/tests/
--rw-rw-rw-   0        0        0     2178 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/tests/test_sandbox.py
--rw-rw-rw-   0        0        0       75 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/tests/__init__.py
--rw-rw-rw-   0        0        0        4 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/test_requirements.txt
--rw-rw-rw-   0        0        0       12 2022-08-31 12:57:06.000000 cloudshell-orch-core-4.2.0.263/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/helpers/
+-rw-rw-rw-   0        0        0     2620 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/helpers/resource_helpers.py
+-rw-rw-rw-   0        0        0     8711 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/helpers/sandbox_helpers.py
+-rw-rw-rw-   0        0        0      102 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/
+-rw-rw-rw-   0        0        0     1496 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/app.py
+-rw-rw-rw-   0        0        0     3831 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/apps_configuration.py
+-rw-rw-rw-   0        0        0     3304 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/components.py
+-rw-rw-rw-   0        0        0    11021 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/sandbox.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/setup/
+-rw-rw-rw-   0        0        0    28315 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/setup/default_setup_logic.py
+-rw-rw-rw-   0        0        0     5303 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/setup/default_setup_orchestrator.py
+-rw-rw-rw-   0        0        0       97 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/teardown/
+-rw-rw-rw-   0        0        0     8487 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/teardown/default_teardown_logic.py
+-rw-rw-rw-   0        0        0     1924 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/teardown/default_teardown_orchestrator.py
+-rw-rw-rw-   0        0        0       99 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/teardown/__init__.py
+-rw-rw-rw-   0        0        0     6214 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/workflow.py
+-rw-rw-rw-   0        0        0       97 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/profiler/
+-rw-rw-rw-   0        0        0     1207 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/profiler/env_profiler.py
+-rw-rw-rw-   0        0        0      102 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/profiler/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/workflow/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/cloudshell/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:22:35.000000 cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      538 2023-07-31 12:22:35.000000 cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2023-07-31 12:22:35.000000 cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1302 2023-07-31 12:22:35.000000 cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 12:22:35.000000 cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/MANIFEST.in
+-rw-rw-rw-   0        0        0      538 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:22:36.000000 cloudshell-orch-core-4.3.0.282/tests/
+-rw-rw-rw-   0        0        0      884 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/tests/test_py3_type_hints.py
+-rw-rw-rw-   0        0        0     2178 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/tests/test_sandbox.py
+-rw-rw-rw-   0        0        0       75 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/tests/__init__.py
+-rw-rw-rw-   0        0        0        4 2023-07-31 11:33:22.000000 cloudshell-orch-core-4.3.0.282/test_requirements.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 11:33:24.000000 cloudshell-orch-core-4.3.0.282/version.txt
```

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/helpers/resource_helpers.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/helpers/resource_helpers.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/helpers/sandbox_helpers.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/helpers/sandbox_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import json
-
+import sys
 
 def get_reservation_context_details_dict():
     """
     Get the reservation details dictionary for this execution
     These details are automatically passed to the driver by CloudShell
     :rtype: dict[str,str]
     """
@@ -134,25 +134,27 @@
         """:type : dict[str, dict[str, ResourceInputData]]"""
 
     def __getitem__(self, resource_name):
         """:rtype: dict[str, dict[str, ResourceInputData]]"""
         return self._dictionary[resource_name]
 
     def __setitem__(self, resource_name, resource_input_data):
-        if resource_name not in self._dictionary.keys():
+        if resource_name not in list(self._dictionary.keys()):
             self._dictionary[resource_name] = {}
         self._dictionary[resource_name][resource_input_data.param_name] \
             = resource_input_data
 
-    def __iter__(self):
-        return self._dictionary.iteritems()
-
     def iteritems(self):
         return self.__iter__()
 
+    def __iter__(self):
+        if sys.version_info[0] < 3:
+            return self._dictionary.iteritems()
+        else:
+            return self._dictionary.items()
 
 class ReservationLifecycleContext:
     def __init__(self, reservation_id, saved_sandbox_name, saved_sandbox_description, currentUserName):
         self.reservation_id = reservation_id
         """:type : str"""
         self.saved_sandbox_name = saved_sandbox_name
         """:type : str"""
```

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/app.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/app.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/apps_configuration.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/apps_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/components.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/components.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/sandbox.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/sandbox.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/setup/default_setup_logic.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/setup/default_setup_logic.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/setup/default_setup_orchestrator.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/setup/default_setup_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/teardown/default_teardown_logic.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/teardown/default_teardown_logic.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/teardown/default_teardown_orchestrator.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/teardown/default_teardown_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/orchestration/workflow.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/orchestration/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import sys
 
 
 class WorkflowObject(object):
     def __init__(self, function, components):
         self.function = function
         self.components = components
 
@@ -127,15 +128,19 @@
         :param function:
         :param components: list of components: App, ReservedResourceInfo or ServiceInstance
         """
         self._validate_function(function)
         self._before_teardown.append(WorkflowObject(function=function, components=components))
 
     def _validate_function(self, func):
-        args = inspect.getargspec(func).args
+        # PY3 type hints support for workflow functions
+        if sys.version_info >= (3, 0):
+            args = inspect.getfullargspec(func).args
+        else:
+            args = inspect.getargspec(func).args
         self.sandbox.logger.info(
             'Validating custom function "{0}": {1}. '.format(func.__name__, args))
         if len(args) < 2:
             self.sandbox.automation_api.WriteMessageToReservationOutput(reservationId=self.sandbox.id,
                                                                         message='Sandbox orchestration workflow processes "{0}" should have 2 parameters (sandbox and components), see documentation for more information.'.format(
                                                                             func.__name__))
             raise Exception("Sandbox is Active with Errors")
```

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell/workflow/profiler/env_profiler.py` & `cloudshell-orch-core-4.3.0.282/cloudshell/workflow/profiler/env_profiler.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/PKG-INFO` & `cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudshell-orch-core
-Version: 4.2.0.263
+Version: 4.3.0.282
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Quali
 Author-email: support@qualisystems.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: sandbox cloud cloudshell
```

### Comparing `cloudshell-orch-core-4.2.0.263/cloudshell_orch_core.egg-info/SOURCES.txt` & `cloudshell-orch-core-4.3.0.282/cloudshell_orch_core.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 cloudshell/workflow/profiler/env_profiler.py
 cloudshell_orch_core.egg-info/PKG-INFO
 cloudshell_orch_core.egg-info/SOURCES.txt
 cloudshell_orch_core.egg-info/dependency_links.txt
 cloudshell_orch_core.egg-info/requires.txt
 cloudshell_orch_core.egg-info/top_level.txt
 tests/__init__.py
+tests/test_py3_type_hints.py
 tests/test_sandbox.py
```

### Comparing `cloudshell-orch-core-4.2.0.263/PKG-INFO` & `cloudshell-orch-core-4.3.0.282/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudshell-orch-core
-Version: 4.2.0.263
+Version: 4.3.0.282
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Quali
 Author-email: support@qualisystems.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: sandbox cloud cloudshell
```

### Comparing `cloudshell-orch-core-4.2.0.263/setup.py` & `cloudshell-orch-core-4.3.0.282/setup.py`

 * *Files identical despite different names*

### Comparing `cloudshell-orch-core-4.2.0.263/tests/test_sandbox.py` & `cloudshell-orch-core-4.3.0.282/tests/test_sandbox.py`

 * *Files identical despite different names*

