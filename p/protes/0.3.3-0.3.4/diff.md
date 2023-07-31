# Comparing `tmp/protes-0.3.3.tar.gz` & `tmp/protes-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protes-0.3.3.tar", last modified: Tue Jul 25 14:48:31 2023, max compression
+gzip compressed data, was "protes-0.3.4.tar", last modified: Mon Jul 31 12:52:55 2023, max compression
```

## Comparing `protes-0.3.3.tar` & `protes-0.3.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.910621 protes-0.3.3/
--rw-r--r--   0 andrei     (501) staff       (20)      118 2023-07-25 11:52:11.000000 protes-0.3.3/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     9793 2023-07-25 14:48:31.909955 protes-0.3.3/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     8555 2023-07-25 14:48:12.000000 protes-0.3.3/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.879732 protes-0.3.3/calc/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-07-14 14:53:51.000000 protes-0.3.3/calc/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)     7201 2023-05-17 19:07:28.000000 protes-0.3.3/calc/calc.py
--rw-r--r--   0 andrei     (501) staff       (20)     1716 2023-07-25 13:56:59.000000 protes-0.3.3/calc/calc_one.py
--rw-r--r--   0 andrei     (501) staff       (20)     1429 2023-05-16 21:18:20.000000 protes-0.3.3/calc/constr.py
--rw-r--r--   0 andrei     (501) staff       (20)    25285 2023-05-15 20:02:07.000000 protes-0.3.3/calc/construct_TT.py
--rw-r--r--   0 andrei     (501) staff       (20)   212397 2023-05-17 19:07:32.000000 protes-0.3.3/calc/deps.png
--rw-r--r--   0 andrei     (501) staff       (20)    23388 2023-06-13 07:47:54.000000 protes-0.3.3/calc/log.txt
--rw-r--r--   0 andrei     (501) staff       (20)     6927 2023-07-25 13:56:59.000000 protes-0.3.3/calc/log_one.txt
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.886166 protes-0.3.3/calc/opti/
--rw-r--r--   0 andrei     (501) staff       (20)      295 2023-05-14 21:16:31.000000 protes-0.3.3/calc/opti/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.891141 protes-0.3.3/calc/opti/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)      527 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3929 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)      999 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_nb.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_opo.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1378 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1039 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1476 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_protes.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)      997 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_pso.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:25.000000 protes-0.3.3/calc/opti/__pycache__/opti_spsa.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1478 2023-05-17 14:35:25.000000 protes-0.3.3/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3667 2023-05-15 17:29:36.000000 protes-0.3.3/calc/opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      452 2023-05-14 21:10:44.000000 protes-0.3.3/calc/opti/opti_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      453 2023-05-14 21:10:36.000000 protes-0.3.3/calc/opti/opti_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)      763 2023-05-16 22:11:55.000000 protes-0.3.3/calc/opti/opti_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      464 2023-05-14 21:10:27.000000 protes-0.3.3/calc/opti/opti_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)      923 2023-05-17 14:32:54.000000 protes-0.3.3/calc/opti/opti_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      446 2023-05-14 21:10:16.000000 protes-0.3.3/calc/opti/opti_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      449 2023-05-14 21:09:27.000000 protes-0.3.3/calc/opti/opti_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1042 2023-05-16 22:11:42.000000 protes-0.3.3/calc/opti/opti_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)    42609 2023-06-13 07:47:54.000000 protes-0.3.3/calc/res.pickle
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.898066 protes-0.3.3/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:44.000000 protes-0.3.3/demo/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)   342526 2023-05-18 12:20:34.000000 protes-0.3.3/demo/check_ackley.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)   536657 2023-05-18 11:46:30.000000 protes-0.3.3/demo/check_knapsack.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     2512 2023-07-25 14:47:04.000000 protes-0.3.3/demo/demo_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     2738 2023-07-25 14:47:29.000000 protes-0.3.3/demo/demo_qubo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.903964 protes-0.3.3/demo/figures/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:49.000000 protes-0.3.3/demo/figures/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)   137856 2023-05-18 12:01:07.000000 protes-0.3.3/demo/figures/check_ackley.png
--rw-r--r--   0 andrei     (501) staff       (20)    99993 2023-05-18 12:20:12.000000 protes-0.3.3/demo/figures/check_ackley_ext.png
--rw-r--r--   0 andrei     (501) staff       (20)   202943 2023-05-17 15:13:23.000000 protes-0.3.3/demo/figures/check_knapsack.png
--rw-r--r--   0 andrei     (501) staff       (20)   180807 2023-05-18 11:44:44.000000 protes-0.3.3/demo/figures/check_knapsack_ext.png
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.907246 protes-0.3.3/protes/
--rw-r--r--   0 andrei     (501) staff       (20)      127 2023-07-25 14:48:06.000000 protes-0.3.3/protes/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.3/protes/animation.py
--rw-r--r--   0 andrei     (501) staff       (20)     5962 2023-07-25 14:29:04.000000 protes-0.3.3/protes/protes.py
--rw-r--r--   0 andrei     (501) staff       (20)     5450 2023-07-25 14:29:03.000000 protes-0.3.3/protes/protes_general.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.909246 protes-0.3.3/protes.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     9793 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1400 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      189 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        7 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/top_level.txt
--rw-r--r--   0 andrei     (501) staff       (20)      243 2023-07-25 13:10:12.000000 protes-0.3.3/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      118 2023-05-15 20:03:14.000000 protes-0.3.3/requirements_calc.txt
--rw-r--r--   0 andrei     (501) staff       (20)       38 2023-07-25 14:48:31.910780 protes-0.3.3/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2467 2023-05-19 10:43:02.000000 protes-0.3.3/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.972177 protes-0.3.4/
+-rw-r--r--   0 andrei     (501) staff       (20)      118 2023-07-25 11:52:11.000000 protes-0.3.4/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     9793 2023-07-31 12:52:55.971413 protes-0.3.4/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     8555 2023-07-31 12:52:13.000000 protes-0.3.4/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.935503 protes-0.3.4/calc/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-07-14 14:53:51.000000 protes-0.3.4/calc/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)     7201 2023-05-17 19:07:28.000000 protes-0.3.4/calc/calc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1716 2023-07-25 13:56:59.000000 protes-0.3.4/calc/calc_one.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1429 2023-05-16 21:18:20.000000 protes-0.3.4/calc/constr.py
+-rw-r--r--   0 andrei     (501) staff       (20)    25285 2023-05-15 20:02:07.000000 protes-0.3.4/calc/construct_TT.py
+-rw-r--r--   0 andrei     (501) staff       (20)   212397 2023-05-17 19:07:32.000000 protes-0.3.4/calc/deps.png
+-rw-r--r--   0 andrei     (501) staff       (20)    23388 2023-06-13 07:47:54.000000 protes-0.3.4/calc/log.txt
+-rw-r--r--   0 andrei     (501) staff       (20)     6927 2023-07-31 12:52:26.000000 protes-0.3.4/calc/log_one.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.941065 protes-0.3.4/calc/opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      295 2023-05-14 21:16:31.000000 protes-0.3.4/calc/opti/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.944430 protes-0.3.4/calc/opti/__pycache__/
+-rw-r--r--   0 andrei     (501) staff       (20)      527 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     3929 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)      999 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti_nb.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti_opo.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1378 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1039 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1476 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti_protes.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)      997 2023-05-17 14:35:24.000000 protes-0.3.4/calc/opti/__pycache__/opti_pso.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:25.000000 protes-0.3.4/calc/opti/__pycache__/opti_spsa.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1478 2023-05-17 14:35:25.000000 protes-0.3.4/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     3667 2023-05-15 17:29:36.000000 protes-0.3.4/calc/opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      452 2023-05-14 21:10:44.000000 protes-0.3.4/calc/opti/opti_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      453 2023-05-14 21:10:36.000000 protes-0.3.4/calc/opti/opti_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      763 2023-05-16 22:11:55.000000 protes-0.3.4/calc/opti/opti_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      464 2023-05-14 21:10:27.000000 protes-0.3.4/calc/opti/opti_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)      923 2023-05-17 14:32:54.000000 protes-0.3.4/calc/opti/opti_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      446 2023-05-14 21:10:16.000000 protes-0.3.4/calc/opti/opti_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      449 2023-05-14 21:09:27.000000 protes-0.3.4/calc/opti/opti_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1042 2023-05-16 22:11:42.000000 protes-0.3.4/calc/opti/opti_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)    42609 2023-06-13 07:47:54.000000 protes-0.3.4/calc/res.pickle
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.951933 protes-0.3.4/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:44.000000 protes-0.3.4/demo/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)   342526 2023-05-18 12:20:34.000000 protes-0.3.4/demo/check_ackley.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)   536657 2023-05-18 11:46:30.000000 protes-0.3.4/demo/check_knapsack.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     2512 2023-07-25 14:47:04.000000 protes-0.3.4/demo/demo_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2738 2023-07-25 14:47:29.000000 protes-0.3.4/demo/demo_qubo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.960839 protes-0.3.4/demo/figures/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:49.000000 protes-0.3.4/demo/figures/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)   137856 2023-05-18 12:01:07.000000 protes-0.3.4/demo/figures/check_ackley.png
+-rw-r--r--   0 andrei     (501) staff       (20)    99993 2023-05-18 12:20:12.000000 protes-0.3.4/demo/figures/check_ackley_ext.png
+-rw-r--r--   0 andrei     (501) staff       (20)   202943 2023-05-17 15:13:23.000000 protes-0.3.4/demo/figures/check_knapsack.png
+-rw-r--r--   0 andrei     (501) staff       (20)   180807 2023-05-18 11:44:44.000000 protes-0.3.4/demo/figures/check_knapsack_ext.png
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.966731 protes-0.3.4/protes/
+-rw-r--r--   0 andrei     (501) staff       (20)      127 2023-07-31 12:52:09.000000 protes-0.3.4/protes/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.4/protes/animation.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5962 2023-07-25 14:29:04.000000 protes-0.3.4/protes/protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5450 2023-07-25 14:29:03.000000 protes-0.3.4/protes/protes_general.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 12:52:55.970387 protes-0.3.4/protes.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     9793 2023-07-31 12:52:55.000000 protes-0.3.4/protes.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1400 2023-07-31 12:52:55.000000 protes-0.3.4/protes.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-31 12:52:55.000000 protes-0.3.4/protes.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      228 2023-07-31 12:52:55.000000 protes-0.3.4/protes.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        7 2023-07-31 12:52:55.000000 protes-0.3.4/protes.egg-info/top_level.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      370 2023-07-31 12:41:40.000000 protes-0.3.4/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      118 2023-05-15 20:03:14.000000 protes-0.3.4/requirements_calc.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       38 2023-07-31 12:52:55.972377 protes-0.3.4/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2467 2023-05-19 10:43:02.000000 protes-0.3.4/setup.py
```

### Comparing `protes-0.3.3/PKG-INFO` & `protes-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.3
+Version: 0.3.4
 Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,15 @@
 ## Description
 
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-> Current version "0.3.3".
+> Current version "0.3.4".
 
 To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip: `pip install protes`.
 
 > Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.4+), [scipy](https://github.com/scipy/scipy) (1.9+) and [seaborn](https://seaborn.pydata.org/) (0.12.2+) will be automatically installed during the installation of the main software product (see `requirements.txt` for more details). To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
 To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt` (please, note that the versions specified in this file are only suitable for `python 3.8`).
```

### Comparing `protes-0.3.3/README.md` & `protes-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-> Current version "0.3.3".
+> Current version "0.3.4".
 
 To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip: `pip install protes`.
 
 > Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.4+), [scipy](https://github.com/scipy/scipy) (1.9+) and [seaborn](https://seaborn.pydata.org/) (0.12.2+) will be automatically installed during the installation of the main software product (see `requirements.txt` for more details). To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
 To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt` (please, note that the versions specified in this file are only suitable for `python 3.8`).
```

### Comparing `protes-0.3.3/calc/.DS_Store` & `protes-0.3.4/calc/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/calc.py` & `protes-0.3.4/calc/calc.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/calc_one.py` & `protes-0.3.4/calc/calc_one.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/constr.py` & `protes-0.3.4/calc/constr.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/construct_TT.py` & `protes-0.3.4/calc/construct_TT.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/deps.png` & `protes-0.3.4/calc/deps.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/log.txt` & `protes-0.3.4/calc/log.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/log_one.txt` & `protes-0.3.4/calc/log_one.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/__init__.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_nb.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_nb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_opo.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_opo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_protes.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_protes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_pso.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_pso.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_spsa.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_spsa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc` & `protes-0.3.4/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/opti.py` & `protes-0.3.4/calc/opti/opti.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/opti_optimatt.py` & `protes-0.3.4/calc/opti/opti_optimatt.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/opti_protes.py` & `protes-0.3.4/calc/opti/opti_protes.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/opti/opti_ttopt.py` & `protes-0.3.4/calc/opti/opti_ttopt.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/calc/res.pickle` & `protes-0.3.4/calc/res.pickle`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/.DS_Store` & `protes-0.3.4/demo/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/check_ackley.ipynb` & `protes-0.3.4/demo/check_ackley.ipynb`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/check_knapsack.ipynb` & `protes-0.3.4/demo/check_knapsack.ipynb`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/demo_func.py` & `protes-0.3.4/demo/demo_func.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/demo_qubo.py` & `protes-0.3.4/demo/demo_qubo.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/figures/.DS_Store` & `protes-0.3.4/demo/figures/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/figures/check_ackley.png` & `protes-0.3.4/demo/figures/check_ackley.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/figures/check_ackley_ext.png` & `protes-0.3.4/demo/figures/check_ackley_ext.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/figures/check_knapsack.png` & `protes-0.3.4/demo/figures/check_knapsack.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/demo/figures/check_knapsack_ext.png` & `protes-0.3.4/demo/figures/check_knapsack_ext.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/protes/animation.py` & `protes-0.3.4/protes/animation.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/protes/protes.py` & `protes-0.3.4/protes/protes.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/protes/protes_general.py` & `protes-0.3.4/protes/protes_general.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/protes.egg-info/PKG-INFO` & `protes-0.3.4/protes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.3
+Version: 0.3.4
 Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,15 @@
 ## Description
 
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-> Current version "0.3.3".
+> Current version "0.3.4".
 
 To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip: `pip install protes`.
 
 > Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.4+), [scipy](https://github.com/scipy/scipy) (1.9+) and [seaborn](https://seaborn.pydata.org/) (0.12.2+) will be automatically installed during the installation of the main software product (see `requirements.txt` for more details). To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
 To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt` (please, note that the versions specified in this file are only suitable for `python 3.8`).
```

### Comparing `protes-0.3.3/protes.egg-info/SOURCES.txt` & `protes-0.3.4/protes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.3/setup.py` & `protes-0.3.4/setup.py`

 * *Files identical despite different names*

