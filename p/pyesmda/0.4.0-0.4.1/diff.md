# Comparing `tmp/pyesmda-0.4.0.tar.gz` & `tmp/pyesmda-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesmda-0.4.0.tar", last modified: Wed Jun 28 14:04:18 2023, max compression
+gzip compressed data, was "pyesmda-0.4.1.tar", last modified: Mon Jul 31 12:37:30 2023, max compression
```

## Comparing `pyesmda-0.4.0.tar` & `pyesmda-0.4.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.046695 pyesmda-0.4.0/
--rw-r--r--   0 acollet  (11734) geosciences (10000)      197 2022-03-01 14:30:06.000000 pyesmda-0.4.0/AUTHORS.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     4337 2023-06-28 13:57:51.000000 pyesmda-0.4.0/CHANGELOG.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     6433 2022-08-12 09:15:56.000000 pyesmda-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1072 2022-03-01 14:30:06.000000 pyesmda-0.4.0/LICENSE
--rw-r--r--   0 acollet  (11734) geosciences (10000)      264 2022-03-01 14:30:06.000000 pyesmda-0.4.0/MANIFEST.in
--rw-r--r--   0 acollet  (11734) geosciences (10000)     9730 2023-06-28 14:04:18.046695 pyesmda-0.4.0/PKG-INFO
--rw-r--r--   0 acollet  (11734) geosciences (10000)     3385 2023-06-28 13:57:41.000000 pyesmda-0.4.0/README.rst
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.038695 pyesmda-0.4.0/docs/
--rw-r--r--   0 acollet  (11734) geosciences (10000)      612 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/Makefile
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.034695 pyesmda-0.4.0/docs/build/
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.034695 pyesmda-0.4.0/docs/build/doctrees/
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.038695 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/
--rw-r--r--   0 acollet  (11734) geosciences (10000)    72926 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_10_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    63459 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    28241 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_16_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    28598 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_21_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    21306 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_25_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    19821 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_29_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    23160 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_31_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    21960 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_34_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    24483 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_36_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    24951 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_38_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    21251 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_8_1.png
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.034695 pyesmda-0.4.0/docs/build/html/
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/docs/build/html/_images/
--rw-r--r--   0 acollet  (11734) geosciences (10000)    72926 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_10_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    63459 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    28241 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_16_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    28598 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_21_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    21306 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_25_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    19821 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_29_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    23160 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_31_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    21960 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_34_2.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    24483 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_36_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    24951 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_38_1.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)    21251 2023-06-28 10:22:23.000000 pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_8_1.png
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/docs/build/html/_static/
--rw-r--r--   0 acollet  (11734) geosciences (10000)      286 2022-12-06 09:06:20.000000 pyesmda-0.4.0/docs/build/html/_static/file.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.0/docs/build/html/_static/minus.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.0/docs/build/html/_static/plus.png
--rw-r--r--   0 acollet  (11734) geosciences (10000)      773 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/make.bat
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/docs/source/
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/docs/source/_autosummary/
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1326 2023-06-28 10:17:43.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.ESMDA.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1563 2023-06-28 10:17:43.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.ESMDA_RS.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      126 2022-12-06 10:05:09.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.approximate_cov_mm.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      208 2022-12-06 10:05:09.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.approximate_covariance_matrix_from_ensembles.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      149 2022-12-06 10:05:09.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.check_nans_in_predictions.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      240 2022-12-06 10:05:09.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.compute_ensemble_average_normalized_objective_function.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      185 2022-12-06 10:05:09.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.compute_normalized_objective_function.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      135 2023-06-28 10:17:43.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.get_ensemble_variance.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      172 2022-12-06 10:05:09.000000 pyesmda-0.4.0/docs/source/_autosummary/pyesmda.inflate_ensemble_around_its_mean.rst
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/docs/source/_templates/
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/docs/source/_templates/autosummary/
--rw-r--r--   0 acollet  (11734) geosciences (10000)      106 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/_templates/class.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1079 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/_templates/module.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      114 2022-10-07 21:02:34.000000 pyesmda-0.4.0/docs/source/api_reference.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)       31 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/authors.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)       75 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/bibliography.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)       33 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/changelog.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)    14867 2023-06-28 13:57:41.000000 pyesmda-0.4.0/docs/source/conf.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)       36 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/contributing.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      458 2022-08-11 22:32:41.000000 pyesmda-0.4.0/docs/source/index.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1138 2022-08-11 22:32:41.000000 pyesmda-0.4.0/docs/source/installation.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)       30 2022-08-11 22:03:08.000000 pyesmda-0.4.0/docs/source/readme.rst
--rw-r--r--   0 acollet  (11734) geosciences (10000)      288 2022-08-12 09:15:56.000000 pyesmda-0.4.0/docs/source/usage.rst
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/pyesmda/
--rw-r--r--   0 acollet  (11734) geosciences (10000)       96 2023-06-28 13:57:51.000000 pyesmda-0.4.0/pyesmda/__about__.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1609 2023-06-28 13:57:41.000000 pyesmda-0.4.0/pyesmda/__init__.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)    31881 2023-06-28 13:57:41.000000 pyesmda-0.4.0/pyesmda/esmda.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)    16165 2023-06-28 13:57:41.000000 pyesmda-0.4.0/pyesmda/esmda_rs.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)     7805 2023-06-28 13:57:41.000000 pyesmda-0.4.0/pyesmda/utils.py
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.042695 pyesmda-0.4.0/pyesmda.egg-info/
--rw-r--r--   0 acollet  (11734) geosciences (10000)     9730 2023-06-28 14:04:17.000000 pyesmda-0.4.0/pyesmda.egg-info/PKG-INFO
--rw-r--r--   0 acollet  (11734) geosciences (10000)     3337 2023-06-28 14:04:18.000000 pyesmda-0.4.0/pyesmda.egg-info/SOURCES.txt
--rw-r--r--   0 acollet  (11734) geosciences (10000)        1 2023-06-28 14:04:17.000000 pyesmda-0.4.0/pyesmda.egg-info/dependency_links.txt
--rw-r--r--   0 acollet  (11734) geosciences (10000)        1 2023-06-28 14:04:17.000000 pyesmda-0.4.0/pyesmda.egg-info/not-zip-safe
--rw-r--r--   0 acollet  (11734) geosciences (10000)       25 2023-06-28 14:04:17.000000 pyesmda-0.4.0/pyesmda.egg-info/requires.txt
--rw-r--r--   0 acollet  (11734) geosciences (10000)       14 2023-06-28 14:04:17.000000 pyesmda-0.4.0/pyesmda.egg-info/top_level.txt
--rw-r--r--   0 acollet  (11734) geosciences (10000)      173 2023-06-28 13:57:51.000000 pyesmda-0.4.0/pyproject.toml
--rw-r--r--   0 acollet  (11734) geosciences (10000)     1481 2023-06-28 14:04:18.046695 pyesmda-0.4.0/setup.cfg
-drwxr-xr-x   0 acollet  (11734) geosciences (10000)        0 2023-06-28 14:04:18.046695 pyesmda-0.4.0/tests/
--rw-r--r--   0 acollet  (11734) geosciences (10000)        0 2022-03-01 14:30:06.000000 pyesmda-0.4.0/tests/__init__.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)    14545 2023-06-28 13:57:41.000000 pyesmda-0.4.0/tests/test_esmda.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)     2172 2023-06-28 07:47:34.000000 pyesmda-0.4.0/tests/test_esmda_rs.py
--rw-r--r--   0 acollet  (11734) geosciences (10000)     5136 2023-06-28 13:57:41.000000 pyesmda-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.025393 pyesmda-0.4.1/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      197 2022-03-01 14:30:06.000000 pyesmda-0.4.1/AUTHORS.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     4523 2023-07-31 12:26:01.000000 pyesmda-0.4.1/CHANGELOG.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6433 2022-08-12 09:15:56.000000 pyesmda-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1072 2022-03-01 14:30:06.000000 pyesmda-0.4.1/LICENSE
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      264 2022-03-01 14:30:06.000000 pyesmda-0.4.1/MANIFEST.in
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     9916 2023-07-31 12:37:30.025393 pyesmda-0.4.1/PKG-INFO
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3385 2023-06-28 13:57:41.000000 pyesmda-0.4.1/README.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.953393 pyesmda-0.4.1/docs/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      612 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/Makefile
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.945393 pyesmda-0.4.1/docs/build/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.945393 pyesmda-0.4.1/docs/build/doctrees/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.969393 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    72926 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_10_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    63459 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28241 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_16_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28598 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_21_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21306 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_25_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19821 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_29_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23160 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_31_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21960 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_34_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24483 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_36_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24951 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_38_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21251 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_8_1.png
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.949393 pyesmda-0.4.1/docs/build/html/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.985393 pyesmda-0.4.1/docs/build/html/_images/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    72926 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_10_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    63459 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28241 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_16_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28598 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_21_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21306 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_25_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19821 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_29_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23160 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_31_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21960 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_34_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24483 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_36_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24951 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_38_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21251 2023-07-31 12:26:22.000000 pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_8_1.png
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:29.989393 pyesmda-0.4.1/docs/build/html/_static/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      286 2022-12-06 09:06:20.000000 pyesmda-0.4.1/docs/build/html/_static/file.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.1/docs/build/html/_static/minus.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.1/docs/build/html/_static/plus.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      773 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/make.bat
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.001393 pyesmda-0.4.1/docs/source/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.009393 pyesmda-0.4.1/docs/source/_autosummary/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1326 2023-06-28 10:17:43.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.ESMDA.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1563 2023-06-28 10:17:43.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.ESMDA_RS.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      126 2022-12-06 10:05:09.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.approximate_cov_mm.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      208 2022-12-06 10:05:09.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.approximate_covariance_matrix_from_ensembles.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      149 2022-12-06 10:05:09.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.check_nans_in_predictions.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      240 2022-12-06 10:05:09.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.compute_ensemble_average_normalized_objective_function.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      185 2022-12-06 10:05:09.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.compute_normalized_objective_function.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      135 2023-06-28 10:17:43.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.get_ensemble_variance.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2022-12-06 10:05:09.000000 pyesmda-0.4.1/docs/source/_autosummary/pyesmda.inflate_ensemble_around_its_mean.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.009393 pyesmda-0.4.1/docs/source/_templates/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.013393 pyesmda-0.4.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      106 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/_templates/class.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1079 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/_templates/module.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      114 2022-10-07 21:02:34.000000 pyesmda-0.4.1/docs/source/api_reference.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       31 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/authors.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       75 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/bibliography.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       33 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/changelog.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    14867 2023-06-28 13:57:41.000000 pyesmda-0.4.1/docs/source/conf.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       36 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/contributing.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      458 2022-08-11 22:32:41.000000 pyesmda-0.4.1/docs/source/index.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1138 2022-08-11 22:32:41.000000 pyesmda-0.4.1/docs/source/installation.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       30 2022-08-11 22:03:08.000000 pyesmda-0.4.1/docs/source/readme.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      288 2022-08-12 09:15:56.000000 pyesmda-0.4.1/docs/source/usage.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.017393 pyesmda-0.4.1/pyesmda/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       96 2023-07-31 12:25:12.000000 pyesmda-0.4.1/pyesmda/__about__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1609 2023-06-28 13:57:41.000000 pyesmda-0.4.1/pyesmda/__init__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    31964 2023-07-27 16:18:59.000000 pyesmda-0.4.1/pyesmda/esmda.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    16165 2023-06-28 13:57:41.000000 pyesmda-0.4.1/pyesmda/esmda_rs.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     7805 2023-06-28 13:57:41.000000 pyesmda-0.4.1/pyesmda/utils.py
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.021393 pyesmda-0.4.1/pyesmda.egg-info/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     9916 2023-07-31 12:37:29.000000 pyesmda-0.4.1/pyesmda.egg-info/PKG-INFO
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3337 2023-07-31 12:37:29.000000 pyesmda-0.4.1/pyesmda.egg-info/SOURCES.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2023-07-31 12:37:29.000000 pyesmda-0.4.1/pyesmda.egg-info/dependency_links.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2023-07-31 12:37:29.000000 pyesmda-0.4.1/pyesmda.egg-info/not-zip-safe
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       25 2023-07-31 12:37:29.000000 pyesmda-0.4.1/pyesmda.egg-info/requires.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       14 2023-07-31 12:37:29.000000 pyesmda-0.4.1/pyesmda.egg-info/top_level.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      173 2023-06-28 13:57:51.000000 pyesmda-0.4.1/pyproject.toml
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1481 2023-07-31 12:37:30.033393 pyesmda-0.4.1/setup.cfg
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-07-31 12:37:30.025393 pyesmda-0.4.1/tests/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        0 2022-03-01 14:30:06.000000 pyesmda-0.4.1/tests/__init__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    14545 2023-06-28 13:57:41.000000 pyesmda-0.4.1/tests/test_esmda.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2172 2023-06-28 07:47:34.000000 pyesmda-0.4.1/tests/test_esmda_rs.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5136 2023-06-28 13:57:41.000000 pyesmda-0.4.1/tests/test_utils.py
```

### Comparing `pyesmda-0.4.0/CHANGELOG.rst` & `pyesmda-0.4.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ==============
 Changelog
 ==============
 
