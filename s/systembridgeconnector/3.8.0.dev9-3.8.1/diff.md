# Comparing `tmp/systembridgeconnector-3.8.0.dev9.tar.gz` & `tmp/systembridgeconnector-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeconnector-3.8.0.dev9.tar", last modified: Tue Jul 18 14:34:42 2023, max compression
+gzip compressed data, was "systembridgeconnector-3.8.1.tar", last modified: Mon Jul 31 14:17:35 2023, max compression
```

## Comparing `systembridgeconnector-3.8.0.dev9.tar` & `systembridgeconnector-3.8.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:34:42.707561 systembridgeconnector-3.8.0.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 14:34:42.703561 systembridgeconnector-3.8.0.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:34:42.707561 systembridgeconnector-3.8.0.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:34:42.699560 systembridgeconnector-3.8.0.dev9/systembridgeconnector/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 14:34:41.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:34:42.703561 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data_remote_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/open_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/open_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/register_data_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/update_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17270 2023-07-18 14:34:26.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:34:42.699560 systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 14:34:42.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-18 14:34:42.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:34:42.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 14:34:42.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 14:34:42.000000 systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:17:35.975778 systembridgeconnector-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-31 14:17:35.975778 systembridgeconnector-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:17:35.975778 systembridgeconnector-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:17:35.971778 systembridgeconnector-3.8.1/systembridgeconnector/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:17:35.975778 systembridgeconnector-3.8.1/systembridgeconnector/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/database_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/database_data_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/database_data_remote_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/database_data_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/media_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/register_data_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/models/update_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-07-31 14:17:24.000000 systembridgeconnector-3.8.1/systembridgeconnector/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:17:35.971778 systembridgeconnector-3.8.1/systembridgeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-31 14:17:35.000000 systembridgeconnector-3.8.1/systembridgeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-31 14:17:35.000000 systembridgeconnector-3.8.1/systembridgeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:17:35.000000 systembridgeconnector-3.8.1/systembridgeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 14:17:35.000000 systembridgeconnector-3.8.1/systembridgeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 14:17:35.000000 systembridgeconnector-3.8.1/systembridgeconnector.egg-info/top_level.txt
```

### Comparing `systembridgeconnector-3.8.0.dev9/pyproject.toml` & `systembridgeconnector-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/setup.py` & `systembridgeconnector-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/const.py` & `systembridgeconnector-3.8.1/systembridgeconnector/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,27 @@
 SUBTYPE_BAD_API_KEY = "BAD_API_KEY"
 SUBTYPE_BAD_DIRECTORY = "BAD_DIRECTORY"
 SUBTYPE_BAD_FILE = "BAD_FILE"
 SUBTYPE_BAD_JSON = "BAD_JSON"
 SUBTYPE_BAD_KEY = "MISSING_KEY"
 SUBTYPE_BAD_PATH = "BAD_PATH"
 SUBTYPE_BAD_REQUEST = "BAD_REQUEST"
+SUBTYPE_INVALID_ACTION = "INVALID_ACTION"
 SUBTYPE_LISTENER_ALREADY_REGISTERED = "LISTENER_ALREADY_REGISTERED"
 SUBTYPE_LISTENER_NOT_REGISTERED = "LISTENER_NOT_REGISTERED"
+SUBTYPE_MISSING_ACTION = "MISSING_ACTION"
 SUBTYPE_MISSING_API_KEY = "MISSING_API_KEY"
 SUBTYPE_MISSING_BASE = "MISSING_BASE"
 SUBTYPE_MISSING_KEY = "MISSING_KEY"
-SUBTYPE_MISSING_TITLE = "MISSING_TITLE"
 SUBTYPE_MISSING_MODULES = "MISSING_MODULES"
 SUBTYPE_MISSING_PATH = "MISSING_PATH"
 SUBTYPE_MISSING_PATH_URL = "MISSING_PATH_URL"
 SUBTYPE_MISSING_SETTING = "MISSING_SETTING"
 SUBTYPE_MISSING_TEXT = "MISSING_TEXT"
+SUBTYPE_MISSING_TITLE = "MISSING_TITLE"
 SUBTYPE_MISSING_VALUE = "MISSING_VALUE"
 SUBTYPE_UNKNOWN_EVENT = "UNKNOWN_EVENT"
 TYPE_APPLICATION_UPDATE = "APPLICATION_UPDATE"
 TYPE_APPLICATION_UPDATING = "APPLICATION_UPDATING"
 TYPE_DATA_GET = "DATA_GET"
 TYPE_DATA_LISTENER_REGISTERED = "DATA_LISTENER_REGISTERED"
 TYPE_DATA_LISTENER_UNREGISTERED = "DATA_LISTENER_UNREGISTERED"
