# Comparing `tmp/fleck-0.0.dev72.tar.gz` & `tmp/fleck-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fleck-0.0.dev72.tar", last modified: Fri Aug 28 14:57:21 2020, max compression
+gzip compressed data, was "fleck-1.1.tar", last modified: Mon Jul 31 14:19:28 2023, max compression
```

## Comparing `fleck-0.0.dev72.tar` & `fleck-1.1.tar`

### file list

```diff
@@ -1,95 +1,74 @@
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/
--rw-r--r--   0 bmmorris   (501) staff       (20)      345 2020-08-28 14:57:21.000000 fleck-0.0.dev72/PKG-INFO
--rw-r--r--   0 bmmorris   (501) staff       (20)     1541 2020-02-14 02:05:31.000000 fleck-0.0.dev72/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    35654 2019-02-27 15:16:59.000000 fleck-0.0.dev72/ah_bootstrap.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/
--rw-r--r--   0 bmmorris   (501) staff       (20)    19190 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/CHANGES.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1491 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/LICENSE.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    14206 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    35654 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/ah_bootstrap.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/
--rw-r--r--   0 bmmorris   (501) staff       (20)     1738 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/__init__.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2738 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    19821 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    10072 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/build_sphinx.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      120 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/setup_package.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/src/
--rw-r--r--   0 bmmorris   (501) staff       (20)     3033 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-r--r--   0 bmmorris   (501) staff       (20)     1283 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/commands/test.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1930 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/conftest.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     7922 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/distutils_helpers.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     6465 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/git_helpers.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     9381 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/openmp_helpers.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    26278 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/sphinx/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      156 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/sphinx/conf.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    24773 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/utils.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      604 2019-02-27 16:25:22.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/version.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     9728 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers/version_helpers.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers.egg-info/
--rw-r--r--   0 bmmorris   (501) staff       (20)    17995 2019-02-27 16:25:22.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 bmmorris   (501) staff       (20)      919 2019-02-27 16:25:22.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)        1 2019-02-27 16:25:22.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)        1 2019-02-27 16:25:22.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-r--r--   0 bmmorris   (501) staff       (20)       16 2019-02-27 16:25:22.000000 fleck-0.0.dev72/astropy_helpers/astropy_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/astropy_helpers/licenses/
--rw-r--r--   0 bmmorris   (501) staff       (20)     1644 2019-02-27 15:16:58.000000 fleck-0.0.dev72/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/docs/
--rw-r--r--   0 bmmorris   (501) staff       (20)     4581 2019-02-27 15:16:56.000000 fleck-0.0.dev72/docs/Makefile
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/docs/_templates/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/docs/_templates/autosummary/
--rw-r--r--   0 bmmorris   (501) staff       (20)      250 2019-02-27 15:14:50.000000 fleck-0.0.dev72/docs/_templates/autosummary/base.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      251 2019-02-27 15:14:50.000000 fleck-0.0.dev72/docs/_templates/autosummary/class.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      252 2019-02-27 15:14:50.000000 fleck-0.0.dev72/docs/_templates/autosummary/module.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     7387 2019-02-27 15:16:56.000000 fleck-0.0.dev72/docs/conf.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/docs/fleck/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/docs/fleck/bayes/
--rw-r--r--   0 bmmorris   (501) staff       (20)     5370 2020-02-14 07:14:24.000000 fleck-0.0.dev72/docs/fleck/bayes/abc.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/docs/fleck/bayes/images/
--rw-r--r--   0 bmmorris   (501) staff       (20)  1721489 2020-02-14 03:43:34.000000 fleck-0.0.dev72/docs/fleck/bayes/images/corner.png
--rw-r--r--   0 bmmorris   (501) staff       (20)   139919 2020-02-14 04:42:53.000000 fleck-0.0.dev72/docs/fleck/bayes/images/corner_pra.png
--rw-r--r--   0 bmmorris   (501) staff       (20)    89422 2020-02-14 03:43:58.000000 fleck-0.0.dev72/docs/fleck/bayes/images/posterior.png
--rw-r--r--   0 bmmorris   (501) staff       (20)     6614 2020-02-14 07:30:04.000000 fleck-0.0.dev72/docs/fleck/bayes/mcmc.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     4683 2019-03-15 18:09:15.000000 fleck-0.0.dev72/docs/fleck/details.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     9428 2020-06-26 10:58:16.000000 fleck-0.0.dev72/docs/fleck/dr.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     8891 2020-03-01 15:09:36.000000 fleck-0.0.dev72/docs/fleck/gettingstarted.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      154 2019-03-12 03:24:53.000000 fleck-0.0.dev72/docs/fleck/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      468 2019-03-13 03:36:33.000000 fleck-0.0.dev72/docs/fleck/installation.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1316 2020-06-26 10:40:13.000000 fleck-0.0.dev72/docs/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     4549 2019-02-27 15:16:56.000000 fleck-0.0.dev72/docs/make.bat
--rw-r--r--   0 bmmorris   (501) staff       (20)     7221 2020-03-06 18:00:47.000000 fleck-0.0.dev72/docs/paper.bib
--rw-r--r--   0 bmmorris   (501) staff       (20)     3236 2020-06-26 07:04:39.000000 fleck-0.0.dev72/docs/paper.md
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/
--rw-r--r--   0 bmmorris   (501) staff       (20)      871 2019-02-27 15:49:45.000000 fleck-0.0.dev72/fleck/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2023 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/_astropy_init.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2513 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/conftest.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    30228 2020-08-28 14:49:53.000000 fleck-0.0.dev72/fleck/core.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/data/
--rw-r--r--   0 bmmorris   (501) staff       (20)      246 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/data/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    25000 2019-03-12 17:16:25.000000 fleck-0.0.dev72/fleck/data/stsp_double_transit.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)    25000 2019-03-05 19:57:04.000000 fleck-0.0.dev72/fleck/data/stsp_rotation.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)    12500 2019-03-12 00:17:04.000000 fleck-0.0.dev72/fleck/data/stsp_single_transit.txt
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/extern/
--rw-r--r--   0 bmmorris   (501) staff       (20)      366 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/extern/__init__.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/tests/
--rw-r--r--   0 bmmorris   (501) staff       (20)      108 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/tests/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      768 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/tests/coveragerc
--rw-r--r--   0 bmmorris   (501) staff       (20)      289 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/tests/setup_package.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     4192 2020-08-28 14:51:30.000000 fleck-0.0.dev72/fleck/tests/test_core.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/utils/
--rw-r--r--   0 bmmorris   (501) staff       (20)      148 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/utils/__init__.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/utils/tests/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2019-02-27 15:16:56.000000 fleck-0.0.dev72/fleck/utils/tests/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     7382 2020-08-28 14:57:21.000000 fleck-0.0.dev72/fleck/version.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2020-08-28 14:57:21.000000 fleck-0.0.dev72/licenses/
--rw-r--r--   0 bmmorris   (501) staff       (20)     9722 2019-02-27 15:16:56.000000 fleck-0.0.dev72/licenses/APACHE2.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1282 2019-02-27 15:16:56.000000 fleck-0.0.dev72/licenses/BSD2.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1487 2019-02-27 15:16:56.000000 fleck-0.0.dev72/licenses/BSD3.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    37570 2019-02-27 15:16:56.000000 fleck-0.0.dev72/licenses/GPLv3.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      372 2019-02-27 15:16:56.000000 fleck-0.0.dev72/licenses/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1659 2019-02-27 15:16:56.000000 fleck-0.0.dev72/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1209 2020-08-28 14:50:38.000000 fleck-0.0.dev72/setup.cfg
--rwxr-xr-x   0 bmmorris   (501) staff       (20)     5312 2019-02-27 15:16:56.000000 fleck-0.0.dev72/setup.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.911644 fleck-1.1/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.890880 fleck-1.1/.github/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.894882 fleck-1.1/.github/workflows/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      482 2023-07-30 01:12:25.000000 fleck-1.1/.github/workflows/ci.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      679 2022-12-13 02:39:39.000000 fleck-1.1/.gitignore
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      606 2023-07-30 00:31:46.000000 fleck-1.1/.readthedocs.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1072 2022-12-13 02:39:39.000000 fleck-1.1/LICENSE
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1058 2022-12-13 02:39:39.000000 fleck-1.1/MANIFEST.in
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3082 2023-07-31 14:19:28.911782 fleck-1.1/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1424 2023-07-30 00:30:23.000000 fleck-1.1/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.896488 fleck-1.1/docs/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       98 2023-07-28 18:37:19.000000 fleck-1.1/docs/.rtd_environment.yaml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2719 2023-07-30 00:33:03.000000 fleck-1.1/docs/Makefile
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.891158 fleck-1.1/docs/_templates/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.897257 fleck-1.1/docs/_templates/autosummary/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2022-12-13 02:39:39.000000 fleck-1.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-12-13 02:39:39.000000 fleck-1.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2022-12-13 02:39:39.000000 fleck-1.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5895 2023-07-30 00:32:39.000000 fleck-1.1/docs/conf.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.898555 fleck-1.1/docs/fleck/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.899057 fleck-1.1/docs/fleck/bayes/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5370 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/bayes/abc.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.904534 fleck-1.1/docs/fleck/bayes/images/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)  1721489 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/bayes/images/corner.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   139919 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/bayes/images/corner_pra.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    89422 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/bayes/images/posterior.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6614 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/bayes/mcmc.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4683 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/details.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9428 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/dr.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9212 2023-07-30 00:59:30.000000 fleck-1.1/docs/fleck/gettingstarted.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      154 2022-12-13 02:39:39.000000 fleck-1.1/docs/fleck/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      309 2023-07-30 00:51:39.000000 fleck-1.1/docs/fleck/installation.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1316 2022-12-13 02:39:39.000000 fleck-1.1/docs/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     7221 2022-12-13 02:39:39.000000 fleck-1.1/docs/paper.bib
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3236 2022-12-13 02:39:39.000000 fleck-1.1/docs/paper.md
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      886 2022-12-13 02:39:39.000000 fleck-1.1/example.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.906654 fleck-1.1/fleck/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      367 2023-07-30 00:33:52.000000 fleck-1.1/fleck/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      878 2023-07-30 00:36:08.000000 fleck-1.1/fleck/conftest.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    30897 2023-07-30 01:10:45.000000 fleck-1.1/fleck/core.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       59 2023-01-18 21:10:32.000000 fleck-1.1/fleck/cython_version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.908799 fleck-1.1/fleck/data/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      246 2022-12-13 02:39:39.000000 fleck-1.1/fleck/data/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    25000 2022-12-13 02:39:39.000000 fleck-1.1/fleck/data/stsp_double_transit.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    25000 2022-12-13 02:39:39.000000 fleck-1.1/fleck/data/stsp_rotation.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    12500 2022-12-13 02:39:39.000000 fleck-1.1/fleck/data/stsp_single_transit.txt
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.908995 fleck-1.1/fleck/extern/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      366 2022-12-13 02:39:39.000000 fleck-1.1/fleck/extern/__init__.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.909640 fleck-1.1/fleck/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      108 2022-12-13 02:39:39.000000 fleck-1.1/fleck/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4192 2022-12-13 02:39:39.000000 fleck-1.1/fleck/tests/test_core.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.909853 fleck-1.1/fleck/utils/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      148 2022-12-13 02:39:39.000000 fleck-1.1/fleck/utils/__init__.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.910040 fleck-1.1/fleck/utils/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-12-13 02:39:39.000000 fleck-1.1/fleck/utils/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      155 2023-07-31 14:19:28.000000 fleck-1.1/fleck/version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.907748 fleck-1.1/fleck.egg-info/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3082 2023-07-31 14:19:28.000000 fleck-1.1/fleck.egg-info/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1269 2023-07-31 14:19:28.000000 fleck-1.1/fleck.egg-info/SOURCES.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-31 14:19:28.000000 fleck-1.1/fleck.egg-info/dependency_links.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2022-12-13 02:39:52.000000 fleck-1.1/fleck.egg-info/not-zip-safe
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      247 2023-07-31 14:19:28.000000 fleck-1.1/fleck.egg-info/requires.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       31 2023-07-31 14:19:28.000000 fleck-1.1/fleck.egg-info/top_level.txt
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 14:19:28.911481 fleck-1.1/licenses/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9722 2022-12-13 02:39:39.000000 fleck-1.1/licenses/APACHE2.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1282 2022-12-13 02:39:39.000000 fleck-1.1/licenses/BSD2.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1487 2022-12-13 02:39:39.000000 fleck-1.1/licenses/BSD3.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    37570 2022-12-13 02:39:39.000000 fleck-1.1/licenses/GPLv3.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      372 2022-12-13 02:39:39.000000 fleck-1.1/licenses/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1659 2022-12-13 02:39:39.000000 fleck-1.1/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2043 2023-07-30 00:53:16.000000 fleck-1.1/pyproject.toml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      954 2023-07-31 14:19:28.912198 fleck-1.1/setup.cfg
+-rwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)       61 2023-07-30 00:30:07.000000 fleck-1.1/setup.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1757 2023-07-30 00:38:15.000000 fleck-1.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fleck-0.0.dev72/README.rst` & `fleck-1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 *****
 fleck
 *****
 
