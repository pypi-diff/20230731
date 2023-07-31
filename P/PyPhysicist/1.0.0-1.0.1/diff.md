# Comparing `tmp/PyPhysicist-1.0.0.tar.gz` & `tmp/PyPhysicist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyPhysicist-1.0.0.tar", last modified: Mon Jul 31 09:24:30 2023, max compression
+gzip compressed data, was "dist\PyPhysicist-1.0.1.tar", last modified: Mon Jul 31 10:38:56 2023, max compression
```

## Comparing `PyPhysicist-1.0.0.tar` & `PyPhysicist-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/
--rw-rw-rw-   0        0        0      237 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/PyPhysicist.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/PyPhysicist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/PyPhysicist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/PyPhysicist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/PyPhysicist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 09:24:30.000000 PyPhysicist-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      239 2023-07-31 09:24:00.000000 PyPhysicist-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/
+-rw-rw-rw-   0        0        0      237 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/PyPhysicist.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/PyPhysicist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/PyPhysicist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/PyPhysicist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/PyPhysicist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 10:38:56.000000 PyPhysicist-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      239 2023-07-31 09:28:08.000000 PyPhysicist-1.0.1/setup.py
```

