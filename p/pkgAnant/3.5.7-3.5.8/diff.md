# Comparing `tmp/pkgAnant-3.5.7.tar.gz` & `tmp/pkgAnant-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgAnant-3.5.7.tar", last modified: Mon Jul 31 06:06:04 2023, max compression
+gzip compressed data, was "pkgAnant-3.5.8.tar", last modified: Mon Jul 31 06:17:10 2023, max compression
```

## Comparing `pkgAnant-3.5.7.tar` & `pkgAnant-3.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:06:04.163726 pkgAnant-3.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 06:05:49.000000 pkgAnant-3.5.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:06:04.163726 pkgAnant-3.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 06:05:49.000000 pkgAnant-3.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:06:04.163726 pkgAnant-3.5.7/pkgAnant/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 06:05:49.000000 pkgAnant-3.5.7/pkgAnant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 06:05:49.000000 pkgAnant-3.5.7/pkgAnant/passwd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:06:04.163726 pkgAnant-3.5.7/pkgAnant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:06:03.000000 pkgAnant-3.5.7/pkgAnant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 06:06:04.000000 pkgAnant-3.5.7/pkgAnant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:06:03.000000 pkgAnant-3.5.7/pkgAnant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:06:03.000000 pkgAnant-3.5.7/pkgAnant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:06:04.163726 pkgAnant-3.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-31 06:06:02.000000 pkgAnant-3.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/pkgAnant/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/pkgAnant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/pkgAnant/passwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/pkgAnant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-31 06:16:59.000000 pkgAnant-3.5.8/setup.py
```

### Comparing `pkgAnant-3.5.7/LICENSE.txt` & `pkgAnant-3.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.5.7/README.md` & `pkgAnant-3.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.5.7/pkgAnant/passwd.py` & `pkgAnant-3.5.8/pkgAnant/passwd.py`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.5.7/setup.py` & `pkgAnant-3.5.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 import os
 
 # Get the version from the environment variable (RELEASE_VERSION) set by the GitHub Action workflow
-version = os.getenv("RELEASE_VERSION", "3.5.7")  # Provide a default version if RELEASE_VERSION is not set
+version = os.getenv("RELEASE_VERSION", "3.5.8")  # Provide a default version if RELEASE_VERSION is not set
 
 setuptools.setup(
     name="pkgAnant",
     version=version,
     author="Anant Chaudhary",
     description="password generator package",
     long_description_content_type="text/markdown",
```

