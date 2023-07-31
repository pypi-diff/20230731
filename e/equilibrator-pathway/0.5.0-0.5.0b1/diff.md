# Comparing `tmp/equilibrator-pathway-0.5.0.tar.gz` & `tmp/equilibrator-pathway-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-pathway-0.5.0.tar", last modified: Mon Jul 31 13:15:01 2023, max compression
+gzip compressed data, was "equilibrator-pathway-0.5.0b1.tar", last modified: Sun Jul 30 13:07:49 2023, max compression
```

## Comparing `equilibrator-pathway-0.5.0.tar` & `equilibrator-pathway-0.5.0b1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:15:01.153653 equilibrator-pathway-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4066 2023-07-31 13:15:01.153653 equilibrator-pathway-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-07-31 13:15:01.154653 equilibrator-pathway-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:15:01.147657 equilibrator-pathway-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:15:01.154653 equilibrator-pathway-0.5.0/src/equilibrator_pathway/
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-31 13:15:01.154653 equilibrator-pathway-0.5.0/src/equilibrator_pathway/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/analysis_solution.py
--rwxrwxrwx   0 root         (0) root         (0)    23350 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/cost_function.py
--rw-rw-rw-   0 root         (0) root         (0)    12964 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/ecm_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10311 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/ecm_solution.py
--rw-rw-rw-   0 root         (0) root         (0)     6600 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/mdf_solution.py
--rwxrwxrwx   0 root         (0) root         (0)     7446 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/mdmc_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    10429 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/pathway.py
--rw-rw-rw-   0 root         (0) root         (0)     4343 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    10878 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/thermo_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4363 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:15:01.153653 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4066 2023-07-31 13:15:01.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      832 2023-07-31 13:15:01.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:15:01.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-31 13:15:01.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 13:15:01.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:15:01.000000 equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-31 13:14:48.000000 equilibrator-pathway-0.5.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.531733 equilibrator-pathway-0.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-30 13:07:49.531733 equilibrator-pathway-0.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-07-30 13:07:49.532733 equilibrator-pathway-0.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.524733 equilibrator-pathway-0.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.532733 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 13:07:49.532733 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/analysis_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)    23350 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/cost_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    12964 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10311 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)     6600 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdf_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)     7446 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdmc_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    10429 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/pathway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4343 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10878 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/thermo_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:07:49.531733 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      294 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 13:07:49.000000 equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-07-30 13:07:37.000000 equilibrator-pathway-0.5.0b1/versioneer.py
```

### Comparing `equilibrator-pathway-0.5.0/LICENSE` & `equilibrator-pathway-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/PKG-INFO` & `equilibrator-pathway-0.5.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.5.0
+Version: 0.5.0b1
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
@@ -12,14 +12,15 @@
 Keywords: biochemical reaction,eQuilibrator,pathway analysis,enzyme cost minimization,max-min driving force
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `equilibrator-pathway-0.5.0/README.md` & `equilibrator-pathway-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/setup.cfg` & `equilibrator-pathway-0.5.0b1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Chemistry
 license = MIT
 description = Pathway analysis tools by eQuilibrator
@@ -31,17 +32,17 @@
 	max-min driving force
 
 [options]
 zip_safe = True
 install_requires = 
 	seaborn~=0.12
 	osqp~=0.6
-	cvxpy~=1.3,>=1.3.2
+	cvxpy~=1.3
 	sbtab~=1.0
-	equilibrator-api~=0.5.0
+	equilibrator-api==0.5.0b1
 python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
```

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/__init__.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/analysis_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/analysis_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/cost_function.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/cost_function.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/ecm_model.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_model.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/ecm_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/ecm_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/mdf_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdf_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/mdmc_solution.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/mdmc_solution.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/pathway.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/pathway.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/simulator.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/simulator.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/thermo_models.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/thermo_models.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway/util.py` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway/util.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/PKG-INFO` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.5.0
+Version: 0.5.0b1
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
@@ -12,14 +12,15 @@
 Keywords: biochemical reaction,eQuilibrator,pathway analysis,enzyme cost minimization,max-min driving force
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `equilibrator-pathway-0.5.0/src/equilibrator_pathway.egg-info/SOURCES.txt` & `equilibrator-pathway-0.5.0b1/src/equilibrator_pathway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.5.0/versioneer.py` & `equilibrator-pathway-0.5.0b1/versioneer.py`

 * *Files identical despite different names*