-.. image:: https://travis-ci.org/bmorris3/fleck.svg?branch=master
-    :target: https://travis-ci.org/bmorris3/fleck
-
 .. image:: https://readthedocs.org/projects/fleck/badge/?version=latest
     :target: https://fleck.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
```

### Comparing `fleck-0.0.dev72/astropy_helpers/LICENSE.rst` & `fleck-1.1/licenses/BSD3.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-Copyright (c) 2014, Astropy Developers
-
+Copyright (c) 2019, Brett M. Morris
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `fleck-0.0.dev72/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst` & `fleck-1.1/licenses/TEMPLATE_LICENCE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# The OpenMP helpers include code heavily adapted from astroscrappy, released
-# under the following license:
-#
-# Copyright (c) 2015, Curtis McCully
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-# * Redistributions of source code must retain the above copyright notice, this
-#   list of conditions and the following disclaimer.
-# * Redistributions in binary form must reproduce the above copyright notice, this
-#   list of conditions and the following disclaimer in the documentation and/or
-#   other materials provided with the distribution.
-# * Neither the name of the Astropy Team nor the names of its contributors may be
-#   used to endorse or promote products derived from this software without
-#   specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+This project is based upon the Astropy package template
+(https://github.com/astropy/package-template/) which is licenced under the terms
+of the following licence.
+
+---
+
+Copyright (c) 2018, Astropy Developers
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+* Neither the name of the Astropy Team nor the names of its contributors may be
+  used to endorse or promote products derived from this software without
+  specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `fleck-0.0.dev72/docs/fleck/bayes/abc.rst` & `fleck-1.1/docs/fleck/bayes/abc.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/bayes/images/corner.png` & `fleck-1.1/docs/fleck/bayes/images/corner.png`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/bayes/images/corner_pra.png` & `fleck-1.1/docs/fleck/bayes/images/corner_pra.png`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/bayes/images/posterior.png` & `fleck-1.1/docs/fleck/bayes/images/posterior.png`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/bayes/mcmc.rst` & `fleck-1.1/docs/fleck/bayes/mcmc.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/details.rst` & `fleck-1.1/docs/fleck/details.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/dr.rst` & `fleck-1.1/docs/fleck/dr.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/fleck/gettingstarted.rst` & `fleck-1.1/docs/fleck/gettingstarted.rst`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 ---------------------
 
 Suppose you want to observe 100 stars with randomly drawn stellar inclinations,
 each with spot contrast ``c=0.7`` (where ``c=0`` means perfectly dark spots),
 with quadratic limb-darkening. Let's distribute three spots on each star
 randomly above 70 degrees latitude up to the pole. We can use the
 `~fleck.generate_spots` method to quickly create spot property matrices in the