@@ -111,14 +113,15 @@
 TYPE_GET_REMOTE_BRIDGES_RESULT = "GET_REMOTE_BRIDGES_RESULT"
 TYPE_GET_SETTING = "GET_SETTING"
 TYPE_GET_SETTINGS = "GET_SETTINGS"
 TYPE_KEYBOARD_KEY_PRESSED = "KEYBOARD_KEY_PRESSED"
 TYPE_KEYBOARD_KEYPRESS = "KEYBOARD_KEYPRESS"
 TYPE_KEYBOARD_TEXT = "KEYBOARD_TEXT"
 TYPE_KEYBOARD_TEXT_SENT = "KEYBOARD_TEXT_SENT"
+TYPE_MEDIA_CONTROL = "MEDIA_CONTROL"
 TYPE_NOTIFICATION = "NOTIFICATION"
 TYPE_NOTIFICATION_SENT = "NOTIFICATION_SENT"
 TYPE_OPEN = "OPEN"
 TYPE_OPENED = "OPENED"
 TYPE_POWER_HIBERNATE = "POWER_HIBERNATE"
 TYPE_POWER_HIBERNATING = "POWER_HIBERNATING"
 TYPE_POWER_LOCK = "POWER_LOCK"
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/http_client.py` & `systembridgeconnector-3.8.1/systembridgeconnector/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/battery.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/battery.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  battery.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
@@ -18,11 +18,14 @@
 
 
 class Battery(BaseModel):
     """
     Battery
     """
 
+    class Config:
+        extra = Extra.allow
+
     id: Optional[str] = Field(None, description="Event ID")
     is_charging: Optional[bool] = None
     percentage: Optional[float] = None
     last_updated: Optional[LastUpdated] = Field(None, description="Last updated")
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/cpu.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/data.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/data.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/database_data.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data_bridge.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/database_data_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/database_data_remote_bridge.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/database_data_remote_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/disk.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/disk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  disk.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
@@ -24,14 +24,17 @@
 
 
 class Disk(BaseModel):
     """
     Disk
     """
 
+    class Config:
+        extra = Extra.allow
+
     id: Optional[str] = Field(None, description="Event ID")
     devices: list
     io_counters_read_count: Optional[int] = None
     io_counters_write_count: Optional[int] = None
     io_counters_read_bytes: Optional[int] = None
     io_counters_write_bytes: Optional[int] = None
     io_counters_read_time: Optional[int] = None
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # generated by datamodel-codegen:
 #   filename:  media.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Extra
 
 
 class Media(BaseModel):
     """
     Media Info
     """
 
+    class Config:
+        extra = Extra.allow
+
     album_artist: Optional[str] = None
     album_title: Optional[str] = None
     artist: Optional[str] = None
     duration: Optional[float] = None
     is_fast_forward_enabled: Optional[bool] = None
     is_next_enabled: Optional[bool] = None
     is_pause_enabled: Optional[bool] = None
@@ -30,7 +33,8 @@
     shuffle: Optional[bool] = None
     status: Optional[str] = None
     subtitle: Optional[str] = None
     thumbnail: Optional[str] = None
     title: Optional[str] = None
     track_number: Optional[int] = None
     type: Optional[str] = None
+    updated_at: Optional[float] = None
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/media_files.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/memory.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  memory.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
@@ -27,14 +27,17 @@
 
 
 class Memory(BaseModel):
     """
     Memory
     """
 
+    class Config:
+        extra = Extra.allow
+
     id: Optional[str] = Field(None, description="Event ID")
     swap_total: Optional[int] = None
     swap_used: Optional[int] = None
     swap_free: Optional[float] = None
     swap_percent: Optional[float] = None
     swap_sin: Optional[int] = None
     swap_sout: Optional[int] = None
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/network.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  network.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
@@ -24,14 +24,17 @@
 
 
 class Network(BaseModel):
     """
     Network
     """
 
