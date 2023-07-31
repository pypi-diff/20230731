# Comparing `tmp/snitch-protos-0.0.54.tar.gz` & `tmp/snitch-protos-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.54.tar", last modified: Sun Jul 30 18:55:41 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.55.tar", last modified: Mon Jul 31 01:31:56 2023, max compression
```

## Comparing `snitch-protos-0.0.54.tar` & `snitch-protos-0.0.55.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.122539 snitch-protos-0.0.54/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:55:41.122539 snitch-protos-0.0.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-30 18:55:40.000000 snitch-protos-0.0.54/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    34958 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-30 18:55:08.000000 snitch-protos-0.0.54/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:55:41.118538 snitch-protos-0.0.54/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 18:55:41.000000 snitch-protos-0.0.54/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    34904 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-31 01:31:19.000000 snitch-protos-0.0.55/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:31:56.964095 snitch-protos-0.0.55/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 01:31:56.000000 snitch-protos-0.0.55/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.54/PKG-INFO` & `snitch-protos-0.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.54
+Version: 0.0.55
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.54/setup.py` & `snitch-protos-0.0.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.54',
+    version='0.0.55',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.54/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.55/snitch_protos/protos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,50 +394,48 @@
 @dataclass(eq=False, repr=False)
 class DeregisterRequest(betterproto.Message):
     """
     Same as RegisterRequest - used for broadcasting a deregistration event
     """
 
     service_name: str = betterproto.string_field(1)
+    session_id: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class BusEvent(betterproto.Message):
     """
     Type used by `snitch-server` for broadcasting events to other snitch nodes
     """
 
     source: str = betterproto.string_field(1)
     register_request: "RegisterRequest" = betterproto.message_field(100, group="event")
     deregister_request: "DeregisterRequest" = betterproto.message_field(
         101, group="event"
     )
-    heartbeat_request: "HeartbeatRequest" = betterproto.message_field(
-        102, group="event"
-    )
     create_pipeline_request: "CreatePipelineRequest" = betterproto.message_field(
-        103, group="event"
+        102, group="event"
     )
     delete_pipeline_request: "DeletePipelineRequest" = betterproto.message_field(
-        104, group="event"
+        103, group="event"
     )
     update_pipeline_request: "UpdatePipelineRequest" = betterproto.message_field(
-        105, group="event"
+        104, group="event"
     )
     attach_pipeline_request: "AttachPipelineRequest" = betterproto.message_field(
-        106, group="event"
+        105, group="event"
     )
     detach_pipeline_request: "DetachPipelineRequest" = betterproto.message_field(
-        107, group="event"
+        106, group="event"
     )
     pause_pipeline_request: "PausePipelineRequest" = betterproto.message_field(
-        108, group="event"
+        107, group="event"
     )
     resume_pipeline_request: "ResumePipelineRequest" = betterproto.message_field(
-        109, group="event"
+        108, group="event"
     )
     metadata: Dict[str, str] = betterproto.map_field(
         1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
     )
     """
     All gRPC metadata is stored in ctx; when request goes outside of gRPC
     bounds, we will translate ctx metadata into this field. Example: 1. Request
```

### Comparing `snitch-protos-0.0.54/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.55/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.54/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.55/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.54
+Version: 0.0.55
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

