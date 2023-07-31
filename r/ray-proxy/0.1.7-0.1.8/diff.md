# Comparing `tmp/ray_proxy-0.1.7.tar.gz` & `tmp/ray_proxy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ray_proxy-0.1.7.tar", max compression
+gzip compressed data, was "ray_proxy-0.1.8.tar", max compression
```

## Comparing `ray_proxy-0.1.7.tar` & `ray_proxy-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 ray_proxy-0.1.7/LICENSE
--rw-r--r--   0        0        0      537 2023-05-30 06:13:53.441052 ray_proxy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      114 2022-10-01 08:27:27.000000 ray_proxy-0.1.7/ray_proxy/__init__.py
--rw-r--r--   0        0        0    13299 2022-10-18 04:07:37.000000 ray_proxy-0.1.7/ray_proxy/async_interpreter.py
--rw-r--r--   0        0        0     8367 2023-05-30 06:13:37.245007 ray_proxy-0.1.7/ray_proxy/cluster_resource.py
--rw-r--r--   0        0        0    16420 2022-10-18 12:38:00.000000 ray_proxy-0.1.7/ray_proxy/cluster_task_scheduler.py
--rw-r--r--   0        0        0     2838 2022-10-19 02:45:28.000000 ray_proxy-0.1.7/ray_proxy/injected_resource.py
--rw-r--r--   0        0        0     5025 2022-10-25 10:32:32.000000 ray_proxy-0.1.7/ray_proxy/interface.py
--rw-r--r--   0        0        0     2398 2023-05-30 06:13:37.245690 ray_proxy-0.1.7/ray_proxy/local_var.py
--rw-r--r--   0        0        0      272 2022-10-18 04:07:37.000000 ray_proxy-0.1.7/ray_proxy/prepared.py
--rw-r--r--   0        0        0    11689 2023-05-30 06:13:37.246538 ray_proxy-0.1.7/ray_proxy/py_environment.py
--rw-r--r--   0        0        0      746 2022-08-26 04:22:55.000000 ray_proxy-0.1.7/ray_proxy/ray_queue.py
--rw-r--r--   0        0        0     1107 2022-10-24 06:03:35.000000 ray_proxy-0.1.7/ray_proxy/releasable.py
--rw-r--r--   0        0        0     8706 2022-10-25 10:32:32.000000 ray_proxy-0.1.7/ray_proxy/remote_env.py
--rw-r--r--   0        0        0     2461 2022-10-01 06:48:59.000000 ray_proxy-0.1.7/ray_proxy/remote_prog_bar.py
--rw-r--r--   0        0        0    11617 2023-05-30 06:13:37.247177 ray_proxy-0.1.7/ray_proxy/remote_proxy.py
--rw-r--r--   0        0        0     4891 2023-05-30 06:13:37.247571 ray_proxy-0.1.7/ray_proxy/resource_design.py
--rw-r--r--   0        0        0    15326 2023-05-30 06:13:37.248223 ray_proxy-0.1.7/ray_proxy/resource_scheduler.py
--rw-r--r--   0        0        0     9108 2023-05-30 06:13:37.248746 ray_proxy-0.1.7/ray_proxy/resource_scheduler_client.py
--rw-r--r--   0        0        0     1170 2022-10-06 07:02:24.000000 ray_proxy-0.1.7/ray_proxy/serialization_check.py
--rw-r--r--   0        0        0      222 2022-10-24 06:03:35.000000 ray_proxy-0.1.7/ray_proxy/type_aliases.py
--rw-r--r--   0        0        0      239 2022-10-18 04:07:37.000000 ray_proxy-0.1.7/ray_proxy/util.py
--rw-r--r--   0        0        0     2696 2022-11-19 11:26:29.000000 ray_proxy-0.1.7/ray_proxy/var_interface.py
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 ray_proxy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 ray_proxy-0.1.8/LICENSE
+-rw-r--r--   0        0        0      537 2023-07-31 04:12:19.668327 ray_proxy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      114 2022-10-01 08:27:27.000000 ray_proxy-0.1.8/ray_proxy/__init__.py
+-rw-r--r--   0        0        0    13299 2022-10-18 04:07:37.000000 ray_proxy-0.1.8/ray_proxy/async_interpreter.py
+-rw-r--r--   0        0        0     8370 2023-07-19 15:55:45.068289 ray_proxy-0.1.8/ray_proxy/cluster_resource.py
+-rw-r--r--   0        0        0    16420 2022-10-18 12:38:00.000000 ray_proxy-0.1.8/ray_proxy/cluster_task_scheduler.py
+-rw-r--r--   0        0        0     2854 2023-07-28 06:53:51.201820 ray_proxy-0.1.8/ray_proxy/injected_resource.py
+-rw-r--r--   0        0        0     5025 2022-10-25 10:32:32.000000 ray_proxy-0.1.8/ray_proxy/interface.py
+-rw-r--r--   0        0        0     2398 2023-05-30 06:13:37.245690 ray_proxy-0.1.8/ray_proxy/local_var.py
+-rw-r--r--   0        0        0      272 2022-10-18 04:07:37.000000 ray_proxy-0.1.8/ray_proxy/prepared.py
+-rw-r--r--   0        0        0    11689 2023-05-30 06:13:37.246538 ray_proxy-0.1.8/ray_proxy/py_environment.py
+-rw-r--r--   0        0        0      746 2022-08-26 04:22:55.000000 ray_proxy-0.1.8/ray_proxy/ray_queue.py
+-rw-r--r--   0        0        0     1107 2022-10-24 06:03:35.000000 ray_proxy-0.1.8/ray_proxy/releasable.py
+-rw-r--r--   0        0        0     8706 2022-10-25 10:32:32.000000 ray_proxy-0.1.8/ray_proxy/remote_env.py
+-rw-r--r--   0        0        0     2461 2022-10-01 06:48:59.000000 ray_proxy-0.1.8/ray_proxy/remote_prog_bar.py
+-rw-r--r--   0        0        0    11617 2023-05-30 06:13:37.247177 ray_proxy-0.1.8/ray_proxy/remote_proxy.py
+-rw-r--r--   0        0        0     4832 2023-07-13 02:04:05.014307 ray_proxy-0.1.8/ray_proxy/resource_design.py
+-rw-r--r--   0        0        0    15326 2023-05-30 06:13:37.248223 ray_proxy-0.1.8/ray_proxy/resource_scheduler.py
+-rw-r--r--   0        0        0     9108 2023-05-30 06:13:37.248746 ray_proxy-0.1.8/ray_proxy/resource_scheduler_client.py
+-rw-r--r--   0        0        0     1170 2022-10-06 07:02:24.000000 ray_proxy-0.1.8/ray_proxy/serialization_check.py
+-rw-r--r--   0        0        0      222 2022-10-24 06:03:35.000000 ray_proxy-0.1.8/ray_proxy/type_aliases.py
+-rw-r--r--   0        0        0      239 2022-10-18 04:07:37.000000 ray_proxy-0.1.8/ray_proxy/util.py
+-rw-r--r--   0        0        0     2696 2022-11-19 11:26:29.000000 ray_proxy-0.1.8/ray_proxy/var_interface.py
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 ray_proxy-0.1.8/PKG-INFO
```

### Comparing `ray_proxy-0.1.7/LICENSE` & `ray_proxy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/pyproject.toml` & `ray_proxy-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ray-proxy"
-version = "0.1.7"
+version = "0.1.8"
 description = "A library which enables the creation of proxy variables for remote python interpreter in ray cluster."
 authors = ["proboscis <nameissoap@gmail.com>"]
 packages = [{ include = "ray_proxy" }]
 license = "MIT"
 [tool.poetry.dependencies]
 python = "^3.7"
 ray = "^2.0.0"
