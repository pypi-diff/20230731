# Comparing `tmp/pywemo-1.1.0.tar.gz` & `tmp/pywemo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywemo-1.1.0.tar", max compression
+gzip compressed data, was "pywemo-1.2.0.tar", max compression
```

## Comparing `pywemo-1.1.0.tar` & `pywemo-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     2831 2023-07-03 15:47:34.389949 pywemo-1.1.0/LICENSE
--rw-r--r--   0        0        0     8322 2023-07-03 15:47:34.389949 pywemo-1.1.0/README.rst
--rw-r--r--   0        0        0     3196 2023-07-03 15:47:34.389949 pywemo-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2889 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/README.md
--rw-r--r--   0        0        0     1254 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/__init__.py
--rw-r--r--   0        0        0     2762 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/color.py
--rw-r--r--   0        0        0     6709 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/discovery.py
--rw-r--r--   0        0        0     2753 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/exceptions.py
--rw-r--r--   0        0        0     1468 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/LICENSE
--rw-r--r--   0        0        0    26370 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/__init__.py
--rw-r--r--   0        0        0       23 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/__init__.py
--rw-r--r--   0        0        0     4843 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/attributes.py
--rw-r--r--   0        0        0     6733 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/db_orm.py
--rw-r--r--   0        0        0     6059 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/long_press.py
--rw-r--r--   0        0        0    14976 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/rules_db.py
--rw-r--r--   0        0        0    12705 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/service.py
--rw-r--r--   0        0        0      912 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.py
--rw-r--r--   0        0        0     6838 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.pyi
--rw-r--r--   0        0        0       60 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/__init__.py
--rw-r--r--   0        0        0   126828 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.py
--rw-r--r--   0        0        0     4305 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.xsd
--rw-r--r--   0        0        0   122520 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.py
--rw-r--r--   0        0        0     3526 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.xsd
--rw-r--r--   0        0        0     7275 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd_types.py
--rw-r--r--   0        0        0    18975 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/bridge.py
--rw-r--r--   0        0        0     3345 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/coffeemaker.py
--rw-r--r--   0        0        0     5035 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/crockpot.py
--rw-r--r--   0        0        0     2250 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/dimmer.py
--rw-r--r--   0        0        0     7162 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/humidifier.py
--rw-r--r--   0        0        0     6125 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/insight.py
--rw-r--r--   0        0        0      328 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/lightswitch.py
--rw-r--r--   0        0        0     1645 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/maker.py
--rw-r--r--   0        0        0      141 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/motion.py
--rw-r--r--   0        0        0      157 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/outdoor_plug.py
--rw-r--r--   0        0        0     1023 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/switch.py
--rw-r--r--   0        0        0        0 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/py.typed
--rw-r--r--   0        0        0    12531 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ssdp.py
--rw-r--r--   0        0        0    28315 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/subscribe.py
--rw-r--r--   0        0        0     4417 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/util.py
--rw-r--r--   0        0        0     9084 1970-01-01 00:00:00.000000 pywemo-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-07-31 02:36:23.986254 pywemo-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8322 2023-07-31 02:36:23.986254 pywemo-1.2.0/README.rst
+-rw-r--r--   0        0        0     3196 2023-07-31 02:36:23.986254 pywemo-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2889 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/README.md
+-rw-r--r--   0        0        0     1254 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/__init__.py
+-rw-r--r--   0        0        0     2762 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/color.py
+-rw-r--r--   0        0        0     6806 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/discovery.py
+-rw-r--r--   0        0        0     2753 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/exceptions.py
+-rw-r--r--   0        0        0     1468 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/LICENSE
+-rw-r--r--   0        0        0    26370 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/__init__.py
+-rw-r--r--   0        0        0     4843 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/attributes.py
+-rw-r--r--   0        0        0     6733 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/db_orm.py
+-rw-r--r--   0        0        0     6059 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/long_press.py
+-rw-r--r--   0        0        0    14976 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/rules_db.py
+-rw-r--r--   0        0        0    12705 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/service.py
+-rw-r--r--   0        0        0      912 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.py
+-rw-r--r--   0        0        0     6838 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.pyi
+-rw-r--r--   0        0        0       60 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/__init__.py
+-rw-r--r--   0        0        0   126828 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.py
+-rw-r--r--   0        0        0     4305 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.xsd
+-rw-r--r--   0        0        0   122520 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.py
+-rw-r--r--   0        0        0     3526 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.xsd
+-rw-r--r--   0        0        0     7275 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd_types.py
+-rw-r--r--   0        0        0    18975 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/bridge.py
+-rw-r--r--   0        0        0     3345 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/coffeemaker.py
+-rw-r--r--   0        0        0     5035 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/crockpot.py
+-rw-r--r--   0        0        0     2250 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/dimmer.py
+-rw-r--r--   0        0        0     7162 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/humidifier.py
+-rw-r--r--   0        0        0     6125 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/insight.py
+-rw-r--r--   0        0        0      328 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/lightswitch.py
+-rw-r--r--   0        0        0     1645 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/maker.py
+-rw-r--r--   0        0        0      141 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/motion.py
+-rw-r--r--   0        0        0      157 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/outdoor_plug.py
+-rw-r--r--   0        0        0     1023 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/switch.py
+-rw-r--r--   0        0        0        0 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/py.typed
+-rw-r--r--   0        0        0    12531 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ssdp.py
+-rw-r--r--   0        0        0    28315 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/subscribe.py
+-rw-r--r--   0        0        0     4417 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/util.py
+-rw-r--r--   0        0        0     9084 1970-01-01 00:00:00.000000 pywemo-1.2.0/PKG-INFO
```

### Comparing `pywemo-1.1.0/LICENSE` & `pywemo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/README.rst` & `pywemo-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pyproject.toml` & `pywemo-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pywemo"
-version = "1.1.0"
+version = "1.2.0"
 description = "Lightweight Python module to discover and control WeMo devices"
 authors = ["Eric Severance <pywemo@esev.com>"]
 license = "MIT"
 
 readme = 'README.rst'
 
 repository = "https://github.com/pywemo/pywemo"
