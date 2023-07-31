# Comparing `tmp/MedPalm-0.0.1.tar.gz` & `tmp/MedPalm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedPalm-0.0.1.tar", last modified: Mon Jul 31 04:14:47 2023, max compression
+gzip compressed data, was "MedPalm-0.0.2.tar", last modified: Mon Jul 31 04:24:24 2023, max compression
```

## Comparing `MedPalm-0.0.1.tar` & `MedPalm-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:14:47.024075 MedPalm-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 04:14:37.000000 MedPalm-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:14:47.024075 MedPalm-0.0.1/MedPalm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 04:14:47.000000 MedPalm-0.0.1/MedPalm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 04:14:47.000000 MedPalm-0.0.1/MedPalm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:14:47.000000 MedPalm-0.0.1/MedPalm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 04:14:47.000000 MedPalm-0.0.1/MedPalm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 04:14:47.000000 MedPalm-0.0.1/MedPalm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 04:14:47.024075 MedPalm-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-31 04:14:37.000000 MedPalm-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:14:47.024075 MedPalm-0.0.1/med_palm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/ppo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/reward_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-31 04:14:37.000000 MedPalm-0.0.1/med_palm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 04:14:47.024075 MedPalm-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 04:14:37.000000 MedPalm-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:24:24.067710 MedPalm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 04:24:12.000000 MedPalm-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:24:24.063710 MedPalm-0.0.2/MedPalm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 04:24:24.067710 MedPalm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-31 04:24:12.000000 MedPalm-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:24:24.067710 MedPalm-0.0.2/med_palm/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/reward_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 04:24:24.067710 MedPalm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 04:24:12.000000 MedPalm-0.0.2/setup.py
```

### Comparing `MedPalm-0.0.1/LICENSE` & `MedPalm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/MedPalm.egg-info/PKG-INFO` & `MedPalm-0.0.2/MedPalm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedPalm
-Version: 0.0.1
+Version: 0.0.2
 Summary: MedPalm - Pytorch
 Home-page: https://github.com/kyegomez/med-palm
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MedPalm-0.0.1/PKG-INFO` & `MedPalm-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedPalm
-Version: 0.0.1
+Version: 0.0.2
 Summary: MedPalm - Pytorch
 Home-page: https://github.com/kyegomez/med-palm
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MedPalm-0.0.1/med_palm/attention.py` & `MedPalm-0.0.2/med_palm/attention.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/lora.py` & `MedPalm-0.0.2/med_palm/lora.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/model.py` & `MedPalm-0.0.2/med_palm/model.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/optimizer.py` & `MedPalm-0.0.2/med_palm/optimizer.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/palm.py` & `MedPalm-0.0.2/med_palm/palm.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/ppo.py` & `MedPalm-0.0.2/med_palm/ppo.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/reward_model.py` & `MedPalm-0.0.2/med_palm/reward_model.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/med_palm/utils.py` & `MedPalm-0.0.2/med_palm/utils.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.1/setup.py` & `MedPalm-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MedPalm',
   packages = find_packages(exclude=['examples']),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'MedPalm - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/med-palm',
   long_description_content_type = 'text/markdown',
   keywords = [
```

