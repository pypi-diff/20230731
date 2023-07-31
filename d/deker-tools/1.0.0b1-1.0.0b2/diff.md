# Comparing `tmp/deker_tools-1.0.0b1.tar.gz` & `tmp/deker_tools-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker_tools-1.0.0b1.tar", last modified: Mon Jul 31 09:14:04 2023, max compression
+gzip compressed data, was "deker_tools-1.0.0b2.tar", last modified: Mon Jul 31 09:42:58 2023, max compression
```

## Comparing `deker_tools-1.0.0b1.tar` & `deker_tools-1.0.0b2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:14:04.064333 deker_tools-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 09:14:04.064333 deker_tools-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:14:04.064333 deker_tools-1.0.0b1/deker_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/deker_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/deker_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/deker_tools/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/deker_tools/slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/deker_tools/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:14:04.064333 deker_tools-1.0.0b1/deker_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 09:14:04.000000 deker_tools-1.0.0b1/deker_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-31 09:14:04.000000 deker_tools-1.0.0b1/deker_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:14:04.000000 deker_tools-1.0.0b1/deker_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:14:04.000000 deker_tools-1.0.0b1/deker_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:14:04.000000 deker_tools-1.0.0b1/deker_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-31 09:14:04.064333 deker_tools-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:14:04.064333 deker_tools-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-07-31 09:13:56.000000 deker_tools-1.0.0b1/tests/test_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:42:58.652096 deker_tools-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 09:42:58.652096 deker_tools-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:42:58.648095 deker_tools-1.0.0b2/deker_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/deker_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/deker_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/deker_tools/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/deker_tools/slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/deker_tools/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:42:58.652096 deker_tools-1.0.0b2/deker_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 09:42:58.000000 deker_tools-1.0.0b2/deker_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-31 09:42:58.000000 deker_tools-1.0.0b2/deker_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:42:58.000000 deker_tools-1.0.0b2/deker_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:42:58.000000 deker_tools-1.0.0b2/deker_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:42:58.000000 deker_tools-1.0.0b2/deker_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-31 09:42:58.652096 deker_tools-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:42:58.652096 deker_tools-1.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-07-31 09:42:49.000000 deker_tools-1.0.0b2/tests/test_slices.py
```

### Comparing `deker_tools-1.0.0b1/LICENSE` & `deker_tools-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/PKG-INFO` & `deker_tools-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker_tools
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Tools for Deker management
 Home-page: https://github.com/openweathermap/deker-tools
 Author: OpenWeatherMap
 Author-email: info@openweathermap.org
 Maintainer-email: info@openweathermap.org
 License: GPL-3.0-only
 Platform: any
```

### Comparing `deker_tools-1.0.0b1/deker_tools/path.py` & `deker_tools-1.0.0b2/deker_tools/path.py`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/deker_tools/slices.py` & `deker_tools-1.0.0b2/deker_tools/slices.py`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/deker_tools/time.py` & `deker_tools-1.0.0b2/deker_tools/time.py`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/deker_tools.egg-info/PKG-INFO` & `deker_tools-1.0.0b2/deker_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker-tools
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Tools for Deker management
 Home-page: https://github.com/openweathermap/deker-tools
 Author: OpenWeatherMap
 Author-email: info@openweathermap.org
 Maintainer-email: info@openweathermap.org
 License: GPL-3.0-only
 Platform: any
```

### Comparing `deker_tools-1.0.0b1/pyproject.toml` & `deker_tools-1.0.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/setup.cfg` & `deker_tools-1.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/setup.py` & `deker_tools-1.0.0b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def get_version() -> str:
     """Get version from commit tag.
 
     Regexp reference:
     https://gitlab.openweathermap.org/help/user/packages/pypi_repository/index.md#ensure-your-version-string-is-valid
     """
-    ci_commit_tag: Optional[str] = os.getenv("PACKAGE_VERSION", "0.0.0")
+    ci_commit_tag: Optional[str] = os.getenv("PACKAGE_VERSION", "1.0.0b-2")
     regex = (
         r"(?:"
         r"(?:([0-9]+)!)?"
         r"([0-9]+(?:\.[0-9]+)*)"
         r"([-_\.]?((a|b|c|rc|alpha|beta|pre|preview))[-_\.]?([0-9]+)?)?"
         r"((?:-([0-9]+))|(?:[-_\.]?(post|rev|r)[-_\.]?([0-9]+)?))?"
         r"([-_\.]?(dev)[-_\.]?([0-9]+)?)?"
```

### Comparing `deker_tools-1.0.0b1/tests/test_path.py` & `deker_tools-1.0.0b2/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `deker_tools-1.0.0b1/tests/test_slices.py` & `deker_tools-1.0.0b2/tests/test_slices.py`

 * *Files identical despite different names*