-correct shape::
+correct shape:
+
+.. code-block:: python
 
     from fleck import generate_spots
 
     spot_contrast = 0.7
     u_ld = [0.5079, 0.2239]
 
     n_phases = 30
@@ -27,29 +29,33 @@
 
     lons, lats, radii, inc_stellar = generate_spots(min_latitude, max_latitude,
                                                     spot_radius, n_spots,
                                                     n_inclinations=n_inclinations)
 
 ``lons, lats, radii`` will each have shape ``(n_spots, n_inclinations)`` and
 ``inc_stellar`` will have shape ``(n_inclinations, )``. Now let's initialize
-a `~fleck.Star` object::
+a `~fleck.Star` object:
+
+.. code-block:: python
 
     from fleck import Star
 
     star = Star(spot_contrast=spot_contrast, n_phases=n_phases, u_ld=u_ld)
 
 If we initialize the `~fleck.Star` object with a number of phases ``n_phases``,
 it will evenly sample all phases on :math:`(0, 2\pi)`.
 
 Now we can compute light curves for stars with the spots we generated like so::
 
     lcs = star.light_curve(lons, lats, radii, inc_stellar)
 
 where ``lcs`` will have shape ``(n_phases, n_inclinations)``. Let's plot each of
-the light curves::
+the light curves:
+
+.. code-block:: python
 
     import matplotlib.pyplot as plt
     plt.plot(star.phases, lcs)
     plt.show()
 
 .. plot::
 
