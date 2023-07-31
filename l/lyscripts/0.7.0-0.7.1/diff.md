# Comparing `tmp/lyscripts-0.7.0.tar.gz` & `tmp/lyscripts-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyscripts-0.7.0.tar", last modified: Mon Jun 26 14:39:51 2023, max compression
+gzip compressed data, was "lyscripts-0.7.1.tar", last modified: Mon Jul 31 08:49:37 2023, max compression
```

## Comparing `lyscripts-0.7.0.tar` & `lyscripts-0.7.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.803161 lyscripts-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.795160 lyscripts-0.7.0/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.791160 lyscripts-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.795160 lyscripts-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-26 14:39:33.000000 lyscripts-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-26 14:39:33.000000 lyscripts-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 14:39:33.000000 lyscripts-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-26 14:39:51.799160 lyscripts-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-26 14:39:33.000000 lyscripts-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-26 14:39:33.000000 lyscripts-0.7.0/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-06-26 14:39:33.000000 lyscripts-0.7.0/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.795160 lyscripts-0.7.0/lyscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.795160 lyscripts-0.7.0/lyscripts/app/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/app/prevalence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/lyscripts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/enhance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/join.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/lyproxify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/split.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/lyscripts/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/plot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/plot/corner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/plot/histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/plot/thermo_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/lyscripts/predict/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/predict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/predict/prevalences.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/predict/risks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/predict/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/temp_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-06-26 14:39:33.000000 lyscripts-0.7.0/lyscripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.795160 lyscripts-0.7.0/lyscripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:39:51.000000 lyscripts-0.7.0/lyscripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-26 14:39:33.000000 lyscripts-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:39:51.803161 lyscripts-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:39:33.000000 lyscripts-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/tests/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/tests/plot/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/plot/baseline/sine.png
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/plot/baseline/sine.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/plot/baseline/sine_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/plot/baseline/test_draw.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/tests/plot/data/
--rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/plot/data/beta_samples.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/plot/plot_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:51.799160 lyscripts-0.7.0/tests/predict/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/predict/predict_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/predict/prevalences_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/run_doctests.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/test_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-26 14:39:33.000000 lyscripts-0.7.0/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.615684 lyscripts-0.7.1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.615684 lyscripts-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.619685 lyscripts-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-31 08:49:18.000000 lyscripts-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-07-31 08:49:18.000000 lyscripts-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 08:49:18.000000 lyscripts-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-31 08:49:37.623685 lyscripts-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-07-31 08:49:18.000000 lyscripts-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-07-31 08:49:18.000000 lyscripts-0.7.1/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-07-31 08:49:18.000000 lyscripts-0.7.1/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.619685 lyscripts-0.7.1/lyscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.619685 lyscripts-0.7.1/lyscripts/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/app/prevalence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.619685 lyscripts-0.7.1/lyscripts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/lyproxify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.619685 lyscripts-0.7.1/lyscripts/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/plot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/plot/corner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/plot/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/plot/thermo_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/lyscripts/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/predict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/predict/prevalences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/predict/risks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/predict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/temp_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-07-31 08:49:18.000000 lyscripts-0.7.1/lyscripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.619685 lyscripts-0.7.1/lyscripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 08:49:37.000000 lyscripts-0.7.1/lyscripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-31 08:49:18.000000 lyscripts-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:49:37.623685 lyscripts-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:49:18.000000 lyscripts-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/tests/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/tests/plot/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/plot/baseline/sine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/plot/baseline/sine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/plot/baseline/sine_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/plot/baseline/test_draw.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/tests/plot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/plot/data/beta_samples.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/plot/plot_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:49:37.623685 lyscripts-0.7.1/tests/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/predict/predict_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/predict/prevalences_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/run_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/test_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-31 08:49:18.000000 lyscripts-0.7.1/tests/utils_test.py
```

### Comparing `lyscripts-0.7.0/.chglog/CHANGELOG.tpl.md` & `lyscripts-0.7.1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/.chglog/config.yml` & `lyscripts-0.7.1/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/.github/workflows/build.yml` & `lyscripts-0.7.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/.github/workflows/docs.yml` & `lyscripts-0.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/.github/workflows/tests.yml` & `lyscripts-0.7.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/.gitignore` & `lyscripts-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/.pre-commit-config.yaml` & `lyscripts-0.7.1/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v2.3.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
+  - id: end-of-file-fixer
 - repo: https://github.com/hadialqattan/pycln