+0.4.1 (2023-07-31)
+------------------
+
+* `!PR33 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/33>`_ FIX: the covariance inflation is now applied before the forecast step.
+
 0.4.0 (2023-06-28)
 ------------------
 
 * `!PR30 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/30>`_ ENH: Allow to perform the analyse step by batches of gridblocks and avoid the
   construction on large (N, M) correlation matrices. Three new parameters have been introduced - **batch_size**: Number of parameters that are assimilated at once. This option is
   available to overcome memory limitations when the number of updated parameters is large. In that case, the size of the covariance matrices tends to explode
   and the update step must be performed by chunks of parameters.
```

### Comparing `pyesmda-0.4.0/CONTRIBUTING.rst` & `pyesmda-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/LICENSE` & `pyesmda-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/PKG-INFO` & `pyesmda-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesmda
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Ensemble Smoother with Multiple Data Assimilation.
 Home-page: https://gitlab.com/antoinecollet5/pyesmda
 Author: attr: pyesmda.__author__
 Author-email: antoinecollet5@gmail.com
 License: MIT license
 Keywords: esmda,es-mda,inversion,inverse problem,parameter estimation,stochastic-optimization,ensemble smoother
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -105,14 +105,19 @@
   Engineers - SPE Reservoir Simulation Symposium
   1.    2. 10.2118/163675-MS.
 
 ==============
 Changelog
 ==============
 
