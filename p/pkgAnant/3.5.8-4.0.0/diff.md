# Comparing `tmp/pkgAnant-3.5.8.tar.gz` & `tmp/pkgAnant-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgAnant-3.5.8.tar", last modified: Mon Jul 31 06:17:10 2023, max compression
+gzip compressed data, was "pkgAnant-4.0.0.tar", last modified: Mon Jul 31 06:53:11 2023, max compression
```

## Comparing `pkgAnant-3.5.8.tar` & `pkgAnant-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/pkgAnant/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/pkgAnant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 06:16:58.000000 pkgAnant-3.5.8/pkgAnant/passwd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/pkgAnant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:17:10.000000 pkgAnant-3.5.8/pkgAnant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:17:10.696114 pkgAnant-3.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-31 06:16:59.000000 pkgAnant-3.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/pkgAnant/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/pkgAnant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/pkgAnant/passwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/pkgAnant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:53:10.000000 pkgAnant-4.0.0/pkgAnant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 06:53:11.000000 pkgAnant-4.0.0/pkgAnant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:53:10.000000 pkgAnant-4.0.0/pkgAnant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:53:10.000000 pkgAnant-4.0.0/pkgAnant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/setup.py
```

### Comparing `pkgAnant-3.5.8/LICENSE.txt` & `pkgAnant-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.5.8/README.md` & `pkgAnant-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.5.8/pkgAnant/passwd.py` & `pkgAnant-4.0.0/pkgAnant/passwd.py`

 * *Files identical despite different names*

### Comparing `pkgAnant-3.5.8/setup.py` & `pkgAnant-4.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import setuptools
-import os
-
-# Get the version from the environment variable (RELEASE_VERSION) set by the GitHub Action workflow
-version = os.getenv("RELEASE_VERSION", "3.5.8")  # Provide a default version if RELEASE_VERSION is not set
+from version import ver
 
 setuptools.setup(
     name="pkgAnant",
-    version=version,
+    version=ver,
     author="Anant Chaudhary",
     description="password generator package",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

