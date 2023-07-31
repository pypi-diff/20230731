# Comparing `tmp/caloutils-0.0.3.tar.gz` & `tmp/caloutils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caloutils-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caloutils-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caloutils-0.0.3.tar` & `caloutils-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,46 @@
--rw-r--r--   0        0        0      305 2023-07-28 14:47:00.347636 caloutils-0.0.3/.bumpversion.cfg
--rw-r--r--   0        0        0      292 2023-07-28 14:47:00.347636 caloutils-0.0.3/.editorconfig
--rw-r--r--   0        0        0      320 2023-07-28 14:47:00.347636 caloutils-0.0.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1036 2023-07-28 14:47:00.347636 caloutils-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3078 2023-07-28 14:47:00.347636 caloutils-0.0.3/.gitignore
--rw-r--r--   0        0        0     1122 2023-07-28 14:47:00.347636 caloutils-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      728 2023-07-28 14:47:00.347636 caloutils-0.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0      685 2023-07-28 14:47:00.347636 caloutils-0.0.3/.travis.yml
--rw-r--r--   0        0        0     3517 2023-07-28 14:47:00.347636 caloutils-0.0.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0       89 2023-07-28 14:47:00.347636 caloutils-0.0.3/HISTORY.rst
--rw-r--r--   0        0        0     1062 2023-07-28 14:47:00.347636 caloutils-0.0.3/LICENSE
--rw-r--r--   0        0        0      262 2023-07-28 14:47:00.347636 caloutils-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0      928 2023-07-28 14:47:00.347636 caloutils-0.0.3/Makefile
--rw-r--r--   0        0        0      937 2023-07-28 14:47:00.347636 caloutils-0.0.3/README.rst
--rw-r--r--   0        0        0      610 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/Makefile
--rw-r--r--   0        0        0       28 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/authors.rst
--rwxr-xr-x   0        0        0     4787 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/conf.py
--rw-r--r--   0        0        0       33 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/contributing.rst
--rw-r--r--   0        0        0       28 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/history.rst
--rw-r--r--   0        0        0      306 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/index.rst
--rw-r--r--   0        0        0     1126 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/installation.rst
--rw-r--r--   0        0        0      807 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/make.bat
--rw-r--r--   0        0        0       27 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/readme.rst
--rw-r--r--   0        0        0       73 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/usage.rst
--rw-r--r--   0        0        0     2431 2023-07-28 14:47:00.347636 caloutils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      143 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/__init__.py
--rw-r--r--   0        0        0       19 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/caloutils.py
--rw-r--r--   0        0        0     1644 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/metrics/pca.py
--rw-r--r--   0        0        0     1287 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/metrics/postprocess.py
--rw-r--r--   0        0        0     4829 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/metrics/shower.py
--rw-r--r--   0        0        0      182 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/binborders.py
--rw-r--r--   0        0        0     1286 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/hist1d.py
--rw-r--r--   0        0        0     3408 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/hist2d.py
--rw-r--r--   0        0        0     1545 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/infolut.py
--rw-r--r--   0        0        0     3097 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/ratioplot.py
--rw-r--r--   0        0        0     1360 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/processing/alpharot.py
--rw-r--r--   0        0        0      945 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/processing/convcoord.py
--rw-r--r--   0        0        0     1758 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/processing/dequantscaler.py
--rw-r--r--   0        0        0     2148 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/idxscale.py
--rw-r--r--   0        0        0     3184 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/objcol.py
--rw-r--r--   0        0        0     1564 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/seq.py
--rw-r--r--   0        0        0     7376 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/voxelize.py
--rw-r--r--   0        0        0       39 2023-07-28 14:47:00.351636 caloutils-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      364 2023-07-28 14:47:00.351636 caloutils-0.0.3/tests/test_caloutils.py
--rw-r--r--   0        0        0     5385 2023-07-28 14:47:00.351636 caloutils-0.0.3/tests/voxelize.py
--rw-r--r--   0        0        0      230 2023-07-28 14:47:00.351636 caloutils-0.0.3/tox.ini
--rwxr-xr-x   0        0        0      318 2023-07-28 14:47:00.351636 caloutils-0.0.3/venv_setup.sh
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 caloutils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      311 2023-07-31 14:32:23.107529 caloutils-0.0.8/.bumpversion.cfg
+-rw-r--r--   0        0        0      292 2023-07-31 14:32:23.107529 caloutils-0.0.8/.editorconfig
+-rw-r--r--   0        0        0      320 2023-07-31 14:32:23.107529 caloutils-0.0.8/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1536 2023-07-31 14:32:23.107529 caloutils-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3095 2023-07-31 14:32:23.107529 caloutils-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1122 2023-07-31 14:32:23.107529 caloutils-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      718 2023-07-31 14:32:23.107529 caloutils-0.0.8/.readthedocs.yaml
+-rw-r--r--   0        0        0      685 2023-07-31 14:32:23.107529 caloutils-0.0.8/.travis.yml
+-rw-r--r--   0        0        0     1062 2023-07-31 14:32:23.107529 caloutils-0.0.8/LICENSE
+-rw-r--r--   0        0        0      277 2023-07-31 14:32:23.107529 caloutils-0.0.8/MANIFEST.in
+-rw-r--r--   0        0        0      618 2023-07-31 14:32:23.107529 caloutils-0.0.8/Makefile
+-rw-r--r--   0        0        0      937 2023-07-31 14:32:23.107529 caloutils-0.0.8/README.rst
+-rw-r--r--   0        0        0      388 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/__init__.py
+-rw-r--r--   0        0        0      628 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/calorimeter.py
+-rw-r--r--   0        0        0      151 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/__init__.py
+-rw-r--r--   0        0        0     2101 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/batch_to_Exyz.py
+-rw-r--r--   0        0        0     2575 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/pc_from_voxel.py
+-rw-r--r--   0        0        0     8698 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/utils.py
+-rw-r--r--   0        0        0     1346 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/processing/voxelize.py
+-rw-r--r--   0        0        0       68 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/utils/__init__.py
+-rw-r--r--   0        0        0     1790 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/utils/batch.py
+-rw-r--r--   0        0        0      232 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/__init__.py
+-rw-r--r--   0        0        0     3172 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/analyze_layers.py
+-rw-r--r--   0        0        0     1867 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/calculate_variables.py
+-rw-r--r--   0        0        0     4370 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/energy_ratios.py
+-rw-r--r--   0        0        0     2220 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/first_principal_components.py
+-rw-r--r--   0        0        0      794 2023-07-31 14:32:23.107529 caloutils-0.0.8/caloutils/variables/response.py
+-rw-r--r--   0        0        0      610 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/Makefile
+-rw-r--r--   0        0        0      202 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/authors.rst
+-rwxr-xr-x   0        0        0     5098 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/conf.py
+-rw-r--r--   0        0        0     3517 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/contributing.rst
+-rw-r--r--   0        0        0       89 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/history.rst
+-rw-r--r--   0        0        0      408 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/index.rst
+-rw-r--r--   0        0        0     1126 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/installation.rst
+-rw-r--r--   0        0        0      121 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/processing.rst
+-rw-r--r--   0        0        0       27 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/readme.rst
+-rw-r--r--   0        0        0      103 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/utils.rst
+-rw-r--r--   0        0        0      119 2023-07-31 14:32:23.107529 caloutils-0.0.8/docs/variables.rst
+-rw-r--r--   0        0        0     2484 2023-07-31 14:32:23.111529 caloutils-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/test_batch.py
+-rw-r--r--   0        0        0      364 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/test_caloutils.py
+-rw-r--r--   0        0        0     5682 2023-07-31 14:32:23.111529 caloutils-0.0.8/tests/voxelize.py
+-rw-r--r--   0        0        0      230 2023-07-31 14:32:23.111529 caloutils-0.0.8/tox.ini
+-rwxr-xr-x   0        0        0      318 2023-07-31 14:32:23.111529 caloutils-0.0.8/venv_setup.sh
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 caloutils-0.0.8/PKG-INFO
```

### Comparing `caloutils-0.0.3/.gitignore` & `caloutils-0.0.8/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+*.code-workspace
```

### Comparing `caloutils-0.0.3/.pre-commit-config.yaml` & `caloutils-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/.readthedocs.yaml` & `caloutils-0.0.8/.readthedocs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build:
   os: ubuntu-22.04
   tools:
     python: "3.10"
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
-   configuration: caloutils/docs/conf.py
+   configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
 # formats:
 #    - pdf
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
```

### Comparing `caloutils-0.0.3/.travis.yml` & `caloutils-0.0.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/CONTRIBUTING.rst` & `caloutils-0.0.8/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/LICENSE` & `caloutils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/README.rst` & `caloutils-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/docs/Makefile` & `caloutils-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/docs/conf.py` & `caloutils-0.0.8/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,27 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autosummary",
+    "autodocsumm",
+]
+
+autosummary_generate = True  # Turn on sphinx.ext.autosummary
+autosummary_generate_overwrite = True
+autodoc_default_options = {
+    "autosummary": True,
+}
+
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -61,15 +73,15 @@
 release = caloutils.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -80,26 +92,30 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "alabaster"