```

### Comparing `ray_proxy-0.1.7/ray_proxy/async_interpreter.py` & `ray_proxy-0.1.8/ray_proxy/async_interpreter.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/cluster_resource.py` & `ray_proxy-0.1.8/ray_proxy/cluster_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     @property
     def required_resources(self) -> Dict[str, int]:
         return self._required_resources
 
     def run(self, resources: Resources) -> Awaitable:
         print(f"calling lambda cluster task:{resources},{self.args},{self.kwargs}")
         values = {k: [item.value for item in v] for k, v in resources.items()}
-        from archpainter.picklability_checker import assert_picklable
+        from injected_utils.picklability_checker import assert_picklable
         assert_picklable(
             dict(func=self.f, values=values)
         )
         remote_f = ray.remote(self.f).options(**self.ray_options)
         # print(f"created task:{remote_f}")
         res = remote_f.remote(values, *self.args, **self.kwargs)
         # print(f"ray task is submitted as :{res}")
```

### Comparing `ray_proxy-0.1.7/ray_proxy/cluster_task_scheduler.py` & `ray_proxy-0.1.8/ray_proxy/cluster_task_scheduler.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/injected_resource.py` & `ray_proxy-0.1.8/ray_proxy/injected_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field, replace
 from typing import Generic, Union, Optional, Callable, Awaitable, TypeVar
 
 from pinject_design import Injected
 from pinject_design.di.applicative import Applicative
 from pinject_design.di.proxiable import DelegatedVar
