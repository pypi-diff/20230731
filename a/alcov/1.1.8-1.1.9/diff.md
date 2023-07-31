# Comparing `tmp/alcov-1.1.8.tar.gz` & `tmp/alcov-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcov-1.1.8.tar", last modified: Tue Jul 25 15:18:20 2023, max compression
+gzip compressed data, was "alcov-1.1.9.tar", last modified: Mon Jul 31 17:02:24 2023, max compression
```

## Comparing `alcov-1.1.8.tar` & `alcov-1.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-25 15:18:20.277369 alcov-1.1.8/
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4795 2023-07-25 15:18:20.273369 alcov-1.1.8/PKG-INFO
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4463 2023-07-10 20:59:26.000000 alcov-1.1.8/README.md
-drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-25 15:18:20.257368 alcov-1.1.8/alcov/
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     1194 2023-01-04 16:05:57.000000 alcov-1.1.8/alcov/__init__.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     5566 2022-12-20 19:00:26.000000 alcov-1.1.8/alcov/amplicon_coverage.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     8933 2023-06-14 17:58:05.000000 alcov-1.1.8/alcov/analyze.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     6800 2022-05-17 19:36:10.000000 alcov-1.1.8/alcov/artic_amplicons.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      279 2022-05-17 19:36:10.000000 alcov-1.1.8/alcov/cmds.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       73 2022-05-17 19:36:10.000000 alcov-1.1.8/alcov/command_line.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      546 2022-05-17 19:36:10.000000 alcov-1.1.8/alcov/consensus.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)   730320 2023-07-25 15:13:43.000000 alcov-1.1.8/alcov/constellations.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     3713 2022-12-20 19:00:26.000000 alcov-1.1.8/alcov/convert_mutations.py
--rwxrwxr-x   0 jknapp    (1008) jknapp    (1010)    17219 2023-06-27 20:30:38.000000 alcov-1.1.8/alcov/lineages.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     3726 2023-07-10 20:24:55.000000 alcov-1.1.8/alcov/make_constellations.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010) 59233478 2023-07-25 15:13:44.000000 alcov-1.1.8/alcov/mutations.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     6789 2023-06-02 17:37:59.000000 alcov-1.1.8/alcov/precompute.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)    30784 2022-10-14 21:05:11.000000 alcov-1.1.8/alcov/sars_cov_2.py
-drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-25 15:18:20.273369 alcov-1.1.8/alcov.egg-info/
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4795 2023-07-25 15:18:19.000000 alcov-1.1.8/alcov.egg-info/PKG-INFO
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      493 2023-07-25 15:18:19.000000 alcov-1.1.8/alcov.egg-info/SOURCES.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        1 2023-07-25 15:18:19.000000 alcov-1.1.8/alcov.egg-info/dependency_links.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       50 2023-07-25 15:18:19.000000 alcov-1.1.8/alcov.egg-info/entry_points.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       62 2023-07-25 15:18:19.000000 alcov-1.1.8/alcov.egg-info/requires.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        6 2023-07-25 15:18:19.000000 alcov-1.1.8/alcov.egg-info/top_level.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       38 2023-07-25 15:18:20.277369 alcov-1.1.8/setup.cfg
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      811 2023-07-25 14:18:41.000000 alcov-1.1.8/setup.py
+drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-31 17:02:24.137747 alcov-1.1.9/
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4795 2023-07-31 17:02:24.137747 alcov-1.1.9/PKG-INFO
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4463 2023-07-10 20:59:26.000000 alcov-1.1.9/README.md
+drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-31 17:02:24.121746 alcov-1.1.9/alcov/
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     1194 2023-01-04 16:05:57.000000 alcov-1.1.9/alcov/__init__.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     5566 2022-12-20 19:00:26.000000 alcov-1.1.9/alcov/amplicon_coverage.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     8933 2023-06-14 17:58:05.000000 alcov-1.1.9/alcov/analyze.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     6800 2022-05-17 19:36:10.000000 alcov-1.1.9/alcov/artic_amplicons.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      279 2022-05-17 19:36:10.000000 alcov-1.1.9/alcov/cmds.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       73 2022-05-17 19:36:10.000000 alcov-1.1.9/alcov/command_line.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      546 2022-05-17 19:36:10.000000 alcov-1.1.9/alcov/consensus.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)   730320 2023-07-31 16:50:36.000000 alcov-1.1.9/alcov/constellations.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     3713 2022-12-20 19:00:26.000000 alcov-1.1.9/alcov/convert_mutations.py
+-rwxrwxr-x   0 jknapp    (1008) jknapp    (1010)    17219 2023-06-27 20:30:38.000000 alcov-1.1.9/alcov/lineages.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     3726 2023-07-10 20:24:55.000000 alcov-1.1.9/alcov/make_constellations.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010) 59233478 2023-07-31 16:50:37.000000 alcov-1.1.9/alcov/mutations.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     6789 2023-06-02 17:37:59.000000 alcov-1.1.9/alcov/precompute.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)    30784 2022-10-14 21:05:11.000000 alcov-1.1.9/alcov/sars_cov_2.py
+drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-31 17:02:24.137747 alcov-1.1.9/alcov.egg-info/
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4795 2023-07-31 17:02:23.000000 alcov-1.1.9/alcov.egg-info/PKG-INFO
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      493 2023-07-31 17:02:23.000000 alcov-1.1.9/alcov.egg-info/SOURCES.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        1 2023-07-31 17:02:23.000000 alcov-1.1.9/alcov.egg-info/dependency_links.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       50 2023-07-31 17:02:23.000000 alcov-1.1.9/alcov.egg-info/entry_points.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       62 2023-07-31 17:02:23.000000 alcov-1.1.9/alcov.egg-info/requires.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        6 2023-07-31 17:02:23.000000 alcov-1.1.9/alcov.egg-info/top_level.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       38 2023-07-31 17:02:24.137747 alcov-1.1.9/setup.cfg
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      811 2023-07-31 16:57:10.000000 alcov-1.1.9/setup.py
```

### Comparing `alcov-1.1.8/PKG-INFO` & `alcov-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcov
-Version: 1.1.8
+Version: 1.1.9
 Summary: Identify frequencies of concerning mutations from aligned reads
 Home-page: https://github.com/Ellmen/alcov
 Author: Isaac Ellmen
 Author-email: isaac.ellmen@uwaterloo.ca
 Maintainer: Jenn Knapp
 Maintainer-email: jenn.knapp@uwaterloo.ca
 Description-Content-Type: text/markdown
