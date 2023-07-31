# Comparing `tmp/plugp100-3.3.0.tar.gz` & `tmp/plugp100-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-3.3.0.tar", last modified: Fri Jul 21 17:06:14 2023, max compression
+gzip compressed data, was "plugp100-3.4.0.tar", last modified: Mon Jul 31 19:46:32 2023, max compression
```

## Comparing `plugp100-3.3.0.tar` & `plugp100-3.4.0.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.236220 plugp100-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 17:06:03.000000 plugp100-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 17:06:03.000000 plugp100-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-21 17:06:14.236220 plugp100-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-21 17:06:03.000000 plugp100-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.228220 plugp100-3.3.0/plugp100/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/api/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/hub_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/hub_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/s200b_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/t100_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/t110_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/hub/t31x_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/ledstrip_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/light_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/light_effect_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/plug_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/power_strip_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/api/tapo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/common/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/functional/either.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/common/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/discover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/encryption/tp_link_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/handshake_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/login_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/secure_passthrough_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/requests/set_device_info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/set_device_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/set_device_info/play_alarm_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/set_device_info/set_light_color_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/set_device_info/set_light_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/set_device_info/set_plug_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/tapo_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/requests/trigger_logs_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.232220 plugp100-3.3.0/plugp100/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/alarm_type_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/child_device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/energy_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.236220 plugp100-3.3.0/plugp100/responses/hub_childs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/hub_childs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/hub_childs/s200b_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/hub_childs/t100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/hub_childs/t110_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/hub_childs/t31x_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/hub_childs/trigger_log_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/power_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 17:06:03.000000 plugp100-3.3.0/plugp100/responses/tapo_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:06:14.228220 plugp100-3.3.0/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-21 17:06:14.000000 plugp100-3.3.0/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-21 17:06:14.000000 plugp100-3.3.0/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:06:14.000000 plugp100-3.3.0/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-21 17:06:14.000000 plugp100-3.3.0/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 17:06:14.000000 plugp100-3.3.0/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 17:06:03.000000 plugp100-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 17:06:14.236220 plugp100-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-21 17:06:03.000000 plugp100-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.096267 plugp100-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 19:46:20.000000 plugp100-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 19:46:20.000000 plugp100-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-31 19:46:32.096267 plugp100-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-31 19:46:20.000000 plugp100-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.088266 plugp100-3.4.0/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/hub_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/hub_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/s200b_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/t100_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/t110_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/t31x_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/ledstrip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/light_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/light_effect_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/plug_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/power_strip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/functional/either.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/discover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/handshake_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/requests/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/internal/snowflake_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/play_alarm_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/tapo_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/trigger_logs_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.096267 plugp100-3.4.0/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/alarm_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/energy_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.096267 plugp100-3.4.0/plugp100/responses/hub_childs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/s200b_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/t100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/t110_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/t31x_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/trigger_log_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/tapo_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.088266 plugp100-3.4.0/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 19:46:20.000000 plugp100-3.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 19:46:20.000000 plugp100-3.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 19:46:32.096267 plugp100-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-31 19:46:20.000000 plugp100-3.4.0/setup.py
```

### Comparing `plugp100-3.3.0/LICENSE` & `plugp100-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/PKG-INFO` & `plugp100-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.3.0
+Version: 3.4.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.3.0/README.md` & `plugp100-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/__init__.py` & `plugp100-3.4.0/plugp100/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         sys.path.append(os.path.join(vendor_dir, vendor_path))
 
 from plugp100.responses import *
 from plugp100.requests import *
 from plugp100.api import *
 from plugp100.common import *
 
-__version__ = "3.3.0"
+__version__ = "3.4.0"
```

### Comparing `plugp100-3.3.0/plugp100/api/hub/hub_device.py` & `plugp100-3.4.0/plugp100/api/hub/hub_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         The function `login` attempts to log in to an API using a given address and returns either `True` if successful or
         an `Exception` if there is an error.
         @return: The login method is returning an Either type, which can either be True or an Exception.
         """
         return await self._api.login(self._address)
 
     async def turn_alarm_on(self, alarm: PlayAlarmParams = None) -> Either[True, Exception]:
-        request = TapoRequest(method='play_alarm', params=dataclass_encode_json(alarm))
+        request = TapoRequest(method='play_alarm', params=dataclass_encode_json(alarm) if alarm is not None else None)
         return (await self._api.execute_raw_request(request)).map(lambda _: True)
 
     async def turn_alarm_off(self) -> Either[True, Exception]:
         return (await self._api.execute_raw_request(TapoRequest(method='stop_alarm', params=None))).map(lambda _: True)
 
     async def get_state(self) -> Either[HubDeviceState, Exception]:
         """
