# Comparing `tmp/caloutils-0.0.8.tar.gz` & `tmp/caloutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caloutils-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caloutils-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caloutils-0.0.8.tar` & `caloutils-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      311 2023-07-31 14:32:23.107529 caloutils-0.0.8/.bumpversion.cfg
--rw-r--r--   0        0        0      292 2023-07-31 14:32:23.107529 caloutils-0.0.8/.editorconfig
--rw-r--r--   0        0        0      320 2023-07-31 14:32:23.107529 caloutils-0.0.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1536 2023-07-31 14:32:23.107529 caloutils-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3095 2023-07-31 14:32:23.107529 caloutils-0.0.8/.gitignore
--rw-r--r--   0        0        0     1122 2023-07-31 14:32:23.107529 caloutils-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      718 2023-07-31 14:32:23.107529 caloutils-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      685 2023-07-31 14:32:23.107529 caloutils-0.0.8/.travis.yml
--rw-r--r--   0        0        0     1062 2023-07-31 14:32:23.107529 caloutils-0.0.8/LICENSE
--rw-r--r--   0        0        0      277 2023-07-31 14:32:23.107529 caloutils-0.0.8/MANIFEST.in
--rw-r--r--   0        0        0      618 2023-07-31 14:32:23.107529 caloutils-0.0.8/Makefile
--rw-r--r--   0        0        0      937 2023-07-31 14:32:23.107529 caloutils-0.0.8/README.rst
--rw-r--r--   0        0        0      388 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/__init__.py
--rw-r--r--   0        0        0      628 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/calorimeter.py
--rw-r--r--   0        0        0      151 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/__init__.py
--rw-r--r--   0        0        0     2101 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/batch_to_Exyz.py
--rw-r--r--   0        0        0     2575 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/pc_from_voxel.py
--rw-r--r--   0        0        0     8698 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/utils.py
--rw-r--r--   0        0        0     1346 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/voxelize.py
--rw-r--r--   0        0        0       68 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/utils/__init__.py
--rw-r--r--   0        0        0     1790 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/utils/batch.py
--rw-r--r--   0        0        0      232 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/__init__.py
--rw-r--r--   0        0        0     3172 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/analyze_layers.py
--rw-r--r--   0        0        0     1867 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/calculate_variables.py
--rw-r--r--   0        0        0     4370 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/energy_ratios.py
--rw-r--r--   0        0        0     2220 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/first_principal_components.py
--rw-r--r--   0        0        0      794 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/response.py
--rw-r--r--   0        0        0      610 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/Makefile
--rw-r--r--   0        0        0      202 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/authors.rst
--rwxr-xr-x   0        0        0     5098 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/conf.py
--rw-r--r--   0        0        0     3517 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/contributing.rst
--rw-r--r--   0        0        0       89 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/history.rst
--rw-r--r--   0        0        0      408 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/index.rst
--rw-r--r--   0        0        0     1126 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/installation.rst
--rw-r--r--   0        0        0      121 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/processing.rst
--rw-r--r--   0        0        0       27 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/readme.rst
--rw-r--r--   0        0        0      103 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/utils.rst
--rw-r--r--   0        0        0      119 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/variables.rst
--rw-r--r--   0        0        0     2484 2023-07-31 14:32:23.111529 caloutils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       39 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/test_batch.py
--rw-r--r--   0        0        0      364 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/test_caloutils.py
--rw-r--r--   0        0        0     5682 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/voxelize.py
--rw-r--r--   0        0        0      230 2023-07-31 14:32:23.111529 caloutils-0.0.8/tox.ini
--rwxr-xr-x   0        0        0      318 2023-07-31 14:32:23.111529 caloutils-0.0.8/venv_setup.sh
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 caloutils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      311 2023-07-31 15:11:12.848149 caloutils-0.0.9/.bumpversion.cfg
+-rw-r--r--   0        0        0      292 2023-07-31 15:11:12.848149 caloutils-0.0.9/.editorconfig
+-rw-r--r--   0        0        0      320 2023-07-31 15:11:12.848149 caloutils-0.0.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1086 2023-07-31 15:11:12.848149 caloutils-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3095 2023-07-31 15:11:12.848149 caloutils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1122 2023-07-31 15:11:12.848149 caloutils-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      712 2023-07-31 15:11:12.848149 caloutils-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      685 2023-07-31 15:11:12.848149 caloutils-0.0.9/.travis.yml
+-rw-r--r--   0        0        0     1062 2023-07-31 15:11:12.848149 caloutils-0.0.9/LICENSE
+-rw-r--r--   0        0        0      277 2023-07-31 15:11:12.848149 caloutils-0.0.9/MANIFEST.in
+-rw-r--r--   0        0        0      628 2023-07-31 15:11:12.848149 caloutils-0.0.9/Makefile
+-rw-r--r--   0        0        0      937 2023-07-31 15:11:12.848149 caloutils-0.0.9/README.rst
+-rw-r--r--   0        0        0      388 2023-07-31 15:11:12.848149 caloutils-0.0.9/caloutils/__init__.py
+-rw-r--r--   0        0        0      628 2023-07-31 15:11:12.848149 caloutils-0.0.9/caloutils/calorimeter.py
+-rw-r--r--   0        0        0      151 2023-07-31 15:11:12.848149 caloutils-0.0.9/caloutils/processing/__init__.py
+-rw-r--r--   0        0        0     2101 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/processing/batch_to_Exyz.py
+-rw-r--r--   0        0        0     2575 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/processing/pc_from_voxel.py
+-rw-r--r--   0        0        0     8698 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/processing/utils.py
+-rw-r--r--   0        0        0     1346 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/processing/voxelize.py
+-rw-r--r--   0        0        0       68 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/utils/__init__.py
+-rw-r--r--   0        0        0     1790 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/utils/batch.py
+-rw-r--r--   0        0        0      232 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/variables/__init__.py
+-rw-r--r--   0        0        0     3172 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/variables/analyze_layers.py
+-rw-r--r--   0        0        0     1867 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/variables/calculate_variables.py
+-rw-r--r--   0        0        0     4370 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/variables/energy_ratios.py
+-rw-r--r--   0        0        0     2220 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/variables/first_principal_components.py
+-rw-r--r--   0        0        0      794 2023-07-31 15:11:12.852149 caloutils-0.0.9/caloutils/variables/response.py
+-rw-r--r--   0        0        0      610 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0      202 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/authors.rst
+-rwxr-xr-x   0        0        0     5240 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0     3517 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/contributing.rst
+-rw-r--r--   0        0        0       89 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/history.rst
+-rw-r--r--   0        0        0      408 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/index.rst
+-rw-r--r--   0        0        0     1126 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/installation.rst
+-rw-r--r--   0        0        0      121 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/processing.rst
+-rw-r--r--   0        0        0       27 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/readme.rst
+-rw-r--r--   0        0        0       62 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0      103 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/utils.rst
+-rw-r--r--   0        0        0      119 2023-07-31 15:11:12.852149 caloutils-0.0.9/docs/variables.rst
+-rw-r--r--   0        0        0     2512 2023-07-31 15:11:12.852149 caloutils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-07-31 15:11:12.852149 caloutils-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-31 15:11:12.852149 caloutils-0.0.9/tests/test_batch.py
+-rw-r--r--   0        0        0      364 2023-07-31 15:11:12.852149 caloutils-0.0.9/tests/test_caloutils.py
+-rw-r--r--   0        0        0     5682 2023-07-31 15:11:12.852149 caloutils-0.0.9/tests/voxelize.py
+-rw-r--r--   0        0        0      230 2023-07-31 15:11:12.852149 caloutils-0.0.9/tox.ini
+-rwxr-xr-x   0        0        0      318 2023-07-31 15:11:12.852149 caloutils-0.0.9/venv_setup.sh
+-rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 caloutils-0.0.9/PKG-INFO
```

### Comparing `caloutils-0.0.8/.gitignore` & `caloutils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/.pre-commit-config.yaml` & `caloutils-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/.readthedocs.yaml` & `caloutils-0.0.9/.readthedocs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 # formats:
 #    - pdf
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
-# python:
-#    install:
-#    - requirements: docs/requirements.txt
+python:
+   install:
+   - requirements: docs/requirements.txt
```

### Comparing `caloutils-0.0.8/.travis.yml` & `caloutils-0.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/LICENSE` & `caloutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/Makefile` & `caloutils-0.0.9/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 release_local: clean test build
 	flit publish
 
 
 release_remote:
 	bump2version patch
