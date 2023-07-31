# Comparing `tmp/rxn-chem-utils-1.1.5.tar.gz` & `tmp/rxn-chem-utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-chem-utils-1.1.5.tar", last modified: Thu Jul 13 15:21:36 2023, max compression
+gzip compressed data, was "rxn-chem-utils-1.2.0.tar", last modified: Mon Jul 31 13:04:45 2023, max compression
```

## Comparing `rxn-chem-utils-1.1.5.tar` & `rxn-chem-utils-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.366419 rxn-chem-utils-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.366419 rxn-chem-utils-1.1.5/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.370420 rxn-chem-utils-1.1.5/src/rxn/chemutils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/extended_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/multicomponent_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.370420 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/combine_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/src/rxn/chemutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 15:21:36.000000 rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:21:36.374420 rxn-chem-utils-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_extended_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_multicomponent_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_reaction_combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_reaction_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_smiles_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_smiles_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 15:21:25.000000 rxn-chem-utils-1.1.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.351865 rxn-chem-utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-31 13:04:45.351865 rxn-chem-utils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 13:04:45.355865 rxn-chem-utils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.339865 rxn-chem-utils-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.339865 rxn-chem-utils-1.2.0/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.347865 rxn-chem-utils-1.2.0/src/rxn/chemutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/extended_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/multicomponent_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.347865 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/combine_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.347865 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.351865 rxn-chem-utils-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_extended_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_multicomponent_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_reaction_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_reaction_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_smiles_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_smiles_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_utils.py
```

### Comparing `rxn-chem-utils-1.1.5/LICENSE` & `rxn-chem-utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/README.md` & `rxn-chem-utils-1.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # RXN chemistry utilities package
 
 [![Actions tests](https://github.com/rxn4chemistry/rxn-chemutils/actions/workflows/tests.yaml/badge.svg)](https://github.com/rxn4chemistry/rxn-chemutils/actions)
 
 This repository contains various chemistry-related Python utilities used in the RXN universe.
 For general utilities not related to chemistry, see our other repository [`rxn-utilities`](https://github.com/rxn4chemistry/rxn-utilities).
 
-The documentation can be found [here](https://rxn4chemistry.github.io/rxn-chemutils/).
+Links:
+* [GitHub repository](https://github.com/rxn4chemistry/rxn-chemutils)
+* [Documentation](https://rxn4chemistry.github.io/rxn-chemutils/)
+* [PyPI package](https://pypi.org/project/rxn-chem-utils/)
 
 ## System Requirements
 
 This package is supported on all operating systems. 
 It has been tested on the following systems:
 + macOS: Big Sur (11.1)
 + Linux: Ubuntu 18.04.4
 
-A Python version of 3.6 or greater is recommended.
+A Python version of 3.7 or greater is recommended.
 
 ## Installation guide
 
 The package can be installed from Pypi:
 ```bash
 pip install rxn-chem-utils
 ```
@@ -31,10 +34,8 @@
 The `RDKit` dependency is not installed automatically and can be installed via Conda or Pypi:
 ```bash
 # Install RDKit from Conda
 conda install -c conda-forge rdkit
 
 # Install RDKit from Pypi
 pip install rdkit
-# for Python<3.7
-# pip install rdkit-pypi
 ```
```

### Comparing `rxn-chem-utils-1.1.5/setup.cfg` & `rxn-chem-utils-1.2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 author_email = rxn4chemistry@zurich.ibm.com
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
-python_requires = >= 3.6
+python_requires = >= 3.7
 zip_safe = False
 include_package_data = True
 install_requires = 
 	attrs>=21.2.0
-	click>=7.0,<8.1.4
+	click>=7.0
 	rxn-utils>=1.1.9
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 rxn.chemutils = 
@@ -37,16 +41,15 @@
 	bump2version>=1.0.1
 	flake8>=3.7.9
 	isort>=5.9.3
 	mypy>=0.910
 	pytest>=5.3.4
 	types-setuptools>=57.4.17
 rdkit = 
-	rdkit-pypi>=2021.3.2 ; python_version<"3.7"
-	rdkit>=2022.3.4 ; python_version>="3.7"
+	rdkit>=2022.3.4
 
 [options.entry_points]
 console_scripts = 
 	rxn-canonicalize = rxn.chemutils.scripts.canonicalize:main
 	rxn-combine-reaction = rxn.chemutils.scripts.combine_reaction:main
 	rxn-detokenize = rxn.chemutils.scripts.detokenize:main
 	rxn-tokenize = rxn.chemutils.scripts.tokenize:main
```

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/conversion.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/conversion.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/exceptions.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/extended_reaction_smiles.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/extended_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/miscellaneous.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/miscellaneous.py`

 * *Files 4% similar despite different names*

```diff
@@ -313,7 +313,32 @@
     agents = []
     products = []
     for reaction in reactions:
         reactants.extend(reaction.reactants)
         agents.extend(reaction.agents)
         products.extend(reaction.products)
     return ReactionEquation(reactants=reactants, agents=agents, products=products)
+
+
+def mol_has_atom_mapping(mol: Mol) -> bool:
+    """
+    Whether at least one atom of an RDKit Mol contains an atom map number.
+
+    Args:
+        mol: RDKit Mol.
+    """
+    atom: Atom
+    for atom in mol.GetAtoms():
+        if atom.GetAtomMapNum() != 0:
+            return True
+    return False
+
+
+def smiles_has_atom_mapping(smiles: str) -> bool:
+    """
+    Whether at least one atom of a compound SMILES contains an atom map number.
+
+    Args:
+        smiles: compound SMILES.
+    """
+    mol = smiles_to_mol(smiles, sanitize=False)
+    return mol_has_atom_mapping(mol)
```

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/multicomponent_smiles.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/multicomponent_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_combiner.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_combiner.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_equation.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_equation.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/reaction_smiles.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/canonicalize.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/canonicalize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/combine_reaction.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/combine_reaction.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/detokenize.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/detokenize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/scripts/tokenize.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/tokenize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_augmenter.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/smiles_randomization.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_randomization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/tokenization.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/tokenization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn/chemutils/utils.py` & `rxn-chem-utils-1.2.0/src/rxn/chemutils/utils.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/src/rxn_chem_utils.egg-info/SOURCES.txt` & `rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_conversion.py` & `rxn-chem-utils-1.2.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_extended_reaction_smiles.py` & `rxn-chem-utils-1.2.0/tests/test_extended_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_miscellaneous.py` & `rxn-chem-utils-1.2.0/tests/test_miscellaneous.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     canonicalize_any,
     equivalent_smiles,
     get_individual_compounds,
     is_valid_smiles,
     merge_reactions,
     remove_chiral_centers,
     remove_double_bond_stereochemistry,
+    smiles_has_atom_mapping,
     sort_any,
 )
 from rxn.chemutils.reaction_equation import ReactionEquation
 
 
 def test_equivalent_smiles() -> None:
     assert equivalent_smiles("CCO", "C(C)O")
@@ -256,7 +257,24 @@
 
     # more than two reactions
     r3 = ReactionEquation([], ["H"], [])
     r4 = ReactionEquation([], [], ["I"])
     assert merge_reactions(r1, r2, r3, r4) == ReactionEquation(
         ["A", "B", "F"], ["C", "G", "H"], ["D", "I"]
     )
+
+
+def test_smiles_has_atom_mapping() -> None:
+    assert smiles_has_atom_mapping("[CH3:9][CH:8]([CH3:10])c1ccccc1")
+    assert smiles_has_atom_mapping("CCO[CH3:9]")
+    assert smiles_has_atom_mapping("C[CH3:9].O")
+
+    assert not smiles_has_atom_mapping("CC")
+    assert not smiles_has_atom_mapping("C[CH3]")
+    assert not smiles_has_atom_mapping("C[12CH3]")
+
+    # Note: does not care about valence, but SMILES must be valid
+    # invalid valence -> call succeeds:
+    assert smiles_has_atom_mapping("CF(C)CC[C:9]")
+    # invalid SMILES -> call raises:
+    with pytest.raises(InvalidSmiles):
+        _ = canonicalize_any("[CH3:9]C(")
```

### Comparing `rxn-chem-utils-1.1.5/tests/test_multicomponent_smiles.py` & `rxn-chem-utils-1.2.0/tests/test_multicomponent_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_rdkit_utils.py` & `rxn-chem-utils-1.2.0/tests/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_reaction_combiner.py` & `rxn-chem-utils-1.2.0/tests/test_reaction_combiner.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_reaction_equation.py` & `rxn-chem-utils-1.2.0/tests/test_reaction_equation.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_reaction_smiles.py` & `rxn-chem-utils-1.2.0/tests/test_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_smiles_augmenter.py` & `rxn-chem-utils-1.2.0/tests/test_smiles_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_smiles_randomization.py` & `rxn-chem-utils-1.2.0/tests/test_smiles_randomization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_tokenization.py` & `rxn-chem-utils-1.2.0/tests/test_tokenization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.1.5/tests/test_utils.py` & `rxn-chem-utils-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

