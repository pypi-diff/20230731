# Comparing `tmp/zigpy-zboss-1.0.2.tar.gz` & `tmp/zigpy-zboss-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-zboss-1.0.2.tar", last modified: Fri Jul  7 16:15:02 2023, max compression
+gzip compressed data, was "zigpy-zboss-1.1.0.tar", last modified: Mon Jul 31 13:54:27 2023, max compression
```

## Comparing `zigpy-zboss-1.0.2.tar` & `zigpy-zboss-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/af.py
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/aps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/ncp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/nwk_mgmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/zdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/nvram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/factory_reset_ncp.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/get_ncp_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/zigpy_zboss/types/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/nvids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/uart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.485622 zigpy-zboss-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-31 13:54:27.485622 zigpy-zboss-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-31 13:54:27.485622 zigpy-zboss-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.481622 zigpy-zboss-1.1.0/zigpy_zboss/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.481622 zigpy-zboss-1.1.0/zigpy_zboss/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/af.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/aps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/ncp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/nwk_mgmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/commands/zdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/nvram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.481622 zigpy-zboss-1.1.0/zigpy_zboss/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/tools/factory_reset_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/tools/get_ncp_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.481622 zigpy-zboss-1.1.0/zigpy_zboss/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/nvids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/types/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.485622 zigpy-zboss-1.1.0/zigpy_zboss/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/zigbee/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-31 13:54:16.000000 zigpy-zboss-1.1.0/zigpy_zboss/zigbee/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:54:27.481622 zigpy-zboss-1.1.0/zigpy_zboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-31 13:54:27.000000 zigpy-zboss-1.1.0/zigpy_zboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-31 13:54:27.000000 zigpy-zboss-1.1.0/zigpy_zboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:54:27.000000 zigpy-zboss-1.1.0/zigpy_zboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 13:54:27.000000 zigpy-zboss-1.1.0/zigpy_zboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 13:54:27.000000 zigpy-zboss-1.1.0/zigpy_zboss.egg-info/top_level.txt
```

### Comparing `zigpy-zboss-1.0.2/COPYING` & `zigpy-zboss-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/LICENSE` & `zigpy-zboss-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/PKG-INFO` & `zigpy-zboss-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-zboss
-Version: 1.0.2
+Version: 1.1.0
 Summary: A library for zigpy which communicates with Nordic nRF52 radios
 Home-page: https://github.com/kardia-as/zigpy-zboss
 Author: Damien Kastner
 Author-email: damien.kastner@kardia.no
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `zigpy-zboss-1.0.2/README.md` & `zigpy-zboss-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/pyproject.toml` & `zigpy-zboss-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/setup.cfg` & `zigpy-zboss-1.1.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 author_email = damien.kastner@kardia.no
 license = GPL-3.0
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	pyserial-asyncio; platform_system!="Windows"
-	pyserial-asyncio!=0.5; platform_system=="Windows"  # 0.5 broke writes
-	zigpy>=0.54.1
+	zigpy>=0.55.0
 	async_timeout
 	voluptuous
 	coloredlogs
 	jsonschema
 
 [options.packages.find]
 exclude =
```

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/api.py` & `zigpy-zboss-1.1.0/zigpy_zboss/api.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/checksum.py` & `zigpy-zboss-1.1.0/zigpy_zboss/checksum.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/__init__.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/af.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/af.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/aps.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/aps.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/ncp_config.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/ncp_config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/nwk_mgmt.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/nwk_mgmt.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/security.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/commands/zdo.py` & `zigpy-zboss-1.1.0/zigpy_zboss/commands/zdo.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/config.py` & `zigpy-zboss-1.1.0/zigpy_zboss/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/debug.py` & `zigpy-zboss-1.1.0/zigpy_zboss/debug.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/frames.py` & `zigpy-zboss-1.1.0/zigpy_zboss/frames.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/logger.py` & `zigpy-zboss-1.1.0/zigpy_zboss/logger.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/nvram.py` & `zigpy-zboss-1.1.0/zigpy_zboss/nvram.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/tools/config.py` & `zigpy-zboss-1.1.0/zigpy_zboss/tools/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/tools/factory_reset_ncp.py` & `zigpy-zboss-1.1.0/zigpy_zboss/tools/factory_reset_ncp.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/tools/get_ncp_version.py` & `zigpy-zboss-1.1.0/zigpy_zboss/tools/get_ncp_version.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/types/basic.py` & `zigpy-zboss-1.1.0/zigpy_zboss/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/types/commands.py` & `zigpy-zboss-1.1.0/zigpy_zboss/types/commands.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/types/cstruct.py` & `zigpy-zboss-1.1.0/zigpy_zboss/types/cstruct.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/types/named.py` & `zigpy-zboss-1.1.0/zigpy_zboss/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/types/nvids.py` & `zigpy-zboss-1.1.0/zigpy_zboss/types/nvids.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/types/structs.py` & `zigpy-zboss-1.1.0/zigpy_zboss/types/structs.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/uart.py` & `zigpy-zboss-1.1.0/zigpy_zboss/uart.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 """Module that connects and sends/receives bytes from the nRF52 SoC."""
 import typing
 import asyncio
 import logging
