# Comparing `tmp/tortoise_api_model-0.0.6.tar.gz` & `tmp/tortoise_api_model-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.0.6.tar", last modified: Fri Jul 28 19:29:09 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.0.7.tar", last modified: Mon Jul 31 08:43:23 2023, max compression
```

## Comparing `tortoise_api_model-0.0.6.tar` & `tortoise_api_model-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:29:09.697956 tortoise_api_model-0.0.6/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-28 19:29:09.697739 tortoise_api_model-0.0.6/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 19:29:09.698016 tortoise_api_model-0.0.6/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-28 18:12:45.000000 tortoise_api_model-0.0.6/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:29:09.696027 tortoise_api_model-0.0.6/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)       50 2023-07-25 15:09:00.000000 tortoise_api_model-0.0.6/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)      921 2023-07-28 18:00:16.000000 tortoise_api_model-0.0.6/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:29:09.697471 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:43:23.155046 tortoise_api_model-0.0.7/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 08:43:23.154822 tortoise_api_model-0.0.7/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 08:43:23.155107 tortoise_api_model-0.0.7/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-31 08:43:02.000000 tortoise_api_model-0.0.7/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:43:23.153413 tortoise_api_model-0.0.7/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)       90 2023-07-30 17:17:05.000000 tortoise_api_model-0.0.7/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     1595 2023-07-30 20:10:46.000000 tortoise_api_model-0.0.7/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:43:23.154549 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.0.6/setup.py` & `tortoise_api_model-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

