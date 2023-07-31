# Comparing `tmp/BundesligaPredictor-0.0.5.tar.gz` & `tmp/BundesligaPredictor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BundesligaPredictor-0.0.5.tar", last modified: Mon Jul 31 12:41:46 2023, max compression
+gzip compressed data, was "BundesligaPredictor-0.0.6.tar", last modified: Mon Jul 31 13:06:53 2023, max compression
```

## Comparing `BundesligaPredictor-0.0.5.tar` & `BundesligaPredictor-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:41:46.594484 BundesligaPredictor-0.0.5/
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:41:46.589872 BundesligaPredictor-0.0.5/BundesligaPredictor.egg-info/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 12:41:46.000000 BundesligaPredictor-0.0.5/BundesligaPredictor.egg-info/PKG-INFO
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      483 2023-07-31 12:41:46.000000 BundesligaPredictor-0.0.5/BundesligaPredictor.egg-info/SOURCES.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        1 2023-07-31 12:41:46.000000 BundesligaPredictor-0.0.5/BundesligaPredictor.egg-info/dependency_links.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       54 2023-07-31 12:41:46.000000 BundesligaPredictor-0.0.5/BundesligaPredictor.egg-info/requires.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       14 2023-07-31 12:41:46.000000 BundesligaPredictor-0.0.5/BundesligaPredictor.egg-info/top_level.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 12:41:46.594187 BundesligaPredictor-0.0.5/PKG-INFO
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/README.md
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:41:46.591047 BundesligaPredictor-0.0.5/scripts/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/__init__.py
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:41:46.593152 BundesligaPredictor-0.0.5/scripts/data/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)  2545843 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/data/germany_all.csv
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)   154448 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/data/preprocessed.csv
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      101 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/load.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1987 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/preprocess.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1858 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/scraper.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      719 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/serve.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      344 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/test.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     2330 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/scripts/train.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       38 2023-07-31 12:41:46.594539 BundesligaPredictor-0.0.5/setup.cfg
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      394 2023-07-31 12:41:41.000000 BundesligaPredictor-0.0.5/setup.py
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:41:46.593817 BundesligaPredictor-0.0.5/tests/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/tests/__init__.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1471 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/tests/preprocess_test.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      427 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.5/tests/scraper_test.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 13:06:53.154049 BundesligaPredictor-0.0.6/
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 13:06:53.151660 BundesligaPredictor-0.0.6/BundesligaPredictor.egg-info/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 13:06:53.000000 BundesligaPredictor-0.0.6/BundesligaPredictor.egg-info/PKG-INFO
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      414 2023-07-31 13:06:53.000000 BundesligaPredictor-0.0.6/BundesligaPredictor.egg-info/SOURCES.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        1 2023-07-31 13:06:53.000000 BundesligaPredictor-0.0.6/BundesligaPredictor.egg-info/dependency_links.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       54 2023-07-31 13:06:53.000000 BundesligaPredictor-0.0.6/BundesligaPredictor.egg-info/requires.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       14 2023-07-31 13:06:53.000000 BundesligaPredictor-0.0.6/BundesligaPredictor.egg-info/top_level.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 13:06:53.153902 BundesligaPredictor-0.0.6/PKG-INFO
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 13:06:53.153071 BundesligaPredictor-0.0.6/scripts/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/__init__.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      101 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/load.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1987 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/preprocess.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1858 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/scraper.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      719 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/serve.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      344 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/test.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     2330 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/scripts/train.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       38 2023-07-31 13:06:53.154093 BundesligaPredictor-0.0.6/setup.cfg
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      394 2023-07-31 13:06:48.000000 BundesligaPredictor-0.0.6/setup.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 13:06:53.153560 BundesligaPredictor-0.0.6/tests/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/tests/__init__.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1471 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/tests/preprocess_test.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      427 2023-07-31 12:03:52.000000 BundesligaPredictor-0.0.6/tests/scraper_test.py
```

### Comparing `BundesligaPredictor-0.0.5/scripts/preprocess.py` & `BundesligaPredictor-0.0.6/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.5/scripts/scraper.py` & `BundesligaPredictor-0.0.6/scripts/scraper.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.5/scripts/serve.py` & `BundesligaPredictor-0.0.6/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.5/scripts/train.py` & `BundesligaPredictor-0.0.6/scripts/train.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.5/tests/preprocess_test.py` & `BundesligaPredictor-0.0.6/tests/preprocess_test.py`

 * *Files identical despite different names*

