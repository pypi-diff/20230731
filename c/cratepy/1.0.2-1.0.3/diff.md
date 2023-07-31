# Comparing `tmp/cratepy-1.0.2.tar.gz` & `tmp/cratepy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cratepy-1.0.2.tar", last modified: Mon May 15 22:52:03 2023, max compression
+gzip compressed data, was "cratepy-1.0.3.tar", last modified: Mon Jul 31 13:38:01 2023, max compression
```

## Comparing `cratepy-1.0.2.tar` & `cratepy-1.0.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     1525 2023-05-15 14:55:44.000000 cratepy-1.0.2/LICENSE
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)       75 2023-05-15 14:55:44.000000 cratepy-1.0.2/MANIFEST.in
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     4665 2023-05-15 22:52:03.751179 cratepy-1.0.2/PKG-INFO
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     3851 2023-05-15 22:46:57.000000 cratepy-1.0.2/README.md
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)        6 2023-05-15 22:50:56.000000 cratepy-1.0.2/VERSION
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)       81 2023-05-15 14:55:44.000000 cratepy-1.0.2/pyproject.toml
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      134 2023-05-15 14:55:44.000000 cratepy-1.0.2/requirements.txt
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     1014 2023-05-15 22:52:03.755180 cratepy-1.0.2/setup.cfg
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     1508 2023-05-15 21:34:05.000000 cratepy-1.0.2/src/cratepy/__init__.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/clustering/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      506 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/__init__.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/clustering/adaptivity/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      307 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/adaptivity/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    54156 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/adaptivity/adaptivity_criterion.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    70161 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/adaptivity/crve_adaptivity.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    21769 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/citoperations.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    21321 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/clusteringalgs.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    50314 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/clusteringdata.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    71591 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/clusteringphase.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    79595 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/crve.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    15200 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/rveelasticdatabase.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/clustering/solution/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      304 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/solution/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     3656 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/solution/dnshomogenization.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)   109156 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/clustering/solution/ffthombasicscheme.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/ioput/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      443 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    13734 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/fileoperations.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      375 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6785 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/efftanoutput.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    10333 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/homresoutput.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     2603 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/interface.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    13944 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/refmatoutput.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    28041 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/info.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     8292 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/ioutilities.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/ioput/miscoutputfiles/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      287 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/miscoutputfiles/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    18581 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/miscoutputfiles/voxelsoutput.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    55868 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/miscoutputfiles/vtkoutput.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    19728 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/packager.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    25603 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/readinputdata.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)   115426 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/ioput/readprocedures.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    21452 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/main.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/material/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      344 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    13038 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/isotropichardlaw.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    63443 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/materialmodeling.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    22472 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/materialoperations.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/material/models/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      357 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/models/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    31841 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/models/elastic.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6340 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/models/interface.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    17406 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/models/stvenant_kirchhoff.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    23770 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/material/models/von_mises.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/online/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      270 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/online/__init__.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/online/crom/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      236 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/online/crom/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)   183505 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/online/crom/asca.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/online/loading/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      246 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/online/loading/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    68287 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/online/loading/macloadincrem.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/optimization/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      301 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/optimization/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    17001 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/optimization/optimizationfunction.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6066 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/optimization/optimizer.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy/tensor/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      287 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/tensor/__init__.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    25806 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/tensor/matrixoperations.py
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    30124 2023-05-15 14:55:44.000000 cratepy-1.0.2/src/cratepy/tensor/tensoroperations.py
-drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-05-15 22:52:03.751179 cratepy-1.0.2/src/cratepy.egg-info/
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     4665 2023-05-15 22:52:03.000000 cratepy-1.0.2/src/cratepy.egg-info/PKG-INFO
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     2270 2023-05-15 22:52:03.000000 cratepy-1.0.2/src/cratepy.egg-info/SOURCES.txt
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)        1 2023-05-15 22:52:03.000000 cratepy-1.0.2/src/cratepy.egg-info/dependency_links.txt
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      134 2023-05-15 22:52:03.000000 cratepy-1.0.2/src/cratepy.egg-info/requires.txt
--rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)        8 2023-05-15 22:52:03.000000 cratepy-1.0.2/src/cratepy.egg-info/top_level.txt
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     1525 2023-05-15 14:55:44.000000 cratepy-1.0.3/LICENSE
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)       75 2023-05-15 14:55:44.000000 cratepy-1.0.3/MANIFEST.in
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6917 2023-07-31 13:38:01.810375 cratepy-1.0.3/PKG-INFO
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6109 2023-07-17 19:22:53.000000 cratepy-1.0.3/README.md
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)        6 2023-07-31 13:13:07.000000 cratepy-1.0.3/VERSION
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)       81 2023-05-15 14:55:44.000000 cratepy-1.0.3/pyproject.toml
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      134 2023-05-15 14:55:44.000000 cratepy-1.0.3/requirements.txt
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     1008 2023-07-31 13:38:01.810375 cratepy-1.0.3/setup.cfg
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.806375 cratepy-1.0.3/src/
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.806375 cratepy-1.0.3/src/cratepy/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     1508 2023-05-15 21:34:05.000000 cratepy-1.0.3/src/cratepy/__init__.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.806375 cratepy-1.0.3/src/cratepy/clustering/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      506 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/__init__.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.806375 cratepy-1.0.3/src/cratepy/clustering/adaptivity/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      307 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/adaptivity/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    54156 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/adaptivity/adaptivity_criterion.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    70161 2023-07-06 21:43:41.000000 cratepy-1.0.3/src/cratepy/clustering/adaptivity/crve_adaptivity.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    21769 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/citoperations.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    21321 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/clusteringalgs.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    50314 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/clusteringdata.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    71591 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/clusteringphase.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    79595 2023-07-03 19:20:49.000000 cratepy-1.0.3/src/cratepy/clustering/crve.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    15200 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/rveelasticdatabase.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.806375 cratepy-1.0.3/src/cratepy/clustering/solution/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      304 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/solution/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     3656 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/solution/dnshomogenization.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)   109156 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/clustering/solution/ffthombasicscheme.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/ioput/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      443 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    13734 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/fileoperations.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      375 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6785 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/efftanoutput.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    10333 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/homresoutput.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     2603 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/interface.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    13944 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/refmatoutput.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    28041 2023-07-31 13:13:10.000000 cratepy-1.0.3/src/cratepy/ioput/info.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     8310 2023-07-17 18:50:24.000000 cratepy-1.0.3/src/cratepy/ioput/ioutilities.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/ioput/miscoutputfiles/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      287 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/miscoutputfiles/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    18581 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/miscoutputfiles/voxelsoutput.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    55868 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/miscoutputfiles/vtkoutput.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    19728 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/packager.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    25603 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/readinputdata.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)   115426 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/ioput/readprocedures.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    21452 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/main.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/material/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      344 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    13038 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/isotropichardlaw.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    63443 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/materialmodeling.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    22472 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/materialoperations.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/material/models/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      357 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/models/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    31841 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/models/elastic.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6340 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/models/interface.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    17406 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/models/stvenant_kirchhoff.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    23770 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/material/models/von_mises.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/online/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      270 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/online/__init__.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/online/crom/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      236 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/online/crom/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)   183505 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/online/crom/asca.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/online/loading/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      246 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/online/loading/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    68287 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/online/loading/macloadincrem.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/optimization/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      301 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/optimization/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    17001 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/optimization/optimizationfunction.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6066 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/optimization/optimizer.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.810375 cratepy-1.0.3/src/cratepy/tensor/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      287 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/tensor/__init__.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    25806 2023-05-15 14:55:44.000000 cratepy-1.0.3/src/cratepy/tensor/matrixoperations.py
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)    30055 2023-07-31 13:20:27.000000 cratepy-1.0.3/src/cratepy/tensor/tensoroperations.py
+drwxrwxr-x   0 bernardoferreira  (1000) bernardoferreira  (1000)        0 2023-07-31 13:38:01.806375 cratepy-1.0.3/src/cratepy.egg-info/
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     6917 2023-07-31 13:38:01.000000 cratepy-1.0.3/src/cratepy.egg-info/PKG-INFO
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)     2270 2023-07-31 13:38:01.000000 cratepy-1.0.3/src/cratepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)        1 2023-07-31 13:38:01.000000 cratepy-1.0.3/src/cratepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)      134 2023-07-31 13:38:01.000000 cratepy-1.0.3/src/cratepy.egg-info/requires.txt
+-rw-rw-r--   0 bernardoferreira  (1000) bernardoferreira  (1000)        8 2023-07-31 13:38:01.000000 cratepy-1.0.3/src/cratepy.egg-info/top_level.txt
```

### Comparing `cratepy-1.0.2/LICENSE` & `cratepy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/setup.cfg` & `cratepy-1.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = file: VERSION
 author = Bernardo Ferreira
 author_email = bernardoferreiraacc@gmail.com
 description = CRATE: Clustering-based Nonlinear Analysis of Materials
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = simulation, clustering, materials, homogenization, modeling
-url = https://github.com/BernardoFerreira/CRATE
+url = https://github.com/bessagroup/CRATE
 license = BSD-3-Clause License
 license_files = file: LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -21,15 +21,15 @@
 	Programming Language :: Python :: 3
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = file: requirements.txt
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `cratepy-1.0.2/src/cratepy/__init__.py` & `cratepy-1.0.3/src/cratepy/__init__.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/adaptivity/adaptivity_criterion.py` & `cratepy-1.0.3/src/cratepy/clustering/adaptivity/adaptivity_criterion.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/adaptivity/crve_adaptivity.py` & `cratepy-1.0.3/src/cratepy/clustering/adaptivity/crve_adaptivity.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/citoperations.py` & `cratepy-1.0.3/src/cratepy/clustering/citoperations.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/clusteringalgs.py` & `cratepy-1.0.3/src/cratepy/clustering/clusteringalgs.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/clusteringdata.py` & `cratepy-1.0.3/src/cratepy/clustering/clusteringdata.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/clusteringphase.py` & `cratepy-1.0.3/src/cratepy/clustering/clusteringphase.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/crve.py` & `cratepy-1.0.3/src/cratepy/clustering/crve.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/rveelasticdatabase.py` & `cratepy-1.0.3/src/cratepy/clustering/rveelasticdatabase.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/solution/dnshomogenization.py` & `cratepy-1.0.3/src/cratepy/clustering/solution/dnshomogenization.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/clustering/solution/ffthombasicscheme.py` & `cratepy-1.0.3/src/cratepy/clustering/solution/ffthombasicscheme.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/fileoperations.py` & `cratepy-1.0.3/src/cratepy/ioput/fileoperations.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/efftanoutput.py` & `cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/efftanoutput.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/homresoutput.py` & `cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/homresoutput.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/interface.py` & `cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/interface.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/incoutputfiles/refmatoutput.py` & `cratepy-1.0.3/src/cratepy/ioput/incoutputfiles/refmatoutput.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/info.py` & `cratepy-1.0.3/src/cratepy/ioput/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             ioutil.print2('Please rerun the program and provide a different '
                           'problem name.' + '\n')
             sys.exit(1)
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     elif code == '0':
         arguments = \
             ['CRATE - Clustering-based Nonlinear Analysis of Materials',
-             'Created by Bernardo P. Ferreira', 'Release 1.0.0 (Jun 2023)'] \
+             'Created by Bernardo P. Ferreira', 'Release 1.0.3 (Jul 2023)'] \
             + 2*[args[0], ] + list(args[1:3])
         info = tuple(arguments)
         template = '\n' + colorama.Fore.WHITE + tilde_line \
                    + colorama.Style.RESET_ALL \
                    + colorama.Fore.WHITE + '\n{:^{width}}\n\n' \
                    + '{:^{width}}\n' + '\n{:^{width}}\n\n' \
                    + colorama.Fore.YELLOW + 'Problem under analysis: ' \
```

