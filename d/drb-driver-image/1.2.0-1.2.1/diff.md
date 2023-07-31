# Comparing `tmp/drb-driver-image-1.2.0.tar.gz` & `tmp/drb-driver-image-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-image-1.2.0.tar", last modified: Thu Apr 20 13:45:43 2023, max compression
+gzip compressed data, was "drb-driver-image-1.2.1.tar", last modified: Mon Jul 31 11:52:42 2023, max compression
```

## Comparing `drb-driver-image-1.2.0.tar` & `drb-driver-image-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.915057 drb-driver-image-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 15:53:50.000000 drb-driver-image-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2084 2023-04-20 13:45:43.915057 drb-driver-image-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1539 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.871056 drb-driver-image-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.871056 drb-driver-image-1.2.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.919057 drb-driver-image-1.2.0/drb/drivers/image/
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/drb/drivers/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-20 13:45:43.919057 drb-driver-image-1.2.0/drb/drivers/image/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7904 2023-04-20 13:23:36.000000 drb-driver-image-1.2.0/drb/drivers/image/base_node.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/drb/drivers/image/list_node.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/drb/drivers/image/simple_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.895056 drb-driver-image-1.2.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/drb/exceptions/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.871056 drb-driver-image-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.895056 drb-driver-image-1.2.0/drb/topics/image/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/drb/topics/image/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-20 13:44:38.000000 drb-driver-image-1.2.0/drb/topics/image/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.899056 drb-driver-image-1.2.0/drb_driver_image.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2084 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-20 12:54:00.000000 drb-driver-image-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-20 13:45:43.919057 drb-driver-image-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.915057 drb-driver-image-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3441 2023-03-29 11:51:14.000000 drb-driver-image-1.2.0/tests/test_drb_image_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6710 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/tests/test_drb_image_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/tests/test_drb_image_node_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/tests/test_drb_image_signature.py
--rw-rw-rw-   0 root         (0) root         (0)     3622 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/tests/test_drb_image_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-03-29 11:51:14.000000 drb-driver-image-1.2.0/tests/test_drb_image_value_node.py
--rw-rw-rw-   0 root         (0) root         (0)    78254 2022-03-22 16:40:06.000000 drb-driver-image-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.783944 drb-driver-image-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 15:53:50.000000 drb-driver-image-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-31 11:51:16.000000 drb-driver-image-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-07-31 11:52:42.783944 drb-driver-image-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2022-12-20 15:01:55.000000 drb-driver-image-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.647942 drb-driver-image-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.647942 drb-driver-image-1.2.1/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.691943 drb-driver-image-1.2.1/drb/drivers/image/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-31 11:51:16.000000 drb-driver-image-1.2.1/drb/drivers/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-07-31 11:52:42.787944 drb-driver-image-1.2.1/drb/drivers/image/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7904 2023-04-20 13:23:36.000000 drb-driver-image-1.2.1/drb/drivers/image/base_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-19 16:07:18.000000 drb-driver-image-1.2.1/drb/drivers/image/list_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-04-19 16:07:18.000000 drb-driver-image-1.2.1/drb/drivers/image/simple_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.707943 drb-driver-image-1.2.1/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-12-20 15:01:55.000000 drb-driver-image-1.2.1/drb/exceptions/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.647942 drb-driver-image-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.711943 drb-driver-image-1.2.1/drb/topics/image/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 15:01:55.000000 drb-driver-image-1.2.1/drb/topics/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-25 14:25:20.000000 drb-driver-image-1.2.1/drb/topics/image/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.723943 drb-driver-image-1.2.1/drb_driver_image.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-31 11:52:42.000000 drb-driver-image-1.2.1/drb_driver_image.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-31 11:51:16.000000 drb-driver-image-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-11 13:52:00.000000 drb-driver-image-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-31 11:52:42.787944 drb-driver-image-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 11:51:16.000000 drb-driver-image-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:52:42.771944 drb-driver-image-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3441 2023-03-29 11:51:14.000000 drb-driver-image-1.2.1/tests/test_drb_image_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2022-12-20 15:01:55.000000 drb-driver-image-1.2.1/tests/test_drb_image_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2683 2023-07-31 11:51:16.000000 drb-driver-image-1.2.1/tests/test_drb_image_node_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-04-19 16:07:18.000000 drb-driver-image-1.2.1/tests/test_drb_image_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3622 2022-12-20 15:01:55.000000 drb-driver-image-1.2.1/tests/test_drb_image_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2023-03-29 11:51:14.000000 drb-driver-image-1.2.1/tests/test_drb_image_value_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2023-07-31 11:51:16.000000 drb-driver-image-1.2.1/versioneer.py
```

### Comparing `drb-driver-image-1.2.0/LICENCE.txt` & `drb-driver-image-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/PKG-INFO` & `drb-driver-image-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-image
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB Image driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, http://drb-python.gitlab.io/impl/image
 Project-URL: Source, https://gitlab.com/drb-python/impl/image
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-image-1.2.0/README.md` & `drb-driver-image-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/drb/drivers/image/base_node.py` & `drb-driver-image-1.2.1/drb/drivers/image/base_node.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/drb/drivers/image/list_node.py` & `drb-driver-image-1.2.1/drb/drivers/image/list_node.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/drb/drivers/image/simple_node.py` & `drb-driver-image-1.2.1/drb/drivers/image/simple_node.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/drb/topics/image/cortex.yml` & `drb-driver-image-1.2.1/drb/topics/image/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/drb_driver_image.egg-info/PKG-INFO` & `drb-driver-image-1.2.1/drb_driver_image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-image
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB Image driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, http://drb-python.gitlab.io/impl/image
 Project-URL: Source, https://gitlab.com/drb-python/impl/image
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-image-1.2.0/drb_driver_image.egg-info/SOURCES.txt` & `drb-driver-image-1.2.1/drb_driver_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/setup.cfg` & `drb-driver-image-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/tests/test_drb_image_list.py` & `drb-driver-image-1.2.1/tests/test_drb_image_list.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/tests/test_drb_image_node.py` & `drb-driver-image-1.2.1/tests/test_drb_image_node.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/tests/test_drb_image_node_factory.py` & `drb-driver-image-1.2.1/tests/test_drb_image_node_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,18 +55,17 @@
         self.assertTrue(node.has_child())
         self.assertEqual(len(node.children), 8)
 
     def test_base_node_attribute(self):
         node = self.open_node(str(self.image_tif_one))
 
         self.assertEqual(node.attributes, self.node_file.attributes)