```

### Comparing `plugp100-3.3.0/plugp100/api/hub/hub_device_tracker.py` & `plugp100-3.4.0/plugp100/api/hub/hub_device_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/hub/s200b_device.py` & `plugp100-3.4.0/plugp100/api/hub/s200b_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/hub/t100_device.py` & `plugp100-3.4.0/plugp100/api/hub/t100_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/hub/t110_device.py` & `plugp100-3.4.0/plugp100/api/hub/t110_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/hub/t31x_device.py` & `plugp100-3.4.0/plugp100/api/hub/t31x_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/ledstrip_device.py` & `plugp100-3.4.0/plugp100/api/ledstrip_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/light_device.py` & `plugp100-3.4.0/plugp100/api/light_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/light_effect.py` & `plugp100-3.4.0/plugp100/api/light_effect.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/light_effect_preset.py` & `plugp100-3.4.0/plugp100/api/light_effect_preset.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/plug_device.py` & `plugp100-3.4.0/plugp100/api/plug_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/power_strip_device.py` & `plugp100-3.4.0/plugp100/api/power_strip_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/api/tapo_client.py` & `plugp100-3.4.0/plugp100/api/tapo_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
+import uuid
 from dataclasses import dataclass
 from time import time
 from typing import Optional, Any, cast
 
 import aiohttp
 import jsons
 
 from plugp100.api.light_effect import LightEffect
 from plugp100.common.functional.either import Either, Right, Left
 from plugp100.common.utils.http_client import AsyncHttp
 from plugp100.common.utils.json_utils import dataclass_encode_json, Json
 from plugp100.requests.handshake_params import HandshakeParams
+from plugp100.requests.internal.snowflake_id import SnowflakeId
 from plugp100.requests.login_device import LoginDeviceParams
 from plugp100.requests.secure_passthrough_params import SecurePassthroughParams
 from plugp100.requests.tapo_request import TapoRequest, MultipleRequestParams
 from plugp100.responses.child_device_list import ChildDeviceList
 from plugp100.responses.energy_info import EnergyInfo
 from plugp100.responses.power_info import PowerInfo
 from plugp100.responses.tapo_response import TapoResponse
@@ -27,29 +29,33 @@
 @dataclass
 class Session:
     url: str
     key_pair: KeyPair
     chiper: TpLinkCipher
     cookie_token: Optional[str]
     token: Optional[str]
+    terminal_uuid: str
 
 
 class TapoClient:
-    TERMINAL_UUID = "88-00-DE-AD-52-E1"
 
     def __init__(
             self,
             username: str,
             password: str,
             http_session: Optional[aiohttp.ClientSession] = None,
     ):
         self._username = username
         self._password = password
         self._http = AsyncHttp(aiohttp.ClientSession() if http_session is None else http_session)
         self._session = None
+        self._request_id_generator = SnowflakeId(1, 1)
+
+    async def close(self):
+        await self._http.close()
 
     async def login(self, url: str) -> Either[True, Exception]:
         """
         The `login` function performs a handshake with a given URL, and if successful, sends a login request with a username
         and password, returning a token if successful or an exception if not.
 
         @param url: The `url` parameter is a string that represents the URL of the login endpoint
@@ -62,15 +68,15 @@
             token_or_error = await self._login_request(self._username, self._password)
             self._session.token = token_or_error.value if isinstance(token_or_error, Right) else None
             return token_or_error.map(lambda _: True)
 
         return handshake
 
     async def execute_raw_request(self, request: 'TapoRequest') -> Either[Json, Exception]:
-        request.with_terminal_uuid(self.TERMINAL_UUID).with_request_time_millis(time())
+        request.with_terminal_uuid(self._session.terminal_uuid).with_request_time_millis(round(time() * 1000))
         return (await self._execute_with_passthrough(request, require_token=True)).map(lambda x: x.result)
 
     async def get_device_info(self) -> Either[Json, Exception]:
         """
         The function `get_device_info` sends a request to retrieve device information and returns the result or an
         exception.
         @return: an `Either` object that contains either a `Json` object or an `Exception`.
