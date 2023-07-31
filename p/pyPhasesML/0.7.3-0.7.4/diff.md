# Comparing `tmp/pyPhasesML-0.7.3.tar.gz` & `tmp/pyPhasesML-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.7.3.tar", last modified: Mon Jul 31 09:59:36 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.4.tar", last modified: Mon Jul 31 12:35:10 2023, max compression
```

## Comparing `pyPhasesML-0.7.3.tar` & `pyPhasesML-0.7.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.246838 pyPhasesML-0.7.3/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 09:59:36.246838 pyPhasesML-0.7.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.240838 pyPhasesML-0.7.3/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4074 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.242838 pyPhasesML-0.7.3/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.243838 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2613 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.244838 pyPhasesML-0.7.3/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.245838 pyPhasesML-0.7.3/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.245838 pyPhasesML-0.7.3/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:59:36.241838 pyPhasesML-0.7.3/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 09:59:36.000000 pyPhasesML-0.7.3/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-31 09:59:18.000000 pyPhasesML-0.7.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 09:59:36.246838 pyPhasesML-0.7.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 09:59:19.000000 pyPhasesML-0.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.496791 pyPhasesML-0.7.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 12:35:10.496791 pyPhasesML-0.7.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.490791 pyPhasesML-0.7.4/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4074 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.492791 pyPhasesML-0.7.4/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9986 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.493791 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.494791 pyPhasesML-0.7.4/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.495791 pyPhasesML-0.7.4/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.496791 pyPhasesML-0.7.4/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:35:10.491791 pyPhasesML-0.7.4/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 12:35:10.000000 pyPhasesML-0.7.4/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 12:35:10.000000 pyPhasesML-0.7.4/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 12:35:10.000000 pyPhasesML-0.7.4/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 12:35:10.000000 pyPhasesML-0.7.4/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 12:35:10.000000 pyPhasesML-0.7.4/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-31 12:34:51.000000 pyPhasesML-0.7.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 12:35:10.496791 pyPhasesML-0.7.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 12:34:53.000000 pyPhasesML-0.7.4/setup.py
```

### Comparing `pyPhasesML-0.7.3/LICENSE` & `pyPhasesML-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/PKG-INFO` & `pyPhasesML-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.3/README.md` & `pyPhasesML-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.4/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.4/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.4/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.4/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/Model.py` & `pyPhasesML-0.7.4/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.4/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.4/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.4/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,16 @@
             dataset.x = dataset.x.cuda()
             dataset.y = dataset.y.cuda()
 
         return self.prepareData(dataset, validation)
 
     def registerCB(self, cb):
         self.cbs.append(cb)
+        self.cbs.sort(key=lambda x: x.priority)
+        cb.trigger("register", self)
 
     def initAdapter(self, findingLearningRate=False):
         config = self.config
 
         self.registerCB(LoadOptimizer(config))
         self.registerCB(CSVLogger(config))
         self.registerCB(SystemCheckPoint(config))
```

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.7.4/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class OptimizerNotFound(Exception):
     pass
 
 
 @classLogger
 class LoadOptimizer(Callback):
     def __init__(self, modelConfig: ModelConfig) -> None:
+        super().__init__(modelConfig)
         self.optimizerId = modelConfig.optimizerId
         self.lr = modelConfig.learningRate
         self.lr_decay = modelConfig.learningRateDecay
 
     def onTrainingStart(self, model, dataset):
         if self.optimizerId == "adams":
             model.optimizer = optim.Adam(model.model.parameters(), lr=self.lr, weight_decay=self.lr_decay)
```

### Comparing `pyPhasesML-0.7.3/pyPhasesML/config.yaml` & `pyPhasesML-0.7.4/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.4/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.4/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.4/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.4/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.4/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.4/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.3/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.7.4/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.3/setup.py` & `pyPhasesML-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.7.3"[1:],
+    version="v0.7.4"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

