# Comparing `tmp/neon_gui-1.2.0.tar.gz` & `tmp/neon_gui-1.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_gui-1.2.0.tar", last modified: Thu Jul 20 16:38:24 2023, max compression
+gzip compressed data, was "neon_gui-1.2.1a1.tar", last modified: Mon Jul 31 20:26:53 2023, max compression
```

## Comparing `neon_gui-1.2.0.tar` & `neon_gui-1.2.1a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:38:24.785737 neon_gui-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-20 16:38:18.000000 neon_gui-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-20 16:38:24.785737 neon_gui-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 16:38:18.000000 neon_gui-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:38:24.785737 neon_gui-1.2.0/neon_gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:38:24.785737 neon_gui-1.2.0/neon_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:38:24.785737 neon_gui-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-20 16:38:18.000000 neon_gui-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:26:53.807909 neon_gui-1.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 20:26:53.807909 neon_gui-1.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:26:53.807909 neon_gui-1.2.1a1/neon_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/neon_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/neon_gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/neon_gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/neon_gui/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/neon_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:26:53.807909 neon_gui-1.2.1a1/neon_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 20:26:53.000000 neon_gui-1.2.1a1/neon_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 20:26:53.000000 neon_gui-1.2.1a1/neon_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:26:53.000000 neon_gui-1.2.1a1/neon_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 20:26:53.000000 neon_gui-1.2.1a1/neon_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 20:26:53.000000 neon_gui-1.2.1a1/neon_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 20:26:53.000000 neon_gui-1.2.1a1/neon_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:26:53.807909 neon_gui-1.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-31 20:26:43.000000 neon_gui-1.2.1a1/setup.py
```

### Comparing `neon_gui-1.2.0/LICENSE.md` & `neon_gui-1.2.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.2.0/PKG-INFO` & `neon_gui-1.2.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_gui
-Version: 1.2.0
+Version: 1.2.1a1
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.2.0/README.md` & `neon_gui-1.2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.2.0/neon_gui/__init__.py` & `neon_gui-1.2.1a1/neon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.2.0/neon_gui/__main__.py` & `neon_gui-1.2.1a1/neon_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.2.0/neon_gui/cli.py` & `neon_gui-1.2.1a1/neon_gui/cli.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.2.0/neon_gui/service.py` & `neon_gui-1.2.1a1/neon_gui/service.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.2.0/neon_gui/utils.py` & `neon_gui-1.2.1a1/neon_gui/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,25 +86,33 @@
         extra_data.append({'display_key': 'Image Updated',
                            'display_value': image_recipe_time})
         extra_data.append({'display_key': 'Core Updated',
                            'display_value': core_time})
 
         if build_info.get('base_os'):
             base_os = build_info['base_os']['name']
-            if build_info['base_os'].get('time', 'unknown') != 'unknown':
-                time_str = datetime.fromtimestamp(
-                    build_info['base_os'].get('time')).strftime('%Y-%m-%d')
+            base_os_time = build_info['base_os'].get('time', 'unknown')
+            if base_os_time != 'unknown':
+                if isinstance(base_os_time, float):
+                    time_str = datetime.fromtimestamp(base_os_time).strftime(
+                        '%Y-%m-%d')
+                else:
+                    time_str = str(base_os_time).replace('_',
+                                                         ' ', 1).replace('_',
+                                                                         ':', 1)
                 base_os = f'{base_os} ({time_str})'
             extra_data.append({'display_key': 'Base OS',
                                'display_value': base_os})
         if installed_core_spec != core_version:
             extra_data.append({'display_key': "Shipped Core Version",
                                'display_value': installed_core_spec})
     except FileNotFoundError:
         pass
+    except Exception as e:
+        LOG.exception(e)
 
     for pkg in ('neon_speech', 'neon_audio', 'neon_gui', 'neon_enclosure'):
         try:
             pkg_data = {"display_key": pkg,
                         "display_value": get_package_version_spec(pkg)}
         except ModuleNotFoundError:
             pkg_data = {"display_key": pkg,
```

### Comparing `neon_gui-1.2.0/neon_gui.egg-info/PKG-INFO` & `neon_gui-1.2.1a1/neon_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.2.0
+Version: 1.2.1a1
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.2.0/setup.py` & `neon_gui-1.2.1a1/setup.py`

 * *Files identical despite different names*

