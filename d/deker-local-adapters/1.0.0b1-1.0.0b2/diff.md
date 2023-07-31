# Comparing `tmp/deker_local_adapters-1.0.0b1.tar.gz` & `tmp/deker_local_adapters-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker_local_adapters-1.0.0b1.tar", last modified: Mon Jul 31 09:19:07 2023, max compression
+gzip compressed data, was "deker_local_adapters-1.0.0b2.tar", last modified: Mon Jul 31 10:03:39 2023, max compression
```

## Comparing `deker_local_adapters-1.0.0b1.tar` & `deker_local_adapters-1.0.0b2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/deker_local_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/array_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/collection_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/deker_local_adapters/varray_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 09:19:07.000000 deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 09:19:07.000000 deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:19:07.000000 deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 09:19:07.000000 deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 09:19:07.000000 deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-31 09:19:07.111079 deker_local_adapters-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-31 09:18:55.000000 deker_local_adapters-1.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:03:39.167446 deker_local_adapters-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 10:03:39.167446 deker_local_adapters-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:03:39.163446 deker_local_adapters-1.0.0b2/deker_local_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/array_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/collection_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:03:39.163446 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:03:39.167446 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/deker_local_adapters/varray_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:03:39.163446 deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 10:03:39.000000 deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 10:03:39.000000 deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:03:39.000000 deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-31 10:03:39.000000 deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 10:03:39.000000 deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-31 10:03:39.167446 deker_local_adapters-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-31 10:03:27.000000 deker_local_adapters-1.0.0b2/setup.py
```

### Comparing `deker_local_adapters-1.0.0b1/LICENSE` & `deker_local_adapters-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/PKG-INFO` & `deker_local_adapters-1.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker_local_adapters
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: adapters for Deker embedded databases management
 Home-page: https://github.com/openweathermap/deker-local-adapters
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Maintainer: OpenWeather
 Maintainer-email: info@openweathermap.org
 License: GPL-3.0-only
```

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/array_adapter.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/array_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/collection_adapter.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/collection_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/factory.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/factory.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/mixin.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/mixin.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters/varray_adapter.py` & `deker_local_adapters-1.0.0b2/deker_local_adapters/varray_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/PKG-INFO` & `deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker-local-adapters
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: adapters for Deker embedded databases management
 Home-page: https://github.com/openweathermap/deker-local-adapters
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Maintainer: OpenWeather
 Maintainer-email: info@openweathermap.org
 License: GPL-3.0-only
```

### Comparing `deker_local_adapters-1.0.0b1/deker_local_adapters.egg-info/SOURCES.txt` & `deker_local_adapters-1.0.0b2/deker_local_adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/pyproject.toml` & `deker_local_adapters-1.0.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/setup.cfg` & `deker_local_adapters-1.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.0.0b1/setup.py` & `deker_local_adapters-1.0.0b2/setup.py`

 * *Files 0% similar despite different names*

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