-  rev: v1.1.0
+  rev: v2.1.3
   hooks:
   - id: pycln
     args: [--config=pyproject.toml]
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
```

### Comparing `lyscripts-0.7.0/CHANGELOG.md` & `lyscripts-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+<a name="0.7.1"></a>
+## [0.7.1] - 2023-07-31
+
+### Bug Fixes
+- **enhance:** negative sublevels don't overwrite superlevels anymore. Fixes [#44].
+
+### Maintenance
+- bump pre-commit hooks
+
+
 <a name="0.7.0"></a>
 ## [0.7.0] - 2023-06-26
 
 ### Bug Fixes
 - add modalities from params in synthetic data generation
 
 ### Features
@@ -276,14 +286,15 @@
 - add pre-commit hook to check commit msg
 
 
 <a name="0.5.3"></a>
 ## [0.5.3] - 2022-08-22
 
 [Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.7.0...HEAD
+[0.7.1]: https://github.com/rmnldwg/lyscripts/compare/0.7.0...0.7.1
 [0.7.0]: https://github.com/rmnldwg/lyscripts/compare/0.6.9...0.7.0
 [0.6.9]: https://github.com/rmnldwg/lyscripts/compare/0.6.8...0.6.9
 [0.6.8]: https://github.com/rmnldwg/lyscripts/compare/0.6.7...0.6.8
 [0.6.7]: https://github.com/rmnldwg/lyscripts/compare/0.6.6...0.6.7
 [0.6.6]: https://github.com/rmnldwg/lyscripts/compare/0.6.5...0.6.6
 [0.6.5]: https://github.com/rmnldwg/lyscripts/compare/0.6.4...0.6.5
 [0.6.4]: https://github.com/rmnldwg/lyscripts/compare/0.6.3...0.6.4
@@ -313,12 +324,13 @@
 [#21]: https://github.com/rmnldwg/lyscripts/issues/21
 [#23]: https://github.com/rmnldwg/lyscripts/issues/23
 [#25]: https://github.com/rmnldwg/lyscripts/issues/25
 [#30]: https://github.com/rmnldwg/lyscripts/issues/30
 [#31]: https://github.com/rmnldwg/lyscripts/issues/31
 [#33]: https://github.com/rmnldwg/lyscripts/issues/33
 [#41]: https://github.com/rmnldwg/lyscripts/issues/41
+[#44]: https://github.com/rmnldwg/lyscripts/issues/44
 
 [`emcee`]: https://emcee.readthedocs.io/en/stable/
 [`rich`]: https://rich.readthedocs.io/en/latest/
 [`rich_argparse`]: https://github.com/hamdanal/rich_argparse
 [LyProX]: https://lyprox.org
```

### Comparing `lyscripts-0.7.0/LICENSE` & `lyscripts-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/PKG-INFO` & `lyscripts-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lyscripts-0.7.0/README.md` & `lyscripts-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/favicon.png` & `lyscripts-0.7.1/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/github-social-card.png` & `lyscripts-0.7.1/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/__init__.py` & `lyscripts-0.7.1/lyscripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/app/__init__.py` & `lyscripts-0.7.1/lyscripts/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/app/prevalence.py` & `lyscripts-0.7.1/lyscripts/app/prevalence.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/__init__.py` & `lyscripts-0.7.1/lyscripts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/__main__.py` & `lyscripts-0.7.1/lyscripts/data/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/clean.py` & `lyscripts-0.7.1/lyscripts/data/clean.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/enhance.py` & `lyscripts-0.7.1/lyscripts/data/enhance.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,19 +134,24 @@
             for lnl in lnls_with_sub:
                 sublvl_values = get_sublvl_values(
                         table[mod,side], lnl, sublvls
                     )
                 if sublvl_values is None:
                     continue
 
+                # sometimes, the sublevels both report `False` (healthy) but the
+                # superlevel is involved. In this case, we want to keep the superlevel
+                # as involved.
+                is_superlvl_involved = table[mod,side,lnl] == True
+
                 has_sublvl_involved = np.any(sublvl_values==True , axis=1)
                 all_sublvls_healthy = np.all(sublvl_values==False, axis=1)
 
                 fixed_table.loc[has_sublvl_involved, (mod,side,lnl)] = True
-                fixed_table.loc[all_sublvls_healthy, (mod,side,lnl)] = False
+                fixed_table.loc[all_sublvls_healthy & ~is_superlvl_involved, (mod,side,lnl)] = False
 
     return fixed_table
 
 
 def get_lnl_observations(
     patient: pd.Series,
     side: str,
```

### Comparing `lyscripts-0.7.0/lyscripts/data/generate.py` & `lyscripts-0.7.1/lyscripts/data/generate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/join.py` & `lyscripts-0.7.1/lyscripts/data/join.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/lyproxify.py` & `lyscripts-0.7.1/lyscripts/data/lyproxify.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/split.py` & `lyscripts-0.7.1/lyscripts/data/split.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/data/utils.py` & `lyscripts-0.7.1/lyscripts/data/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/decorators.py` & `lyscripts-0.7.1/lyscripts/decorators.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/evaluate.py` & `lyscripts-0.7.1/lyscripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/plot/__init__.py` & `lyscripts-0.7.1/lyscripts/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/plot/__main__.py` & `lyscripts-0.7.1/lyscripts/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/plot/corner.py` & `lyscripts-0.7.1/lyscripts/plot/corner.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/plot/histograms.py` & `lyscripts-0.7.1/lyscripts/plot/histograms.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/plot/thermo_int.py` & `lyscripts-0.7.1/lyscripts/plot/thermo_int.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/plot/utils.py` & `lyscripts-0.7.1/lyscripts/plot/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/predict/__init__.py` & `lyscripts-0.7.1/lyscripts/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/predict/__main__.py` & `lyscripts-0.7.1/lyscripts/predict/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/predict/prevalences.py` & `lyscripts-0.7.1/lyscripts/predict/prevalences.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/predict/risks.py` & `lyscripts-0.7.1/lyscripts/predict/risks.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/predict/utils.py` & `lyscripts-0.7.1/lyscripts/predict/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/sample.py` & `lyscripts-0.7.1/lyscripts/sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/temp_schedule.py` & `lyscripts-0.7.1/lyscripts/temp_schedule.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts/utils.py` & `lyscripts-0.7.1/lyscripts/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/lyscripts.egg-info/PKG-INFO` & `lyscripts-0.7.1/lyscripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lyscripts-0.7.0/lyscripts.egg-info/SOURCES.txt` & `lyscripts-0.7.1/lyscripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/pyproject.toml` & `lyscripts-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/_sample.py` & `lyscripts-0.7.1/tests/_sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/plot/baseline/sine.png` & `lyscripts-0.7.1/tests/plot/baseline/sine.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/plot/baseline/sine.svg` & `lyscripts-0.7.1/tests/plot/baseline/sine.svg`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/plot/baseline/sine_svg.png` & `lyscripts-0.7.1/tests/plot/baseline/sine_svg.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/plot/baseline/test_draw.png` & `lyscripts-0.7.1/tests/plot/baseline/test_draw.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/plot/data/beta_samples.hdf5` & `lyscripts-0.7.1/tests/plot/data/beta_samples.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/plot/plot_utils_test.py` & `lyscripts-0.7.1/tests/plot/plot_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/predict/predict_utils_test.py` & `lyscripts-0.7.1/tests/predict/predict_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/predict/prevalences_test.py` & `lyscripts-0.7.1/tests/predict/prevalences_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/test_params.yaml` & `lyscripts-0.7.1/tests/test_params.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.7.0/tests/utils_test.py` & `lyscripts-0.7.1/tests/utils_test.py`

 * *Files identical despite different names*

