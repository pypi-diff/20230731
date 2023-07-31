# Comparing `tmp/ethcx-0.0.2.tar.gz` & `tmp/ethcx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethcx-0.0.2.tar", last modified: Mon Jul 31 16:34:01 2023, max compression
+gzip compressed data, was "ethcx-0.0.3.tar", last modified: Mon Jul 31 16:31:57 2023, max compression
```

## Comparing `ethcx-0.0.2.tar` & `ethcx-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/
--rw-r--r--   0 honululu  (1000) honululu  (1000)     1080 2023-07-25 15:15:47.000000 ethcx-0.0.2/LICENSE
--rw-r--r--   0 honululu  (1000) honululu  (1000)       96 2023-07-25 15:15:48.000000 ethcx-0.0.2/MANIFEST.in
--rw-rw-r--   0 honululu  (1000) honululu  (1000)     2824 2023-07-31 16:34:01.725033 ethcx-0.0.2/PKG-INFO
--rw-r--r--   0 honululu  (1000) honululu  (1000)     2051 2023-07-25 15:15:49.000000 ethcx-0.0.2/README.md
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/ethcx/
--rw-r--r--   0 honululu  (1000) honululu  (1000)      956 2023-07-26 18:24:19.000000 ethcx-0.0.2/ethcx/__init__.py
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/ethcx/compilers/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        0 2023-07-27 13:07:43.000000 ethcx-0.0.2/ethcx/compilers/__init__.py
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/ethcx/compilers/solidity/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        0 2023-07-27 13:08:06.000000 ethcx-0.0.2/ethcx/compilers/solidity/__init__.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)    22302 2023-07-27 11:17:32.000000 ethcx-0.0.2/ethcx/compilers/solidity/install.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)    16043 2023-07-27 11:19:01.000000 ethcx-0.0.2/ethcx/compilers/solidity/main.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)     6076 2023-07-27 11:18:51.000000 ethcx-0.0.2/ethcx/compilers/solidity/wrapper.py
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/ethcx/compilers/vyper/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        0 2023-07-27 13:07:51.000000 ethcx-0.0.2/ethcx/compilers/vyper/__init__.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)    23265 2023-07-27 00:23:43.000000 ethcx-0.0.2/ethcx/compilers/vyper/install.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)    15097 2023-07-27 01:01:53.000000 ethcx-0.0.2/ethcx/compilers/vyper/main.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)     5831 2023-07-25 13:59:02.000000 ethcx-0.0.2/ethcx/compilers/vyper/wrapper.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)     1540 2023-07-26 21:36:29.000000 ethcx-0.0.2/ethcx/exceptions.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)     2519 2023-07-24 14:28:48.000000 ethcx-0.0.2/ethcx/lock.py
--rw-r--r--   0 honululu  (1000) honululu  (1000)     2809 2023-07-26 18:25:00.000000 ethcx-0.0.2/ethcx/utils.py
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/ethcx.egg-info/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)     2824 2023-07-31 16:34:01.000000 ethcx-0.0.2/ethcx.egg-info/PKG-INFO
--rw-rw-r--   0 honululu  (1000) honululu  (1000)      624 2023-07-31 16:34:01.000000 ethcx-0.0.2/ethcx.egg-info/SOURCES.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        1 2023-07-31 16:34:01.000000 ethcx-0.0.2/ethcx.egg-info/dependency_links.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        1 2023-07-31 16:31:25.000000 ethcx-0.0.2/ethcx.egg-info/not-zip-safe
--rw-rw-r--   0 honululu  (1000) honululu  (1000)       58 2023-07-31 16:34:01.000000 ethcx-0.0.2/ethcx.egg-info/requires.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        6 2023-07-31 16:34:01.000000 ethcx-0.0.2/ethcx.egg-info/top_level.txt
--rw-r--r--   0 honululu  (1000) honululu  (1000)      245 2023-07-24 14:28:48.000000 ethcx-0.0.2/pyproject.toml
--rw-r--r--   0 honululu  (1000) honululu  (1000)      518 2023-07-31 16:34:01.725033 ethcx-0.0.2/setup.cfg
--rw-r--r--   0 honululu  (1000) honululu  (1000)     1298 2023-07-31 16:33:57.000000 ethcx-0.0.2/setup.py
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:34:01.725033 ethcx-0.0.2/tests/
--rw-r--r--   0 honululu  (1000) honululu  (1000)     2527 2023-07-24 14:28:48.000000 ethcx-0.0.2/tests/test_wrapper.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.844201 ethcx-0.0.3/
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     1080 2023-07-25 15:15:47.000000 ethcx-0.0.3/LICENSE
+-rw-r--r--   0 honululu  (1000) honululu  (1000)       96 2023-07-25 15:15:48.000000 ethcx-0.0.3/MANIFEST.in
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)     2824 2023-07-31 16:31:57.844201 ethcx-0.0.3/PKG-INFO
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     2051 2023-07-25 15:15:49.000000 ethcx-0.0.3/README.md
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.840201 ethcx-0.0.3/ethcx/
+-rw-r--r--   0 honululu  (1000) honululu  (1000)      956 2023-07-26 18:24:19.000000 ethcx-0.0.3/ethcx/__init__.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.840201 ethcx-0.0.3/ethcx/compilers/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        0 2023-07-27 13:07:43.000000 ethcx-0.0.3/ethcx/compilers/__init__.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.840201 ethcx-0.0.3/ethcx/compilers/solidity/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        0 2023-07-27 13:08:06.000000 ethcx-0.0.3/ethcx/compilers/solidity/__init__.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)    22302 2023-07-27 11:17:32.000000 ethcx-0.0.3/ethcx/compilers/solidity/install.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)    16043 2023-07-27 11:19:01.000000 ethcx-0.0.3/ethcx/compilers/solidity/main.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     6076 2023-07-27 11:18:51.000000 ethcx-0.0.3/ethcx/compilers/solidity/wrapper.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.844201 ethcx-0.0.3/ethcx/compilers/vyper/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        0 2023-07-27 13:07:51.000000 ethcx-0.0.3/ethcx/compilers/vyper/__init__.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)    23265 2023-07-27 00:23:43.000000 ethcx-0.0.3/ethcx/compilers/vyper/install.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)    15097 2023-07-27 01:01:53.000000 ethcx-0.0.3/ethcx/compilers/vyper/main.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     5831 2023-07-25 13:59:02.000000 ethcx-0.0.3/ethcx/compilers/vyper/wrapper.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     1540 2023-07-26 21:36:29.000000 ethcx-0.0.3/ethcx/exceptions.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     2519 2023-07-24 14:28:48.000000 ethcx-0.0.3/ethcx/lock.py
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     2809 2023-07-26 18:25:00.000000 ethcx-0.0.3/ethcx/utils.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.840201 ethcx-0.0.3/ethcx.egg-info/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)     2824 2023-07-31 16:31:57.000000 ethcx-0.0.3/ethcx.egg-info/PKG-INFO
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)      624 2023-07-31 16:31:57.000000 ethcx-0.0.3/ethcx.egg-info/SOURCES.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        1 2023-07-31 16:31:57.000000 ethcx-0.0.3/ethcx.egg-info/dependency_links.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        1 2023-07-31 16:31:25.000000 ethcx-0.0.3/ethcx.egg-info/not-zip-safe
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)       58 2023-07-31 16:31:57.000000 ethcx-0.0.3/ethcx.egg-info/requires.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        6 2023-07-31 16:31:57.000000 ethcx-0.0.3/ethcx.egg-info/top_level.txt
+-rw-r--r--   0 honululu  (1000) honululu  (1000)      245 2023-07-24 14:28:48.000000 ethcx-0.0.3/pyproject.toml
+-rw-r--r--   0 honululu  (1000) honululu  (1000)      518 2023-07-31 16:31:57.844201 ethcx-0.0.3/setup.cfg
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     1298 2023-07-31 16:30:25.000000 ethcx-0.0.3/setup.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 16:31:57.844201 ethcx-0.0.3/tests/
+-rw-r--r--   0 honululu  (1000) honululu  (1000)     2527 2023-07-24 14:28:48.000000 ethcx-0.0.3/tests/test_wrapper.py
```

### Comparing `ethcx-0.0.2/LICENSE` & `ethcx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/PKG-INFO` & `ethcx-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethcx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper and version management tool for ethereum-targeting compilers.
 Home-page: https://github.com/ethpwn/ethcx
 Author: Lukas Dresel (forked from py-solc-x by Ben Hause)
 Author-email: Lukas-Dresel@users.noreply.github.com
 License: MIT
 Keywords: ethereum solidity solc vyper
 Classifier: Intended Audience :: Developers
