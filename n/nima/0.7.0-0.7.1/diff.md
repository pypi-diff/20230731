# Comparing `tmp/nima-0.7.0.tar.gz` & `tmp/nima-0.7.1.tar.gz`

## Comparing `nima-0.7.0.tar` & `nima-0.7.1.tar`

### file list

```diff
@@ -1,56 +1,64 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nima-0.7.0/.codespellrc
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nima-0.7.0/.darglint
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 nima-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nima-0.7.0/.python-version
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nima-0.7.0/.readthedocs.yml
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 nima-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nima-0.7.0/bandit.yml
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 nima-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nima-0.7.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nima-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nima-0.7.0/docs/AUTHORS.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.7.0/docs/CHANGELOG.md -> ../CHANGELOG.md
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 nima-0.7.0/docs/conf.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 nima-0.7.0/docs/index.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima-0.7.0/docs/license.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nima-0.7.0/docs/reference.rst
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nima-0.7.0/docs/_static/.gitignore
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nima-0.7.0/docs/_static/custom.css
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nima-0.7.0/examples/holoview.ipynb.REMOVED.git-id
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/__init__.py
--rw-r--r--   0        0        0    15527 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/__main__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/generat.py
--rw-r--r--   0        0        0    32310 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/nima.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/py.typed
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nima-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nima-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nima-0.7.0/tests/test_generat.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 nima-0.7.0/tests/test_nima.py
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 nima-0.7.0/tests/test_scripts.py
--rw-r--r--   0        0        0  6538791 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/1b_c16_15.tif
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/test_flat0.tif
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/test_flat1.tif
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/test_flat2.tif
--rw-r--r--   0        0        0   746328 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15_dim.png
--rw-r--r--   0        0        0   101490 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15_meas.png
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/test_flat.tif
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/test_flat_gaussnorm.tif
--rw-r--r--   0        0        0   616620 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf
--rw-r--r--   0        0        0   469663 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf
--rw-r--r--   0        0        0   626676 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg.csv
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label1.csv
--rw-r--r--   0        0        0   179299 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label1_rcl.tif
--rw-r--r--   0        0        0   186357 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label1_rpH.tif
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label2.csv
--rw-r--r--   0        0        0    96791 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label2_rcl.tif
--rw-r--r--   0        0        0   114272 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label2_rpH.tif
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label3.csv
--rw-r--r--   0        0        0    54510 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label3_rcl.tif
--rw-r--r--   0        0        0    50655 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label3_rpH.tif
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 nima-0.7.0/.gitignore
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nima-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 nima-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nima-0.7.0/docs/README.md
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 nima-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nima-0.7.1/.codespellrc
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nima-0.7.1/.darglint
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 nima-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nima-0.7.1/.python-version
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nima-0.7.1/.readthedocs.yml
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 nima-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nima-0.7.1/bandit.yml
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 nima-0.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nima-0.7.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nima-0.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nima-0.7.1/docs/click.rst
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 nima-0.7.1/docs/conf.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 nima-0.7.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nima-0.7.1/docs/_static/.gitignore
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nima-0.7.1/docs/_static/custom.css
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nima-0.7.1/docs/api/api.rst
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nima-0.7.1/docs/api/generat.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nima-0.7.1/docs/api/nima.rst
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 nima-0.7.1/docs/references/contributing.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nima-0.7.1/docs/references/description.rst
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nima-0.7.1/docs/references/development.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 nima-0.7.1/docs/references/nima.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima-0.7.1/docs/references/references.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 nima-0.7.1/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nima-0.7.1/examples/holoview.ipynb.REMOVED.git-id
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nima-0.7.1/src/nima/__init__.py
+-rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 nima-0.7.1/src/nima/__main__.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 nima-0.7.1/src/nima/generat.py
+-rw-r--r--   0        0        0    32740 2020-02-02 00:00:00.000000 nima-0.7.1/src/nima/nima.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.7.1/src/nima/py.typed
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nima-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nima-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 nima-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 nima-0.7.1/tests/test_generat.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nima-0.7.1/tests/test_nima.py
+-rw-r--r--   0        0        0  6538791 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/1b_c16_15.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/test_flat0.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/test_flat1.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/test_flat2.tif
+-rw-r--r--   0        0        0   746328 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15_dim.png
+-rw-r--r--   0        0        0   101490 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15_meas.png
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/test_flat.tif
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/test_flat_gaussnorm.tif
+-rw-r--r--   0        0        0   616620 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf
+-rw-r--r--   0        0        0   469663 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf
+-rw-r--r--   0        0        0   626676 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/bg.csv
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label1.csv
+-rw-r--r--   0        0        0   179299 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label1_rcl.tif
+-rw-r--r--   0        0        0   186357 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label1_rpH.tif
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label2.csv
+-rw-r--r--   0        0        0    96791 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label2_rcl.tif
+-rw-r--r--   0        0        0   114272 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label2_rpH.tif
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label3.csv
+-rw-r--r--   0        0        0    54510 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label3_rcl.tif
+-rw-r--r--   0        0        0    50655 2020-02-02 00:00:00.000000 nima-0.7.1/tests/data/output/1b_c16_15/label3_rpH.tif
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nima-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nima-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nima-0.7.1/README.md
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nima-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 nima-0.7.1/PKG-INFO
```

### Comparing `nima-0.7.0/.pre-commit-config.yaml` & `nima-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/CHANGELOG.md` & `nima-0.7.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,36 @@
 # Changelog
 
