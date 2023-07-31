# Comparing `tmp/arfs-2.0.1.tar.gz` & `tmp/arfs-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-2.0.1.tar", last modified: Fri Jul 28 14:34:02 2023, max compression
+gzip compressed data, was "arfs-2.0.2.tar", last modified: Mon Jul 31 10:42:15 2023, max compression
```

## Comparing `arfs-2.0.1.tar` & `arfs-2.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:02.274474 arfs-2.0.1/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    11965 2023-07-28 14:34:02.275476 arfs-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11275 2023-07-28 10:30:07.000000 arfs-2.0.1/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1377 2023-07-28 14:34:02.285475 arfs-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.724457 arfs-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.879464 arfs-2.0.1/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-07-28 13:13:55.000000 arfs-2.0.1/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    86758 2023-07-28 13:17:02.000000 arfs-2.0.1/src/arfs/association.py
--rw-rw-rw-   0        0        0     6689 2023-07-24 20:31:43.000000 arfs-2.0.1/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.726458 arfs-2.0.1/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.994466 arfs-2.0.1/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.1/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.1/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:02.224473 arfs-2.0.1/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.1/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    95567 2023-07-28 14:32:16.000000 arfs-2.0.1/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-2.0.1/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    19893 2023-07-26 16:20:34.000000 arfs-2.0.1/src/arfs/feature_selection/lasso.py
--rw-rw-rw-   0        0        0    13397 2023-07-27 13:39:47.000000 arfs-2.0.1/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-2.0.1/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15832 2023-07-26 16:49:41.000000 arfs-2.0.1/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    15689 2023-07-24 19:47:35.000000 arfs-2.0.1/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-2.0.1/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-2.0.1/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    40462 2023-07-27 07:24:21.000000 arfs-2.0.1/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-2.0.1/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    25248 2023-07-26 08:46:59.000000 arfs-2.0.1/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:01.962468 arfs-2.0.1/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11965 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.1/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      355 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 14:34:01.000000 arfs-2.0.1/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-28 14:34:02.257474 arfs-2.0.1/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.1/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.1/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.193393 arfs-2.0.2/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    11967 2023-07-31 10:42:15.194393 arfs-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11277 2023-07-29 14:45:54.000000 arfs-2.0.2/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1611 2023-07-31 10:42:15.203395 arfs-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.709393 arfs-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.894397 arfs-2.0.2/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-07-31 10:33:14.000000 arfs-2.0.2/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    87074 2023-07-29 17:00:56.000000 arfs-2.0.2/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6689 2023-07-24 20:31:43.000000 arfs-2.0.2/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.712393 arfs-2.0.2/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.001395 arfs-2.0.2/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.2/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.2/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.148393 arfs-2.0.2/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.2/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    96187 2023-07-29 17:00:56.000000 arfs-2.0.2/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-2.0.2/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    21314 2023-07-31 10:40:40.000000 arfs-2.0.2/src/arfs/feature_selection/lasso.py
+-rw-rw-rw-   0        0        0    13385 2023-07-29 17:00:51.000000 arfs-2.0.2/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-2.0.2/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15864 2023-07-29 17:00:51.000000 arfs-2.0.2/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    15806 2023-07-29 17:00:51.000000 arfs-2.0.2/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-2.0.2/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-2.0.2/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    40517 2023-07-29 17:00:53.000000 arfs-2.0.2/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-2.0.2/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    25367 2023-07-29 17:00:53.000000 arfs-2.0.2/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.978395 arfs-2.0.2/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11967 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.2/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      573 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.179392 arfs-2.0.2/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.2/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.2/tests/test_featselect.py
```

### Comparing `arfs-2.0.1/LICENSE.md` & `arfs-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/PKG-INFO` & `arfs-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.1
+Version: 2.0.2
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
@@ -28,15 +28,15 @@
 
 # All relevant feature selection
 
 All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
 
 This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
 
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for intrucing non-linearities into linear models and perform feature selection.
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
 
 Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
 `$ pip install arfs`, requires python <3.10
```

### Comparing `arfs-2.0.1/README.md` & `arfs-2.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # All relevant feature selection
 
 All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
 
 This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
 
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for intrucing non-linearities into linear models and perform feature selection.
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
 
 Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
 `$ pip install arfs`, requires python <3.10
```

### Comparing `arfs-2.0.1/setup.cfg` & `arfs-2.0.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -63,25 +63,39 @@
 000003e0: 7461 5d0d 0a61 7266 732e 6461 7461 7365  ta]..arfs.datase
 000003f0: 742e 6461 7461 203d 200d 0a09 2a2e 6a6f  t.data = ...*.jo
 00000400: 626c 6962 0d0a 092a 2e7a 6970 0d0a 6172  blib...*.zip..ar
 00000410: 6673 2e64 6174 6173 6574 2e64 6573 6372  fs.dataset.descr
 00000420: 6970 7469 6f6e 203d 200d 0a09 2a2e 7273  iption = ...*.rs
 00000430: 740d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  t....[options.ex
 00000440: 7472 6173 5f72 6571 7569 7265 5d0d 0a64  tras_require]..d
