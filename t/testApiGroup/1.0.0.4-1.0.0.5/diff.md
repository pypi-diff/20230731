# Comparing `tmp/testApiGroup-1.0.0.4.tar.gz` & `tmp/testApiGroup-1.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.4.tar", last modified: Mon Jul 31 06:33:33 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.5.tar", last modified: Mon Jul 31 06:41:35 2023, max compression
```

## Comparing `testApiGroup-1.0.0.4.tar` & `testApiGroup-1.0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:33:33.942099 testApiGroup-1.0.0.4/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:33:33.854189 testApiGroup-1.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 06:33:33.943124 testApiGroup-1.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:33:33.833137 testApiGroup-1.0.0.4/testApiGroup/
--rw-rw-rw-   0        0        0     1120 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup/testApiGroup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:33:33.849136 testApiGroup-1.0.0.4/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:41:35.440784 testApiGroup-1.0.0.5/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:41:35.439785 testApiGroup-1.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:41:35.440784 testApiGroup-1.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      281 2023-07-31 06:41:34.000000 testApiGroup-1.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:41:35.322019 testApiGroup-1.0.0.5/testApiGroup/
+-rw-rw-rw-   0        0        0     1120 2023-07-31 06:41:34.000000 testApiGroup-1.0.0.5/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:41:35.437786 testApiGroup-1.0.0.5/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/top_level.txt
```

### Comparing `testApiGroup-1.0.0.4/testApiGroup/testApiGroup.py` & `testApiGroup-1.0.0.5/testApiGroup/testApiGroup.py`

 * *Files identical despite different names*

