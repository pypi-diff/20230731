# Comparing `tmp/newPassword-1.1.9.9.tar.gz` & `tmp/newPassword-2.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newPassword-1.1.9.9.tar", last modified: Mon Jul 31 06:42:32 2023, max compression
+gzip compressed data, was "newPassword-2.1.1.1.tar", last modified: Mon Jul 31 06:45:08 2023, max compression
```

## Comparing `newPassword-1.1.9.9.tar` & `newPassword-2.1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:42:32.855376 newPassword-1.1.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 06:42:14.000000 newPassword-1.1.9.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 06:42:32.855376 newPassword-1.1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-31 06:42:14.000000 newPassword-1.1.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:42:32.855376 newPassword-1.1.9.9/newPassword/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 06:42:14.000000 newPassword-1.1.9.9/newPassword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-31 06:42:14.000000 newPassword-1.1.9.9/newPassword/passwordGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:42:32.855376 newPassword-1.1.9.9/newPassword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 06:42:32.000000 newPassword-1.1.9.9/newPassword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 06:42:32.000000 newPassword-1.1.9.9/newPassword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:42:32.000000 newPassword-1.1.9.9/newPassword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 06:42:32.000000 newPassword-1.1.9.9/newPassword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:42:32.855376 newPassword-1.1.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 06:42:14.000000 newPassword-1.1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:45:08.132016 newPassword-2.1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 06:44:46.000000 newPassword-2.1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 06:45:08.132016 newPassword-2.1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-31 06:44:46.000000 newPassword-2.1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:45:08.132016 newPassword-2.1.1.1/newPassword/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 06:44:46.000000 newPassword-2.1.1.1/newPassword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-31 06:44:46.000000 newPassword-2.1.1.1/newPassword/passwordGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:45:08.132016 newPassword-2.1.1.1/newPassword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 06:45:08.000000 newPassword-2.1.1.1/newPassword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 06:45:08.000000 newPassword-2.1.1.1/newPassword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:45:08.000000 newPassword-2.1.1.1/newPassword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 06:45:08.000000 newPassword-2.1.1.1/newPassword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:45:08.132016 newPassword-2.1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 06:44:46.000000 newPassword-2.1.1.1/setup.py
```

### Comparing `newPassword-1.1.9.9/LICENSE.txt` & `newPassword-2.1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newPassword-1.1.9.9/README.md` & `newPassword-2.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `newPassword-1.1.9.9/setup.py` & `newPassword-2.1.1.1/setup.py`

 * *Files identical despite different names*