-00000450: 6f63 7320 3d20 0d0a 096e 6273 7068 696e  ocs = ...nbsphin
-00000460: 783e 3d30 2e38 2e38 0d0a 0969 7079 6b65  x>=0.8.8...ipyke
-00000470: 726e 656c 3e3d 362e 392e 310d 0a09 6970  rnel>=6.9.1...ip
-00000480: 7974 686f 6e5f 6765 6e75 7469 6c73 0d0a  ython_genutils..
-00000490: 0970 616e 646f 630d 0a09 7370 6869 6e78  .pandoc...sphinx
-000004a0: 3e3d 342e 342e 300d 0a09 7370 6869 6e78  >=4.4.0...sphinx
-000004b0: 2d61 7574 6f64 6f63 2d74 7970 6568 696e  -autodoc-typehin
-000004c0: 7473 3e3d 312e 3136 2e30 0d0a 0973 7068  ts>=1.16.0...sph
-000004d0: 696e 782d 636f 7079 6275 7474 6f6e 3e3d  inx-copybutton>=
-000004e0: 302e 352e 300d 0a09 7370 6869 6e78 2d72  0.5.0...sphinx-r
-000004f0: 7464 2d74 6865 6d65 3e3d 312e 302e 300d  td-theme>=1.0.0.
-00000500: 0a09 7370 6869 6e78 2d74 6162 733e 3d33  ..sphinx-tabs>=3
-00000510: 2e32 2e30 0d0a 7465 7374 203d 200d 0a09  .2.0..test = ...
-00000520: 7079 7465 7374 0d0a 0970 7974 6573 742d  pytest...pytest-
-00000530: 636f 760d 0a0d 0a5b 6567 675f 696e 666f  cov....[egg_info
-00000540: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000550: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000560: 0a                                       .
+00000450: 6f63 7320 3d20 0d0a 0969 7079 6b65 726e  ocs = ...ipykern
+00000460: 656c 0d0a 0969 7079 7468 6f6e 5f67 656e  el...ipython_gen
+00000470: 7574 696c 730d 0a09 7061 6e64 6f63 0d0a  utils...pandoc..
+00000480: 0973 7068 696e 783d 3d37 2e31 2e31 0d0a  .sphinx==7.1.1..
+00000490: 096e 6273 7068 696e 783d 3d30 2e39 2e32  .nbsphinx==0.9.2
+000004a0: 0d0a 0973 7068 696e 782d 6175 746f 646f  ...sphinx-autodo
+000004b0: 632d 7479 7065 6869 6e74 733d 3d31 2e32  c-typehints==1.2
+000004c0: 342e 300d 0a09 7370 6869 6e78 2d63 6f70  4.0...sphinx-cop
+000004d0: 7962 7574 746f 6e3d 3d30 2e35 2e32 0d0a  ybutton==0.5.2..
+000004e0: 0973 7068 696e 782d 7461 6273 3d3d 332e  .sphinx-tabs==3.
+000004f0: 342e 310d 0a09 7370 6869 6e78 6177 6573  4.1...sphinxawes
+00000500: 6f6d 652d 7468 656d 653d 3d34 2e31 2e30  ome-theme==4.1.0
+00000510: 0d0a 0973 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
+00000520: 2d61 7070 6c65 6865 6c70 3d3d 312e 302e  -applehelp==1.0.
+00000530: 340d 0a09 7370 6869 6e78 636f 6e74 7269  4...sphinxcontri
+00000540: 622d 6465 7668 656c 703d 3d31 2e30 2e32  b-devhelp==1.0.2
+00000550: 0d0a 0973 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
+00000560: 2d68 746d 6c68 656c 703d 3d32 2e30 2e31  -htmlhelp==2.0.1
+00000570: 0d0a 0973 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
+00000580: 2d6a 7175 6572 793d 3d34 2e31 0d0a 0973  -jquery==4.1...s
+00000590: 7068 696e 7863 6f6e 7472 6962 2d6a 736d  phinxcontrib-jsm
+000005a0: 6174 683d 3d31 2e30 2e31 0d0a 0973 7068  ath==1.0.1...sph
+000005b0: 696e 7863 6f6e 7472 6962 2d71 7468 656c  inxcontrib-qthel
+000005c0: 703d 3d31 2e30 2e33 0d0a 0973 7068 696e  p==1.0.3...sphin
+000005d0: 7863 6f6e 7472 6962 2d73 6572 6961 6c69  xcontrib-seriali
+000005e0: 7a69 6e67 6874 6d6c 3d3d 312e 312e 350d  zinghtml==1.1.5.
+000005f0: 0a09 6661 7374 7472 6565 7368 6170 0d0a  ..fasttreeshap..
+00000600: 7465 7374 203d 200d 0a09 7079 7465 7374  test = ...pytest
+00000610: 0d0a 0970 7974 6573 742d 636f 760d 0a0d  ...pytest-cov...
+00000620: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000630: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000640: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `arfs-2.0.1/src/arfs/association.py` & `arfs-2.0.2/src/arfs/association.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import pandas as pd
 import scipy.stats as ss
 import matplotlib.pyplot as plt
 import scipy.cluster.hierarchy as sch
 import scipy.stats as ss
 
 
-
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from sklearn.utils import as_float_array, safe_sqr, safe_mask
 from multiprocessing import cpu_count
 from itertools import combinations, permutations, product
 from pandas.api.types import is_numeric_dtype
 from scipy.stats import rankdata
 from functools import partial
@@ -1432,27 +1431,35 @@
 
 ################################
 # Association predictor-target
 ################################
 
 
 def f_oneway_weighted(*args):
-    """f_oneway_weighted calculates the weighted F-statistic
-    (continuous target, categorical predictor)
+    """Calculate the weighted F-statistic for one-way ANOVA (continuous target, categorical predictor).
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples,)
+        The predictor dataframe.
+    y : array-like of shape (n_samples,)
+        The target vector.
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None.
 
     Returns
     -------
     float
-        value of the F-statistic
+        The value of the F-statistic.
 
-    Notes:
-    ------
-    F-statistic is calculated as:
+    Notes
+    -----
+    The F-statistic is calculated as:
     .. math::
-        F(rf)=\frac{\sum_i (\bar{Y}_{i \bullet}-\bar{Y})^2 \mathbin{/} (K-1)}{\sum_i \sum_k (\bar{Y}_{ij}-\bar{Y}_{i\bullet})^2 \mathbin{/} (N - K)}
+        F(rf) = \\frac{\\sum_i (\\bar{Y}_{i \\bullet} - \\bar{Y})^2 / (K-1)}{\\sum_i \\sum_k (\\bar{Y}_{ij} - \\bar{Y}_{i\\bullet})^2 / (N - K)}
     """
     # how many levels (predictor)
     n_classes = len(args)
     # convert to float 2-uple d'array
     args = [as_float_array(a) for a in args]
     # compute the total weight per level
     weight_per_class = np.array([a[1].sum() for a in args])
@@ -1579,58 +1586,56 @@
     )
 
 
 def f_cont_regression_parallel(
     X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
 ):
     """Univariate linear regression tests returning F-statistic.
+
     Quick linear model for testing the effect of a single regressor,
     sequentially for many regressors.
     This is done in 2 steps:
-    1. The cross correlation between each regressor and the target is computed
-       using
+    1. The cross-correlation between each regressor and the target is computed using:
            E[(X[:, i] - mean(X[:, i])) * (y - mean(y))] / (std(X[:, i]) * std(y))
-    2. It is converted to an F score ranks
-    features in the same order if all the features are positively correlated
-    with the target.
-    Note it is therefore recommended as a feature selection criterion to identify
-    potentially predictive feature for a downstream classifier, irrespective of
+    2. It is converted to an F score ranks features in the same order if all the features
+       are positively correlated with the target.
+    Note that it is therefore recommended as a feature selection criterion to identify
+    potentially predictive features for a downstream classifier, irrespective of
     the sign of the association with the target variable.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
-        predictor dataframe
+        The predictor dataframe.
     y : array-like of shape (n_samples,)
-        The target vector
+        The target vector.
     sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
+        The weight vector, by default None.
     n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
+        The number of cores to use for the computation, by default -1.
     handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    force_finite :
+        Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
         Whether or not to force the F-statistics and associated p-values to
         be finite. There are two cases where the F-statistic is expected to not
         be finite:
         - when the target `y` or some features in `X` are constant. In this
           case, the Pearson's R correlation is not defined leading to obtain
           `np.nan` values in the F-statistic and p-value. When
           `force_finite=True`, the F-statistic is set to `0.0` and the
           associated p-value is set to `1.0`.
-        - when the a feature in `X` is perfectly correlated (or
+        - when a feature in `X` is perfectly correlated (or
           anti-correlated) with the target `y`. In this case, the F-statistic
           is expected to be `np.inf`. When `force_finite=True`, the F-statistic
           is set to `np.finfo(dtype).max`.
 
-
     Returns
     -------
-    float :
-        F-statistic for each feature of shape (n_features,)
+    f_statistic : array-like of shape (n_features,)
+        F-statistic for each feature.
     """
     if not isinstance(y, pd.Series):
         y = pd.Series(y)
         y.name = "target"
 
     target = y.name
     X[target] = y.values
@@ -1663,41 +1668,38 @@
 ):
     """f_stat_regression_parallel computes the weighted explained variance for the provided categorical
     and numerical predictors using parallelization of the code.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
-        predictor dataframe
+        Predictor dataframe.
     y : array-like of shape (n_samples,)
-        The target vector
+        The target vector.
     sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
+        The weight vector, by default None.
     n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
+        The number of cores to use for the computation, by default -1.
     handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    force_finite :
-        Whether or not to force the F-statistics and associated p-values to
-        be finite. There are two cases where the F-statistic is expected to not
-        be finite:
-        - when the target `y` or some features in `X` are constant. In this
-          case, the Pearson's R correlation is not defined leading to obtain
-          `np.nan` values in the F-statistic and p-value. When
-          `force_finite=True`, the F-statistic is set to `0.0` and the
-          associated p-value is set to `1.0`.
-        - when the a feature in `X` is perfectly correlated (or
-          anti-correlated) with the target `y`. In this case, the F-statistic
-          is expected to be `np.inf`. When `force_finite=True`, the F-statistic
-          is set to `np.finfo(dtype).max`.
+        Either drop rows with NA, fill NA with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
+        Whether or not to force the F-statistics and associated p-values to be finite.
+        There are two cases where the F-statistic is expected to not be finite:
+        - When the target `y` or some features in `X` are constant. In this case,
+          the Pearson's R correlation is not defined leading to obtain `np.nan`
+          values in the F-statistic and p-value. When `force_finite=True`, the
+          F-statistic is set to `0.0` and the associated p-value is set to `1.0`.
+        - When a feature in `X` is perfectly correlated (or anti-correlated)
+          with the target `y`. In this case, the F-statistic is expected to be `np.inf`.
+          When `force_finite=True`, the F-statistic is set to `np.finfo(dtype).max`.
 
     Returns
     -------
     pd.Series
-        the value of the F-statistic for each predictor
+        The value of the F-statistic for each predictor.
     """
     f_stat_cont_series = f_cont_regression_parallel(
         X,
         y,
         sample_weight,
         n_jobs,
         force_finite=force_finite,
@@ -1828,51 +1830,51 @@
     X,
     y,
     sample_weight=None,
     n_jobs=-1,
     force_finite=True,
     handle_na="drop",
 ):
-    """Univariate information dependence
-    It is converted to an F score ranks features in the same order if
-    all the features are positively correlated with the target.
-    Note it is therefore recommended as a feature selection criterion to identify
-    potentially predictive feature for a downstream classifier, irrespective of
+    """Univariate information dependence.
+
+    It ranks features in the same order if all the features are positively correlated with the target.
+    Note that it is therefore recommended as a feature selection criterion to identify
+    potentially predictive features for a downstream classifier, irrespective of
     the sign of the association with the target variable.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
-        predictor dataframe
+        The predictor dataframe.
     y : array-like of shape (n_samples,)
-        The target vector
+        The target vector.
     sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
+        The weight vector, by default None.
     n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
+        The number of cores to use for the computation, by default -1.
     handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    force_finite :
+        Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
         Whether or not to force the F-statistics and associated p-values to
         be finite. There are two cases where the F-statistic is expected to not
         be finite:
         - when the target `y` or some features in `X` are constant. In this
           case, the Pearson's R correlation is not defined leading to obtain
           `np.nan` values in the F-statistic and p-value. When
           `force_finite=True`, the F-statistic is set to `0.0` and the
           associated p-value is set to `1.0`.
-        - when the a feature in `X` is perfectly correlated (or
+        - when a feature in `X` is perfectly correlated (or
           anti-correlated) with the target `y`. In this case, the F-statistic
           is expected to be `np.inf`. When `force_finite=True`, the F-statistic
           is set to `np.finfo(dtype).max`.
 
     Returns
     -------
-    f_statistic :
-        F-statistic for each feature of shape (n_features,)
+    f_statistic : array-like of shape (n_features,)
+        F-statistic for each feature.
     """
     if not isinstance(y, pd.Series):
         y = pd.Series(y)
         y.name = "target"
 
     target = y.name
     X[target] = y.values
@@ -1907,41 +1909,38 @@
 ):
     """f_stat_classification_parallel computes the weighted ANOVA F-value for the provided categorical
     and numerical predictors using parallelization of the code.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
-        predictor dataframe
+        Predictor dataframe.
     y : array-like of shape (n_samples,)
-        The target vector
+        The target vector.
     sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
+        The weight vector, by default None.
     n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
+        The number of cores to use for the computation, by default -1.
     handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    force_finite :
-        Whether or not to force the F-statistics and associated p-values to
-        be finite. There are two cases where the F-statistic is expected to not
-        be finite:
-        - when the target `y` or some features in `X` are constant. In this
-          case, the Pearson's R correlation is not defined leading to obtain
-          `np.nan` values in the F-statistic and p-value. When
-          `force_finite=True`, the F-statistic is set to `0.0` and the
-          associated p-value is set to `1.0`.
-        - when the a feature in `X` is perfectly correlated (or
-          anti-correlated) with the target `y`. In this case, the F-statistic
-          is expected to be `np.inf`. When `force_finite=True`, the F-statistic
-          is set to `np.finfo(dtype).max`.
+        Either drop rows with NA, fill NA with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
+        Whether or not to force the F-statistics and associated p-values to be finite.
+        There are two cases where the F-statistic is expected to not be finite:
+        - When the target `y` or some features in `X` are constant. In this case,
+          the Pearson's R correlation is not defined leading to obtain `np.nan`
+          values in the F-statistic and p-value. When `force_finite=True`, the
+          F-statistic is set to `0.0` and the associated p-value is set to `1.0`.
+        - When a feature in `X` is perfectly correlated (or anti-correlated)
+          with the target `y`. In this case, the F-statistic is expected to be `np.inf`.
+          When `force_finite=True`, the F-statistic is set to `np.finfo(dtype).max`.
 
     Returns
     -------
     pd.Series
-        the value of the F-statistic for each predictor
+        The value of the F-statistic for each predictor.
     """
     f_stat_cont_series = f_cont_classification_parallel(
         X, y, sample_weight, n_jobs, handle_na=handle_na
     )
     f_stat_cat_series = f_cat_classification_parallel(
         X,
         y,
@@ -2123,18 +2122,15 @@
     Returns
     -------
     pd.DataFrame
         a sorted square matrix
 
     Example:
     --------
-    >>> assoc = association_matrix(
-    ...     iris_df,
-    ...     plot=False
-    ... )
+    >>> assoc = association_matrix(iris_df, plot=False)
     >>> assoc_clustered = cluster_sq_matrix(assoc, method="complete")
 
     """
     d = sch.distance.pdist(sq_matrix.values)
     L = sch.linkage(d, method=method)
     ind = sch.fcluster(L, 0.5 * d.max(), "distance")
     columns = [sq_matrix.columns.tolist()[i] for i in list((np.argsort(ind)))]
@@ -2401,20 +2397,24 @@
     -------
     panel.Column
         the panel object
     """
     try:
         import holoviews as hv
     except ImportError:
-        raise ImportError("Holoviews is not installed. Please install it using 'pip install holoviews'.")
-    
+        raise ImportError(
+            "Holoviews is not installed. Please install it using 'pip install holoviews'."
+        )
+
     try:
         import panel as pn
     except ImportError:
-        raise ImportError("Panel is not installed. Please install it using 'pip install panel'.")
+        raise ImportError(
+            "Panel is not installed. Please install it using 'pip install panel'."
+        )
 
     cmap = cmap if cmap is not None else "coolwarm"
 
     # rename the columns for keeping track of num vs cat columns
     if suffix_dic is not None:
         rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
         assoc_mat = assoc_mat.rename(columns=rename_dic)
```

### Comparing `arfs-2.0.1/src/arfs/benchmark.py` & `arfs-2.0.2/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.0.2/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/dataset/data/housing.zip` & `arfs-2.0.2/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/feature_selection/__init__.py` & `arfs-2.0.2/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/feature_selection/allrelevant.py` & `arfs-2.0.2/src/arfs/feature_selection/allrelevant.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
         """
         try:
             from fasttreeshap import TreeExplainer as FastTreeExplainer
         except ImportError:
             warnings.warn("fasttreeshap is not installed. Fallback to shap.")
             self.importance = "shap"
-        
+
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a dataframe")
 
         self.imp_real_hist = np.empty((0, X.shape[1]), float)
         self._fit(X, y, sample_weight=sample_weight)
@@ -434,15 +434,15 @@
         # the basic cat features encoding
         # is performed when getting importances
         # because the columns are dynamically created/rejected
         X = X_raw
 
         # only sklearn requires to fillna data
         # modern GBM implementations can handle this
-        #X = X.fillna(0)
+        # X = X.fillna(0)
         y = pd.Series(y).fillna(0) if not isinstance(y, pd.Series) else y.fillna(0)
 
         # check input params
         self._check_params(X, y)
         sample_weight = validate_sample_weight(sample_weight)
         self.random_state = check_random_state(self.random_state)
 
@@ -497,15 +497,19 @@
             The number of features
 
         Returns
         -------
         n_estimators : int
             the number of trees
         """
-        depth = self.estimator.get_params()["max_depth"] if not self.is_cat else self.estimator.get_param("max_depth")
+        depth = (
+            self.estimator.get_params()["max_depth"]
+            if not self.is_cat
+            else self.estimator.get_param("max_depth")
+        )
         if depth is None:
             depth = 10
         # how many times a feature should be considered on average
         f_repr = 100
         # n_feat * 2 because the training matrix is extended with n shadow features
         multi = (n_feat * 2) / (np.sqrt(n_feat * 2) * depth)
         n_estimators = int(multi * f_repr)
@@ -1255,15 +1259,16 @@
                 # https://github.com/slundberg/shap/issues/526
                 shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_values], axis=0)
             else:
                 shap_imp = np.abs(shap_values).mean(0)
         else:
             shap_imp = np.abs(shap_values).mean(0)
     return shap_imp
