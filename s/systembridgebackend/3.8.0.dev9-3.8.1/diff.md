# Comparing `tmp/systembridgebackend-3.8.0.dev9.tar.gz` & `tmp/systembridgebackend-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-3.8.0.dev9.tar", last modified: Tue Jul 18 14:36:15 2023, max compression
+gzip compressed data, was "systembridgebackend-3.8.1.tar", last modified: Mon Jul 31 14:18:45 2023, max compression
```

## Comparing `systembridgebackend-3.8.0.dev9.tar` & `systembridgebackend-3.8.1.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 14:36:12.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/remote_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/battery/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/battery/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/cpu/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/disk/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/display/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/gpu/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend/modules/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/memory/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/modules/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/network/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/modules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/sensors/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/modules/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/system/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22647 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43853 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.142630 systembridgebackend-3.8.1/systembridgebackend/utilities/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/remote_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-31 14:18:01.000000 systembridgebackend-3.8.1/systembridgebackend/utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:45.138630 systembridgebackend-3.8.1/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 14:18:45.000000 systembridgebackend-3.8.1/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-31 14:18:45.000000 systembridgebackend-3.8.1/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:18:45.000000 systembridgebackend-3.8.1/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 14:18:45.000000 systembridgebackend-3.8.1/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 14:18:45.000000 systembridgebackend-3.8.1/systembridgebackend.egg-info/top_level.txt
```

### Comparing `systembridgebackend-3.8.0.dev9/pyproject.toml` & `systembridgebackend-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/setup.py` & `systembridgebackend-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from systembridgeshared.database import Database
 from systembridgeshared.settings import Settings
 
 from .modules.listeners import Listeners
 from .modules.system import System
 from .server import Server
 from .utilities.autostart import autostart_disable, autostart_enable
