# Comparing `tmp/testApiGroup-1.0.0.3.tar.gz` & `tmp/testApiGroup-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.3.tar", last modified: Mon Jul 31 06:30:00 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.4.tar", last modified: Mon Jul 31 06:33:33 2023, max compression
```

## Comparing `testApiGroup-1.0.0.3.tar` & `testApiGroup-1.0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:30:00.801101 testApiGroup-1.0.0.3/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:30:00.799139 testApiGroup-1.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 06:30:00.801101 testApiGroup-1.0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 06:30:00.768104 testApiGroup-1.0.0.3/testApiGroup/
--rw-rw-rw-   0        0        0      289 2023-07-31 06:29:59.000000 testApiGroup-1.0.0.3/testApiGroup/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:30:00.795099 testApiGroup-1.0.0.3/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:30:00.000000 testApiGroup-1.0.0.3/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-31 06:30:00.000000 testApiGroup-1.0.0.3/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:30:00.000000 testApiGroup-1.0.0.3/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 06:30:00.000000 testApiGroup-1.0.0.3/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 06:30:00.000000 testApiGroup-1.0.0.3/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:33:33.942099 testApiGroup-1.0.0.4/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:33:33.854189 testApiGroup-1.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:33:33.943124 testApiGroup-1.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:33:33.833137 testApiGroup-1.0.0.4/testApiGroup/
+-rw-rw-rw-   0        0        0     1120 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:33:33.849136 testApiGroup-1.0.0.4/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 06:33:33.000000 testApiGroup-1.0.0.4/testApiGroup.egg-info/top_level.txt
```

