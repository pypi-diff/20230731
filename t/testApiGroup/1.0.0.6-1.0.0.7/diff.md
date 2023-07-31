# Comparing `tmp/testApiGroup-1.0.0.6.tar.gz` & `tmp/testApiGroup-1.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.6.tar", last modified: Mon Jul 31 06:44:06 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.7.tar", last modified: Mon Jul 31 06:50:43 2023, max compression
```

## Comparing `testApiGroup-1.0.0.6.tar` & `testApiGroup-1.0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:44:06.551614 testApiGroup-1.0.0.6/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:44:06.542533 testApiGroup-1.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 06:44:06.553616 testApiGroup-1.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      281 2023-07-31 06:44:05.000000 testApiGroup-1.0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:44:06.476247 testApiGroup-1.0.0.6/testApiGroup/
--rw-rw-rw-   0        0        0     1122 2023-07-31 06:44:05.000000 testApiGroup-1.0.0.6/testApiGroup/testApiGroup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:44:06.525302 testApiGroup-1.0.0.6/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:50:43.273041 testApiGroup-1.0.0.7/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:50:43.272174 testApiGroup-1.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:50:43.273041 testApiGroup-1.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      281 2023-07-31 06:50:42.000000 testApiGroup-1.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:50:43.257042 testApiGroup-1.0.0.7/testApiGroup/
+-rw-rw-rw-   0        0        0     1122 2023-07-31 06:50:42.000000 testApiGroup-1.0.0.7/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:50:43.269041 testApiGroup-1.0.0.7/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/top_level.txt
```

### Comparing `testApiGroup-1.0.0.6/testApiGroup/testApiGroup.py` & `testApiGroup-1.0.0.7/testApiGroup/testApiGroup.py`

 * *Files identical despite different names*

