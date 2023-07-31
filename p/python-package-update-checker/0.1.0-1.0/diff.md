# Comparing `tmp/python_package_update_checker-0.1.0.tar.gz` & `tmp/python_package_update_checker-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_package_update_checker-0.1.0.tar", last modified: Mon Jul 31 16:58:32 2023, max compression
+gzip compressed data, was "python_package_update_checker-1.0.tar", last modified: Mon Jul 31 16:43:55 2023, max compression
```

## Comparing `python_package_update_checker-0.1.0.tar` & `python_package_update_checker-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:58:32.655958 python_package_update_checker-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 python_package_update_checker-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      210 2023-07-31 16:58:32.654993 python_package_update_checker-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5884 2023-07-31 16:09:26.000000 python_package_update_checker-0.1.0/PythonPackageUpdateChecker.py
--rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 python_package_update_checker-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:58:32.653962 python_package_update_checker-0.1.0/python_package_update_checker.egg-info/
--rw-rw-rw-   0        0        0      210 2023-07-31 16:58:32.000000 python_package_update_checker-0.1.0/python_package_update_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-31 16:58:32.000000 python_package_update_checker-0.1.0/python_package_update_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:58:32.000000 python_package_update_checker-0.1.0/python_package_update_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:58:32.000000 python_package_update_checker-0.1.0/python_package_update_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 16:58:32.655958 python_package_update_checker-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      371 2023-07-31 16:55:37.000000 python_package_update_checker-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:43:55.951204 python_package_update_checker-1.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 python_package_update_checker-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      170 2023-07-31 16:43:55.950207 python_package_update_checker-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5884 2023-07-31 16:09:26.000000 python_package_update_checker-1.0/PythonPackageUpdateChecker.py
+-rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 python_package_update_checker-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:43:55.949210 python_package_update_checker-1.0/python_package_update_checker.egg-info/
+-rw-rw-rw-   0        0        0      170 2023-07-31 16:43:55.000000 python_package_update_checker-1.0/python_package_update_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-31 16:43:55.000000 python_package_update_checker-1.0/python_package_update_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:43:55.000000 python_package_update_checker-1.0/python_package_update_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:43:55.000000 python_package_update_checker-1.0/python_package_update_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:43:55.951204 python_package_update_checker-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-07-31 16:43:45.000000 python_package_update_checker-1.0/setup.py
```

### Comparing `python_package_update_checker-0.1.0/LICENSE.txt` & `python_package_update_checker-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_package_update_checker-0.1.0/PythonPackageUpdateChecker.py` & `python_package_update_checker-1.0/PythonPackageUpdateChecker.py`

 * *Files identical despite different names*

### Comparing `python_package_update_checker-0.1.0/README.md` & `python_package_update_checker-1.0/README.md`

 * *Files identical despite different names*