+0.4.1 (2023-07-31)
+------------------
+
+* `!PR33 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/33>`_ FIX: the covariance inflation is now applied before the forecast step.
+
 0.4.0 (2023-06-28)
 ------------------
 
 * `!PR30 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/30>`_ ENH: Allow to perform the analyse step by batches of gridblocks and avoid the
   construction on large (N, M) correlation matrices. Three new parameters have been introduced - **batch_size**: Number of parameters that are assimilated at once. This option is
   available to overcome memory limitations when the number of updated parameters is large. In that case, the size of the covariance matrices tends to explode
   and the update step must be performed by chunks of parameters.
```

### Comparing `pyesmda-0.4.0/README.rst` & `pyesmda-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/Makefile` & `pyesmda-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_10_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_10_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_16_2.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_16_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_21_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_21_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_25_2.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_25_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_29_2.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_29_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_31_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_31_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_34_2.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_34_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_36_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_36_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_38_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_38_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_8_1.png` & `pyesmda-0.4.1/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_8_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_10_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_10_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_16_2.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_16_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_21_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_21_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_25_2.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_25_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_29_2.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_29_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_31_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_31_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_34_2.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_34_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_36_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_36_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_38_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_38_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/build/html/_images/tutorials_correlation_matrices_building_8_1.png` & `pyesmda-0.4.1/docs/build/html/_images/tutorials_correlation_matrices_building_8_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/make.bat` & `pyesmda-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_autosummary/pyesmda.ESMDA.rst` & `pyesmda-0.4.1/docs/source/_autosummary/pyesmda.ESMDA.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_autosummary/pyesmda.ESMDA_RS.rst` & `pyesmda-0.4.1/docs/source/_autosummary/pyesmda.ESMDA_RS.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_templates/autosummary/class.rst` & `pyesmda-0.4.1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_templates/autosummary/module.rst` & `pyesmda-0.4.1/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_templates/class.rst` & `pyesmda-0.4.1/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_templates/custom-module-template.rst` & `pyesmda-0.4.1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/_templates/module.rst` & `pyesmda-0.4.1/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/conf.py` & `pyesmda-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/docs/source/installation.rst` & `pyesmda-0.4.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/pyesmda/__init__.py` & `pyesmda-0.4.1/pyesmda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/pyesmda/esmda.py` & `pyesmda-0.4.1/pyesmda/esmda.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,25 +489,27 @@
 
     def _solve(self) -> None:
         """Solve the optimization problem with ES-MDA algorithm."""
         if self.save_ensembles_history:
             self.m_history.append(self.m_prior)  # save m_init
         for self._assimilation_step in range(self.n_assimilations):
             print(f"Assimilation # {self._assimilation_step + 1}")
