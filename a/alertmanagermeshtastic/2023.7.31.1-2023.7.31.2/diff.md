# Comparing `tmp/alertmanagermeshtastic-2023.7.31.1.tar.gz` & `tmp/alertmanagermeshtastic-2023.7.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.7.31.1.tar", last modified: Mon Jul 31 19:01:34 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.7.31.2.tar", last modified: Mon Jul 31 19:07:12 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.7.31.1.tar` & `alertmanagermeshtastic-2023.7.31.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:01:34.722191 alertmanagermeshtastic-2023.7.31.1/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-31 19:01:34.722191 alertmanagermeshtastic-2023.7.31.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-31 19:01:34.726191 alertmanagermeshtastic-2023.7.31.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:01:34.718191 alertmanagermeshtastic-2023.7.31.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:01:34.722191 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:01:34.722191 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:01:34.000000 alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:01:34.722191 alertmanagermeshtastic-2023.7.31.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-31 19:01:26.000000 alertmanagermeshtastic-2023.7.31.1/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:07:12.395115 alertmanagermeshtastic-2023.7.31.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-31 19:07:12.395115 alertmanagermeshtastic-2023.7.31.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-31 19:07:12.395115 alertmanagermeshtastic-2023.7.31.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:07:12.387115 alertmanagermeshtastic-2023.7.31.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:07:12.391115 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:07:12.391115 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:07:12.000000 alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:07:12.395115 alertmanagermeshtastic-2023.7.31.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-31 19:07:04.000000 alertmanagermeshtastic-2023.7.31.2/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.7.31.1/Dockerfile` & `alertmanagermeshtastic-2023.7.31.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/LICENSE` & `alertmanagermeshtastic-2023.7.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/PKG-INFO` & `alertmanagermeshtastic-2023.7.31.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.7.31.1
+Version: 2023.7.31.2
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
```

### Comparing `alertmanagermeshtastic-2023.7.31.1/README.md` & `alertmanagermeshtastic-2023.7.31.2/README.md`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/setup.cfg` & `alertmanagermeshtastic-2023.7.31.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/meshtastic.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.7.31.1
+Version: 2023.7.31.2
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
```

### Comparing `alertmanagermeshtastic-2023.7.31.1/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.7.31.2/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.7.31.2/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.7.31.2/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/tests/test_load_config.py` & `alertmanagermeshtastic-2023.7.31.2/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.7.31.2/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.7.31.2/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.7.31.1/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.7.31.2/tests/test_token_cli.py`

 * *Files identical despite different names*