-        
+
+
 def _get_shap_imp_fast(estimator, X, y, sample_weight=None, cat_feature=None):
     """Get the SHAP feature importance using the fasttreeshap implementation
 
     Parameters
     ----------
     estimator : estimator object
         An estimator object implementing `fit` and `predict` methods.
@@ -1285,15 +1290,20 @@
     # Clone the estimator to avoid modifying the original one
     estimator = clone(estimator)
 
     # Split the data into train and test sets and fit the model
     model, X_tt, y_tt, w_tt = _split_fit_estimator(
         estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
     )
-    explainer = FastTreeExplainer(model, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
+    explainer = FastTreeExplainer(
+        model,
+        algorithm="auto",
+        shortcut=False,
+        feature_perturbation="tree_path_dependent",
+    )
     shap_matrix = explainer.shap_values(X_tt)
     # multiclass returns a list
     # for binary and for some models, shap is still returning a list
     if is_classifier(estimator):
         if isinstance(shap_matrix, list):
             # For LightGBM classifier, RF, in sklearn API, SHAP returns a list of arrays
             # https://github.com/slundberg/shap/issues/526
@@ -1372,15 +1382,14 @@
     estimator = clone(estimator)
 
     try:
         if cat_feature is None:
             X, _, cat_idx = get_pandas_cat_codes(X)
         else:
             cat_idx = cat_feature
-        
 
         # handle catboost and cat features
         if is_catboost(estimator) or (
             "cat_feature" in estimator.fit.__code__.co_varnames
         ):
             X = pd.DataFrame(X)
             estimator.fit(X, y, sample_weight=sample_weight, cat_features=cat_idx)
@@ -1547,23 +1556,22 @@
             sample_weight, if any
         """
         try:
             from fasttreeshap import TreeExplainer as FastTreeExplainer
         except ImportError:
             warnings.warn("fasttreeshap is not installed. Fallback to shap.")
             self.importance = "shap"
-            
+
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a dataframe")
 
         if sample_weight is not None:
             sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
-            
 
         # crit, keep_vars, df_vimp, mean_shadow
         _, self.selected_features_, self.sha_cutoff_df, self.mean_shadow = _boostaroota(
             X,
             y,
             # metric=self.metric,
             estimator=self.estimator,
@@ -1751,15 +1759,20 @@
     ValueError
         error if the feature importance type is not
     """
     # Set up the parameters for running the model in XGBoost - split is on multi log loss
     for i in range(1, n_iterations + 1):
         # Create the shadow variables and run the model to obtain importances
         new_x, shadow_names = _create_shadow(X)
-        imp_func = {"shap": _get_shap_imp, "fastshap": _get_shap_imp, "pimp": _get_perm_imp, "native": _get_imp}
+        imp_func = {
+            "shap": _get_shap_imp,
+            "fastshap": _get_shap_imp,
+            "pimp": _get_perm_imp,
+            "native": _get_imp,
+        }
         importance = imp_func[imp_kind](
             estimator, new_x, y, sample_weight=weight, cat_feature=cat_feature
         )
 
         # Create a dataframe to store the feature importances
         if i == 1:
             df = pd.DataFrame({"feature": new_x.columns})
@@ -1911,15 +1924,15 @@
     - Cross-validated feature importance to smooth out the noise, based on lightGBM only
       (which is, most of the time, the fastest and more accurate Boosting).
     - the feature importance is derived using SHAP importance
     - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
       it improves the convergence (needs less evaluation to find a threshold)
     - Not based on a given percentage of cols needed to be deleted
     - Plot method for var. imp
-    
+
     Parameters
     ----------
     objective: str
         the lightGBM objective
     cutoff: float
         the value by which the max of shadow imp is divided, to compare to real importance
     n_folds: int, default=5
@@ -1935,16 +1948,16 @@
     lgbm_params: dict, Optional
         the parameters to pass to the lightGBM algorithm (python API). Note that some of
         those parameters will be overridden by the algorithm. Namely:
         objective, verbose, is_balanced
     n_jobs: int, default 0
         0 means default number of threads in OpenMP
         for the best speed, set this to the number of real CPU cores, not the number of threads
-    
-    
+
+
     Attributes
     ----------
     selected_features_: list of str
         the list of columns to keep
     ranking_ : array of shape [n_features]
         The feature ranking, such that ``ranking_[i]`` corresponds to the
         ranking position of the i-th feature. Selected (i.e., estimated
@@ -1966,29 +1979,38 @@
     >>>
     >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
     """
 
     def __init__(
-        self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False, fastshap=False, n_jobs=0, lgbm_params=None
+        self,
+        objective=None,
+        cutoff=1,
+        n_folds=5,
+        n_iter=5,
+        silent=True,
+        rf=False,
+        fastshap=False,
+        n_jobs=0,
+        lgbm_params=None,
     ):
         self.objective = objective
         self.cutoff = cutoff
         self.n_folds = n_folds
         self.n_iter = n_iter
         self.silent = silent
         self.rf = rf
-        self.fastshap = fastshap 
+        self.fastshap = fastshap
         self.cv_df = None
         self.sha_cutoff = None
         self.ranking_absolutes_ = None
         self.ranking_ = None
         self.lgbm_params = lgbm_params
-        self.n_jobs=n_jobs
+        self.n_jobs = n_jobs
 
         # Throw errors if the inputted parameters don't meet the necessary criteria
         # Ensure parameters meet necessary criteria
         if cutoff <= 0 or n_iter <= 0 or n_folds <= 0:
             raise ValueError("cutoff, n_iter, and n_folds should be greater than 0.")
 
     def fit(self, X, y, sample_weight=None):
@@ -2029,15 +2051,15 @@
             n_folds=self.n_folds,
             n_iter=self.n_iter,
             silent=self.silent,
             weight=sample_weight,
             rf=self.rf,
             fastshap=self.fastshap,
             lgbm_params=self.lgbm_params,
-            n_jobs=self.n_jobs
+            n_jobs=self.n_jobs,
         )
 
         self.selected_features_ = self.selected_features_.values
         self.support_ = np.asarray(
             [c in self.selected_features_ for c in self.feature_names_in_]
         )
         self.ranking_ = np.where(self.support_, 2, 1)
