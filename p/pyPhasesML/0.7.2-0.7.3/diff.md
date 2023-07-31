# Comparing `tmp/pyPhasesML-0.7.2.tar.gz` & `tmp/pyPhasesML-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.7.2.tar", last modified: Sun Jul 30 15:27:52 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.3.tar", last modified: Mon Jul 31 09:59:36 2023, max compression
```

## Comparing `pyPhasesML-0.7.2.tar` & `pyPhasesML-0.7.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.160562 pyPhasesML-0.7.2/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-30 15:27:52.160562 pyPhasesML-0.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.155562 pyPhasesML-0.7.2/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4077 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.156562 pyPhasesML-0.7.2/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.158562 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3654 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2613 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.158562 pyPhasesML-0.7.2/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.159562 pyPhasesML-0.7.2/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.159562 pyPhasesML-0.7.2/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 15:27:52.156562 pyPhasesML-0.7.2/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-30 15:27:52.000000 pyPhasesML-0.7.2/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-30 15:27:52.000000 pyPhasesML-0.7.2/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 15:27:52.000000 pyPhasesML-0.7.2/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-30 15:27:52.000000 pyPhasesML-0.7.2/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-30 15:27:52.000000 pyPhasesML-0.7.2/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-30 15:27:34.000000 pyPhasesML-0.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 15:27:52.160562 pyPhasesML-0.7.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-30 15:27:36.000000 pyPhasesML-0.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.246838 pyPhasesML-0.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 09:59:36.246838 pyPhasesML-0.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.240838 pyPhasesML-0.7.3/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4074 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.242838 pyPhasesML-0.7.3/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.243838 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2613 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.244838 pyPhasesML-0.7.3/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.245838 pyPhasesML-0.7.3/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.245838 pyPhasesML-0.7.3/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.241838 pyPhasesML-0.7.3/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 09:59:36.246838 pyPhasesML-0.7.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 09:59:19.000000 pyPhasesML-0.7.3/setup.py
```

### Comparing `pyPhasesML-0.7.2/LICENSE` & `pyPhasesML-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/PKG-INFO` & `pyPhasesML-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.2/README.md` & `pyPhasesML-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.3/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.3/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.3/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.3/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/Model.py` & `pyPhasesML-0.7.3/pyPhasesML/Model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     pass
 
 class ModelConfig:
     def __init__(self):
         self.optimizerId = "adams"
         self.learningRate = 0.001
         self.learningRateDecay = None
-        self.stopAfterNotImproving = None
+        self.stopAfterNotImproving = 0
         
         # cyclic lr
         self.cycleLRDivisor = 4  # minLR = lr / cycleLRFactor
         
         # logging
         self.logPath = "logs"
         self.csvLogFile = "log.csv"
```

### Comparing `pyPhasesML-0.7.2/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.3/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.3/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.3/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/Callback.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/Callback.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import os
 import timeit
-import psutil
 
-import torch
 from pyPhases import classLogger
+
 from pyPhasesML.adapter.torch.Callback import Callback
+from pyPhasesML.Model import ModelConfig
 
 
 @classLogger
 class CheckPoint(Callback):
+    def __init__(self, config: ModelConfig) -> None:
+        super().__init__(config)
+        self.metricDefinitions = None
+        self.notImprovedSince = 0
 
     def onTrainingStart(self, model, dataset):
         self.epochStartTime = timeit.default_timer()
 
     def onValidationStart(self, model, dataset):
         self.epochEndTime = timeit.default_timer()
-        
+
     def prettyPrintConfusionMatrix(self, confusion_matrix):
         num_rows, num_cols = confusion_matrix.shape
         max_value_length = max(len(str(confusion_matrix.max())), len(str(confusion_matrix.min())))
         separator = "-" * ((max_value_length + 2) * num_cols)
 
         rows = []
         for i in range(num_rows):
@@ -33,34 +36,31 @@
     def onValidationEnd(self, model, results, scorer):
         metricsValues = {m: results[m] for m in scorer.metrics}
         metricDiffStrings = []
         metricValuetrings = []
         improved = False
         modelId = "checkpointModel_%i_" % model.epoch
 
-        metrics = model.validationMetrics
-        metricDefinitions = {m: scorer.getMetricDefinition(m) for m in metrics}
+        if self.metricDefinitions is None:
+            self.metricDefinitions = {m: scorer.getMetricDefinition(m) for m in model.validationMetrics}
+
         globalBestMetric = model.validationMetrics[0]
 
         metricStrings = []
         for metricName, metricVal in metricsValues.items():
