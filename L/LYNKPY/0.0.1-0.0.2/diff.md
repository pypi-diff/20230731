# Comparing `tmp/LYNKPY-0.0.1.tar.gz` & `tmp/LYNKPY-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LYNKPY-0.0.1.tar", last modified: Mon Jul 31 08:54:46 2023, max compression
+gzip compressed data, was "LYNKPY-0.0.2.tar", last modified: Mon Jul 31 09:11:24 2023, max compression
```

## Comparing `LYNKPY-0.0.1.tar` & `LYNKPY-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 08:54:46.101447 LYNKPY-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-31 08:54:46.079590 LYNKPY-0.0.1/LYNKPY.egg-info/
--rw-rw-rw-   0        0        0      234 2023-07-31 08:54:44.000000 LYNKPY-0.0.1/LYNKPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-31 08:54:45.000000 LYNKPY-0.0.1/LYNKPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:54:44.000000 LYNKPY-0.0.1/LYNKPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-31 08:54:44.000000 LYNKPY-0.0.1/LYNKPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:54:44.000000 LYNKPY-0.0.1/LYNKPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      234 2023-07-31 08:54:46.095549 LYNKPY-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 08:54:46.102447 LYNKPY-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      488 2023-07-31 08:54:02.000000 LYNKPY-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:11:24.829046 LYNKPY-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-31 09:11:24.818531 LYNKPY-0.0.2/LYNKPY.egg-info/
+-rw-rw-rw-   0        0        0      234 2023-07-31 09:11:24.000000 LYNKPY-0.0.2/LYNKPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-31 09:11:24.000000 LYNKPY-0.0.2/LYNKPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:11:24.000000 LYNKPY-0.0.2/LYNKPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-31 09:11:24.000000 LYNKPY-0.0.2/LYNKPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:11:24.000000 LYNKPY-0.0.2/LYNKPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      234 2023-07-31 09:11:24.826611 LYNKPY-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:11:24.829847 LYNKPY-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-07-31 09:11:05.000000 LYNKPY-0.0.2/setup.py
```