+    class Config:
+        extra = Extra.allow
+
     id: Optional[str] = Field(None, description="Event ID")
     io_counters_bytes_sent: Optional[int] = None
     io_counters_bytes_recv: Optional[int] = None
     io_counters_packets_sent: Optional[int] = None
     io_counters_packets_recv: Optional[int] = None
     io_counters_errin: Optional[int] = None
     io_counters_errout: Optional[int] = None
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/notification.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/response.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # generated by datamodel-codegen:
 #   filename:  response.json
 
 from __future__ import annotations
 
 from typing import Any, Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 
 class Response(BaseModel):
     """
     Response
     """
 
+    class Config:
+        extra = Extra.allow
+
     id: Optional[str] = Field(None, description="Message ID")
     type: str = Field(..., description="Type")
     subtype: Optional[str] = Field(None, description="Subtype")
     message: Optional[str] = Field(None, description="Message")
     module: Optional[str] = Field(None, description="Module")
     data: Optional[Any] = Field(None, description="Data")
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/models/system.py` & `systembridgeconnector-3.8.1/systembridgeconnector/models/system.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/version.py` & `systembridgeconnector-3.8.1/systembridgeconnector/version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector/websocket_client.py` & `systembridgeconnector-3.8.1/systembridgeconnector/websocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     TYPE_EXIT_APPLICATION,
     TYPE_GET_DATA,
     TYPE_GET_DIRECTORIES,
     TYPE_GET_FILE,
     TYPE_GET_FILES,
     TYPE_KEYBOARD_KEYPRESS,
     TYPE_KEYBOARD_TEXT,
+    TYPE_MEDIA_CONTROL,
     TYPE_NOTIFICATION,
     TYPE_OPEN,
     TYPE_POWER_HIBERNATE,
     TYPE_POWER_LOCK,
     TYPE_POWER_LOGOUT,
     TYPE_POWER_RESTART,
     TYPE_POWER_SHUTDOWN,
@@ -48,14 +49,15 @@
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
 )
 from .models.get_data import GetData
 from .models.keyboard_key import KeyboardKey
 from .models.keyboard_text import KeyboardText
+from .models.media_control import MediaControl
 from .models.media_directories import MediaDirectories
 from .models.media_files import File as MediaFile
 from .models.media_files import MediaFiles
 from .models.media_get_file import MediaGetFile
 from .models.media_get_files import MediaGetFiles
 from .models.notification import Notification
 from .models.open_path import OpenPath
@@ -87,15 +89,15 @@
     @property
     def connected(self) -> bool:
         """Get connection state."""
         return self._websocket is not None and not self._websocket.closed
 
     async def _send_message(
         self,
-        request,
+        request: Request,
         wait_for_response: bool = True,
         response_type: Optional[str] = None,
     ) -> Response:
         """Send a message to the WebSocket"""
         if not self.connected or self._websocket is None:
             raise ConnectionClosedException("Connection is closed")
 
@@ -285,14 +287,29 @@
                 **{
                     EVENT_EVENT: TYPE_KEYBOARD_TEXT,
                     **model.dict(),
                 }
             )
         )
 
+    async def media_control(
+        self,
+        model: MediaControl,
+    ) -> Response:
+        """Media control"""
+        self._logger.info("Media control: %s", model.json())
+        return await self._send_message(
+            Request(
+                **{
+                    EVENT_EVENT: TYPE_MEDIA_CONTROL,
+                    **model.dict(),
+                }
+            )
+        )
+
     async def send_notification(
         self,
         model: Notification,
     ) -> Response:
         """Send notification"""
         self._logger.info("Send notification: %s", model.json())
         return await self._send_message(
```

### Comparing `systembridgeconnector-3.8.0.dev9/systembridgeconnector.egg-info/SOURCES.txt` & `systembridgeconnector-3.8.1/systembridgeconnector.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 systembridgeconnector/models/generic.py
 systembridgeconnector/models/get_data.py
 systembridgeconnector/models/get_setting.py
 systembridgeconnector/models/gpu.py
 systembridgeconnector/models/keyboard_key.py
 systembridgeconnector/models/keyboard_text.py
 systembridgeconnector/models/media.py
+systembridgeconnector/models/media_control.py
 systembridgeconnector/models/media_directories.py
 systembridgeconnector/models/media_files.py
 systembridgeconnector/models/media_get_file.py
 systembridgeconnector/models/media_get_files.py
 systembridgeconnector/models/media_play.py
 systembridgeconnector/models/memory.py
 systembridgeconnector/models/network.py
```