### Comparing `cratepy-1.0.2/src/cratepy/ioput/ioutilities.py` & `cratepy-1.0.3/src/cratepy/ioput/ioutilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         Objects to print.
     """
     # Print to default sys.stdout
     print(*objects)
     # Print to '.screen' file
     global screen_file_path
     if screen_file_path is not None:
-        screen_file = open(screen_file_path, 'a')
+        screen_file = open(screen_file_path, 'a', encoding='utf-8')
         objects_esc = list()
         for i in range(len(objects)):
             objects_esc.append(escapeANSI(objects[i]))
         print(*objects_esc, file=screen_file)
         screen_file.close()
 # =============================================================================
 def setdisplayfeatures():
```

### Comparing `cratepy-1.0.2/src/cratepy/ioput/miscoutputfiles/voxelsoutput.py` & `cratepy-1.0.3/src/cratepy/ioput/miscoutputfiles/voxelsoutput.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/miscoutputfiles/vtkoutput.py` & `cratepy-1.0.3/src/cratepy/ioput/miscoutputfiles/vtkoutput.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/packager.py` & `cratepy-1.0.3/src/cratepy/ioput/packager.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/readinputdata.py` & `cratepy-1.0.3/src/cratepy/ioput/readinputdata.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/ioput/readprocedures.py` & `cratepy-1.0.3/src/cratepy/ioput/readprocedures.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/main.py` & `cratepy-1.0.3/src/cratepy/main.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/isotropichardlaw.py` & `cratepy-1.0.3/src/cratepy/material/isotropichardlaw.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/materialmodeling.py` & `cratepy-1.0.3/src/cratepy/material/materialmodeling.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/materialoperations.py` & `cratepy-1.0.3/src/cratepy/material/materialoperations.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/models/elastic.py` & `cratepy-1.0.3/src/cratepy/material/models/elastic.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/models/interface.py` & `cratepy-1.0.3/src/cratepy/material/models/interface.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/models/stvenant_kirchhoff.py` & `cratepy-1.0.3/src/cratepy/material/models/stvenant_kirchhoff.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/material/models/von_mises.py` & `cratepy-1.0.3/src/cratepy/material/models/von_mises.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/online/crom/asca.py` & `cratepy-1.0.3/src/cratepy/online/crom/asca.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/online/loading/macloadincrem.py` & `cratepy-1.0.3/src/cratepy/online/loading/macloadincrem.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/optimization/optimizationfunction.py` & `cratepy-1.0.3/src/cratepy/optimization/optimizationfunction.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/optimization/optimizer.py` & `cratepy-1.0.3/src/cratepy/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/tensor/matrixoperations.py` & `cratepy-1.0.3/src/cratepy/tensor/matrixoperations.py`

 * *Files identical despite different names*

### Comparing `cratepy-1.0.2/src/cratepy/tensor/tensoroperations.py` & `cratepy-1.0.3/src/cratepy/tensor/tensoroperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,15 @@
     else:
         raise RuntimeError('The rotation tensor is not available for '
                            + 'tensor order greater than 4.')
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     # Return
     return rtensor
 # =============================================================================
-def rotation_tensor_from_euler_angles(n_dim, euler_deg):
+def rotation_tensor_from_euler_angles(euler_deg):
     """Set rotation tensor from Euler angles (Bunge convention).
 
     The rotation tensor is defined as
 
     .. math::
 
        \\mathbf{R} =