@@ -80,15 +86,17 @@
     plt.show()
 
 Spot Occultations
 -----------------
 
 Now let's make a transiting exoplanet, and observe spot occultations. We can
 specify the parameters of the transiting exoplanet using the same specification
-used by `batman <https://github.com/lkreidberg/batman>`_::
+used by `batman <https://github.com/lkreidberg/batman>`_:
+
+.. code-block:: python
 
     from batman import TransitParams
     import astropy.units as u
 
     planet = TransitParams()
     planet.per = 88
     planet.a = float(0.387*u.AU / u.R_sun)
@@ -96,41 +104,51 @@
     planet.w = 90
     planet.ecc = 0
     planet.inc = 90
     planet.t0 = 0
     planet.limb_dark = 'quadratic'
     planet.u = [0.5079, 0.2239]
 
-Let's now specify some spots on the stellar surface::
+Let's now specify some spots on the stellar surface:
+
+.. code-block:: python
 
     import numpy as np
 
     inc_stellar = 90 * u.deg
     spot_radii = np.array([[0.1], [0.1]])
     spot_lats = np.array([[0], [0]]) * u.deg
     spot_lons = np.array([[360-30], [30]]) * u.deg
 
-and some times at which to observe the system::
+and some times at which to observe the system:
+
+.. code-block:: python
 
     times = np.linspace(-0.5, 0.5, 500)
 
 let's initialize our `~fleck.Star` object, specifying a stellar rotation
