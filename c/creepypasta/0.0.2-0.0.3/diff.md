# Comparing `tmp/creepypasta-0.0.2.tar.gz` & `tmp/creepypasta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creepypasta-0.0.2.tar", last modified: Mon Jul 31 04:13:51 2023, max compression
+gzip compressed data, was "creepypasta-0.0.3.tar", last modified: Mon Jul 31 04:41:58 2023, max compression
```

## Comparing `creepypasta-0.0.2.tar` & `creepypasta-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:13:51.106222 creepypasta-0.0.2/
--rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-07-31 04:13:51.106275 creepypasta-0.0.2/PKG-INFO
--rw-r--r--   0 sandrews   (501) staff       (20)       66 2023-07-31 03:53:30.000000 creepypasta-0.0.2/README.md
--rw-r--r--   0 sandrews   (501) staff       (20)      898 2023-07-31 04:02:45.000000 creepypasta-0.0.2/pyproject.toml
--rw-r--r--   0 sandrews   (501) staff       (20)      918 2023-07-31 04:13:51.106528 creepypasta-0.0.2/setup.cfg
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:13:51.103858 creepypasta-0.0.2/src/
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:13:51.104862 creepypasta-0.0.2/src/creepypasta/
--rw-r--r--   0 sandrews   (501) staff       (20)       59 2023-07-31 03:53:33.000000 creepypasta-0.0.2/src/creepypasta/__init__.py
--rw-r--r--   0 sandrews   (501) staff       (20)     8825 2023-07-28 13:46:50.000000 creepypasta-0.0.2/src/creepypasta/pasta-listings.py
--rw-r--r--   0 sandrews   (501) staff       (20)    16890 2023-07-28 13:46:50.000000 creepypasta-0.0.2/src/creepypasta/pasta-stories.py
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:13:51.105759 creepypasta-0.0.2/src/creepypasta.egg-info/
--rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-07-31 04:13:51.000000 creepypasta-0.0.2/src/creepypasta.egg-info/PKG-INFO
--rw-r--r--   0 sandrews   (501) staff       (20)      342 2023-07-31 04:13:51.000000 creepypasta-0.0.2/src/creepypasta.egg-info/SOURCES.txt
--rw-r--r--   0 sandrews   (501) staff       (20)        1 2023-07-31 04:13:51.000000 creepypasta-0.0.2/src/creepypasta.egg-info/dependency_links.txt
--rw-r--r--   0 sandrews   (501) staff       (20)      181 2023-07-31 04:13:51.000000 creepypasta-0.0.2/src/creepypasta.egg-info/requires.txt
--rw-r--r--   0 sandrews   (501) staff       (20)       12 2023-07-31 04:13:51.000000 creepypasta-0.0.2/src/creepypasta.egg-info/top_level.txt
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:13:51.105880 creepypasta-0.0.2/test/
--rw-r--r--   0 sandrews   (501) staff       (20)     2453 2023-07-28 13:51:00.000000 creepypasta-0.0.2/test/test-units.py
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.554147 creepypasta-0.0.3/
+-rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-07-31 04:41:58.554192 creepypasta-0.0.3/PKG-INFO
+-rw-r--r--   0 sandrews   (501) staff       (20)       66 2023-07-31 03:53:30.000000 creepypasta-0.0.3/README.md
+-rw-r--r--   0 sandrews   (501) staff       (20)      898 2023-07-31 04:41:43.000000 creepypasta-0.0.3/pyproject.toml
+-rw-r--r--   0 sandrews   (501) staff       (20)      918 2023-07-31 04:41:58.554454 creepypasta-0.0.3/setup.cfg
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.552567 creepypasta-0.0.3/src/
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.553324 creepypasta-0.0.3/src/creepypasta/
+-rw-r--r--   0 sandrews   (501) staff       (20)       59 2023-07-31 04:40:38.000000 creepypasta-0.0.3/src/creepypasta/__init__.py
+-rw-r--r--   0 sandrews   (501) staff       (20)     8825 2023-07-28 13:46:50.000000 creepypasta-0.0.3/src/creepypasta/pasta_listings.py
+-rw-r--r--   0 sandrews   (501) staff       (20)    16890 2023-07-28 13:46:50.000000 creepypasta-0.0.3/src/creepypasta/pasta_stories.py
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.553937 creepypasta-0.0.3/src/creepypasta.egg-info/
+-rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/PKG-INFO
+-rw-r--r--   0 sandrews   (501) staff       (20)      342 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)        1 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)      181 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/requires.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)       12 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/top_level.txt
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.554053 creepypasta-0.0.3/test/
+-rw-r--r--   0 sandrews   (501) staff       (20)     2453 2023-07-28 13:51:00.000000 creepypasta-0.0.3/test/test-units.py
```

### Comparing `creepypasta-0.0.2/PKG-INFO` & `creepypasta-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creepypasta
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package to crawl CreepyPasta and parse into structured data.
 Home-page: https://jellomoat.github.io/pasta/
 Author: Stephanie Andrews
 Author-email: Stephanie Andrews <jellomoat@gmail.com>
 Project-URL: Homepage, https://github.com/jellomoat/pasta
 Project-URL: Bug Tracker, https://github.com/jellomoat/pasta/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `creepypasta-0.0.2/pyproject.toml` & `creepypasta-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "selenium-wire==5.1.0",
     "tqdm==4.65.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "creepypasta"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Stephanie Andrews", email="jellomoat@gmail.com" },
 ]
 description = "A small package to crawl CreepyPasta and parse into structured data."
 
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `creepypasta-0.0.2/setup.cfg` & `creepypasta-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = creepypasta
-version = 0.0.2
+version = 0.0.3
 author = Stephanie Andrews
 author_email = jellomoat@gmail.com
 description = A small package to crawl CreepyPasta and parse into structured data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://jellomoat.github.io/pasta/
 project_urls =
```

### Comparing `creepypasta-0.0.2/src/creepypasta/pasta-listings.py` & `creepypasta-0.0.3/src/creepypasta/pasta_listings.py`

 * *Files identical despite different names*

### Comparing `creepypasta-0.0.2/src/creepypasta/pasta-stories.py` & `creepypasta-0.0.3/src/creepypasta/pasta_stories.py`

 * *Files identical despite different names*

### Comparing `creepypasta-0.0.2/src/creepypasta.egg-info/PKG-INFO` & `creepypasta-0.0.3/src/creepypasta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creepypasta
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package to crawl CreepyPasta and parse into structured data.
 Home-page: https://jellomoat.github.io/pasta/
 Author: Stephanie Andrews
 Author-email: Stephanie Andrews <jellomoat@gmail.com>
 Project-URL: Homepage, https://github.com/jellomoat/pasta
 Project-URL: Bug Tracker, https://github.com/jellomoat/pasta/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `creepypasta-0.0.2/test/test-units.py` & `creepypasta-0.0.3/test/test-units.py`

 * *Files identical despite different names*