+	git push
 	git push --tags
 
 install:
 	# flit install --editable
 	pip install --no-deps -e .
```

### Comparing `caloutils-0.0.8/README.rst` & `caloutils-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/calorimeter.py` & `caloutils-0.0.9/caloutils/calorimeter.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/processing/batch_to_Exyz.py` & `caloutils-0.0.9/caloutils/processing/batch_to_Exyz.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/processing/pc_from_voxel.py` & `caloutils-0.0.9/caloutils/processing/pc_from_voxel.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/processing/utils.py` & `caloutils-0.0.9/caloutils/processing/utils.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/processing/voxelize.py` & `caloutils-0.0.9/caloutils/processing/voxelize.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/utils/batch.py` & `caloutils-0.0.9/caloutils/utils/batch.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/variables/analyze_layers.py` & `caloutils-0.0.9/caloutils/variables/analyze_layers.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/variables/calculate_variables.py` & `caloutils-0.0.9/caloutils/variables/calculate_variables.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/variables/energy_ratios.py` & `caloutils-0.0.9/caloutils/variables/energy_ratios.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/variables/first_principal_components.py` & `caloutils-0.0.9/caloutils/variables/first_principal_components.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/caloutils/variables/response.py` & `caloutils-0.0.9/caloutils/variables/response.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/docs/Makefile` & `caloutils-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/docs/conf.py` & `caloutils-0.0.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 # absolute, like shown here.
 #
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
+autodoc_mock_imports = [
+    "torch_geometric",
+    "torch",
+    "torch_scatter",
+    "tqdm",
+    "numpy",
+]
+
+
 import caloutils
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
@@ -33,14 +42,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.autosummary",
     "autodocsumm",