-period::
+period:
+
+.. code-block:: python
 
     from fleck import Star
     star = Star(spot_contrast=0.7, u_ld=planet.u, rotation_period=10)
 
 We generate a light curve using the same `~fleck.Star.light_curve` method that
 we used earlier, but this time we will supply it with the planet's parameters
-and the times at which to evaluate the model::
+and the times at which to evaluate the model:
+
+.. code-block:: python
 
     lc = star.light_curve(spot_lons, spot_lats, spot_radii,
                           inc_stellar, planet=planet, times=times)
 
-Finally we can plot the transit light curve::
+Finally we can plot the transit light curve:
+
+.. code-block:: python
 
     import matplotlib.pyplot as plt
     plt.plot(times, lc, color='k')
     plt.show()
 
 .. plot::
 
@@ -168,15 +186,17 @@
 
 
 Plotting
 --------
 
 You can make quick plots for debugging and understanding a system's geometry
 using the `~fleck.Star.plot` method. For example, let's create a star observed
-at an odd angle, with a misaligned planet::
+at an odd angle, with a misaligned planet:
+
+.. code-block:: python
 
     from batman import TransitParams
     import matplotlib.pyplot as plt
     import numpy as np
     import astropy.units as u
     from fleck import Star
 
@@ -189,31 +209,38 @@
     planet.inc = 89.65
     planet.t0 = 0
     planet.limb_dark = 'quadratic'
     planet.u = [0.5079, 0.2239]
 
 We define the angular offset between the planet's orbit normal and the spin the
 star projected onto the sky plane (often denoted :math:`\lambda`) using the