```

### Comparing `ethcx-0.0.2/README.md` & `ethcx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/__init__.py` & `ethcx-0.0.3/ethcx/__init__.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/compilers/solidity/install.py` & `ethcx-0.0.3/ethcx/compilers/solidity/install.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/compilers/solidity/main.py` & `ethcx-0.0.3/ethcx/compilers/solidity/main.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/compilers/solidity/wrapper.py` & `ethcx-0.0.3/ethcx/compilers/solidity/wrapper.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/compilers/vyper/install.py` & `ethcx-0.0.3/ethcx/compilers/vyper/install.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/compilers/vyper/main.py` & `ethcx-0.0.3/ethcx/compilers/vyper/main.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/compilers/vyper/wrapper.py` & `ethcx-0.0.3/ethcx/compilers/vyper/wrapper.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/exceptions.py` & `ethcx-0.0.3/ethcx/exceptions.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/lock.py` & `ethcx-0.0.3/ethcx/lock.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx/utils.py` & `ethcx-0.0.3/ethcx/utils.py`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/ethcx.egg-info/PKG-INFO` & `ethcx-0.0.3/ethcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethcx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper and version management tool for ethereum-targeting compilers.
 Home-page: https://github.com/ethpwn/ethcx
 Author: Lukas Dresel (forked from py-solc-x by Ben Hause)
 Author-email: Lukas-Dresel@users.noreply.github.com
 License: MIT
 Keywords: ethereum solidity solc vyper
 Classifier: Intended Audience :: Developers
```

### Comparing `ethcx-0.0.2/ethcx.egg-info/SOURCES.txt` & `ethcx-0.0.3/ethcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/setup.cfg` & `ethcx-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ethcx-0.0.2/setup.py` & `ethcx-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 setup(
     name="ethcx",
-    version="0.0.2",  # don't change this manually, use bumpversion instead
+    version="0.0.3",  # don't change this manually, use bumpversion instead
     description="Python wrapper and version management tool for ethereum-targeting compilers.",
     long_description=readme,
     author="Lukas Dresel (forked from py-solc-x by Ben Hause)",
     author_email="Lukas-Dresel@users.noreply.github.com",
     url="https://github.com/ethpwn/ethcx",
     include_package_data=True,
     py_modules=["ethcx"],
```

### Comparing `ethcx-0.0.2/tests/test_wrapper.py` & `ethcx-0.0.3/tests/test_wrapper.py`

 * *Files identical despite different names*

