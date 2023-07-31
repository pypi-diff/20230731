# Comparing `tmp/mpoints-0.3.0.tar.gz` & `tmp/mpoints-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpoints-0.3.0.tar", last modified: Mon Jul 31 07:57:35 2023, max compression
+gzip compressed data, was "mpoints-1.0.0.tar", last modified: Mon Jul 31 08:01:00 2023, max compression
```

## Comparing `mpoints-0.3.0.tar` & `mpoints-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 07:57:35.755788 mpoints-0.3.0/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1073 2023-07-30 16:40:03.000000 mpoints-0.3.0/LICENSE
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      254 2023-07-31 07:57:35.755788 mpoints-0.3.0/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1758 2023-07-30 16:40:03.000000 mpoints-0.3.0/README.md
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 07:57:35.751788 mpoints-0.3.0/doc/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5471 2023-07-30 16:40:03.000000 mpoints-0.3.0/doc/conf.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 07:57:35.755788 mpoints-0.3.0/mpoints/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       17 2023-07-30 16:40:03.000000 mpoints-0.3.0/mpoints/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    65227 2023-07-30 16:40:03.000000 mpoints-0.3.0/mpoints/hybrid_hawkes_exp.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)  1053904 2023-07-30 16:40:03.000000 mpoints-0.3.0/mpoints/hybrid_hawkes_exp_cython.c
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    31779 2023-07-30 16:40:03.000000 mpoints-0.3.0/mpoints/plot_tools.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      766 2023-07-30 16:40:03.000000 mpoints-0.3.0/mpoints/setup.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 07:57:35.755788 mpoints-0.3.0/mpoints.egg-info/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      254 2023-07-31 07:57:35.000000 mpoints-0.3.0/mpoints.egg-info/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      362 2023-07-31 07:57:35.000000 mpoints-0.3.0/mpoints.egg-info/SOURCES.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-07-31 07:57:35.000000 mpoints-0.3.0/mpoints.egg-info/dependency_links.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       38 2023-07-31 07:57:35.000000 mpoints-0.3.0/mpoints.egg-info/requires.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       23 2023-07-31 07:57:35.000000 mpoints-0.3.0/mpoints.egg-info/top_level.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      515 2023-07-31 07:57:07.000000 mpoints-0.3.0/pyproject.toml
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       38 2023-07-31 07:57:35.755788 mpoints-0.3.0/setup.cfg
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      386 2023-07-30 16:40:03.000000 mpoints-0.3.0/setup.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 07:57:35.755788 mpoints-0.3.0/tests/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5894 2023-07-30 17:39:48.000000 mpoints-0.3.0/tests/hybrid_hawkes_exp_test.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 08:01:00.016442 mpoints-1.0.0/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1073 2023-07-30 16:40:03.000000 mpoints-1.0.0/LICENSE
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2053 2023-07-31 08:01:00.016442 mpoints-1.0.0/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1758 2023-07-30 16:40:03.000000 mpoints-1.0.0/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 08:01:00.016442 mpoints-1.0.0/doc/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5471 2023-07-30 16:40:03.000000 mpoints-1.0.0/doc/conf.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 08:01:00.016442 mpoints-1.0.0/mpoints/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       17 2023-07-30 16:40:03.000000 mpoints-1.0.0/mpoints/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    65227 2023-07-30 16:40:03.000000 mpoints-1.0.0/mpoints/hybrid_hawkes_exp.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)  1053904 2023-07-30 16:40:03.000000 mpoints-1.0.0/mpoints/hybrid_hawkes_exp_cython.c
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    31779 2023-07-30 16:40:03.000000 mpoints-1.0.0/mpoints/plot_tools.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      766 2023-07-30 16:40:03.000000 mpoints-1.0.0/mpoints/setup.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 08:01:00.016442 mpoints-1.0.0/mpoints.egg-info/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2053 2023-07-31 08:01:00.000000 mpoints-1.0.0/mpoints.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      362 2023-07-31 08:01:00.000000 mpoints-1.0.0/mpoints.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-07-31 08:01:00.000000 mpoints-1.0.0/mpoints.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       38 2023-07-31 08:01:00.000000 mpoints-1.0.0/mpoints.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       23 2023-07-31 08:01:00.000000 mpoints-1.0.0/mpoints.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      536 2023-07-31 08:00:41.000000 mpoints-1.0.0/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       38 2023-07-31 08:01:00.016442 mpoints-1.0.0/setup.cfg
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      386 2023-07-30 16:40:03.000000 mpoints-1.0.0/setup.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-31 08:01:00.016442 mpoints-1.0.0/tests/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5894 2023-07-30 17:39:48.000000 mpoints-1.0.0/tests/hybrid_hawkes_exp_test.py
```

### Comparing `mpoints-0.3.0/LICENSE` & `mpoints-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/README.md` & `mpoints-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/doc/conf.py` & `mpoints-1.0.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/mpoints/hybrid_hawkes_exp.py` & `mpoints-1.0.0/mpoints/hybrid_hawkes_exp.py`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/mpoints/hybrid_hawkes_exp_cython.c` & `mpoints-1.0.0/mpoints/hybrid_hawkes_exp_cython.c`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/mpoints/plot_tools.py` & `mpoints-1.0.0/mpoints/plot_tools.py`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/mpoints/setup.py` & `mpoints-1.0.0/mpoints/setup.py`

 * *Files identical despite different names*

### Comparing `mpoints-0.3.0/tests/hybrid_hawkes_exp_test.py` & `mpoints-1.0.0/tests/hybrid_hawkes_exp_test.py`

 * *Files identical despite different names*