```

### Comparing `alcov-1.1.8/README.md` & `alcov-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/__init__.py` & `alcov-1.1.9/alcov/__init__.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/amplicon_coverage.py` & `alcov-1.1.9/alcov/amplicon_coverage.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/analyze.py` & `alcov-1.1.9/alcov/analyze.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/artic_amplicons.py` & `alcov-1.1.9/alcov/artic_amplicons.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/consensus.py` & `alcov-1.1.9/alcov/consensus.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/constellations.py` & `alcov-1.1.9/alcov/constellations.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/convert_mutations.py` & `alcov-1.1.9/alcov/convert_mutations.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/lineages.py` & `alcov-1.1.9/alcov/lineages.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/make_constellations.py` & `alcov-1.1.9/alcov/make_constellations.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/mutations.py` & `alcov-1.1.9/alcov/mutations.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/precompute.py` & `alcov-1.1.9/alcov/precompute.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov/sars_cov_2.py` & `alcov-1.1.9/alcov/sars_cov_2.py`

 * *Files identical despite different names*

### Comparing `alcov-1.1.8/alcov.egg-info/PKG-INFO` & `alcov-1.1.9/alcov.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcov
-Version: 1.1.8
+Version: 1.1.9
 Summary: Identify frequencies of concerning mutations from aligned reads
 Home-page: https://github.com/Ellmen/alcov
 Author: Isaac Ellmen
 Author-email: isaac.ellmen@uwaterloo.ca
 Maintainer: Jenn Knapp
 Maintainer-email: jenn.knapp@uwaterloo.ca
 Description-Content-Type: text/markdown
```

### Comparing `alcov-1.1.8/setup.py` & `alcov-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='alcov',
-    version='1.1.8',
+    version='1.1.9',
     description='Identify frequencies of concerning mutations from aligned reads',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Isaac Ellmen',
     author_email='isaac.ellmen@uwaterloo.ca',
     maintainer='Jenn Knapp',
     maintainer_email='jenn.knapp@uwaterloo.ca',
```