@@ -126,40 +132,40 @@
 
         @param light_effect: The `light_effect` parameter is of type `LightEffect`. It represents the desired lighting
         effect that you want to set for a device
         @type light_effect: LightEffect
         @return: an `Either` object that contains either a `True` value or an `Exception`.
         """
         request = TapoRequest.set_lighting_effect(light_effect) \
-            .with_terminal_uuid(self.TERMINAL_UUID) \
-            .with_request_time_millis(time())
+            .with_terminal_uuid(self._session.terminal_uuid) \
+            .with_request_time_millis(round(time() * 1000))
         response = await self._execute_with_passthrough(request, require_token=True)
         return response.map(lambda _: True)
 
     async def get_child_device_list(self) -> Either[ChildDeviceList, Exception]:
         """
         The function `get_child_device_list` retrieves a list of child devices asynchronously and returns either the list or
         an exception.
         @return: an `Either` object, which can contain either a `ChildDeviceList` or an `Exception`.
         """
         request = TapoRequest.get_child_device_list() \
-            .with_terminal_uuid(self.TERMINAL_UUID) \
-            .with_request_time_millis(time())
+            .with_terminal_uuid(self._session.terminal_uuid) \
+            .with_request_time_millis(round(time() * 1000))
         response = await self._execute_with_passthrough(request, require_token=True)
         return response.map(lambda x: ChildDeviceList.try_from_json(**x.result))
 
     async def get_child_device_component_list(self) -> Either[Json, Exception]:
         """
         The function `get_child_device_component_list` retrieves a list of child device components asynchronously and
         returns either the JSON response or an exception.
         @return: an `Either` object, which can contain either a `Json` object or an `Exception`.
         """
         request = TapoRequest.get_child_device_component_list() \
-            .with_terminal_uuid(self.TERMINAL_UUID) \
-            .with_request_time_millis(time())
+            .with_terminal_uuid(self._session.terminal_uuid) \
+            .with_request_time_millis(round(time() * 1000))
         response = await self._execute_with_passthrough(request, require_token=True)
         return response.map(lambda x: x.result)
 
     async def control_child(self, child_id: str, request: TapoRequest) -> Either[Json, Exception]:
         """
         The function `control_child` is an asynchronous method that sends a control request to a child device and returns
         the response or an exception.
