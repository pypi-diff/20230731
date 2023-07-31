# Comparing `tmp/pygdebias-1.0.0.tar.gz` & `tmp/pygdebias-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdebias-1.0.0.tar", last modified: Sun Jul 30 20:43:05 2023, max compression
+gzip compressed data, was "pygdebias-1.0.1.tar", last modified: Mon Jul 31 00:45:30 2023, max compression
```

## Comparing `pygdebias-1.0.0.tar` & `pygdebias-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-30 20:43:05.100631 pygdebias-1.0.0/
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     1062 2023-07-27 04:15:21.000000 pygdebias-1.0.0/LICENSE
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)       33 2023-07-27 04:15:21.000000 pygdebias-1.0.0/MANIFEST.in
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    31076 2023-07-30 20:43:05.100631 pygdebias-1.0.0/PKG-INFO
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    30645 2023-07-28 09:32:02.000000 pygdebias-1.0.0/README.md
-drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-30 20:43:05.096631 pygdebias-1.0.0/pygdebias/
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)       71 2023-07-27 05:00:53.000000 pygdebias-1.0.0/pygdebias/__init__.py
-drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-30 20:43:05.096631 pygdebias-1.0.0/pygdebias/datasets/
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      427 2023-07-27 05:00:55.000000 pygdebias-1.0.0/pygdebias/datasets/__init__.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)   104373 2023-07-28 09:31:10.000000 pygdebias-1.0.0/pygdebias/datasets/datasets.py
-drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-30 20:43:05.100631 pygdebias-1.0.0/pygdebias/debiasing/
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    28717 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/CrossWalk.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    32907 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/EDITS.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    41621 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/FairEdit.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    11009 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/FairGNN.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    48942 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/FairVGNN.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    28959 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/FairWalk.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    63392 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/GEAR.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    14053 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/GNN.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    29205 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/GUIDE.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    21616 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/InFoRM_GNN.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    22468 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/NIFTY.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    27778 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/REDRESS.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    31254 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/RawlsGCN.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    29465 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/UGE.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      706 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/debiasing/__init__.py
-drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-30 20:43:05.100631 pygdebias-1.0.0/pygdebias/metrics/
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     1557 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/metrics/__init__.py
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    13802 2023-07-27 04:15:20.000000 pygdebias-1.0.0/pygdebias/metrics/metrics.py
-drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-30 20:43:05.096631 pygdebias-1.0.0/pygdebias.egg-info/
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    31076 2023-07-30 20:43:05.000000 pygdebias-1.0.0/pygdebias.egg-info/PKG-INFO
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      813 2023-07-30 20:43:05.000000 pygdebias-1.0.0/pygdebias.egg-info/SOURCES.txt
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)        1 2023-07-30 20:43:05.000000 pygdebias-1.0.0/pygdebias.egg-info/dependency_links.txt
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     2895 2023-07-30 20:43:05.000000 pygdebias-1.0.0/pygdebias.egg-info/requires.txt
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)       10 2023-07-30 20:43:05.000000 pygdebias-1.0.0/pygdebias.egg-info/top_level.txt
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      361 2023-07-30 20:43:05.100631 pygdebias-1.0.0/setup.cfg
--rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      418 2023-07-30 20:40:34.000000 pygdebias-1.0.0/setup.py
+drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-31 00:45:30.946748 pygdebias-1.0.1/
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     1062 2023-07-27 04:15:21.000000 pygdebias-1.0.1/LICENSE
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)       58 2023-07-31 00:44:24.000000 pygdebias-1.0.1/MANIFEST.in
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    31076 2023-07-31 00:45:30.946748 pygdebias-1.0.1/PKG-INFO
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    30645 2023-07-28 09:32:02.000000 pygdebias-1.0.1/README.md
+drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-31 00:45:30.942748 pygdebias-1.0.1/pygdebias/
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)       71 2023-07-27 05:00:53.000000 pygdebias-1.0.1/pygdebias/__init__.py
+drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-31 00:45:30.942748 pygdebias-1.0.1/pygdebias/datasets/
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      427 2023-07-27 05:00:55.000000 pygdebias-1.0.1/pygdebias/datasets/__init__.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)   104373 2023-07-28 09:31:10.000000 pygdebias-1.0.1/pygdebias/datasets/datasets.py
+drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-31 00:45:30.946748 pygdebias-1.0.1/pygdebias/debiasing/
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    28717 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/CrossWalk.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    32907 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/EDITS.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    41621 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/FairEdit.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    11009 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/FairGNN.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    48942 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/FairVGNN.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    28959 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/FairWalk.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    63392 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/GEAR.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    14053 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/GNN.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    29205 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/GUIDE.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    21616 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/InFoRM_GNN.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    22468 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/NIFTY.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    27778 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/REDRESS.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    31254 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/RawlsGCN.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    29465 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/UGE.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      706 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/debiasing/__init__.py
+drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-31 00:45:30.946748 pygdebias-1.0.1/pygdebias/metrics/
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     1557 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/metrics/__init__.py
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    13802 2023-07-27 04:15:20.000000 pygdebias-1.0.1/pygdebias/metrics/metrics.py
+drwxrwxr-x   0 sjc4fq    (1017) sjc4fq    (1017)        0 2023-07-31 00:45:30.942748 pygdebias-1.0.1/pygdebias.egg-info/
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)    31076 2023-07-31 00:45:30.000000 pygdebias-1.0.1/pygdebias.egg-info/PKG-INFO
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      830 2023-07-31 00:45:30.000000 pygdebias-1.0.1/pygdebias.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)        1 2023-07-31 00:45:30.000000 pygdebias-1.0.1/pygdebias.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     2895 2023-07-31 00:45:30.000000 pygdebias-1.0.1/pygdebias.egg-info/requires.txt
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)       10 2023-07-31 00:45:30.000000 pygdebias-1.0.1/pygdebias.egg-info/top_level.txt
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)     2911 2023-07-27 04:15:21.000000 pygdebias-1.0.1/requirements.txt
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      361 2023-07-31 00:45:30.946748 pygdebias-1.0.1/setup.cfg
+-rw-rw-r--   0 sjc4fq    (1017) sjc4fq    (1017)      418 2023-07-30 20:40:34.000000 pygdebias-1.0.1/setup.py
```

### Comparing `pygdebias-1.0.0/LICENSE` & `pygdebias-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/PKG-INFO` & `pygdebias-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdebias
-Version: 1.0.0
+Version: 1.0.1
 Summary: Attributed Network Datasets and Fairness-Aware Graph Mining Algorithms
 Author: Yushun Dong, Song Wang, Zaiyi Zheng, Zhenyu Lei, Jing Ma, Chen Chen, Jundong Li
 Author-email: yd6eb@virginia.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `pygdebias-1.0.0/README.md` & `pygdebias-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/datasets/datasets.py` & `pygdebias-1.0.1/pygdebias/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/CrossWalk.py` & `pygdebias-1.0.1/pygdebias/debiasing/CrossWalk.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/EDITS.py` & `pygdebias-1.0.1/pygdebias/debiasing/EDITS.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/FairEdit.py` & `pygdebias-1.0.1/pygdebias/debiasing/FairEdit.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/FairGNN.py` & `pygdebias-1.0.1/pygdebias/debiasing/FairGNN.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/FairVGNN.py` & `pygdebias-1.0.1/pygdebias/debiasing/FairVGNN.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/FairWalk.py` & `pygdebias-1.0.1/pygdebias/debiasing/FairWalk.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/GEAR.py` & `pygdebias-1.0.1/pygdebias/debiasing/GEAR.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/GNN.py` & `pygdebias-1.0.1/pygdebias/debiasing/GNN.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/GUIDE.py` & `pygdebias-1.0.1/pygdebias/debiasing/GUIDE.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/InFoRM_GNN.py` & `pygdebias-1.0.1/pygdebias/debiasing/InFoRM_GNN.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/NIFTY.py` & `pygdebias-1.0.1/pygdebias/debiasing/NIFTY.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/REDRESS.py` & `pygdebias-1.0.1/pygdebias/debiasing/REDRESS.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/RawlsGCN.py` & `pygdebias-1.0.1/pygdebias/debiasing/RawlsGCN.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/UGE.py` & `pygdebias-1.0.1/pygdebias/debiasing/UGE.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/debiasing/__init__.py` & `pygdebias-1.0.1/pygdebias/debiasing/__init__.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/metrics/__init__.py` & `pygdebias-1.0.1/pygdebias/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias/metrics/metrics.py` & `pygdebias-1.0.1/pygdebias/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `pygdebias-1.0.0/pygdebias.egg-info/PKG-INFO` & `pygdebias-1.0.1/pygdebias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdebias
-Version: 1.0.0
+Version: 1.0.1
 Summary: Attributed Network Datasets and Fairness-Aware Graph Mining Algorithms
 Author: Yushun Dong, Song Wang, Zaiyi Zheng, Zhenyu Lei, Jing Ma, Chen Chen, Jundong Li
 Author-email: yd6eb@virginia.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `pygdebias-1.0.0/pygdebias.egg-info/SOURCES.txt` & `pygdebias-1.0.1/pygdebias.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 pygdebias/__init__.py
 pygdebias.egg-info/PKG-INFO
 pygdebias.egg-info/SOURCES.txt
 pygdebias.egg-info/dependency_links.txt
 pygdebias.egg-info/requires.txt
```

### Comparing `pygdebias-1.0.0/pygdebias.egg-info/requires.txt` & `pygdebias-1.0.1/pygdebias.egg-info/requires.txt`

 * *Files identical despite different names*

