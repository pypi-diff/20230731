# Comparing `tmp/logger_extras-0.3.1.tar.gz` & `tmp/logger_extras-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_extras-0.3.1.tar", last modified: Sat Jul 29 13:52:00 2023, max compression
+gzip compressed data, was "logger_extras-0.3.2.tar", last modified: Mon Jul 31 20:57:00 2023, max compression
```

## Comparing `logger_extras-0.3.1.tar` & `logger_extras-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:52:00.100489 logger_extras-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-29 13:51:44.000000 logger_extras-0.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:52:00.096489 logger_extras-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:52:00.096489 logger_extras-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-29 13:51:44.000000 logger_extras-0.3.1/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-29 13:51:44.000000 logger_extras-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 13:51:44.000000 logger_extras-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-29 13:51:44.000000 logger_extras-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-29 13:52:00.100489 logger_extras-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-29 13:51:44.000000 logger_extras-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:52:00.100489 logger_extras-0.3.1/logger_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-29 13:51:44.000000 logger_extras-0.3.1/logger_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-29 13:51:59.000000 logger_extras-0.3.1/logger_extras/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-29 13:51:44.000000 logger_extras-0.3.1/logger_extras/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-29 13:51:44.000000 logger_extras-0.3.1/logger_extras/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-29 13:51:44.000000 logger_extras-0.3.1/logger_extras/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-29 13:51:44.000000 logger_extras-0.3.1/logger_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-29 13:51:44.000000 logger_extras-0.3.1/logger_extras/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:52:00.100489 logger_extras-0.3.1/logger_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-29 13:52:00.000000 logger_extras-0.3.1/logger_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-29 13:52:00.000000 logger_extras-0.3.1/logger_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:52:00.000000 logger_extras-0.3.1/logger_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-29 13:52:00.000000 logger_extras-0.3.1/logger_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 13:52:00.000000 logger_extras-0.3.1/logger_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-29 13:51:44.000000 logger_extras-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:52:00.100489 logger_extras-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:52:00.100489 logger_extras-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-29 13:51:44.000000 logger_extras-0.3.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 20:56:38.000000 logger_extras-0.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.950458 logger_extras-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.950458 logger_extras-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-31 20:56:38.000000 logger_extras-0.3.2/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-31 20:56:38.000000 logger_extras-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 20:56:38.000000 logger_extras-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-31 20:56:38.000000 logger_extras-0.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-31 20:57:00.954458 logger_extras-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-31 20:56:38.000000 logger_extras-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/logger_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/logger_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-31 20:56:38.000000 logger_extras-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:57:00.954458 logger_extras-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-31 20:56:38.000000 logger_extras-0.3.2/tests/test_tools.py
```

### Comparing `logger_extras-0.3.1/.github/workflows/test_build.yml` & `logger_extras-0.3.2/.github/workflows/test_build.yml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/.gitignore` & `logger_extras-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/LICENSE` & `logger_extras-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/PKG-INFO` & `logger_extras-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_extras
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `logger_extras-0.3.1/README.md` & `logger_extras-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/logger_extras/filters.py` & `logger_extras-0.3.2/logger_extras/filters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/logger_extras/formatters.py` & `logger_extras-0.3.2/logger_extras/formatters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/logger_extras/mqtt.py` & `logger_extras-0.3.2/logger_extras/mqtt.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,22 @@
         protocol: int = mqtt.MQTTv311,
         qos: int = 0,
         transport: str = 'tcp',
         use_tls: bool | str = False,
         username: str = '',
         password: str = '',
         append_logger_name: bool = False,
+        connected_topic: str = '',
     ):
         super().__init__()
 
         self._topic = topic
         self._qos = qos
         self._append_logger_name = append_logger_name
+        self._connected_topic = connected_topic
 
         self.mqtt = mqtt.Client(
             client_id=client_id,
             userdata=userdata,
             protocol=protocol,
             transport=transport)
 
@@ -51,16 +53,24 @@
                 port=port,
                 keepalive=keepalive,
                 bind_address=bind_address)
         except (TimeoutError, ValueError, ConnectionRefusedError):
             print(f"Failed to connect to MQTT broker at {host}:{port}")
             return
         self.mqtt.loop_start()
+        if connected_topic:
+            self.mqtt.publish(connected_topic, '{"state": "connected"}', qos=1, retain=True)
+            self.mqtt.will_set(
+                connected_topic, '{"state": "disconnected"}', qos=1, retain=True)
 
     def __del__(self) -> None:
+        if self._connected_topic:
+            res = self.mqtt.publish(
+                self._connected_topic, '{"state": "disconnected"}', qos=1, retain=True)
+            res.wait_for_publish(1)
         self.mqtt.disconnect()
         self.mqtt.loop_stop()
 
     def emit(self, record: logging.LogRecord) -> None:
         try:
             if (
                 self.mqtt._logger  # type: ignore[attr-defined]
```

### Comparing `logger_extras-0.3.1/logger_extras/utils.py` & `logger_extras-0.3.2/logger_extras/utils.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/logger_extras.egg-info/PKG-INFO` & `logger_extras-0.3.2/logger_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-extras
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `logger_extras-0.3.1/pyproject.toml` & `logger_extras-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.1/tests/test_tools.py` & `logger_extras-0.3.2/tests/test_tools.py`

 * *Files identical despite different names*