@@ -168,16 +174,16 @@
         @type child_id: str
         @param request: The `request` parameter is an instance of the `TapoRequest` class. It represents a request to be
         sent to the Tapo device.
         @type request: TapoRequest
         @return: an instance of the `Either` class, which can contain either a `Json` object or an `Exception`.
         """
         multiple_request = TapoRequest.multiple_request(MultipleRequestParams([request])) \
-            .with_terminal_uuid(self.TERMINAL_UUID) \
-            .with_request_time_millis(time())
+            .with_terminal_uuid(self._session.terminal_uuid) \
+            .with_request_time_millis(round(time() * 1000))
         request = TapoRequest.control_child(child_id, multiple_request)
         response = await self._execute_with_passthrough(request, require_token=True)
         if isinstance(response, Right):
             try:
                 responses = response.value.result['responseData']['result']['responses']
                 if len(responses) > 0:
                     return Right(responses[0]['result'])
@@ -186,29 +192,30 @@
             except Exception as e:
                 return Left(e)
         return cast(Left, response)
 
     async def _login_request(self, username: str, password: str) -> Either[str, Exception]:
         login_device_params = LoginDeviceParams(username, password)
         login_request = TapoRequest.login(login_device_params) \
-            .with_request_time_millis(time())
+            .with_request_time_millis(round(time() * 1000))
         response_as_dict = await self._execute_with_passthrough(login_request)
         return response_as_dict.map(lambda x: x.result['token'])
 
     async def _handshake(self, url: str) -> Either[True, Exception]:
         logger.debug("Will perform handshaking...")
         logger.debug("Generating keypair")
 
         url = f"http://{url}/app"
         key_pair = KeyPair.create_key_pair()
 
         handshake_params = HandshakeParams(key_pair.get_public_key())
         logger.debug(f"Handshake params: {jsons.dumps(handshake_params)}")
 
         request = TapoRequest.handshake(handshake_params)
+
         request_body = jsons.loads(jsons.dumps(request))
         logger.debug(f"Request {request_body}")
 
         response = await self._http.async_make_post(url, json=request_body)
         resp_dict = await response.json(content_type=None)
         logger.debug(f"Device responded with: {resp_dict}")
         response_or_error = TapoResponse.try_from_json(resp_dict).map(lambda _: True)
@@ -217,24 +224,25 @@
             cookie_token = response.cookies.get('TP_SESSIONID').value
             logger.debug(f"Got TP_SESSIONID token: ...{cookie_token[5:]}")
 
             logger.debug("Decoding handshake key...")
             handshake_key = resp_dict['result']['key']
             tp_link_cipher = TpLinkCipherCryptography.create_from_keypair(handshake_key, key_pair)
 
-            self._session = Session(url, key_pair, tp_link_cipher, cookie_token, token=None)
+            self._session = Session(url, key_pair, tp_link_cipher, cookie_token, token=None, terminal_uuid=str(uuid.uuid4()))
             return Right(True)
         else:
             return response_or_error
 
     async def _execute_with_passthrough(
             self,
             request: TapoRequest,
             require_token: bool = False
     ) -> Either[TapoResponse[Json], Exception]:
+        request.with_request_id(self._request_id_generator.generate_id()).with_terminal_uuid(self._session.terminal_uuid)
         encrypted_request = self._session.chiper.encrypt(jsons.dumps(request))
         passthrough_request = TapoRequest.secure_passthrough(SecurePassthroughParams(encrypted_request))
         request_body = jsons.loads(jsons.dumps(passthrough_request))
 
         logger.debug(f"Request body: {request_body}")
 
         response_encrypted = await self._http.async_make_post_cookie(
@@ -247,11 +255,11 @@
 
         return TapoResponse.try_from_json(response_as_dict) \
             .map(lambda response: jsons.loads(self._session.chiper.decrypt(response.result['response']))) \
             .bind(lambda decrypted_response: TapoResponse.try_from_json(decrypted_response))
 
     async def _set_device_info(self, device_info: Json) -> Either[True, Exception]:
         request = TapoRequest.set_device_info(device_info) \
-            .with_terminal_uuid(self.TERMINAL_UUID) \
-            .with_request_time_millis(time())
+            .with_terminal_uuid(self._session.terminal_uuid) \
+            .with_request_time_millis(round(time() * 1000))
         response = await self._execute_with_passthrough(request, require_token=True)
         return response.map(lambda _: True)
```

### Comparing `plugp100-3.3.0/plugp100/common/functional/either.py` & `plugp100-3.4.0/plugp100/common/functional/either.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import abstractmethod
 from functools import partial
 
-from typing import Callable, TypeVar, Generic
+from typing import Callable, TypeVar, Generic, Union
 
 TSource = TypeVar("TSource")
 TResult = TypeVar("TResult")
 TError = TypeVar("TError")
 TFold = TypeVar("TFold")
 
+
 # from OSlash library, copied it to avoid external dependencies and issues especially for migration to python 11
 
 class Either(Generic[TSource, TError]):
     """The Either Monad.
 
     Represents either a successful computation, or a computation that
     has failed.
@@ -142,7 +143,18 @@
         return left(self._error)
 
     def __eq__(self, other) -> bool:
         return isinstance(other, Left) and self._error == other._error
 
     def __str__(self) -> str:
         return "Left: %s" % self._error
+
+
+T = TypeVar("T")
+
+
+def value_or_raise(either: Either[T, Exception]) -> T:
+    value_or_error: Union[T, Exception] = either.fold(lambda x: x, lambda y: y)
+    if isinstance(value_or_error, Exception):
+        raise value_or_error
+    else:
+        return value_or_error
```

### Comparing `plugp100-3.3.0/plugp100/common/state_tracker.py` & `plugp100-3.4.0/plugp100/common/state_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/common/utils/http_client.py` & `plugp100-3.4.0/plugp100/common/utils/http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,11 +24,14 @@
                 url,
                 json=json,
                 cookies=cookie,
                 headers=self.common_headers
         ) as response:
             return await self._force_read_release(response)
 
