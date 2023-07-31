# Comparing `tmp/equilibrator-api-0.5.0.tar.gz` & `tmp/equilibrator-api-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-api-0.5.0.tar", last modified: Mon Jul 31 11:42:34 2023, max compression
+gzip compressed data, was "equilibrator-api-0.5.0b1.tar", last modified: Sun Jul 30 12:15:52 2023, max compression
```

## Comparing `equilibrator-api-0.5.0.tar` & `equilibrator-api-0.5.0b1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:42:34.126520 equilibrator-api-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4631 2023-07-31 11:42:34.126520 equilibrator-api-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-07-31 11:42:34.127519 equilibrator-api-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:42:34.121519 equilibrator-api-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:42:34.127519 equilibrator-api-0.5.0/src/equilibrator_api/
--rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-31 11:42:34.127519 equilibrator-api-0.5.0/src/equilibrator_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)    35662 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/component_contribution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:42:34.126520 equilibrator-api-0.5.0/src/equilibrator_api/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/data/cofactors.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:42:34.126520 equilibrator-api-0.5.0/src/equilibrator_api/model/
--rw-rw-rw-   0 root         (0) root         (0)     2171 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10479 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/model/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)    34576 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)    18294 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/phased_compound.py
--rw-rw-rw-   0 root         (0) root         (0)    15969 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/phased_reaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/src/equilibrator_api/reaction_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:42:34.125520 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4631 2023-07-31 11:42:34.000000 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      796 2023-07-31 11:42:34.000000 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:42:34.000000 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-31 11:42:34.000000 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 11:42:34.000000 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:42:34.000000 equilibrator-api-0.5.0/src/equilibrator_api.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-31 11:42:22.000000 equilibrator-api-0.5.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.723698 equilibrator-api-0.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.717698 equilibrator-api-0.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/src/equilibrator_api/
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 12:15:52.724698 equilibrator-api-0.5.0b1/src/equilibrator_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    35662 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/component_contribution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.723698 equilibrator-api-0.5.0b1/src/equilibrator_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/data/cofactors.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.723698 equilibrator-api-0.5.0b1/src/equilibrator_api/model/
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10479 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/model/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)    34576 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    18294 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/phased_compound.py
+-rw-rw-rw-   0 root         (0) root         (0)    15969 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/phased_reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/src/equilibrator_api/reaction_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:15:52.722698 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      796 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      307 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 12:15:52.000000 equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-30 12:15:41.000000 equilibrator-api-0.5.0b1/versioneer.py
```

### Comparing `equilibrator-api-0.5.0/LICENSE` & `equilibrator-api-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/PKG-INFO` & `equilibrator-api-0.5.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-api
-Version: 0.5.0
+Version: 0.5.0b1
 Summary: Calculation of standard thermodynamic potentials of biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/equilibrator-api/
 Download-URL: https://pypi.org/project/equilibrator-api/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-api/
```

### Comparing `equilibrator-api-0.5.0/README.md` & `equilibrator-api-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/setup.cfg` & `equilibrator-api-0.5.0b1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 	eQuilibrator
 
 [options]
 zip_safe = True
 install_requires = 
 	pyparsing~=3.0
 	python-slugify~=5.0
-	equilibrator-cache~=0.5.0
-	component-contribution~=0.5.0
+	equilibrator-cache~=0.5.0b2
+	component-contribution~=0.5.0b1
 python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
```

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/__init__.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/compatibility.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/component_contribution.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/component_contribution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/data/cofactors.csv` & `equilibrator-api-0.5.0b1/src/equilibrator_api/data/cofactors.csv`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/model/__init__.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/model/bounds.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/model/bounds.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/model/model.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/model/model.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/phased_compound.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/phased_compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/phased_reaction.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/phased_reaction.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api/reaction_parser.py` & `equilibrator-api-0.5.0b1/src/equilibrator_api/reaction_parser.py`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api.egg-info/PKG-INFO` & `equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-api
-Version: 0.5.0
+Version: 0.5.0b1
 Summary: Calculation of standard thermodynamic potentials of biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/equilibrator-api/
 Download-URL: https://pypi.org/project/equilibrator-api/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-api/
```

### Comparing `equilibrator-api-0.5.0/src/equilibrator_api.egg-info/SOURCES.txt` & `equilibrator-api-0.5.0b1/src/equilibrator_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-api-0.5.0/versioneer.py` & `equilibrator-api-0.5.0b1/versioneer.py`

 * *Files identical despite different names*