@@ -2135,15 +2157,28 @@
 #
 # GrootCV. In principle, you cannot/don't need to access those methods (reason of
 # the _ in front of the function name, they're internal functions)
 #
 ########################################################################################
 
 
-def _reduce_vars_lgb_cv(X, y, objective, n_folds, cutoff, n_iter, silent, weight, rf, fastshap, lgbm_params=None, n_jobs=0):
+def _reduce_vars_lgb_cv(
+    X,
+    y,
+    objective,
+    n_folds,
+    cutoff,
+    n_iter,
+    silent,
+    weight,
+    rf,
+    fastshap,
+    lgbm_params=None,
+    n_jobs=0,
+):
     """
     Reduce the number of predictors using a lightgbm (python API)
 
     Parameters
     ----------
     X : pd.DataFrame
             the dataframe to create shadow features on
@@ -2176,15 +2211,23 @@
             feature importance of the real predictors over iter
     df : pd.DataFrame
             feature importance of the real+shadow predictors over iter
     cutoff_shadow : float
             the feature importance threshold, to reject or not the predictors
     """
 
-    params = _set_lgb_parameters(X=X, y=y, objective=objective, rf=rf, silent=silent, n_jobs=n_jobs, lgbm_params=lgbm_params)
+    params = _set_lgb_parameters(
+        X=X,
+        y=y,
+        objective=objective,
+        rf=rf,
+        silent=silent,
+        n_jobs=n_jobs,
+        lgbm_params=lgbm_params,
+    )
 
     dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
     category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
     cat_idx = [X.columns.get_loc(col) for col in category_cols]
 
     rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
     iter = 0
@@ -2209,15 +2252,17 @@
             weight_val,
             category_cols=category_cols,
             early_stopping_rounds=20,
             fastshap=fastshap,
             **params,
         )
 
-        importance = _compute_importance(new_x_tr, shap_matrix, params, objective, fastshap)
+        importance = _compute_importance(
+            new_x_tr, shap_matrix, params, objective, fastshap
+        )
         df = _merge_importance_df(
             df=df,
             importance=importance,
             iter=iter,
             n_folds=n_folds,
             column_names=new_x_tr.columns,
             silent=silent,
@@ -2235,15 +2280,21 @@
     cutoff_shadow = shadow_vars.select_dtypes(include=[np.number]).max().mean() / cutoff
     real_vars = real_vars[(real_vars.Med.values >= cutoff_shadow)]
 
     return real_vars["feature"], df, cutoff_shadow
 
 
 def _set_lgb_parameters(
-    X: np.ndarray, y: np.ndarray, objective: str, rf: bool, silent: bool, n_jobs: int = 0, lgbm_params: dict = None
+    X: np.ndarray,
+    y: np.ndarray,
+    objective: str,
+    rf: bool,
+    silent: bool,
+    n_jobs: int = 0,
+    lgbm_params: dict = None,
 ) -> dict:
     """Set parameters for a LightGBM model based on the input features and the objective.
 
     Parameters
     ----------
     X : numpy array or pandas DataFrame
         The feature matrix of the training data.
@@ -2286,15 +2337,25 @@
                 "boosting_type": "rf",
                 "bagging_fraction": 0.7,
                 "feature_fraction": feat_frac,
                 "bagging_freq": 1,
             }
         )
 
-    clf_losses = [ "binary", "softmax", "multi_logloss", "multiclassova", "multiclass", "multiclass_ova", "ova", "ovr", "binary_logloss"]
+    clf_losses = [
+        "binary",
+        "softmax",
+        "multi_logloss",
+        "multiclassova",
+        "multiclass",
+        "multiclass_ova",
+        "ova",
+        "ovr",
+        "binary_logloss",
+    ]
     if objective in clf_losses:
         y = y.astype(int)
         y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
         n_classes = y_freq_table.size
         if n_classes > 2 and objective != "softmax":
             params["objective"] = "softmax"
             params["num_class"] = len(np.unique(y))
@@ -2303,25 +2364,34 @@
         main_class = y_freq_table[0]
         if not silent:
             print("GrootCV: classification with unbalance classes")
         if main_class > 0.8:
             params.update({"is_unbalance": True})
 
     params.update({"num_threads": n_jobs})
-    
+
     # we are using early_stopping
     # we prevent the overridding of it by popping the n_iterations
-    keys_to_pop = ['num_iterations', 'num_iteration', 'n_iter', 'num_tree', 'num_trees',
-                   'num_round', 'num_rounds', 'nrounds', 'num_boost_round', 'n_estimators', 'max_iter']
+    keys_to_pop = [
+        "num_iterations",
+        "num_iteration",
+        "n_iter",
+        "num_tree",
+        "num_trees",
+        "num_round",
+        "num_rounds",
+        "nrounds",
+        "num_boost_round",
+        "n_estimators",
+        "max_iter",
+    ]
     for key in keys_to_pop:
         params.pop(key, None)
-    
-    return params
-
 
+    return params
 
 
 def _split_data(X, y, tridx, validx, weight=None):
     """
     Split data into train and validation sets based on provided indices.
 
     Parameters
@@ -2423,21 +2493,28 @@
         callbacks=[early_stopping(early_stopping_rounds, False, False)],
     )
 
     if fastshap:
         try:
             from fasttreeshap import TreeExplainer as FastTreeExplainer
         except ImportError:
-            raise ImportError("fasttreeshap is not installed. Please install it using 'pip/conda install fasttreeshap'.")
-        
-        explainer = FastTreeExplainer(bst, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
+            raise ImportError(
+                "fasttreeshap is not installed. Please install it using 'pip/conda install fasttreeshap'."
+            )
+
+        explainer = FastTreeExplainer(
+            bst,
+            algorithm="auto",
+            shortcut=False,
+            feature_perturbation="tree_path_dependent",
+        )
         shap_matrix = explainer.shap_values(X_train)
     else:
         shap_matrix = bst.predict(X_train, pred_contrib=True)
-    
+
     return bst, shap_matrix, bst.best_iteration
 
 
 def _compute_importance(new_x_tr, shap_matrix, param, objective, fastshap):
     """
     Compute feature importance scores using SHAP values.
```

### Comparing `arfs-2.0.1/src/arfs/feature_selection/base.py` & `arfs-2.0.2/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/feature_selection/lasso.py` & `arfs-2.0.2/src/arfs/feature_selection/lasso.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 from sklearn.base import BaseEstimator, TransformerMixin, RegressorMixin
 from sklearn.base import clone
 from sklearn.utils import check_array
 from sklearn.model_selection import StratifiedKFold, KFold
 from joblib import Parallel, delayed
 from typing import Any, Callable, Union, List, Tuple, Optional, Dict, Literal
 
-def _map_family_link(family: str = "gaussian", link: Optional[str]=None):
+
+def _map_family_link(family: str = "gaussian", link: Optional[str] = None):
     family_mapping = {
         "gaussian": sm.families.Gaussian,
         "binomial": sm.families.Binomial,
         "poisson": sm.families.Poisson,
         "gamma": sm.families.Gamma,
         "negativebinomial": sm.families.NegativeBinomial,
-        "tweedie": sm.families.Tweedie
-        }
+        "tweedie": sm.families.Tweedie,
+    }
     link_mapping = {
         "identity": sm.genmod.families.links.Identity(),
         "log": sm.genmod.families.links.Log(),
         "logit": sm.genmod.families.links.Logit(),
         "probit": sm.genmod.families.links.Probit(),
         "cloglog": sm.genmod.families.links.CLogLog(),
-        "inverse_squared": sm.genmod.families.links.InverseSquared()
-        }
+        "inverse_squared": sm.genmod.families.links.InverseSquared(),
+    }
     if link is not None:
         objective = family_mapping[family](link_mapping[link])
     else:
         objective = family_mapping[family]()
     return objective
 
+
 class EnetGLM(BaseEstimator, RegressorMixin):
     """
     Elastic Net Generalized Linear Model.
 
     Parameters
     ----------
     family : statsmodels.family object, optional (default=sm.families.Gaussian())
@@ -45,194 +47,223 @@
     L1_wt : float, optional (default=0.0)
         The weight of the L1 penalty term. 0 <= L1_wt <= 1.
         L1_wt = 0 is equivalent to ridge regression, L1_wt = 1 is equivalent to lasso regression.
     fit_intercept : bool, optional (default=True)
         Whether to fit an intercept term in the model.
     """
 
-    def __init__(self, family: str = "gaussian", link: Optional[str] = None, alpha: float = 0.0, L1_wt: float = 0.0, fit_intercept: bool = True):
+    def __init__(
+        self,
+        family: str = "gaussian",
+        link: Optional[str] = None,
+        alpha: float = 0.0,
+        L1_wt: float = 1e-6,
+        fit_intercept: bool = True,
+    ):
         """
         Initialize self.
 
         Parameters
         ----------
-        family : 
+        family :
             The distributional assumption of the model.
         link:
             the GLM link function
-        alpha : 
-            The elastic net mixing parameter. 0 <= alpha <= 1.
-            alpha = 0 is equivalent to ridge regression, alpha = 1 is equivalent to lasso regression.
-        L1_wt : 
-            The weight of the L1 penalty term. 0 <= L1_wt <= 1.
-            L1_wt = 0 is equivalent to ridge regression, L1_wt = 1 is equivalent to lasso regression.
-        fit_intercept : 
+        alpha :
+            The penalty weight. If a scalar, the same penalty weight applies to all variables in the model. 
+            If a vector, it must have the same length as params, and contains a penalty weight for each coefficient.
+        L1_wt :
+            The `L1_wt` parameter represents the weight of the L1 penalty term in the model and 
+            should be within the range 0 to 1. A value of 0 corresponds to ridge regression, 
+            while a value of 1 corresponds to lasso regression. However, for obtaining statistics, 
+            `L1_wt` should be set to a value greater than 0. If it is set to 0.0, statsmodels returns 
+            a ridge regularized wrapper without refitting the model, making the statistics unavailable 
+            and breaking the class. Nevertheless, you can set `L1_wt` to a very small value, such as 1e-9, 
+            to obtain close-to-ridge behavior while still obtaining the necessary statistics.
+            
+        fit_intercept :
             Whether to fit an intercept term in the model.
         """
         self.family = family
         self.link = link
         self.alpha = alpha
         self.L1_wt = L1_wt
         self.model = None
         self.result = None
         self.fit_intercept = fit_intercept
         self.objective = _map_family_link(family=family, link=link)
 
-    def fit(self, X: pd.DataFrame, y: Union[np.ndarray, pd.Series], sample_weight: Optional[Union[np.ndarray, pd.Series]] = None):
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: Union[np.ndarray, pd.Series],
+        sample_weight: Optional[Union[np.ndarray, pd.Series]] = None,
+    ):
         """
         Fit the model to the data.
-        
+
         Notes
         -----
-        In statsmodels and GLMs in general, you can use either an offset or a weight to account for 
-        differences in exposure between observations. However, if you choose to use an offset, 
-        you need to pass the number of cases (ncl) instead of the frequency and set the offset to 
-        the logarithm of the exposure due to the log link function. It is recommended to use the frequency 
-        and the weights instead of the offset because this ensures that all models have the same inputs. 
+        In statsmodels and GLMs in general, you can use either an offset or a weight to account for
+        differences in exposure between observations. However, if you choose to use an offset,
+        you need to pass the number of cases (ncl) instead of the frequency and set the offset to
+        the logarithm of the exposure due to the log link function. It is recommended to use the frequency
+        and the weights instead of the offset because this ensures that all models have the same inputs.
         To use the frequency and the weights, you can fit the model using the following code:
-        
+
         ```python
         self.model = sm.GLM(endog=y, exog=X, var_weights=sample_weight, family=self.family)
         ```
-        
+
         This is equivalent to using the exposure and the log of the exposure internally, which can be done using the following code:
-                
+
         ```python
         self.model = sm.GLM(endog=y, exog=sm.add_constant(X), exposure=sample_weight, family=sm.families.Poisson())
         self.result = self.model.fit()
         ```
-        
+
         Parameters
         ----------
-        X : 
+        X :
             array-like, shape (n_samples, n_features)
             The input data.
-        y : 
+        y :
             array-like, shape (n_samples,)
             The target values.
         sample_weight : array-like, shape (n_samples,), optional (default=None)
             Sample weights.
 
         Returns
         -------
         self : object
             Returns self.
         """
+        
+        # see the if kwargs.get("L1_wt", 1) == 0 condition in
+        # https://www.statsmodels.org/dev/_modules/statsmodels/genmod/generalized_linear_model.html#GLM.fit_regularized
+        # workaround to get the statistics
+        if self.alpha == 0.0:
+            self.alpha = 1e-9
+        
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
             X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-            
+
         if self.fit_intercept:
             X = sm.add_constant(X)
-            X = X.rename(columns={'const': 'Intercept'})
+            X = X.rename(columns={"const": "Intercept"})
         else:
             X = drop_existing_sm_constant_from_df(X)
 
         self.n_features_in_ = X.shape[1]
-        
+
         self.model = sm.GLM(
             endog=y,
             exog=X,
             var_weights=sample_weight,
             family=self.objective,
         )
-        
-        
-        self.result = self.model.fit_regularized(method="elastic_net", alpha=self.alpha, L1_wt=self.L1_wt, refit=True)
+
+        self.result = self.model.fit_regularized(
+            method="elastic_net", alpha=self.alpha, L1_wt=self.L1_wt, refit=True
+        )
         self.coef_ = self.result.params
         self.bse_ = self.result.bse
         self.deviance_ = self.result.deviance
         self.pseudo_rsquared_ = self.result.pseudo_rsquared()
         self.aic_ = self.result.aic
         self.bic_ = self.result.bic_llf
         self.pvalues_ = self.result.pvalues
         self.tvalues_ = self.result.tvalues
         self.pearson_chi2_ = self.result.pearson_chi2
 
-
     def predict(self, X):
         """
         Predict using the fitted model.
 
         Parameters
         ----------
-        X : 
+        X :
             array-like, shape (n_samples, n_features)
             The input data.
-            
+
         Returns
         -------
         y : array-like, shape (n_samples,)
             The predicted target values.
 
         Raises
         ------
         ValueError
             If the model has not been fit.
         """
         if self.model is None:
             raise ValueError("Fit the model first.")
-        
+
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
             X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-        
+
         if self.fit_intercept:
             X = sm.add_constant(X)
-            X = X.rename(columns={'const': 'Intercept'})
+            X = X.rename(columns={"const": "Intercept"})
 
-        return self.result.predict()
+        return self.result.predict(X)
 
     def get_coef(self):
         """
         Get the estimated coefficients of the fitted model.
 
         Returns
         -------
         coef_ : array-like, shape (n_features,)
             The estimated coefficients of the fitted model.
         """
         return self.coef_
 
-    def score(self, X: pd.DataFrame, y: pd.Series, sample_weight: Optional[Union[np.ndarray, pd.Series]] = None):
+    def score(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        sample_weight: Optional[Union[np.ndarray, pd.Series]] = None,
+    ):
         """
         Return the deviance of the fitted model.
 
         Parameters
         ----------
-        X : 
+        X :
             array-like, shape (n_samples, n_features)
             The input data.
         sample_weight : array-like, shape (n_samples,), optional (default=None)
             Sample weights.
 
         Returns
         -------
         deviance : float
             The deviance of the fitted model.
         """
         mu = self.objective.link.inverse(self.predict(X))
 
         var_weights = sample_weight if sample_weight is not None else 1.0
         return self.objective.deviance(endog=y, mu=mu, var_weights=var_weights)
-            
+
     def summary(self):
         """
         Print a summary of the fitted model.
 
         Returns
         -------
         summary : str
             The summary of the fitted model.
         """
         return self.result.summary()
 
-def weighted_cross_val_score(
-    estimator, X, y, sample_weight=None, cv=5, n_jobs=-1
-):
+
+def weighted_cross_val_score(estimator, X, y, sample_weight=None, cv=5, n_jobs=-1):
     """
     Perform cross-validation for a scikit-learn estimator with a score function that requires sample_weight.
 
     Parameters
     ----------
     estimator : estimator
         The scikit-learn estimator object.
@@ -240,44 +271,49 @@
         The input features.
     y : array-like of shape (n_samples,)
         The target variable.
     sample_weight : array-like of shape (n_samples,), optional
         The sample weights for each data point.
     cv : int, default=5
         The number of cross-validation folds.
-    n_jobs: 
+    n_jobs:
         the number of processes
 
     Returns
     -------
     scores : array of shape (cv,)
         The list of scores for each fold.
     average_score : float
         The average score across all folds.
 
     """
 
     # logging.info("Starting cross-validation...")
 
-    splitter = KFold(n_splits=cv) if len(np.unique(y)) > 2 else StratifiedKFold(n_splits=cv)
-    
-    if not hasattr(estimator, 'score') or not callable(getattr(estimator, 'score')):
+    splitter = (
+        KFold(n_splits=cv) if len(np.unique(y)) > 2 else StratifiedKFold(n_splits=cv)
+    )
+
+    if not hasattr(estimator, "score") or not callable(getattr(estimator, "score")):
         raise ValueError(
             "The estimator does not have a score method that takes a sample_weight argument."
         )
 
     with Parallel(n_jobs=-1) as parallel:
         scores = parallel(
-            delayed(_fit_and_score)(estimator, X, y, train_index, test_index, sample_weight)
+            delayed(_fit_and_score)(
+                estimator, X, y, train_index, test_index, sample_weight
+            )
             for train_index, test_index in splitter.split(X)
         )
 
     # logging.info("Finished cross-validation.")
     return scores
 
+
 def _fit_and_score(
     estimator: BaseEstimator,
     X: Union[pd.DataFrame, np.ndarray],
     y: Union[pd.Series, np.ndarray],
     train_index: np.ndarray,
     test_index: np.ndarray,
     sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
@@ -312,27 +348,30 @@
     """
     # X = X.values if isinstance(X, pd.DataFrame) else X
     y = y.values if isinstance(y, pd.Series) else y
     X_train, X_test = X.iloc[train_index, :], X.iloc[test_index, :]
     y_train, y_test = y[train_index], y[test_index]
 
     if sample_weight is not None:
-        sample_weight = sample_weight.values if isinstance(sample_weight, pd.Series) else sample_weight
+        sample_weight = (
+            sample_weight.values
+            if isinstance(sample_weight, pd.Series)
+            else sample_weight
+        )
         sample_weight_train = sample_weight[train_index]
         sample_weight_test = sample_weight[test_index]
         estimator.fit(X_train, y_train, sample_weight=sample_weight_train)
         score = estimator.score(X_test, y_test, sample_weight=sample_weight_test)
     else:
         estimator.fit(X_train, y_train)
         score = estimator.score(X_test, y_test)
 
     return score
 
 
-
 def grid_search_cv(
     X: Union[pd.DataFrame, np.ndarray],
     y: Union[pd.Series, np.ndarray],
     sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
     n_iterations: int = 10,
     family: str = "gaussian",
     score: str = "bic",
@@ -376,30 +415,47 @@
         raise ValueError("Invalid score value. Options are: 'bic' or 'deviance'.")
 
     grid = np.logspace(-3, 3, n_iterations)
     param_score = []
 
     for param in grid:
         estimator = clone(estimator)
-        estimator.set_params(**{'alpha': param, 'L1_wt': 1.0, 'fit_intercept': fit_intercept, 'family': family})
+        estimator.set_params(
+            **{
+                "alpha": param,
+                "L1_wt": 1.0,
+                "fit_intercept": fit_intercept,
+                "family": family,
+            }
+        )
 
         if score == "bic":
             estimator.fit(X=X, y=y, sample_weight=sample_weight)
             param_score.append(estimator.bic_)
         else:
-            scores = weighted_cross_val_score(estimator, X, y, sample_weight=sample_weight, cv=5, n_jobs=-1)
+            scores = weighted_cross_val_score(
+                estimator, X, y, sample_weight=sample_weight, cv=5, n_jobs=-1
+            )
             param_score.append(np.mean(scores))
     # min deviance or min BIC
     best_alpha_value = grid[np.argmin(param_score)]
     best_estimator = clone(estimator)
-    best_estimator.set_params(**{'alpha': best_alpha_value, 'L1_wt': 1.0, 'fit_intercept': fit_intercept, 'family': family})
+    best_estimator.set_params(
+        **{
+            "alpha": best_alpha_value,
+            "L1_wt": 1.0,
+            "fit_intercept": fit_intercept,
+            "family": family,
+        }
+    )
     best_estimator.fit(X, y, sample_weight=sample_weight)
 
     return best_estimator
 
+
 class LassoFeatureSelection(BaseEstimator, TransformerMixin):
     """
     LassoFeatureSelection performs feature selection using GLM Lasso regularization.
 
     Parameters
     ----------
     family : str, default="gaussian"
@@ -433,15 +489,21 @@
     transform(X)
         Transform the input data to keep only the selected features.
     get_feature_names_out()
         Get the names of the selected features.
 
     """
 
-    def __init__(self, family: str = "gaussian", n_iterations: int = 10, score: str = "bic", fit_intercept: bool = True):
+    def __init__(
+        self,
+        family: str = "gaussian",
+        n_iterations: int = 10,
+        score: str = "bic",
+        fit_intercept: bool = True,
+    ):
         self.family = family
         self.n_iterations = n_iterations
         self.best_estimator_ = None
         self.selected_features_ = None
         self.support_ = None
         self.feature_names_in_ = None
         self.score = score
@@ -470,21 +532,33 @@
         LassoFeatureSelection
             The fitted LassoFeatureSelection model.
 
         """
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
             X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-            
+
         if not self.fit_intercept:
             X = drop_existing_sm_constant_from_df(X)
-        
-        self.feature_names_in_ = X.columns.insert(0, "Intercept") if self.fit_intercept and "Intercept" not in X.columns else X.columns
 
-        self.best_estimator_ = grid_search_cv(family=self.family, X=X, y=y, sample_weight=sample_weight, n_iterations=self.n_iterations, score=self.score, fit_intercept=self.fit_intercept)
+        self.feature_names_in_ = (
+            X.columns.insert(0, "Intercept")
+            if self.fit_intercept and "Intercept" not in X.columns
+            else X.columns
+        )
+
+        self.best_estimator_ = grid_search_cv(
+            family=self.family,
+            X=X,
+            y=y,
+            sample_weight=sample_weight,
+            n_iterations=self.n_iterations,
+            score=self.score,
+            fit_intercept=self.fit_intercept,
+        )
         self.support_ = self.best_estimator_.coef_ != 0
         self.selected_features_ = self.feature_names_in_[self.support_]
         return self
 
     def transform(self, X: Union[pd.DataFrame, np.ndarray]) -> pd.DataFrame:
         """
         Transform the input data to keep only the selected features.
@@ -497,37 +571,37 @@
         Returns
         -------
         Union[pd.DataFrame, np.ndarray]
             The transformed data with only the selected features.
 
         """
 
-            
         if self.fit_intercept:
             X = sm.add_constant(X)
-            
+
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
-            # if not a DF, assuming the col orders is 
+            # if not a DF, assuming the col orders is
             # the same, as required anyway
             X.columns = self.feature_names_in_
-            
-        X = X.rename(columns={'const': 'Intercept'}) if "const" in X.columns else X
+
+        X = X.rename(columns={"const": "Intercept"}) if "const" in X.columns else X
         return X[self.selected_features_]
 
     def get_feature_names_out(self) -> np.ndarray:
         """
         Get the names of the selected features.
 
         Returns
         -------
         np.ndarray
             The names of the selected features.
 
         """
         return self.feature_names_in_[self.support_]
-    
+
+
 def drop_existing_sm_constant_from_df(X):
-    X = X.drop(columns=['Intercept']) if 'Intercept' in X.columns else X
-    X = X.drop(columns=['const']) if 'const' in X.columns else X
-    X = X.drop(columns=['intercept']) if 'intercept' in X.columns else X
-    return X
+    X = X.drop(columns=["Intercept"]) if "Intercept" in X.columns else X
+    X = X.drop(columns=["const"]) if "const" in X.columns else X
+    X = X.drop(columns=["intercept"]) if "intercept" in X.columns else X
+    return X
```

### Comparing `arfs-2.0.1/src/arfs/feature_selection/mrmr.py` & `arfs-2.0.2/src/arfs/feature_selection/mrmr.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         if isinstance(X, pd.DataFrame):
             self.feature_names_in_ = X.columns.to_numpy()
         else:
             raise TypeError("X is not a pd.DataFrame")
 
         if not isinstance(y, pd.Series):
             y = pd.Series(y)
-            
+
         y.name = "target"
 
         target = y.copy()
         if self.task == "classification":
             target = target.astype("category")
 
         self.relevance_args = {"X": X, "y": target, "sample_weight": sample_weight}
```

### Comparing `arfs-2.0.1/src/arfs/feature_selection/summary.py` & `arfs-2.0.2/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/feature_selection/unsupervised.py` & `arfs-2.0.2/src/arfs/feature_selection/unsupervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,21 +35,23 @@
 
 
 def _missing_ratio(df):
     if not isinstance(df, pd.DataFrame):
         raise TypeError("df should be a pandas DataFrame")
     numeric_columns = df.select_dtypes(np.number).columns
     n_samples = len(df)
-    
+
     missing_counts = {}
     for column in df.columns:
         if column in numeric_columns:
-            missing_counts[column] = (df[column].isnull().sum() + np.isinf(df[column]).sum())/n_samples
+            missing_counts[column] = (
+                df[column].isnull().sum() + np.isinf(df[column]).sum()
+            ) / n_samples
         else:
-            missing_counts[column] = df[column].isnull().sum()/n_samples
+            missing_counts[column] = df[column].isnull().sum() / n_samples
     return pd.Series(missing_counts)
 
 
 class MissingValueThreshold(BaseThresholdSelector):
     """Feature selector that removes all high missing percentage features.
     This feature selection algorithm looks only at the features (X),
     not the desired outputs (y), and can thus be used for unsupervised learning.
```

### Comparing `arfs-2.0.1/src/arfs/feature_selection/variable_importance.py` & `arfs-2.0.2/src/arfs/feature_selection/variable_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             sample_weight=sample_weight,
             encode=self.encode,
             task=self.task,
             n_iterations=self.n_iterations,
             verbose=self.verbose,
             encoder_kwargs=self.encoder_kwargs,
             lgb_kwargs=self.lgb_kwargs,
-            fastshap=self.fastshap
+            fastshap=self.fastshap,
         )
 
         self.feature_importances_summary_ = feature_importances
 
         support_ordered = (
             self.feature_importances_summary_["cumulative_importance"] >= self.threshold
         )
@@ -368,24 +368,31 @@
 
         # pimp cool but too slow
         # perm_imp =  permutation_importance(
         # model, valid_features, valid_labels, n_repeats=10, random_state=42, n_jobs=-1
         # )
         # perm_imp = perm_imp.importances_mean
         if fastshap:
-            explainer = FastTreeExplainer(gbm_model.model, algorithm="auto", shortcut=False, feature_perturbation="tree_path_dependent")
+            explainer = FastTreeExplainer(
+                gbm_model.model,
+                algorithm="auto",
+                shortcut=False,
+                feature_perturbation="tree_path_dependent",
+            )
             shap_matrix = explainer.shap_values(gbm_model.valid_features)
             if isinstance(shap_matrix, list):
                 # For LightGBM classifier, RF, in sklearn API, SHAP returns a list of arrays
                 # https://github.com/slundberg/shap/issues/526
                 shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_matrix], axis=0)
             else:
                 shap_imp = np.abs(shap_matrix).mean(0)
         else:
-            shap_matrix = gbm_model.model.predict(gbm_model.valid_features, pred_contrib=True)
+            shap_matrix = gbm_model.model.predict(
+                gbm_model.valid_features, pred_contrib=True
+            )
             # the dim changed in lightGBM >= 3.0.0
             if task == "multiclass":
                 # X_SHAP_values (array-like of shape = [n_samples, n_features + 1]
                 # or shape = [n_samples, (n_features + 1) * n_classes])
                 # index starts from 0
                 n_feat = gbm_model.valid_features.shape[1]
                 y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
```

### Comparing `arfs-2.0.1/src/arfs/gbm.py` & `arfs-2.0.2/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/parallel.py` & `arfs-2.0.2/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/preprocessing.py` & `arfs-2.0.2/src/arfs/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -393,79 +393,78 @@
         # Map is faster than replace
     if return_cat:
         df.loc[:, non_num_cols] = df.loc[:, non_num_cols].astype("category")
     return df, cat_var_df, inv_mapper, mapper
 
 
 class TreeDiscretizer(BaseEstimator, TransformerMixin):
-    """The purpose of the function is to discretize continuous and/or categorical data, returning a pandas DataFrame. 
-    It is designed to support regression and binary classification tasks. Discretization, also known as quantization or binning, 
-    allows for the partitioning of continuous features into discrete values. In certain datasets with continuous attributes, 
-    discretization can be beneficial as it transforms the dataset into one with only nominal attributes. 
+    """The purpose of the function is to discretize continuous and/or categorical data, returning a pandas DataFrame.
+    It is designed to support regression and binary classification tasks. Discretization, also known as quantization or binning,
+    allows for the partitioning of continuous features into discrete values. In certain datasets with continuous attributes,
+    discretization can be beneficial as it transforms the dataset into one with only nominal attributes.
     Additionally, for categorical predictors, grouping levels can help reduce overfitting and create meaningful clusters.
 
