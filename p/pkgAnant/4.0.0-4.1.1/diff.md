# Comparing `tmp/pkgAnant-4.0.0.tar.gz` & `tmp/pkgAnant-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgAnant-4.0.0.tar", last modified: Mon Jul 31 06:53:11 2023, max compression
+gzip compressed data, was "pkgAnant-4.1.1.tar", last modified: Mon Jul 31 07:00:49 2023, max compression
```

## Comparing `pkgAnant-4.0.0.tar` & `pkgAnant-4.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/pkgAnant/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/pkgAnant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/pkgAnant/passwd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/pkgAnant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 06:53:10.000000 pkgAnant-4.0.0/pkgAnant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 06:53:11.000000 pkgAnant-4.0.0/pkgAnant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:53:10.000000 pkgAnant-4.0.0/pkgAnant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:53:10.000000 pkgAnant-4.0.0/pkgAnant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:53:11.749632 pkgAnant-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 06:52:47.000000 pkgAnant-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:00:49.809218 pkgAnant-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 07:00:28.000000 pkgAnant-4.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 07:00:49.809218 pkgAnant-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 07:00:28.000000 pkgAnant-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:00:49.809218 pkgAnant-4.1.1/pkgAnant/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 07:00:28.000000 pkgAnant-4.1.1/pkgAnant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 07:00:28.000000 pkgAnant-4.1.1/pkgAnant/passwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:00:49.809218 pkgAnant-4.1.1/pkgAnant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 07:00:49.000000 pkgAnant-4.1.1/pkgAnant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 07:00:49.000000 pkgAnant-4.1.1/pkgAnant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 07:00:49.000000 pkgAnant-4.1.1/pkgAnant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 07:00:49.000000 pkgAnant-4.1.1/pkgAnant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 07:00:49.809218 pkgAnant-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 07:00:28.000000 pkgAnant-4.1.1/setup.py
```

### Comparing `pkgAnant-4.0.0/LICENSE.txt` & `pkgAnant-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgAnant-4.0.0/README.md` & `pkgAnant-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pkgAnant-4.0.0/pkgAnant/passwd.py` & `pkgAnant-4.1.1/pkgAnant/passwd.py`

 * *Files identical despite different names*

### Comparing `pkgAnant-4.0.0/setup.py` & `pkgAnant-4.1.1/setup.py`

 * *Files identical despite different names*

