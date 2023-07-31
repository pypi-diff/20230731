# Comparing `tmp/newPassword-0.0.0.tar.gz` & `tmp/newPassword-1.1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newPassword-0.0.0.tar", last modified: Mon Jul 31 06:36:51 2023, max compression
+gzip compressed data, was "newPassword-1.1.7.7.tar", last modified: Mon Jul 31 06:05:11 2023, max compression
```

## Comparing `newPassword-0.0.0.tar` & `newPassword-1.1.7.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:36:51.702374 newPassword-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 06:36:32.000000 newPassword-0.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 06:36:51.702374 newPassword-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-31 06:36:32.000000 newPassword-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:36:51.702374 newPassword-0.0.0/newPassword/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 06:36:32.000000 newPassword-0.0.0/newPassword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-31 06:36:32.000000 newPassword-0.0.0/newPassword/passwordGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:36:51.702374 newPassword-0.0.0/newPassword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 06:36:51.000000 newPassword-0.0.0/newPassword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 06:36:51.000000 newPassword-0.0.0/newPassword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:36:51.000000 newPassword-0.0.0/newPassword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 06:36:51.000000 newPassword-0.0.0/newPassword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:36:51.702374 newPassword-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 06:36:32.000000 newPassword-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:05:11.098463 newPassword-1.1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 06:04:53.000000 newPassword-1.1.7.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 06:05:11.098463 newPassword-1.1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-31 06:04:53.000000 newPassword-1.1.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:05:11.098463 newPassword-1.1.7.7/newPassword/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 06:04:53.000000 newPassword-1.1.7.7/newPassword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-31 06:04:53.000000 newPassword-1.1.7.7/newPassword/passwordGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:05:11.098463 newPassword-1.1.7.7/newPassword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 06:05:11.000000 newPassword-1.1.7.7/newPassword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 06:05:11.000000 newPassword-1.1.7.7/newPassword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:05:11.000000 newPassword-1.1.7.7/newPassword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 06:05:11.000000 newPassword-1.1.7.7/newPassword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:05:11.098463 newPassword-1.1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 06:04:53.000000 newPassword-1.1.7.7/setup.py
```

### Comparing `newPassword-0.0.0/LICENSE.txt` & `newPassword-1.1.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newPassword-0.0.0/README.md` & `newPassword-1.1.7.7/README.md`

 * *Files identical despite different names*