@@ -23,15 +23,15 @@
 urllib3 = ">=1.26.0"
 lxml = "^4.6"
 
 [tool.poetry.group.dev.dependencies]
 # toml is used by multiple tools to read this pyproject.toml file
 toml = ">=0.10"
 # formatters
-black = "23.3.0"
+black = "23.7.0"
 isort = "^5.6.4"
 # linters/code analysis
 flake8 = "^6.0.0"
 flake8-docstrings = ">=1.3.0"
 flake8-bugbear = ">=20.11.1"
 pylint = "^2.17.3"
 rstcheck = ">=3.3.1,<7.0.0"
@@ -40,15 +40,15 @@
 lxml-stubs = "^0.4.0"
 pytest = "^7.3.1"
 pytest-vcr = "1.0.2"
 types-requests = ">=2.0"
 coverage = "^7.2.4"
 hypothesis = "^6.75.3"
 # version of generateDS used to create device.py and service.py in .../api/xsd
-generateDS = "2.41.5"
+generateDS = "2.42.2"
 # other
 deptry = ">=0.11,<0.13"
 pre-commit = ">=2.10,<4.0"
 # docs
 pdoc = ">=13.1.1,<15.0.0"
 
 [tool.poetry.group.bootstrap.dependencies]
```

### Comparing `pywemo-1.1.0/pywemo/README.md` & `pywemo-1.2.0/pywemo/README.md`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/__init__.py` & `pywemo-1.2.0/pywemo/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/color.py` & `pywemo-1.2.0/pywemo/color.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/discovery.py` & `pywemo-1.2.0/pywemo/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
     """Determine device class based on the device uuid."""
     if not (uuid and location):
         return None
     try:
         if uuid.startswith("uuid:Socket"):
             return Switch(location)
         if uuid.startswith("uuid:Lightswitch-1_0"):
+            if not location.endswith("/setup.xml"):
+                return LightSwitch(location)
             return LightSwitchLongPress(location)
         if uuid.startswith("uuid:Lightswitch-2_0"):
             return LightSwitchLongPress(location)
         if uuid.startswith("uuid:Lightswitch-3_0"):
             return LightSwitchLongPress(location)
         if uuid.startswith("uuid:Lightswitch"):
             return LightSwitch(location)
```

### Comparing `pywemo-1.1.0/pywemo/exceptions.py` & `pywemo-1.2.0/pywemo/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/LICENSE` & `pywemo-1.2.0/pywemo/ouimeaux_device/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/__init__.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/attributes.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/attributes.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/db_orm.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/db_orm.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/long_press.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/long_press.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/rules_db.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/rules_db.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/service.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/service.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.pyi` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.pyi`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 # isort: skip_file
 # mypy: ignore-errors
 # pylint: skip-file
 
 #
-# Generated  by generateDS.py version 2.41.5.
+# Generated  by generateDS.py version 2.42.2.
 # Python [sys.version]
 #
 # Command line options:
 #   ('-f', '')
 #   ('--no-dates', '')
 #   ('-o', 'device.py')
 #
```

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.xsd` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 # isort: skip_file
 # mypy: ignore-errors
 # pylint: skip-file
 
 #
-# Generated  by generateDS.py version 2.41.5.
+# Generated  by generateDS.py version 2.42.2.
 # Python [sys.version]
 #
 # Command line options:
 #   ('-f', '')
 #   ('--no-dates', '')
 #   ('-o', 'service.py')
 #
```

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.xsd` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd_types.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd_types.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/bridge.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/bridge.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/coffeemaker.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/coffeemaker.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/crockpot.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/crockpot.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/dimmer.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/dimmer.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/humidifier.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/humidifier.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/insight.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/insight.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/maker.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/maker.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ouimeaux_device/switch.py` & `pywemo-1.2.0/pywemo/ouimeaux_device/switch.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/ssdp.py` & `pywemo-1.2.0/pywemo/ssdp.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/subscribe.py` & `pywemo-1.2.0/pywemo/subscribe.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/pywemo/util.py` & `pywemo-1.2.0/pywemo/util.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.1.0/PKG-INFO` & `pywemo-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywemo
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lightweight Python module to discover and control WeMo devices
 Home-page: https://github.com/pywemo/pywemo
 License: MIT
 Keywords: wemo,api
 Author: Eric Severance
 Author-email: pywemo@esev.com
 Requires-Python: >=3.8.1,<4.0.0
```