-extra planet parameter `planet.lam`, in units of degrees::
+extra planet parameter `planet.lam`, in units of degrees:
 
-    planet.lam = 45
+.. code-block:: python
 
+    planet.lam = 45
 
 The stellar inclination (measured away from the sub-observer point) often
-denoted :math:`i_s` is defined::
+denoted :math:`i_s` is defined:
+
+.. code-block:: python
 
     inc_stellar = 70 * u.deg
 
-Let's create two spots along one line of longitude::
+Let's create two spots along one line of longitude:
+
+.. code-block:: python
 
     spot_radii = np.array([[0.1], [0.1]])
     spot_lons = np.array([[0], [0]]) * u.deg
     spot_lats = np.array([[25], [-25]]) * u.deg
 
-Let's now observe the system::
+Let's now observe the system:
+
+.. code-block:: python
 
     times = np.linspace(-0.5, 0.5, 500)
 
     star = Star(spot_contrast=0.7, u_ld=planet.u, rotation_period=10)
     ax = star.plot(spot_lons, spot_lats, spot_radii, inc_stellar, planet=planet,
                    time=0)
```

### Comparing `fleck-0.0.dev72/docs/index.rst` & `fleck-1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/paper.bib` & `fleck-1.1/docs/paper.bib`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/docs/paper.md` & `fleck-1.1/docs/paper.md`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/fleck/core.py` & `fleck-1.1/fleck/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     """
     Iteratively identify a continuous path from the given points xy_coord,
     starting by the point indexed by k0
     """
     n = len(xy_coord)
     distance_matrix = squareform(pdist(xy_coord, metric='euclidean'))
     mask = np.ones(n, dtype='bool')
-    sorted_order = np.zeros(n, dtype=np.int)
+    sorted_order = np.zeros(n, dtype=int)
     indices = np.arange(n)
 
     i = 0
     k = k0
     while True:
         sorted_order[i] = k
         mask[k] = False
@@ -439,19 +439,24 @@
                 if tilted_spots.x.value[t0_ind, i] > 0:
                     spot_y = tilted_spots.y.value[t0_ind, i]
                     spot_z = tilted_spots.z.value[t0_ind, i]
 
                     # Compute the spot position and ellipsoidal shape
                     r_spot = np.hypot(spot_z, spot_y)
                     angle = np.arctan2(spot_z, spot_y)
