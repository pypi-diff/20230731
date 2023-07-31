# Comparing `tmp/hpdag-0.1.tar.gz` & `tmp/hpdag-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpdag-0.1.tar", last modified: Mon Jul 31 19:24:50 2023, max compression
+gzip compressed data, was "hpdag-0.2.tar", last modified: Mon Jul 31 19:32:02 2023, max compression
```

## Comparing `hpdag-0.1.tar` & `hpdag-0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 ohadr      (501) staff       (20)        0 2023-07-31 19:24:50.103963 hpdag-0.1/
--rw-r--r--   0 ohadr      (501) staff       (20)     1867 2023-07-31 19:24:50.103825 hpdag-0.1/PKG-INFO
--rw-r--r--   0 ohadr      (501) staff       (20)     1645 2023-07-31 19:21:25.000000 hpdag-0.1/README.md
-drwxr-xr-x   0 ohadr      (501) staff       (20)        0 2023-07-31 19:24:50.103529 hpdag-0.1/hpdag.egg-info/
--rw-r--r--   0 ohadr      (501) staff       (20)     1867 2023-07-31 19:24:50.000000 hpdag-0.1/hpdag.egg-info/PKG-INFO
--rw-r--r--   0 ohadr      (501) staff       (20)      162 2023-07-31 19:24:50.000000 hpdag-0.1/hpdag.egg-info/SOURCES.txt
--rw-r--r--   0 ohadr      (501) staff       (20)        1 2023-07-31 19:24:50.000000 hpdag-0.1/hpdag.egg-info/dependency_links.txt
--rw-r--r--   0 ohadr      (501) staff       (20)        9 2023-07-31 19:24:50.000000 hpdag-0.1/hpdag.egg-info/requires.txt
--rw-r--r--   0 ohadr      (501) staff       (20)        1 2023-07-31 19:24:50.000000 hpdag-0.1/hpdag.egg-info/top_level.txt
--rw-r--r--   0 ohadr      (501) staff       (20)       38 2023-07-31 19:24:50.104005 hpdag-0.1/setup.cfg
--rw-r--r--   0 ohadr      (501) staff       (20)      437 2023-07-31 19:23:20.000000 hpdag-0.1/setup.py
+drwxr-xr-x   0 ohadr      (501) staff       (20)        0 2023-07-31 19:32:02.827390 hpdag-0.2/
+-rw-r--r--   0 ohadr      (501) staff       (20)     1867 2023-07-31 19:32:02.827262 hpdag-0.2/PKG-INFO
+-rw-r--r--   0 ohadr      (501) staff       (20)     1645 2023-07-31 19:21:25.000000 hpdag-0.2/README.md
+drwxr-xr-x   0 ohadr      (501) staff       (20)        0 2023-07-31 19:32:02.826186 hpdag-0.2/hpdag/
+-rw-r--r--   0 ohadr      (501) staff       (20)       40 2023-07-31 19:30:35.000000 hpdag-0.2/hpdag/__init__.py
+-rw-r--r--   0 ohadr      (501) staff       (20)     5059 2023-07-31 19:21:15.000000 hpdag-0.2/hpdag/dag.py
+drwxr-xr-x   0 ohadr      (501) staff       (20)        0 2023-07-31 19:32:02.827076 hpdag-0.2/hpdag.egg-info/
+-rw-r--r--   0 ohadr      (501) staff       (20)     1867 2023-07-31 19:32:02.000000 hpdag-0.2/hpdag.egg-info/PKG-INFO
+-rw-r--r--   0 ohadr      (501) staff       (20)      193 2023-07-31 19:32:02.000000 hpdag-0.2/hpdag.egg-info/SOURCES.txt
+-rw-r--r--   0 ohadr      (501) staff       (20)        1 2023-07-31 19:32:02.000000 hpdag-0.2/hpdag.egg-info/dependency_links.txt
+-rw-r--r--   0 ohadr      (501) staff       (20)        9 2023-07-31 19:32:02.000000 hpdag-0.2/hpdag.egg-info/requires.txt
+-rw-r--r--   0 ohadr      (501) staff       (20)        6 2023-07-31 19:32:02.000000 hpdag-0.2/hpdag.egg-info/top_level.txt
+-rw-r--r--   0 ohadr      (501) staff       (20)       38 2023-07-31 19:32:02.827427 hpdag-0.2/setup.cfg
+-rw-r--r--   0 ohadr      (501) staff       (20)      437 2023-07-31 19:31:51.000000 hpdag-0.2/setup.py
```

### Comparing `hpdag-0.1/PKG-INFO` & `hpdag-0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpdag
-Version: 0.1
+Version: 0.2
 Summary: A DAG library to manage hyperparameter search and ablations
 Home-page: https://github.com/OhadRubin/hpdag
 Author: Ohad Rubin
 Description-Content-Type: text/markdown
 
 # hpdag
```

### Comparing `hpdag-0.1/README.md` & `hpdag-0.2/README.md`

 * *Files identical despite different names*

### Comparing `hpdag-0.1/hpdag.egg-info/PKG-INFO` & `hpdag-0.2/hpdag.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpdag
-Version: 0.1
+Version: 0.2
 Summary: A DAG library to manage hyperparameter search and ablations
 Home-page: https://github.com/OhadRubin/hpdag
 Author: Ohad Rubin
 Description-Content-Type: text/markdown
 
 # hpdag
```