+    "sphinx_search.extension",
 ]
 
 autosummary_generate = True  # Turn on sphinx.ext.autosummary
 autosummary_generate_overwrite = True
 autodoc_default_options = {
     "autosummary": True,
 }
```

### Comparing `caloutils-0.0.8/docs/contributing.rst` & `caloutils-0.0.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/docs/installation.rst` & `caloutils-0.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/pyproject.toml` & `caloutils-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caloutils"
-version = '0.0.8'
+version = '0.0.9'
 authors = [
   { name="mova", email="mova@users.noreply.github.com" },
   { name="kaechb", email="kaechb@users.noreply.github.com" },
 ]
 description = "Metrics and tools for evaluation generative models for calorimeter shower based on pytorch_geometric."
 requires-python = ">=3.8"
 readme="README.rst"
@@ -25,15 +25,15 @@
   "pytest >=2.7.3",
   "pytest-cov",
   "bump2version",
   "black",
   "pre-commit",
   "ruff",
 ]
-doc = ["sphinx","sphinx_rtd_theme","autodocsumm"]
+doc = ["sphinx","sphinx_rtd_theme","autodocsumm","readthedocs-sphinx-search"]
 
 
 [project.urls]
 "Homepage" = "https://github.com/DeGeSim/caloutils"
 "Bug Tracker" = "https://github.com/DeGeSim/caloutils/issues"
 
 # [project.scripts]
```

### Comparing `caloutils-0.0.8/tests/test_batch.py` & `caloutils-0.0.9/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/tests/voxelize.py` & `caloutils-0.0.9/tests/voxelize.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.8/PKG-INFO` & `caloutils-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caloutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Metrics and tools for evaluation generative models for calorimeter shower based on pytorch_geometric.
 Author-email: mova <mova@users.noreply.github.com>, kaechb <kaechb@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
 Requires-Dist: autodocsumm ; extra == "doc"
+Requires-Dist: readthedocs-sphinx-search ; extra == "doc"
 Project-URL: Bug Tracker, https://github.com/DeGeSim/caloutils/issues
 Project-URL: Homepage, https://github.com/DeGeSim/caloutils
 Provides-Extra: dev
 Provides-Extra: doc
 
 =========
 caloutils
```

