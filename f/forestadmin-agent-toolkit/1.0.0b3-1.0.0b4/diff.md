# Comparing `tmp/forestadmin_agent_toolkit-1.0.0b3.tar.gz` & `tmp/forestadmin_agent_toolkit-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b3.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b4.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.0.0b3.tar` & `forestadmin_agent_toolkit-1.0.0b4.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/README.md
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     4908 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0      628 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2292 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     6127 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0      913 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1708 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    15947 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    19417 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     2966 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    11045 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5624 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0     9466 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      144 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     3763 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0     8403 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0      264 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     1660 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0     9523 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3227 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     2266 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1392 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3039 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4308 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2236 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     4508 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0     2288 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     7847 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     3057 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     4019 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1683 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0      541 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1771 2023-07-27 12:29:17.163636 forestadmin_agent_toolkit-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     5450 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0      856 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2292 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     6127 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0      913 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1708 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    15947 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    19417 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     2966 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    11045 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5624 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0     9466 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     3763 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0     8403 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0      264 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     1660 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0     9523 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3227 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     2266 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1392 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3039 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4367 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2236 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     4508 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0     2288 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     7847 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     3057 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     4265 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1683 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0      541 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1771 2023-07-31 15:38:05.659583 forestadmin_agent_toolkit-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b4/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.options import DEFAULT_OPTIONS, Options
 from forestadmin.agent_toolkit.resources.actions.resources import ActionResource
 from forestadmin.agent_toolkit.resources.collections import BoundCollection
 from forestadmin.agent_toolkit.resources.collections.charts_collection import ChartsCollectionResource
 from forestadmin.agent_toolkit.resources.collections.charts_datasource import ChartsDatasourceResource
 from forestadmin.agent_toolkit.resources.collections.crud import CrudResource
 from forestadmin.agent_toolkit.resources.collections.crud_related import CrudRelatedResource
@@ -42,21 +43,22 @@
     META: AgentMeta = None
 
     def __init__(self, options: Options):
         self.options = copy.copy(DEFAULT_OPTIONS)
         self.options.update({k: v for k, v in options.items() if v is not None})
         self.customizer: DatasourceCustomizer = DatasourceCustomizer()
         self._resources = None
+        ForestLogger.setup_logger(self.options["logger_level"], self.options["logger"])
 
         self._permission_service = PermissionService(
             {
                 "env_secret": self.options["env_secret"],
                 "forest_server_url": self.options["forest_server_url"],
                 "is_production": self.options["is_production"],
-                "permission_cache_duration": 60,
+                "permission_cache_duration": self.options["permissions_cache_duration_in_seconds"],
             }
         )
 
     def __mk_resources(self):
         self._resources: Resources = {
             "authentication": Authentication(self.options),
             "crud": CrudResource(self.customizer.stack.datasource, self._permission_service, self.options),
@@ -94,16 +96,26 @@
         meta = getattr(self, "META", None)
         if meta is None:
             raise AgentToolkitException("The agent subclass should set the META attribute")
         return meta
 
     async def start(self):
         if Agent.__IS_INITIALIZED is True:
+            ForestLogger.log("debug", "Agent already started.")
             return
+        ForestLogger.log("debug", "Starting agent")
 
         for collection in self.customizer.stack.datasource.collections:
             create_json_api_schema(collection)
 
-        api_map = await SchemaEmitter.get_serialized_schema(self.options, self.customizer.stack.datasource, self.meta)
+        try:
+            api_map = await SchemaEmitter.get_serialized_schema(
+                self.options, self.customizer.stack.datasource, self.meta
+            )
 
-        await ForestHttpApi.send_schema(self.options, api_map)
+            await ForestHttpApi.send_schema(self.options, api_map)
+
+        except Exception:
+            ForestLogger.log("warning", "Cannot send the apimap to Forest. Are you online?")
+
+        ForestLogger.log("info", "Agent started")
         Agent.__IS_INITIALIZED = True
```

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/__init__.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/permissions/__init__.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 from typing import Any, Dict, List, Union
 
-from forestadmin.agent_toolkit.exceptions import ForestException
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.options import Options
 from forestadmin.agent_toolkit.utils.forest_schema.generator_collection import SchemaCollectionGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.type import AgentMeta, ForestServerCollection
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.datasource_customizer.datasource_customizer import DatasourceCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource
 
@@ -73,17 +73,19 @@
         else:
             try:
                 with open(options["schema_path"], "r", encoding="utf-8") as schema_file:
                     schema = json.load(schema_file)
                 meta.update(schema["meta"])
                 collections_schema = schema["collections"]
             except Exception:
-                raise ForestException(
-                    f"Can't read {options['schema_path']}. Providing a schema is mandatory in production."
+                ForestLogger.log(
+                    "error",
+                    f"Can't read {options['schema_path']}. Providing a schema is mandatory in production. Skipping...",
                 )
+                raise
 
         return cls.serialize(collections_schema, meta)
 
     @staticmethod
     async def generate(
         prefix: str, datasource: Union[Datasource[Collection], DatasourceCustomizer]
     ) -> List[ForestServerCollection]:
```

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
+from typing import Any, Dict, Optional
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-from typing import Any, Dict, Optional
-
 import aiohttp
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.options import Options
 from forestadmin.agent_toolkit.utils.forest_schema.type import ForestSchema
 
 
 class ForestHttpApiException(AgentToolkitException):
     pass
 
@@ -79,20 +79,23 @@
                     if response.status == 200:
                         return await response.json()
                     return None
             except aiohttp.ClientError as exc:
                 raise ForestHttpApiException(f"Failed to fetch {endpoint} : {exc}")
 
     @classmethod
-    async def send_schema(cls, options: Options, schema: ForestSchema):
+    async def send_schema(cls, options: Options, schema: ForestSchema) -> bool:
         ret = await cls.post(
             cls.build_enpoint(options["forest_server_url"], "/forest/apimaps/hashcheck"),
             {"schemaFileHash": schema["meta"]["schemaFileHash"]},
             {"forest-secret-key": options["env_secret"], "content-type": "application/json"},
         )
 
         if ret["sendSchema"] is True:
+            ForestLogger.log("info", "Schema was updated, sending new version.")
             await cls.post(
                 cls.build_enpoint(options["forest_server_url"], "/forest/apimaps"),
                 schema,
                 {"forest-secret-key": options["env_secret"], "content-type": "application/json"},
             )
+        else:
+            ForestLogger.log("info", "Schema was not updated since last run.")
```

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b3/pyproject.toml` & `forestadmin_agent_toolkit-1.0.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
-version = "1.0.0-beta.3"
+version = "1.0.0-beta.4"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 tzdata = "~2022.6"
 aiohttp = "~=3.8"
 oic = "~=1.4"
 python-jose = ">=3.3, <4.0"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
-forestadmin-datasource-toolkit = "^1.0.0-beta.3"
+forestadmin-datasource-toolkit = "^1.0.0-beta.4"
 [[tool.poetry.dependencies.pandas]]
 version = "<=1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.3.4,<=1.3.5"
 python = ">=3.7.1,<3.8"
```

### Comparing `forestadmin_agent_toolkit-1.0.0b3/PKG-INFO` & `forestadmin_agent_toolkit-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.3,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.4,<2.0.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (<=1.1.5) ; python_full_version < "3.7.1"
 Requires-Dist: pandas (>=1.3.4,<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: python-jose (>=3.3,<4.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
```