+import sphinx_rtd_theme
+
+html_theme = "sphinx_rtd_theme"
+
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+# html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "caloutilsdoc"
```

### Comparing `caloutils-0.0.3/docs/installation.rst` & `caloutils-0.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.3/pyproject.toml` & `caloutils-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caloutils"
-version = '0.0.3'
+version = '0.0.8'
 authors = [
   { name="mova", email="mova@users.noreply.github.com" },
   { name="kaechb", email="kaechb@users.noreply.github.com" },
 ]
 description = "Metrics and tools for evaluation generative models for calorimeter shower based on pytorch_geometric."
 requires-python = ">=3.8"
 readme="README.rst"
@@ -14,24 +14,26 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "torch>=2.0.0",
     "torch_geometric>=2.3.0",
     "torch-scatter>=2.1.1",
 ]
+
+
 [project.optional-dependencies]
 dev = [
   "pytest >=2.7.3",
   "pytest-cov",
   "bump2version",
   "black",
   "pre-commit",
   "ruff",
 ]
-doc = ["sphinx"]
+doc = ["sphinx","sphinx_rtd_theme","autodocsumm"]
 
 
 [project.urls]
 "Homepage" = "https://github.com/DeGeSim/caloutils"
 "Bug Tracker" = "https://github.com/DeGeSim/caloutils/issues"
 
 # [project.scripts]
@@ -126,11 +128,12 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
+ignore = ["E501"]
 target-version = "py310"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402","F401"]
```

### Comparing `caloutils-0.0.3/PKG-INFO` & `caloutils-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caloutils
-Version: 0.0.3
+Version: 0.0.8
 Summary: Metrics and tools for evaluation generative models for calorimeter shower based on pytorch_geometric.
 Author-email: mova <mova@users.noreply.github.com>, kaechb <kaechb@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 Requires-Dist: pytest >=2.7.3 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: sphinx_rtd_theme ; extra == "doc"
+Requires-Dist: autodocsumm ; extra == "doc"
 Project-URL: Bug Tracker, https://github.com/DeGeSim/caloutils/issues
 Project-URL: Homepage, https://github.com/DeGeSim/caloutils
 Provides-Extra: dev
 Provides-Extra: doc
 
 =========
 caloutils
```