-from pinject_design.di.static_proxy import AstProxyContextImpl, eval_app
+from pinject_design.di.static_proxy import AstProxyContextImpl, eval_applicative
 from ray_proxy.cluster_resource import ResourceScope, Resources
 from ray_proxy.util import run_injected
 
 T = TypeVar("T")
 @dataclass
 class InjectedResource(Generic[T]):
     factory: Injected
@@ -68,9 +68,9 @@
 
     def is_instance(self, item) -> bool:
         return isinstance(item, InjectedResource)
 
 
 INJECTED_RESOURCE_APPLICATIVE = InjectedResourceApplicative()
 INJECTED_RESOURCE_EVAL_CONTEXT = AstProxyContextImpl(
-    lambda expr: eval_app(expr, INJECTED_RESOURCE_APPLICATIVE),
+    lambda expr: eval_applicative(expr, INJECTED_RESOURCE_APPLICATIVE),
 )
```

### Comparing `ray_proxy-0.1.7/ray_proxy/interface.py` & `ray_proxy-0.1.8/ray_proxy/interface.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/local_var.py` & `ray_proxy-0.1.8/ray_proxy/local_var.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/py_environment.py` & `ray_proxy-0.1.8/ray_proxy/py_environment.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/ray_queue.py` & `ray_proxy-0.1.8/ray_proxy/ray_queue.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/releasable.py` & `ray_proxy-0.1.8/ray_proxy/releasable.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/remote_env.py` & `ray_proxy-0.1.8/ray_proxy/remote_env.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/remote_prog_bar.py` & `ray_proxy-0.1.8/ray_proxy/remote_prog_bar.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/remote_proxy.py` & `ray_proxy-0.1.8/ray_proxy/remote_proxy.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/resource_design.py` & `ray_proxy-0.1.8/ray_proxy/resource_design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from dataclasses import dataclass, field, replace
 from typing import Dict, Union, TypeVar
 
 import frozendict
 from bidict import bidict
-from diffusers.configuration_utils import FrozenDict
 
 from pinject_design import Injected
 from pinject_design.di.app_injected import EvaledInjected
 from pinject_design.di.injected import MappedInjected, InjectedFunction, ZippedInjected, MZippedInjected, InjectedPure, \
     InjectedByName
 from ray_proxy.cluster_resource import ResourceScope
 from ray_proxy.injected_resource import InjectedResource
 
 T = TypeVar("T")
 
 
 @dataclass
 class ResourcePrioritizer:
-    targets: Dict[FrozenDict[str, int], int] = field(default_factory=dict)
+    targets: Dict[Dict[str, int], int] = field(default_factory=dict)
 
     def __call__(self, req: Dict[str, int]):
         q = frozendict.frozendict(req)
         return self.targets.get(q, 0)
 
     def add_priority(self, q: Dict[str, int], priority: int):
         targets = {frozendict.frozendict(q): priority}
```

### Comparing `ray_proxy-0.1.7/ray_proxy/resource_scheduler.py` & `ray_proxy-0.1.8/ray_proxy/resource_scheduler.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/resource_scheduler_client.py` & `ray_proxy-0.1.8/ray_proxy/resource_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/serialization_check.py` & `ray_proxy-0.1.8/ray_proxy/serialization_check.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/ray_proxy/var_interface.py` & `ray_proxy-0.1.8/ray_proxy/var_interface.py`

 * *Files identical despite different names*

### Comparing `ray_proxy-0.1.7/PKG-INFO` & `ray_proxy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ray-proxy
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library which enables the creation of proxy variables for remote python interpreter in ray cluster.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

