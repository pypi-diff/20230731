# Comparing `tmp/qcelemental-0.8.0.tar.gz` & `tmp/qcelemental-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcelemental-0.8.0.tar", last modified: Fri Sep 13 21:12:18 2019, max compression
+gzip compressed data, was "dist/qcelemental-0.9.0.tar", last modified: Mon Sep 30 23:18:05 2019, max compression
```

## Comparing `qcelemental-0.8.0.tar` & `qcelemental-0.9.0.tar`

### file list

```diff
@@ -1,97 +1,232 @@
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1541 2019-09-13 21:11:51.000000 qcelemental-0.8.0/LICENSE
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      227 2019-09-13 21:11:51.000000 qcelemental-0.8.0/MANIFEST.in
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5786 2019-09-13 21:12:18.000000 qcelemental-0.8.0/PKG-INFO
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4216 2019-09-13 21:11:51.000000 qcelemental-0.8.0/README.md
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1185 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      498 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/_version.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7219 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/covalent_radii.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/data/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      152 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/data/README.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      292 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/data/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5531 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/data/alvarez_2008_covalent_radii.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1779 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/data/mantina_2009_vanderwaals_radii.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)   117788 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/data/nist_2011_atomic_weights.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    74402 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/data/nist_2014_codata.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6595 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/datum.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1392 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/exceptions.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      481 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/extras.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/models/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      564 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5731 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/align.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5922 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/basemodels.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4220 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/common_models.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    50922 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/molecule.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1869 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/procedures.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4403 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/results.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      534 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/models/types.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/molparse/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      337 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    25750 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/chgmult.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    29229 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/from_arrays.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7107 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/from_schema.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    28885 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/from_string.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15059 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/nucleus.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6385 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/pubchem.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2798 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/regex.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4703 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/to_schema.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    12380 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molparse/to_string.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/molutil/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       56 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molutil/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    25360 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molutil/align.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    22509 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/molutil/test_align.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    16257 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/periodic_table.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/physical_constants/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      386 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/physical_constants/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18509 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/physical_constants/context.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5936 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/physical_constants/ureg.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18576 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/testing.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/tests/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1209 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/addons.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2520 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_constants.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2162 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_covalentradii.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3970 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_datum.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2153 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_importing.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7721 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_model_serials.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18314 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molecule.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    19655 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_align_chiral.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4835 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_from_schema.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    65539 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_from_string.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2115 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_parse_nucleus_label.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6675 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_pubchem.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3697 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_reconcile_nucleus.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    10573 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_to_schema.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5884 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_to_string.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     8556 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_molparse_validate_and_fill_chgmult.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4077 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_periodictable.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9105 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_testing.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2767 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_units.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9933 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_utils.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2104 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/tests/test_vanderwaalsradii.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental/util/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      807 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9292 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/autodocs.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    16242 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/gph_uno_bipartite.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2754 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/importing.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      493 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/internal.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      697 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/itertools.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9581 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/misc.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3736 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/np_blockwise.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2392 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/np_rand3drot.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    10469 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/scipy_hungarian.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7120 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/serialization.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     8778 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/test_gph_uno_bipartite.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2946 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/util/test_scipy_hungarian.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6276 2019-09-13 21:11:51.000000 qcelemental-0.8.0/qcelemental/vanderwaals_radii.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5786 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/PKG-INFO
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2876 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/SOURCES.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        1 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/dependency_links.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        1 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/not-zip-safe
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      157 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/requires.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       12 2019-09-13 21:12:18.000000 qcelemental-0.8.0/qcelemental.egg-info/top_level.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      941 2019-09-13 21:12:18.000000 qcelemental-0.8.0/setup.cfg
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2320 2019-09-13 21:11:51.000000 qcelemental-0.8.0/setup.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    68611 2019-09-13 21:11:51.000000 qcelemental-0.8.0/versioneer.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/
+-rw-r--r--   0 levinaden   (501) staff       (20)     5791 2019-09-30 23:18:05.000000 qcelemental-0.9.0/PKG-INFO
+-rw-r--r--   0 levinaden   (501) staff       (20)     1541 2019-01-17 19:32:50.000000 qcelemental-0.9.0/LICENSE
+-rw-r--r--   0 levinaden   (501) staff       (20)      227 2019-01-17 19:32:50.000000 qcelemental-0.9.0/MANIFEST.in
+-rw-r--r--   0 levinaden   (501) staff       (20)     4221 2019-09-30 13:54:51.000000 qcelemental-0.9.0/README.md
+-rw-r--r--   0 levinaden   (501) staff       (20)     2320 2019-09-30 13:54:31.000000 qcelemental-0.9.0/setup.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental.egg-info/
+-rw-r--r--   0 levinaden   (501) staff       (20)     5791 2019-09-30 23:18:04.000000 qcelemental-0.9.0/qcelemental.egg-info/PKG-INFO
+-rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-01-20 20:30:55.000000 qcelemental-0.9.0/qcelemental.egg-info/not-zip-safe
+-rw-r--r--   0 levinaden   (501) staff       (20)     9181 2019-09-30 23:18:04.000000 qcelemental-0.9.0/qcelemental.egg-info/SOURCES.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)      157 2019-09-30 23:18:04.000000 qcelemental-0.9.0/qcelemental.egg-info/requires.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)       12 2019-09-30 23:18:04.000000 qcelemental-0.9.0/qcelemental.egg-info/top_level.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-09-30 23:18:04.000000 qcelemental-0.9.0/qcelemental.egg-info/dependency_links.txt
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/
+-rw-r--r--   0 levinaden   (501) staff       (20)      481 2019-05-31 17:28:36.000000 qcelemental-0.9.0/qcelemental/extras.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    16257 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/periodic_table.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/molparse/
+-rw-r--r--   0 levinaden   (501) staff       (20)     6385 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/molparse/pubchem.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    25750 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/molparse/chgmult.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    29229 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/molparse/from_arrays.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      337 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/molparse/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4703 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/molparse/to_schema.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    15059 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/molparse/nucleus.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    28885 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/molparse/from_string.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     7107 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/molparse/from_schema.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    13108 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/molparse/to_string.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2798 2019-05-31 17:28:36.000000 qcelemental-0.9.0/qcelemental/molparse/regex.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     6595 2019-05-31 17:28:36.000000 qcelemental-0.9.0/qcelemental/datum.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     6276 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/vanderwaals_radii.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     7219 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/covalent_radii.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/molutil/
+-rw-r--r--   0 levinaden   (501) staff       (20)    25360 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/molutil/align.py
+-rw-r--r--   0 levinaden   (501) staff       (20)       56 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/molutil/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    22509 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/molutil/test_align.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/util/
+-rw-r--r--   0 levinaden   (501) staff       (20)      493 2019-05-31 17:28:36.000000 qcelemental-0.9.0/qcelemental/util/internal.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     9581 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/util/misc.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    16242 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/util/gph_uno_bipartite.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2392 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/util/np_rand3drot.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     9292 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/util/autodocs.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2754 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/util/importing.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     3736 2019-05-01 12:24:57.000000 qcelemental-0.9.0/qcelemental/util/np_blockwise.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    10469 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/util/scipy_hungarian.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      807 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/util/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     8778 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/util/test_gph_uno_bipartite.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     7120 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/util/serialization.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2946 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/util/test_scipy_hungarian.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      697 2019-01-17 19:32:50.000000 qcelemental-0.9.0/qcelemental/util/itertools.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      498 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/_version.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/tests/
+-rw-r--r--   0 levinaden   (501) staff       (20)     9933 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/tests/test_utils.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4077 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_periodictable.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2115 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_parse_nucleus_label.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1209 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/tests/addons.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     3697 2019-07-29 15:51:14.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_reconcile_nucleus.py
+-rw-r--r--   0 levinaden   (501) staff       (20)        0 2019-05-01 12:24:57.000000 qcelemental-0.9.0/qcelemental/tests/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    18314 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_molecule.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2153 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_importing.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2104 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_vanderwaalsradii.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     9751 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_model_results.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     6675 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_pubchem.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2767 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_units.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     3970 2019-07-29 15:51:14.000000 qcelemental-0.9.0/qcelemental/tests/test_datum.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     7721 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_model_serials.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    19655 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_align_chiral.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4835 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_from_schema.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    10573 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_to_schema.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    65539 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_from_string.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2520 2019-07-29 15:51:14.000000 qcelemental-0.9.0/qcelemental/tests/test_constants.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     6186 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_to_string.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2162 2019-08-23 19:47:52.000000 qcelemental-0.9.0/qcelemental/tests/test_covalentradii.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     8556 2019-07-29 15:51:14.000000 qcelemental-0.9.0/qcelemental/tests/test_molparse_validate_and_fill_chgmult.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     9105 2019-07-29 15:51:14.000000 qcelemental-0.9.0/qcelemental/tests/test_testing.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1172 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/__init__.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/models/
+-rw-r--r--   0 levinaden   (501) staff       (20)     6092 2019-09-30 23:17:45.000000 qcelemental-0.9.0/qcelemental/models/basis.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5731 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/models/align.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    50922 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/models/molecule.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    16993 2019-09-30 23:17:45.000000 qcelemental-0.9.0/qcelemental/models/results.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      592 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/models/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      534 2019-08-29 15:04:25.000000 qcelemental-0.9.0/qcelemental/models/types.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5802 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/models/basemodels.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4629 2019-09-30 23:17:45.000000 qcelemental-0.9.0/qcelemental/models/procedures.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4324 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/models/common_models.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/
+-rw-r--r--   0 levinaden   (501) staff       (20)   103453 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/datetime.data.json
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/distutils/
+-rw-r--r--   0 levinaden   (501) staff       (20)    25050 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/distutils/version.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1503 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/distutils/version.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1469 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/distutils/__init__.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1015 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/distutils/__init__.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1500 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/builtins.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    39438 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/time.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   156320 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/decimal.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    56757 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/sys.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    18717 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/textwrap.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1473 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/enum.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    26332 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/mmap.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1443 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/abc.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1456 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/itertools.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    34707 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/dataclasses.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   362950 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/typing.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1505 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/contextlib.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    27918 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/contextlib.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1527 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/typing.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    12864 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/abc.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    79259 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/itertools.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1479 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/dataclasses.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1518 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/decimal.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1550 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/sys.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    36707 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/enum.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1468 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/textwrap.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1478 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/mmap.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   676291 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/builtins.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1493 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/time.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)        2 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/@plugins_snapshot.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1501 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/datetime.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1457 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/colorsys.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    78527 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/io.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   104419 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/codecs.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1473 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/warnings.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    51696 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pathlib.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1509 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/typing_extensions.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    24537 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/ast.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     4887 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/copy.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    70800 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/functools.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1471 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/ujson.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1474 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/_ast.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1488 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/posix.meta.json
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/
+-rw-r--r--   0 levinaden   (501) staff       (20)    13211 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/decoder.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1557 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/__init__.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     8200 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/encoder.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1475 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/encoder.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    15757 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/__init__.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1490 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/json/decoder.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1478 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/math.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    29607 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/uuid.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1482 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pickle.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   239966 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/inspect.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    13659 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/_importlib_modulespec.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    77309 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/types.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    55613 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/numbers.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1486 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/re.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   100151 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/ipaddress.data.json
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/os/
+-rw-r--r--   0 levinaden   (501) staff       (20)    74921 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/os/path.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1494 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/os/path.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1538 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/os/__init__.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   213274 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/os/__init__.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1484 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/numbers.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    82640 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/re.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1484 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/ipaddress.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1517 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/inspect.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    36528 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pickle.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1510 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/_importlib_modulespec.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1508 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/types.meta.json
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/importlib/
+-rw-r--r--   0 levinaden   (501) staff       (20)     1551 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/importlib/abc.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    28279 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/importlib/abc.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1532 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/importlib/__init__.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     5536 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/importlib/__init__.data.json
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/
+-rw-r--r--   0 levinaden   (501) staff       (20)     1768 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/fields.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1530 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/env_settings.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1633 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/json.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1695 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/class_validators.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    19470 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/error_wrappers.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     9667 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/dataclasses.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    78248 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/main.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1735 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/schema.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1689 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/version.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    58122 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/schema.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1475 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/version.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1898 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/main.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1519 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/error_wrappers.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    22579 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/class_validators.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1655 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/dataclasses.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     7675 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/env_settings.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     8111 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/json.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    46680 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/fields.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     4684 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/parse.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    30297 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/color.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    90016 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/errors.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1788 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/validators.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1759 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/utils.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     7770 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/datetime_parse.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     2031 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/__init__.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   146862 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/types.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1809 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/types.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    39414 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/validators.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1584 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/datetime_parse.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    25042 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/utils.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    14780 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/__init__.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1597 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/color.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1484 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/errors.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1528 2019-08-27 17:13:09.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pydantic/parse.meta.json
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/collections/
+-rw-r--r--   0 levinaden   (501) staff       (20)     1518 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/collections/abc.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     3518 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/collections/abc.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1541 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/collections/__init__.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   235163 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/collections/__init__.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    25070 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/math.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1478 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/uuid.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    66770 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/posix.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)   101319 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/_ast.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1514 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/ast.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1449 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/copy.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     7441 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/ujson.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1484 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/functools.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     6751 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/colorsys.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1517 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/io.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1498 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/codecs.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    17467 2019-08-27 17:13:06.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/typing_extensions.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1508 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/pathlib.meta.json
+-rw-r--r--   0 levinaden   (501) staff       (20)    28969 2019-08-27 17:13:07.000000 qcelemental-0.9.0/qcelemental/.mypy_cache/3.6/warnings.data.json
+-rw-r--r--   0 levinaden   (501) staff       (20)     1392 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/exceptions.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    18576 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/testing.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/physical_constants/
+-rw-r--r--   0 levinaden   (501) staff       (20)      386 2019-08-14 18:54:26.000000 qcelemental-0.9.0/qcelemental/physical_constants/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5936 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/physical_constants/ureg.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    18509 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/physical_constants/context.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-09-30 23:18:05.000000 qcelemental-0.9.0/qcelemental/data/
+-rw-r--r--   0 levinaden   (501) staff       (20)    74402 2019-02-15 21:10:24.000000 qcelemental-0.9.0/qcelemental/data/nist_2014_codata.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1779 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/data/mantina_2009_vanderwaals_radii.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      292 2019-09-30 13:54:51.000000 qcelemental-0.9.0/qcelemental/data/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5531 2019-08-23 18:34:22.000000 qcelemental-0.9.0/qcelemental/data/alvarez_2008_covalent_radii.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      152 2019-01-17 19:32:50.000000 qcelemental-0.9.0/qcelemental/data/README.md
+-rw-r--r--   0 levinaden   (501) staff       (20)   117788 2019-01-17 19:32:50.000000 qcelemental-0.9.0/qcelemental/data/nist_2011_atomic_weights.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      941 2019-09-30 23:18:05.000000 qcelemental-0.9.0/setup.cfg
+-rw-r--r--   0 levinaden   (501) staff       (20)    68611 2019-01-17 19:32:50.000000 qcelemental-0.9.0/versioneer.py
```

### Comparing `qcelemental-0.8.0/LICENSE` & `qcelemental-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/PKG-INFO` & `qcelemental-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qcelemental
-Version: 0.8.0
+Version: 0.9.0
 Summary: Essentials for Quantum Chemistry.
 Home-page: https://github.com/MolSSI/QCElemental
 Author: The QCArchive Development Team
 Author-email: qcarchive@molssi.org
 License: BSD-3C
 Description: # QCElemental
         
         [![Build Status](https://travis-ci.org/MolSSI/QCElemental.svg?branch=master)](https://travis-ci.org/MolSSI/QCElemental)
         [![codecov](https://codecov.io/gh/MolSSI/QCElemental/branch/master/graph/badge.svg)](https://codecov.io/gh/MolSSI/QCElemental)
         [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/MolSSI/QCElemental.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/MolSSI/QCElemental/context:python)
         [![Documentation Status](https://readthedocs.org/projects/qcelemental/badge/?version=latest)](https://qcelemental.readthedocs.io/en/latest/?badge=latest)
-        [![Chat on Slack](https://img.shields.io/badge/chat-on_slack-green.svg?longCache=true&style=flat&logo=slack)](https://join.slack.com/t/qcdb/shared_invite/enQtNDIzNTQ2OTExODk0LWM3OTgxN2ExYTlkMTlkZjA0OTExZDlmNGRlY2M4NWJlNDlkZGQyYWUxOTJmMzc3M2VlYzZjMjgxMDRkYzFmOTE)
+        [![Chat on Slack](https://img.shields.io/badge/chat-on_slack-green.svg?longCache=true&style=flat&logo=slack)](https://join.slack.com/t/qcarchive/shared_invite/enQtNDIzNTQ2OTExODk0LTE3MWI0YzBjNzVhNzczNDM0ZTA5MmQ1ODcxYTc0YTA1ZDQ2MTk1NDhlMjhjMmQ0YWYwOGMzYzJkZTM2NDlmOGM)
         ![python](https://img.shields.io/badge/python-3.6+-blue.svg)
         
         QCElemental is a resource module for quantum chemistry containing physical
         constants and periodic table data from NIST and molecule handlers.
         
         Periodic Table and Physical Constants data are pulled from NIST srd144 and
         srd121, respectively ([details](nist_data/README.md)) in a renewable manner
@@ -121,9 +121,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: align
 Provides-Extra: docs
-Provides-Extra: viz
 Provides-Extra: tests
+Provides-Extra: viz
```

### Comparing `qcelemental-0.8.0/README.md` & `qcelemental-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # QCElemental
 
 [![Build Status](https://travis-ci.org/MolSSI/QCElemental.svg?branch=master)](https://travis-ci.org/MolSSI/QCElemental)
 [![codecov](https://codecov.io/gh/MolSSI/QCElemental/branch/master/graph/badge.svg)](https://codecov.io/gh/MolSSI/QCElemental)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/MolSSI/QCElemental.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/MolSSI/QCElemental/context:python)
 [![Documentation Status](https://readthedocs.org/projects/qcelemental/badge/?version=latest)](https://qcelemental.readthedocs.io/en/latest/?badge=latest)
-[![Chat on Slack](https://img.shields.io/badge/chat-on_slack-green.svg?longCache=true&style=flat&logo=slack)](https://join.slack.com/t/qcdb/shared_invite/enQtNDIzNTQ2OTExODk0LWM3OTgxN2ExYTlkMTlkZjA0OTExZDlmNGRlY2M4NWJlNDlkZGQyYWUxOTJmMzc3M2VlYzZjMjgxMDRkYzFmOTE)
+[![Chat on Slack](https://img.shields.io/badge/chat-on_slack-green.svg?longCache=true&style=flat&logo=slack)](https://join.slack.com/t/qcarchive/shared_invite/enQtNDIzNTQ2OTExODk0LTE3MWI0YzBjNzVhNzczNDM0ZTA5MmQ1ODcxYTc0YTA1ZDQ2MTk1NDhlMjhjMmQ0YWYwOGMzYzJkZTM2NDlmOGM)
 ![python](https://img.shields.io/badge/python-3.6+-blue.svg)
 
 QCElemental is a resource module for quantum chemistry containing physical
 constants and periodic table data from NIST and molecule handlers.
 
 Periodic Table and Physical Constants data are pulled from NIST srd144 and
 srd121, respectively ([details](nist_data/README.md)) in a renewable manner
```

### Comparing `qcelemental-0.8.0/qcelemental/__init__.py` & `qcelemental-0.9.0/qcelemental/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Main init for QCElemental
 """
 
-from . import models, molparse, molutil, util
+# Handle singletons, not their classes or modules
+from . import covalent_radii, models, molparse, molutil, periodic_table, physical_constants, util, vanderwaals_radii
 from .datum import Datum
 from .exceptions import ChoicesError, DataUnavailableError, MoleculeFormatError, NotAnElementError, ValidationError
 # Handle versioneer
 from .extras import get_information
-# Handle singletons, not their classes or modules
-from . import covalent_radii, vanderwaals_radii, periodic_table, physical_constants
 # from .physical_constants import PhysicalConstantsContext, constants
 from .testing import compare, compare_recursive, compare_values
 
 # Expose singletons from the modules
 periodictable = periodic_table.periodictable
 PhysicalConstantsContext = physical_constants.PhysicalConstantsContext
 constants = physical_constants.constants
```

### Comparing `qcelemental-0.8.0/qcelemental/covalent_radii.py` & `qcelemental-0.9.0/qcelemental/covalent_radii.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains covalent radii
 """
 
 import collections
 from decimal import Decimal
-from typing import Union, Dict
+from typing import Dict, Union
 
 from .datum import Datum, print_variables
 from .exceptions import DataUnavailableError
 from .periodic_table import periodictable
 
 
 class CovalentRadii:
```

### Comparing `qcelemental-0.8.0/qcelemental/data/alvarez_2008_covalent_radii.py` & `qcelemental-0.9.0/qcelemental/data/alvarez_2008_covalent_radii.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/data/mantina_2009_vanderwaals_radii.py` & `qcelemental-0.9.0/qcelemental/data/mantina_2009_vanderwaals_radii.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/data/nist_2011_atomic_weights.py` & `qcelemental-0.9.0/qcelemental/data/nist_2011_atomic_weights.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/data/nist_2014_codata.py` & `qcelemental-0.9.0/qcelemental/data/nist_2014_codata.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/datum.py` & `qcelemental-0.9.0/qcelemental/datum.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/exceptions.py` & `qcelemental-0.9.0/qcelemental/exceptions.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/models/__init__.py` & `qcelemental-0.9.0/qcelemental/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,12 +2,13 @@
     import pydantic
 except ImportError:  # pragma: no cover
     raise ImportError("Python module pydantic not found. Solve by installing it: "
                       "`conda install pydantic -c conda-forge` or `pip install pydantic`")
 
 from . import types
 from .align import AlignmentMill
-from .basemodels import ProtoModel, AutodocBaseSettings
+from .basemodels import AutodocBaseSettings, ProtoModel
+from .basis import BasisSet
 from .common_models import ComputeError, FailedOperation, Provenance
 from .molecule import Molecule
 from .procedures import Optimization, OptimizationInput
 from .results import Result, ResultInput, ResultProperties
```

### Comparing `qcelemental-0.8.0/qcelemental/models/align.py` & `qcelemental-0.9.0/qcelemental/models/align.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/models/basemodels.py` & `qcelemental-0.9.0/qcelemental/models/basemodels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 import json
 from pathlib import Path
 from typing import Any, Dict, Optional, Set, Union
 
 import numpy as np
 from pydantic import BaseModel, BaseSettings
-from pydantic.main import MetaModel
 
 from qcelemental.testing import compare_recursive
 from qcelemental.util import deserialize, serialize
 from qcelemental.util.autodocs import AutoPydanticDocGenerator
 
 
-class PydanticAutodocMeta(MetaModel):
-    def __new__(mcs, name, bases, namespace):
-
-        ret = super().__new__(mcs, name, bases, namespace)
-        ret.__doc__ = AutoPydanticDocGenerator(ret, always_apply=True)
-        return ret
-
-
-class ProtoModel(BaseModel, metaclass=PydanticAutodocMeta):
+class ProtoModel(BaseModel):
     class Config:
         allow_mutation = False
         extra = "forbid"
         json_encoders = {np.ndarray: lambda v: v.flatten().tolist()}
         serialize_default_excludes: Set = set()
         serialize_skip_defaults = False
         force_skip_defaults = False
         canonical_repr = False
 
+    def __init_subclass__(cls) -> None:
+        cls.__doc__ = AutoPydanticDocGenerator(cls, always_apply=True)
+
     @classmethod
     def parse_raw(cls, data: Union[bytes, str], *, encoding: str = None) -> 'ProtoModel':  # type: ignore
         """
         Parses raw string or bytes into a Model object.
 
         Parameters
         ----------
@@ -161,9 +155,10 @@
     def __str__(self) -> str:  # lgtm: [py/inheritance/incorrect-overridden-signature]
         if self.__config__.canonical_repr:  # type: ignore
             return super().to_string()
         else:
             return f"{self.__class__.__name__}(ProtoModel)"
 
 
-class AutodocBaseSettings(BaseSettings, metaclass=PydanticAutodocMeta):
-    pass
+class AutodocBaseSettings(BaseSettings):
+    def __init_subclass__(cls) -> None:
+        cls.__doc__ = AutoPydanticDocGenerator(cls, always_apply=True)
```

### Comparing `qcelemental-0.8.0/qcelemental/models/common_models.py` & `qcelemental-0.9.0/qcelemental/models/common_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from .basemodels import ProtoModel
 
 # Encoders, to be deprecated
 ndarray_encoder = {np.ndarray: lambda v: v.flatten().tolist()}
 
 
 class Provenance(ProtoModel):
+    """
+    Provenance information.
+    """
     creator: str
     version: Optional[str] = None
     routine: Optional[str] = None
 
     class Config(ProtoModel.Config):
         canonical_repr = True
         extra = "allow"
@@ -35,29 +38,31 @@
 
     class Config(ProtoModel.Config):
         canonical_repr = True
         extra = "allow"
 
 
 class DriverEnum(str, Enum):
+    """Allowed quantum chemistry driver values.
+    """
     energy = 'energy'
     gradient = 'gradient'
     hessian = 'hessian'
     properties = 'properties'
 
     def derivative_int(self):
         egh = ['energy', 'gradient', 'hessian', 'third', 'fourth', 'fifth']
         if self == 'properties':
             return 0
         else:
             return egh.index(self)
 
 
 class ComputeError(ProtoModel):
-    """The type of error message raised"""
+    """A complete description of the error."""
     error_type: str = Schema(  # type: ignore
         ...,  # Error enumeration not yet strict
         description="The type of error which was thrown. Restrict this field short classifiers e.g. 'input_error'.")
     error_message: str = Schema(  # type: ignore
         ...,
         description="Text associated with the thrown error, often the backtrace, but can contain additional "
         "information as well.")
```

### Comparing `qcelemental-0.8.0/qcelemental/models/molecule.py` & `qcelemental-0.9.0/qcelemental/models/molecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 from pydantic import Schema, constr, validator
 
 from ..molparse import from_arrays, from_schema, from_string, to_schema, to_string
 from ..periodic_table import periodictable
 from ..physical_constants import constants
 from ..testing import compare, compare_values
-from ..util import deserialize, measure_coordinates, provenance_stamp, which_import, msgpackext_loads
+from ..util import deserialize, measure_coordinates, msgpackext_loads, provenance_stamp, which_import
 from .basemodels import ProtoModel
 from .common_models import Provenance, qcschema_molecule_default
 from .types import Array
 
 # Rounding quantities for hashing
 GEOMETRY_NOISE = 8
 MASS_NOISE = 6
```

### Comparing `qcelemental-0.8.0/qcelemental/models/types.py` & `qcelemental-0.9.0/qcelemental/models/types.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/chgmult.py` & `qcelemental-0.9.0/qcelemental/molparse/chgmult.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/from_arrays.py` & `qcelemental-0.9.0/qcelemental/molparse/from_arrays.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/from_schema.py` & `qcelemental-0.9.0/qcelemental/molparse/from_schema.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/from_string.py` & `qcelemental-0.9.0/qcelemental/molparse/from_string.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/nucleus.py` & `qcelemental-0.9.0/qcelemental/molparse/nucleus.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/pubchem.py` & `qcelemental-0.9.0/qcelemental/molparse/pubchem.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/regex.py` & `qcelemental-0.9.0/qcelemental/molparse/regex.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/to_schema.py` & `qcelemental-0.9.0/qcelemental/molparse/to_schema.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molparse/to_string.py` & `qcelemental-0.9.0/qcelemental/molparse/to_string.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import collections
-from typing import Dict, Any, List, Union, Tuple
+from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 
 from ..physical_constants import constants
 
 
 def to_string(molrec: Dict,
@@ -17,15 +17,15 @@
               return_data: bool = False) -> Union[str, Tuple[str, Dict]]:
     """Format a string representation of QM molecule.
 
     Parameters
     ----------
     molrec : Dict
         Psi4 json Molecule spec.
-    dtype : str, {'xyz', 'cfour', 'nwchem', 'molpro'}
+    dtype : str, {'xyz', 'cfour', 'nwchem', 'molpro', 'turbomole'}
         Overall string format. Note that it's possible to request variations
         that don't fit the dtype spec so may not be re-readable (e.g., ghost
         and mass in nucleus label with ``'xyz'``).
         'cfour' forces nucleus label, ignoring atom_format, ghost_format
     units : str, optional
         Units in which to write string. Usually ``Angstrom`` or ``Bohr``
         but may be any length unit.  There is not an option to write in
@@ -70,15 +70,16 @@
     default_units = {
         "xyz": "Angstrom",
         "cfour": "Bohr",
         "gamess": "Bohr",
         "molpro": "Bohr",
         "nwchem": "Bohr",
         "psi4": "Bohr",
-        "terachem": "Bohr"
+        "terachem": "Bohr",
+        "turbomole": "Bohr",
     }
     if dtype not in default_units:
         raise KeyError(f"dtype '{dtype}' not understood.")
 
     # Handle units
     if units is None:
         units = default_units[dtype]
@@ -285,28 +286,42 @@
             'fragment_multiplicities',
             'fix_com',
             'fix_orientation',
             'real',
         ])
         data.keywords = {}
 
+    elif dtype == 'turbomole':
+        # In Turbomole coord files the coordinates come first, and the atomic
+        # symbol comes afterwards.
+        # Handling of ghost atoms is done in the basis section of the control
+        # file by setting the nuclear charge of certain atoms to zero.
+        atom_format = '{elem}'
+        ghost_format = '{elem}'
+        umap = {'bohr': 'bohr'}
+        umap[units.lower()]  # trigger error if downstream can't handle
+
+        atoms = _atoms_formatter(molrec, geom, atom_format, ghost_format, width, prec, 2, xyze=True)
+        atoms = [at.lower() for at in atoms]
+
+        smol = ["$coord"] + atoms + ["$end"]
+
     else:
         raise KeyError(f"dtype '{dtype}' not understood.")
 
     smol_ret = '\n'.join(smol) + '\n'
     if return_data:
         return smol_ret, data.to_dict()
     else:
         return smol_ret
 
 
-def _atoms_formatter(molrec, geom, atom_format, ghost_format, width, prec, sp):
+def _atoms_formatter(molrec, geom, atom_format, ghost_format, width, prec, sp, xyze=False):
     """Format a list of strings, one per atom from `molrec`."""
 
-    #geom = molrec['geom'].reshape((-1, 3))
     nat = geom.shape[0]
     fxyz = """{:>{width}.{prec}f}"""
     sp = """{:{sp}}""".format('', sp=sp)
 
     atoms = []
     for iat in range(nat):
         atom = []
@@ -325,14 +340,16 @@
             if ghost_format == '':
                 continue
             else:
                 nuc = """{:{width}}""".format(ghost_format.format(**atominfo), width=width)
                 atom.append(nuc)
 
         atom.extend([fxyz.format(x, width=width, prec=prec) for x in geom[iat]])
+        if xyze:
+            atom.append(atom.pop(0).rstrip())
         atoms.append(sp.join(atom))
 
     return atoms
 
 
 def formula_generator(elem):
     """Return simple chemical formula from element list `elem`.
```

### Comparing `qcelemental-0.8.0/qcelemental/molutil/align.py` & `qcelemental-0.9.0/qcelemental/molutil/align.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/molutil/test_align.py` & `qcelemental-0.9.0/qcelemental/molutil/test_align.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/periodic_table.py` & `qcelemental-0.9.0/qcelemental/periodic_table.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/physical_constants/context.py` & `qcelemental-0.9.0/qcelemental/physical_constants/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Contains relevant physical constants
 """
 
 import collections
 from decimal import Decimal
 from functools import lru_cache
-from typing import Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
 from ..datum import Datum, print_variables
 from .ureg import build_units_registry
 
 if TYPE_CHECKING:
     from pint import quantity, UnitRegistry  # lgtm: [py/unused-import]
```

### Comparing `qcelemental-0.8.0/qcelemental/physical_constants/ureg.py` & `qcelemental-0.9.0/qcelemental/physical_constants/ureg.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/testing.py` & `qcelemental-0.9.0/qcelemental/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import logging
 import pprint
 import sys
-from typing import Callable, List, Dict, Union
+from typing import Callable, Dict, List, Union
 
 import numpy as np
 from pydantic import BaseModel
 
 pp = pprint.PrettyPrinter(width=120)
```

### Comparing `qcelemental-0.8.0/qcelemental/tests/addons.py` & `qcelemental-0.9.0/qcelemental/tests/addons.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_constants.py` & `qcelemental-0.9.0/qcelemental/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_covalentradii.py` & `qcelemental-0.9.0/qcelemental/tests/test_covalentradii.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_datum.py` & `qcelemental-0.9.0/qcelemental/tests/test_datum.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_importing.py` & `qcelemental-0.9.0/qcelemental/tests/test_importing.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_model_serials.py` & `qcelemental-0.9.0/qcelemental/tests/test_model_serials.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molecule.py` & `qcelemental-0.9.0/qcelemental/tests/test_molecule.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_align_chiral.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_align_chiral.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_from_schema.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_from_schema.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_from_string.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_from_string.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_parse_nucleus_label.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_parse_nucleus_label.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_pubchem.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_pubchem.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_reconcile_nucleus.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_reconcile_nucleus.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_to_schema.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_to_schema.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_to_string.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_to_string.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,14 +132,22 @@
 H                    -1.058354421340     0.000000000000     0.000000000000
 }
 dummy,2
 set,charge=0.0
 set,spin=2
 """,
 
+"ans2_turbomole_au": """$coord
+   0.000000000000     0.000000000000     0.000000000000  co
+   2.000000000000     0.000000000000     0.000000000000  h
+  -2.000000000000     0.000000000000     0.000000000000  h
+$end
+"""
+
+
 }  # yapf: disable
 
 
 @pytest.mark.parametrize("inp,expected", [
     (("subject1", {'dtype': 'xyz', 'units': 'Bohr'}), "ans1_au"),
     (("subject1", {'dtype': 'xyz', 'units': 'Angstrom'}), "ans1_ang"),
     (("subject1", {'dtype': 'xyz', 'prec': 8, 'atom_format': '{elea}{elem}{elbl}'}), "ans1c_ang"),
@@ -150,14 +158,15 @@
     (("subject2", {'dtype': 'nwchem', 'units': 'angstrom'}), "ans2_nwchem_ang"),
     (("subject1", {'dtype': 'xyz', 'units': 'nm', 'prec': 8, 'atom_format': '{elea}{elem}{elbl}'}), "ans1c_nm"),
     (("subject2", {'dtype': 'terachem', 'units': 'angstrom'}), "ans2_terachem_ang"),
     (("subject2", {'dtype': 'terachem'}), "ans2_terachem_au"),
     (("subject2", {'dtype': 'psi4', 'units': 'bohr'}), "ans2_psi4_au"),
     (("subject2", {'dtype': 'molpro', 'units': 'bohr'}), "ans2_molpro_au"),
     (("subject2", {'dtype': 'molpro', 'units': 'angstrom'}), "ans2_molpro_ang"),
+    (("subject2", {'dtype': 'turbomole', 'units': 'bohr'}), "ans2_turbomole_au"),
 ])  # yapf: disable
 def test_to_string_xyz(inp, expected):
     molrec = qcelemental.molparse.from_string(_results[inp[0]])
     smol = qcelemental.molparse.to_string(molrec['qm'], **inp[1])
     print(smol)
 
     assert compare(_results[expected], smol)
```

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_molparse_validate_and_fill_chgmult.py` & `qcelemental-0.9.0/qcelemental/tests/test_molparse_validate_and_fill_chgmult.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_periodictable.py` & `qcelemental-0.9.0/qcelemental/tests/test_periodictable.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_testing.py` & `qcelemental-0.9.0/qcelemental/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_units.py` & `qcelemental-0.9.0/qcelemental/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_utils.py` & `qcelemental-0.9.0/qcelemental/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/tests/test_vanderwaalsradii.py` & `qcelemental-0.9.0/qcelemental/tests/test_vanderwaalsradii.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/__init__.py` & `qcelemental-0.9.0/qcelemental/util/__init__.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/autodocs.py` & `qcelemental-0.9.0/qcelemental/util/autodocs.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/gph_uno_bipartite.py` & `qcelemental-0.9.0/qcelemental/util/gph_uno_bipartite.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/importing.py` & `qcelemental-0.9.0/qcelemental/util/importing.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/itertools.py` & `qcelemental-0.9.0/qcelemental/util/itertools.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/misc.py` & `qcelemental-0.9.0/qcelemental/util/misc.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/np_blockwise.py` & `qcelemental-0.9.0/qcelemental/util/np_blockwise.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/np_rand3drot.py` & `qcelemental-0.9.0/qcelemental/util/np_rand3drot.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/scipy_hungarian.py` & `qcelemental-0.9.0/qcelemental/util/scipy_hungarian.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/serialization.py` & `qcelemental-0.9.0/qcelemental/util/serialization.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/test_gph_uno_bipartite.py` & `qcelemental-0.9.0/qcelemental/util/test_gph_uno_bipartite.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/util/test_scipy_hungarian.py` & `qcelemental-0.9.0/qcelemental/util/test_scipy_hungarian.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/qcelemental/vanderwaals_radii.py` & `qcelemental-0.9.0/qcelemental/vanderwaals_radii.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains van der Waals radii
 """
 
 import collections
 from decimal import Decimal
-from typing import Union, Dict
+from typing import Dict, Union
 
 from .datum import Datum, print_variables
 from .exceptions import DataUnavailableError
 from .periodic_table import periodictable
 
 
 class VanderWaalsRadii:
```

### Comparing `qcelemental-0.8.0/qcelemental.egg-info/PKG-INFO` & `qcelemental-0.9.0/qcelemental.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qcelemental
-Version: 0.8.0
+Version: 0.9.0
 Summary: Essentials for Quantum Chemistry.
 Home-page: https://github.com/MolSSI/QCElemental
 Author: The QCArchive Development Team
 Author-email: qcarchive@molssi.org
 License: BSD-3C
 Description: # QCElemental
         
         [![Build Status](https://travis-ci.org/MolSSI/QCElemental.svg?branch=master)](https://travis-ci.org/MolSSI/QCElemental)
         [![codecov](https://codecov.io/gh/MolSSI/QCElemental/branch/master/graph/badge.svg)](https://codecov.io/gh/MolSSI/QCElemental)
         [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/MolSSI/QCElemental.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/MolSSI/QCElemental/context:python)
         [![Documentation Status](https://readthedocs.org/projects/qcelemental/badge/?version=latest)](https://qcelemental.readthedocs.io/en/latest/?badge=latest)
-        [![Chat on Slack](https://img.shields.io/badge/chat-on_slack-green.svg?longCache=true&style=flat&logo=slack)](https://join.slack.com/t/qcdb/shared_invite/enQtNDIzNTQ2OTExODk0LWM3OTgxN2ExYTlkMTlkZjA0OTExZDlmNGRlY2M4NWJlNDlkZGQyYWUxOTJmMzc3M2VlYzZjMjgxMDRkYzFmOTE)
+        [![Chat on Slack](https://img.shields.io/badge/chat-on_slack-green.svg?longCache=true&style=flat&logo=slack)](https://join.slack.com/t/qcarchive/shared_invite/enQtNDIzNTQ2OTExODk0LTE3MWI0YzBjNzVhNzczNDM0ZTA5MmQ1ODcxYTc0YTA1ZDQ2MTk1NDhlMjhjMmQ0YWYwOGMzYzJkZTM2NDlmOGM)
         ![python](https://img.shields.io/badge/python-3.6+-blue.svg)
         
         QCElemental is a resource module for quantum chemistry containing physical
         constants and periodic table data from NIST and molecule handlers.
         
         Periodic Table and Physical Constants data are pulled from NIST srd144 and
         srd121, respectively ([details](nist_data/README.md)) in a renewable manner
@@ -121,9 +121,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: align
 Provides-Extra: docs
-Provides-Extra: viz
 Provides-Extra: tests
+Provides-Extra: viz
```

### Comparing `qcelemental-0.8.0/setup.cfg` & `qcelemental-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/setup.py` & `qcelemental-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `qcelemental-0.8.0/versioneer.py` & `qcelemental-0.9.0/versioneer.py`

 * *Files identical despite different names*