@@ -704,16 +704,14 @@
     and :math:`(\\alpha, \\beta, \\gamma)` are the Euler angles corresponding
     to the Bunge convention (Z1-X2-Z3).
 
     ----
 
     Parameters
     ----------
-    n_dim : int
-        Number of spatial dimensions.
     euler_deg : tuple
         Euler angles (degrees) sorted according to Bunge convention (Z1-X2-Z3).
 
     Returns
     -------
     r : numpy.ndarray (2d)
         Rotation tensor (for given rotation angle theta, active transformation
@@ -726,15 +724,15 @@
     s2 = np.sin(euler_rad[1])
     s3 = np.sin(euler_rad[2])
     c1 = np.cos(euler_rad[0])
     c2 = np.cos(euler_rad[1])
     c3 = np.cos(euler_rad[2])
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     # Initialize rotation tensor
-    r = np.zeros((n_dim, n_dim))
+    r = np.zeros((3, 3))
     # Build rotation tensor
     r[0, 0] = c1*c3 - c2*s1*s3
     r[1, 0] = c3*s1 + c1*c2*s3
     r[2, 0] = s2*s3
     r[0, 1] = -c1*s3 - c2*c3*s1
     r[1, 1] = c1*c2*c3 - s1*s3
     r[2, 1] = c3*s2
```

### Comparing `cratepy-1.0.2/src/cratepy.egg-info/SOURCES.txt` & `cratepy-1.0.3/src/cratepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