-from .utilities.shortcuts import create_shortcuts
 
 
 class Application(Base):
     """Application"""
 
     def __init__(
         self,
@@ -41,16 +40,14 @@
             autostart = settings.get(SETTING_AUTOSTART)
             self._logger.info("Autostart enabled: %s", autostart)
             if autostart:
                 autostart_enable()
             else:
                 autostart_disable()
 
-            create_shortcuts()
-
         implemented_modules = []
         for _, dirs, _ in os.walk(os.path.join(os.path.dirname(__file__), "./modules")):
             implemented_modules = list(filter(lambda d: "__" not in d, dirs))
             break
 
         listeners = Listeners(database, implemented_modules)
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/__main__.py` & `systembridgebackend-3.8.1/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/gui.py` & `systembridgebackend-3.8.1/systembridgebackend/gui.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/icon.ico` & `systembridgebackend-3.8.1/systembridgebackend/icon.ico`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/icon.png` & `systembridgebackend-3.8.1/systembridgebackend/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/battery/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/battery/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/cpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/disk/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/display/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/display/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/gpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/listeners.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/network/update.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,52 @@
-"""System Bridge: Update Media"""
+"""System Bridge: Update Network"""
 import asyncio
 
 from systembridgeshared.database import Database
-from systembridgeshared.models.database_data import Media as DatabaseModel
+from systembridgeshared.models.database_data import Network as DatabaseModel
 
+from . import Network
 from ..base import ModuleUpdateBase
-from . import Media
 
 
-class MediaUpdate(ModuleUpdateBase):
-    """Media Update"""
+class NetworkUpdate(ModuleUpdateBase):
+    """Network Update"""
 
     def __init__(
         self,
         database: Database,
     ) -> None:
         """Initialize"""
         super().__init__(database)
-        self._media = Media()
+        self._network = Network()
 
-    async def update_media_info(self) -> None:
-        """Update media info"""
-        if media_info := await self._media.get_media_info():
-            for key, value in media_info.dict().items():
+    async def update_stats(self) -> None:
+        """Update stats"""
+        for key, value in self._network.stats().items():
+            for subkey, subvalue in value._asdict().items():
                 self._database.update_data(
                     DatabaseModel,
                     DatabaseModel(
-                        key=key,
-                        value=value,
+                        key=f"stat_{key.replace(' ', '')}_{subkey}",
+                        value=subvalue,
                     ),
                 )
 
+    async def update_io_counters(self) -> None:
+        """Update IO counters"""
+        for key, value in self._network.io_counters()._asdict().items():
+            self._database.update_data(
+                DatabaseModel,
+                DatabaseModel(
+                    key=f"io_counters_{key}",
+                    value=value,
+                ),
+            )
+
     async def update_all_data(self) -> None:
         """Update data"""
         await asyncio.gather(
             *[
-                self.update_media_info(),
+                self.update_stats(),
+                self.update_io_counters(),
             ]
         )
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/memory/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/network/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/sensors/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,19 @@
             with subprocess.Popen(
                 [path],
                 stdout=subprocess.PIPE,
             ) as pipe:
                 result = pipe.communicate()[0].decode()
             self._logger.debug("Windows sensors result: %s", result)
         except Exception as error:  # pylint: disable=broad-except
-            self._logger.error("Windows sensors error: %s", error)
+            self._logger.error(
+                "Windows sensors error: %s (%s)",
+                error,
+                path,
+            )
             return None
 
         try:
             return json.loads(result)
         except json.decoder.JSONDecodeError as error:
             self._logger.error(error)
             return None
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/sensors/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/system/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     def users(self) -> list[suser]:  # pylint: disable=unsubscriptable-object
         """Get users"""
         return users()
 
     def uuid(self) -> str:
         """Get UUID"""
-        return str(uuid.getnode())
+        return uniqueid.id or self.mac_address()
 
     def version(self) -> str:
         """Get version"""
         return __version__.public()
 
     async def version_latest(self) -> Optional[GitHubReleaseModel]:
         """Get latest version from GitHub"""
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/system/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/update.py` & `systembridgebackend-3.8.1/systembridgebackend/modules/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,75 +6,68 @@
 from systembridgeshared.database import Database
 
 from .battery.update import BatteryUpdate
 from .cpu.update import CPUUpdate
 from .disk.update import DiskUpdate
 from .display.update import DisplayUpdate
 from .gpu.update import GPUUpdate
-from .media.update import MediaUpdate
 from .memory.update import MemoryUpdate
 from .network.update import NetworkUpdate
 from .sensors.update import SensorsUpdate
 from .system.update import SystemUpdate
 
 
 class Update(Base):
     """Modules Update"""
 
     def __init__(
         self,
         database: Database,
+        updated_callback: Callable[[str], Awaitable[None]],
     ) -> None:
         """Initialize"""
         super().__init__()
         self._database = database  # pylint: disable=duplicate-code
+        self.updated_callback = updated_callback
 
         self._classes = [
             {"name": "battery", "cls": BatteryUpdate(self._database)},
             {"name": "disk", "cls": DiskUpdate(self._database)},
             {"name": "system", "cls": SystemUpdate(self._database)},
         ]
         self._classes_frequent = [
             {"name": "cpu", "cls": CPUUpdate(self._database)},
             {"name": "display", "cls": DisplayUpdate(self._database)},
             {"name": "gpu", "cls": GPUUpdate(self._database)},
-            {"name": "media", "cls": MediaUpdate(self._database)},
             {"name": "memory", "cls": MemoryUpdate(self._database)},
             {"name": "network", "cls": NetworkUpdate(self._database)},
         ]
 
     async def _update(
         self,
         class_obj: dict,
-        updated_callback: Callable[[str], Awaitable[None]],
     ) -> None:
         """Update"""
         await class_obj["cls"].update_all_data()
-        await updated_callback(class_obj["name"])
+        await self.updated_callback(class_obj["name"])
 
-    async def update_data(
-        self,
-        updated_callback: Callable[[str], Awaitable[None]],
-    ) -> None:
+    async def update_data(self) -> None:
         """Update Data"""
         self._logger.info("Update data")
 
-        tasks = [self._update(cls, updated_callback) for cls in self._classes]
+        tasks = [self._update(cls) for cls in self._classes]
         await asyncio.gather(*tasks)
 
         self._logger.info("Finished updating data")
 
-    async def update_frequent_data(
-        self,
-        updated_callback: Callable[[str], Awaitable[None]],
-    ) -> None:
+    async def update_frequent_data(self) -> None:
         """Update Data"""
         self._logger.info("Update frequent data")
 
         sensors_update = SensorsUpdate(self._database)
         await sensors_update.update_all_data()
-        await updated_callback("sensors")
+        await self.updated_callback("sensors")
 
-        tasks = [self._update(cls, updated_callback) for cls in self._classes_frequent]
+        tasks = [self._update(cls) for cls in self._classes_frequent]
         await asyncio.gather(*tasks)
 
         self._logger.info("Finished updating frequent data")
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/server/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,14 +108,18 @@
                     self.update_data(),
                     name="Update data",
                 ),
                 api_app.loop.create_task(
                     self.update_frequent_data(),
                     name="Update frequent data",
                 ),
+                api_app.loop.create_task(
+                    self.update_events_data(),
+                    name="Update events data",
+                ),
             ]
         )
         if not self.no_gui:
             self._gui = GUI(self._settings)
             self._tasks.extend(
                 [
                     api_app.loop.create_task(
@@ -221,14 +225,20 @@
         """Update data"""
         self._logger.info("Update data")
         self._data.request_update_data()
         self._logger.info("Schedule next update in 2 minutes")
         await asyncio.sleep(120)
         await self.update_data()
 
+    async def update_events_data(self) -> None:
+        """Update events data"""
+        self._logger.info("Update events data")
+        self._data.request_update_events_data()
+        asyncio.get_running_loop().run_forever()
+
     async def update_frequent_data(self) -> None:
         """Update frequent data"""
         self._logger.info("Update frequent data")
         self._data.request_update_frequent_data()
         self._logger.info("Schedule next frequent update in 30 seconds")
         await asyncio.sleep(30)
         await self.update_frequent_data()
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/server/api.py` & `systembridgebackend-3.8.1/systembridgebackend/server/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,27 +14,42 @@
 from systembridgeshared.common import asyncio_get_loop, convert_string_to_correct_type
 from systembridgeshared.const import HEADER_API_KEY, QUERY_API_KEY, SECRET_API_KEY
 from systembridgeshared.database import TABLE_MAP, Database
 from systembridgeshared.models.data import DataDict
 from systembridgeshared.models.database_data_remote_bridge import RemoteBridge
 from systembridgeshared.models.keyboard_key import KeyboardKey
 from systembridgeshared.models.keyboard_text import KeyboardText
+from systembridgeshared.models.media_control import Action as MediaAction
+from systembridgeshared.models.media_control import MediaControl
 from systembridgeshared.models.media_files import File as MediaFile
 from systembridgeshared.models.media_files import MediaFiles
 from systembridgeshared.models.media_play import MediaPlay
 from systembridgeshared.models.notification import Notification
 from systembridgeshared.models.open_path import OpenPath
 from systembridgeshared.models.open_url import OpenUrl
 from systembridgeshared.settings import Settings
 
 from .._version import __version__
 from ..gui import GUI
 from ..modules.listeners import Listeners
 from ..utilities.keyboard import keyboard_keypress, keyboard_text
 from ..utilities.media import (
+    control_fastforward,
+    control_mute,
+    control_next,
+    control_pause,
+    control_play,
+    control_previous,
+    control_repeat,
+    control_rewind,
+    control_seek,
+    control_shuffle,
+    control_stop,
+    control_volume_down,
+    control_volume_up,
     get_directories,
     get_file,
     get_file_data,
     get_files,
     play_media,
     write_file,
 )
@@ -225,14 +240,77 @@
         return {
             "message": "Text sent",
             **keyboard_event.dict(),
         }
     raise HTTPException(status.HTTP_400_BAD_REQUEST, detail="Invalid keyboard event")
 
 
+@app.post("/api/media/control", dependencies=[Depends(security_api_key)])
+async def send_media_control(
+    data: MediaControl,
+) -> dict[str, str]:
+    """Send media control."""
+    if data.action not in MediaAction:
+        raise HTTPException(
+            status.HTTP_400_BAD_REQUEST,
+            detail="Invalid media action",
+        )
+    if data.action == MediaAction.play:
+        await control_play()
+    elif data.action == MediaAction.pause:
+        await control_pause()
+    elif data.action == MediaAction.stop:
+        await control_stop()
+    elif data.action == MediaAction.previous:
+        await control_previous()
+    elif data.action == MediaAction.next:
+        await control_next()
+    elif data.action == MediaAction.seek:
+        if data.value is None:
+            raise HTTPException(
+                status.HTTP_400_BAD_REQUEST,
+                detail="Invalid seek value",
+            )
+        await control_seek(int(data.value))
+    elif data.action == MediaAction.rewind:
+        await control_rewind()
+    elif data.action == MediaAction.fastforward:
+        await control_fastforward()
+    elif data.action == MediaAction.shuffle:
+        if data.value is None:
+            raise HTTPException(
+                status.HTTP_400_BAD_REQUEST,
+                detail="Invalid shuffle value",
+            )
+        await control_shuffle(bool(data.value))
+    elif data.action == MediaAction.repeat:
+        if data.value is None:
+            raise HTTPException(
+                status.HTTP_400_BAD_REQUEST,
+                detail="Invalid repeat value",
+            )
+        await control_repeat(int(data.value))
+    elif data.action == MediaAction.mute:
+        await control_mute()
+    elif data.action == MediaAction.volumedown:
+        await control_volume_down()
+    elif data.action == MediaAction.volumeup:
+        await control_volume_up()
+    else:
+        raise HTTPException(
+            status.HTTP_400_BAD_REQUEST,
+            detail="Invalid media action",
+        )
+
+    return {
+        "message": "Media control sent",
+        **data.dict(),
+    }
+
+
 @app.get("/api/media", dependencies=[Depends(security_api_key)])
 def get_media_directories() -> dict[str, list[dict[str, str]]]:
     """Get media directories."""
     return {
         "directories": get_directories(settings),
     }
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/server/mdns.py` & `systembridgebackend-3.8.1/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/server/websocket.py` & `systembridgebackend-3.8.1/systembridgebackend/server/websocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,24 @@
     SETTING_AUTOSTART,
     SUBTYPE_BAD_API_KEY,
     SUBTYPE_BAD_DIRECTORY,
     SUBTYPE_BAD_FILE,
     SUBTYPE_BAD_JSON,
     SUBTYPE_BAD_PATH,
     SUBTYPE_BAD_REQUEST,
+    SUBTYPE_INVALID_ACTION,
     SUBTYPE_LISTENER_ALREADY_REGISTERED,
     SUBTYPE_LISTENER_NOT_REGISTERED,
+    SUBTYPE_MISSING_ACTION,
     SUBTYPE_MISSING_KEY,
     SUBTYPE_MISSING_MODULES,
     SUBTYPE_MISSING_PATH_URL,
     SUBTYPE_MISSING_TEXT,
     SUBTYPE_MISSING_TITLE,
+    SUBTYPE_MISSING_VALUE,
     SUBTYPE_UNKNOWN_EVENT,
     TYPE_APPLICATION_UPDATE,
     TYPE_APPLICATION_UPDATING,
     TYPE_DATA_GET,
     TYPE_DATA_LISTENER_REGISTERED,
     TYPE_DATA_LISTENER_UNREGISTERED,
     TYPE_DATA_UPDATE,
@@ -59,14 +62,15 @@
     TYPE_GET_REMOTE_BRIDGES_RESULT,
     TYPE_GET_SETTING,
     TYPE_GET_SETTINGS,
     TYPE_KEYBOARD_KEY_PRESSED,
     TYPE_KEYBOARD_KEYPRESS,
     TYPE_KEYBOARD_TEXT,
     TYPE_KEYBOARD_TEXT_SENT,
+    TYPE_MEDIA_CONTROL,
     TYPE_NOTIFICATION,
     TYPE_NOTIFICATION_SENT,
     TYPE_OPEN,
     TYPE_OPENED,
     TYPE_POWER_HIBERNATE,
     TYPE_POWER_HIBERNATING,
     TYPE_POWER_LOCK,
@@ -91,14 +95,16 @@
 from systembridgeshared.database import TABLE_MAP, Database
 from systembridgeshared.models.data import DataDict
 from systembridgeshared.models.database_data_remote_bridge import RemoteBridge
 from systembridgeshared.models.get_data import GetData
 from systembridgeshared.models.get_setting import GetSetting
 from systembridgeshared.models.keyboard_key import KeyboardKey
 from systembridgeshared.models.keyboard_text import KeyboardText
+from systembridgeshared.models.media_control import Action as MediaAction
+from systembridgeshared.models.media_control import MediaControl
 from systembridgeshared.models.media_get_file import MediaGetFile
 from systembridgeshared.models.media_get_files import MediaGetFiles
 from systembridgeshared.models.notification import Notification
 from systembridgeshared.models.open_path import OpenPath
 from systembridgeshared.models.open_url import OpenUrl
 from systembridgeshared.models.register_data_listener import RegisterDataListener
 from systembridgeshared.models.request import Request
@@ -107,15 +113,32 @@
 from systembridgeshared.models.update_setting import UpdateSetting
 from systembridgeshared.settings import SECRET_API_KEY, Settings
 from systembridgeshared.update import Update
 
 from ..modules.listeners import Listeners
 from ..utilities.autostart import autostart_disable, autostart_enable
 from ..utilities.keyboard import keyboard_keypress, keyboard_text
-from ..utilities.media import get_directories, get_file, get_files
+from ..utilities.media import (
+    control_fastforward,
+    control_mute,
+    control_next,
+    control_pause,
+    control_play,
+    control_previous,
+    control_repeat,
+    control_rewind,
+    control_seek,
+    control_shuffle,
+    control_stop,
+    control_volume_down,
+    control_volume_up,
+    get_directories,
+    get_file,
+    get_files,
+)
 from ..utilities.open import open_path, open_url
 from ..utilities.power import hibernate, lock, logout, restart, shutdown, sleep
 from ..utilities.remote_bridge import get_remote_bridges
 
 
 class WebSocketHandler(Base):
     """WebSocket handler"""
@@ -168,871 +191,1007 @@
                     EVENT_MESSAGE: "Data changed",
                     EVENT_MODULE: module,
                     EVENT_DATA: data,
                 }
             )
         )
 
-    async def _handler(
+    async def _handle_event(
         self,
         listener_id: str,
+        data: dict,
+        request: Request,
     ) -> None:
-        """Handler"""
-        # Loop until the connection is closed
-        while self._active:
+        """Handle event"""
+        if request.event == TYPE_APPLICATION_UPDATE:
             try:
-                data = await self._websocket.receive_json()
-                request = Request(**data)
-            except JSONDecodeError as error:
-                message = f"Invalid JSON: {error}"
-                self._logger.error(message)
+                model = UpdateModel(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
+                            EVENT_ID: request.id,
                             EVENT_TYPE: TYPE_ERROR,
-                            EVENT_SUBTYPE: SUBTYPE_BAD_JSON,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
                             EVENT_MESSAGE: message,
                         }
                     )
                 )
-                continue
+                return
+            versions = Update().update(
+                model.version,
+                wait=False,
+            )
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_APPLICATION_UPDATING,
+                        EVENT_MESSAGE: "Updating application",
+                        EVENT_VERSIONS: versions,
+                    }
+                )
+            )
+        elif request.event == TYPE_EXIT_APPLICATION:
+            self._callback_exit_application()
+            self._logger.info("Exit application called")
+        elif request.event == TYPE_KEYBOARD_KEYPRESS:
+            try:
+                model = KeyboardKey(**data)
             except ValueError as error:
                 message = f"Invalid request: {error}"
-                self._logger.error(message)
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
+                            EVENT_ID: request.id,
                             EVENT_TYPE: TYPE_ERROR,
                             EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
                             EVENT_MESSAGE: message,
                         }
                     )
                 )
-                continue
+                return
+            if model.key is None:
+                self._logger.warning("No key provided")
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_KEY,
+                            EVENT_MESSAGE: "No key provided",
+                        }
+                    )
+                )
+                return
 
-            self._logger.info("Received: %s", request.event)
+            try:
+                keyboard_keypress(model.key)
+            except ValueError as err:
+                self._logger.warning(err.args[0])
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_KEY,
+                            EVENT_MESSAGE: "Invalid key",
+                        }
+                    )
+                )
+                return
 
-            api_key = self._settings.get_secret(SECRET_API_KEY)
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_KEYBOARD_KEY_PRESSED,
+                        EVENT_MESSAGE: "Key pressed",
+                        EVENT_ID: listener_id,
+                        "key": model.key,
+                    }
+                )
+            )
+        elif request.event == TYPE_KEYBOARD_TEXT:
+            try:
+                model = KeyboardText(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
+                        }
+                    )
+                )
+                return
+            if model.text is None:
+                self._logger.warning("No text provided")
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_TEXT,
+                            EVENT_MESSAGE: "No text provided",
+                        }
+                    )
+                )
+                return
 
-            if request.api_key != api_key:
-                self._logger.warning(
-                    "Invalid api-key: %s != %s",
-                    request.api_key,
-                    api_key,
+            keyboard_text(model.text)
+
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_KEYBOARD_TEXT_SENT,
+                        EVENT_MESSAGE: "Key pressed",
+                        EVENT_ID: listener_id,
+                        "text": model.text,
+                    }
                 )
+            )
+        elif request.event == TYPE_MEDIA_CONTROL:
+            try:
+                model = MediaControl(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
                             EVENT_TYPE: TYPE_ERROR,
-                            EVENT_SUBTYPE: SUBTYPE_BAD_API_KEY,
-                            EVENT_MESSAGE: "Invalid api-key",
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-                continue
-            if request.event == TYPE_APPLICATION_UPDATE:
-                try:
-                    model = UpdateModel(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
+                return
+            if model.action is None:
+                self._logger.warning("No action provided")
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_ACTION,
+                            EVENT_MESSAGE: "No action provided",
+                        }
                     )
-                    continue
-                versions = Update().update(
-                    model.version,
-                    wait=False,
                 )
+                return
+            if model.action not in MediaAction:
+                self._logger.warning("Invalid action provided")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_APPLICATION_UPDATING,
-                            EVENT_MESSAGE: "Updating application",
-                            EVENT_VERSIONS: versions,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_INVALID_ACTION,
+                            EVENT_MESSAGE: "Invalid action provided",
                         }
                     )
                 )
-            elif request.event == TYPE_EXIT_APPLICATION:
-                self._callback_exit_application()
-                self._logger.info("Exit application called")
-            elif request.event == TYPE_KEYBOARD_KEYPRESS:
-                try:
-                    model = KeyboardKey(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
+                return
+            if model.action == MediaAction.play:
+                await control_play()
+            elif model.action == MediaAction.pause:
+                await control_pause()
+            elif model.action == MediaAction.stop:
+                await control_stop()
+            elif model.action == MediaAction.previous:
+                await control_previous()
+            elif model.action == MediaAction.next:
+                await control_next()
+            elif model.action == MediaAction.seek:
+                if model.value is None:
+                    self._logger.warning("No position value provided")
                     await self._send_response(
                         Response(
                             **{
                                 EVENT_ID: request.id,
                                 EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
+                                EVENT_SUBTYPE: SUBTYPE_MISSING_VALUE,
+                                EVENT_MESSAGE: "No value provided",
                             }
                         )
                     )
-                    continue
-                if model.key is None:
-                    self._logger.warning("No key provided")
+                    return
+                await control_seek(int(model.value))
+            elif model.action == MediaAction.rewind:
+                await control_rewind()
+            elif model.action == MediaAction.fastforward:
+                await control_fastforward()
+            elif model.action == MediaAction.shuffle:
+                if model.value is None:
+                    self._logger.warning("No shuffle value provided")
                     await self._send_response(
                         Response(
                             **{
                                 EVENT_ID: request.id,
                                 EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_MISSING_KEY,
-                                EVENT_MESSAGE: "No key provided",
+                                EVENT_SUBTYPE: SUBTYPE_MISSING_VALUE,
+                                EVENT_MESSAGE: "No value provided",
                             }
                         )
                     )
-                    continue
-
-                try:
-                    keyboard_keypress(model.key)
-                except ValueError as err:
-                    self._logger.warning(err.args[0])
+                    return
+                await control_shuffle(bool(model.value))
+            elif model.action == MediaAction.repeat:
+                if model.value is None:
+                    self._logger.warning("No repeat value provided")
                     await self._send_response(
                         Response(
                             **{
                                 EVENT_ID: request.id,
                                 EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_MISSING_KEY,
-                                EVENT_MESSAGE: "Invalid key",
+                                EVENT_SUBTYPE: SUBTYPE_MISSING_VALUE,
+                                EVENT_MESSAGE: "No value provided",
                             }
                         )
                     )
-                    continue
+                    return
+                await control_repeat(int(model.value))
+            elif model.action == MediaAction.mute:
+                await control_mute()
+            elif model.action == MediaAction.volumedown:
+                await control_volume_down()
+            elif model.action == MediaAction.volumeup:
+                await control_volume_up()
 
+        elif request.event == TYPE_NOTIFICATION:
+            try:
+                model = Notification(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
+                        }
+                    )
+                )
+                return
+            if model.title is None:
+                self._logger.warning("No title provided")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_KEYBOARD_KEY_PRESSED,
-                            EVENT_MESSAGE: "Key pressed",
-                            EVENT_ID: listener_id,
-                            "key": model.key,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_TITLE,
+                            EVENT_MESSAGE: "No title provided",
                         }
                     )
                 )
-            elif request.event == TYPE_KEYBOARD_TEXT:
+                return
+
+            self._callback_open_gui("notification", model.json())
+
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_NOTIFICATION_SENT,
+                        EVENT_MESSAGE: "Notification sent",
+                    }
+                )
+            )
+        elif request.event == TYPE_OPEN:
+            if "path" in data:
                 try:
-                    model = KeyboardText(**data)
+                    model = OpenPath(**data)
                 except ValueError as error:
                     message = f"Invalid request: {error}"
                     self._logger.warning(message)
                     await self._send_response(
                         Response(
                             **{
                                 EVENT_ID: request.id,
                                 EVENT_TYPE: TYPE_ERROR,
                                 EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
                                 EVENT_MESSAGE: message,
                             }
                         )
                     )
-                    continue
-                if model.text is None:
-                    self._logger.warning("No text provided")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_MISSING_TEXT,
-                                EVENT_MESSAGE: "No text provided",
-                            }
-                        )
-                    )
-                    continue
-
-                keyboard_text(model.text)
-
+                    return
+                open_path(model.path)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_KEYBOARD_TEXT_SENT,
-                            EVENT_MESSAGE: "Key pressed",
-                            EVENT_ID: listener_id,
-                            "text": model.text,
+                            EVENT_TYPE: TYPE_OPENED,
+                            EVENT_MESSAGE: "Path opened",
+                            EVENT_PATH: model.path,
                         }
                     )
                 )
-            elif request.event == TYPE_NOTIFICATION:
+                return
+            if "url" in data:
                 try:
-                    model = Notification(**data)
+                    model = OpenUrl(**data)
                 except ValueError as error:
                     message = f"Invalid request: {error}"
                     self._logger.warning(message)
                     await self._send_response(
                         Response(
                             **{
                                 EVENT_ID: request.id,
                                 EVENT_TYPE: TYPE_ERROR,
                                 EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
                                 EVENT_MESSAGE: message,
                             }
                         )
                     )
-                    continue
-                if model.title is None:
-                    self._logger.warning("No title provided")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_MISSING_TITLE,
-                                EVENT_MESSAGE: "No title provided",
-                            }
-                        )
-                    )
-                    continue
-
-                self._callback_open_gui("notification", model.json())
-
+                    return
+                open_url(model.url)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_NOTIFICATION_SENT,
-                            EVENT_MESSAGE: "Notification sent",
+                            EVENT_TYPE: TYPE_OPENED,
+                            EVENT_MESSAGE: "URL opened",
+                            EVENT_URL: model.url,
                         }
                     )
                 )
-            elif request.event == TYPE_OPEN:
-                if "path" in data:
-                    try:
-                        model = OpenPath(**data)
-                    except ValueError as error:
-                        message = f"Invalid request: {error}"
-                        self._logger.warning(message)
-                        await self._send_response(
-                            Response(
-                                **{
-                                    EVENT_ID: request.id,
-                                    EVENT_TYPE: TYPE_ERROR,
-                                    EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                    EVENT_MESSAGE: message,
-                                }
-                            )
-                        )
-                        continue
-                    open_path(model.path)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_OPENED,
-                                EVENT_MESSAGE: "Path opened",
-                                EVENT_PATH: model.path,
-                            }
-                        )
-                    )
-                    continue
-                if "url" in data:
-                    try:
-                        model = OpenUrl(**data)
-                    except ValueError as error:
-                        message = f"Invalid request: {error}"
-                        self._logger.warning(message)
-                        await self._send_response(
-                            Response(
-                                **{
-                                    EVENT_ID: request.id,
-                                    EVENT_TYPE: TYPE_ERROR,
-                                    EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                    EVENT_MESSAGE: message,
-                                }
-                            )
-                        )
-                        continue
-                    open_url(model.url)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_OPENED,
-                                EVENT_MESSAGE: "URL opened",
-                                EVENT_URL: model.url,
-                            }
-                        )
-                    )
-                    continue
+                return
 
-                self._logger.warning("No path or url provided")
+            self._logger.warning("No path or url provided")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_ERROR,
+                        EVENT_SUBTYPE: SUBTYPE_MISSING_PATH_URL,
+                        EVENT_MESSAGE: "No path or url provided",
+                    }
+                )
+            )
+        elif request.event == TYPE_REGISTER_DATA_LISTENER:
+            try:
+                model = RegisterDataListener(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
                             EVENT_TYPE: TYPE_ERROR,
-                            EVENT_SUBTYPE: SUBTYPE_MISSING_PATH_URL,
-                            EVENT_MESSAGE: "No path or url provided",
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-            elif request.event == TYPE_REGISTER_DATA_LISTENER:
-                try:
-                    model = RegisterDataListener(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
-                if model.modules is None or len(model.modules) == 0:
-                    self._logger.warning("No modules provided")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_MISSING_MODULES,
-                                EVENT_MESSAGE: "No modules provided",
-                            }
-                        )
+                return
+            if model.modules is None or len(model.modules) == 0:
+                self._logger.warning("No modules provided")
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_MODULES,
+                            EVENT_MESSAGE: "No modules provided",
+                        }
                     )
-                    continue
-
-                self._logger.info(
-                    "Registering data listener: %s - %s",
-                    listener_id,
-                    model.modules,
                 )
+                return
 
-                if await self._listeners.add_listener(
-                    listener_id,
-                    self._data_changed,
-                    model.modules,
-                ):
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_LISTENER_ALREADY_REGISTERED,
-                                EVENT_MESSAGE: "Listener already registered with this connection",
-                                EVENT_MODULES: model.modules,
-                            }
-                        )
-                    )
-                    continue
+            self._logger.info(
+                "Registering data listener: %s - %s",
+                listener_id,
+                model.modules,
+            )
 
+            if await self._listeners.add_listener(
+                listener_id,
+                self._data_changed,
+                model.modules,
+            ):
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_DATA_LISTENER_REGISTERED,
-                            EVENT_MESSAGE: "Data listener registered",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_LISTENER_ALREADY_REGISTERED,
+                            EVENT_MESSAGE: "Listener already registered with this connection",
                             EVENT_MODULES: model.modules,
                         }
                     )
                 )
-            elif request.event == TYPE_UNREGISTER_DATA_LISTENER:
-                self._logger.info("Unregistering data listener %s", listener_id)
+                return
 
-                if not self._listeners.remove_listener(listener_id):
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_LISTENER_NOT_REGISTERED,
-                                EVENT_MESSAGE: "Listener not registered with this connection",
-                            }
-                        )
-                    )
-                    continue
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_DATA_LISTENER_REGISTERED,
+                        EVENT_MESSAGE: "Data listener registered",
+                        EVENT_MODULES: model.modules,
+                    }
+                )
+            )
+        elif request.event == TYPE_UNREGISTER_DATA_LISTENER:
+            self._logger.info("Unregistering data listener %s", listener_id)
 
+            if not self._listeners.remove_listener(listener_id):
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_DATA_LISTENER_UNREGISTERED,
-                            EVENT_MESSAGE: "Data listener unregistered",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_LISTENER_NOT_REGISTERED,
+                            EVENT_MESSAGE: "Listener not registered with this connection",
                         }
                     )
                 )
-            elif request.event == TYPE_GET_DATA:
-                try:
-                    model = GetData(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
-                if model.modules is None or len(model.modules) == 0:
-                    self._logger.warning("No modules provided")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_MISSING_MODULES,
-                                EVENT_MESSAGE: "No modules provided",
-                            }
-                        )
-                    )
-                    continue
-                self._logger.info("Getting data: %s", model.modules)
+                return
 
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_DATA_LISTENER_UNREGISTERED,
+                        EVENT_MESSAGE: "Data listener unregistered",
+                    }
+                )
+            )
+        elif request.event == TYPE_GET_DATA:
+            try:
+                model = GetData(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_DATA_GET,
-                            EVENT_MESSAGE: "Getting data",
-                            EVENT_MODULES: model.modules,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-
-                for module in model.modules:
-                    table = TABLE_MAP.get(module)
-                    data = self._database.get_data_dict(table)
-                    if data is not None:
-                        await self._send_response(
-                            Response(
-                                **{
-                                    EVENT_ID: request.id,
-                                    EVENT_TYPE: TYPE_DATA_UPDATE,
-                                    EVENT_MESSAGE: "Data received",
-                                    EVENT_MODULE: module,
-                                    EVENT_DATA: data,
-                                }
-                            )
-                        )
-            elif request.event == TYPE_GET_DIRECTORIES:
+                return
+            if model.modules is None or len(model.modules) == 0:
+                self._logger.warning("No modules provided")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_DIRECTORIES,
-                            EVENT_DIRECTORIES: get_directories(self._settings),
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_MISSING_MODULES,
+                            EVENT_MESSAGE: "No modules provided",
                         }
                     )
                 )
-            elif request.event == TYPE_GET_FILES:
-                try:
-                    model = MediaGetFiles(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
-
-                root_path = None
-                for item in get_directories(self._settings):
-                    if item["key"] == model.base:
-                        root_path = item["path"]
-                        break
-
-                if root_path is None or not os.path.exists(root_path):
-                    self._logger.warning("Cannot find base path")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
-                                EVENT_MESSAGE: "Cannot find base path",
-                                EVENT_BASE: model.base,
-                            }
-                        )
-                    )
-                    continue
-
-                path = (
-                    os.path.join(root_path, model.path)
-                    if model.path is not None
-                    else root_path
-                )
+                return
+            self._logger.info("Getting data: %s", model.modules)
 
-                self._logger.info(
-                    "Getting files: %s - %s - %s",
-                    model.base,
-                    model.path,
-                    path,
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_DATA_GET,
+                        EVENT_MESSAGE: "Getting data",
+                        EVENT_MODULES: model.modules,
+                    }
                 )
+            )
 
-                if not os.path.exists(path):
-                    self._logger.warning("Cannot find path")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
-                                EVENT_MESSAGE: "Cannot find path",
-                                EVENT_PATH: path,
-                            }
-                        )
-                    )
-                    continue
-                if not os.path.isdir(path):
-                    self._logger.warning("Path is not a directory")
+            for module in model.modules:
+                table = TABLE_MAP.get(module)
+                data = self._database.get_data_dict(table)
+                if data is not None:
                     await self._send_response(
                         Response(
                             **{
                                 EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_DIRECTORY,
-                                EVENT_MESSAGE: "Path is not a directory",
-                                EVENT_PATH: path,
+                                EVENT_TYPE: TYPE_DATA_UPDATE,
+                                EVENT_MESSAGE: "Data received",
+                                EVENT_MODULE: module,
+                                EVENT_DATA: data,
                             }
                         )
                     )
-                    continue
-
+        elif request.event == TYPE_GET_DIRECTORIES:
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_DIRECTORIES,
+                        EVENT_DIRECTORIES: get_directories(self._settings),
+                    }
+                )
+            )
+        elif request.event == TYPE_GET_FILES:
+            try:
+                model = MediaGetFiles(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_FILES,
-                            EVENT_FILES: get_files(self._settings, model.base, path),
-                            EVENT_PATH: path,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-            elif request.event == TYPE_GET_FILE:
-                try:
-                    model = MediaGetFile(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
+                return
 
-                root_path = None
-                for item in get_directories(self._settings):
-                    if item["key"] == model.base:
-                        root_path = item["path"]
-                        break
+            root_path = None
+            for item in get_directories(self._settings):
+                if item["key"] == model.base:
+                    root_path = item["path"]
+                    break
 
-                if root_path is None or not os.path.exists(root_path):
-                    self._logger.warning("Cannot find base path")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
-                                EVENT_MESSAGE: "Cannot find base path",
-                                EVENT_BASE: model.base,
-                            }
-                        )
+            if root_path is None or not os.path.exists(root_path):
+                self._logger.warning("Cannot find base path")
+                await self._send_response(
+                    Response(
+                        **{
+                            EVENT_ID: request.id,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
+                            EVENT_MESSAGE: "Cannot find base path",
+                            EVENT_BASE: model.base,
+                        }
                     )
-                    continue
-
-                path = os.path.join(root_path, model.path)
-
-                self._logger.info(
-                    "Getting file: %s - %s - %s",
-                    model.base,
-                    model.path,
-                    path,
                 )
+                return
 
-                if not os.path.exists(path):
-                    self._logger.warning("Cannot find path")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
-                                EVENT_MESSAGE: "Cannot find path",
-                                EVENT_PATH: path,
-                            }
-                        )
-                    )
-                    continue
-                if not os.path.isfile(path):
-                    self._logger.warning("Path is not a file")
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_FILE,
-                                EVENT_MESSAGE: "Path is not a file",
-                                EVENT_PATH: path,
-                            }
-                        )
-                    )
-                    continue
+            path = (
+                os.path.join(root_path, model.path)
+                if model.path is not None
+                else root_path
+            )
 
+            self._logger.info(
+                "Getting files: %s - %s - %s",
+                model.base,
+                model.path,
+                path,
+            )
+
+            if not os.path.exists(path):
+                self._logger.warning("Cannot find path")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_FILE,
-                            EVENT_FILE: get_file(root_path, path),
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
+                            EVENT_MESSAGE: "Cannot find path",
                             EVENT_PATH: path,
                         }
                     )
                 )
-            elif request.event == TYPE_GET_SETTINGS:
-                self._logger.info("Getting settings")
+                return
+            if not os.path.isdir(path):
+                self._logger.warning("Path is not a directory")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_SETTINGS_RESULT,
-                            EVENT_MESSAGE: "Got settings",
-                            EVENT_DATA: self._settings.get_all(),
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_DIRECTORY,
+                            EVENT_MESSAGE: "Path is not a directory",
+                            EVENT_PATH: path,
                         }
                     )
                 )
-            elif request.event == TYPE_GET_SETTING:
-                try:
-                    model = GetSetting(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
-
-                self._logger.info("Getting setting: %s", model.setting)
+                return
 
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_FILES,
+                        EVENT_FILES: get_files(self._settings, model.base, path),
+                        EVENT_PATH: path,
+                    }
+                )
+            )
+        elif request.event == TYPE_GET_FILE:
+            try:
+                model = MediaGetFile(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_SETTING_RESULT,
-                            EVENT_MESSAGE: "Got setting",
-                            EVENT_SETTING: model.setting,
-                            EVENT_DATA: self._settings.get(model.setting),
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-            elif request.event == TYPE_GET_REMOTE_BRIDGES:
-                self._logger.info("Getting remote bridges")
+                return
+
+            root_path = None
+            for item in get_directories(self._settings):
+                if item["key"] == model.base:
+                    root_path = item["path"]
+                    break
+
+            if root_path is None or not os.path.exists(root_path):
+                self._logger.warning("Cannot find base path")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_GET_REMOTE_BRIDGES_RESULT,
-                            EVENT_MESSAGE: "Got remote bridges",
-                            EVENT_DATA: get_remote_bridges(self._database),
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
+                            EVENT_MESSAGE: "Cannot find base path",
+                            EVENT_BASE: model.base,
                         }
                     )
                 )
-            elif request.event == TYPE_UPDATE_REMOTE_BRIDGE:
-                try:
-                    model = RemoteBridge(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
+                return
 
-                self._logger.info("Remote bridge: %s", model)
+            path = os.path.join(root_path, model.path)
 
-                model = self._database.update_remote_bridge(model)
+            self._logger.info(
+                "Getting file: %s - %s - %s",
+                model.base,
+                model.path,
+                path,
+            )
 
+            if not os.path.exists(path):
+                self._logger.warning("Cannot find path")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_UPDATE_REMOTE_BRIDGE_RESULT,
-                            EVENT_MESSAGE: "Data updated",
-                            EVENT_DATA: model,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_PATH,
+                            EVENT_MESSAGE: "Cannot find path",
+                            EVENT_PATH: path,
                         }
                     )
                 )
-            elif request.event == TYPE_UPDATE_SETTING:
-                try:
-                    model = UpdateSetting(**data)
-                except ValueError as error:
-                    message = f"Invalid request: {error}"
-                    self._logger.warning(message)
-                    await self._send_response(
-                        Response(
-                            **{
-                                EVENT_ID: request.id,
-                                EVENT_TYPE: TYPE_ERROR,
-                                EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
-                                EVENT_MESSAGE: message,
-                            }
-                        )
-                    )
-                    continue
-
-                self._logger.info(
-                    "Setting setting %s to: %s",
-                    model.setting,
-                    model.value,
-                )
-
-                self._settings.set(model.setting, model.value)
-
+                return
+            if not os.path.isfile(path):
+                self._logger.warning("Path is not a file")
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_SETTING_UPDATED,
-                            EVENT_MESSAGE: "Setting updated",
-                            EVENT_SETTING: model.setting,
-                            EVENT_VALUE: model.value,
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_FILE,
+                            EVENT_MESSAGE: "Path is not a file",
+                            EVENT_PATH: path,
                         }
                     )
                 )
+                return
 
-                if model.setting != SETTING_AUTOSTART:
-                    continue
-                self._logger.info("Setting autostart to %s", model.value)
-                if model.value is True:
-                    autostart_enable()
-                else:
-                    autostart_disable()
-            elif request.event == TYPE_POWER_SLEEP:
-                self._logger.info("Sleeping")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_FILE,
+                        EVENT_FILE: get_file(root_path, path),
+                        EVENT_PATH: path,
+                    }
+                )
+            )
+        elif request.event == TYPE_GET_SETTINGS:
+            self._logger.info("Getting settings")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_SETTINGS_RESULT,
+                        EVENT_MESSAGE: "Got settings",
+                        EVENT_DATA: self._settings.get_all(),
+                    }
+                )
+            )
+        elif request.event == TYPE_GET_SETTING:
+            try:
+                model = GetSetting(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_POWER_SLEEPING,
-                            EVENT_MESSAGE: "Sleeping",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-                sleep()
-            elif request.event == TYPE_POWER_HIBERNATE:
-                self._logger.info("Sleeping")
+                return
+
+            self._logger.info("Getting setting: %s", model.setting)
+
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_SETTING_RESULT,
+                        EVENT_MESSAGE: "Got setting",
+                        EVENT_SETTING: model.setting,
+                        EVENT_DATA: self._settings.get(model.setting),
+                    }
+                )
+            )
+        elif request.event == TYPE_GET_REMOTE_BRIDGES:
+            self._logger.info("Getting remote bridges")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_GET_REMOTE_BRIDGES_RESULT,
+                        EVENT_MESSAGE: "Got remote bridges",
+                        EVENT_DATA: get_remote_bridges(self._database),
+                    }
+                )
+            )
+        elif request.event == TYPE_UPDATE_REMOTE_BRIDGE:
+            try:
+                model = RemoteBridge(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_POWER_HIBERNATING,
-                            EVENT_MESSAGE: "Hiibernating",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-                hibernate()
-            elif request.event == TYPE_POWER_RESTART:
-                self._logger.info("Sleeping")
+                return
+
+            self._logger.info("Remote bridge: %s", model)
+
+            model = self._database.update_remote_bridge(model)
+
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_UPDATE_REMOTE_BRIDGE_RESULT,
+                        EVENT_MESSAGE: "Data updated",
+                        EVENT_DATA: model,
+                    }
+                )
+            )
+        elif request.event == TYPE_UPDATE_SETTING:
+            try:
+                model = UpdateSetting(**data)
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.warning(message)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_POWER_RESTARTING,
-                            EVENT_MESSAGE: "Restarting",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-                restart()
-            elif request.event == TYPE_POWER_SHUTDOWN:
-                self._logger.info("Sleeping")
+                return
+
+            self._logger.info(
+                "Setting setting %s to: %s",
+                model.setting,
+                model.value,
+            )
+
+            self._settings.set(model.setting, model.value)
+
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_SETTING_UPDATED,
+                        EVENT_MESSAGE: "Setting updated",
+                        EVENT_SETTING: model.setting,
+                        EVENT_VALUE: model.value,
+                    }
+                )
+            )
+
+            if model.setting != SETTING_AUTOSTART:
+                return
+            self._logger.info("Setting autostart to %s", model.value)
+            if model.value is True:
+                autostart_enable()
+            else:
+                autostart_disable()
+        elif request.event == TYPE_POWER_SLEEP:
+            self._logger.info("Sleeping")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_POWER_SLEEPING,
+                        EVENT_MESSAGE: "Sleeping",
+                    }
+                )
+            )
+            sleep()
+        elif request.event == TYPE_POWER_HIBERNATE:
+            self._logger.info("Sleeping")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_POWER_HIBERNATING,
+                        EVENT_MESSAGE: "Hiibernating",
+                    }
+                )
+            )
+            hibernate()
+        elif request.event == TYPE_POWER_RESTART:
+            self._logger.info("Sleeping")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_POWER_RESTARTING,
+                        EVENT_MESSAGE: "Restarting",
+                    }
+                )
+            )
+            restart()
+        elif request.event == TYPE_POWER_SHUTDOWN:
+            self._logger.info("Sleeping")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_POWER_SHUTTINGDOWN,
+                        EVENT_MESSAGE: "Shutting down",
+                    }
+                )
+            )
+            shutdown()
+        elif request.event == TYPE_POWER_LOCK:
+            self._logger.info("Locking")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_POWER_LOCKING,
+                        EVENT_MESSAGE: "Locking",
+                    }
+                )
+            )
+            lock()
+        elif request.event == TYPE_POWER_LOGOUT:
+            self._logger.info("Logging out")
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_POWER_LOGGINGOUT,
+                        EVENT_MESSAGE: "Logging out",
+                    }
+                )
+            )
+            logout()
+        else:
+            self._logger.warning("Unknown event: %s", request.event)
+            await self._send_response(
+                Response(
+                    **{
+                        EVENT_ID: request.id,
+                        EVENT_TYPE: TYPE_ERROR,
+                        EVENT_SUBTYPE: SUBTYPE_UNKNOWN_EVENT,
+                        EVENT_MESSAGE: "Unknown event",
+                        EVENT_EVENT: request.event,
+                    }
+                )
+            )
+
+    async def _handler(
+        self,
+        listener_id: str,
+    ) -> None:
+        """Handler"""
+        # Loop until the connection is closed
+        while self._active:
+            try:
+                data = await self._websocket.receive_json()
+                request = Request(**data)
+            except JSONDecodeError as error:
+                message = f"Invalid JSON: {error}"
+                self._logger.error(message)
                 await self._send_response(
                     Response(
                         **{
-                            EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_POWER_SHUTTINGDOWN,
-                            EVENT_MESSAGE: "Shutting down",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_JSON,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-                shutdown()
-            elif request.event == TYPE_POWER_LOCK:
-                self._logger.info("Locking")
+                return
+            except ValueError as error:
+                message = f"Invalid request: {error}"
+                self._logger.error(message)
                 await self._send_response(
                     Response(
                         **{
-                            EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_POWER_LOCKING,
-                            EVENT_MESSAGE: "Locking",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_REQUEST,
+                            EVENT_MESSAGE: message,
                         }
                     )
                 )
-                lock()
-            elif request.event == TYPE_POWER_LOGOUT:
-                self._logger.info("Logging out")
+                return
+
+            self._logger.info("Received: %s", request.event)
+
+            api_key = self._settings.get_secret(SECRET_API_KEY)
+
+            if request.api_key != api_key:
+                self._logger.warning(
+                    "Invalid api-key: %s != %s",
+                    request.api_key,
+                    api_key,
+                )
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
-                            EVENT_TYPE: TYPE_POWER_LOGGINGOUT,
-                            EVENT_MESSAGE: "Logging out",
+                            EVENT_TYPE: TYPE_ERROR,
+                            EVENT_SUBTYPE: SUBTYPE_BAD_API_KEY,
+                            EVENT_MESSAGE: "Invalid api-key",
                         }
                     )
                 )
-                logout()
-            else:
-                self._logger.warning("Unknown event: %s", request.event)
+                return
+
+            try:
+                await self._handle_event(
+                    listener_id,
+                    data,
+                    request,
+                )
+            except Exception as error:  # pylint: disable=broad-except
+                self._logger.error(error)
                 await self._send_response(
                     Response(
                         **{
                             EVENT_ID: request.id,
                             EVENT_TYPE: TYPE_ERROR,
                             EVENT_SUBTYPE: SUBTYPE_UNKNOWN_EVENT,
-                            EVENT_MESSAGE: "Unknown event",
-                            EVENT_EVENT: request.event,
+                            EVENT_MESSAGE: str(error),
                         }
                     )
                 )
 
     async def handler(self) -> None:
         """Handler"""
         listener_id = str(uuid4())
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/action.py` & `systembridgebackend-3.8.1/systembridgebackend/utilities/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/__init__.py` & `systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/linux.py` & `systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/linux.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 
 desktop_entry = f"""
 [Desktop Entry]
 Name=System Bridge
 Comment=System Bridge
-Exec={sys.executable} -m systembridgebackend
+Exec={'{sys.executable} -m systembridgebackend' if 'python' in sys.executable else sys.executable} --silent
 Icon={os.path.join(os.path.dirname(__file__),'../../icon.png')}
 Terminal=false
 Type=Application
 Categories=Application;
 """
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/windows.py` & `systembridgebackend-3.8.1/systembridgebackend/utilities/autostart/windows.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,10 +49,12 @@
         access=KEY_ALL_ACCESS,
     )
     SetValueEx(
         key,
         "systembridgebackend",
         0,
         REG_SZ,
-        f'"{os.path.join(os.path.dirname(sys.executable), "pythonw.exe")}" -m systembridgebackend --silent',
+        f'"{os.path.join(os.path.dirname(sys.executable), "pythonw.exe")}" -m systembridgebackend --silent'
+        if "python" in sys.executable
+        else f'"{sys.executable}" --silent',
     )
     CloseKey(key)
```

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/keyboard.py` & `systembridgebackend-3.8.1/systembridgebackend/utilities/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/power.py` & `systembridgebackend-3.8.1/systembridgebackend/utilities/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-3.8.1/systembridgebackend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 systembridgebackend/modules/disk/__init__.py
 systembridgebackend/modules/disk/update.py
 systembridgebackend/modules/display/__init__.py
 systembridgebackend/modules/display/update.py
 systembridgebackend/modules/gpu/__init__.py
 systembridgebackend/modules/gpu/update.py
 systembridgebackend/modules/media/__init__.py
-systembridgebackend/modules/media/update.py
 systembridgebackend/modules/memory/__init__.py
 systembridgebackend/modules/memory/update.py
 systembridgebackend/modules/network/__init__.py
 systembridgebackend/modules/network/update.py
 systembridgebackend/modules/sensors/__init__.py
 systembridgebackend/modules/sensors/update.py
 systembridgebackend/modules/system/__init__.py
@@ -39,18 +38,16 @@
 systembridgebackend/server/__init__.py
 systembridgebackend/server/api.py
 systembridgebackend/server/mdns.py
 systembridgebackend/server/websocket.py
 systembridgebackend/utilities/__init__.py
 systembridgebackend/utilities/action.py
 systembridgebackend/utilities/keyboard.py
-systembridgebackend/utilities/media.py
 systembridgebackend/utilities/open.py
 systembridgebackend/utilities/power.py
 systembridgebackend/utilities/remote_bridge.py
 systembridgebackend/utilities/update.py
 systembridgebackend/utilities/autostart/__init__.py
 systembridgebackend/utilities/autostart/linux.py
 systembridgebackend/utilities/autostart/windows.py
-systembridgebackend/utilities/shortcuts/__init__.py
-systembridgebackend/utilities/shortcuts/linux.py
-systembridgebackend/utilities/shortcuts/windows.py
+systembridgebackend/utilities/media/__init__.py
+systembridgebackend/utilities/media/windows.py
```

