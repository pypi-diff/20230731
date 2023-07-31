# Comparing `tmp/hahomematic-2023.7.6.tar.gz` & `tmp/hahomematic-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.6.tar", last modified: Sat Jul 29 06:40:40 2023, max compression
+gzip compressed data, was "hahomematic-2023.8.0.tar", last modified: Mon Jul 31 17:34:42 2023, max compression
```

## Comparing `hahomematic-2023.7.6.tar` & `hahomematic-2023.8.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    55163 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    48392 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27926 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:40:40.508001 hahomematic-2023.7.6/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-29 06:40:39.000000 hahomematic-2023.7.6/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-29 06:40:40.000000 hahomematic-2023.7.6/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:40:39.000000 hahomematic-2023.7.6/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:40:38.000000 hahomematic-2023.7.6/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-29 06:40:40.000000 hahomematic-2023.7.6/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 06:40:40.000000 hahomematic-2023.7.6/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-29 06:40:10.000000 hahomematic-2023.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-29 06:40:40.512001 hahomematic-2023.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.473857 hahomematic-2023.8.0/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.473857 hahomematic-2023.8.0/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55163 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48392 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.477857 hahomematic-2023.8.0/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.477857 hahomematic-2023.8.0/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.477857 hahomematic-2023.8.0/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.473857 hahomematic-2023.8.0/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-31 17:34:41.000000 hahomematic-2023.8.0/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-31 17:34:42.000000 hahomematic-2023.8.0/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:34:41.000000 hahomematic-2023.8.0/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:34:40.000000 hahomematic-2023.8.0/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 17:34:42.000000 hahomematic-2023.8.0/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 17:34:42.000000 hahomematic-2023.8.0/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/setup.cfg
```

### Comparing `hahomematic-2023.7.6/LICENSE` & `hahomematic-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/PKG-INFO` & `hahomematic-2023.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.6
+Version: 2023.8.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.6/README.md` & `hahomematic-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/__init__.py` & `hahomematic-2023.8.0/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/caches/dynamic.py` & `hahomematic-2023.8.0/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/caches/persistent.py` & `hahomematic-2023.8.0/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/caches/visibility.py` & `hahomematic-2023.8.0/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/central_unit.py` & `hahomematic-2023.8.0/hahomematic/central_unit.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/client.py` & `hahomematic-2023.8.0/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/const.py` & `hahomematic-2023.8.0/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/decorators.py` & `hahomematic-2023.8.0/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/exceptions.py` & `hahomematic-2023.8.0/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/exporter.py` & `hahomematic-2023.8.0/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/hmcli.py` & `hahomematic-2023.8.0/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/json_rpc_client.py` & `hahomematic-2023.8.0/hahomematic/json_rpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     async def _do_logout(self, session_id: str | None) -> None:
         """Logout of CCU."""
         if not session_id:
             _LOGGER.debug("DO_LOGOUT: Not logged in. Not logging out.")
             return
 
         method = "Session.logout"
-        params = {"_session_id_": session_id}
+        params = {SESSION_ID: session_id}
         await self._do_post(
             session_id=session_id,
             method=method,
             extra_params=params,
         )
         _LOGGER.debug("DO_LOGOUT: Method: %s [%s]", method, session_id)
 
@@ -712,15 +712,15 @@
 
 def _get_params(
     session_id: bool | str,
     extra_params: dict[str, Any] | None,
     use_default_params: bool,
 ) -> dict[str, Any]:
     """Add additional params to default prams."""
-    params: dict[str, Any] = {"_session_id_": session_id} if use_default_params else {}
+    params: dict[str, Any] = {SESSION_ID: session_id} if use_default_params else {}
     if extra_params:
         params.update(extra_params)
     return params
 
 
 def _convert_to_values_cache(
     all_device_data: dict[str, Any]
```

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/__init__.py` & `hahomematic-2023.8.0/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/const.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/light.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/support.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.8.0/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/device.py` & `hahomematic-2023.8.0/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/entity.py` & `hahomematic-2023.8.0/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/event.py` & `hahomematic-2023.8.0/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/action.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/button.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/number.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/select.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.8.0/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/button.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/button.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     def available(self) -> bool:
         """Return the availability of the device."""
         return self.is_active
 
     def get_name(self, data: HubData) -> str:
         """Return the name of the program button entity."""
         if data.name.lower().startswith(tuple({"p_", "prg_"})):
-            return data.name.title()
-        return f"P_{data.name}".title()
+            return data.name
+        return f"P_{data.name}"
 
     def update_data(self, data: ProgramData) -> None:
         """Set variable value on CCU/Homegear."""
         do_update: bool = False
         if self.is_active != data.is_active:
             self.is_active = data.is_active
             do_update = True
```

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,17 @@
     @property
     def is_extended(self) -> bool:
         """Return if the entity is an extended type."""
         return self._attr_is_extended
 
     def get_name(self, data: HubData) -> str:
         """Return the name of the sysvar entity."""
-        if data.name.lower().startswith(tuple({"v_", "sv_"})):
-            return data.name.title()
-        return f"Sv_{data.name}".title()
+        if data.name.lower().startswith(tuple({"v_", "sv_", "sv"})):
+            return data.name
+        return f"Sv_{data.name}"
 
     def update_value(self, value: Any) -> None:
         """Set variable value on CCU/Homegear."""
         if self.data_type:
             value = parse_sys_var(data_type=self.data_type, raw_value=value)
         else:
             old_value = self._attr_value
```

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/number.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/select.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/hub/text.py` & `hahomematic-2023.8.0/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/support.py` & `hahomematic-2023.8.0/hahomematic/platforms/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         """Return an empty EntityNameData."""
         return EntityNameData(device_name="", channel_name="")
 
     @property
     def entity_name(self) -> str | None:
         """Return the name of the entity only name."""
         if self._device_name and self._name and self._name.startswith(self._device_name):
-            return self._name.replace(self._device_name, "").strip()
+            return self._name[len(self._device_name) :].lstrip()
         return self._name
 
     @property
     def full_name(self) -> str:
         """Return the full name of the entity."""
         if self.entity_name:
             return f"{self._device_name} {self.entity_name}".strip()
```

### Comparing `hahomematic-2023.7.6/hahomematic/platforms/update.py` & `hahomematic-2023.8.0/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.8.0/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.8.0/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.8.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/support.py` & `hahomematic-2023.8.0/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.8.0/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic/xml_rpc_server.py` & `hahomematic-2023.8.0/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.8.0/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.6
+Version: 2023.8.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.6/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.8.0/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.6/pyproject.toml` & `hahomematic-2023.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.6"
+version     = "2023.8.0"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

