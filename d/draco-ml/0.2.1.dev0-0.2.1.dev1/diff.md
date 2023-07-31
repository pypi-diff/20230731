# Comparing `tmp/draco-ml-0.2.1.dev0.tar.gz` & `tmp/draco-ml-0.2.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draco-ml-0.2.1.dev0.tar", last modified: Wed Apr 26 14:33:59 2023, max compression
+gzip compressed data, was "draco-ml-0.2.1.dev1.tar", last modified: Mon Jul 31 14:34:14 2023, max compression
```

## Comparing `draco-ml-0.2.1.dev0.tar` & `draco-ml-0.2.1.dev1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.012706 draco-ml-0.2.1.dev0/
--rw-r--r--   0 sarah      (501) staff       (20)       94 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8306 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3069 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/HISTORY.md
--rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      297 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)    14191 2023-04-26 14:33:59.013166 draco-ml-0.2.1.dev0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)    10324 2023-04-13 20:29:53.000000 draco-ml-0.2.1.dev0/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.968815 draco-ml-0.2.1.dev0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      606 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/Makefile
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.970767 draco-ml-0.2.1.dev0/docs/advanced_usage/
--rw-r--r--   0 sarah      (501) staff       (20)     2501 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/advanced_usage/concepts.md
--rw-r--r--   0 sarah      (501) staff       (20)     2537 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/advanced_usage/csv.md
--rw-r--r--   0 sarah      (501) staff       (20)     3532 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/advanced_usage/docker.md
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/authors.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5886 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)       33 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/history.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.973358 draco-ml-0.2.1.dev0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)     7263 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/images/Draco-200.png
--rw-r--r--   0 sarah      (501) staff       (20)    27132 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/images/Draco.png
--rw-r--r--   0 sarah      (501) staff       (20)   886153 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/images/dai-logo.png
--rw-r--r--   0 sarah      (501) staff       (20)      541 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      767 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/make.bat
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/readme.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.985453 draco-ml-0.2.1.dev0/draco/
--rw-r--r--   0 sarah      (501) staff       (20)      517 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    36486 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/benchmark.py
--rw-r--r--   0 sarah      (501) staff       (20)     2103 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/db.py
--rw-r--r--   0 sarah      (501) staff       (20)     2925 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/demo.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.987092 draco-ml-0.2.1.dev0/draco/loaders/
--rw-r--r--   0 sarah      (501) staff       (20)       72 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/loaders/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     8858 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/loaders/csv.py
--rw-r--r--   0 sarah      (501) staff       (20)     2768 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/metrics.py
--rw-r--r--   0 sarah      (501) staff       (20)    23386 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipeline.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.955813 draco-ml-0.2.1.dev0/draco/pipelines/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.991727 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/
--rw-r--r--   0 sarah      (501) staff       (20)     2516 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     2716 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob.json
--rw-r--r--   0 sarah      (501) staff       (20)     3502 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     3302 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_with_unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.992797 draco-ml-0.2.1.dev0/draco/pipelines/dummy/
--rw-r--r--   0 sarah      (501) staff       (20)      166 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/dummy/dummy.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.997426 draco-ml-0.2.1.dev0/draco/pipelines/lstm/
--rw-r--r--   0 sarah      (501) staff       (20)     2504 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     2704 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob.json
--rw-r--r--   0 sarah      (501) staff       (20)     3490 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob_with_unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     3290 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_with_unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.000169 draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/
--rw-r--r--   0 sarah      (501) staff       (20)     2502 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     3286 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.003246 draco-ml-0.2.1.dev0/draco/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)      862 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/primitives/mlblocks.MLPipeline.json
--rw-r--r--   0 sarah      (501) staff       (20)      918 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/primitives/numpy.take.json
--rw-r--r--   0 sarah      (501) staff       (20)     2232 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/primitives/xgboost.XGBClassifier:probabilities.json
--rw-r--r--   0 sarah      (501) staff       (20)     3852 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/results.py
--rw-r--r--   0 sarah      (501) staff       (20)     6143 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/targets.py
--rw-r--r--   0 sarah      (501) staff       (20)     1682 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.008370 draco-ml-0.2.1.dev0/draco_ml.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    14191 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1523 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)       87 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      833 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        6 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1023 2023-04-26 14:33:59.015084 draco-ml-0.2.1.dev0/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     2999 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.011654 draco-ml-0.2.1.dev0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)     1860 2023-04-13 20:29:53.000000 draco-ml-0.2.1.dev0/tests/test_benchmark.py
--rw-r--r--   0 sarah      (501) staff       (20)     1218 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/tests/test_metrics.py
--rw-r--r--   0 sarah      (501) staff       (20)     2547 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/tests/test_pipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.536177 draco-ml-0.2.1.dev1/
+-rw-r--r--   0 sarah      (501) staff       (20)       94 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8306 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3543 2023-07-31 14:33:58.000000 draco-ml-0.2.1.dev1/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      297 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    14665 2023-07-31 14:34:14.536333 draco-ml-0.2.1.dev1/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)    10324 2023-04-13 20:29:53.000000 draco-ml-0.2.1.dev1/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.510249 draco-ml-0.2.1.dev1/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      606 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/Makefile
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.511985 draco-ml-0.2.1.dev1/docs/advanced_usage/
+-rw-r--r--   0 sarah      (501) staff       (20)     2501 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/advanced_usage/concepts.md
+-rw-r--r--   0 sarah      (501) staff       (20)     2537 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/advanced_usage/csv.md
+-rw-r--r--   0 sarah      (501) staff       (20)     3532 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/advanced_usage/docker.md
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/authors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5886 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/conf.py
+-rw-r--r--   0 sarah      (501) staff       (20)       33 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.514289 draco-ml-0.2.1.dev1/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)     7263 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/images/Draco-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)    27132 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/images/Draco.png
+-rw-r--r--   0 sarah      (501) staff       (20)   886153 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/images/dai-logo.png
+-rw-r--r--   0 sarah      (501) staff       (20)      541 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      767 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/make.bat
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/docs/readme.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.523566 draco-ml-0.2.1.dev1/draco/
+-rw-r--r--   0 sarah      (501) staff       (20)      517 2023-07-31 14:33:58.000000 draco-ml-0.2.1.dev1/draco/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    36486 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/benchmark.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2103 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/db.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2922 2023-07-20 22:13:55.000000 draco-ml-0.2.1.dev1/draco/demo.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.524638 draco-ml-0.2.1.dev1/draco/loaders/
+-rw-r--r--   0 sarah      (501) staff       (20)       72 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/loaders/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8858 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/loaders/csv.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2768 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/metrics.py
+-rw-r--r--   0 sarah      (501) staff       (20)    23386 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.500582 draco-ml-0.2.1.dev1/draco/pipelines/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.526449 draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/
+-rw-r--r--   0 sarah      (501) staff       (20)     2516 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2716 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm_prob.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3502 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3302 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm_with_unstack.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.526866 draco-ml-0.2.1.dev1/draco/pipelines/dummy/
+-rw-r--r--   0 sarah      (501) staff       (20)      166 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/dummy/dummy.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.529116 draco-ml-0.2.1.dev1/draco/pipelines/lstm/
+-rw-r--r--   0 sarah      (501) staff       (20)     2504 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2704 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm_prob.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3490 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm_prob_with_unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3290 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm_with_unstack.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.530251 draco-ml-0.2.1.dev1/draco/pipelines/lstm_regressor/
+-rw-r--r--   0 sarah      (501) staff       (20)     2502 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/lstm_regressor/lstm_regressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3286 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.531738 draco-ml-0.2.1.dev1/draco/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)      862 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/primitives/mlblocks.MLPipeline.json
+-rw-r--r--   0 sarah      (501) staff       (20)      918 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/primitives/numpy.take.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2232 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/primitives/xgboost.XGBClassifier:probabilities.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3852 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/results.py
+-rw-r--r--   0 sarah      (501) staff       (20)     6143 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/targets.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1682 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/draco/utils.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.534169 draco-ml-0.2.1.dev1/draco_ml.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    14665 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     1523 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       87 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      833 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        6 2023-07-31 14:34:14.000000 draco-ml-0.2.1.dev1/draco_ml.egg-info/top_level.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1023 2023-07-31 14:34:14.537095 draco-ml-0.2.1.dev1/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     2999 2023-07-31 14:33:58.000000 draco-ml-0.2.1.dev1/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-07-31 14:34:14.535727 draco-ml-0.2.1.dev1/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)     1860 2023-04-13 20:29:53.000000 draco-ml-0.2.1.dev1/tests/test_benchmark.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1218 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev1/tests/test_metrics.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2547 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev1/tests/test_pipeline.py
```

### Comparing `draco-ml-0.2.1.dev0/CONTRIBUTING.rst` & `draco-ml-0.2.1.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/HISTORY.md` & `draco-ml-0.2.1.dev1/HISTORY.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # History
 
