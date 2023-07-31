# Comparing `tmp/hypergo-0.1.3.tar.gz` & `tmp/hypergo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.3.tar", last modified: Mon Jul 17 14:35:13 2023, max compression
+gzip compressed data, was "hypergo-0.1.4.tar", last modified: Mon Jul 31 14:49:18 2023, max compression
```

## Comparing `hypergo-0.1.3.tar` & `hypergo-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.113808 hypergo-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.105808 hypergo-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.109808 hypergo-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 14:34:59.000000 hypergo-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-17 14:34:59.000000 hypergo-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 14:34:59.000000 hypergo-0.1.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-17 14:34:59.000000 hypergo-0.1.3/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:59.000000 hypergo-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-17 14:35:13.113808 hypergo-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 14:34:59.000000 hypergo-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.109808 hypergo-0.1.3/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-17 14:34:59.000000 hypergo-0.1.3/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.113808 hypergo-0.1.3/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:35:13.000000 hypergo-0.1.3/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-07-17 14:34:59.000000 hypergo-0.1.3/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 14:34:59.000000 hypergo-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 14:34:59.000000 hypergo-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 14:35:13.113808 hypergo-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:13.113808 hypergo-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-17 14:34:59.000000 hypergo-0.1.3/tests/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.435377 hypergo-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.427377 hypergo-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.427377 hypergo-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 14:49:08.000000 hypergo-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-31 14:49:08.000000 hypergo-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 14:49:08.000000 hypergo-0.1.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-31 14:49:08.000000 hypergo-0.1.4/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:08.000000 hypergo-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:49:18.435377 hypergo-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 14:49:08.000000 hypergo-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-31 14:49:08.000000 hypergo-0.1.4/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 14:49:08.000000 hypergo-0.1.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.431378 hypergo-0.1.4/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.431378 hypergo-0.1.4/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-07-31 14:49:08.000000 hypergo-0.1.4/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 14:49:08.000000 hypergo-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 14:49:18.435377 hypergo-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-31 14:49:08.000000 hypergo-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.435377 hypergo-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.1.3/.github/workflows/python-publish.yml` & `hypergo-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/.gitignore` & `hypergo-0.1.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 *.log
 
 # Directories
 log/
 logs/
 tmp/
 cache/
+sandbox/
 
 
 #######################################
 # Archives                            #
 #######################################
 
 *.7z
```

### Comparing `hypergo-0.1.3/BACKLOG.md` & `hypergo-0.1.4/BACKLOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,64 @@
+----------
+# PHASE 1
+- [x] local component runner
+- [x] decorators
+        - [x] serialization
+- [ ] decorator refactor
+- [ ] sdk unit tests
+        - [ ] automated in linter
+- [ ] create an SDK file and message viewer (for compressed and encrypted and serialized messages)
+- [ ] more decorators
+        - [x] passbyref
+        - [ ] validation
+        - [x] compression
+        - [ ] encryption
+        - [ ] mapping
+        - [ ] transactions
+- [ ] clean up utility class
+- [ ] graph fixes
+        - [ ] xenon complexity issues
+        - [ ] group like types into subgraphs
+        - [ ] support wildcard configurations
+        - [ ] show payloads or bindings
+- [ ] routing key specific configuration
+        - [ ] consolidate custom_properties into routing key configurations
+        - [ ] custom_properties support (or equivalent)
+- [ ] automatic passthru routing keys
+        - [ ] how do we terminate them if unconsumed
+- [ ] function injection
+        - safe cast arguments
+- [ ] mapper library
+- [ ] configuration version routing
+        - [ ] use mapper library to map old configuration into new
+- [ ] mapping instead of bindings
+        - [ ] dict/list/str parsing (use mapper library)
+                - [ ] functions with eval?
+                - [ ] "?" wildcards
+- [ ] routing key management
+        - [ ] "matched input key"
+- [ ] transaction support
+        - [ ] higher level transactions
+                - [ ] request response
+                - [ ] map/reduce
+- [ ] linting and mypy
+
+
+----------
+# PHASE 2
+
+- [ ] component unit test template
+- [ ] instrumentation
+- [ ] monitoring
+- [ ] exception handling
+- [ ] logging
+- [ ] kafka (or similar) event stream
+- [ ] additional decorators
+        - [ ] streaming
+----------
 
 - [ ] pycoverage
 - [ ] pytest on top of unittest
 - [ ] make sure utiltiy/safecast tests are thorough
 - [ ] hypergo cli
         hypergo http, stdio, azure, rabbit, etc.
 - [ ] Combine Config and ConfigType, And Message and MessageType