+            # inflating the covariance
+            self.m_prior = self._apply_bounds(
+                inflate_ensemble_around_its_mean(
+                    self.m_prior,
+                    self.cov_mm_inflation_factors[self._assimilation_step],
+                )
+            )
             self._forecast()
             self._pertrub(self.cov_obs_inflation_factors[self._assimilation_step])
             self._approximate_covariance_matrices()
             # Update the prior parameter for next iteration
             self.m_prior = self._apply_bounds(
-                inflate_ensemble_around_its_mean(
-                    self._analyse(
-                        self.cov_obs_inflation_factors[self._assimilation_step]
-                    ),
-                    self.cov_mm_inflation_factors[self._assimilation_step],
-                )
+                self._analyse(self.cov_obs_inflation_factors[self._assimilation_step])
             )
             # Saving the parameters history
             if self.save_ensembles_history:
                 self.m_history.append(self.m_prior)
 
         if self.is_forecast_for_last_assimilation:
             self._forecast()
```

### Comparing `pyesmda-0.4.0/pyesmda/esmda_rs.py` & `pyesmda-0.4.1/pyesmda/esmda_rs.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/pyesmda/utils.py` & `pyesmda-0.4.1/pyesmda/utils.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/pyesmda.egg-info/PKG-INFO` & `pyesmda-0.4.1/pyesmda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesmda
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Ensemble Smoother with Multiple Data Assimilation.
 Home-page: https://gitlab.com/antoinecollet5/pyesmda
 Author: attr: pyesmda.__author__
 Author-email: antoinecollet5@gmail.com
 License: MIT license
 Keywords: esmda,es-mda,inversion,inverse problem,parameter estimation,stochastic-optimization,ensemble smoother
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -105,14 +105,19 @@
   Engineers - SPE Reservoir Simulation Symposium
   1.    2. 10.2118/163675-MS.
 
 ==============
 Changelog
 ==============
 
+0.4.1 (2023-07-31)
+------------------
+
+* `!PR33 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/33>`_ FIX: the covariance inflation is now applied before the forecast step.
+
 0.4.0 (2023-06-28)
 ------------------
 
 * `!PR30 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/30>`_ ENH: Allow to perform the analyse step by batches of gridblocks and avoid the
   construction on large (N, M) correlation matrices. Three new parameters have been introduced - **batch_size**: Number of parameters that are assimilated at once. This option is
   available to overcome memory limitations when the number of updated parameters is large. In that case, the size of the covariance matrices tends to explode
   and the update step must be performed by chunks of parameters.
```

### Comparing `pyesmda-0.4.0/pyesmda.egg-info/SOURCES.txt` & `pyesmda-0.4.1/pyesmda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/setup.cfg` & `pyesmda-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/tests/test_esmda.py` & `pyesmda-0.4.1/tests/test_esmda.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/tests/test_esmda_rs.py` & `pyesmda-0.4.1/tests/test_esmda_rs.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.0/tests/test_utils.py` & `pyesmda-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

