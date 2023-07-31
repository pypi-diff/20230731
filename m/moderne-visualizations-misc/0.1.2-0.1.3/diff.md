# Comparing `tmp/moderne_visualizations_misc-0.1.2.tar.gz` & `tmp/moderne_visualizations_misc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderne_visualizations_misc-0.1.2.tar", last modified: Mon Jul 31 15:57:07 2023, max compression
+gzip compressed data, was "moderne_visualizations_misc-0.1.3.tar", last modified: Mon Jul 31 16:00:36 2023, max compression
```

## Comparing `moderne_visualizations_misc-0.1.2.tar` & `moderne_visualizations_misc-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/language_composition.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/parse_failure_analysis.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/sql_crud.300.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/language_composition.yml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/parse_failure_analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/sql_crud.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 15:57:07.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 15:57:07.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:57:07.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 15:57:07.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 15:57:07.000000 moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 15:56:50.000000 moderne_visualizations_misc-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:57:07.607147 moderne_visualizations_misc-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.448368 moderne_visualizations_misc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/language_composition.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/parse_failure_analysis.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/sql_crud.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/language_composition.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/parse_failure_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/language_composition.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/parse_failure_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/sql_crud.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/sql_crud.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:00:36.448368 moderne_visualizations_misc-0.1.3/setup.cfg
```

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/language_composition.300.png` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/language_composition.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/parse_failure_analysis.300.png` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/parse_failure_analysis.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/images/sql_crud.300.png` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/sql_crud.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc/specs/parse_failure_analysis.yml` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/parse_failure_analysis.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.2/moderne_visualizations_misc.egg-info/SOURCES.txt` & `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 moderne_visualizations_misc/__init__.py
+moderne_visualizations_misc/dependency_vulnerabilities.ipynb
+moderne_visualizations_misc/language_composition.ipynb
+moderne_visualizations_misc/parse_failure_analysis.ipynb
+moderne_visualizations_misc/sql_crud.ipynb
 moderne_visualizations_misc.egg-info/PKG-INFO
 moderne_visualizations_misc.egg-info/SOURCES.txt
 moderne_visualizations_misc.egg-info/dependency_links.txt
 moderne_visualizations_misc.egg-info/requires.txt
 moderne_visualizations_misc.egg-info/top_level.txt
 moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
 moderne_visualizations_misc/images/language_composition.300.png
```

### Comparing `moderne_visualizations_misc-0.1.2/pyproject.toml` & `moderne_visualizations_misc-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "moderne_visualizations_misc"
-version = "0.1.2"
+version = "0.1.3"
 description = "Miscellaneous visualizations for the Moderne platform"
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

