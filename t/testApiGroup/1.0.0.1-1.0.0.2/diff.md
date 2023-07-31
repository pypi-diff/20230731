# Comparing `tmp/testApiGroup-1.0.0.1.tar.gz` & `tmp/testApiGroup-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.1.tar", last modified: Mon Jul 31 05:23:17 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.2.tar", last modified: Mon Jul 31 06:16:40 2023, max compression
```

## Comparing `testApiGroup-1.0.0.1.tar` & `testApiGroup-1.0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 05:23:17.919393 testApiGroup-1.0.0.1/
--rw-rw-rw-   0        0        0      129 2023-07-31 05:23:17.918570 testApiGroup-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 05:23:17.919393 testApiGroup-1.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 05:23:17.907393 testApiGroup-1.0.0.1/testApiGroup/
--rw-rw-rw-   0        0        0      289 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup/setup.py
--rw-rw-rw-   0        0        0     1120 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup/testApiGroup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:23:17.915392 testApiGroup-1.0.0.1/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:16:40.576771 testApiGroup-1.0.0.2/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:16:40.575760 testApiGroup-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:16:40.577760 testApiGroup-1.0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 06:16:40.553762 testApiGroup-1.0.0.2/testApiGroup/
+-rw-rw-rw-   0        0        0      289 2023-07-31 06:16:39.000000 testApiGroup-1.0.0.2/testApiGroup/setup.py
+-rw-rw-rw-   0        0        0     1120 2023-07-31 06:16:39.000000 testApiGroup-1.0.0.2/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:16:40.572356 testApiGroup-1.0.0.2/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:16:40.000000 testApiGroup-1.0.0.2/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-31 06:16:40.000000 testApiGroup-1.0.0.2/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:16:40.000000 testApiGroup-1.0.0.2/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 06:16:40.000000 testApiGroup-1.0.0.2/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 06:16:40.000000 testApiGroup-1.0.0.2/testApiGroup.egg-info/top_level.txt
```

### Comparing `testApiGroup-1.0.0.1/testApiGroup/testApiGroup.py` & `testApiGroup-1.0.0.2/testApiGroup/testApiGroup.py`

 * *Files identical despite different names*