-    By encoding discretized features, a model can become more expressive while maintaining interpretability. 
-    For example, preprocessing with a discretizer can introduce nonlinearity to linear models. 
+    By encoding discretized features, a model can become more expressive while maintaining interpretability.
+    For example, preprocessing with a discretizer can introduce nonlinearity to linear models.
     For more advanced possibilities, particularly smooth ones, you can refer to the section on generating polynomial features.
-    The TreeDiscretizer function utilizes univariate regularized trees, with one tree per column to be binned. 
-    It finds the optimal partition and returns numerical intervals for numerical continuous columns and pd.Categorical for categorical columns. 
+    The TreeDiscretizer function utilizes univariate regularized trees, with one tree per column to be binned.
+    It finds the optimal partition and returns numerical intervals for numerical continuous columns and pd.Categorical for categorical columns.
     This approach groups similar levels together, reducing dimensionality and regularizing the model.
-    
-    TreeDiscretizer handles missing values for both numerical and categorical predictors, 
+
+    TreeDiscretizer handles missing values for both numerical and categorical predictors,
     eliminating the need for encoding categorical predictors separately.
 
     Notes
     -----
-     This is a substitution to proper regularization scheme such as
-     - GroupLasso (categorical predictors, which are usually encoded as multiple dummy variables: one for each category.
-                   It makes sense in many analyses to consider these dummy variables (representing one categorical predictor)
-                   together rather than separately)
-     - FusedLasso (One drawback of the Lasso is it ignores ordering of the features, FusedLasso takes into account the ordering)
+    This is a substitution to proper regularization schemes such as:
+    - GroupLasso: Categorical predictors, which are usually encoded as multiple dummy variables,
+                  are considered together rather than separately.
+    - FusedLasso: Takes into account the ordering of the features.
 
     Parameters
     ----------
-    bin_features : List of string, str or None
-        the list of names of the variable that has to be binned, or "all", "numerical" or "categorical"
+    bin_features : List of string or None
+        The list of names of the variable that has to be binned, or "all", "numerical" or "categorical"
         for splitting and grouping all, only numerical or only categorical columns.
     n_bins : int
-        the number of bins that has to be created while binning the variables in "bin_features" list
+        The number of bins that has to be created while binning the variables in the "bin_features" list.
     n_bins_max : int, optional
-        the maximum number of levels that a categorical column can have in order to avoid being binned
+        The maximum number of levels that a categorical column can have to avoid being binned.
     num_bins_as_category: bool, default=False
-        save the numeric bins as pandas category or as pandas interval
-    boost_params : dic
-        the boosting parameters dictionary
+        Save the numeric bins as pandas category or as pandas interval.
+    boost_params : dict
+        The boosting parameters dictionary.
     raw : bool
-        returns raw levels (non human-interpretable) or levels matching the orginal ones
+        Returns raw levels (non-human-interpretable) or levels matching the original ones.
     task : str
-        either regression or classification (binary)
+        Either regression or classification (binary).
 
     Attributes
     ----------
-    tree_dic : dic
-        the dictionary keys are binned column names and items are the univariate trees
-    bin_upper_bound_dic : dic
-        the upper bound of the numerical intervals
-    cat_bin_dict : dic
-        the mapping dictionary for the categorical columns
-    tree_imputer : dic
-        the missing values are split by the tree and lead to similar splits and are mapped to this value
-    ordinal_encoder_dic : dic
-        dictionary with the fitted encoder, if any
+    tree_dic : dict
+        The dictionary keys are binned column names and items are the univariate trees.
+    bin_upper_bound_dic : dict
+        The upper bound of the numerical intervals.
+    cat_bin_dict : dict
+        The mapping dictionary for the categorical columns.
+    tree_imputer : dict
+        The missing values are split by the tree and lead to similar splits and are mapped to this value.
+    ordinal_encoder_dic : dict
+        Dictionary with the fitted encoder, if any.
     cat_features : list
-        names of the found categorical columns
+        Names of the found categorical columns.
 
     Methods
     -------
     fit(X, y, sample_weight=None)
-        fit the transformer object on data
-    transform(x)
-        apply the fitted transformer object on new data
-    fit_transform(x)
-        fit and apply the transformer object on data
+        Fit the transformer object on data.
+    transform(X)
+        Apply the fitted transformer object on new data.
+    fit_transform(X)
+        Fit and apply the transformer object on data.
 
     Example
     -------
     >>> lgb_params = {'min_split_gain': 5}
     >>> disc = TreeDiscretizer(bin_features='all', n_bins=10)
     >>> disc.fit(X=df[predictors], y=df['Frequency'], sample_weight=df['Exposure'])
     """
@@ -506,37 +505,38 @@
         self.cat_bin_dict = {}
         self.tree_imputer = {}
         self.ordinal_encoder_dic = {}
         self.cat_features = None
 
     def fit(self, X, y, sample_weight=None):
         """Fit the discretizer on `X`.
+
         Parameters
         ----------
-        X :
-            Input data shape (n_samples, n_features), where `n_samples` is the number of samples and
+        X : array-like of shape (n_samples, n_features)
+            Input data with shape (n_samples, n_features), where `n_samples` is the number of samples and
             `n_features` is the number of features.
-        y :
-            target for internally fitting the tree(s)
-        sample_weight :
-            sample weight (e.g. exposure) if any
+        y : array-like of shape (n_samples,)
+            Target for internally fitting the tree(s).
+        sample_weight : array-like of shape (n_samples,), optional
+            Sample weight (e.g., exposure) if any.
 
         Returns
         -------
-        X :
-            pd.DataFrame with the binned and grouped columns
+        X : pd.DataFrame
+            DataFrame with the binned and grouped columns.
         """
         X = X.copy()
-        
+
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
             X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-        
+
         self.feature_names_in_ = X.columns.to_numpy()
-        
+
         if self.bin_features is None:
             self.bin_features = list(X.select_dtypes("number").columns)
             self.cat_features = []
         elif isinstance(self.bin_features, list):
             self.cat_features = list(
                 set(self.bin_features)
                 - set(list(X[self.bin_features].select_dtypes("number").columns))
@@ -549,18 +549,22 @@
         elif isinstance(self.bin_features, str) and (self.bin_features == "numerical"):
             self.bin_features = list(X.select_dtypes("number").columns)
         elif isinstance(self.bin_features, str) and (
             self.bin_features == "categorical"
         ):
             self.bin_features = list(X.select_dtypes(["category", "object"]).columns)
             self.cat_features = self.bin_features
-            
+
         self.n_unique_table_ = X[self.bin_features].nunique()
         # transform only the columns with more than n_bins_max
-        self.bin_features = self.n_unique_table_[self.n_unique_table_ > self.n_bins_max].index.to_list() if self.n_bins_max else self.bin_features
+        self.bin_features = (
+            self.n_unique_table_[self.n_unique_table_ > self.n_bins_max].index.to_list()
+            if self.n_bins_max
+            else self.bin_features
+        )
 
         for col in self.bin_features:
             is_categorical = (self.cat_features is not None) and (
                 col in self.cat_features
             )
             if is_categorical:
                 encoder = OrdinalEncoder(
@@ -576,16 +580,15 @@
                 # encode
                 self.ordinal_encoder_dic[col] = encoder.fit(X[[col]])
                 dum = encoder.transform(X[[col]])
                 if isinstance(dum, pd.DataFrame):
                     X[col] = dum.values.ravel()
                 else:
                     X[col] = dum.ravel()
-                
-                
+
             else:
                 encoder = None
 
             gbm_param = self.boost_params.copy()
             tree = GradientBoosting(
                 cat_feat=None, params=gbm_param, show_learning_curve=False
             )
@@ -602,15 +605,15 @@
             if is_categorical:
                 # retrieve original values
                 dum = encoder.inverse_transform(X[[col]])
                 if isinstance(dum, pd.DataFrame):
                     X[col] = dum.values.ravel()
                 else:
                     X[col] = dum.ravel()
-                
+
                 self.cat_bin_dict[col] = (
                     X[[f"{col}_g", col]]
                     .groupby(f"{col}_g")
                     .apply(lambda x: " / ".join(map(str, x[col].unique())))
                     .to_dict()
                 )
             else:
@@ -640,26 +643,25 @@
 
             del tree
 
         return self
 
     def transform(self, X):
         """Apply the discretizer on `X`. Only the columns with more than n_bins_max unique values will be transformed.
-        
+
         Parameters
         ----------
-        X :
-            Input data shape (n_samples, n_features), where `n_samples` is the number of samples and
+        X : array-like of shape (n_samples, n_features)
+            Input data with shape (n_samples, n_features), where `n_samples` is the number of samples and
             `n_features` is the number of features.
 
-
         Returns
         -------
-        X :
-            pd.DataFrame with the binned and grouped columns
+        X : pd.DataFrame
+            DataFrame with the binned and grouped columns.
         """
         X = X.copy()
 
         for col in self.bin_features:
             if self.raw:
                 # predict each univariate tree
                 X[col] = self.tree_dic[col].predict(X[[col]])
@@ -683,15 +685,15 @@
                     # apply the binning
                     X[col] = pd.cut(
                         X[col],
                         bins=self.bin_upper_bound_dic[col],
                         include_lowest=True,
                         precision=2,
                     )
-                    
+
                     if not self.num_bins_as_category:
                         X[col] = X[col].astype(IntervalDtype())
         return X
 
 
 def highlight_discarded(s):
     """highlight X in red and V in green.
