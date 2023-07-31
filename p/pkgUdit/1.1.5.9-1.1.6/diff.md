# Comparing `tmp/pkgUdit-1.1.5.9.tar.gz` & `tmp/pkgUdit-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgUdit-1.1.5.9.tar", last modified: Fri Jul 28 09:38:36 2023, max compression
+gzip compressed data, was "pkgUdit-1.1.6.tar", last modified: Mon Jul 31 07:02:53 2023, max compression
```

## Comparing `pkgUdit-1.1.5.9.tar` & `pkgUdit-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/pkgUdit/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/pkgUdit/data/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/data/Names.csv
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/data/Places.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/pswdGen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/pkgUdit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:02:53.835549 pkgUdit-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 07:02:53.835549 pkgUdit-1.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:02:53.831549 pkgUdit-1.1.6/pkgUdit/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 07:02:36.000000 pkgUdit-1.1.6/pkgUdit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-31 07:02:36.000000 pkgUdit-1.1.6/pkgUdit/pswdGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-31 07:02:36.000000 pkgUdit-1.1.6/pkgUdit/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 07:02:52.000000 pkgUdit-1.1.6/pkgUdit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:02:53.831549 pkgUdit-1.1.6/pkgUdit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 07:02:53.000000 pkgUdit-1.1.6/pkgUdit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 07:02:53.000000 pkgUdit-1.1.6/pkgUdit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 07:02:53.000000 pkgUdit-1.1.6/pkgUdit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 07:02:53.000000 pkgUdit-1.1.6/pkgUdit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 07:02:53.835549 pkgUdit-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-31 07:02:36.000000 pkgUdit-1.1.6/setup.py
```

### Comparing `pkgUdit-1.1.5.9/pkgUdit/pswdGen.py` & `pkgUdit-1.1.6/pkgUdit/pswdGen.py`

 * *Files identical despite different names*

### Comparing `pkgUdit-1.1.5.9/pkgUdit/test.py` & `pkgUdit-1.1.6/pkgUdit/test.py`

 * *Files identical despite different names*