+## v0.7.1 (2023-07-31)
+
+### Fix
+
+- **docs**: Update .gitignore
+
+### Docs
+
+- Update tfor API inclusion
+
+### Test
+
+- Rename script to cli
+
+### Build
+
+- **deps-dev**: bump commitizen from 3.5.3 to 3.5.4 (#249)
+- drop python 3.8 and 3.9
+- **deps-dev**: bump typeguard from 2.13.3 to 4.1.0
+- **deps-dev**: bump sphinx from 7.1.0 to 7.1.1 (#247)
+
+### Refactor
+
+- Follow also SIM code in ruff
+- After adding ANN code to ruff
+- Align code to ruff linter provisions
+
 ## v0.7.0 (2023-07-27)
 
 ### Feat
 
 - Add support for python 3.11
 - add generat
```

### Comparing `nima-0.7.0/.github/workflows/ci.yml` & `nima-0.7.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
       'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' ||
       'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python: ["3.8", "3.9", "3.10", "3.11"]
+        python: ["3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Cache pip
@@ -122,15 +122,15 @@
   tests:
     name: Tests Python-${{ matrix.python }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python: ["3.8", "3.9", "3.10", "3.11"]
+        python: ["3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Cache pip
         uses: actions/cache@v3
```

### Comparing `nima-0.7.0/.github/workflows/docs.yml` & `nima-0.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/docs/conf.py` & `nima-0.7.1/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,88 @@
-"""Sphinx configuration."""
-from datetime import datetime
+"""Configuration file for the Sphinx documentation builder."""
+
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Path setup --------------------------------------------------------------
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+#
+
+import sys
+from pathlib import Path
+
+sys.path.insert(0, str(Path("../..").resolve()))
+
+
+# -- Project information -----------------------------------------------------
 
 project = "nima"
+release = "0.7.1"
 author = "Daniele Arosio"
-copyright = f"{datetime.now().year}, {author}"
+copyright = f"2023, {author}"  # noqa A001
 html_static_path = ["_static"]
-# -- General configuration -----------------------------------------------------
+
+# -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "autodocsumm",
     "sphinx.ext.napoleon",
+    "sphinx_autodoc_typehints",
     "sphinx_click",
-    "myst_parser",
 ]
-autodoc_typehints = "description"
+
+
+# Napoleon settings to Default
+napoleon_use_ivar = False
 napoleon_include_init_with_doc = False
-napoleon_include_private_with_doc = True
+napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
-napoleon_use_rtype = False
+
+autodoc_default_options = {
+    "members": True,
+    "member-order": "bysource",
+    "undoc-members": False,
+    "autosummary": True,
+}
+
+autodoc_typehints = "description"
 
 # The suffix of source filenames.
 source_suffix = {
     ".rst": "restructuredtext",
     ".md": "markdown",
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
+latex_elements = {
+    "papersize": "a4paper",
+    "pointsize": "10pt",
+    # Additional preamble content
+    "preamble": r"""
+\usepackage[utf8]{inputenc}
+\usepackage{newunicodechar}
+\newunicodechar{█}{\rule{1ex}{1ex}}
+""",
+}
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nima-0.7.0/src/nima/__main__.py` & `nima-0.7.1/src/nima/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Command-line interface."""
-from __future__ import annotations
 
 import os
-import sys
 import zipfile
 from pathlib import Path
+from typing import Any
 
 import click
 import dask.array as da
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 import sigfig  # type: ignore
@@ -17,14 +16,16 @@
 from dask.distributed import Client, progress
 from matplotlib.backends import backend_pdf  # type: ignore
 from scipy import ndimage  # type: ignore
 
 from nima import nima
 from nima.nima import ImArray
 
+AXES_LENGTH_2D = 2
+
 
 @click.command()
 @click.version_option()
 @click.option("--silent", is_flag=True, help="Do not print; verbose=0.")
 @click.option(
     "-o",
     "--output",
@@ -34,16 +35,20 @@
 )
 @click.option(
     "--hotpixels",
     is_flag=True,
     default=False,
     help="Median filter (rad=0.5) to remove hotpixels.",
 )
-@click.option("-f", "--flat", type=str, help="Dark for shading correction.")
-@click.option("-d", "--dark", type=str, help="Flat for shading correction.")
+@click.option(
+    "-f", "--flat", "flat_f", type=str, default="", help="Dark for shading correction."
+)
+@click.option(
+    "-d", "--dark", "dark_f", type=str, default="", help="Flat for shading correction."
+)
 @click.option(
     "--bg-method",
     type=click.Choice(
         ["li_adaptive", "entropy", "arcsinh", "adaptive", "li_li"], case_sensitive=False
     ),
     default="li_adaptive",
     prompt_required=False,
@@ -105,43 +110,41 @@
 )
 @click.option(
     "--channels-ph",
     type=(str, str),
     default=("G", "C"),
     help="Channels for pH ratio [default:G/C].",
 )
-# # TODO: @click.argument("tiffstk", type=click.File("r"))
 @click.argument("tiffstk", type=click.Path(path_type=Path))
-# @click.argument("channels", type=list[str], default=["G", "R", "C"])
 @click.argument("channels", type=str, nargs=-1)
-def main(  # type: ignore
-    silent,
-    output,
-    hotpixels,
-    flat,
-    dark,
-    fg_method,
-    min_size,
-    clear_border,
-    wiener,
-    watershed,
-    randomwalk,
-    bg_method,
-    bg_downscale,
-    bg_radius,
-    bg_adaptive_radius,
-    bg_percentile,
-    bg_percentile_filter,
-    image_ratios,
-    ratio_median_radii,
-    channels_cl,
-    channels_ph,
-    tiffstk,
-    channels,
-):
+def main(  # noqa: C901"
+    silent: bool | None,
+    output: Path,
+    hotpixels: bool,
+    flat_f: str,
+    dark_f: str,
+    bg_method: str,
+    bg_downscale: tuple[int, int] | None,
+    bg_radius: float | None,
+    bg_adaptive_radius: float | None,
+    bg_percentile: float | None,
+    bg_percentile_filter: float | None,
+    fg_method: str,
+    min_size: float | None,
+    clear_border: bool | None,
+    wiener: bool | None,
+    watershed: bool | None,
+    randomwalk: bool | None,
+    image_ratios: bool,
+    ratio_median_radii: str | None,
+    channels_cl: tuple[str, str],
+    channels_ph: tuple[str, str],
+    tiffstk: Path,
+    channels: tuple[str, ...],
+) -> None:
     """Analyze multichannel (default:["G", "R", "C"]) tiff time-lapse stack.
 
     TIFFSTK  :  Image file.
 
     CHANNELS :  Channel names.
 
     Save:
@@ -158,19 +161,20 @@
     channels = ("G", "R", "C") if len(channels) == 0 else channels
     click.echo(channels)
     d_im, _, t = nima.read_tiff(tiffstk, channels)
     if not silent:
         print("  Times: ", t)
     if hotpixels:
         d_im = nima.d_median(d_im)
-    if flat:
+    if flat_f:
         # XXX: this is imperfect: dark must be present of flat
-        dark, _, _ = nima.read_tiff(dark, channels)
-        flat, _, _ = nima.read_tiff(flat, channels)
+        dark, _, _ = nima.read_tiff(Path(dark_f), channels)
+        flat, _, _ = nima.read_tiff(Path(flat_f), channels)
         d_im = nima.d_shading(d_im, dark, flat, clip=True)
+    kwargs_bg: dict[str, Any]
     kwargs_bg = {"kind": bg_method}
     if bg_downscale:
         kwargs_bg["downscale"] = bg_downscale
     if bg_radius:
         kwargs_bg["radius"] = bg_radius
     if bg_adaptive_radius:
         kwargs_bg["adaptive_radius"] = bg_adaptive_radius
@@ -178,41 +182,42 @@
         kwargs_bg["perc"] = bg_percentile
     if bg_percentile_filter:
         kwargs_bg["arcsinh_perc"] = bg_percentile_filter
     click.echo(kwargs_bg)
     d_im_bg, bgs, ff, _bgv = nima.d_bg(d_im, **kwargs_bg)  # clip=True
     print(bgs)
 
+    kwargs_mask_label: dict[str, Any]
     kwargs_mask_label = {"channels": channels, "threshold_method": fg_method}
     if min_size:
         kwargs_mask_label["min_size"] = min_size
     if clear_border:
         kwargs_mask_label["clear_border"] = True
     if wiener:
         kwargs_mask_label["wiener"] = True
     if watershed:
         kwargs_mask_label["watershed"] = True
     if randomwalk:
         kwargs_mask_label["randomwalk"] = True
     click.secho(kwargs_mask_label)
     nima.d_mask_label(d_im_bg, **kwargs_mask_label)
-    kwargs_meas_props = {"channels": channels}
+    kwargs_meas_props: dict[str, Any] = {"channels": channels}
     kwargs_meas_props["ratios_from_image"] = image_ratios
     if ratio_median_radii:
         kwargs_meas_props["radii"] = tuple(
             int(r) for r in ratio_median_radii.split(",")
         )
     click.secho(kwargs_meas_props)
     meas, pr = nima.d_meas_props(
         d_im_bg, channels_cl=channels_cl, channels_ph=channels_ph, **kwargs_meas_props
     )
-    #     # output for bg
-    bname = tiffstk.with_suffix("").name
+    # output for bg
+    bname_str = tiffstk.with_suffix("").name
     output.mkdir(exist_ok=True)
-    bname = output / bname
+    bname = output / bname_str
     if not bname.exists():
         bname.mkdir()
     for ch, llf in ff.items():
         pp = backend_pdf.PdfPages(
             bname / Path("bg-" + ch + "-" + bg_method).with_suffix(".pdf")
         )
         for lf in llf:
@@ -227,15 +232,14 @@
     f.savefig(bname.with_name(bname.name + "_meas.png"))
     ##
     # show all channels and labels only.
     d = {ch: d_im_bg[ch] for ch in channels}
     d["labels"] = d_im_bg["labels"]
     f = nima.d_show(d, cmap=mpl.cm.inferno_r)  # type: ignore
     f.savefig(bname.with_name(bname.name + "_dim.png"))
-    ##
     # meas csv
     for k, df in meas.items():
         column_order = [
             "C",
             "G",
             "R",
             "area",
@@ -243,16 +247,15 @@
             "equivalent_diameter",
             "r_cl",
             "r_pH",
             "r_cl_median",
             "r_pH_median",
         ]
         df[column_order].to_csv(bname / Path("label" + str(k)).with_suffix(".csv"))
-    # ##
-    # labelX_{rcl,rpH}.tif ### require r_cl and r_pH present in d_im
+    # # XXX: labelX_{rcl,rpH}.tif ### require r_cl and r_pH present in d_im
     objs = ndimage.find_objects(d_im_bg["labels"])
     for n, o in enumerate(objs):
         name = bname / Path("label" + str(n + 1) + "_rcl").with_suffix(".tif")
         tifffile.imwrite(
             name, d_im_bg["r_cl"][o], compression="lzma", photometric="minisblack"
         )
         name = bname / Path("label" + str(n + 1) + "_rpH").with_suffix(".tif")
@@ -301,30 +304,27 @@
     else:
         store = tifffile.imread(fpath)
     click.secho("Bias image-stack shape: " + str(store.shape), fg="green")
     bias = np.median(store, axis=0)
     err = np.std(store, axis=0)
     # hotpixels
     hpix = nima.hotpixels(bias)
-    if ctx.obj["output"]:
-        output = ctx.obj["output"]
-    else:
-        output = fpath.with_suffix(".png")
+    output = ctx.obj["output"] if ctx.obj["output"] else fpath.with_suffix(".png")
     if not hpix.empty:
         hpix.to_csv(output.with_suffix(".csv"), index=False)
         # FIXME hpix.y is a pd.Series[int]; it could be cast into NDArray[int]
         # TODO: if any of x y is out of the border ignore them
         nima.correct_hotpixel(err, hpix.y, hpix.x)  # type: ignore
     p25, p50, p75 = np.percentile(err.ravel(), [25, 50, 75])
     err_str = sigfig.round(p50, p75 - p25)
     click.secho("Estimated read noise: " + err_str)
     tifffile.imwrite(output.with_suffix(".tiff"), bias)
     # Output summary graphics.
     title = os.fspath(output.with_suffix("").name)
-    if bias.ndim == 2:
+    if bias.ndim == AXES_LENGTH_2D:
         plt_img_profiles(bias, title, output, hpix)
         plt_img_profiles(
             err,
             "".join(("[", title[:9], "] $\\sigma_{read} = $", err_str)),
             output.with_suffix(".err.png"),
         )
     else:
@@ -340,37 +340,35 @@
 def dark(ctx: click.Context, fpath: Path, bias: Path, time: float) -> None:
     """Compute DARK.
 
     FPATH: the bias stack (Light Off - Long acquisition time).
 
 
     """
+    dark_thr = 4.5
     store = tifffile.imread(fpath)
     click.secho("Dark image-stack shape: " + str(store.shape), fg="green")
     dark = np.median(store, axis=0)
-    if ctx.obj["output"]:
-        output = ctx.obj["output"]
-    else:
-        output = fpath.with_suffix(".png")
+    output = ctx.obj["output"] if ctx.obj["output"] else fpath.with_suffix(".png")
     # Output summary graphics.
     title = os.fspath(output.with_suffix("").name)
     if bias is not None:
         bias = tifffile.imread(bias)
         dark = dark - bias
     if time:
         dark /= time
     plt_img_profiles(dark, title, output)
-    print(np.where(dark > 4.5))
+    print(np.where(dark > dark_thr))
 
 
 @bima.command()
 @click.pass_context
 @click.option("--bias", type=click.Path(path_type=Path))
 @click.argument("globpath", type=str)
-def mflat(ctx: click.Context, globpath: str, bias: Path) -> None:
+def mflat(ctx: click.Context, globpath: str, bias: Path | None) -> None:
     """Flat from a collection of (.tif) files."""
     image_sequence = tifffile.TiffSequence(globpath)
     axes_n_shape = " ".join((str(image_sequence.axes), str(image_sequence.shape)))
     click.secho(axes_n_shape, fg="green")
     store = image_sequence.aszarr()
     Client()  # type: ignore
     f = da.mean(da.from_zarr(store).rechunk(), axis=0)  # type: ignore
@@ -393,18 +391,15 @@
 @click.argument("fpath", type=click.Path(path_type=Path))
 def flat(ctx: click.Context, fpath: Path, bias: Path) -> None:
     """Flat from (.tf8) file."""
     store = tifffile.imread(fpath, aszarr=True)
     f = da.mean(da.from_zarr(store).rechunk(), axis=0)  # type: ignore
     with ProgressBar():  # type: ignore
         tprojection = f.compute()
-    if ctx.obj["output"]:
-        output = ctx.obj["output"]
-    else:
-        output = fpath.with_suffix(".tiff")
+    output = ctx.obj["output"] if ctx.obj["output"] else fpath.with_suffix(".tiff")
     if bias is not None:
         bias = tifffile.imread(bias)
     _output_flat(output, tprojection, bias)
 
 
 def _output_flat(
     output: Path, tprojection: ImArray, bias: ImArray | None = None
@@ -421,19 +416,15 @@
         Base for output file paths.
     tprojection : ImArray
         Raw flat array (mean of frames).
     bias : ImArray
         Bias frame.
 
     """
-    if sys.version_info >= (3, 9):
-        tifffile.imwrite(output.with_stem("-".join([output.stem, "raw"])), tprojection)
-    else:
-        rename = "-".join([output.stem, "raw"]) + output.suffix
-        tifffile.imwrite(output.with_name(rename), tprojection)
+    tifffile.imwrite(output.with_stem("-".join([output.stem, "raw"])), tprojection)
     if bias is None:
         flat = ndimage.gaussian_filter(tprojection, sigma=100)
     else:
         flat = ndimage.gaussian_filter(tprojection + 20 - bias, sigma=100)  # FIXME
     flat /= flat.mean()
     tifffile.imwrite(output, flat)
     title = os.fspath(output.with_suffix("").name)
@@ -442,27 +433,24 @@
 
 @bima.command()
 @click.pass_context
 @click.argument("fpath", type=click.Path(exists=True, path_type=Path))
 def plot(ctx: click.Context, fpath: Path) -> None:
     """Plot profiles of 2D (Bias-Flat) image."""
     img = tifffile.imread(fpath)
-    if ctx.obj["output"]:
-        output = ctx.obj["output"]
-    else:
-        output = fpath.with_suffix(".png")
+    output = ctx.obj["output"] if ctx.obj["output"] else fpath.with_suffix(".png")
     title = os.fspath(output.with_suffix("").name)
     plt_img_profiles(img, title, output)
 
 
 def plt_img_profiles(
     img: ImArray, title: str, output: Path, hpix: pd.DataFrame | None = None
 ) -> None:
     """Compute and save image profiles graphics."""
-    if img.ndim == 2:
+    if img.ndim == AXES_LENGTH_2D:
         f = nima.plt_img_profile(img, title=title, hpix=hpix)
         f.savefig(output.with_suffix(".png"), dpi=250, facecolor="w")
         # mark f = nima.plt_img_profile_2(img, title=title)
         # mark f.savefig(output.with_suffix(".2.png"), dpi=250, facecolor="w")
     else:
         for i in range(img.shape[0]):
             title += f" C:{i}"
```

### Comparing `nima-0.7.0/src/nima/generat.py` & `nima-0.7.1/src/nima/generat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Generate mock images."""
 
-from __future__ import annotations
-
 import warnings
 
 import numpy as np
 import numpy.typing as npt
 
 
 def gen_bias(nrows: int = 128, ncols: int = 128) -> npt.NDArray[np.float_]:
@@ -78,17 +76,17 @@
     noise_sd: float = 1,
 ) -> npt.NDArray[np.float_]:  # pylint: disable=too-many-arguments
     """Simulate an acquired frame [bias + noise + dark + flat * (sky + obj)]."""
     (nrows, ncols) = objs.shape
     if bias is None:
         bias = gen_bias(nrows, ncols)
     elif bias.shape != (nrows, ncols):
-        warnings.warn("Shape mismatch. Generate Bias...", UserWarning)
+        warnings.warn("Shape mismatch. Generate Bias...", UserWarning, stacklevel=2)
         bias = gen_bias(nrows, ncols)
     if flat is None:
         flat = gen_flat(nrows, ncols)
     elif flat.shape != (nrows, ncols):
-        warnings.warn("Shape mismatch. Generate Flat...", UserWarning)
+        warnings.warn("Shape mismatch. Generate Flat...", UserWarning, stacklevel=2)
         flat = gen_flat(nrows, ncols)
     noise = np.random.normal(0, noise_sd, size=(nrows, ncols))
     img = bias + flat * (sky + objs) + dark + noise
     return img  # type: ignore
```

### Comparing `nima-0.7.0/src/nima/nima.py` & `nima-0.7.1/src/nima/nima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Main library module.
 
 Contains functions for the analysis of multichannel timelapse images. It can
 be used to apply dark, flat correction; segment cells from bg; label cells;
 obtain statistics for each label; compute ratio and ratio images between
 channels.
 """
-from __future__ import annotations
 
 from collections import defaultdict
+from collections.abc import Sequence
 from itertools import chain
 from pathlib import Path
-from typing import Any, Sequence, TypeVar
+from typing import Any, TypeVar
 
 import matplotlib as mpl
 import matplotlib.cm
 import matplotlib.colors  # type: ignore
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -25,15 +25,20 @@
 import tifffile  # type: ignore
 from numpy.typing import NDArray
 from scipy import ndimage, signal  # type: ignore
 from skimage import filters
 from skimage.morphology import disk  # type: ignore
 
 ImArray = TypeVar("ImArray", NDArray[np.int_], NDArray[np.float_], NDArray[np.bool_])
-
+Im = TypeVar("Im", NDArray[np.int_], NDArray[np.float_])
+# MAYBE: DIm eq TypeVar("DIm", Dict[str, Im])
+Kwargs = dict[str, str | int | float | bool | None]
+AXES_LENGTH_4D = 4
+AXES_LENGTH_3D = 3
+AXES_LENGTH_2D = 2
 # TODO: https://towardsdatascience.com/creating-custom-plotting-functions-with-matplotlib-1f4b8eba6aa1
 
 
 def myhist(
     im: ImArray,
     bins: int = 60,
     log: bool = False,
@@ -82,37 +87,34 @@
 
     """
     n_channels = len(channels)
     with tifffile.TiffFile(fp) as tif:
         im = tif.asarray()
         axes = tif.series[0].axes
     idx = axes.rfind("T")
-    if idx >= 0:
-        n_times = im.shape[idx]
-    else:
-        n_times = 1
+    n_times = im.shape[idx] if idx >= 0 else 1
     if im.shape[axes.rfind("C")] % n_channels:
         raise Exception("n_channel mismatch total length of tif sequence")
     else:
         d_im = {}
         for i, ch in enumerate(channels):
             # FIXME: must be 'TCYX' or 'ZCYX'
-            if len(axes) == 4:
+            if len(axes) == AXES_LENGTH_4D:
                 d_im[ch] = im[:, i]  # im[i::n_channels]
-            elif len(axes) == 3:
+            elif len(axes) == AXES_LENGTH_3D:
                 d_im[ch] = im[np.newaxis, i]
         print(d_im["G"].shape)
         return d_im, n_channels, n_times
 
 
-def d_show(d_im: dict[str, ImArray], **kws: Any) -> plt.Figure:
+def d_show(d_im: dict[str, ImArray], **kws: Any) -> plt.Figure:  # noqa: ANN401
     """Imshow for dictionary of image (d_im). Support plt.imshow kws."""
     max_rows = 9
     n_channels = len(d_im.keys())
-    first_channel = d_im[list(d_im.keys())[0]]
+    first_channel = d_im[next(iter(d_im.keys()))]
     n_times = len(first_channel)
     if n_times <= max_rows:
         rng = range(n_times)
         n_rows = n_times
     else:
         step = np.ceil(n_times / max_rows).astype(int)
         rng = range(0, n_times, step)
@@ -149,18 +151,18 @@
     d_im : dict of images
         preserve dtype of input
 
     """
     d_out = {}
     for k, im in d_im.items():
         disk = skimage.morphology.disk(1)
-        if im.ndim == 3:
+        if im.ndim == AXES_LENGTH_3D:
             sel = np.conj((np.zeros((3, 3)), disk, np.zeros((3, 3))))
             d_out[k] = ndimage.median_filter(im, footprint=sel)
-        elif im.ndim == 2:
+        elif im.ndim == AXES_LENGTH_2D:
             d_out[k] = ndimage.median_filter(im, footprint=disk)
         else:
             raise Exception("Only for single image or stack (3D).")
     return d_out
 
 
 def d_shading(
@@ -195,45 +197,45 @@
 
     """
     # TODO inplace=True tosave memory
     # assertion type(dark) == np.ndarray or dark.keys() == d_im.keys(), raise_msg
     # assertion type(flat) == np.ndarray or flat.keys() == d_im.keys(),
     # raise_msg will be replaced by type checking.
     d_cor = {}
-    for k in d_im.keys():
+    for k in d_im:
         d_cor[k] = d_im[k].astype(float)
         if type(dark) == dict:
             d_cor[k] -= dark[k]
         else:
             d_cor[k] -= dark  # numpy.ndarray
         if type(flat) == dict:
             d_cor[k] /= flat[k]
         else:
             d_cor[k] /= flat  # numpy.ndarray
     if clip:
-        for k in d_cor.keys():
+        for k in d_cor:
             d_cor[k] = d_cor[k].clip(0)
     return d_cor
 
 
-def bg(
-    im: NDArray[Any],
+def bg(  # noqa: C901
+    im: Im,
     kind: str = "arcsinh",
     perc: float = 10.0,
     radius: int | None = 10,
     adaptive_radius: int | None = None,
     arcsinh_perc: int | None = 80,
-) -> tuple[float, ImArray, list[Any]]:
+) -> tuple[float, NDArray[np.int_] | NDArray[np.float_], list[plt.Figure]]:
     """Bg segmentation.
 
     Return median, whole vector, figures (in a [list])
 
     Parameters
     ----------
-    im
+    im: Im
         An image stack.
     kind : str
         Method {'arcsinh', 'entropy', 'adaptive', 'li_adaptive', 'li_li'} used for the
         segmentation.
     perc : float
         Perc % of max-min (default=10) for thresholding *entropy* and *arcsinh*
         methods.
@@ -256,20 +258,21 @@
         List of fig(s). Only entropy and arcsinh methods have 2 elements.
 
     """
     if adaptive_radius is None:
         adaptive_radius = int(im.shape[1] / 2)
         if adaptive_radius % 2 == 0:  # sk >0.12.0 check for even value
             adaptive_radius += 1
-    if (perc < 0.0) or (perc > 100.0):
+    min_perc, max_perc = 0.0, 100.0
+    if (perc < min_perc) or (perc > max_perc):
         raise Exception("perc must be in [0, 100] range")
     else:
         perc /= 100
     lim_ = False
-    m = None
+    m = np.ones_like(im)  # default value for m; instead of m = None
     if kind == "arcsinh":
         lim = np.arcsinh(im)
         lim = ndimage.percentile_filter(lim, arcsinh_perc, size=radius)
         lim_ = True
         title: Any = radius, perc
         thr = (1 - perc) * lim.min() + perc * lim.max()
         m = lim < thr
@@ -366,39 +369,36 @@
 
 
 # TODO: add new bg/fg segmentation based on conditional probability but
 # working with dask arrays.
 
 
 def d_bg(
-    d_im: dict[str, ImArray],
+    d_im: dict[str, Im],
     downscale: tuple[int, int] | None = None,
     kind: str = "li_adaptive",
     clip: bool = True,
-    **kw: dict[str, Any],
 ) -> tuple[
-    dict[str, ImArray],
+    dict[str, Im],
     pd.DataFrame,
     dict[str, list[list[plt.Figure]]],
-    dict[str, list[Any]],
+    dict[str, list[NDArray[np.int_] | NDArray[np.float_]]],
 ]:
     """Bg segmentation for d_im.
 
     Parameters
     ----------
     d_im : d_im
         desc
     downscale : {None, tupla}
         Tupla, x, y are downscale factors for rows, cols.
     kind : str
         Bg method among {'li_adaptive', 'arcsinh', 'entropy', 'adaptive', 'li_li'}.
     clip : bool
         Boolean (default=True) for clipping values >=0.
-    kw : dict
-        Keywords passed to bg() function.
 
     Returns
     -------
     d_cor : d_im
         Dictionary of images subtracted for the estimated bg.
     bgs : pd.DataFrame
         Median of the estimated bg; columns for channels and index for time
@@ -410,27 +410,28 @@
         point) of list of values.
 
     """
     d_bg = defaultdict(list)
     d_bg_values = defaultdict(list)
     d_cor = defaultdict(list)
     d_fig = defaultdict(list)
-    dd_cor: dict[str, NDArray[Any]] = {}
-    for k in d_im.keys():
+    dd_cor: dict[str, Im] = {}
+    for k in d_im:
         for t, im in enumerate(d_im[k]):
+            im_for_bg = im
             if downscale:
-                im = skimage.transform.downscale_local_mean(im, downscale)
-            med, v, ff = bg(im, kind=kind, perc=10)
+                im_for_bg = skimage.transform.downscale_local_mean(im, downscale)
+            med, v, ff = bg(im_for_bg, kind=kind, perc=10)
             d_bg[k].append(med)
             d_bg_values[k].append(v)
             d_cor[k].append(d_im[k][t] - med)
             d_fig[k].append(ff)
         dd_cor[k] = np.array(d_cor[k])
     if clip:
-        for k in d_cor.keys():
+        for k in d_cor:
             dd_cor[k] = dd_cor[k].clip(0)
     bgs = pd.DataFrame({k: np.array(v) for k, v in d_bg.items()})
     return dd_cor, bgs, d_fig, d_bg_values
 
 
 def d_mask_label(
     d_im: dict[str, ImArray],
@@ -521,15 +522,15 @@
         )
         max_diameter = pr[0].equivalent_diameter
         size = max_diameter * 2.20
         for p in pr[1:]:
             max_diameter = max(max_diameter, p.equivalent_diameter)
         print(max_diameter)
         # for time, (d, l) in enumerate(zip(ga_wiener, labels)):
-        for time, (d, lbl) in enumerate(zip(distance, labels)):
+        for time, (d, lbl) in enumerate(zip(distance, labels, strict=True)):
             local_maxi = skimage.feature.peak_local_max(
                 d,
                 labels=lbl,
                 footprint=np.ones((size, size)),
                 min_distance=size,
                 indices=False,
                 exclude_border=False,
@@ -579,28 +580,29 @@
 
     """
     with np.errstate(divide="ignore", invalid="ignore"):
         # 0/0 and num/0 can both happen.
         ratio = np.array(d_im[channels[0]] / d_im[channels[1]], dtype=(float))
     for i, r in enumerate(ratio):
         np.nan_to_num(r, copy=False, posinf=0, neginf=0)
+        filtered_r = r
         for radius in radii:
-            r = ndimage.median_filter(r, radius)
-        ratio[i] = r * d_im["mask"][i]
+            filtered_r = ndimage.median_filter(filtered_r, radius)
+        ratio[i] = filtered_r * d_im["mask"][i]
     d_im[name] = ratio
 
 
 def d_meas_props(
-    d_im: dict[str, ImArray],
+    d_im: dict[str, Im],
     channels: Sequence[str] = ("C", "G", "R"),
     channels_cl: tuple[str, str] = ("C", "R"),
     channels_ph: tuple[str, str] = ("G", "C"),
     ratios_from_image: bool | None = True,
     radii: tuple[int, int] | None = None,
-) -> tuple[dict[np.int32, pd.DataFrame], dict[str, list[Any]]]:
+) -> tuple[dict[np.int32, pd.DataFrame], dict[str, list[list[Any]]]]:
     """Calculate pH and cl ratios and labelprops.
 
     Parameters
     ----------
     d_im : d_im
         desc
     channels : list of string
@@ -623,65 +625,65 @@
         DataFrame columns are: mean intensity of all channels,
         'equivalent_diameter', 'eccentricity', 'area', ratios from the mean
         intensities and optionally ratios from ratio-image.
     pr : dict of list of list
         For each channel: {'channel': [props]} i.e. {'channel': [time][label]}.
 
     """
-    pr: dict[str, list[Any]] = defaultdict(list)
+    pr: dict[str, list[list[Any]]] = defaultdict(list)
     for ch in channels:
         pr[ch] = []
         for time, label_im in enumerate(d_im["labels"]):
             im = d_im[ch][time]
             props = skimage.measure.regionprops(label_im, intensity_image=im)
             pr[ch].append(props)
     meas = {}
     # labels are 3D and "0" is always label for background
     labels = np.unique(d_im["labels"])[1:]
-    for label in labels:
+    for lbl in labels:
         idx = []
         d = defaultdict(list)
         for time, props in enumerate(pr[channels[0]]):
             try:
-                i_label = [prop.label == label for prop in props].index(True)
+                i_label = [prop.label == lbl for prop in props].index(True)
                 prop_ch0 = props[i_label]
                 idx.append(time)
                 d["equivalent_diameter"].append(prop_ch0.equivalent_diameter)
                 d["eccentricity"].append(prop_ch0.eccentricity)
                 d["area"].append(prop_ch0.area)
                 for ch in pr:
                     d[ch].append(pr[ch][time][i_label].mean_intensity)
             except ValueError:
                 pass  # label is absent in this timepoint
-        df = pd.DataFrame({k: np.array(v) for k, v in d.items()}, index=idx)
-        df["r_cl"] = df[channels_cl[0]] / df[channels_cl[1]]
-        df["r_pH"] = df[channels_ph[0]] / df[channels_ph[1]]
-        meas[label] = df
+        res_df = pd.DataFrame({k: np.array(v) for k, v in d.items()}, index=idx)
+        res_df["r_cl"] = res_df[channels_cl[0]] / res_df[channels_cl[1]]
+        res_df["r_pH"] = res_df[channels_ph[0]] / res_df[channels_ph[1]]
+        meas[lbl] = res_df
     if ratios_from_image:
         kwargs = {}
         if radii:
             kwargs["radii"] = radii
         d_ratio(d_im, "r_cl", channels=channels_cl, **kwargs)
         d_ratio(d_im, "r_pH", channels=channels_ph, **kwargs)
         r_ph = []
         r_cl = []
-        for time, (ph, cl) in enumerate(zip(d_im["r_pH"], d_im["r_cl"])):
+        for time, (ph, cl) in enumerate(zip(d_im["r_pH"], d_im["r_cl"], strict=True)):
             r_ph.append(ndimage.median(ph, d_im["labels"][time], index=labels))
             r_cl.append(ndimage.median(cl, d_im["labels"][time], index=labels))
         ratios_ph = np.array(r_ph)
         ratios_cl = np.array(r_cl)
-        for label in meas:
-            df = pd.DataFrame(
+        for lbl in meas:
+            res_df = pd.DataFrame(
                 {
-                    "r_pH_median": ratios_ph[:, label - 1],
-                    "r_cl_median": ratios_cl[:, label - 1],
+                    "r_pH_median": ratios_ph[:, lbl - 1],
+                    "r_cl_median": ratios_cl[:, lbl - 1],
                 }
             )
             # concat only on index that are present in both
-            meas[label] = pd.concat([meas[label], df], axis=1, join="inner")
+            meas[lbl] = pd.concat([meas[lbl], res_df], axis=1, join="inner")
     return meas, pr
 
 
 def d_plot_meas(
     bgs: pd.DataFrame, meas: dict[np.int32, pd.DataFrame], channels: Sequence[str]
 ) -> plt.Figure:
     """Plot meas object.
@@ -811,15 +813,14 @@
 
     def img_hist(
         im: ImArray,
         ax: plt.Axes,
         ax_px: plt.Axes,
         ax_py: plt.Axes,
         axh: plt.Axes,
-        axc: plt.Axes,
         vmin: float | None = None,
         vmax: float | None = None,
     ) -> mpl.image.AxesImage:
         ax_px.tick_params(  # type: ignore
             axis="x", labelbottom=False, labeltop=True, top=True
         )
         ax_py.tick_params(  # type: ignore
@@ -856,19 +857,18 @@
             log=True,
             alpha=0.6,
             lw=4,
             histtype="bar",
         )
         return img
 
-    if hpix is not None:
-        if not hpix.empty:
-            ax.plot(hpix["x"], hpix["y"], "+", mfc="gray", mew=2, ms=14)
+    if hpix is not None and not hpix.empty:
+        ax.plot(hpix["x"], hpix["y"], "+", mfc="gray", mew=2, ms=14)
 
-    im2c = img_hist(img, ax, ax_px, ax_py, ax_hist, ax_cm, vmin, vmax)
+    im2c = img_hist(img, ax, ax_px, ax_py, ax_hist, vmin, vmax)
     ax_cm.axis("off")
     fig.colorbar(  # type: ignore
         im2c, ax=ax_cm, fraction=0.99, shrink=0.99, aspect=4, orientation="horizontal"
     )
     return fig
 
 
@@ -945,17 +945,17 @@
         m_ave = np.ma.masked_array(bias, m).mean()
         m_std = np.ma.masked_array(bias, m).std()
         m = bias > m_ave + n_sd * m_std
         if n_hpix == m.sum():
             break
         n_hpix = m.sum()
     w = np.where(m)
-    df = pd.DataFrame({"y": w[0], "x": w[1]})
-    df = df.assign(val=lambda row: bias[row.y, row.x])
-    return df
+    hpix_df = pd.DataFrame({"y": w[0], "x": w[1]})
+    hpix_df = hpix_df.assign(val=lambda row: bias[row.y, row.x])
+    return hpix_df
 
 
 def correct_hotpixel(
     img: ImArray, y: int | NDArray[np.int_], x: int | NDArray[np.int_]
 ) -> None:
     """Correct hot pixels in a frame.
 
@@ -968,14 +968,14 @@
         Frame (2D) image.
     y : int | list(int)
         y-coordinate(s).
     x : int | list(int)
         x-coordinate(s).
 
     """
-    if img.ndim == 2:
+    if img.ndim == AXES_LENGTH_2D:
         v1 = img[y - 1, x]
         v2 = img[y + 1, x]
         v3 = img[y, x - 1]
         v4 = img[y, x + 1]
         correct = np.median([v1, v2, v3, v4])
         img[y, x] = correct
```

### Comparing `nima-0.7.0/tests/test_generat.py` & `nima-0.7.1/tests/test_generat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for generat module."""
 
 import numpy as np
 import pytest
+from numpy import typing as npt
 
 from nima import generat
 
 
 def test_bias() -> None:
     """Test generation of bias."""
     bias = generat.gen_bias(nrows=3, ncols=128)
@@ -17,35 +18,40 @@
     """Test generation of bias."""
     flat = generat.gen_flat(nrows=10, ncols=10)
     assert np.mean(flat) == 1.0
 
 
 def test_flat_shape() -> None:
     """Test nrows and ncols."""
-    object = generat.gen_flat(nrows=12)
-    assert object.shape == (12, 128)
+    obj = generat.gen_flat(nrows=12)
+    assert obj.shape == (12, 128)
 
 
 def test_object() -> None:
     """Test generation of a single cell object in a frame."""
     np.random.seed(111)
-    object = generat.gen_object(nrows=10, ncols=10, min_radius=2, max_radius=5)
-    assert object[4, 4]
-    assert not object[8, 8]
+    obj = generat.gen_object(nrows=10, ncols=10, min_radius=2, max_radius=5)
+    assert obj[4, 4]
+    assert not obj[8, 8]
 
 
 def test_object_shape() -> None:
     """Test nrows and ncols."""
-    object = generat.gen_object(nrows=12)
-    assert object.shape == (12, 128)
+    obj = generat.gen_object(nrows=12)
+    assert obj.shape == (12, 128)
 
 
 class TestFrame:
     """Test simulation of an acquired frame."""
 
+    bias: npt.NDArray[np.float_]
+    flat: npt.NDArray[np.float_]
+    objs: npt.NDArray[np.float_]
+    frame: npt.NDArray[np.float_]
+
     def setup_class(self) -> None:
         """Read test data."""
         self.bias = generat.gen_bias(ncols=6)
         self.flat = generat.gen_flat(ncols=4)
         np.random.seed(121)
         self.objs = generat.gen_objs(ncols=64)
         self.frame = generat.gen_frame(self.objs)
```

### Comparing `nima-0.7.0/tests/test_nima.py` & `nima-0.7.1/tests/test_nima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests for nima module."""
-import os
+
+from pathlib import Path
 
 import numpy as np
 import tifffile as tff  # type: ignore
 from numpy.testing import assert_array_equal
 
 from nima import nima
 
@@ -85,17 +86,15 @@
 
 def test_plot_img_profile() -> None:
     """Plot summary graphics for Bias-Flat images.
 
     Test both lines (whole frame and central region) along x (axis=0).
 
     """
-    sample_flat_image = os.path.join(
-        "tests", "data", "output", "test_flat_gaussnorm.tif"
-    )
+    sample_flat_image = Path("tests") / "data" / "output" / "test_flat_gaussnorm.tif"
     img = tff.imread(sample_flat_image)
     f = nima.plt_img_profile(img)
     _, y_plot = f.get_axes()[1].lines[0].get_xydata().T  # type: ignore
     ydata = np.array([1.00000001, 0.99999999, 1.00000002, 1.0, 0.99999999])
     np.testing.assert_allclose(y_plot, ydata)
     _, y_plot = f.get_axes()[1].lines[1].get_xydata().T  # type: ignore
     ydata = np.array([1.0, 0.99999997, 1.0, 0.99999998, 0.99999997])
```

### Comparing `nima-0.7.0/tests/test_scripts.py` & `nima-0.7.1/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 """Tests for nima script."""
-import os
 from pathlib import Path
-from typing import Any, Tuple
 
 import numpy as np
 import pandas as pd
 import pytest
 import skimage.io  # type: ignore
 import skimage.measure  # type: ignore
 import tifffile as tff  # type: ignore
-from click.testing import CliRunner
+from click.testing import CliRunner, Result
 from matplotlib.testing.compare import compare_images  # type: ignore
 from matplotlib.testing.exceptions import ImageComparisonFailure  # type: ignore
 
-from nima import __main__
+from nima.__main__ import bima, main
 
+# tests path
+tpath = Path(__file__).parent
 # test data: (rootname, times)
-rootnames = [(Path("1b_c16_15"), 4)]
+rootnames = [("1b_c16_15", 4)]
+ResultFolder = tuple[Path, tuple[str, int], Result]
 
 
 @pytest.fixture(scope="module", params=rootnames)
-def result_folder(tmp_path_factory: Any, request: Any) -> Tuple[Path, Any, Any]:
-    # ) -> Tuple[Path, Any, subprocess.Popen[bytes]]: # requires python>=3.9
+def result_folder(
+    tmp_path_factory: pytest.TempPathFactory, request: pytest.FixtureRequest
+) -> ResultFolder:
     """Fixture for creating results folder and opening a sub-process."""
     tmpdir = tmp_path_factory.getbasetemp()
-    filename = Path("tests/data") / request.param[0].with_suffix(".tif")
+    filename = (tpath / "data" / request.param[0]).with_suffix(".tif")
     runner = CliRunner()
-    result = runner.invoke(
-        __main__.main, [f"{filename.resolve()}", "G", "R", "C", "-o", tmpdir]
-    )
+    result = runner.invoke(main, [str(filename), "G", "R", "C", "-o", str(tmpdir)])
     return tmpdir, request.param, result
 
 
-def test_stdout(result_folder: Any) -> None:
+def test_stdout(result_folder: ResultFolder) -> None:
     """It outputs the correct value for 'Times'."""
     out = result_folder[2].output
     assert result_folder[2].return_value is None
     assert result_folder[2].exit_code == 0
     assert (
-        int([line for line in out.splitlines() if "Times:" in str(line)][0].split()[1])
+        int(next(line for line in out.splitlines() if "Times:" in str(line)).split()[1])
         == result_folder[1][1]
     )
 
 
 class TestOutputFiles:
     """It checks all output files."""
 
     @pytest.mark.parametrize("f", ["bg.csv", "label1.csv", "label2.csv", "label3.csv"])
-    def test_csv(self, result_folder: str, f: str) -> None:
+    def test_csv(self: "TestOutputFiles", result_folder: ResultFolder, f: str) -> None:
         """It checks csv tables."""
         fp_expected = Path("tests/data/output/") / result_folder[1][0] / f
         # # TODO: why Path is needed?
-        fp_result = result_folder[0] / Path(result_folder[1][0]) / f
+        fp_result = result_folder[0] / result_folder[1][0] / f
         expected = pd.read_csv(fp_expected)
         result = pd.read_csv(fp_result)
         pd.testing.assert_frame_equal(expected, result, atol=1e-15)
 
     @pytest.mark.parametrize(
         "f",
         [
@@ -63,38 +63,36 @@
             "label1_rcl.tif",
             "label2_rpH.tif",
             "label2_rcl.tif",
             "label3_rpH.tif",
             "label3_rcl.tif",
         ],
     )
-    def test_tif(self, result_folder: Any, f: str) -> None:
+    def test_tif(self, result_folder: ResultFolder, f: str) -> None:
         """It checks tif files: r_Cl, r_pH of segmented cells."""
         fp_expected = Path("tests/data/output/") / result_folder[1][0] / f
         fp_result = result_folder[0] / result_folder[1][0] / f
         expected = skimage.io.imread(fp_expected)
         result = skimage.io.imread(str(fp_result))  # for utf8 encoding?
         assert np.sum(result - expected) == pytest.approx(0, 2.3e-06)
 
     # @pytest.mark.mpl_image_compare(remove_text=True, tolerance=13)
     @pytest.mark.parametrize(("f", "tol"), [("_dim.png", 8.001), ("_meas.png", 20)])
-    def test_png(self, result_folder: Any, f: str, tol: float) -> None:
+    def test_png(self, result_folder: ResultFolder, f: str, tol: float) -> None:
         """It checks png files: saved segmentation and analysis."""
-        fp_expected = Path("tests/data/output/") / "".join(
-            (result_folder[1][0].name, f)
-        )
-        fp_result = result_folder[0] / "".join((result_folder[1][0].name, f))
+        fp_expected = tpath / "data" / "output" / "".join([result_folder[1][0], f])
+        fp_result = result_folder[0] / "".join((result_folder[1][0], f))
         msg = compare_images(fp_expected, fp_result, tol)
         if msg:
             raise ImageComparisonFailure(msg)
 
     @pytest.mark.parametrize(
         "f", ["bg-C-li_adaptive.pdf", "bg-G-li_adaptive.pdf", "bg-R-li_adaptive.pdf"]
     )
-    def test_pdf(self, result_folder: Any, f: str) -> None:
+    def test_pdf(self, result_folder: ResultFolder, f: str) -> None:
         """It checks pdf files: saved bg estimation."""
         fp_expected = Path("tests/data/output/") / result_folder[1][0] / f
         fp_result = result_folder[0] / result_folder[1][0] / f
         msg = compare_images(fp_expected, fp_result, 13)
         # Created by compare_images into tests/data folder
         rename = "_".join((fp_expected.name[:-4], "pdf.png"))
         fp_expected.with_name(rename).unlink()
@@ -103,20 +101,17 @@
 
 
 def test_bias_mflat(tmp_path: Path) -> None:
     """Check `bias dflat` cli."""
     d = tmp_path
     tmpflt = d / "ff.tif"
     tmpraw = d / "ff-raw.tif"
-    filename = os.path.join("tests", "data", "test_flat*.tif")
+    filename = str(Path("tests") / "data" / "test_flat*.tif")
     runner = CliRunner()
-    result = runner.invoke(
-        __main__.bima,
-        ["-o", f"{tmpflt.resolve()}", "mflat", filename],
-    )
+    result = runner.invoke(bima, ["-o", f"{tmpflt.resolve()}", "mflat", filename])
     assert str(3) in result.output
     test = tff.imread(tmpraw)
     expect = tff.imread(Path("tests") / "data" / "output" / "test_flat.tif")
     np.testing.assert_allclose(test, expect)
     test = tff.imread(tmpflt)
     expect = tff.imread(Path("tests") / "data" / "output" / "test_flat_gaussnorm.tif")
     np.testing.assert_allclose(test, expect)
```

### Comparing `nima-0.7.0/tests/data/1b_c16_15.tif` & `nima-0.7.1/tests/data/1b_c16_15.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15_dim.png` & `nima-0.7.1/tests/data/output/1b_c16_15_dim.png`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15_meas.png` & `nima-0.7.1/tests/data/output/1b_c16_15_meas.png`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf` & `nima-0.7.1/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf` & `nima-0.7.1/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf` & `nima-0.7.1/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label1.csv` & `nima-0.7.1/tests/data/output/1b_c16_15/label1.csv`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label1_rcl.tif` & `nima-0.7.1/tests/data/output/1b_c16_15/label1_rcl.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label1_rpH.tif` & `nima-0.7.1/tests/data/output/1b_c16_15/label1_rpH.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label2.csv` & `nima-0.7.1/tests/data/output/1b_c16_15/label2.csv`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label2_rcl.tif` & `nima-0.7.1/tests/data/output/1b_c16_15/label2_rcl.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label2_rpH.tif` & `nima-0.7.1/tests/data/output/1b_c16_15/label2_rpH.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label3_rcl.tif` & `nima-0.7.1/tests/data/output/1b_c16_15/label3_rcl.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/tests/data/output/1b_c16_15/label3_rpH.tif` & `nima-0.7.1/tests/data/output/1b_c16_15/label3_rpH.tif`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/LICENSE.txt` & `nima-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nima-0.7.0/pyproject.toml` & `nima-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,40 +29,41 @@
   "sigfig == 1.3.2"
 ]
 description = "Numerical IMage Analyses."
 keywords = ["ClopHensor", "ratio imaging", "image analysis", "chloride", "pH"]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "nima"
-readme = "docs/README.md"
-requires-python = ">=3.8,<3.12"
-version = "0.7.0"
+readme = "README.md"
+requires-python = ">=3.10,<3.12"
+version = "0.7.1"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen == 3.5.3",
+  "commitizen == 3.5.4",
   "pre-commit == 3.3.3",
   "ipykernel >=6.16.0",
   "ruff == 0.0.280",
   "pylsp-mypy",
   "jupyter",
   "jupyterlab",
   "python-lsp-ruff"
 ]
 docs = [
-  "pydata-sphinx-theme ==0.13.2",
-  "sphinx-click == 4.4.0",
-  "Sphinx == 7.1.0",
+  "autodocsumm == 0.2.11",
+  "pydata-sphinx-theme == 0.13.3",
   "Pygments == 2.15.1",
-  "myst-parser == 2.0.0"
+  "Sphinx == 7.1.1",
+  "sphinx-click == 4.4.0",
+  "sphinx_autodoc_typehints == 1.24.0"
 ]
 tests = [
   "pytest == 7.4.0",
   "coverage[toml] == 7.2.7",
-  "typeguard ==2.13.3",
+  "typeguard ==4.1.0",
   "pandas-stubs == 2.0.2.230605",
   "mypy == 1.4.1",
   "data-science-types == 0.2.23",
   "xdoctest == 1.1.1",
   "types-setuptools == 68.0.0.3"
 ]
 
@@ -91,19 +92,19 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.7.0"
+version = "0.7.1"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
-  "docs/README.md:Version"
+  "README.md:Version"
 ]
 
 [tool.commitizen.customize]
 bump_map = {"^.+!:" = "MAJOR", "BREAKING CHANGE" = "MAJOR", "feat" = "MINOR", "fix" = "PATCH", "perf" = "PATCH", "refactor" = "PATCH"}
 bump_pattern = "^(BREAKING CHANGE|feat|fix|perf|refactor)"
 change_type_map = {"feat" = "Feat", "fix" = "Fix", "docs" = "Docs", "build" = "Build", "style" = "Style", "refactor" = "Refactor", "perf" = "Perf", "test" = "Test", "ci" = "CI/CD"}
 change_type_order = ["BREAKING CHANGE", "Feat", "Fix", "Docs", "Style", "Perf", "Test", "Build", "CI/CD"]
@@ -192,15 +193,15 @@
 typeguard = "pytest --typeguard-packages=nima {args}"
 
 [tool.hatch.envs.tests]
 features = ["tests"]
 template = "tests"
 
 [[tool.hatch.envs.tests.matrix]]
-python = ["3.11", "3.10", "3.9", "3.8"]  # reverse order to ensure the presence in older python of module included in newer versions
+python = ["3.11", "3.10"]  # reverse order to ensure the presence in older python of module included in newer versions
 
 [tool.hatch.envs.tests.scripts]
 all = ["test", "type", "xdoc", "cov"]
 cov = [
   "coverage combine",
   "coverage report",
   "coverage xml"
@@ -231,50 +232,45 @@
 dmypy = false
 enabled = true
 live_mode = true
 strict = true
 
 [tool.ruff]
 force-exclude = true
-# ignore = [
-# "ANN101",
-# "ANN102",
-# "ANN201",
-# "E501"
-# ]
+ignore = ["ANN101", "ANN102"]
 line-length = 88
 select = [
-  # "A",  # builtins
-  # "ANN",  # typing annotation
-  # "ARG",  # unused arguments
-  # "B",  # bugbear
-  # "C",
+  "A",  # builtins
+  "ANN",  # typing annotation
+  "ARG",  # unused arguments
+  "B",  # bugbear
+  "C",
   "C4",  # comprehensions
-  # "C90",  # mccabe
+  "C90",  # mccabe
   "D",  # pydocstyle
-  # "DTZ",  # dates
+  "DTZ",  # dates
   "E",  # pycodestyle
   # "TRY",  # exceptions
   # "EM",  # exceptions
   "ERA",  # eradicate
   "F",  # pyflakes
   # # "FBT",    # boolean-trap
   "I",  # isort
   "ICN",  # import conventions (opinionated)
   "ISC",  # implicit-str-concat
   "N",  # pep8-naming
-  # "PD",  # pandas-vet
+  "PD",  # pandas-vet
   # # "PGH",  # pygrep WAIT
   # "PL",  # pylint see PLR2004...
   "PT",  # pytest-style
-  # "PTH",  # use-pathlib
+  "PTH",  # use-pathlib
   "Q",  # quotes
-  # "RUF",  # Ruff
+  "RUF",  # Ruff
   "S",  # bandit XXX
-  # "SIM",  # simplify
+  "SIM",  # simplify
   "TID",  # tidy-imports
   "UP",  # pyupgrade
   "YTT",  # 2020
   "W"  # pycodestyle
 ]
 
 [tool.ruff.isort]
```

### Comparing `nima-0.7.0/docs/README.md` & `nima-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![CI](https://github.com/darosio/nima/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/nima/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/nima/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/nima)
 [![RtD](https://readthedocs.org/projects/nima/badge/)](https://nima.readthedocs.io/)
 
 A library and a cli to help image analyses based on scipy.ndimage and
 scikit-image.
 
-- Version: “0.7.0”
+- Version: “0.7.1”
 
 ## Features
 
 - easy dark and flat correction
 - automatic cell segmentation
 - easy ratio analyses
```

### Comparing `nima-0.7.0/PKG-INFO` & `nima-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 Metadata-Version: 2.1
 Name: nima
-Version: 0.7.0
+Version: 0.7.1
 Summary: Numerical IMage Analyses.
 Project-URL: homepage, https://github.com/darosio/nima/
 Project-URL: repository, https://github.com/darosio/nima/
 Author-email: daniele arosio <daniele.arosio@cnr.it>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Keywords: ClopHensor,chloride,image analysis,pH,ratio imaging
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.12,>=3.8
+Requires-Python: <3.12,>=3.10
 Requires-Dist: bokeh<3.2.2
 Requires-Dist: click==8.1.6
 Requires-Dist: dask[distributed]<=2023.7.1
 Requires-Dist: matplotlib==3.7.2
 Requires-Dist: numpy<1.25.2
 Requires-Dist: pandas==2.0.3
 Requires-Dist: scikit-image==0.21.0
 Requires-Dist: scipy<1.11.2
 Requires-Dist: sigfig==1.3.2
 Requires-Dist: tifffile<=2023.7.18
 Requires-Dist: zarr==2.16.0
 Provides-Extra: dev
-Requires-Dist: commitizen==3.5.3; extra == 'dev'
+Requires-Dist: commitizen==3.5.4; extra == 'dev'
 Requires-Dist: ipykernel>=6.16.0; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: pre-commit==3.3.3; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
 Requires-Dist: ruff==0.0.280; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: myst-parser==2.0.0; extra == 'docs'
-Requires-Dist: pydata-sphinx-theme==0.13.2; extra == 'docs'
+Requires-Dist: autodocsumm==0.2.11; extra == 'docs'
+Requires-Dist: pydata-sphinx-theme==0.13.3; extra == 'docs'
 Requires-Dist: pygments==2.15.1; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints==1.24.0; extra == 'docs'
 Requires-Dist: sphinx-click==4.4.0; extra == 'docs'
-Requires-Dist: sphinx==7.1.0; extra == 'docs'
+Requires-Dist: sphinx==7.1.1; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: coverage[toml]==7.2.7; extra == 'tests'
 Requires-Dist: data-science-types==0.2.23; extra == 'tests'
 Requires-Dist: mypy==1.4.1; extra == 'tests'
 Requires-Dist: pandas-stubs==2.0.2.230605; extra == 'tests'
 Requires-Dist: pytest==7.4.0; extra == 'tests'
-Requires-Dist: typeguard==2.13.3; extra == 'tests'
+Requires-Dist: typeguard==4.1.0; extra == 'tests'
 Requires-Dist: types-setuptools==68.0.0.3; extra == 'tests'
 Requires-Dist: xdoctest==1.1.1; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # NImA
 
 [![PyPI](https://img.shields.io/pypi/v/nima.svg)](https://pypi.org/project/nima/)
 [![CI](https://github.com/darosio/nima/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/nima/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/nima/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/nima)
 [![RtD](https://readthedocs.org/projects/nima/badge/)](https://nima.readthedocs.io/)
 
 A library and a cli to help image analyses based on scipy.ndimage and
 scikit-image.
 
-- Version: “0.7.0”
+- Version: “0.7.1”
 
 ## Features
 
 - easy dark and flat correction
 - automatic cell segmentation
 - easy ratio analyses
```

