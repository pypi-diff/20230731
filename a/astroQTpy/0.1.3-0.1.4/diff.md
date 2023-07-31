# Comparing `tmp/astroQTpy-0.1.3.tar.gz` & `tmp/astroQTpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroQTpy-0.1.3.tar", last modified: Fri Jul 28 23:30:40 2023, max compression
+gzip compressed data, was "astroQTpy-0.1.4.tar", last modified: Mon Jul 31 21:41:39 2023, max compression
```

## Comparing `astroQTpy-0.1.3.tar` & `astroQTpy-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-28 23:30:40.855832 astroQTpy-0.1.3/
--rw-r--r--   0 calebharada   (501) staff       (20)     1069 2023-07-15 16:01:20.000000 astroQTpy-0.1.3/LICENSE
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-28 23:30:40.855507 astroQTpy-0.1.3/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      484 2023-07-27 22:43:58.000000 astroQTpy-0.1.3/README.md
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-28 23:30:40.850850 astroQTpy-0.1.3/astroQTpy.egg-info/
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-28 23:30:40.000000 astroQTpy-0.1.3/astroQTpy.egg-info/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      381 2023-07-28 23:30:40.000000 astroQTpy-0.1.3/astroQTpy.egg-info/SOURCES.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-28 23:30:40.000000 astroQTpy-0.1.3/astroQTpy.egg-info/dependency_links.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       47 2023-07-28 23:30:40.000000 astroQTpy-0.1.3/astroQTpy.egg-info/requires.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       16 2023-07-28 23:30:40.000000 astroQTpy-0.1.3/astroQTpy.egg-info/top_level.txt
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-28 23:30:40.853223 astroQTpy-0.1.3/astroqtpy/
--rw-r--r--   0 calebharada   (501) staff       (20)      135 2023-07-28 23:28:17.000000 astroQTpy-0.1.3/astroqtpy/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)    16457 2023-07-26 22:04:11.000000 astroQTpy-0.1.3/astroqtpy/basetree.py
--rw-r--r--   0 calebharada   (501) staff       (20)     8904 2023-07-26 22:04:11.000000 astroQTpy-0.1.3/astroqtpy/quadnode.py
--rw-r--r--   0 calebharada   (501) staff       (20)      831 2023-07-26 22:04:11.000000 astroQTpy-0.1.3/astroqtpy/quadpoint.py
--rw-r--r--   0 calebharada   (501) staff       (20)    14141 2023-07-26 22:04:11.000000 astroQTpy-0.1.3/astroqtpy/quadtree.py
--rw-r--r--   0 calebharada   (501) staff       (20)       79 2023-07-26 22:04:11.000000 astroQTpy-0.1.3/pyproject.toml
--rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-28 23:30:40.855928 astroQTpy-0.1.3/setup.cfg
--rw-r--r--   0 calebharada   (501) staff       (20)      876 2023-07-26 23:07:18.000000 astroQTpy-0.1.3/setup.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-28 23:30:40.854933 astroQTpy-0.1.3/tests/
--rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-20 22:59:55.000000 astroQTpy-0.1.3/tests/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1383 2023-07-26 22:04:11.000000 astroQTpy-0.1.3/tests/test_quadnode.py
--rw-r--r--   0 calebharada   (501) staff       (20)      721 2023-07-20 01:38:47.000000 astroQTpy-0.1.3/tests/test_quadpoint.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.215078 astroQTpy-0.1.4/
+-rw-r--r--   0 calebharada   (501) staff       (20)     1069 2023-07-15 16:01:20.000000 astroQTpy-0.1.4/LICENSE
+-rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-31 21:41:39.214590 astroQTpy-0.1.4/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)     1307 2023-07-31 21:39:08.000000 astroQTpy-0.1.4/README.md
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.207322 astroQTpy-0.1.4/astroQTpy.egg-info/
+-rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      381 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/SOURCES.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/dependency_links.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       47 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/requires.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       16 2023-07-31 21:41:39.000000 astroQTpy-0.1.4/astroQTpy.egg-info/top_level.txt
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.211280 astroQTpy-0.1.4/astroqtpy/
+-rw-r--r--   0 calebharada   (501) staff       (20)      135 2023-07-31 21:34:54.000000 astroQTpy-0.1.4/astroqtpy/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    16457 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/basetree.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     8904 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/quadnode.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      831 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/quadpoint.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    14141 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/astroqtpy/quadtree.py
+-rw-r--r--   0 calebharada   (501) staff       (20)       79 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/pyproject.toml
+-rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-31 21:41:39.215185 astroQTpy-0.1.4/setup.cfg
+-rw-r--r--   0 calebharada   (501) staff       (20)      876 2023-07-26 23:07:18.000000 astroQTpy-0.1.4/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-31 21:41:39.213451 astroQTpy-0.1.4/tests/
+-rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-20 22:59:55.000000 astroQTpy-0.1.4/tests/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1383 2023-07-26 22:04:11.000000 astroQTpy-0.1.4/tests/test_quadnode.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      721 2023-07-20 01:38:47.000000 astroQTpy-0.1.4/tests/test_quadpoint.py
```

### Comparing `astroQTpy-0.1.3/LICENSE` & `astroQTpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/astroqtpy/basetree.py` & `astroQTpy-0.1.4/astroqtpy/basetree.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/astroqtpy/quadnode.py` & `astroQTpy-0.1.4/astroqtpy/quadnode.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/astroqtpy/quadpoint.py` & `astroQTpy-0.1.4/astroqtpy/quadpoint.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/astroqtpy/quadtree.py` & `astroQTpy-0.1.4/astroqtpy/quadtree.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/setup.py` & `astroQTpy-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/tests/test_quadnode.py` & `astroQTpy-0.1.4/tests/test_quadnode.py`

 * *Files identical despite different names*

### Comparing `astroQTpy-0.1.3/tests/test_quadpoint.py` & `astroQTpy-0.1.4/tests/test_quadpoint.py`

 * *Files identical despite different names*