+## 0.3.0 - 2022-07-20
+
+This release switches from ``MLPrimitives`` to ``ml-stars``.
+Moreover, we remove all pipelines using deep feature synthesis.
+
+* Update demo bucket - [Issue #76](https://github.com/sintel-dev/Draco/issues/76) by @sarahmish
+* Remove ``dfs`` based pipelines - [Issue #73](https://github.com/sintel-dev/Draco/issues/73) by @sarahmish
+* Move from ``MLPrimitives`` to ``ml-stars`` - [Issue #72](https://github.com/sintel-dev/Draco/issues/72) by @sarahmish
+
 
 ## 0.2.0 - 2022-04-12
 
 This release features a reorganization and renaming of ``Draco`` pipelines. In addtion,
 we update some of the dependencies for general housekeeping.
 
 * Update Draco dependencies - [Issue #66](https://github.com/signals-dev/Draco/issues/66) by @sarahmish
```

### Comparing `draco-ml-0.2.1.dev0/LICENSE` & `draco-ml-0.2.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/PKG-INFO` & `draco-ml-0.2.1.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draco-ml
-Version: 0.2.1.dev0
+Version: 0.2.1.dev1
 Summary: AutoML for Time Series.
 Home-page: https://github.com/sintel-dev/Draco
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: wind machine learning draco
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -305,14 +305,23 @@
 [project documentation site](https://sintel-dev.github.io/Draco/)
 Also do not forget to have a look at the [tutorials](
 https://github.com/sintel-dev/Draco/tree/master/tutorials)!
 
 
 # History
 
+## 0.3.0 - 2022-07-20
+
+This release switches from ``MLPrimitives`` to ``ml-stars``.
+Moreover, we remove all pipelines using deep feature synthesis.
+
+* Update demo bucket - [Issue #76](https://github.com/sintel-dev/Draco/issues/76) by @sarahmish
+* Remove ``dfs`` based pipelines - [Issue #73](https://github.com/sintel-dev/Draco/issues/73) by @sarahmish
+* Move from ``MLPrimitives`` to ``ml-stars`` - [Issue #72](https://github.com/sintel-dev/Draco/issues/72) by @sarahmish
+
 
 ## 0.2.0 - 2022-04-12
 
 This release features a reorganization and renaming of ``Draco`` pipelines. In addtion,
 we update some of the dependencies for general housekeeping.
 
 * Update Draco dependencies - [Issue #66](https://github.com/signals-dev/Draco/issues/66) by @sarahmish
```

### Comparing `draco-ml-0.2.1.dev0/README.md` & `draco-ml-0.2.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/Makefile` & `draco-ml-0.2.1.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/advanced_usage/concepts.md` & `draco-ml-0.2.1.dev1/docs/advanced_usage/concepts.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/advanced_usage/csv.md` & `draco-ml-0.2.1.dev1/docs/advanced_usage/csv.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/advanced_usage/docker.md` & `draco-ml-0.2.1.dev1/docs/advanced_usage/docker.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/conf.py` & `draco-ml-0.2.1.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/images/Draco-200.png` & `draco-ml-0.2.1.dev1/docs/images/Draco-200.png`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/images/Draco.png` & `draco-ml-0.2.1.dev1/docs/images/Draco.png`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/images/dai-logo.png` & `draco-ml-0.2.1.dev1/docs/images/dai-logo.png`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/index.rst` & `draco-ml-0.2.1.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/docs/make.bat` & `draco-ml-0.2.1.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/__init__.py` & `draco-ml-0.2.1.dev1/draco/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Draco."""
 
 __author__ = """MIT Data To AI Lab"""
 __email__ = 'dailabmit@gmail.com'
-__version__ = '0.2.1.dev0'
+__version__ = '0.2.1.dev1'
 
 import os
 
 from draco.pipeline import DracoPipeline, get_pipelines
 
 _BASE_PATH = os.path.abspath(os.path.dirname(__file__))
 MLBLOCKS_PRIMITIVES = os.path.join(_BASE_PATH, 'primitives')
```

### Comparing `draco-ml-0.2.1.dev0/draco/benchmark.py` & `draco-ml-0.2.1.dev1/draco/benchmark.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/db.py` & `draco-ml-0.2.1.dev1/draco/db.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/demo.py` & `draco-ml-0.2.1.dev1/draco/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 
 import pandas as pd
 
 LOGGER = logging.getLogger(__name__)
 
-S3_URL = 'https://d3-ai-greenguard.s3.amazonaws.com/'
+S3_URL = 'https://sintel-draco.s3.amazonaws.com/'
 DEMO_PATH = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'demo')
 
 _FILES = {
     'DEFAULT': [
         ('target_times', 'cutoff_time'),
         ('readings', 'timestamp')
     ],
@@ -42,15 +42,15 @@
     """Load the demo included in the Draco project.
 
     The first time that this function is executed, the data will be downloaded
     and cached inside the `draco/demo` folder.
     Subsequent calls will load the cached data instead of downloading it again.
     
     Args:
-        rul (str):
+        name (str):
             Name of the dataset to load. If "RUL", load NASA's CMAPSS dataset
             https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/#turbofan.
             If "default" then load default demo.
         load_readings (bool):
             Whether to load the ``readings`` table or not.
 
     Returns:
```

### Comparing `draco-ml-0.2.1.dev0/draco/loaders/csv.py` & `draco-ml-0.2.1.dev1/draco/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/metrics.py` & `draco-ml-0.2.1.dev1/draco/metrics.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipeline.py` & `draco-ml-0.2.1.dev1/draco/pipeline.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm.json` & `draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob.json` & `draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm_prob.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json` & `draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_with_unstack.json` & `draco-ml-0.2.1.dev1/draco/pipelines/double_lstm/double_lstm_with_unstack.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm.json` & `draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob.json` & `draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm_prob.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob_with_unstack.json` & `draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm_prob_with_unstack.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_with_unstack.json` & `draco-ml-0.2.1.dev1/draco/pipelines/lstm/lstm_with_unstack.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor.json` & `draco-ml-0.2.1.dev1/draco/pipelines/lstm_regressor/lstm_regressor.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json` & `draco-ml-0.2.1.dev1/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/primitives/mlblocks.MLPipeline.json` & `draco-ml-0.2.1.dev1/draco/primitives/mlblocks.MLPipeline.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/primitives/numpy.take.json` & `draco-ml-0.2.1.dev1/draco/primitives/numpy.take.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/primitives/xgboost.XGBClassifier:probabilities.json` & `draco-ml-0.2.1.dev1/draco/primitives/xgboost.XGBClassifier:probabilities.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/results.py` & `draco-ml-0.2.1.dev1/draco/results.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/targets.py` & `draco-ml-0.2.1.dev1/draco/targets.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco/utils.py` & `draco-ml-0.2.1.dev1/draco/utils.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco_ml.egg-info/PKG-INFO` & `draco-ml-0.2.1.dev1/draco_ml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draco-ml
-Version: 0.2.1.dev0
+Version: 0.2.1.dev1
 Summary: AutoML for Time Series.
 Home-page: https://github.com/sintel-dev/Draco
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: wind machine learning draco
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -305,14 +305,23 @@
 [project documentation site](https://sintel-dev.github.io/Draco/)
 Also do not forget to have a look at the [tutorials](
 https://github.com/sintel-dev/Draco/tree/master/tutorials)!
 
 
 # History
 
+## 0.3.0 - 2022-07-20
+
+This release switches from ``MLPrimitives`` to ``ml-stars``.
+Moreover, we remove all pipelines using deep feature synthesis.
+
+* Update demo bucket - [Issue #76](https://github.com/sintel-dev/Draco/issues/76) by @sarahmish
+* Remove ``dfs`` based pipelines - [Issue #73](https://github.com/sintel-dev/Draco/issues/73) by @sarahmish
+* Move from ``MLPrimitives`` to ``ml-stars`` - [Issue #72](https://github.com/sintel-dev/Draco/issues/72) by @sarahmish
+
 
 ## 0.2.0 - 2022-04-12
 
 This release features a reorganization and renaming of ``Draco`` pipelines. In addtion,
 we update some of the dependencies for general housekeeping.
 
 * Update Draco dependencies - [Issue #66](https://github.com/signals-dev/Draco/issues/66) by @sarahmish
```

### Comparing `draco-ml-0.2.1.dev0/draco_ml.egg-info/SOURCES.txt` & `draco-ml-0.2.1.dev1/draco_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/draco_ml.egg-info/requires.txt` & `draco-ml-0.2.1.dev1/draco_ml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/setup.cfg` & `draco-ml-0.2.1.dev1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1.dev0
+current_version = 0.2.1.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `draco-ml-0.2.1.dev0/setup.py` & `draco-ml-0.2.1.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,10 +114,10 @@
     name='draco-ml',
     packages=find_packages(include=['draco', 'draco.*']),
     python_requires='>=3.6,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/Draco',
-    version='0.2.1.dev0',
+    version='0.2.1.dev1',
     zip_safe=False,
 )
```

### Comparing `draco-ml-0.2.1.dev0/tests/test_benchmark.py` & `draco-ml-0.2.1.dev1/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/tests/test_metrics.py` & `draco-ml-0.2.1.dev1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.1.dev0/tests/test_pipeline.py` & `draco-ml-0.2.1.dev1/tests/test_pipeline.py`

 * *Files identical despite different names*