@@ -753,14 +755,15 @@
     tag_df = (
         tag_df.style.apply(highlight_discarded, subset=col_to_apply_style)
         .applymap(lambda x: "" if x == x else "background-color: #ffa500")
         .format(precision=0)
     )
     return tag_df
 
+
 class IntervalToMidpoint(BaseEstimator, TransformerMixin):
     """
     IntervalToMidpoint is a transformer that converts numerical intervals in a pandas DataFrame to their midpoints.
 
     Parameters
     ----------
     cols : list of str or str, default "all"
@@ -781,41 +784,44 @@
         Fit the transformer on the input data.
     transform(X)
         Transform the input data by converting numerical intervals to midpoints.
     inverse_transform(X)
         Inverse transform is not implemented for this transformer.
     """
 
-    def __init__(self, cols: Union[List[str], str]="all"):
-
+    def __init__(self, cols: Union[List[str], str] = "all"):
         self.cols = cols
 
     def fit(self, X: pd.DataFrame = None, y: pd.Series = None):
         """
         Fit the transformer on the input data.
 
         Parameters
         ----------
-        X : 
+        X :
             The input data to fit the transformer on.
-        y : 
+        y :
             Ignored parameter.
 
         Returns
         -------
         self : IntervalToMidpoint
             The fitted transformer object.
         """
         data = X.copy()
-        
+
         if self.cols == "all":
             self.cols = data.columns
-        
-        self.float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")["num_interval"]
-        self.columns_to_transform_ = list(set(self.cols).intersection(set(self.float_interval_cols_)))
+
+        self.float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")[
+            "num_interval"
+        ]
+        self.columns_to_transform_ = list(
+            set(self.cols).intersection(set(self.float_interval_cols_))
+        )
         return self
 
     def transform(self, X: pd.DataFrame):
         """
         Transform the input data by converting numerical intervals to midpoints.
 
         Parameters
@@ -847,43 +853,46 @@
         ------
         NotImplementedError
             Raised since inverse transform is not implemented for this transformer.
         """
         raise NotImplementedError(
             "inverse_transform is not implemented for this transformer."
         )
-        
-def transform_interval_to_midpoint(X: pd.DataFrame, cols: Union[List[str], str] = "all") -> pd.DataFrame:
+
+
+def transform_interval_to_midpoint(
+    X: pd.DataFrame, cols: Union[List[str], str] = "all"
+) -> pd.DataFrame:
     """
     Transforms interval columns in a pandas DataFrame to their midpoint values.
-    
+
     Notes
     -----
     Equivalent function to ``IntervalToMidpoint`` without the estimator API
 
     Parameters
     ----------
     X : pd.DataFrame
         The input DataFrame containing the data to be transformed.
     cols : list of str or str
         The columns to be transformed. Defaults to "all" which transforms all columns.
 
     Returns
     -------
-    pd.DataFrame : 
+    pd.DataFrame :
         The transformed DataFrame with interval columns replaced by their midpoint values.
 
     Raises
     ------
-    TypeError : 
+    TypeError :
         If the input data is not a pandas DataFrame.
     """
     if cols == "all":
         cols = X.columns
-    
+
     X = X.copy()
     float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")["num_interval"]
     columns_to_transform_ = list(set(cols).intersection(set(float_interval_cols_)))
     for c in columns_to_transform_:
         X.loc[:, c] = find_interval_midpoint(X[c])
     return X
 
@@ -903,18 +912,21 @@
     """
     left = interval_series.array.left
     right = interval_series.array.right
     mid = interval_series.array.mid
     left_inf = np.isinf(left)
     right_inf = np.isinf(right)
 
-    return np.where(left_inf & right_inf, np.inf,
-                        np.where(left_inf, right,
-                                 np.where(right_inf, left, mid)))
-    
+    return np.where(
+        left_inf & right_inf,
+        np.inf,
+        np.where(left_inf, right, np.where(right_inf, left, mid)),
+    )
+
+
 class PatsyTransformer(BaseEstimator, TransformerMixin):
     """Transformer using patsy-formulas.
 
     PatsyTransformer transforms a pandas DataFrame (or dict-like)
     according to the formula and produces a numpy array.
 
     Parameters
@@ -953,16 +965,23 @@
     PastyTransformer does by default not add an intercept, even if you
     specified it in the formula. You need to set add_intercept=True.
 
     As scikit-learn transformers can not ouput y, the formula
     should not contain a left hand side.  If you need to transform both
     features and targets, use PatsyModel.
     """
-    def __init__(self, formula=None, add_intercept=True, eval_env=0, NA_action="drop",
-                 return_type='dataframe'):
+
+    def __init__(
+        self,
+        formula=None,
+        add_intercept=True,
+        eval_env=0,
+        NA_action="drop",
+        return_type="dataframe",
+    ):
         self.formula = formula
         self.eval_env = eval_env
         self.add_intercept = add_intercept
         self.NA_action = NA_action
         self.return_type = return_type
 
     def fit(self, data, y=None):
@@ -988,32 +1007,39 @@
         -------
         X_transform : ndarray
             Transformed data
         """
         return self._fit_transform(data, y)
 
     def _fit_transform(self, data, y=None):
-        
         if not isinstance(data, pd.DataFrame):
             data = pd.DataFrame(data)
             data.columns = [f"pred_{i}" for i in range(data.shape[1])]
-        
+
         if not isinstance(y, pd.Series):
             y = pd.Series(y)
             y.name = "target"
-            
+
         target_name = y.name if y is not None else "y"
-        self.formula = self.formula or " + ".join(data.columns.difference([target_name]))
+        self.formula = self.formula or " + ".join(
+            data.columns.difference([target_name])
+        )
         eval_env = EvalEnvironment.capture(self.eval_env, reference=2)
         # self.formula = _drop_intercept(self.formula, self.add_intercept)
 
-        design = dmatrix(self.formula, data, NA_action=self.NA_action, return_type='dataframe', eval_env=eval_env)
+        design = dmatrix(
+            self.formula,
+            data,
+            NA_action=self.NA_action,
+            return_type="dataframe",
+            eval_env=eval_env,
+        )
         self.design_ = design.design_info
 
-        if self.return_type == 'dataframe':
+        if self.return_type == "dataframe":
             return design
         else:
             return np.array(design)
 
     def transform(self, data):
         """Transform with estimator using formula.
 
@@ -1021,22 +1047,22 @@
         using the estimator.
 
         Parameters
         ----------
         data : dict-like (pandas dataframe)
             Input data. Column names need to match variables in formula.
         """
-        if self.return_type == 'dataframe':
-            return dmatrix(self.design_, data, return_type='dataframe')
+        if self.return_type == "dataframe":
+            return dmatrix(self.design_, data, return_type="dataframe")
         else:
             return np.array(dmatrix(self.design_, data))
 
 
 def _drop_intercept(formula, add_intercept):
     """Drop the intercept from formula if not add_intercept"""
     if not add_intercept:
         if not isinstance(formula, ModelDesc):
             formula = ModelDesc.from_formula(formula)
         if INTERCEPT in formula.rhs_termlist:
             formula.rhs_termlist.remove(INTERCEPT)
         return formula
-    return formula
+    return formula
```

### Comparing `arfs-2.0.1/src/arfs/sampling.py` & `arfs-2.0.2/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/src/arfs/utils.py` & `arfs-2.0.2/src/arfs/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,27 +104,38 @@
     if not isinstance(df, pd.DataFrame):
         raise TypeError("df should be a pandas DataFrame")
 
     categorical_cols = df.select_dtypes(include=["object", "category", "bool"]).columns
     time_cols = df.select_dtypes(
         include=["datetime", "timedelta", "datetimetz"]
     ).columns
-    numerical_interval_cols = df.select_dtypes(["Interval[float]", "Interval[int]"]).columns
+    numerical_interval_cols = df.select_dtypes(
+        ["Interval[float]", "Interval[int]"]
+    ).columns
     numerical_cols = df.select_dtypes(include=np.number).columns
     remaining_cols = (
-        df.columns.difference(categorical_cols).difference(numerical_cols).difference(time_cols).difference(numerical_interval_cols)
+        df.columns.difference(categorical_cols)
+        .difference(numerical_cols)
+        .difference(time_cols)
+        .difference(numerical_interval_cols)
     )
 
     if dic_keys == "col_names":
         cat_dict = dict.fromkeys(categorical_cols, "cat")
         num_dict = dict.fromkeys(numerical_cols, "num")
         num_interval_dict = dict.fromkeys(numerical_interval_cols, "num_interval")
         time_dict = dict.fromkeys(time_cols, "time")
         remaining_dict = dict.fromkeys(remaining_cols, "unk")
-        return {**cat_dict, **num_dict, **num_interval_dict, **time_dict, **remaining_dict}
+        return {
+            **cat_dict,
+            **num_dict,
+            **num_interval_dict,
+            **time_dict,
+            **remaining_dict,
+        }
 
     if dic_keys == "dtypes":
         return {
             "cat": categorical_cols.tolist(),
             "num": numerical_cols.tolist(),
             "num_interval": numerical_interval_cols.tolist(),
             "time": time_cols.tolist(),
@@ -855,9 +866,9 @@
         "Gruber",
         "KeyserSoze",
         "Luthor",
         "Klaue",
         "Bane",
         "MarkZ",
     ]
-    
+
     return X, y, w
```

### Comparing `arfs-2.0.1/src/arfs.egg-info/PKG-INFO` & `arfs-2.0.2/src/arfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.1
+Version: 2.0.2
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
@@ -28,15 +28,15 @@
 
 # All relevant feature selection
 
 All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
 
 This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
 
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for intrucing non-linearities into linear models and perform feature selection.
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
 
 Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
 `$ pip install arfs`, requires python <3.10
```

### Comparing `arfs-2.0.1/src/arfs.egg-info/SOURCES.txt` & `arfs-2.0.2/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/tests/test_allrelevant.py` & `arfs-2.0.2/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.1/tests/test_featselect.py` & `arfs-2.0.2/tests/test_featselect.py`

 * *Files identical despite different names*