-            bestValue, useAsBest, biggerIsBetter = metricDefinitions[metricName]
+            bestValue, useAsBest, biggerIsBetter = self.metricDefinitions[metricName]
             diff = metricVal - bestValue
-            metricStrings.append(
-                f"{metricName}: "
-                + "{:.3f}".format(metricVal)
-                + " [best: {:.3f}]".format(bestValue)
-            )
+            metricStrings.append(f"{metricName}: " + "{:.3f}".format(metricVal) + " [best: {:.3f}]".format(bestValue))
             metricDiffStrings.append(f"{metricName}: " + "{:.3f}".format(diff))
             metricValuetrings.append("{:.3f}".format(metricVal))
 
             isBigger = metricVal > bestValue
 
             if (biggerIsBetter and isBigger) or (not biggerIsBetter and not isBigger):
-                metricDefinitions[metricName][0] = metricVal
+                self.metricDefinitions[metricName][0] = metricVal
                 if useAsBest:
                     improved = True
                     if metricName == globalBestMetric:
                         model.bestMetric = max(model.bestMetric, metricsValues[globalBestMetric])
 
         validationEndTime = timeit.default_timer()
 
@@ -75,19 +75,18 @@
         self.log(f"Training Stats: {trainingStats} ")
         self.log(" ".join(metricStrings))
 
         if improved:
             self.log("Model Improved: " + " ".join(metricDiffStrings))
             path = f"{self.getLogPath()}/{modelId}" + "_".join(metricValuetrings) + ".pkl"
             with open(path, "wb") as f:
+                import torch
                 torch.save(model.model.state_dict(), f)
-            notImprovedSince = 0
+            self.notImprovedSince = 0
             self.bestModelPath = path
         else:
-            notImprovedSince += 1
-            self.log("Model not improving since %i epochs" % (notImprovedSince))
+            self.notImprovedSince += 1
+            self.log("Model not improving since %i epochs" % (self.notImprovedSince))
 
-        if self.config.stopAfterNotImproving > 0 and notImprovedSince >= self.config.stopAfterNotImproving:
+        if self.config.stopAfterNotImproving > 0 and self.notImprovedSince >= self.config.stopAfterNotImproving:
             model.fnished = True
 
-        process = psutil.Process(os.getpid())
-        self.log(f"memory usage: {process.memory_info().rss / 1024 / 1024}M")
```

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/CyclicLearningrate.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CyclicLearningrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import math
-import torch.optim as optim
 from pyPhases import classLogger
 from pyPhasesML.Model import ModelConfig
 from pyPhasesML.adapter.torch.Callback import Callback
 
 
 @classLogger
 class CyclicLearningrate(Callback):
     def __init__(self, config: ModelConfig) -> None:
         self.learningRateMax = config.learningRate
         self.learningRateMin = config.learningRate / config.cycleLRDivisor
         self.stepSizeInEpochs = 4
 
     def onTrainingStart(self, model, dataset):
+        import torch.optim as optim
         def cyclical_lr(stepsize, min_lr=3e-4, max_lr=3e-3):
             # Scaler: we can adapt this if we do not want the triangular CLR
             scaler = lambda x: 1.0
 
             # calculate the LR
             def getLR(it):
                 return min_lr + (max_lr - min_lr) * relative(it, stepsize)
```

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 import numpy as np
 
-import torch
 from pyPhases import classLogger
 from pyPhasesML.Model import ModelConfig
 from pyPhasesML.adapter.torch.Callback import Callback
 
 
 @classLogger
 class FindLearningRate(Callback):
@@ -14,14 +13,15 @@
         self.smoothing = 0.05
         self.findLearningRatePlotPath = self.getLogPath() + "/lrRangeTest.png"
         self.minLR = minLR
         self.maxLR = maxLR
         self.iterations = iterations
 
     def onTrainingStart(self, model, dataset):
+        import torch
         model.maxEpochs = self.iterations
         start_lr = self.minLR
         end_lr = self.maxLR
 
         def cyclical_lr(x):
             return math.exp(x * math.log(end_lr / start_lr) / (model.maxEpochs * len(dataset.trainingData)))
```

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/adapter/torch/SystemCheckPoint.py` & `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/SystemCheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/config.yaml` & `pyPhasesML-0.7.3/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.3/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.3/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.3/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.3/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.3/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.3/pyPhasesML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.2/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.7.3/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.2/setup.py` & `pyPhasesML-0.7.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.7.2"[1:],
+    version="v0.7.3"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

