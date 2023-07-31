# Comparing `tmp/moderne_visualizations_misc-0.1.0.tar.gz` & `tmp/moderne_visualizations_misc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderne_visualizations_misc-0.1.0.tar", last modified: Mon Jul 31 15:14:09 2023, max compression
+gzip compressed data, was "moderne_visualizations_misc-0.1.1.tar", last modified: Mon Jul 31 15:46:57 2023, max compression
```

## Comparing `moderne_visualizations_misc-0.1.0.tar` & `moderne_visualizations_misc-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:14:09.054593 moderne_visualizations_misc-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 15:14:09.054593 moderne_visualizations_misc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 15:13:47.000000 moderne_visualizations_misc-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:14:09.054593 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:13:47.000000 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:14:09.054593 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 15:14:09.000000 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 15:14:09.000000 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:14:09.000000 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 15:14:09.000000 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 15:14:09.000000 moderne_visualizations_misc-0.1.0/moderne_visualizations_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-31 15:13:47.000000 moderne_visualizations_misc-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:14:09.054593 moderne_visualizations_misc-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:46:57.088008 moderne_visualizations_misc-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 15:46:57.088008 moderne_visualizations_misc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 15:46:33.000000 moderne_visualizations_misc-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:46:57.088008 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:46:33.000000 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:46:57.088008 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 15:46:57.000000 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 15:46:57.000000 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:46:57.000000 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 15:46:57.000000 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 15:46:57.000000 moderne_visualizations_misc-0.1.1/moderne_visualizations_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-31 15:46:33.000000 moderne_visualizations_misc-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:46:57.088008 moderne_visualizations_misc-0.1.1/setup.cfg
```