+import zigpy.serial
 import async_timeout
 import serial  # type: ignore
 import zigpy_zboss.config as conf
 from zigpy_zboss import types as t
 from zigpy_zboss.frames import Frame
 from zigpy_zboss.checksum import CRC8
-import serial_asyncio  # type: ignore
 from zigpy_zboss.logger import SERIAL_LOGGER
 from zigpy_zboss.exceptions import InvalidFrame
 
 LOGGER = logging.getLogger(__name__)
 ACK_TIMEOUT = 1
 SEND_RETRIES = 2
 STARTUP_TIMEOUT = 5
 RECONNECT_TIMEOUT = 10
 
 
 class BufferTooShort(Exception):
     """Exception when the buffer is too short."""
 
 
-class Uart(asyncio.Protocol):
-    """Uart class."""
+class ZbossNcpProtocol(asyncio.Protocol):
+    """Zboss Ncp Protocol class."""
 
     def __init__(self, config, api) -> None:
-        """Initialize the Uart object."""
+        """Initialize the ZbossNcpProtocol object."""
         self._api = api
         self._ack_seq = 0
         self._pack_seq = 0
         self._config = config
         self._transport = None
         self._reset_flag = False
         self._buffer = bytearray()
         self._reconnect_task = None
         self._tx_lock = asyncio.Lock()
         self._ack_received_event = None
         self._connected_event = asyncio.Event()
 
+        self._port = config[conf.CONF_DEVICE_PATH]
+        self._baudrate = config[conf.CONF_DEVICE_BAUDRATE]
+        self._flow_control = config[conf.CONF_DEVICE_FLOW_CONTROL]
+
     @property
     def api(self):
         """Return the owner of that object."""
         return self._api
 
     @property
     def name(self) -> str:
@@ -62,15 +66,15 @@
 
     @reset_flag.setter
     def reset_flag(self, value) -> None:
         if isinstance(value, bool):
             self._reset_flag = value
 
     def connection_made(
-            self, transport: serial_asyncio.SerialTransport) -> None:
+            self, transport: asyncio.BaseTransport) -> None:
         """Notify serial port opened."""
         self._transport = transport
         message = f"Opened {transport.serial.name} serial port"
         if self._reset_flag:
             self._reset_flag = False
             return
         SERIAL_LOGGER.info(message)
@@ -95,25 +99,21 @@
         """Try to reconnect the disconnected serial port."""
         SERIAL_LOGGER.info("Trying to reconnect to the NCP module!")
         assert self._api is not None
         loop = asyncio.get_running_loop()
         async with async_timeout.timeout(timeout):
             while True:
                 try:
-                    _, proto = await serial_asyncio.create_serial_connection(
+                    _, proto = await zigpy.serial.create_serial_connection(
                         loop=loop,
                         protocol_factory=lambda: self,
-                        url=self._config[conf.CONF_DEVICE_PATH],
-                        baudrate=self._config[conf.CONF_DEVICE_BAUDRATE],
-                        parity=serial.PARITY_NONE,
-                        stopbits=serial.STOPBITS_ONE,
-                        xonxoff=(self._config[
-                            conf.CONF_DEVICE_FLOW_CONTROL] == "software"),
-                        rtscts=(self._config[
-                            conf.CONF_DEVICE_FLOW_CONTROL] == "hardware"),
+                        url=self._port,
+                        baudrate=self._baudrate,
+                        xonxoff=(self._flow_control == "software"),
+                        rtscts=(self._flow_control == "hardware"),
                     )
                     self._api._uart = proto
                     break
                 except serial.serialutil.SerialException:
                     await asyncio.sleep(0.1)
 
     def close(self) -> None:
@@ -264,33 +264,31 @@
             f"{type(self).__name__} connected to {self.name!r}"
             f" at {self.baudrate} baud"
             f" (api: {self._api})"
             f">"
         )
 
 