-
-        self.assertEqual(node.get_attribute('directory'),
+        self.assertEqual(node.get_attribute('mode'),
                          self.node_file.get_attribute(
-                             'directory'))
+                             'mode'))
 
     def test_base_node_impl(self):
         node = self.open_node(str(self.image_tif_one))
 
         impl_base_file = io.BufferedIOBase
 
         self.assertTrue(node.has_impl(impl_base_file))
```

### Comparing `drb-driver-image-1.2.0/tests/test_drb_image_signature.py` & `drb-driver-image-1.2.1/tests/test_drb_image_signature.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/tests/test_drb_image_type.py` & `drb-driver-image-1.2.1/tests/test_drb_image_type.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/tests/test_drb_image_value_node.py` & `drb-driver-image-1.2.1/tests/test_drb_image_value_node.py`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.2.0/versioneer.py` & `drb-driver-image-1.2.1/versioneer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 
-# Version: 0.20
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -227,17 +255,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -259,54 +288,89 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods # noqa
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
 
-def get_root():
+
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = ("Versioneer was unable to run the project root directory. "
                "Versioneer requires setup.py to be executed from "
                "its immediate directory (like 'python setup.py COMMAND'), "
                "or in a way that lets it use sys.argv[0] to find the root "
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
@@ -315,86 +379,117 @@
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
                   % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
-        parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
 
-    # pylint:disable=attribute-defined-outside-init # noqa
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
+    cfg.VCS = section['VCS']
     cfg.style = section.get("style", "")
-    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
     cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
-    cfg.verbose = section.get("verbose")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None))
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
@@ -413,44 +508,54 @@
 LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.20 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
     git_date = "%(DOLLAR)sFormat:%%ci%(DOLLAR)s"
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
+
 
-def get_config():
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -460,46 +565,58 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None))
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
@@ -511,15 +628,19 @@
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -536,21 +657,21 @@
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -558,21 +679,25 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -628,48 +753,60 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long",
-                                     "--match", "%%s*" %% tag_prefix],
-                              cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
                              cwd=root)
     # --abbrev-ref was added in git-1.6.3
@@ -715,15 +852,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -740,35 +877,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -785,15 +922,15 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -815,31 +952,49 @@
         rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -858,15 +1013,15 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -887,15 +1042,15 @@
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -909,15 +1064,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -929,15 +1084,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -949,15 +1104,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
@@ -985,15 +1140,15 @@
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -1033,21 +1188,21 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -1055,21 +1210,25 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -1125,48 +1284,60 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long",
-                                     "--match", "%s*" % tag_prefix],
-                              cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
                              cwd=root)
     # --abbrev-ref was added in git-1.6.3
@@ -1212,15 +1383,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1237,65 +1408,70 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
-        versioneer_file = os.path.relpath(my_path)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
                         break
-    except EnvironmentError:
+    except OSError:
         pass
     if not present:
         with open(".gitattributes", "a+") as fobj:
             fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -1312,15 +1488,15 @@
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.20) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1329,50 +1505,49 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
                           indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1389,15 +1564,15 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -1419,31 +1594,49 @@
         rendered += "+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1462,15 +1655,15 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -1491,15 +1684,15 @@
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1513,15 +1706,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1533,15 +1726,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1553,15 +1746,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
@@ -1593,30 +1786,30 @@
             "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert cfg.versionfile_source is not None, \
         "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
@@ -1669,21 +1862,21 @@
         print("unable to compute version")
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools/distutils subclasses used by Versioneer.
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1697,114 +1890,124 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
     if 'build_py' in cmds:
-        _build_py = cmds['build_py']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+        _build_py: Any = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
     if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_ext import build_ext as _build_ext
+        _build_ext: Any = cmds['build_ext']
     else:
-        from distutils.command.build_ext import build_ext as _build_ext
+        from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
             if self.inplace:
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
+            if not cfg.versionfile_build:
+                return
             target_versionfile = os.path.join(self.build_lib,
                                               cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1819,18 +2022,21 @@
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
-        from py2exe.distutils_buildexe import py2exe as _py2exe
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1843,33 +2049,67 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info: Any = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
     if 'sdist' in cmds:
-        _sdist = cmds['sdist']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+        _sdist: Any = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
-            # pylint:disable=attribute-defined-outside-init # noqa
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1926,22 +2166,22 @@
 
 INIT_PY_SNIPPET = """
 from . import {0}
 __version__ = {0}.get_versions()['version']
 """
 
 
-def do_setup():
+def do_setup() -> int:
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1953,19 +2193,20 @@
                         "TAG_PREFIX": cfg.tag_prefix,
                         "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                         "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
         snippet = INIT_PY_SNIPPET.format(module)
         if OLD_SNIPPET in old:
             print(" replacing boilerplate in %s" % ipy)
             with open(ipy, "w") as f:
                 f.write(old.replace(OLD_SNIPPET, snippet))
@@ -1973,56 +2214,24 @@
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
                 f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -2051,14 +2260,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