```

### Comparing `hypergo-0.1.3/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.4/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/hypergo/graph.py` & `hypergo-0.1.4/hypergo/graph.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -118,8 +118,8 @@
     topics(dot, configs)
     derived_topics(dot, configs)
 
     dot.render('.graph.gv', view=True)
 
 
 if __name__ == '__main__':
-    graph(sys.argv[1:])
+    graph(sys.argv[1:])
```

### Comparing `hypergo-0.1.3/hypergo/message.py` & `hypergo-0.1.4/hypergo/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,22 @@
             "body": json.loads(message.get_body().decode("utf-8")),
             "routingkey": message.user_properties["routingkey"],
             "storagekey": cast(str, message.user_properties.get("storagekey")),
         }
 
     @staticmethod
     def from_http_request(request: func.HttpRequest) -> MessageType:
-        return {"body": request.get_json(), "routingkey": "http.azurefunction" + urlparse(request.url).path.replace("/", ".")}
+        return {
+            "body": request.get_json(),
+            "routingkey": "http.azurefunction" + urlparse(request.url).path.replace("/", "."),
+        }
+
+    @staticmethod
+    def from_stdio_message(stdin: str) -> MessageType:
+        return cast(MessageType, json.loads(stdin))
 
     @staticmethod
     def to_azure_service_bus_service_bus_message(message: MessageType) -> ServiceBusMessage:
         ret: ServiceBusMessage = ServiceBusMessage(
             body=json.dumps(message["body"]),
             application_properties={
                 "routingkey": message["routingkey"],
```

### Comparing `hypergo-0.1.3/hypergo/service_bus_connection.py` & `hypergo-0.1.4/hypergo/service_bus_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from abc import ABC, abstractmethod
-from typing import Union
+from typing import Union, cast
 
 from hypergo.config import ConfigType
 from hypergo.executor import Executor
 from hypergo.message import MessageType
 from hypergo.storage import Storage
 
 
 class ServiceBusConnection(ABC):
     def general_consume(self, message: MessageType, config: ConfigType, storage: Union[Storage, None]) -> None:
         executor: Executor = Executor(config, storage)
         for execution in executor.execute(message):
-            self.send(execution, config["namespace"])
+            self.send(cast(MessageType, execution), config["namespace"])
 
     @abstractmethod
     def send(self, message: MessageType, namespace: str) -> None:
         ...
```

### Comparing `hypergo-0.1.3/hypergo/storage.py` & `hypergo-0.1.4/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/hypergo/version.py` & `hypergo-0.1.4/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.4/hypergo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 .gitignore
 .pylintrc
 BACKLOG.md
 LICENSE
 README.md
+RELEASE_NOTES.md
+dev-requirements.txt
 lint.sh
 pyproject.toml
-requirements.txt
 setup.cfg
+setup.py
 .github/workflows/python-publish.yml
 hypergo/__init__.py
 hypergo/azure_service_bus_connection.py
 hypergo/azure_service_bus_executor.py
 hypergo/config.py
 hypergo/context.py
 hypergo/custom_types.py
 hypergo/executor.py
 hypergo/graph.py
+hypergo/hypergo_cli.py
+hypergo/hypergo_click.py
+hypergo/hypergo_cmd.py
 hypergo/key_value_store.py
 hypergo/local_storage.py
 hypergo/message.py
 hypergo/service_bus_connection.py
+hypergo/stdio_connection.py
 hypergo/storage.py
+hypergo/transform.py
 hypergo/utility.py
 hypergo/version.py
 hypergo.egg-info/PKG-INFO
 hypergo.egg-info/SOURCES.txt
 hypergo.egg-info/dependency_links.txt
+hypergo.egg-info/entry_points.txt
 hypergo.egg-info/requires.txt
 hypergo.egg-info/top_level.txt
 tests/test.json
 tests/test.yaml
 tests/test_dynamic_input_bindings.py
 tests/test_dynamic_routing_key.py
 tests/test_local_storage.py
 tests/test_message.py
 tests/test_storage.py
-tests/test_utility.py
+tests/test_utility.py
+tests/test_utility_serialization.py
```

### Comparing `hypergo-0.1.3/lint.sh` & `hypergo-0.1.4/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test.json` & `hypergo-0.1.4/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test.yaml` & `hypergo-0.1.4/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test_dynamic_input_bindings.py` & `hypergo-0.1.4/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test_dynamic_routing_key.py` & `hypergo-0.1.4/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test_local_storage.py` & `hypergo-0.1.4/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test_message.py` & `hypergo-0.1.4/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test_storage.py` & `hypergo-0.1.4/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.3/tests/test_utility.py` & `hypergo-0.1.4/tests/test_utility.py`

 * *Files identical despite different names*