+    async def close(self):
+        await self.session.close()
+
     async def _force_read_release(self, response):
         await response.read()
         await response.release()
         return response
```

### Comparing `plugp100-3.3.0/plugp100/encryption/key_pair.py` & `plugp100-3.4.0/plugp100/encryption/key_pair.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/encryption/tp_link_cipher.py` & `plugp100-3.4.0/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/example.py` & `plugp100-3.4.0/plugp100/example.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/requests/tapo_request.py` & `plugp100-3.4.0/plugp100/requests/tapo_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,18 @@
     def get_temperature_humidity_records() -> 'TapoRequest':
         return TapoRequest(method='get_temp_humidity_records', params=None)
 
     def __init__(self, method: str, params):
         self.method = method
         self.params = params
 
+    def with_request_id(self, request_id: int) -> 'TapoRequest':
+        self.requestID = request_id
+        return self
+
     def with_request_time_millis(self, t: float) -> 'TapoRequest':
         self.request_time_milis = t
         return self
 
     def with_terminal_uuid(self, uuid: str) -> 'TapoRequest':
         self.terminal_uuid = uuid
         return self
```

### Comparing `plugp100-3.3.0/plugp100/responses/alarm_type_list.py` & `plugp100-3.4.0/plugp100/responses/alarm_type_list.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/child_device_list.py` & `plugp100-3.4.0/plugp100/responses/child_device_list.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/device_state.py` & `plugp100-3.4.0/plugp100/responses/device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/energy_info.py` & `plugp100-3.4.0/plugp100/responses/energy_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/hub_childs/s200b_device_state.py` & `plugp100-3.4.0/plugp100/responses/hub_childs/s200b_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/hub_childs/t100_device_state.py` & `plugp100-3.4.0/plugp100/responses/hub_childs/t100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/hub_childs/t110_device_state.py` & `plugp100-3.4.0/plugp100/responses/hub_childs/t110_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/hub_childs/t31x_device_state.py` & `plugp100-3.4.0/plugp100/responses/hub_childs/t31x_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/hub_childs/trigger_log_response.py` & `plugp100-3.4.0/plugp100/responses/hub_childs/trigger_log_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/tapo_exception.py` & `plugp100-3.4.0/plugp100/responses/tapo_exception.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100/responses/tapo_response.py` & `plugp100-3.4.0/plugp100/responses/tapo_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.3.0/plugp100.egg-info/PKG-INFO` & `plugp100-3.4.0/plugp100.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.3.0
+Version: 3.4.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.3.0/plugp100.egg-info/SOURCES.txt` & `plugp100-3.4.0/plugp100.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements-test.txt
 requirements.txt
 setup.cfg
 setup.py
 plugp100/__init__.py
 plugp100/discover.py
 plugp100/example.py
 plugp100.egg-info/PKG-INFO
@@ -40,14 +41,16 @@
 plugp100/encryption/tp_link_cipher.py
 plugp100/requests/__init__.py
 plugp100/requests/handshake_params.py
 plugp100/requests/login_device.py
 plugp100/requests/secure_passthrough_params.py
 plugp100/requests/tapo_request.py
 plugp100/requests/trigger_logs_params.py
+plugp100/requests/internal/__init__.py
+plugp100/requests/internal/snowflake_id.py
 plugp100/requests/set_device_info/__init__.py
 plugp100/requests/set_device_info/play_alarm_params.py
 plugp100/requests/set_device_info/set_light_color_info_params.py
 plugp100/requests/set_device_info/set_light_info_params.py
 plugp100/requests/set_device_info/set_plug_info_params.py
 plugp100/responses/__init__.py
 plugp100/responses/alarm_type_list.py
```

### Comparing `plugp100-3.3.0/setup.py` & `plugp100-3.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     name='plugp100',
     version=get_version('plugp100/__init__.py'),
     install_requires=REQUIREMENTS,
     description='Controller for TP-Link Tapo P100 and other devices',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPL3',
-    packages=find_packages(),
+    packages=find_packages(exclude=("tests",)),
     author='@petretiandrea',
     author_email='petretiandrea@gmail.com',
     keywords=['Tapo', 'P100'],
     url='https://github.com/petretiandrea/plugp100',
     download_url='https://github.com/petretiandrea/plugp100',
     classifiers=[
         # 'Development Status :: 4 - Beta',
```

