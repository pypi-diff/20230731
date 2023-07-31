# Comparing `tmp/pyPhasesML-0.7.5.tar.gz` & `tmp/pyPhasesML-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.7.5.tar", last modified: Mon Jul 31 13:34:00 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.6.tar", last modified: Mon Jul 31 13:39:26 2023, max compression
```

## Comparing `pyPhasesML-0.7.5.tar` & `pyPhasesML-0.7.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.166104 pyPhasesML-0.7.5/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 13:34:00.166104 pyPhasesML-0.7.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.161104 pyPhasesML-0.7.5/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4074 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.163104 pyPhasesML-0.7.5/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     9986 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.164104 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2420 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.165104 pyPhasesML-0.7.5/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.165104 pyPhasesML-0.7.5/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.166104 pyPhasesML-0.7.5/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:34:00.162104 pyPhasesML-0.7.5/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 13:34:00.000000 pyPhasesML-0.7.5/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 13:34:00.000000 pyPhasesML-0.7.5/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:34:00.000000 pyPhasesML-0.7.5/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 13:34:00.000000 pyPhasesML-0.7.5/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 13:34:00.000000 pyPhasesML-0.7.5/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-31 13:33:42.000000 pyPhasesML-0.7.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 13:34:00.166104 pyPhasesML-0.7.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 13:33:43.000000 pyPhasesML-0.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.269157 pyPhasesML-0.7.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 13:39:26.269157 pyPhasesML-0.7.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.264157 pyPhasesML-0.7.6/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4074 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.265157 pyPhasesML-0.7.6/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9986 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.267157 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.267157 pyPhasesML-0.7.6/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.268157 pyPhasesML-0.7.6/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.269157 pyPhasesML-0.7.6/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:39:26.265157 pyPhasesML-0.7.6/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 13:39:26.000000 pyPhasesML-0.7.6/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 13:39:26.000000 pyPhasesML-0.7.6/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:39:26.000000 pyPhasesML-0.7.6/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 13:39:26.000000 pyPhasesML-0.7.6/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 13:39:26.000000 pyPhasesML-0.7.6/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-31 13:39:07.000000 pyPhasesML-0.7.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 13:39:26.269157 pyPhasesML-0.7.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 13:39:09.000000 pyPhasesML-0.7.6/setup.py
```

### Comparing `pyPhasesML-0.7.5/LICENSE` & `pyPhasesML-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/PKG-INFO` & `pyPhasesML-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.5/README.md` & `pyPhasesML-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.6/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.6/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.6/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.6/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/Model.py` & `pyPhasesML-0.7.6/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.6/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.6/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.6/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/Callback.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/Callback.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/CyclicLearningrate.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/CyclicLearningrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # setup optimizer and scheduler
         model.optimizer = optim.Adam(model.model.parameters(), lr=1.0)
         step_size = self.stepSizeInEpochs * len(dataset.trainingData)
         clr = cyclical_lr(step_size, min_lr=self.learningRateMin, max_lr=self.learningRateMax)
         model.batchScheduler = optim.lr_scheduler.LambdaLR(model.optimizer, [clr])
 
     def getResumeBatchOptimizerPath(self):
-        return Path(self.getLogPath(), ".resumeBatchScheduler")
+        return Path(self.getLogPath(), ".resumeBatchScheduler.pt")
     
     def onShutdown(self, model):
         import torch
         torch.save(model.batchScheduler.state_dict(), str(self.getResumeBatchOptimizerPath()))
                 
     def onRestore(self, model):
         import torch
```

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/adapter/torch/SystemCheckPoint.py` & `pyPhasesML-0.7.6/pyPhasesML/adapter/torch/SystemCheckPoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
         self.priority = 1000
 
     def shutdown(self, signum, frame):
         self.shutdownRequest = True
         self.logError("Shutdown requested received, waiting for the next checkpoint")
 
     def getResumeModelPath(self):
-        return Path(self.getLogPath(), ".resumeModel")
+        return Path(self.getLogPath(), ".resumeModel.pt")
 
     def getResumeOptimizerPath(self):
-        return Path(self.getLogPath(), ".resumeOptimizer")
+        return Path(self.getLogPath(), ".resumeOptimizer.pt")
 
     def getResumeAdapterPath(self):
-        return Path(self.getLogPath(), ".resumeAdapter")
+        return Path(self.getLogPath(), ".resumeAdapter.pcl")
 
     def onTrainingStart(self, model, dataset):
         if self.getResumeModelPath().exists():
             self.logSuccess("Restore training")
             modelState = torch.load(str(self.getResumeModelPath()))
             model.loadState(modelState)
             optimizerState = torch.load(str(self.getResumeOptimizerPath()))
```

### Comparing `pyPhasesML-0.7.5/pyPhasesML/config.yaml` & `pyPhasesML-0.7.6/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.6/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.6/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.6/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.6/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.6/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.6/pyPhasesML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.5/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.7.6/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.5/setup.py` & `pyPhasesML-0.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.7.5"[1:],
+    version="v0.7.6"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