-                    ellipse_centroid = [spot_y, spot_z]
-
-                    ellipse_axes = [spot_radii[i, 0] *
-                                    np.sqrt(1 - r_spot**2),
-                                    spot_radii[i, 0]]
+                    ellipse_centroid = np.array([
+                        np.squeeze(spot_y),
+                        np.squeeze(spot_z)
+                    ])
+
+                    ellipse_axes = np.array([
+                        np.squeeze(spot_radii[i, 0] *
+                                   np.sqrt(1 - r_spot**2)),
+                        np.squeeze(spot_radii[i, 0])
+                    ])
 
                     spot = ellipse(ellipse_centroid, ellipse_axes,
                                    np.degrees(angle))
 
                     # Add the spot to our spot list
                     spots.append(spot)
                     spot_ld_factors.append(limb_darkening_normed(self.u_ld,
@@ -528,19 +533,24 @@
                     if tilted_spots.x.value[k, i] > 0:
                         spot_y = tilted_spots.y.value[k, i]
                         spot_z = tilted_spots.z.value[k, i]
 
                         # Compute the spot position and ellipsoidal shape
                         r_spot = np.hypot(spot_z, spot_y)
                         angle = np.arctan2(spot_z, spot_y)
-                        ellipse_centroid = [spot_y, spot_z]
-
-                        ellipse_axes = [spot_radii[i, 0] *
-                                        np.sqrt(1 - r_spot**2),
-                                        spot_radii[i, 0]]
+                        ellipse_centroid = np.array([
+                            np.squeeze(spot_y),
+                            np.squeeze(spot_z)
+                        ])
+
+                        ellipse_axes = np.array([
+                            np.squeeze(spot_radii[i, 0] *
+                                       np.sqrt(1 - r_spot ** 2)),
+                            np.squeeze(spot_radii[i, 0])
+                        ])
 
                         spot = ellipse(ellipse_centroid, ellipse_axes,
                                        np.degrees(angle))
 
                         # Add the spot to our spot list
                         spots.append(spot)
                         spot_ld_factors.append(limb_darkening_normed(self.u_ld,
@@ -619,20 +629,26 @@
             if tilted_spots.x.value[0, i] > 0:
                 spot_y = tilted_spots.y.value[0, i]
                 spot_z = tilted_spots.z.value[0, i]
 
                 # Compute the spot position and ellipsoidal shape
                 r_spot = np.hypot(spot_z, spot_y)
                 angle = np.arctan2(spot_z, spot_y)
-                ellipse_centroid = [spot_y, spot_z]
-
-                ellipse_axes = [spot_radii[i, 0] *
-                                np.sqrt(1 - r_spot**2),
-                                spot_radii[i, 0]]
+                ellipse_centroid = np.array([
+                    np.squeeze(spot_y),
+                    np.squeeze(spot_z)
+                ])
+
+                ellipse_axes = np.array([
+                    np.squeeze(spot_radii[i, 0] *
+                               np.sqrt(1 - r_spot ** 2)),
+                    np.squeeze(spot_radii[i, 0])
+                ])
 
+                print('args', ellipse_centroid, ellipse_axes, angle)
                 spot = ellipse(ellipse_centroid, ellipse_axes,
                                np.degrees(angle))
 
                 # Add the spot to our spot list
                 spots.append(spot)
 
         if ax is None:
@@ -742,15 +758,16 @@
     radii : float or `~numpy.ndarray`
         Spot radii, shape ``(n_spots, n_inclinations)``
     inc_stellar : `~astropy.units.Quantity`
         Stellar inclinations, shape ``(n_inclinations, )``
     """
     delta_latitude = max_latitude - min_latitude
     if n_inclinations is not None and inclinations is None:
-        inc_stellar = (180*np.random.rand(n_inclinations) - 90) * u.deg
+        inc_stellar = np.arccos(np.random.rand(n_inclinations))
+        inc_stellar = inc_stellar * np.sign(np.random.uniform(-1, 1, n_inclinations)) * u.deg
     else:
         n_inclinations = len(inclinations) if not inclinations.isscalar else 1
         inc_stellar = inclinations
     radii = spot_radius * np.ones((n_spots, n_inclinations))
     lats = (delta_latitude*np.random.rand(n_spots, n_inclinations) +
             min_latitude) * u.deg
     lons = 360*np.random.rand(n_spots, n_inclinations) * u.deg
```

### Comparing `fleck-0.0.dev72/fleck/data/stsp_double_transit.txt` & `fleck-1.1/fleck/data/stsp_double_transit.txt`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/fleck/data/stsp_rotation.txt` & `fleck-1.1/fleck/data/stsp_rotation.txt`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/fleck/data/stsp_single_transit.txt` & `fleck-1.1/fleck/data/stsp_single_transit.txt`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/fleck/tests/test_core.py` & `fleck-1.1/fleck/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/licenses/APACHE2.rst` & `fleck-1.1/licenses/APACHE2.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/licenses/BSD2.rst` & `fleck-1.1/licenses/BSD2.rst`

 * *Files identical despite different names*

### Comparing `fleck-0.0.dev72/licenses/GPLv3.rst` & `fleck-1.1/licenses/GPLv3.rst`

 * *Files identical despite different names*

