# Comparing `tmp/peitho_data-2.3.8.tar.gz` & `tmp/peitho_data-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.3.8.tar", last modified: Mon Jun 26 12:28:24 2023, max compression
+gzip compressed data, was "peitho_data-2.3.9.tar", last modified: Wed Jul 26 05:05:22 2023, max compression
```

## Comparing `peitho_data-2.3.8.tar` & `peitho_data-2.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 12:26:04.000000 peitho_data-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 12:26:04.000000 peitho_data-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 12:28:24.206587 peitho_data-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-26 12:26:04.000000 peitho_data-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/graph/knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data/machine_learning/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/cnn/image_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/graph/test_knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.206587 peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/test_image_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-26 12:26:04.000000 peitho_data-2.3.8/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:28:24.202587 peitho_data-2.3.8/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:26:36.000000 peitho_data-2.3.8/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 12:28:24.000000 peitho_data-2.3.8/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 12:28:24.206587 peitho_data-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 12:26:04.000000 peitho_data-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.783898 peitho_data-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 05:03:24.000000 peitho_data-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 05:03:24.000000 peitho_data-2.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-26 05:05:22.783898 peitho_data-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-26 05:03:24.000000 peitho_data-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.779898 peitho_data-2.3.9/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.779898 peitho_data-2.3.9/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.779898 peitho_data-2.3.9/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.779898 peitho_data-2.3.9/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.779898 peitho_data-2.3.9/peitho_data/machine_learning/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/machine_learning/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/machine_learning/cnn/image_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.783898 peitho_data-2.3.9/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.783898 peitho_data-2.3.9/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.783898 peitho_data-2.3.9/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.783898 peitho_data-2.3.9/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.783898 peitho_data-2.3.9/peitho_data/tests/machine_learning/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/machine_learning/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/machine_learning/cnn/test_image_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-26 05:03:24.000000 peitho_data-2.3.9/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:05:22.779898 peitho_data-2.3.9/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-26 05:05:22.000000 peitho_data-2.3.9/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-26 05:05:22.000000 peitho_data-2.3.9/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:05:22.000000 peitho_data-2.3.9/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:03:48.000000 peitho_data-2.3.9/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 05:05:22.000000 peitho_data-2.3.9/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 05:05:22.000000 peitho_data-2.3.9/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 05:05:22.783898 peitho_data-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-26 05:03:24.000000 peitho_data-2.3.9/setup.py
```

### Comparing `peitho_data-2.3.8/LICENSE` & `peitho_data-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/README.md` & `peitho_data-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.3.9/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/datafication/epub.py` & `peitho_data-2.3.9/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/graph/knowledge_graph_spec.py` & `peitho_data-2.3.9/peitho_data/graph/knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/machine_learning/cnn/image_convolution.py` & `peitho_data-2.3.9/peitho_data/machine_learning/cnn/image_convolution.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.3.9/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/tests/datafication/test_epub.py` & `peitho_data-2.3.9/peitho_data/tests/datafication/test_epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/tests/graph/test_knowledge_graph_spec.py` & `peitho_data-2.3.9/peitho_data/tests/graph/test_knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/tests/machine_learning/cnn/test_image_convolution.py` & `peitho_data-2.3.9/peitho_data/tests/machine_learning/cnn/test_image_convolution.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.3.9/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/tests/test_trello_api.py` & `peitho_data-2.3.9/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.3.9/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/trello_api.py` & `peitho_data-2.3.9/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data/word_cloud.py` & `peitho_data-2.3.9/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.3.9/peitho_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.8/setup.py` & `peitho_data-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.3.8",
+    version="2.3.9",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