-async def connect(config: conf.ConfigType, api) -> Uart:
+async def connect(config: conf.ConfigType, api) -> ZbossNcpProtocol:
     """Instantiate Uart object and connect to it."""
     loop = asyncio.get_running_loop()
 
-    LOGGER.info(
-        "Connecting to %s at %s baud",
-        config[conf.CONF_DEVICE_PATH],
-        config[conf.CONF_DEVICE_BAUDRATE]
-    )
+    port = config[conf.CONF_DEVICE_PATH]
+    baudrate = config[conf.CONF_DEVICE_BAUDRATE]
+    flow_control = config[conf.CONF_DEVICE_FLOW_CONTROL]
+
+    LOGGER.info("Connecting to %s at %s baud", port, baudrate)
 
-    _, protocol = await serial_asyncio.create_serial_connection(
+    _, protocol = await zigpy.serial.create_serial_connection(
         loop=loop,
-        protocol_factory=lambda: Uart(config, api),
-        url=config[conf.CONF_DEVICE_PATH],
-        baudrate=config[conf.CONF_DEVICE_BAUDRATE],
-        parity=serial.PARITY_NONE,
-        stopbits=serial.STOPBITS_ONE,
-        xonxoff=(config[conf.CONF_DEVICE_FLOW_CONTROL] == "software"),
-        rtscts=(config[conf.CONF_DEVICE_FLOW_CONTROL] == "hardware"),
+        protocol_factory=lambda: ZbossNcpProtocol(config, api),
+        url=port,
+        baudrate=baudrate,
+        xonxoff=(flow_control == "software"),
+        rtscts=(flow_control == "hardware"),
     )
 
     try:
         async with async_timeout.timeout(STARTUP_TIMEOUT):
             await protocol._connected_event.wait()
     except asyncio.TimeoutError:
         protocol.close()
```

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/utils.py` & `zigpy-zboss-1.1.0/zigpy_zboss/utils.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/zigbee/application.py` & `zigpy-zboss-1.1.0/zigpy_zboss/zigbee/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,28 @@
                 ScanDuration=0x05,
                 DistributedNetFlag=0x00,
                 DistributedNetAddr=t.NWK(0x0000),
                 IEEEAddr=network_info.extended_pan_id
             )
         )
 
+    async def _move_network_to_channel(
+            self, new_channel: int, new_nwk_update_id: int) -> None:
+        """Move device to a new channel."""
+        await self._api.request(
+            request=c.ZDO.MgmtNwkUpdate.Req(
+                TSN=self.get_sequence(),
+                ScanChannelMask=t.Channels.from_channel_list([new_channel]),
+                ScanDuration=zdo_t.NwkUpdate.CHANNEL_CHANGE_REQ,
+                ScanCount=0,
+                MgrAddr=0x0000,
+                DstNWK=0x0000,
+            ),
+        )
+
     async def load_network_info(self, *, load_devices=False):
         """Populate state.node_info and state.network_info."""
         res = await self._api.request(
             c.NcpConfig.GetJoinStatus.Req(TSN=self.get_sequence()))
         if not res.Joined & 0x01:
             raise zigpy.exceptions.NetworkNotFormed
```

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss/zigbee/device.py` & `zigpy-zboss-1.1.0/zigpy_zboss/zigbee/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     async def Mgmt_NWK_Update_req(self, nwkUpdate):
         """Request join permition."""
         res = await self._device._application._api.request(
             c.ZDO.MgmtNwkUpdate.Req(
                 TSN=self._device._application.get_sequence(),
                 ScanChannelMask=nwkUpdate.ScanChannels,
                 ScanDuration=nwkUpdate.ScanDuration,
-                ScanCount=nwkUpdate.ScanCount,
+                ScanCount=nwkUpdate.ScanCount or 0,
                 MgrAddr=self._device.nwk,
                 DstNWK=t.NWK(0x0000),
             )
         )
         if res.StatusCode != 0:
             return (None, None, None, None, None)
         return (None, res.ScannedChannels, None, None, res.EnergyValues)
```

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss.egg-info/PKG-INFO` & `zigpy-zboss-1.1.0/zigpy_zboss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-zboss
-Version: 1.0.2
+Version: 1.1.0
 Summary: A library for zigpy which communicates with Nordic nRF52 radios
 Home-page: https://github.com/kardia-as/zigpy-zboss
 Author: Damien Kastner
 Author-email: damien.kastner@kardia.no
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `zigpy-zboss-1.0.2/zigpy_zboss.egg-info/SOURCES.txt` & `zigpy-zboss-1.1.0/zigpy_zboss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

