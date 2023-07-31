# Comparing `tmp/datafold-1.1.6.tar.gz` & `tmp/datafold-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datafold-1.1.6.tar", last modified: Thu Dec  2 17:42:08 2021, max compression
+gzip compressed data, was "datafold-2.0.0.tar", last modified: Mon Jul 31 21:06:13 2023, max compression
```

## Comparing `datafold-1.1.6.tar` & `datafold-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,79 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      337 2021-07-02 12:09:50.000000 datafold-1.1.6/CONTRIBUTORS
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1108 2021-07-05 20:34:51.000000 datafold-1.1.6/LICENSE
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4523 2021-07-16 07:16:04.000000 datafold-1.1.6/LICENSES_bundled
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       87 2021-06-30 17:00:46.000000 datafold-1.1.6/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15057 2021-12-02 17:42:08.000000 datafold-1.1.6/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12215 2021-07-16 07:16:04.000000 datafold-1.1.6/README.rst
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      220 2021-07-06 13:01:32.000000 datafold-1.1.6/datafold/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2385 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/_decorators.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2303 2021-12-02 16:29:42.000000 datafold-1.1.6/datafold/_version.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold/appfold/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1488 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/appfold/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    70827 2021-08-04 07:55:43.000000 datafold-1.1.6/datafold/appfold/edmd.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold/dynfold/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2678 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/dynfold/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    21754 2021-07-05 07:20:29.000000 datafold-1.1.6/datafold/dynfold/base.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3727 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/dynfold/compose.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    43101 2021-09-14 07:04:07.000000 datafold-1.1.6/datafold/dynfold/dmap.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    64577 2021-08-04 07:55:43.000000 datafold-1.1.6/datafold/dynfold/dmd.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    21413 2021-07-06 10:47:46.000000 datafold-1.1.6/datafold/dynfold/jsf.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    33253 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/dynfold/outofsample.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    43603 2021-07-16 07:16:04.000000 datafold-1.1.6/datafold/dynfold/transform.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold/pcfold/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2439 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/pcfold/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    35766 2021-07-16 07:16:04.000000 datafold-1.1.6/datafold/pcfold/distance.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     8041 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/pcfold/eigsolver.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3756 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/pcfold/estimators.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    76234 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/pcfold/kernels.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13903 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/pcfold/pointcloud.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold/pcfold/timeseries/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/pcfold/timeseries/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    41698 2021-07-02 07:50:01.000000 datafold-1.1.6/datafold/pcfold/timeseries/accessor.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    66289 2021-07-05 16:04:46.000000 datafold-1.1.6/datafold/pcfold/timeseries/collection.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    36486 2021-07-02 07:50:01.000000 datafold-1.1.6/datafold/pcfold/timeseries/metric.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold/utils/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/utils/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    10889 2021-07-02 07:50:01.000000 datafold-1.1.6/datafold/utils/_systems.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12721 2021-07-02 07:50:01.000000 datafold-1.1.6/datafold/utils/general.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9563 2021-06-21 20:03:53.000000 datafold-1.1.6/datafold/utils/plot.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15057 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1028 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      130 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2021-12-02 17:42:08.000000 datafold-1.1.6/datafold.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1149 2021-07-16 07:16:04.000000 datafold-1.1.6/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      130 2021-07-02 07:50:01.000000 datafold-1.1.6/requirements.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2021-12-02 17:42:08.000000 datafold-1.1.6/setup.cfg
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5197 2021-10-22 09:29:31.000000 datafold-1.1.6/setup.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.304578 datafold-2.0.0/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      526 2023-07-21 19:29:26.000000 datafold-2.0.0/CONTRIBUTORS
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1108 2023-07-21 12:20:27.000000 datafold-2.0.0/LICENSE
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     8214 2023-07-21 19:29:26.000000 datafold-2.0.0/LICENSES_bundled
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       87 2023-07-21 12:20:27.000000 datafold-2.0.0/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13383 2023-07-31 21:06:13.300577 datafold-2.0.0/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12516 2023-07-31 19:46:20.000000 datafold-2.0.0/README.rst
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.296578 datafold-2.0.0/datafold/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      411 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2469 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/_decorators.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2279 2023-07-31 19:22:20.000000 datafold-2.0.0/datafold/_version.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.296578 datafold-2.0.0/datafold/appfold/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1488 2023-07-21 12:20:27.000000 datafold-2.0.0/datafold/appfold/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      249 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/appfold/analysis.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)   102127 2023-07-31 18:17:40.000000 datafold-2.0.0/datafold/appfold/edmd.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    38217 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/appfold/mpc.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.296578 datafold-2.0.0/datafold/appfold/tests/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/appfold/tests/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    48607 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/appfold/tests/test_edmd.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7894 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/appfold/tests/test_kmpc.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.300577 datafold-2.0.0/datafold/dynfold/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2793 2023-07-23 20:50:29.000000 datafold-2.0.0/datafold/dynfold/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    30636 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/base.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3081 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/compose.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    24016 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/dictlearning.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    56118 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/dmap.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    91936 2023-07-31 18:17:40.000000 datafold-2.0.0/datafold/dynfold/dmd.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    36050 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/dynsystem.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    18363 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/jsf.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    31076 2023-07-31 19:22:20.000000 datafold-2.0.0/datafold/dynfold/outofsample.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.300577 datafold-2.0.0/datafold/dynfold/tests/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5214 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/helper.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7522 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_base.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9958 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_compose.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    46964 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_dmap.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    53157 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_dmd.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     8652 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_jsf.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    38423 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_outofsample.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13899 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_roseland.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    21208 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/dynfold/tests/test_transform.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    54482 2023-07-31 19:22:20.000000 datafold-2.0.0/datafold/dynfold/transform.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.300577 datafold-2.0.0/datafold/pcfold/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2467 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    38225 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/distance.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    10838 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/eigsolver.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3828 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/estimators.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    90195 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/kernels.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13741 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/pointcloud.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.300577 datafold-2.0.0/datafold/pcfold/tests/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13153 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_distance.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4124 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_estimators.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    23412 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_kernels.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1482 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_pcmanifold.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    24188 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_tsc_accessor.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    61407 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_tsc_collection.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    23627 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_tsc_metric.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1178 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/tests/test_tsc_plots.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.300577 datafold-2.0.0/datafold/pcfold/timeseries/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-21 12:20:27.000000 datafold-2.0.0/datafold/pcfold/timeseries/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    51212 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/timeseries/accessor.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    70156 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/timeseries/collection.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    36627 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/pcfold/timeseries/metric.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.300577 datafold-2.0.0/datafold/utils/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-21 12:20:27.000000 datafold-2.0.0/datafold/utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    46832 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/utils/_systems.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    17702 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/utils/general.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9378 2023-07-21 19:29:26.000000 datafold-2.0.0/datafold/utils/plot.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-07-31 21:06:13.296578 datafold-2.0.0/datafold.egg-info/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13383 2023-07-31 21:06:13.000000 datafold-2.0.0/datafold.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1986 2023-07-31 21:06:13.000000 datafold-2.0.0/datafold.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2023-07-31 21:06:13.000000 datafold-2.0.0/datafold.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      144 2023-07-31 21:06:13.000000 datafold-2.0.0/datafold.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2023-07-31 21:06:13.000000 datafold-2.0.0/datafold.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3071 2023-07-21 19:29:26.000000 datafold-2.0.0/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      144 2023-07-21 19:29:26.000000 datafold-2.0.0/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2023-07-31 21:06:13.304578 datafold-2.0.0/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3441 2023-07-21 19:29:26.000000 datafold-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datafold-1.1.6/LICENSE` & `datafold-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datafold-1.1.6/PKG-INFO` & `datafold-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,268 +1,270 @@
 Metadata-Version: 2.1
 Name: datafold
-Version: 1.1.6
+Version: 2.0.0
 Summary: Operator-theoretic models to identify dynamical systems and parametrize point cloud geometry
 Home-page: https://datafold-dev.gitlab.io/datafold
+Download-URL: https://pypi.org/project/datafold/
 Author: datafold development team
-Author-email: daniel.lehmberg@hm.edu
+Author-email: d.lehmberg@tum.de
 License: MIT
-Download-URL: https://pypi.org/project/datafold/
-Description: Quick links
-        ^^^^^^^^^^^
-        
-        `Source repository <https://gitlab.com/datafold-dev/datafold>`__ |
-        `Contributing and feedback <https://datafold-dev.gitlab.io/datafold/contributing.html>`__ |
-        `PyPI <https://pypi.org/project/datafold/>`__ |
-        `Documentation <https://datafold-dev.gitlab.io/datafold/>`__ |
-        `Tutorials <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__ |
-        `Scientific literature <https://datafold-dev.gitlab.io/datafold/references.html>`__
-        
-        What is *datafold*?
-        ====================
-        
-        *datafold* is a `MIT-licensed <https://gitlab.com/datafold-dev/datafold/-/blob/master/LICENSE>`__
-        Python package containing operator-theoretic, data-driven models to identify dynamical
-        systems from time series data and to infer geometrical structures in point clouds.
-        
-        The package includes:
-        
-        * Data structures to handle point clouds on manifolds (``PCManifold``) and time series
-          collections (``TSCDataFrame``). The data structures are used both internally and for
-          model input/outputs. In contrast to solutions found in other projects, such as
-          lists of Numpy arrays, ``TSCDataFrame`` makes it much easier to describe many forms of
-          time series data in a single object.
-        * An efficient implementation of the ``DiffusionMaps`` model to infer geometric
-          meaningful structures from data, such as the eigenfunctions of the
-          Laplace-Beltrami operator. As a distinguishing factor to other implementations, the
-          model can handle a sparse kernel matrix and allows setting an arbitrary kernel,
-          including the standard Gaussian kernel,
-          `continuous k-nearest neighbor kernel <https://arxiv.org/abs/1606.02353>`__, or
-          `dynamics-adapted cone kernel <https://cims.nyu.edu/~dimitris/files/Giannakis15_cone_kernels.pdf>`__.
-        * Out-of-sample extensions for the Diffusion Maps model, such as the (auto-tuned)
-          Laplacian Pyramids or Geometric Harmonics to interpolate general function values on a
-          point cloud manifold.
-        * An implementation of the (Extended-) Dynamic Mode Decomposition (e.g. model ``DMDFull``
-          or ``EDMD``) as data-driven methods to identify dynamical systems from time series
-          collection data. ``EDMD`` subclasses from the flexible scikit-learn
-          `Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`__,
-          which allows setting up and transforming time series collection data to a more suitable
-          feature state (cf. Koopman operator theory).
-        * ``EDMDCV`` allows model parameters to be optimized with cross-validation splittings that
-          account for the temporal order in time series collections.
-        
-        See also `this introduction page <https://datafold-dev.gitlab.io/datafold/intro.html>`__.
-        For a mathematical thorough introduction, we refer to the `scientific literature
-        <https://datafold-dev.gitlab.io/datafold/references.html>`__.
-        
-        .. note::
-            The project is under active development in a research-driven environment.
-        
-            * Code quality varies from "experimental/early stage" to "well-tested". Well tested
-              code is listed in the
-              `software documentation <https://datafold-dev.gitlab.io/datafold/api.html>`__
-              and are directly accessible through the package levels ``pcfold``, ``dynfold`` or
-              ``appfold`` (e.g. :code:`from datafold.dynfold import ...`). Experimental code is
-              only accessible via "deep imports"
-              (e.g. :code:`from datafol.dynfold.outofsample import ...`) and may raise a warning
-              when using it.
-            * There is no deprecation cycle. Backwards compatibility is indicated by the
-              package version, where we use a `semantic versioning <https://semver.org/>`__
-              policy `[major].[minor].[patch]`, i.e.
-        
-                 * `major` - making incompatible changes in the (documented) API
-                 * `minor` - adding functionality in a backwards-compatible manner
-                 * `patch` - backwards-compatible bug fixes
-        
-              We do not intend to indicate a feature complete milestone with version `1.0`.
-        
-        
-        Cite
-        ====
-        
-        If you use *datafold* in your research, please cite
-        `this paper <https://joss.theoj.org/papers/10.21105/joss.02283>`__ published in the
-        *Journal of Open Source Software* (`JOSS <https://joss.theoj.org/>`__).
-        
-        *Lehmberg et al., (2020). datafold: data-driven models for point clouds and time series on
-        manifolds. Journal of Open Source Software, 5(51), 2283,* https://doi.org/10.21105/joss.02283
-        
-        BibTeX:
-        
-        .. code-block:: latex
-        
-            @article{Lehmberg2020,
-                     doi       = {10.21105/joss.02283},
-                     url       = {https://doi.org/10.21105/joss.02283},
-                     year      = {2020},
-                     publisher = {The Open Journal},
-                     volume    = {5},
-                     number    = {51},
-                     pages     = {2283},
-                     author    = {Daniel Lehmberg and Felix Dietrich and Gerta K{\"o}ster and Hans-Joachim Bungartz},
-                     title     = {datafold: data-driven models for point clouds and time series on manifolds},
-                     journal   = {Journal of Open Source Software}}
-        
-        How to get it?
-        ==============
-        
-        Installation requires `Python>=3.7 <https://www.python.org/>`__ with
-        `pip <https://pip.pypa.io/en/stable/>`__ and
-        `setuptools <https://setuptools.readthedocs.io/en/latest/>`__ installed. Both
-        packages usually ship with a standard Python installation. The package dependencies
-        install automatically. The main dependencies and their role in *datafold* are listed below
-        in "Dependencies".
-        
-        There are two ways to install *datafold*:
-        
-        1. From PyPI
-        ------------
-        
-        This is the standard way for users. The package is hosted on the official Python package
-        index (PyPI) and installs the core package (excluding tutorials and tests). The tutorial
-        files can be downloaded separately
-        `here <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__.
-        
-        To install the package and its dependencies with :code:`pip`, run
-        
-        .. code-block:: bash
-        
-           python -m pip install datafold
-        
-        .. note::
-        
-            If you run Python in an Anaconda environment you can use pip from within ``conda``.
-            See also
-            `official instructions <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages>`__.
-        
-            .. code-block:: bash
-        
-                conda activate venv
-                conda install pip
-                pip install datafold
-        
-        
-        2. From source
-        --------------
-        
-        This way is recommended if you want to access the latest (but potentially unstable)
-        development, run tests or wish to contribute (see section "Contributing" for details).
-        Download or git-clone the source code repository.
-        
-        1. Download the repository
-        
-           a. If you wish to contribute code, it is required to have
-              `git <https://git-scm.com/>`__ installed. Clone the repository with
-        
-              .. code-block:: bash
-        
-                git clone https://gitlab.com/datafold-dev/datafold.git
-        
-           b. If you only want access to the source code (current ``master`` branch), download one
-              of the compressed files
-              (`zip <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.zip>`__,
-              `tar.gz <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.gz>`__,
-              `tar.bz2 <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.bz2>`__,
-              `tar <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar>`__)
-        
-        2. Install the package from the downloaded repository
-        
-           .. code-block:: bash
-        
-               python -m pip install .
-        
-        
-        Contributing
-        ============
-        
-        Any contribution (code/tutorials/documentation improvements), question or feedback is
-        very welcome. Either use the
-        `issue tracker <https://gitlab.com/datafold-dev/datafold/-/issues>`__ or
-        `Email <incoming+datafold-dev-datafold-14878376-issue-@incoming.gitlab.com>`__.
-        Instructions to set up *datafold* for development can be found
-        `here <https://datafold-dev.gitlab.io/datafold/contributing.html>`__.
-        
-        Dependencies
-        ============
-        
-        The dependencies of the core package are managed in the file
-        `requirements.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements.txt>`__
-        and install with *datafold*. The tests, tutorials, documentation and code analysis
-        require additional dependencies which are managed in
-        `requirements-dev.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements-dev.txt>`__.
-        
-        *datafold* integrates with common packages from the
-        `Python scientific computing stack <https://www.scipy.org/about.html>`__:
-        
-        * `NumPy <https://numpy.org/>`__
-           The data structure ``PCManifold`` subclasses from NumPy's
-           `ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`__. The
-           class attaches an kernel object to the data to describe point similarity.
-           NumPy is used throughout *datafold* and is the default package for numerical
-           data and algorithms.
-        
-        * `pandas <https://pandas.pydata.org/pandas-docs/stable/index.html>`__
-           *datafold* uses pandas'
-           `DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`__
-           as a base class for ``TSCDataFrame``, which captures time series data and
-           collections thereof. The data structure indexes time, time series ID and
-           one-or-many spatial features. It includes specific time series collection functionality
-           and is compatible with pandas rich functionality.
-        
-        * `scikit-learn <https://scikit-learn.org/stable/>`__
-           All *datafold* algorithms that are part of the "machine learning pipeline" align
-           to the scikit-learn `API <https://scikit-learn.org/stable/developers/develop.html>`__.
-           This is done by deriving the models from
-           `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
-           and appropriate `MixIns`. *datafold* defines own `MixIns` that align with the
-           API in a duck-typing fashion to allow identifying dynamical systems from temporal data
-           in ``TSCDataFrame``.
-        
-        * `SciPy <https://docs.scipy.org/doc/scipy/reference/index.html>`__
-           The package is used for elementary numerical algorithms and data structures in
-           conjunction with NumPy. This includes (sparse) linear least
-           square regression, (sparse) eigenpairs solver and sparse matrices as
-           optional data structure for kernel matrices.
-        
-        How does it compare to other software?
-        ======================================
-        
-        *The selection only includes other Python packages.*
-        
-        * `scikit-learn <https://scikit-learn.org/stable/>`__
-           provides algorithms and models along the entire machine learning pipeline, with a
-           strong focus on static data (i.e. without temporal context). *datafold* integrates
-           into scikit-learn' API and all data-driven models are subclasses of
-           `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
-           An important contribution of *datafold* is the ``DiffusionMaps`` model as popular
-           framework for manifold learning, which is not contained in scikit-learn's `set of
-           algorithms <https://scikit-learn.org/stable/auto_examples/manifold/plot_compare_methods
-           .html#sphx-glr-auto-examples-manifold-plot-compare-methods-py>`__.
-           Furthermore, *datafold* includes dynamical systems as a new model class that is
-           operable with scikit-learn - the attributes align to supervised learning tasks.
-           The key differences are that a model processes data of type ``TSCDataFrame``
-           and instead of a one-to-one relation in the model's input/output, the model can return
-           arbitrary many output samples (a time series) for a single input
-           (an initial condition).
-        
-        * `PyDMD <https://mathlab.github.io/PyDMD/build/html/index.html>`__
-           provides many variants of the `Dynamic Mode Decomposition (DMD) <https://en.wikipedia.org/wiki/Dynamic_mode_decomposition>`__.
-           *datafold* provides a wrapper to make models of ``PyDMD`` accessible. However, a
-           limitation of ``PyDMD`` is that it only processes single coherent time series, see
-           `PyDMD issue 86 <https://github.com/mathLab/PyDMD/issues/86>`__. The DMD models that
-           are directly included in *datafold* utilize the functionality of the data
-           structure ``TSCDataFrame`` and can therefore process time
-           series collections - in an extreme case only containing snapshot pairs.
-        
-        * `PySINDy <https://pysindy.readthedocs.io/en/latest/>`__
-           specializes on a *sparse* system identification of nonlinear dynamical systems to
-           infer governing equations.
-        
 Keywords: mathematics, machine learning, dynamical system, data-driven, time series, regression, forecasting, manifold learning, diffusion map, koopman operator, nonlinear
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: LICENSES_bundled
+
+Quick links
+^^^^^^^^^^^
+
+`Source repository <https://gitlab.com/datafold-dev/datafold>`__ |
+`Contributing and feedback <https://datafold-dev.gitlab.io/datafold/contributing.html>`__ |
+`PyPI <https://pypi.org/project/datafold/>`__ |
+`Documentation <https://datafold-dev.gitlab.io/datafold/>`__ |
+`Tutorials <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__ |
+`Scientific literature <https://datafold-dev.gitlab.io/datafold/references.html>`__
+
+What is *datafold*?
+====================
+
+*datafold* is a `MIT-licensed <https://gitlab.com/datafold-dev/datafold/-/blob/master/LICENSE>`__
+Python package containing operator-theoretic, data-driven models to identify dynamical
+systems from time series data and to infer geometrical structures in point clouds.
+
+The package includes:
+
+* An efficient implementation of the ``DiffusionMaps`` model to infer geometric
+  meaningful structures from data, such as the eigenfunctions of the
+  Laplace-Beltrami operator. As a distinguishing factor to other implementations, the
+  model can handle a sparse kernel matrix and allows setting an arbitrary kernel,
+  including the standard Gaussian kernel,
+  `continuous k-nearest neighbor kernel <https://arxiv.org/abs/1606.02353>`__, or
+  `dynamics-adapted cone kernel <https://cims.nyu.edu/~dimitris/files/Giannakis15_cone_kernels.pdf>`__.
+* Implementations and variants of the Dynamic Mode Decomposition as data-driven methods to
+  identify and analyze dynamical systems from time series collection data. This incldues:
+  * ``DMDFull`` or ``DMDEco`` as standard methods of DMD
+  * ``OnlineDMD`` or ``StreamingDMD`` modify the DMD to handle streaming data
+  * ``DMDControl`` augments the DMD to handle additional control input
+  * ``EDMD`` - The Extended-DMD, which allows setting up a highly flexible dictionary to
+  transform time series data and thereby handle nonlinear dynamics within the Koopman
+  operator framework. The EDMD wraps an arbitrary DMD variation for the decomposition.
+  The key advantage of this is, that the ``EDMD`` directly profits from the above
+  functionalities. ``EDMD`` can be used in control or streaming settings. Furthermore it is
+  possible to learn the dictionary directly from data (commonly referred to EDMD-DL)
+* Handling of cross-validation. The method ``EDMDCV``, for example, allows model parameters to
+  be optimized with cross-validation splittings that account for the temporal order in time
+  series data.
+* Methods to perform Model Predictive Control (MPC) with Koopman operator-based methods (
+  mainly the ``EDMD``). *This is currently still under development and experimental*.
+* Regression models for high-dimensional data (often used for out-of-sample extensions for the
+  Diffusion Maps model), such as the (auto-tuned) Laplacian Pyramids or Geometric Harmonics to
+  interpolate general function values on a point cloud manifold.
+* A data structure ``TSCDataFrame`` to handle time series collection data. It simplifies model
+  inputs/outputs and make it easier to describe various forms of time series data.
+
+See also `this introduction page <https://datafold-dev.gitlab.io/datafold/intro.html>`__.
+For a mathematical thorough introduction, we refer to the `scientific literature
+<https://datafold-dev.gitlab.io/datafold/references.html>`__.
+
+.. note::
+    The project is under active development in a research-driven environment.
+
+    * Code quality varies from "experimental/early stage" to "well-tested". Well tested
+      code is listed in the
+      `software documentation <https://datafold-dev.gitlab.io/datafold/api.html>`__
+      and are directly accessible through the highest module level (e.g.
+      :code:`from datafold import ...`). Experimental code is
+      only accessible via "deep imports" (e.g.
+      :code:`from datafol.dynfold.outofsample import ...`) and may raise a warning when using
+      it.
+    * The interfaces within *datafold* are not stable. The software is **not** intended for
+      production. Nevertheless, if we break something it is intentional and we hope that such
+      adaptations become less over time.
+    * There is no deprecation cycle. The software uses
+      `semantic versioning <https://semver.org/>`__ policy `[major].[minor].[patch]`, i.e.
+
+         * `major` - making incompatible changes in the (documented) API
+         * `minor` - adding functionality in a backwards-compatible manner
+         * `patch` - backwards-compatible bug fixes
+
+      We do not intend to indicate a feature complete milestone with version `1.0`.
+
+Cite
+====
+
+If you use *datafold* in your research, please cite
+`this paper <https://joss.theoj.org/papers/10.21105/joss.02283>`__ published in the
+*Journal of Open Source Software* (`JOSS <https://joss.theoj.org/>`__).
+
+*Lehmberg et al., (2020). datafold: data-driven models for point clouds and time series on
+manifolds. Journal of Open Source Software, 5(51), 2283,* https://doi.org/10.21105/joss.02283
+
+BibTeX:
+
+.. code-block:: latex
+
+    @article{Lehmberg2020,
+             doi       = {10.21105/joss.02283},
+             url       = {https://doi.org/10.21105/joss.02283},
+             year      = {2020},
+             publisher = {The Open Journal},
+             volume    = {5},
+             number    = {51},
+             pages     = {2283},
+             author    = {Daniel Lehmberg and Felix Dietrich and Gerta K{\"o}ster and Hans-Joachim Bungartz},
+             title     = {datafold: data-driven models for point clouds and time series on manifolds},
+             journal   = {Journal of Open Source Software}}
+
+How to get it?
+==============
+
+Installation requires `Python>=3.9 <https://www.python.org/>`__ with
+`pip <https://pip.pypa.io/en/stable/>`__ and
+`setuptools <https://setuptools.pypa.io/en/latest/>`__ installed (both packages ship with a
+standard Python installation). The package dependencies
+install automatically. The main dependencies and their usage in *datafold* are listed
+in the section "Dependencies" below.
+
+There are two ways to install *datafold*:
+
+1. From PyPI
+------------
+
+This is the standard way for users. The package is hosted on the official Python package
+index (PyPI) and installs the core package (excluding tutorials and tests). The tutorial
+files can be downloaded separately
+`here <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__.
+
+To install the package and its dependencies with :code:`pip`, run
+
+.. code-block:: bash
+
+   python -m pip install datafold
+
+.. note::
+
+    If you run Python in an Anaconda environment you can use pip from within ``conda``.
+    See also
+    `official instructions <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages>`__.
+
+    .. code-block:: bash
+
+        conda activate venv
+        conda install pip
+        pip install datafold
+
+2. From source
+--------------
+
+This way is recommended if you want to access the latest (but potentially unstable)
+development state, run tests or wish to contribute (see section "Contributing" for details).
+Download or git-clone the source code repository.
+
+1. Download the repository
+
+   a. If you wish to contribute code, it is required to have
+      `git <https://git-scm.com/>`__ installed. Clone the repository with
+
+      .. code-block:: bash
+
+        git clone https://gitlab.com/datafold-dev/datafold.git
+
+   b. If you only want access to the source code (current ``master`` branch), download one
+      of the compressed file types
+      (`zip <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.zip>`__,
+      `tar.gz <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.gz>`__,
+      `tar.bz2 <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.bz2>`__,
+      `tar <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar>`__)
+
+2. Install the package from the downloaded repository
+
+   .. code-block:: bash
+
+       python -m pip install .
+
+Contributing
+============
+
+Any contribution (code/tutorials/documentation improvements), question or feedback is
+very welcome. Either use the
+`issue tracker <https://gitlab.com/datafold-dev/datafold/-/issues>`__ or
+`Email <incoming+datafold-dev-datafold-14878376-issue-@incoming.gitlab.com>`__ us.
+Instructions to set up *datafold* for development can be found
+`here <https://datafold-dev.gitlab.io/datafold/contributing.html>`__.
+
+Dependencies
+============
+
+The dependencies of the core package are managed in the file
+`requirements.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements.txt>`__
+and install with *datafold*. The tests, tutorials, documentation and code analysis
+require additional dependencies which are managed in
+`requirements-dev.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements-dev.txt>`__.
+
+*datafold* integrates with common packages from the
+`Python scientific computing stack <https://scipy.org/about/>`__:
+
+* `NumPy <https://numpy.org/>`__
+   NumPy is used throughout *datafold* and is the default package for numerical
+   data and algorithms.
+
+* `pandas <https://pandas.pydata.org/pandas-docs/stable/index.html>`__
+   *datafold* uses pandas'
+   `DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`__
+   as a base class for ``TSCDataFrame`` to capture various forms of time series data. The data
+   It includes specific time series collection functionality and is mostly compatible with
+   pandas' rich functionality.
+
+* `scikit-learn <https://scikit-learn.org/stable/>`__
+   All *datafold* algorithms that are part of the "machine learning pipeline" align
+   to the scikit-learn `API <https://scikit-learn.org/stable/developers/develop.html>`__.
+   This is done by deriving the models from
+   `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
+   and appropriate ``MixIns``. *datafold* defines own ``MixIns`` that align with the
+   API in a duck-typing fashion to allow identifying dynamical systems from temporal data
+   in ``TSCDataFrame``.
+
+* `SciPy <https://docs.scipy.org/doc/scipy/reference/index.html>`__
+   The package is used for elementary numerical algorithms and data structures in
+   conjunction with NumPy. This includes (sparse) linear least
+   square regression, (sparse) eigenpairs solver and sparse matrices as
+   optional data structure for kernel matrices.
+
+How does it compare to other software?
+======================================
+
+*Note: This list covers only Python packages.*
+
+* `scikit-learn <https://scikit-learn.org/stable/>`__
+   provides algorithms and models along the entire machine learning pipeline, with a
+   strong focus on static data (i.e. without temporal context). *datafold* integrates
+   into scikit-learn' API and all data-driven models are subclasses of
+   `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
+   An important contribution of *datafold* is the ``DiffusionMaps`` model as popular
+   framework for manifold learning, which is not contained in scikit-learn's `set of
+   algorithms <https://scikit-learn.org/stable/auto_examples/manifold/plot_compare_methods
+   .html#sphx-glr-auto-examples-manifold-plot-compare-methods-py>`__.
+   Furthermore, *datafold* includes dynamical systems as a new model class that is
+   operable with scikit-learn - the attributes align to supervised learning tasks.
+   The key differences are that a model processes data of type ``TSCDataFrame``
+   and instead of a one-to-one relation in the model's input/output, the model can return
+   arbitrary many output samples (a time series) for a single input
+   (an initial condition).
+
+* `PyDMD <https://github.com/PyDMD/PyDMD>`__
+   provides many variants of the `Dynamic Mode Decomposition (DMD)
+   <https://en.wikipedia.org/wiki/Dynamic_mode_decomposition>`__. *datafold* provides a wrapper
+   to make models of ``PyDMD`` accessible. However, a limitation of ``PyDMD`` is that it only
+   processes single coherent time series, see `PyDMD issue 86
+   <https://github.com/PyDMD/PyDMD/issues/86>`__. The DMD models that are directly included
+   in *datafold* utilize the functionality of the data structure ``TSCDataFrame`` and can
+   therefore process time series collections - in an extreme case only containing snapshot
+   pairs.
+
+* `PySINDy <https://pysindy.readthedocs.io/en/latest/>`__
+   specializes on a *sparse* system identification of nonlinear dynamical systems to
+   infer governing equations.
```

### Comparing `datafold-1.1.6/README.rst` & `datafold-2.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,64 +13,70 @@
 
 *datafold* is a `MIT-licensed <https://gitlab.com/datafold-dev/datafold/-/blob/master/LICENSE>`__
 Python package containing operator-theoretic, data-driven models to identify dynamical
 systems from time series data and to infer geometrical structures in point clouds.
 
 The package includes:
 
-* Data structures to handle point clouds on manifolds (``PCManifold``) and time series
-  collections (``TSCDataFrame``). The data structures are used both internally and for
-  model input/outputs. In contrast to solutions found in other projects, such as
-  lists of Numpy arrays, ``TSCDataFrame`` makes it much easier to describe many forms of
-  time series data in a single object.
 * An efficient implementation of the ``DiffusionMaps`` model to infer geometric
   meaningful structures from data, such as the eigenfunctions of the
   Laplace-Beltrami operator. As a distinguishing factor to other implementations, the
   model can handle a sparse kernel matrix and allows setting an arbitrary kernel,
   including the standard Gaussian kernel,
   `continuous k-nearest neighbor kernel <https://arxiv.org/abs/1606.02353>`__, or
   `dynamics-adapted cone kernel <https://cims.nyu.edu/~dimitris/files/Giannakis15_cone_kernels.pdf>`__.
-* Out-of-sample extensions for the Diffusion Maps model, such as the (auto-tuned)
-  Laplacian Pyramids or Geometric Harmonics to interpolate general function values on a
-  point cloud manifold.
-* An implementation of the (Extended-) Dynamic Mode Decomposition (e.g. model ``DMDFull``
-  or ``EDMD``) as data-driven methods to identify dynamical systems from time series
-  collection data. ``EDMD`` subclasses from the flexible scikit-learn
-  `Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`__,
-  which allows setting up and transforming time series collection data to a more suitable
-  feature state (cf. Koopman operator theory).
-* ``EDMDCV`` allows model parameters to be optimized with cross-validation splittings that
-  account for the temporal order in time series collections.
+* Implementations and variants of the Dynamic Mode Decomposition as data-driven methods to
+  identify and analyze dynamical systems from time series collection data. This incldues:
+  * ``DMDFull`` or ``DMDEco`` as standard methods of DMD
+  * ``OnlineDMD`` or ``StreamingDMD`` modify the DMD to handle streaming data
+  * ``DMDControl`` augments the DMD to handle additional control input
+  * ``EDMD`` - The Extended-DMD, which allows setting up a highly flexible dictionary to
+  transform time series data and thereby handle nonlinear dynamics within the Koopman
+  operator framework. The EDMD wraps an arbitrary DMD variation for the decomposition.
+  The key advantage of this is, that the ``EDMD`` directly profits from the above
+  functionalities. ``EDMD`` can be used in control or streaming settings. Furthermore it is
+  possible to learn the dictionary directly from data (commonly referred to EDMD-DL)
+* Handling of cross-validation. The method ``EDMDCV``, for example, allows model parameters to
+  be optimized with cross-validation splittings that account for the temporal order in time
+  series data.
+* Methods to perform Model Predictive Control (MPC) with Koopman operator-based methods (
+  mainly the ``EDMD``). *This is currently still under development and experimental*.
+* Regression models for high-dimensional data (often used for out-of-sample extensions for the
+  Diffusion Maps model), such as the (auto-tuned) Laplacian Pyramids or Geometric Harmonics to
+  interpolate general function values on a point cloud manifold.
+* A data structure ``TSCDataFrame`` to handle time series collection data. It simplifies model
+  inputs/outputs and make it easier to describe various forms of time series data.
 
 See also `this introduction page <https://datafold-dev.gitlab.io/datafold/intro.html>`__.
 For a mathematical thorough introduction, we refer to the `scientific literature
 <https://datafold-dev.gitlab.io/datafold/references.html>`__.
 
 .. note::
     The project is under active development in a research-driven environment.
 
     * Code quality varies from "experimental/early stage" to "well-tested". Well tested
       code is listed in the
       `software documentation <https://datafold-dev.gitlab.io/datafold/api.html>`__
-      and are directly accessible through the package levels ``pcfold``, ``dynfold`` or
-      ``appfold`` (e.g. :code:`from datafold.dynfold import ...`). Experimental code is
-      only accessible via "deep imports"
-      (e.g. :code:`from datafol.dynfold.outofsample import ...`) and may raise a warning
-      when using it.
-    * There is no deprecation cycle. Backwards compatibility is indicated by the
-      package version, where we use a `semantic versioning <https://semver.org/>`__
-      policy `[major].[minor].[patch]`, i.e.
+      and are directly accessible through the highest module level (e.g.
+      :code:`from datafold import ...`). Experimental code is
+      only accessible via "deep imports" (e.g.
+      :code:`from datafol.dynfold.outofsample import ...`) and may raise a warning when using
+      it.
+    * The interfaces within *datafold* are not stable. The software is **not** intended for
+      production. Nevertheless, if we break something it is intentional and we hope that such
+      adaptations become less over time.
+    * There is no deprecation cycle. The software uses
+      `semantic versioning <https://semver.org/>`__ policy `[major].[minor].[patch]`, i.e.
 
          * `major` - making incompatible changes in the (documented) API
          * `minor` - adding functionality in a backwards-compatible manner
          * `patch` - backwards-compatible bug fixes
 
       We do not intend to indicate a feature complete milestone with version `1.0`.
 
-
 Cite
 ====
 
 If you use *datafold* in your research, please cite
 `this paper <https://joss.theoj.org/papers/10.21105/joss.02283>`__ published in the
 *Journal of Open Source Software* (`JOSS <https://joss.theoj.org/>`__).
 
@@ -92,20 +98,20 @@
              author    = {Daniel Lehmberg and Felix Dietrich and Gerta K{\"o}ster and Hans-Joachim Bungartz},
              title     = {datafold: data-driven models for point clouds and time series on manifolds},
              journal   = {Journal of Open Source Software}}
 
 How to get it?
 ==============
 
-Installation requires `Python>=3.7 <https://www.python.org/>`__ with
+Installation requires `Python>=3.9 <https://www.python.org/>`__ with
 `pip <https://pip.pypa.io/en/stable/>`__ and
-`setuptools <https://setuptools.readthedocs.io/en/latest/>`__ installed. Both
-packages usually ship with a standard Python installation. The package dependencies
-install automatically. The main dependencies and their role in *datafold* are listed below
-in "Dependencies".
+`setuptools <https://setuptools.pypa.io/en/latest/>`__ installed (both packages ship with a
+standard Python installation). The package dependencies
+install automatically. The main dependencies and their usage in *datafold* are listed
+in the section "Dependencies" below.
 
 There are two ways to install *datafold*:
 
 1. From PyPI
 ------------
 
 This is the standard way for users. The package is hosted on the official Python package
@@ -127,101 +133,95 @@
 
     .. code-block:: bash
 
         conda activate venv
         conda install pip
         pip install datafold
 
-
 2. From source
 --------------
 
 This way is recommended if you want to access the latest (but potentially unstable)
-development, run tests or wish to contribute (see section "Contributing" for details).
+development state, run tests or wish to contribute (see section "Contributing" for details).
 Download or git-clone the source code repository.
 
 1. Download the repository
 
    a. If you wish to contribute code, it is required to have
       `git <https://git-scm.com/>`__ installed. Clone the repository with
 
       .. code-block:: bash
 
         git clone https://gitlab.com/datafold-dev/datafold.git
 
    b. If you only want access to the source code (current ``master`` branch), download one
-      of the compressed files
+      of the compressed file types
       (`zip <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.zip>`__,
       `tar.gz <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.gz>`__,
       `tar.bz2 <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.bz2>`__,
       `tar <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar>`__)
 
 2. Install the package from the downloaded repository
 
    .. code-block:: bash
 
        python -m pip install .
 
-
 Contributing
 ============
 
 Any contribution (code/tutorials/documentation improvements), question or feedback is
 very welcome. Either use the
 `issue tracker <https://gitlab.com/datafold-dev/datafold/-/issues>`__ or
-`Email <incoming+datafold-dev-datafold-14878376-issue-@incoming.gitlab.com>`__.
+`Email <incoming+datafold-dev-datafold-14878376-issue-@incoming.gitlab.com>`__ us.
 Instructions to set up *datafold* for development can be found
 `here <https://datafold-dev.gitlab.io/datafold/contributing.html>`__.
 
 Dependencies
 ============
 
 The dependencies of the core package are managed in the file
 `requirements.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements.txt>`__
 and install with *datafold*. The tests, tutorials, documentation and code analysis
 require additional dependencies which are managed in
 `requirements-dev.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements-dev.txt>`__.
 
 *datafold* integrates with common packages from the
-`Python scientific computing stack <https://www.scipy.org/about.html>`__:
+`Python scientific computing stack <https://scipy.org/about/>`__:
 
 * `NumPy <https://numpy.org/>`__
-   The data structure ``PCManifold`` subclasses from NumPy's
-   `ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`__. The
-   class attaches an kernel object to the data to describe point similarity.
    NumPy is used throughout *datafold* and is the default package for numerical
    data and algorithms.
 
 * `pandas <https://pandas.pydata.org/pandas-docs/stable/index.html>`__
    *datafold* uses pandas'
    `DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`__
-   as a base class for ``TSCDataFrame``, which captures time series data and
-   collections thereof. The data structure indexes time, time series ID and
-   one-or-many spatial features. It includes specific time series collection functionality
-   and is compatible with pandas rich functionality.
+   as a base class for ``TSCDataFrame`` to capture various forms of time series data. The data
+   It includes specific time series collection functionality and is mostly compatible with
+   pandas' rich functionality.
 
 * `scikit-learn <https://scikit-learn.org/stable/>`__
    All *datafold* algorithms that are part of the "machine learning pipeline" align
    to the scikit-learn `API <https://scikit-learn.org/stable/developers/develop.html>`__.
    This is done by deriving the models from
    `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
-   and appropriate `MixIns`. *datafold* defines own `MixIns` that align with the
+   and appropriate ``MixIns``. *datafold* defines own ``MixIns`` that align with the
    API in a duck-typing fashion to allow identifying dynamical systems from temporal data
    in ``TSCDataFrame``.
 
 * `SciPy <https://docs.scipy.org/doc/scipy/reference/index.html>`__
    The package is used for elementary numerical algorithms and data structures in
    conjunction with NumPy. This includes (sparse) linear least
    square regression, (sparse) eigenpairs solver and sparse matrices as
    optional data structure for kernel matrices.
 
 How does it compare to other software?
 ======================================
 
-*The selection only includes other Python packages.*
+*Note: This list covers only Python packages.*
 
 * `scikit-learn <https://scikit-learn.org/stable/>`__
    provides algorithms and models along the entire machine learning pipeline, with a
    strong focus on static data (i.e. without temporal context). *datafold* integrates
    into scikit-learn' API and all data-driven models are subclasses of
    `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
    An important contribution of *datafold* is the ``DiffusionMaps`` model as popular
@@ -231,19 +231,20 @@
    Furthermore, *datafold* includes dynamical systems as a new model class that is
    operable with scikit-learn - the attributes align to supervised learning tasks.
    The key differences are that a model processes data of type ``TSCDataFrame``
    and instead of a one-to-one relation in the model's input/output, the model can return
    arbitrary many output samples (a time series) for a single input
    (an initial condition).
 
-* `PyDMD <https://mathlab.github.io/PyDMD/build/html/index.html>`__
-   provides many variants of the `Dynamic Mode Decomposition (DMD) <https://en.wikipedia.org/wiki/Dynamic_mode_decomposition>`__.
-   *datafold* provides a wrapper to make models of ``PyDMD`` accessible. However, a
-   limitation of ``PyDMD`` is that it only processes single coherent time series, see
-   `PyDMD issue 86 <https://github.com/mathLab/PyDMD/issues/86>`__. The DMD models that
-   are directly included in *datafold* utilize the functionality of the data
-   structure ``TSCDataFrame`` and can therefore process time
-   series collections - in an extreme case only containing snapshot pairs.
+* `PyDMD <https://github.com/PyDMD/PyDMD>`__
+   provides many variants of the `Dynamic Mode Decomposition (DMD)
+   <https://en.wikipedia.org/wiki/Dynamic_mode_decomposition>`__. *datafold* provides a wrapper
+   to make models of ``PyDMD`` accessible. However, a limitation of ``PyDMD`` is that it only
+   processes single coherent time series, see `PyDMD issue 86
+   <https://github.com/PyDMD/PyDMD/issues/86>`__. The DMD models that are directly included
+   in *datafold* utilize the functionality of the data structure ``TSCDataFrame`` and can
+   therefore process time series collections - in an extreme case only containing snapshot
+   pairs.
 
 * `PySINDy <https://pysindy.readthedocs.io/en/latest/>`__
    specializes on a *sparse* system identification of nonlinear dynamical systems to
    infer governing equations.
```

### Comparing `datafold-1.1.6/datafold/_decorators.py` & `datafold-2.0.0/datafold/_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 def warn_known_bug(original_function=None, gitlab_issue=None):
     # Function copied from: https://stackoverflow.com/a/24617244
 
     def _decorate(function):
         @wraps(function)
         def wrapped_function(*args, **kwargs):
-
             if gitlab_issue is not None:
                 add_msg = (
                     f"\n\n See gitlab issue #{gitlab_issue} "
                     f"https://gitlab.com/datafold-dev/datafold/issues/{gitlab_issue} \n"
                 )
             else:
                 add_msg = ""
 
             warnings.formatwarning = warning_format
             warnings.warn(
                 f"Function '{function.__name__}' has a known bug. "
-                f"Use with caution {add_msg}"
+                f"Use with caution {add_msg}",
+                stacklevel=1,
             )
             return function(*args, **kwargs)
 
         return wrapped_function
 
     if original_function:
         return _decorate(original_function)
@@ -40,15 +40,16 @@
 
 def warn_experimental_function(original_function):
     def func_wrapper(*args, **kwargs):
         warnings.formatwarning = warning_format
         warnings.warn(
             f"Class '{original_function.__name__}' is marked as experimental. This means "
             f"the intended functionality may not be complete and there is no sufficient "
-            f"testing. Use function with caution!"
+            f"testing. Use function with caution!",
+            stacklevel=1,
         )
         return original_function(*args, **kwargs)
 
     return func_wrapper
 
 
 def warn_experimental_class(cls):
@@ -57,15 +58,16 @@
 
     @wraps(cls)
     def wrapper_class(*args, **kwargs):
         warnings.formatwarning = warning_format
         warnings.warn(
             f"Class '{cls.__name__}' is marked as experimental. This means "
             f"the intended functionality may not be complete and there is no sufficient "
-            f"testing. Use class with caution!"
+            f"testing. Use class with caution!",
+            stacklevel=1,
         )
         return cls(*args, **kwargs)
 
     return wrapper_class
 
 
 if __name__ == "__main__":
```

### Comparing `datafold-1.1.6/datafold/_version.py` & `datafold-2.0.0/datafold/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,39 +15,38 @@
 
     print(f"Platform:       {platform.platform()}")
     print(f"Python:         {python_version}")
     print(f"numpy:          {np.__version__}")
     print(f"pandas:         {pd.__version__}")
     print(f"scipy:          {scipy.__version__}")
     print(f"scikit-learn:   {sklearn.__version__}")
-    print(f"datafold:       {Version.v_short}")
 
 
 class Version:
     """Current datafold version."""
 
     # Semantic versioning policy
     # preferred by Python
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#semantic-versioning-preferred
 
     # See also https://semver.org/
 
     # TO UPDATE -- START
-    major_version: int = 1  # making incompatible API changes,
-    minor_version: int = 1  # adding functionality in a backwards-compatible manner
-    patch: int = 6  # for backwards-compatible bug fixes
+    major_version: int = 2  # making incompatible API changes,
+    minor_version: int = 0  # adding functionality in a backwards-compatible manner
+    patch: int = 0  # for backwards-compatible bug fixes
 
     # additional release suffixes
     post: int = 0  # for minor corrections
-    rc: int = 0  # for release candidate (e.g. for testing upload to PyPI)
+    rc: int = 0  # for release candidate (e.g. to test upload to PyPI-test)
 
     # Set date of release for longer version numbers.
-    year: int = 2021
-    month: int = 12
-    day: int = 2
+    year: int = 2023
+    month: int = 7
+    day: int = 31
     # TO UPDATE -- END
 
     assert major_version >= 0 and isinstance(major_version, int)
     assert minor_version >= 0 and isinstance(minor_version, int)
     assert patch >= 0 and isinstance(patch, int)
     assert post >= 0 and isinstance(post, int)
     assert rc >= 0 and isinstance(rc, int)
@@ -68,10 +67,11 @@
     def print_version():
         print(f"v_short = {Version.v_short}")
         print(f"v_long  = {Version.v_long}")
         print(f"v_gnu   = {Version.v_gnu}")
 
 
 if __name__ == "__main__":
+    print("datafold:")
     Version.print_version()
     print()
     show_versions()
```

### Comparing `datafold-1.1.6/datafold/appfold/__init__.py` & `datafold-2.0.0/datafold/appfold/__init__.py`

 * *Files identical despite different names*

### Comparing `datafold-1.1.6/datafold/appfold/edmd.py` & `datafold-2.0.0/datafold/appfold/edmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This file contains code that is copied and modified from
+"""This file contains code that is copied and modified from:
 
 scikit-learn
 version 0.24.1.
 repository: https://github.com/scikit-learn/scikit-learn/
 project homepage: https://scikit-learn.org/stable/
 
 Specifically, this applies to the following files and functions:
@@ -56,183 +56,268 @@
 import time
 import warnings
 from collections import defaultdict
 from copy import deepcopy
 from functools import partial
 from itertools import product
 from traceback import format_exc
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 import scipy.linalg
 import scipy.sparse
 from joblib import Parallel, delayed, logger
-from sklearn.base import clone
+from sklearn.base import BaseEstimator, clone
 from sklearn.exceptions import FitFailedWarning, NotFittedError
 from sklearn.model_selection import GridSearchCV, check_cv
 from sklearn.model_selection._validation import _num_samples, _score, is_classifier
 from sklearn.pipeline import Pipeline
 from sklearn.utils import _print_elapsed_time, check_scalar
 from sklearn.utils.validation import _check_fit_params, check_is_fitted, indexable
 
-from datafold.dynfold import DMDBase, DMDFull
+from datafold._decorators import warn_experimental_class
+from datafold.dynfold import DMDBase, DMDStandard
 from datafold.dynfold.base import (
     InitialConditionType,
     TimePredictType,
     TransformType,
     TSCPredictMixin,
     TSCTransformerMixin,
 )
+from datafold.dynfold.dictlearning import DMDDictLearning
 from datafold.pcfold import InitialCondition, TSCDataFrame, TSCKfoldSeries, TSCKFoldTime
 from datafold.pcfold.timeseries.metric import TSCCrossValidationSplit
 from datafold.utils.general import (
     df_type_and_indices_from,
-    is_integer,
-    projection_matrix_from_features,
+    if1dim_rowvec,
+    projection_matrix_from_feature_names,
 )
 
 
 class EDMD(
     Pipeline,
     TSCTransformerMixin,
     TSCPredictMixin,
 ):
-    """Extended Dynamic Mode Decomposition.
+    r"""Extended Dynamic Mode Decomposition.
+
+    The aim of this method is to construct a data-driven model that can approximate the
+    Koopman operator from a collection of time series data, represented by a
+    :py:class:`TSCDataFrame`. The method uses a (finite) function basis and may include
+    non-linear transformations of the data to enhance the function space (compared to a
+    dynamic mode decomposition). The model is similar to :class:`sklearn.pipeline.Pipeline`,
+    where the EDMD-dictionary corresponds to the transformations in the pipeline and a
+    :class:`DMDBase` model acts as the final estimator of the pipeline, approximating the
+    Koopman operator using the EDMD-dictionary time series. Unlike a scikit-learn Pipeline,
+    this model not only maps states forward to the EDMD-dictionary but also reconstructs
+    them to the original full-state time series, typically via Koopman modes.
+
+    If the DMD model (as the final estimator of the pipeline) computes the eigenpairs of the
+    Koopman matrix, then the EDMD model will provide the Koopman triplet comprising
+    modes :math:`V`, eigenvalues :math:`\Lambda`, and eigenfunctions :math:`\xi(\mathbf{x})`.
 
-    A data-driven model to approximate the Koopman operator from time series collection
-    data (:py:class:`.TSCDataFrame`) with a finite function basis, specified by the
-    data transformations in the EDMD-dictionary. The model is similar to the superclass
-    :class:`sklearn.pipeline.Pipeline`, in that the EDMD-dictionary corresponds to the
-    transformations in the pipeline and a :class:`.DMDBase` model, approximating the
-    Koopman operator on the EDMD-dictionary time series, is set as the final estimator. A
-    key difference is that the intrinsic EDMD-dictionary states are usually mapped
-    back to full-state time series.
+    .. math::
 
-    If the internal DMD model computes the eigenpairs of the Koopman matrix, then the
-    EDMD model provides the Koopman triplet (modes, eigenvalues and eigenfunctions).
+        \mathbf{x}_{k} = V \Lambda^k \xi(\mathbf{x}_0)
 
     ...
 
     Parameters
     ----------
     dict_steps
         List with `(string_identifier, model)` of models to transform the data. The
         list defines the transformation pipeline and order of execution. All models in
         the list must be able to accept :class:`.TSCDataFrame` as input in `fit` and
         output in `transform`.
 
     dmd_model
-        A :py:class:`.DMDBase` as the final estimator. The DMD model either
-        approximates the Koopman operator or generator based on the EDMD-dictionary data.
+        An model that subclasses :py:class:`.DMDBase`. The model servies as the final
+        estimator in the pipeline. The DMD model either approximates the Koopman
+        operator or generator based on specified time series of the EDMD-dictionary data.at f
 
     include_id_state
-        If True, the original time series data are added to the EDMD-dictionary. The
-        mapping from the EDMD-dictionary states back to the full-state is then only a
-        projection and the cost of an increased EDMD-dictionary dimension.
+        If True, the original time series states are added to the EDMD dictionary. The
+        mapping from the EDMD dictionary states back to the full-state is then only a
+        projection at the cost of an increased EDMD-dictionary dimension. The parameter has
+        no effect if all elements in the pipeline preserve the original states in their output,
+        as this would duplicate data and lead to conflicts in the feature names (see also
+        parameter ``dict_preserves_id_state_``).
+
+    dict_preserves_id_state: str, bool, defaults to "infer"
+        The parameter indicates whether the final dictionary include the original full
+        state. If the parameter is set to
+
+        * True, then this simplifies the inverse map to a projection on the full
+          state coordinates. In this case the parameter ``include_id_state`` is ignored because
+          the full state is already contained. An error is raised if not all features can be
+          matched.
+        * False, then the dictionary does not contain the features of the original full state.
+          If also ``include_id_state=False``, then the (linear) inverse map from dictionary to
+          full state is computed in a least squares sense.
+        * "infer", then there is a routine that checks whether the feature names of the full
+          state are contained in the dictionary, i.e. ``feature_names_in_`` in
+          ``feature_names_out_``. Note that only feature names are matched, there is no
+          guarantee that the values are changed during the dictionary transformation.
+
+    stepwise_transform
+        Controls whether stepwise (i.e. in every time step of a prediction) the inverse and
+        forward map between original and dictionary space is performed. When enabled this
+        can improve the overall predictive accuracy of model. For performance reasons it can be
+        worthwhile to enable ``diagonalize`` in the DMD method (to avoid a least squares
+        optimization in each timestep).
+
+        .. note::
+
+            This feature is still in an experimental phase and does not work for all settings
+            (e.g. if ``y is not None`` during ``fit`` or within ``partial_fit`` for streaming).
 
     sort_koopman_triplets
         Sort the Koopman triplets by the mean absolute value of the initial
         Koopman eigenfunctions of the data passed during fit. Ignored if the Koopman
-        triplet ist not available. Adapted from :cite:`manojlovic_applications_2020`.
+        triplet ist not available. Sorting criteria is adapted from :cite:t:`manojlovic-2020`.
 
     use_transform_inverse
         If True, the mapping from EDMD-dictionary states to the full-state is
         performed with ``inverse_transform`` by the models included the dictionary in
         reverse order. Note that all models need to provide ``inverse_transform``.
 
-    memory: :class:`Optional[None, str, object]`, :class:`object` with the \
+    memory: :class:`Optional[None, str, object]`, :class:`object` with the
     `joblib.Memory` interface
         Used to cache the fitted transformers of the pipeline. By default, no caching is
         performed. If a string is given, it is the path to the caching directory.
         Enabling caching triggers a clone of the transformers before fitting. Therefore,
         the transformer instance given to the pipeline cannot be inspected directly.
         Use the attribute ``named_steps`` or ``steps`` to inspect estimators within the
         pipeline. Caching the transformers is advantageous when fitting is time consuming.
 
     verbose: :class:`bool`
         If True, the time elapsed while fitting each step will be printed as it is
         completed.
 
     Attributes
     ----------
-
     n_features_in_
-        The number of features in the full-state time series (data passed to `fit`).
+        The number of features in the full-state time series (data passed to ``fit``).
 
     feature_names_in_
-        The features names in the full-state time series (data passed to `fit`).
+        The features names in the full-state time series (data passed to ``fit``).
 
     n_features_out_
         The number of features in the EDMD-dictionary time series.
 
     feature_names_out_
         The feature names in the EDMD-dictionary time series.
 
     feature_names_pred_
         The feature names in time series predictions.
 
     named_steps: :class:`Dict[str, object]`
         Read-only attribute to access the EDMD-dictionary models by given name.
 
+    dict_preserves_id_state_: bool
+        Boolean flag of whether the full state is contained in the dictionary state. The
+        attribute depends on the initialization parameters `include_id_state` and
+        `dict_preserves_id_state`.
+
+    is_partial_fit_: bool
+        A boolean flag indicating whether the model is fit using the ``partial_fit`` method
+        If True, then only ``partial_fit`` can be used to initially fit or update the model.
+
+    is_controlled_: bool
+        Indicates whether the system is controlled. When True, it indicates that
+        the input control signals (``U``) were provided during the ``fit`` method,
+        allowing the model to consider the influence of control on the system dynamics.
+
+    is_state_transition_map_: bool
+        A flag indicating whether a the dictionary states are used to reconstruct a
+        different set of state variables (i.e. different states than the ones included in the
+        initial condition). These states are passed as the ``y`` parameter in ``fit``.
+
+    transition_map_contains_id_:
+        A flag indicating whether the original states are included in the state transition map
+        (only applicable if ``is_state_transition_map_ is True``). Note that for the check
+        only feature names are matched (not the actual original values).
+
+    is_dict_learning_: bool
+        Indicates whether the DMD method (as the final estimator of the pipeline) learns
+        dictionary functions before computing the system matrix (or spectral components).
+        If True, the ``fit`` method manipulates the model's pipeline by appending a new
+        transform model. See the ``DMDDictLearning`` class for more details.
+
     koopman_modes: Optional[pandas.DataFrame]
         A ``DataFrame`` of shape `(n_features_original_space, n_features_dict_space)`
-        with the modes to map Koopman eigenfunctions to the full-state. The attribute is
-        ``None`` if ``use_inverse_transform=True`` or if the DMD model does not provide
-        the right eigenvectors of the Koopman matrix.
+        containing the modes which linearly map Koopman eigenfunctions back to the full-state.
+        The attribute is ``None`` if ``use_inverse_transform=True`` or if the DMD model does
+        not provide spectral components of the Koopman matrix.
 
-    koopman_eigenvalues: pandas.Series
+    koopman_eigenvalues: Optinal[pandas.Series]
         The approximate eigenvalues of the Koopman operator or generator of
-        shape `(n_features_dict,)`. The attribute is ``None`` if the DMD model does not
-        provide the right eigenvectors of the Koopman matrix.
+        shape `(n_features_dict,)`. The attribute is ``None`` if
+        ``use_inverse_transform=True`` or if the DMD model does not provide spectral
+        components of the system matrix (Koopman matrix).
 
     n_samples_ic_: int
         The number of time samples required for an initial condition. If the value is
         larger than 1, then for an initial condition a time series is required with the
         same sampling interval of the time series during fit.
 
     See Also
     --------
-
-    :py:class:`EDMDCV`
+    :py:class:`EDMDCV` :py:class:`DMDStandard`
 
     References
     ----------
-    :cite:`williams_datadriven_2015`
-    :cite:`manojlovic_applications_2020`
+    * :cite:t:`williams-2015` for the original EDMD description
+    * :cite:t:`manojlovic-2020` for sorting the spectral Koopman components
+    * :cite:t:`korda-2018` for EDMD with control
+    * :cite:t:`li-2017` for EDMD with dictionary learning
 
     """
 
     def __init__(
         self,
-        dict_steps: List[Tuple[str, object]],
+        dict_steps: list[tuple[str, object]],
         dmd_model: Optional[DMDBase] = None,
         *,
         include_id_state: bool = True,
+        dict_preserves_id_state: Union[Literal["infer"], bool] = "infer",
+        stepwise_transform: bool = False,
         use_transform_inverse: bool = False,
-        sort_koopman_triplets: bool = False,  # TODO: docu
+        sort_koopman_triplets: bool = False,
         memory: Optional[Union[str, object]] = None,
         verbose: bool = False,
     ):
-
         self.dict_steps = dict_steps
-        self.dmd_model = dmd_model if dmd_model is not None else DMDFull()
         self.include_id_state = include_id_state
+        self.dict_preserves_id_state = dict_preserves_id_state
+        self.stepwise_transform = stepwise_transform
         self.use_transform_inverse = use_transform_inverse
         self.sort_koopman_triplets = sort_koopman_triplets
 
         # TODO: if necessary provide option for user defined metric
         self._setup_default_tsc_metric_and_score()
 
-        all_steps = self.dict_steps + [("dmd", self.dmd_model)]
-        super(EDMD, self).__init__(steps=all_steps, memory=memory, verbose=verbose)
+        # type information for some attr set during model construction
+        self.dict_preserves_id_states_: bool
+        self.n_samples_ic_: int
+        self.is_partial_fit_: bool
+        self.is_state_transition_map_: bool
+        self.id_state_in_transition_map_: bool
+        self.is_controlled_: bool
+        self.is_dict_learning_: bool
+
+        if dmd_model is None:
+            dmd_model = DMDStandard()
+        all_steps = self.dict_steps + [("dmd", dmd_model)]
+        super().__init__(steps=all_steps, memory=memory, verbose=verbose)
 
     @property
-    def _dmd_model(self) -> DMDBase:
-        # Improves (internal) code readability when using  attribute
+    def dmd_model(self) -> DMDBase:
+        # Improves (internal) code readability when using attribute
         # '_dmd_model' instead of general '_final_estimator'
         return self._final_estimator
 
     @property
     def koopman_modes(self):
         check_is_fitted(self, attributes=["_koopman_modes"])
 
@@ -247,21 +332,21 @@
                 columns=[f"evec{i}" for i in range(self._koopman_modes.shape[1])],
             )
             return modes
 
     @property
     def koopman_eigenvalues(self):
         check_is_fitted(self)
-        if not self._dmd_model.is_spectral_mode():
+        if not self.dmd_model.is_spectral_mode:
             raise AttributeError(
-                "The DMD model was not configured to provide spectral "
+                "The underlying DMD model was not configured to provide spectral "
                 "components for the Koopman matrix."
             )
 
-        return pd.Series(self._dmd_model.eigenvalues_, name="evals")
+        return pd.Series(self.dmd_model.eigenvalues_, name="evals")
 
     def koopman_eigenfunction(self, X: TransformType) -> TransformType:
         r"""Evaluate the Koopman eigenfunctions.
 
         The Koopman eigenfunctions (:math:`\xi`) are spectrally aligned states of the
         EDMD-dictionary (:math:`g(x)`).
 
@@ -271,182 +356,178 @@
                 \xi(x) = \Psi^{-1} g(x)
 
         * If the DMD model only provides the right eigenvectors (:math:`\Psi`)
 
             .. math::
                 \xi(x) = \Psi^{\dagger} g(x)
 
-        See also Eq. 18 in :cite:`williams_datadriven_2015`.
+        See also Eq. 18 in :cite:t:`williams-2015`.
 
         Parameters
         ----------
-
         X : TSCDataFrame, pandas.DataFrame
-            The points of the original space at which to evaluate the Koopman
+            The samples of the original space at which to evaluate the Koopman
             eigenfunctions. If `n_samples_ic_ > 1`, then the input must be a
             :py:class:`.TSCDataFrame` where each time series must have at least
             ``n_samples_ic_`` samples, with the same time delta as during fit. The input
             must fulfill the first step in the pipeline.
 
         Returns
         -------
         Union[TSCDataFrame, pandas.DataFrame]
             The evaluated Koopman eigenfunctions. The number of samples are reduced
-            accordingly if :code:`n_samples_ic_ > 1` with fallback to
-            ``pandas.DataFrame`` if the it is not not a legal :py:class:`.TSCDataFrame`.
+            accordingly if :code:`n_samples_ic_ > 1`.
         """
         check_is_fitted(self)
-        if not self._dmd_model.is_spectral_mode():
+        if not self.dmd_model.is_spectral_mode:
             raise AttributeError(
-                "The DMD model was not configured to provide spectral "
-                "components for the Koopman matrix."
+                "The DMD model as final estimator was not configured to provide spectral "
+                "components of the identified system matrix."
             )
 
         X_dict = self.transform(X)
 
         # transform of X_dict matrix
         #   -> note that the transpose is required because in the DMD model the
         #      features are column oriented
-        eval_eigenfunction = self._dmd_model.compute_spectral_system_states(
+        eval_eigenfunction = self.dmd_model.compute_spectral_system_states(
             X_dict.to_numpy().T
         )
 
         columns = [f"koop_eigfunc{i}" for i in range(eval_eigenfunction.shape[0])]
         eval_eigenfunction = df_type_and_indices_from(
             indices_from=X_dict, values=eval_eigenfunction.T, except_columns=columns
         )
 
         return eval_eigenfunction
 
-    def _validate_dictionary(self):
-        # Check that elements in the EDMD-dictionary are TSCTransformer
-        for (_, trans_str, transformer) in self._iter(with_final=False):
-            if not isinstance(transformer, TSCTransformerMixin):
-                raise TypeError(
-                    "The EDMD-dictionary only supports transformers that can handle "
-                    "indexed data structures (pd.DataFrame and TSCDataFrame)"
-                )
-
-    @property
-    def feature_names_in_(self):
-        # delegate to first step (which will call _check_is_fitted)
-        # NOTE: n_features_in_ is also delegated, but already included in the super
-        # class Pipeline (implementation by sklearn)
-        return self.steps[0][1].feature_names_in_
-
     @property
     def n_features_out_(self):
         # Note: this returns the number of features by the dictionary transformation,
         # NOT from a EDMD prediction
-        return self._dmd_model.n_features_in_
+        # TODO: raise NotFittedError if trying to access before .fit? (relevant for all
+        #  following attrs)
+        return self.dmd_model.n_features_in_
 
     @property
     def feature_names_out_(self):
         # Note: this returns the feature names of the dictionary
         # transformation NOT from a EDMD prediction (see feature_names_pred_)
-        return self._dmd_model.feature_names_in_
+        return self.dmd_model.feature_names_in_
 
     @property
-    def feature_names_pred_(self):
-        return self._feature_names_pred
-
-    def transform(self, X: TransformType) -> TransformType:
-        """Perform dictionary transformations on time series.
-
-        Parameters
-        ----------
-        X : TSCDataFrame, pandas.DataFrame
-           Time series to transform. Must fulfill the input requirements of
-           first step of the pipeline. Each time series must have a minimum of
-           ``n_samples_ic_`` samples.
-
-        Returns
-        -------
-        TSCDataFrame, pandas.DataFrame
-            The transformed time series. The number of samples are reduced if
-            `n_samples_ic_ > 1`.
-        """
-        if self.include_id_state:
-            # copy required to properly attach X later on
-            X_dict = X.copy(deep=True)
+    def control_names_in_(self):
+        if self.is_controlled_:
+            return self.dmd_model.control_names_in_
         else:
-            X_dict = X
-
-        # carry out dictionary transformations:
-        for _, name, tsc_transform in self._iter(with_final=False):
-            X_dict = tsc_transform.transform(X_dict)
-
-        if self.include_id_state:
-            X_dict = self._attach_id_state(X=X, X_dict=X_dict)
+            return None
 
-        return X_dict
+    @property
+    def n_control_in_(self):
+        if self.is_controlled_:
+            return self.dmd_model.n_control_in_
+        else:
+            return None
 
-    def inverse_transform(self, X: TransformType) -> TransformType:
-        """Perform inverse dictionary transformations on dictionary time series.
+    @property
+    def feature_names_pred_(self):
+        # TODO: should TSCPredictMixin include feature names for prediction?
+        return self._feature_names_pred
 
-        The actual performed inverse transformation depends on the parameter settings
-        ``include_id_state`` and ``use_transform_inverse``.
+    def _validate_dictionary(self) -> bool:
+        """Validates that all elements in the EDMD dictionary.
 
-        Parameters
-        ----------
-        X: TSCDataFrame, pandas.DataFrame
-            Time series to map back to the full-state time series. The feature names
-            must match the ones in attribute ``feature_names_out_``.
+        During the validation the methods evaluates a flag to indicate whether the original
+        states are still the dictionary transformation.
 
         Returns
         -------
-        TSCDataFrame
-            full-state time series
+        bool
+            boolean flag if dictionary preserves the original states
         """
+        for _, _, transformer in self._iter(with_final=False):
+            if not isinstance(transformer, TSCTransformerMixin):
+                raise TypeError(
+                    "The EDMD dictionary only supports datafold transformers that handle the "
+                    "data structure 'TSCDataFrame'."
+                )
 
-        if self._inverse_map is not None:
-            # Note, here the samples are row-wise
-            values = X.to_numpy() @ self._inverse_map
+        return True
 
-            X_ts = df_type_and_indices_from(
-                indices_from=X, values=values, except_columns=self.feature_names_in_
-            )
+    def _set_dict_preserves_id_state(self, X_dict: TSCDataFrame) -> bool:
+        if self.dict_preserves_id_state == "infer":
+            return np.isin(self.feature_names_in_, X_dict.columns).all()
+        elif isinstance(self.dict_preserves_id_state, bool):
+            if self.dict_preserves_id_state and self.include_id_state:
+                warnings.warn(
+                    f"setting {self.dict_preserves_id_state=} and {self.include_id_state=} "
+                    f"duplicates the original features in the dictionary",
+                    stacklevel=1,
+                )
 
+            return self.dict_preserves_id_state
         else:
-            # inverse_transform the pipeline because an inverse linear map is not
-            # available.
-            X_ts = X
-            reverse_iter = reversed(list(self._iter(with_final=False)))
-            for _, _, tsc_transform in reverse_iter:
-                X_ts = tsc_transform.inverse_transform(X_ts)
-
-        return X_ts
+            raise ValueError(
+                f"Could not read {self.dict_preserves_id_state=}. Set to string "
+                f"'infer' or a boolean value"
+            )
 
     def _compute_n_samples_ic(self, X, X_dict):
         diff = X.n_timesteps - X_dict.n_timesteps
 
         if isinstance(diff, pd.Series):
             # time series can have different number of time values (in which case it is
-            # a Series), however, the the difference has to be the same for all time
-            # series
+            # a Series), however, the difference has to be the same for all time series
             assert (diff.iloc[0] == diff).all()
             diff = diff.iloc[0]
 
         # +1 because the diff indicates how many samples were removed -- we want the
         # number that is required for the initial condition
         return int(diff) + 1
 
-    def _least_squares_inverse_map(self, X, X_dict):
+    def _least_squares_inverse_map(self, X, X_dict, U):
         if isinstance(X, pd.DataFrame):
-            X = X.to_numpy()
+            if U is not None:
+                X = X.loc[U.index, :].to_numpy()
+            else:
+                X = X.to_numpy()
 
         if isinstance(X_dict, pd.DataFrame):
-            X_dict = X_dict.to_numpy()
+            if U is not None:
+                X_dict = X_dict.loc[U.index, :].to_numpy()
+                U = U.to_numpy()
+            else:
+                X_dict = X_dict.to_numpy()
 
-        return scipy.linalg.lstsq(X_dict, X, cond=None)[0]
+        if False and U is not None:
+            matrix = scipy.linalg.lstsq(np.column_stack([X_dict, U]), X, cond=None)[0]
+            self._inverse_map_control: np.ndarray = matrix[X_dict.shape[1] :, :]
+            return matrix[: X_dict.shape[1], :]
+        else:
+            return scipy.linalg.lstsq(X_dict, X, cond=None)[0]
 
-    def _compute_inverse_map(self, X: TSCDataFrame, X_dict: TSCDataFrame):
+    def _compute_inverse_map(
+        self, X: TSCDataFrame, y, X_dict: TSCDataFrame, U
+    ) -> Optional[Union[scipy.sparse.csr_matrix, np.ndarray]]:
         """Compute matrix that linearly maps from dictionary space to original feature
         space.
 
+        # TODO: If EDMD is controlled there is currently only a map from dictionary states to
+            the full-state representation.
+            - i.e.
+            X_dict B = X
+            -
+            However, the control states can also be included in the mapping, which can improve
+            the mapping
+            -
+            [X_dict, U] [B_dict, B_u] = X
+            -
+            This is also captured in a typical state space representation (matrix "D")
+            see https://en.wikipedia.org/wiki/State-space_representation#Linear_systems
+
         This is equivalent to matrix :math:`B`, Eq. 16 in
         :cite:`williams_datadriven_2015`.
 
         See also `_compute_koopman_modes` for further details.
 
         Parameters
         ----------
@@ -454,30 +535,40 @@
             Dictionary data.
 
         X
             Original full-state data.
 
         Returns
         -------
-        numpy.ndarray
+        numpy.ndarray, scipy.sparse.csr_matrix, None
 
         """
-
-        if self.include_id_state:
+        if (self.include_id_state or self.dict_preserves_id_state_) and y is None:
             # trivial case: we just need a projection matrix to select the
             # original full-states from the dictionary functions
-            inverse_map = projection_matrix_from_features(
-                X_dict.columns, self.feature_names_in_
-            )
+            try:
+                inverse_map = projection_matrix_from_feature_names(
+                    X_dict.columns, self.feature_names_in_
+                )
+            except ValueError as e:
+                # here it is assumed that the error is not raised if
+                # self.include_id_state=True because we have the control over it
+                raise ValueError(
+                    f"{self.dict_preserves_id_state_=} but not all features "
+                    f"names could be found in the dictionary's feature names"
+                ) from e
         else:
             # Compute the matrix in a least squares sense
             # inverse_map = "B" in Williams et al., Eq. 16
-            inverse_map = self._least_squares_inverse_map(
-                X=X.loc[X_dict.index, :], X_dict=X_dict
-            )
+            if y is None:
+                target = X.loc[X_dict.index, :]
+            else:
+                target = y.loc[X_dict.index, :]
+
+            inverse_map = self._least_squares_inverse_map(X=target, X_dict=X_dict, U=U)
 
         return inverse_map
 
     def _compute_koopman_modes(self, inverse_map: np.ndarray) -> np.ndarray:
         r"""Compute Koopman modes.
 
         The Koopman modes :math:`V` are a computed with
@@ -489,30 +580,30 @@
         features and :math:`\Psi_{DMD}` are the right eigenvectors of the Koopman
         matrix, computed in the internal DMD model.
 
         See :cite:`williams_datadriven_2015` Eq. 20.
 
         Parameters
         ----------
-
         inverse_map
             Matrix :math:`B`, as computed in :py:meth:`._compute_inverse_map`
 
         Returns
         -------
         numpy.ndarray
-            The computed Koopman modes.
+            Koopman modes
         """
-
-        koopman_modes = inverse_map.T @ self._dmd_model.eigenvectors_right_
+        # TODO: if the system is controlled, then currently the control state is not used to
+        #  possibly improve the reconstruction
+        koopman_modes = inverse_map.T @ self.dmd_model.eigenvectors_right_
         return koopman_modes
 
     def _sort_koopman_triplets(self, X_dict_ic: TSCDataFrame) -> None:
         r"""The ranking and sorting of Koopman triplets, adapted from
-        https://arxiv.org/pdf/2006.11765.pdf
+        https://arxiv.org/pdf/2006.11765.pdf.
 
         Given the Koopman mode decomposition
 
         .. math::
 
                 x_{j+1} = V \Lambda \xi(x_j} = \sum_{p=1}^P \vec{v}_p \lambda_p \xi_p(x_j)
 
@@ -539,230 +630,469 @@
         Finally, the triplets (modes, eigenvalues, eigenfunctions) are sorted
         from high importance to low importance according to their computed value.
 
         Parameters
         ----------
         X_dict_ic
             The initial states of the EDMD-dictionary time series.
-
-        Returns
-        -------
-
         """
-
         ic_koop_eigenfunc = self.dmd_model.compute_spectral_system_states(
             X_dict_ic.to_numpy().T
         )
 
         # the importance ranking is with the assumption that the modes are
         # normalized to 1 -- the factor corrects the ic_koop_eigenfunc accordingly
         # (1/factor * modes) * eigvals * (factor * eigfunc)
         factor = np.linalg.norm(self._koopman_modes, axis=0)
-        triplet_importance = np.abs((factor[:, np.newaxis] * ic_koop_eigenfunc))
+        triplet_importance = np.abs(factor[:, np.newaxis] * ic_koop_eigenfunc)
         # take the mean over all
         triplet_importance = np.mean(triplet_importance, axis=1)
 
         argsort_importance = np.argsort(triplet_importance.ravel())[::-1]
 
         # Sort everything:
         self._koopman_modes: np.ndarray = self._koopman_modes[:, argsort_importance]
-        self._dmd_model.eigenvalues_ = self._dmd_model.eigenvalues_[argsort_importance]
-        self._dmd_model.eigenvectors_right_ = self._dmd_model.eigenvectors_right_[
+        self.dmd_model.eigenvalues_ = self.dmd_model.eigenvalues_[argsort_importance]
+        self.dmd_model.eigenvectors_right_ = self.dmd_model.eigenvectors_right_[
             :, argsort_importance
         ]
 
         if (
-            hasattr(self._dmd_model, "eigenvectors_left_")
-            and self._dmd_model.eigenvectors_left_ is not None
+            hasattr(self.dmd_model, "eigenvectors_left_")
+            and self.dmd_model.eigenvectors_left_ is not None
         ):
             # Note the left eigenvectors are in the rows of the matrix by convention
-            self._dmd_model.eigenvectors_left_ = self._dmd_model.eigenvectors_left_[
+            self.dmd_model.eigenvectors_left_ = self.dmd_model.eigenvectors_left_[
                 argsort_importance, :
             ]
 
     def _attach_id_state(self, X, X_dict):
-        # remove states from X (the id-states) that are also removed during dictionary
-        # transformations
-        X = X.loc[X_dict.index, :]
+        # remove states from X that are also removed during dictionary mapping
+        if X.shape[0] > X_dict.shape[0]:
+            X = X.loc[X_dict.index, :]
+
         try:
             X = pd.concat([X, X_dict], axis=1)
-        except AttributeError:
+        except AttributeError as e:
             all_columns = X_dict.columns.append(X.columns)
             duplicates = all_columns[all_columns.duplicated()]
-            raise ValueError(
-                "The ID state could not be attached, because the columns\n"
-                f"{duplicates}\n"
-                f"are also present in the dictionary."
-            )
-
-        return X
-
-    def fit(self, X: TimePredictType, y=None, **fit_params) -> "EDMD":
-        r"""Fit the model.
 
-        Internally calls `fit_transform` of all models contained in the EDMD-dictionary (in
-        given order) and then approximates Koopman operator in the DMD model (final
-        estimator).
-
-        Parameters
-        ----------
-        X
-            Training time series data. Must fulfill input requirements of first
-            `dict_step` in the EDMD-dictionary pipeline.
-
-        y : None
-            ignored
-
-        **fit_params: Dict[str, object]
-            Parameters passed to the ``fit`` method of each step, where
-            each parameter name is prefixed such that parameter ``p`` for step
-            ``s`` has key ``s__p``. To add parameters for the set DMD model use
-            ``s=dmd``, e.g. ``dmd__param``.
+            if len(duplicates) > 0:
+                raise ValueError(
+                    "The ID states could not be attached, because columns\n"
+                    f"{duplicates}\n"
+                    f"are also present in the dictionary mapping."
+                ) from e
+            else:
+                raise e
 
-        Returns
-        -------
-        EDMD
-            self
+        return X
 
-        Raises
-        ------
-        TSCException
-            Time series collection restrictions in `X`: (1) time delta must be constant
-            (2) all time series values must be finite (no `NaN` or `inf`)
-        """
-        self._validate_datafold_data(
-            X,
-            ensure_tsc=True,
-            tsc_kwargs={"ensure_const_delta_time": True},
-        )
+    def _partial_fit(self, X, y=None, **fit_params_steps):
+        # shallow copy of steps - this should really be steps_
+        self.steps = list(self.steps)
+        self._validate_steps()
 
-        self._validate_dictionary()
+        if self.memory is not None:
+            raise ValueError(f"{self.memory=} is not supported for partial fit")
 
-        # NOTE: self._setup_features_and_time_fit(X) is not called here, because the
-        # n_features_in_ and n_feature_names_in_ is delegated to the first instance in
-        # the pipeline. The time values are set separately here:
-        self.time_values_in_ = self._validate_time_values(time_values=X.time_values())
-        self.dt_ = X.delta_time
-        self._feature_names_pred = X.columns
+        for step_idx, name, transformer in self._iter(
+            with_final=False, filter_passthrough=False
+        ):
+            if transformer is None or transformer == "passthrough":
+                with _print_elapsed_time("Pipeline", self._log_message(step_idx)):
+                    continue
+
+            # Fit the current transformer
+            fitted_transformer = transformer.partial_fit(X, y, **fit_params_steps[name])
+            X = transformer.transform(X)
 
-        # '_fit' calls internally fit_transform (!!), and stores results into cache if
-        # "self.memory is not None" (see docu):
-        fit_params = self._check_fit_params(**fit_params or {})
-        dmd_fit_params = fit_params.pop("dmd", None)
-        edmd_fit_params = fit_params.pop("edmd", None)
+            self.steps[step_idx] = (name, fitted_transformer)
+        return X
 
-        X_dict = self._fit(X, y, **fit_params)
+    def _reconstruct(self, X: TSCDataFrame, U: Optional[TSCDataFrame], qois):
+        X_reconstruct = []
 
-        self.n_samples_ic_ = self._compute_n_samples_ic(X, X_dict)
+        if self.dmd_model.is_time_invariant and not X.is_datetime_index():
+            # TODO: support for datetime_index requires implementation.
+            orig_index = X.index.copy(deep=True)
+            X = X.tsc.shift_time_per_time_series(ensure_identical_values=True)
+            normalized_time = True
+        else:
+            normalized_time = False
 
-        if self.include_id_state:
-            X_dict = self._attach_id_state(X=X, X_dict=X_dict)
+        for X_ic, time_values in InitialCondition.iter_reconstruct_ic(
+            X, n_samples_ic=self.n_samples_ic_
+        ):
+            if U is not None:
+                U_select = U.loc[pd.IndexSlice[X_ic.ids, :], :]
+                InitialCondition.validate_control(X_ic, U)
+            else:
+                U_select = None
 
-        with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
-            self._dmd_model.fit(X=X_dict, y=y, **dmd_fit_params)
+            if self.stepwise_transform:
+                X_est_ts = self._predict_stepwise_transform(
+                    X=X_ic, U=U_select, time_values=time_values, qois=qois
+                )
+            else:
+                # transform initial condition to EDMD-dictionary space
+                X_dict_ic = self.transform(X_ic)
+                X_est_ts = self._predict_dict_ic(
+                    X_dict=X_dict_ic, U=U_select, time_values=time_values, qois=qois
+                )
 
-        if not self.use_transform_inverse:
-            self._inverse_map = self._compute_inverse_map(X=X, X_dict=X_dict)
+            X_reconstruct.append(X_est_ts)
 
-            if self.dmd_model.is_spectral_mode():
-                self._koopman_modes = self._compute_koopman_modes(
-                    inverse_map=self._inverse_map,
-                )
+        X_reconstruct = pd.concat(X_reconstruct, axis=0)
 
-                if self.sort_koopman_triplets:
-                    self._sort_koopman_triplets(X_dict_ic=X_dict.initial_states())
+        if normalized_time:
+            # TODO: this can maybe be done better if it becomes in some scenario too
+            #  expensive
+            X.index = orig_index
+
+            if self.n_samples_ic_ > 1:
+
+                def _apply(df):
+                    # drop n instances of index and reset for X_reconstruct
+                    return (
+                        df.index[self.n_samples_ic_ - 1 :]
+                        .to_frame()
+                        .reset_index(drop=True)
+                    )
 
+                recovered_index = X.groupby(TSCDataFrame.tsc_id_idx_name).apply(_apply)
+                recovered_index = pd.MultiIndex.from_frame(recovered_index)
             else:
-                self._koopman_modes = None
-        else:
-            # Indicator to use `ìnverse_transform` of dictionary and not linear map of
-            # Koopman modes.
-            self._inverse_map, self._koopman_modes = None, None
+                recovered_index = orig_index
 
-        return self
+            X_reconstruct = X_reconstruct.set_index(recovered_index)
 
-    def _predict_ic(
-        self, X_dict: TSCDataFrame, time_values, qois, **predict_params
+        # NOTE: time series contained in X_reconstruct can be shorter than
+        # the original time series (i.e. no full reconstruction), because some transform
+        # models drop samples (e.g. time delay embeddings or finite differences)
+        return X_reconstruct
+
+    def _predict_dict_ic(
+        self, X_dict: TSCDataFrame, U, time_values, qois
     ) -> TSCDataFrame:
-        """Prediction with initial condition.
+        """Prediction with initial condition in dictionary states.
 
         Parameters
         ----------
         X_dict
-            The initial condition in EDMD-dictionary space.
+            The initial condition in dictionary space.
+
+        U
+            The control time series (None if not needed)
 
         time_values
             The future time values to evaluate the system at.
 
         qois
             A subselection of quantities of interest (must be in feature_names_pred_).
 
         Returns
         -------
 
         """
-
         if qois is None:
             feature_columns = self.feature_names_pred_
         else:
             feature_columns = qois
 
         if self._inverse_map is not None:
-            if self._koopman_modes is not None:
-                # The DMD model computed spectral components and the
+            if self._koopman_modes is not None and not self.is_controlled_:
+                # NOTE: if the system is controlled, then the Koopman modes are currently not
+                # used for the reconstruction. This is because the linear system form does not
+                # directly reconstruct
+
+                # The spectral components of the DMD model and the
                 # Koopman modes are available.
 
                 if qois is None:
                     modes = self.koopman_modes.to_numpy()
                 else:
-                    project_matrix = projection_matrix_from_features(
+                    project_matrix = projection_matrix_from_feature_names(
                         self.feature_names_pred_, qois
                     )
                     modes = project_matrix.T @ self._koopman_modes
 
                 # compute the time series in original space directly by adapting the modes
-                X_ts = self._dmd_model.predict(
-                    X_dict,
+
+                dmd_params = dict(
+                    U=U,
                     time_values=time_values,
-                    **{"modes": modes, "feature_columns": feature_columns},
+                    modes=modes,
+                    feature_columns=feature_columns,
                 )
+                dmd_params = {k: v for k, v in dmd_params.items() if v is not None}
+
+                X_ts = self.dmd_model.predict(X_dict, **dmd_params)
             else:
                 # The DMD model does not provide the spectral components of the
                 # Koopman matrix. The inverse_map needs to be applied afterwards because
                 # the DMD model requires to maintain a square matrix to forward the
                 # system.
 
                 # computes system in EDMD-dictionary space
-                X_ts = self._dmd_model.predict(
-                    X_dict,
-                    time_values=time_values,
-                )
+                dmd_params = dict(U=U, time_values=time_values)
+                dmd_params = {k: v for k, v in dmd_params.items() if v is not None}
+
+                X_ts = self.dmd_model.predict(X_dict, **dmd_params)
 
                 # map back to original space and select qois
+                if hasattr(self, "_inverse_map_control"):
+                    vals = (X_ts.to_numpy() @ self._inverse_map)[
+                        :-1, :
+                    ] + U.to_numpy() @ self._inverse_map_control
+                    idx = X_ts.index[:-1]
+                else:
+                    vals = X_ts.to_numpy() @ self._inverse_map
+                    idx = X_ts.index
+
                 X_ts = TSCDataFrame(
-                    X_ts.to_numpy() @ self._inverse_map,
+                    vals,
                     columns=self.feature_names_pred_,
-                    index=X_ts.index,
+                    index=idx,
                 ).loc[:, feature_columns]
 
         else:
             # predict all EDMD-dictionary time series
-            X_ts = self._dmd_model.predict(X_dict, time_values=time_values)
+            X_ts = self.dmd_model.predict(X_dict, time_values=time_values)
 
             # transform from EDMD-dictionary space by pipeline inverse_transform
             X_ts = self.inverse_transform(X_ts)
             X_ts = X_ts.loc[:, feature_columns]
 
         return X_ts
 
+    def _predict_stepwise_transform(self, X: TSCDataFrame, U, time_values, qois):
+        if self.is_state_transition_map_ and not self.id_state_in_transition_map_:
+            raise ValueError(
+                "It is not possible tp perform stepwise transform predictions with "
+                "state transition map that does not include the original full-state."
+            )
+        elif self.is_state_transition_map_:
+            raise NotImplementedError(
+                "stepwise transform with state transition map is not implemented yet"
+            )
+            extract_id_columns = self.feature_names_in_
+        else:
+            extract_id_columns = None
+
+        X = X.tsc.expand_time_values(time_values=time_values[1:])
+        all_time_values = X.time_values()
+
+        for i in range(self.n_samples_ic_, len(time_values) + self.n_samples_ic_ - 1):
+            current_ic_time = all_time_values[i - self.n_samples_ic_ : i]
+            assert current_ic_time[-1] == time_values[i - self.n_samples_ic_]
+            _X_current = X.loc[
+                pd.IndexSlice[:, current_ic_time], slice(extract_id_columns)
+            ]
+
+            if U is not None:
+                _U_current = U.loc[pd.IndexSlice[:, current_ic_time], :]
+            else:
+                _U_current = None
+
+            _X_dict = self.transform(_X_current)
+            _X_predict = self._predict_dict_ic(
+                _X_dict,
+                U=_U_current,
+                time_values=all_time_values[i - 1 : i + 1],
+                qois=None,
+            )
+            assert _X_predict.n_timesteps == 2
+
+            _X_predict = _X_predict.final_states()
+
+            # fill in the new state
+            X.loc[_X_predict.index] = _X_predict
+
+        if qois is not None:
+            X = X.loc[:, qois]
+
+        if self.n_samples_ic_ > 1:
+            X = X.loc[pd.IndexSlice[:, time_values], :]
+
+        return X
+
+    def fit(
+        self,
+        X: TimePredictType,
+        *,
+        U: Optional[TimePredictType] = None,
+        P: Optional[pd.DataFrame] = None,
+        y: Optional[TSCDataFrame] = None,
+        **fit_params,
+    ) -> "EDMD":
+        r"""Fit the model.
+
+        Internally the method calls `fit_transform` of all models contained in the
+        EDMD dictionary (in given order) and then approximates the Koopman operator in the
+        DMD model as the final estimator of the pipeline. Finally, the inverse map from
+        dictionary states to the original states is set up.
+
+
+        Parameters
+        ----------
+        X
+            Training time series data. Must fulfill input requirements of first
+            `dict_step` in the EDMD-dictionary pipeline.
+
+        U
+            Time series with control states acting on the system. The states are passed to the
+            DMD model, at which point the time indices must be identical to the states in `X`.
+
+        P
+            ignored -- reservered for parameters
+
+        y
+            A different set of target values than the original states to map to with
+            Koopman modes. **This is an experimental feature.**
+
+        **fit_params: Dict[str, object]
+            Parameters passed to the ``fit`` method of each step, where
+            each parameter name is prefixed such that parameter ``p`` for step
+            ``s`` has key ``s__p``. To add parameters for the internal DMD model use
+            ``s=dmd``, e.g. ``dmd__param``.
+
+        Returns
+        -------
+        EDMD
+            self
+
+        Raises
+        ------
+        TSCException
+            Time series collection restrictions in `X`: (1) time delta must be constant
+            (2) all time series values must be finite (no `NaN` or `inf`)
+        """
+        # Currently, validation of U is only performed in the final DMD estimator
+        self._validate_datafold_data(
+            X,
+            ensure_tsc=True,
+            tsc_kwargs=dict(ensure_const_delta_time=True),
+        )
+
+        if y is not None:
+            # TODO: perform validation
+            self.is_state_transition_map_ = True
+            warnings.warn(
+                "Currently there is no validation on y input. Implementation requires.",
+                stacklevel=1,
+            )
+        else:
+            self.is_state_transition_map_ = False
+            self.id_state_in_transition_map_ = False
+
+        if hasattr(self, "is_partial_fit_") and self.is_partial_fit_:
+            raise ValueError(
+                "The method fit() cannot be called if the model was set up with "
+                f" {self.is_partial_fit_=}. Use partial_fit() instead."
+            )
+        else:
+            self.is_partial_fit_ = False
+
+        self.is_controlled_ = U is not None
+        self.is_dict_learning_ = isinstance(self.dmd_model, DMDDictLearning)
+
+        # 1) first get the EDMD fit_params, 2) validate the fit_params for the pipeline,
+        # 2) separate the DMD fit_params as the dmd is called later
+        # TODO: include validation of disallowed keys in fit_params (edmd, dl_transform(?))
+        fit_params = self._check_fit_params(**fit_params or {})
+        # separated from the dictionary and passed to the DMD as final estimator below
+        dmd_fit_params = fit_params.pop("dmd", None)
+
+        self._validate_dictionary()
+
+        # NOTE: self._setup_features_and_time_fit(X) is not called here, because the
+        # n_features_in_ and n_feature_names_in_ is delegated to the first instance in
+        # the pipeline. The time values are set separately here:
+        self._validate_time_values_format(time_values=X.time_values())
+        self.dt_ = X.delta_time
+
+        if y is None:
+            self._feature_names_pred = X.columns
+        else:
+            self._feature_names_pred = y.columns
+
+        # '_fit' calls internally fit_transform (!), and stores results into cache if
+        # "self.memory is not None" (see docu):
+        X_dict = self._fit(X, y, **fit_params)
+        self.n_samples_ic_ = self._compute_n_samples_ic(X, X_dict)
+
+        # Either automatically detected or enforced in dict_preserves_id_states
+        self.dict_preserves_id_state_ = self._set_dict_preserves_id_state(X_dict)
+
+        if self.is_state_transition_map_:
+            # Check if the original state is contained in the transition map (some
+            # features, such as stepwise_prediction, require the original state in a
+            # prediction to forward in time.
+            assert y is not None  # mypy
+            self.id_state_in_transition_map_ = np.isin(
+                self.feature_names_in_, y.columns
+            ).all()
+
+        if self.include_id_state and not self.dict_preserves_id_state_:
+            # only attach original states if they are not preserved
+            X_dict = self._attach_id_state(X=X, X_dict=X_dict)
+
+        if self.is_controlled_ and self.n_samples_ic_ > 1:
+            # align index of control input with intersection of indices
+            # Some keys may be dropped here (e.g. when using time delay embedding)
+            assert U is not None  # for mypy typing
+            inters_keys = X_dict.index.intersection(U.index)
+            U = U.loc[inters_keys, :]  # type: ignore
+
+        with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
+            if self.is_controlled_:
+                self.dmd_model.fit(X=X_dict, U=U, y=y, **dmd_fit_params)
+            else:
+                self.dmd_model.fit(X=X_dict, y=y, **dmd_fit_params)
+
+        if self.is_dict_learning_:
+            # apply final transformation based on trained dictionary
+            X_dict = self.dmd_model.learning_model.transform(X_dict)
+
+            # apply final dictionary transformation, adapt dictionary pipeline and
+            # reset the identified DMD model
+            self.steps = self.steps[:-1] + [
+                ("dict_learning", self.dmd_model.learning_model),
+                ("dmd", self.dmd_model.dmd_model),
+            ]
+
+        if not self.use_transform_inverse:
+            self._inverse_map = self._compute_inverse_map(X=X, y=y, X_dict=X_dict, U=U)
+
+            if self.dmd_model.is_spectral_mode:
+                self._koopman_modes = self._compute_koopman_modes(
+                    inverse_map=self._inverse_map,
+                )
+
+                if self.sort_koopman_triplets:
+                    self._sort_koopman_triplets(X_dict_ic=X_dict.initial_states())
+
+            else:
+                self._koopman_modes = None
+        else:
+            # Indicator to use `ìnverse_transform` of dictionary and not linear map of
+            # Koopman modes.
+            self._inverse_map, self._koopman_modes = None, None
+
+        return self
+
     def predict(
         self,
         X: InitialConditionType,
+        *,
+        U: Optional[InitialConditionType] = None,
+        P: Optional[pd.DataFrame] = None,
         time_values: Optional[np.ndarray] = None,
-        qois: Optional[Union[pd.Index, List[str]]] = None,
+        qois: Optional[Union[pd.Index, list[str]]] = None,
         **predict_params,
     ):
         """Evaluate dynamical system for one or many initial conditions.
 
         The internal prediction steps are:
 
         1. Transform initial conditions to EDMD-dictionary states.
@@ -775,25 +1105,37 @@
         Parameters
         ----------
         X: TSCDataFrame, numpy.ndarray
             The initial conditions, where initial condition must have exactly
             ``n_samples_ic_`` samples (mapped to a single EDMD-dictionary state). The
             preferred input type is :py:class:`TSCDataFrame`. If only a single state
             is required (``n_samples_ic_ = 1``), then a :class:`numpy.ndarray` is also
-            accepted, where each row corresponds to an initial condition. Must fulfill
-            the input requirements of first step of the pipeline.
+            accepted, where each row corresponds to an initial condition.
+
+        U
+            If the model was fit with control input, then this argument is required.
+            For each initial condition in `X` there must be a corresponding time series with
+            the control states over the prediction horizon in `U`. Each time series in `U`
+            must have the same time values. The time horizon is taken from `U` (i.e.
+            ``time_values`` has to be either identical or ``None``).
+
+        P
+            ignored -- reserved for parameters
 
         time_values
-            The time values to evaluate the model for each initial condition.
-            Defaults to time values contained in the data available during ``fit``. The
-            values should be ascending, non-negative numeric values.
+            The time values to evaluate the model at for each initial condition. The values
+            should be ascending and non-negative numeric values. Default parameter
+
+            * uncontrolled system: time series of lengths two, where the first state is the
+              initial condition and the second state the evaluation after `self.dt_`
+            * controlled system: the time values are taken from the parameter ``U``.
 
         qois
             A list of feature names of interest to be included in the returned
-            predictions. Must be a subset of ``feature_names_pred_``.
+            predictions. Must be a subset of names in attribute ``feature_names_pred_``.
 
         **predict_params: Dict[str, object]
             ignored
 
         Returns
         -------
         TSCDataFrame
@@ -805,76 +1147,351 @@
         TSCException
             Time series collection requirements in `X`: (1) same (constant) time delta as
             during fit (2) all time series must have identical
             time values (3) all values must be finite (i.e. no `NaN` or `inf` values).
         """
         check_is_fitted(self)
 
+        time_values = self._validate_and_set_time_values_predict(
+            time_values=time_values, X=X, U=U
+        )
+
         if isinstance(X, np.ndarray):
-            # work internally only with TSCDataFrame
-            X = InitialCondition.from_array(X, columns=self.feature_names_in_)
+            # internally only work with TSCDataFrame
+            X = InitialCondition.from_array(
+                if1dim_rowvec(X),
+                time_value=time_values[0],
+                feature_names=self.feature_names_in_,
+                ts_ids=U.ids if isinstance(U, TSCDataFrame) else None,
+            )
         else:
             InitialCondition.validate(
                 X,
                 n_samples_ic=self.n_samples_ic_,
                 dt=self.dt_ if self.n_samples_ic_ > 1 else None,
             )
 
-        if time_values is None:
-            # If samples were dropped during fit, then for the first
-            # self.n_samples_ic_ - 1 there was is evaluation.
-            # Because this is different from the behaviour in
-            # '_validate_features_and_time_values' this is done separately here.
-            time_values = self.time_values_in_[self.n_samples_ic_ - 1 :]
+        if self.is_controlled_:
+            if isinstance(U, np.ndarray):
+                if X.n_timeseries > 1:
+                    raise NotImplementedError(
+                        "If U is of type np.ndarray, then only prediction for "
+                        "a single initial condition is allowed."
+                        f"Got {X.n_timeseries}"
+                    )
+
+                U = InitialCondition.from_array_control(
+                    U,
+                    control_names=self.control_names_in_,
+                    dt=self.dt_,
+                    time_values=time_values[:-1],
+                    ts_id=int(X.ids[0]) if isinstance(X, TSCDataFrame) else None,
+                )
+            elif isinstance(U, TSCDataFrame):
+                InitialCondition.validate_control(X_ic=X, U=U)
+            else:
+                raise TypeError(f"U has invalid type (got {type(U)}.")
 
-        X, time_values = self._validate_features_and_time_values(
-            X=X, time_values=time_values
-        )
+        self._validate_feature_names(X, U)
 
         qois = self._validate_qois(
             qois=qois, valid_feature_names=self._feature_names_pred
         )
 
+        self._validate_datafold_data(X, ensure_tsc=True)
+
+        if self.stepwise_transform:
+            X_ts = self._predict_stepwise_transform(
+                X=X, U=U, time_values=time_values, qois=qois
+            )
+        else:
+            X_dict = self.transform(X)
+            X_ts = self._predict_dict_ic(
+                X_dict=X_dict, U=U, time_values=time_values, qois=qois
+            )
+        return X_ts
+
+    def fit_predict(
+        self,
+        X: TSCDataFrame,
+        *,
+        U: Optional[TSCDataFrame] = None,
+        P: Optional[pd.DataFrame] = None,
+        y=None,
+        qois: Optional[Union[pd.Index, list[str]]] = None,
+        **fit_params,
+    ):
+        """Fit the model and reconstruct the training data.
+
+        Parameters
+        ----------
+        X
+            Training time series data. Must fulfill input requirements of first
+            `dict_step` in the EDMD-dictionary pipeline.
+
+        U
+            Control time series passed to the DMD model. At this point the index of `U` must
+            be identical to `X_dict`.
+        P
+            ignored -- reserved for parameters
+
+        y
+            TODO: update docs
+
+        qois
+            A list of feature names of interest to be included in the returned
+            predictions. Must be a subset of ``feature_names_pred_``. Passed to
+            :py:meth:`.predict`.
+
+        **fit_params: Dict[str, object]
+            Parameters passed to the ``fit`` method of each step, where
+            each parameter name is prefixed such that parameter ``p`` for step
+            ``s`` has key ``s__p``.
+
+        Returns
+        -------
+        TSCDataFrame
+            Reconstructed time series collection. If `n_samples_ic_ > 1` the number
+            of samples for each time series decreases accordingly.
+
+        Raises
+        ------
+        TSCException
+            Time series collection restrictions in **X**: (1) time delta must be constant
+            (2) all values must be finite (no `NaN` or `inf`)
+        """
+        return self.fit(X=X, U=U, y=y, **fit_params).reconstruct(X=X, U=U, qois=qois)
+
+    def __getitem__(self, ind):
+        # Overwrite the super class to distinguish the
+        if isinstance(ind, slice):
+            if ind.step not in (1, None):
+                raise ValueError("Pipeline slicing only supports a step of 1")
+
+            steps = self.steps[ind]
+
+            if len(steps) == len(self.steps):
+                return self
+            elif isinstance(steps[-1][1], TSCPredictMixin):
+                # actually it is possible to return EDMD if the DMD is included in the slice,
+                # however, then we must copy all EDMD specific attributes (also ones set
+                # during fit). This can be implemented when needed.
+                raise ValueError(
+                    "Can only slice transformers of the pipeline and not the "
+                    "final DMD estimator model"
+                )
+            else:
+                return Pipeline(steps=steps, memory=self.memory, verbose=self.verbose)
+        else:
+            return super().__getitem__(ind)
+
+    def partial_fit(
+        self,
+        X: TimePredictType,
+        *,
+        U: Optional[Union[np.ndarray, TSCDataFrame]] = None,
+        P: Optional[pd.DataFrame] = None,
+        y=None,
+        **fit_params,
+    ) -> "EDMD":
+        """Incremental fit of the model.
+
+        The partial fit call is forwarded to all transformers in the dictionary and the set
+        DMD model. The update fails if one model does not support incremental updates.
+
+        Parameters
+        ----------
+        X
+            The new batch of training time series.
+
+        U
+            Currently, there is no implementation that supports both an online/streaming
+            setting with control.
+
+        P
+            ignored -- reserved for parameters
+
+        y
+            ignored
+
+        fit_params
+            Parameters passed to the ``fit`` method of each step, where
+            each parameter name is prefixed such that parameter ``p`` for step
+            ``s`` has key ``s__p``. To add parameters for the set DMD model use
+            ``s=dmd``, e.g. ``dmd__param``.
+
+        Returns
+        -------
+        self
+            updated model
+        """
         self._validate_datafold_data(
             X,
             ensure_tsc=True,
+            tsc_kwargs=dict(ensure_const_delta_time=True),
         )
 
-        X_dict = self.transform(X)
-        X_ts = self._predict_ic(X_dict=X_dict, time_values=time_values, qois=qois)
+        if y is not None:
+            raise NotImplementedError(
+                "The y parameter is currently not supported for partial_fit "
+                "(but should require only little implementation effort)."
+            )
+        if U is not None:
+            raise NotImplementedError(
+                "Currently there are no DMD models that that support both streaming "
+                "and control."
+            )
 
-        return X_ts
+        self.is_controlled_ = False
 
-    def _reconstruct(self, X: TSCDataFrame, qois):
+        try:
+            check_is_fitted(self)
+            initial_fit = False
+            assert self.is_partial_fit_
+        except NotFittedError:
+            initial_fit = True
 
-        X_reconstruct = []
-        for X_ic, time_values in InitialCondition.iter_reconstruct_ic(
-            X, n_samples_ic=self.n_samples_ic_
-        ):
-            # transform initial condition to EDMD-dictionary space
-            X_dict_ic = self.transform(X_ic)
+            if hasattr(self, "is_partial_fit_") and not self.is_partial_fit_:
+                raise ValueError(
+                    "The model is already set up with the 'fit' method. "
+                    "Use `partial_fit` for both the initial and partial fits."
+                )
+            else:
+                self.is_partial_fit_ = True
+            self.dt_ = X.delta_time
+            self._feature_names_pred = X.columns
 
-            X_est_ts = self._predict_ic(
-                X_dict=X_dict_ic, time_values=time_values, qois=qois
+        # '_fit' calls internally fit_transform (!!), and stores results into cache if
+        # "self.memory is not None" (see docu):
+        fit_params = self._check_fit_params(**fit_params or {})
+        dmd_fit_params = fit_params.pop("dmd", None)
+
+        X_dict = self._partial_fit(X, y, **fit_params)
+
+        if initial_fit:
+            self.dict_preserves_id_state_ = self._validate_dictionary()
+
+        if initial_fit:
+            self.n_samples_ic_ = self._compute_n_samples_ic(X, X_dict)
+
+        if self.include_id_state and not self.dict_preserves_id_state_:
+            X_dict = self._attach_id_state(X=X, X_dict=X_dict)
+        elif not self.include_id_state and not not self.dict_preserves_id_state_:
+            raise NotImplementedError(
+                "Currently, there is no implementation to partial_fit non-trivial update of "
+                "the modes. Either the dictionary must preserve the id states or "
+                "`include_is_state=True`."
             )
 
-            X_reconstruct.append(X_est_ts)
+        with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
+            self.dmd_model.partial_fit(X=X_dict, y=y, **dmd_fit_params)
 
-        X_reconstruct = pd.concat(X_reconstruct, axis=0)
-        assert isinstance(X_reconstruct, TSCDataFrame)
+        if (
+            not self.use_transform_inverse
+        ):  # TODO: avoid duplicated code with fit() here!
+            if not self.use_transform_inverse:
+                self._inverse_map = self._compute_inverse_map(
+                    X=X, X_dict=X_dict, y=None, U=U
+                )
 
-        # NOTE: time series contained in X_reconstruct can be shorter in length than
-        # the original time series (i.e. no full reconstruction), because some transform
-        # models drop samples (e.g. time delay embeddings or finite differences)
-        return X_reconstruct
+            if self.dmd_model.is_spectral_mode:
+                self._koopman_modes = self._compute_koopman_modes(
+                    inverse_map=self._inverse_map,
+                )
+
+                if self.sort_koopman_triplets:
+                    self._sort_koopman_triplets(X_dict_ic=X_dict.initial_states())
+
+            else:
+                self._koopman_modes = None
+        else:
+            # Indicator to use `ìnverse_transform` of dictionary and not linear map of
+            # Koopman modes.
+            self._inverse_map, self._koopman_modes = None, None
+
+        return self
+
+    def transform(self, X: TransformType) -> TransformType:
+        """Map the original states to the dictionary representation.
+
+        Parameters
+        ----------
+        X : TSCDataFrame, pandas.DataFrame
+           Time series to transform. Must fulfill the input requirements of
+           first step of the pipeline. Each time series must have a minimum of
+           ``n_samples_ic_`` samples.
+
+        Returns
+        -------
+        TSCDataFrame, pandas.DataFrame
+            The transformed time series. The number of samples of each time series are reduced
+            if `n_samples_ic_ > 1`.
+        """
+        if isinstance(X, np.ndarray):
+            X = TSCDataFrame.from_array(
+                X,
+                feature_names=self.feature_names_in_,
+                time_values=np.arange(0, self.dt_ * X.shape[0], self.dt_),
+            )
+
+        if self.include_id_state:
+            # copy required to properly attach X later on
+            X_dict = X.copy(deep=True)
+        else:
+            X_dict = X
+
+        # carry out dictionary transformations:
+        for _, _, tsc_transform in self._iter(with_final=False):
+            X_dict = tsc_transform.transform(X_dict)
+
+        if self.include_id_state and not self.dict_preserves_id_state_:
+            X_dict = self._attach_id_state(X=X, X_dict=X_dict)
+
+        return X_dict
+
+    def fit_transform(  # type: ignore[override]
+        self, X: TSCDataFrame, *, U: Optional[TSCDataFrame] = None, y=None, **fit_params
+    ):
+        """Fit the model and return the EDMD dictionary time series.
+
+        Parameters
+        ----------
+        X
+            Time series collection data to fit the model.
+
+        U
+            Control time series passed to :py:meth:`.fit`.
+
+        y: None
+            ignored
+
+        **fit_params: Dict[str, object]
+            Parameters passed to the ``fit`` method of each step, where
+            each parameter name is prefixed such that parameter ``p`` for step
+            ``s`` has key ``s__p``.
+
+        Returns
+        -------
+        TSCDataFrame
+             EDMD-dictionary time series data.
+
+        Raises
+        ------
+        TSCException
+            Time series collection restrictions in `X`: (1) time delta must be constant
+            (2) all values must be finite (no `NaN` or `inf`)
+        """
+        return self.fit(X=X, U=U, y=y, **fit_params).transform(X)
 
     def reconstruct(
         self,
         X: TSCDataFrame,
-        qois: Optional[Union[pd.Index, List[str]]] = None,
+        *,
+        U: Optional[TSCDataFrame] = None,
+        qois: Optional[Union[pd.Index, list[str]]] = None,
     ) -> TSCDataFrame:
         """Reconstruct existing time series collection.
 
         Internal steps to reconstruct a time series collection:
 
         1. Extract the initial conditions (first ``n_samples_ic_`` samples) from each
            time series in the collection.
@@ -883,117 +1500,93 @@
 
         Parameters
         ----------
         X
             The time series collection to reconstruct. The first ``n_samples_ic_`` of
             each time series must fulfill the requirements of an initial condition.
 
+        U
+            Control time series for the data. Only required if model was fit with control.
+
         qois
             A list of feature names of interest to be include in the returned
             predictions. Passed to :py:meth:`.predict`.
 
         Returns
         -------
         TSCDataFrame
             Reconstructed time series collection. If `n_samples_ic_ > 1` the number
             of samples for each time series decrease accordingly.
 
         Raises
         ------
         TSCException
-            Time series collection requirements in `X`: (1) all values must be
-            finite (no `NaN` or `inf`)
+            Time series collection requirements in ``X``:
+            * all values must be finite (no `NaN` or ``inf``)
+            * every time series must have at least ``n_samples_ic_`` samples
+              (make sure that these first samples have constant delta time, this is currently
+              not validated)
+
         """
         check_is_fitted(self)
 
         X = self._validate_datafold_data(
             X,
             ensure_tsc=True,
+            #
+            tsc_kwargs={"ensure_min_timesteps": self.n_samples_ic_ + 1}
             # Note: no const_delta_time required here. The required const samples for
             # time series initial conditions is included in the predict method.
         )
-        self._validate_feature_names(X)
+        self._validate_feature_names(X=X, U=U)
         self._validate_qois(qois=qois, valid_feature_names=self.feature_names_pred_)
 
-        return self._reconstruct(X=X, qois=qois)
+        return self._reconstruct(X=X, U=U, qois=qois)
 
-    def fit_predict(
-        self,
-        X: TSCDataFrame,
-        y=None,
-        qois: Optional[Union[pd.Index, List[str]]] = None,
-        **fit_params,
-    ):
-        """Fit the model and reconstruct the training data.
+    def inverse_transform(self, X: TransformType) -> TransformType:
+        """Perform inverse dictionary transformations on dictionary time series.
+
+        The actual performed inverse transformation depends on the parameter settings
+        ``include_id_state`` and ``use_transform_inverse``.
 
         Parameters
         ----------
-        X
-            Training time series data. Must fulfill input requirements of first
-            `dict_step` in the EDMD-dictionary pipeline.
-
-        y: None
-            ignored
-
-        qois
-            A list of feature names of interest to be included in the returned
-            predictions. Must be a subset of ``feature_names_pred_``. Passed to
-            :py:meth:`.predict`.
-
-        **fit_params: Dict[str, object]
-            Parameters passed to the ``fit`` method of each step, where
-            each parameter name is prefixed such that parameter ``p`` for step
-            ``s`` has key ``s__p``.
+        X: TSCDataFrame, pandas.DataFrame
+            Time series to map back to the full-state time series. The feature names
+            must match the ones in attribute ``feature_names_out_``.
 
         Returns
         -------
         TSCDataFrame
-            Reconstructed time series collection. If `n_samples_ic_ > 1` the number
-            of samples for each time series decreases accordingly.
-
-        Raises
-        ------
-        TSCException
-            Time series collection restrictions in **X**: (1) time delta must be constant
-            (2) all values must be finite (no `NaN` or `inf`)
+            full-state time series
         """
-        return self.fit(X=X, y=y, **fit_params).reconstruct(X=X, qois=qois)
-
-    def fit_transform(self, X: TSCDataFrame, y=None, **fit_params):
-        """Fit the model and return the EDMD-dictionary time series.
-
-        Parameters
-        ----------
-        X
-            Time series collection data to fit the model.
-
-        y: None
-            ignored
+        if self._inverse_map is not None:
+            # Note, here the samples are row-wise
+            values = X.to_numpy() @ self._inverse_map
 
-        **fit_params: Dict[str, object]
-            Parameters passed to the ``fit`` method of each step, where
-            each parameter name is prefixed such that parameter ``p`` for step
-            ``s`` has key ``s__p``.
+            X_ts = df_type_and_indices_from(
+                indices_from=X, values=values, except_columns=self.feature_names_in_
+            )
 
-        Returns
-        -------
-        TSCDataFrame
-             EDMD-dictionary time series data.
+        else:
+            # inverse_transform the pipeline because an inverse linear map is not
+            # available.
+            X_ts = X
+            reverse_iter = reversed(list(self._iter(with_final=False)))
+            for _, _, tsc_transform in reverse_iter:
+                X_ts = tsc_transform.inverse_transform(X_ts)
 
-        Raises
-        ------
-        TSCException
-            Time series collection restrictions in `X`: (1) time delta must be constant
-            (2) all values must be finite (no `NaN` or `inf`)
-        """
-        # NOTE: could be improved, but this function is probably not required very often.
-        return self.fit(X=X, y=y, **fit_params).transform(X)
+        return X_ts
 
     def score(
-        self, X: TSCDataFrame, y=None, sample_weight: Optional[np.ndarray] = None
+        self,
+        X: TSCDataFrame,
+        U=None,
+        y=None,
+        sample_weight: Optional[np.ndarray] = None,
     ):
         """Score between given time series and its model reconstruction.
 
         Parameters
         ----------
         X
             The time series collection to reconstruct. The first ``n_samples_ic_`` of
@@ -1013,20 +1606,19 @@
 
         Raises
         ------
         TSCException
             Time series collection restrictions in `X`: (1) time delta must be constant
             (2) all values must be finite (no `NaN` or `inf`)
         """
-
         assert y is None
         self._check_attributes_set_up(check_attributes=["_score_eval"])
 
         # does all the checks:
-        X_reconstruct = self.reconstruct(X)
+        X_reconstruct = self.reconstruct(X=X, U=U)
 
         if self.n_samples_ic_ > 1:
             # Note that during `reconstruct` samples can be discarded (e.g. when
             # applying time delay embedding). In the latent space there are then less
             # samples than in the full-state, which is corrected here:
             X = X.loc[X_reconstruct.index, :]
 
@@ -1074,15 +1666,15 @@
         )
 
     progress_msg = ""
     if verbose > 2:
         if split_progress is not None:
             progress_msg = f" {split_progress[0] + 1}/{split_progress[1]}"
         if candidate_progress and verbose > 9:
-            progress_msg += f"; {candidate_progress[0] + 1}/" f"{candidate_progress[1]}"
+            progress_msg += f"; {candidate_progress[0] + 1}/ {candidate_progress[1]}"
 
     if verbose > 1:
         if parameters is None:
             params_msg = ""
         else:
             sorted_keys = sorted(parameters)  # Ensure deterministic o/p
             params_msg = ", ".join(f"{k}={parameters[k]}" for k in sorted_keys)
@@ -1106,15 +1698,15 @@
     # NOTE: this deviates from the _fit_and_score in sklearn, which uses a
     #  _safe_split function (defined in metaestimators.py)
     X_train, X_test = _split_X_edmd(X, y, train_indices=train, test_indices=test)
 
     result = {}
     try:
         edmd.fit(X_train, y=None, **fit_params)
-    except Exception as e:
+    except Exception:
         # Handle all exception, to not waste other working or complete results
         fit_time = time.time() - start_time  # Note fit time as time until error
         score_time = 0.0
         if error_score == "raise":
             raise
         elif isinstance(error_score, numbers.Number):
             # Note fit time as time until error
@@ -1128,33 +1720,33 @@
                     train_scores = error_score
 
                 warnings.warn(
                     "Estimator fit failed. The score on this train-test"
                     f" partition for these parameters will be set to {error_score}. "
                     "Details: \n%s" % (format_exc()),
                     FitFailedWarning,
+                    stacklevel=2,
                 )
             result["fit_failed"] = True
     else:
         result["fit_failed"] = False
 
         fit_time = time.time() - start_time
         test_scores = _score(edmd, X_test, None, scorer, error_score)
         score_time = time.time() - start_time - fit_time
 
         if return_train_score:
             train_scores = _score(edmd, X_train, None, scorer, error_score)
 
     if verbose > 1:
-
         sorted_keys = sorted(parameters)  # Ensure deterministic o/p
         params_msg = ", ".join(f"{k}={parameters[k]}" for k in sorted_keys)
 
         total_time = score_time + fit_time
-        end_msg = f"[CV] END "
+        end_msg = "[CV] END "
         result_msg = params_msg + (";" if params_msg else "")
         result_msg += f" total time={logger.short_format_time(total_time)}"
 
         # Right align the result_msg
         end_msg += "." * (80 - len(end_msg) - len(result_msg))
         end_msg += result_msg
         print(end_msg)
@@ -1251,15 +1843,14 @@
         parameter settings impact the overfitting/underfitting trade-off.
         However computing the scores on the training set can be computationally
         expensive and is not strictly required to select the parameters that
         yield the best generalization performance.
 
     Attributes
     ----------
-
     cv_results_ : dict of numpy (masked) ndarrays
         A dict with keys as column headers and values as columns, that can be
         imported into a ``pandas.DataFrame``. See documentation in super class.
 
     best_estimator_ : estimator
         Estimator that was chosen by the search, i.e. estimator
         which gave highest score (or smallest loss if specified)
@@ -1296,15 +1887,14 @@
 
     refit_time_ : float
         Seconds used for refitting the best model on the whole dataset.
         This is present only if ``refit`` is True.
 
     Notes
     -----
-
     The parameters selected are those that maximize the score of the left out
     data. If `n_jobs` was set to a value higher than one, the data is copied for each
     point in the grid (and not `n_jobs` times). This is done for efficiency
     reasons if individual jobs take very little time, but may raise errors if
     the dataset is large and not enough memory is available.  A workaround in
     this case is to set `pre_dispatch`. Then, the memory is copied only
     `pre_dispatch` many times. A reasonable value for `pre_dispatch` is `2 *
@@ -1312,25 +1902,24 @@
 
     """
 
     def __init__(
         self,
         estimator: EDMD,
         *,
-        param_grid: Union[Dict, List[Dict]],
+        param_grid: Union[dict, list[dict]],
         cv: TSCCrossValidationSplit,
         n_jobs: Optional[int] = None,
         pre_dispatch: Union[int, str] = "2*n_jobs",
         refit: bool = True,
         verbose: int = 1,
         error_score: Union[str, numbers.Number] = "raise",
         return_train_score: bool = True,
     ):
-
-        super(EDMDCV, self).__init__(
+        super().__init__(
             estimator=estimator,
             param_grid=param_grid,
             scoring=None,
             n_jobs=n_jobs,
             cv=cv,
             refit=refit,
             verbose=verbose,
@@ -1347,15 +1936,14 @@
             raise TypeError(f"cv must be of type {(TSCKfoldSeries, TSCKFoldTime)}")
 
     def fit(self, X: TSCDataFrame, y=None, **fit_params):
         """Fit and score the model for all parameter candidates.
 
         Parameters
         ----------
-
         X
             Training time series data.
 
         y: None
             ignored
 
         **fit_params : Dict[str, object]
@@ -1386,33 +1974,29 @@
             return_n_test_samples=True,
             return_times=True,
             return_parameters=False,
             error_score=self.error_score,
             verbose=self.verbose,
         )
 
-        results: Dict[str, Any] = {}
+        results: dict[str, Any] = {}
         with parallel:
-
-            all_candidate_params: List[List[Dict[str, Any]]] = []
-            all_out: List[Any] = []
+            all_candidate_params: list[list[dict[str, Any]]] = []
+            all_out: list[Any] = []
             all_more_results = defaultdict(list)
 
             def evaluate_candidates(candidate_params, cv=None, more_results=None):
-
                 cv = cv or cv_orig
                 candidate_params = list(candidate_params)
                 n_candidates = len(candidate_params)
 
                 if self.verbose > 0:
                     print(
-                        "Fitting {0} folds for each of {1} candidates,"
-                        " totalling {2} fits".format(
-                            n_splits, n_candidates, n_candidates * n_splits
-                        )
+                        f"Fitting {n_splits} folds for each of {n_candidates} candidates,"
+                        f" totalling {n_candidates * n_splits} fits."
                     )
 
                 out = parallel(
                     delayed(_fit_and_score_edmd)(
                         clone(base_estimator),
                         X,
                         y,
@@ -1486,65 +2070,67 @@
 
         self.cv_results_ = results
         self.n_splits_ = n_splits
 
         return self
 
 
-class EDMDWindowPrediction(object):
+class EDMDWindowPrediction:
     """Adapt EDMD model to perform reconstruct and score time series of same length.
 
     The adaptation of the EDMD model is useful if a fixed prediction horizon is
     tested. Instead of the default behaviour of EDMD to reconstruct the full time series
     found in a :py:class`.TSCDataFrame`, time series of equal length are extracted from
     the data and then reconstructed.
 
     Parameters
     ----------
-
     window_size
         An integer value indicating the time steps to include in a window. The value
-        must be greater than the the attribute ``edmd.n_samples_ic_``, because a
+        must be greater than the attribute ``edmd.n_samples_ic_``, because a
         window also contains the samples dedicated for the initial condition.
 
     offset
         An integer value to indicate the offset between two windows. When setting
         `offset=window_size-edmd.n_samples_ic_`, then the test samples do not overlap
         between windows and samples are not dropped.
 
     """
 
     def __init__(self, window_size: int = 10, offset: int = 10):
         self.window_size = window_size
         self.offset = offset
 
     def _validate(self):
-
         if self.window_size is not None and self.offset is not None:
             check_scalar(
                 self.window_size,
                 name="time_horizon",
                 target_type=(np.integer, int),
                 min_val=1,
             )
 
             check_scalar(
                 self.offset, name="offset", target_type=(np.integer, int), min_val=1
             )
         elif self.window_size is not None or self.offset is not None:
-            raise ValueError("'window_size' and 'offset' must be provided together")
+            raise ValueError(
+                "Parameters 'window_size' and 'offset' must be provided together"
+            )
 
     def _window_reconstruct(
         self,
         X: TSCDataFrame,
         edmd: EDMD,
         offset: int,
+        *,
+        U: Optional[TSCDataFrame] = None,
         y=None,
         qois=None,
-        return_X_windows: bool = False,
+        return_windows: bool = False,
     ):
         """Reconstruct existing time series of equal length.
 
         This method is used to overwrite the default score method of an :py:class:`.EDMD`
         model, which in contrast to this model scores on the time series found in `X`.
 
         In this method, the time series are subdivided into smaller time series of
@@ -1558,100 +2144,165 @@
             The time series collection to reconstruct. From each time series of the
             collection windows are extracted and separately reconstructed.
 
         qois
             A list of feature names of interest to be include in the returned
             predictions. Passed to :py:meth:`.predict`.
 
-        return_X_windows
+        return_windows
             If True, then an additional time series collection is returned,
             which contains extracted windows from `X`.
 
         Returns
         -------
         TSCDataFrame, Optional[TSCDataFrame]
-            The reconstructed time series collection and if `return_X_windows=True`
+            The reconstructed time series collection and if `return_windows=True`
             also the extracted windows from `X`.
 
         """
 
+        check_is_fitted(edmd)
+
         if not hasattr(edmd, "window_size"):
             raise AttributeError(
                 "The EDMD object requires the attribute 'window_size' "
-                "to perform windowed reconstruction in data."
+                "to perform windowed reconstruction of time series data."
             )
 
-        if not isinstance(edmd.window_size, int):
-            raise TypeError("'window_size' must be of type int")
-
         if edmd.window_size <= edmd.n_samples_ic_:
             raise ValueError(
                 f"edmd.window_size={edmd.window_size} must be larger than the number of "
-                "samples required to make an initial condition ("
-                f"edmd.n_samples_ic_={edmd.n_samples_ic_})"
+                f"samples required to make an initial condition ({edmd.n_samples_ic_=})"
+            )
+
+        is_controlled = edmd.is_controlled_
+
+        if is_controlled and U is None:
+            raise ValueError(
+                f"The EDMD model was fit with control input "
+                f"({edmd.is_controlled_=}), but no control input was provided ({U=})"
             )
 
         X = edmd._validate_datafold_data(
             X,
             ensure_tsc=True,
             tsc_kwargs=dict(
                 ensure_const_delta_time=True, ensure_min_timesteps=edmd.window_size
             ),
         )
+
+        if is_controlled:
+            U = edmd._validate_datafold_data(
+                U,
+                ensure_tsc=True,
+                tsc_kwargs=dict(
+                    ensure_const_delta_time=True, ensure_delta_time=edmd.dt_
+                ),
+            )
+
         qois = edmd._validate_qois(
             qois=qois, valid_feature_names=edmd.feature_names_pred_
         )
 
         X_windows = TSCDataFrame.from_frame_list(
             list(
                 X.tsc.iter_timevalue_window(
                     window_size=edmd.window_size,
                     offset=offset,
                     per_time_series=True,
-                    strictly_sequential=True,
                 )
             )
         )
 
-        final_index_windows = X_windows.index.copy()
-
         n_timesteps = X_windows.n_timesteps
         assert isinstance(n_timesteps, int) and n_timesteps == edmd.window_size
 
-        final_index_reconstruct = (
+        # align the index and make equal for each time series
+        # (this way the prediction is vectorized)
+        index_final_reconstruct_X = (
             X_windows.groupby(TSCDataFrame.tsc_id_idx_name)
             .tail(edmd.window_size - edmd.n_samples_ic_ + 1)
             .index
         )
 
-        first_id_time_values = X_windows.loc[X_windows.ids[0]].index
+        if return_windows:
+            index_final_windows_X = X_windows.index.copy()
+        else:
+            index_final_windows_X = None
+
+        # for all time series set equal time values equal to allow for vectorized
+        # reconstruction
+        normalized_time_values = X_windows.loc[X_windows.ids[0]].index
         X_windows.index = pd.MultiIndex.from_product(
-            [X_windows.ids, first_id_time_values],
+            [X_windows.ids, normalized_time_values],
             names=[TSCDataFrame.tsc_id_idx_name, TSCDataFrame.tsc_time_idx_name],
         )
 
-        X_reconstruct = edmd._reconstruct(X=X_windows, qois=qois)
+        if is_controlled:
+            assert U is not None  # for mypy typing
+            U_windows = TSCDataFrame.from_frame_list(
+                list(
+                    U.tsc.iter_timevalue_window(
+                        window_size=edmd.window_size,
+                        offset=offset,
+                        per_time_series=True,
+                    )
+                )
+            )
+
+            group = lambda df: df.groupby(TSCDataFrame.tsc_id_idx_name)
+
+            # remove last state, because it is not needed for the prediction
+            U_windows = group(U_windows).head(edmd.window_size - 1)
+            U_n_timesteps = U_windows.n_timesteps
+            assert (
+                isinstance(U_n_timesteps, int) and U_n_timesteps == edmd.window_size - 1
+            )
+
+            # remove first states that are not needed during initial condition
+            drop_indices = group(U_windows).head(edmd.n_samples_ic_ - 1).index
+            U_windows = U_windows.drop(drop_indices, axis=0, errors="ignore")
+
+            if return_windows:
+                index_final_windows_U = U_windows.index.copy()
+            else:
+                index_final_windows_U = None
+
+            normalized_time_values = U_windows.loc[U_windows.ids[0]].index
+            U_windows.index = pd.MultiIndex.from_product(
+                [U_windows.ids, normalized_time_values],
+                names=[TSCDataFrame.tsc_id_idx_name, TSCDataFrame.tsc_time_idx_name],
+            )
+        else:
+            U_windows, index_final_windows_U = None, None
+
+        # finally reconstruct the data
+        X_reconstruct = edmd._reconstruct(X=X_windows, U=U_windows, qois=qois)
 
         # recover true index:
-        X_windows.index = final_index_windows
-        X_reconstruct.index = final_index_reconstruct
+        X_reconstruct.index = index_final_reconstruct_X
 
-        if return_X_windows:
-            return X_reconstruct, X_windows
+        if return_windows:
+            X_windows.index = index_final_windows_X
+            if is_controlled:
+                U_windows.index = index_final_windows_U
+                return X_reconstruct, X_windows, U_windows
+            else:
+                return X_reconstruct, X_windows
         else:
             return X_reconstruct
 
     def _window_score(self, X, y=None, sample_weight=None, qois=None, edmd=None):
         """Score of reconstructed windowed time series collection.
 
         This method can overwrite the default score method of an EDMD model. In this
         method, the time series in `X` are again subdivided into smaller time series of
         equal length (the windows). Each window contains the initial condition and the
         samples to score the model against. This therefore corresponds to a more
-        systematic approach to analyze the error over a prediciton horizon.
+        systematic approach to analyze the error over a prediction horizon.
 
         Parameters
         ----------
         X
             Time series to reconstruct in windowed fashion.
         y
             ignored
@@ -1665,17 +2316,16 @@
 
         Returns
         -------
         float
             score
 
         """
-
         # does all the checks:
-        X_reconstruct, X = edmd.reconstruct(X=X, y=y, qois=qois, return_X_windows=True)
+        X_reconstruct, X = edmd.reconstruct(X=X, y=y, qois=qois, return_windows=True)
 
         if qois is None:
             X_reconstruct = X_reconstruct.loc[:, X.columns]
             X = X.loc[X_reconstruct.index, :]
         else:
             X = X.loc[X_reconstruct.index, qois]
 
@@ -1694,31 +2344,30 @@
 
         Returns
         -------
         EDMD
             The adapted model.
 
         """
+        # TODO: this is bad style, there is no reason to attach the attribute to the estimator
+        #  instead it can be used like offset below...
         estimator.window_size = self.window_size
 
         # overwrite the two methods with new "windowed" methods
         # ignored types for mypy
         estimator.reconstruct = partial(  # type: ignore
             self._window_reconstruct, edmd=estimator, offset=self.offset
         )
         estimator.score = partial(self._window_score, edmd=estimator)  # type: ignore
         return estimator
 
 
-from datafold._decorators import warn_experimental_class
-
-
 @warn_experimental_class
-class EDMDPostObservable(object):  # pragma: no cover
-    """# TODO
+class EDMDPostObservable:  # pragma: no cover
+    """# TODO.
 
     # TODO: Alternative? EDMDCVErrorObservable?
     # TODO: Testing & Docu
     # TODO: compute mean of error time series if offset < blocksize?
 
     Parameters
     ----------
@@ -1762,15 +2411,14 @@
         self.cv = cv
         self.observable = observable
         self.n_jobs = n_jobs
         self.verbose = verbose
         self.pre_dispatch = pre_dispatch
 
     def _adapt_edmd_model(self, edmd, X_validate, abserr_timeseries):
-
         # 1. get original data
         X_dict = edmd.transform(X_validate)
 
         if self.observable == "std":
             target_timeseries = abserr_timeseries * np.sqrt(np.pi / 2)
         else:
             target_timeseries = abserr_timeseries
@@ -1794,51 +2442,39 @@
             ),
             name=TSCDataFrame.tsc_feature_col_name,
         )
 
         return edmd
 
     def _compute_err_timeseries(self, edmd, X_test):
-        """
-
-        Parameters
-        ----------
-        edmd
-        X_test
-        qois
-
-        Returns
-        -------
-
-        """
+        """Compute the error observables time series."""
         # TODO: here is a distinction that maybe is better to solve via a new parameter
         #  in reconstruct (e.g. return_X to return the samples in X that are actually
         #  reconstructed)
 
         try:
             X_reconstruct, X_test = edmd.reconstruct(
-                X_test, qois=None, return_X_windows=True
+                X_test, qois=None, return_windows=True
             )
         except TypeError:
             X_reconstruct = edmd.reconstruct(X_test)
 
         # remove initial states, because they are often almost exact
         X_reconstruct = X_reconstruct.drop(labels=X_reconstruct.head(1).index)
 
         err_timeseries = (X_test.loc[X_reconstruct.index, :] - X_reconstruct).abs()
 
         return X_test, err_timeseries
 
     def _fit_and_create_error_timeseries(
         self, edmd: EDMD, X: TSCDataFrame, y, split_nr, train, test, fit_params, verbose
     ):
-
         if verbose:
             msg = f"split: {split_nr}"
-            print("[CV] %s %s" % (msg, (64 - len(msg)) * "."), flush=True)
+            print("[CV] {} {}".format(msg, (64 - len(msg)) * "."), flush=True)
 
         X_train, X_test = _split_X_edmd(X, y, train_indices=train, test_indices=test)
 
         edmd = edmd.fit(X=X_train, y=y, **fit_params)
 
         test_score = edmd.score(X_test, y=None)
 
@@ -1867,23 +2503,23 @@
 
         if self.observable not in self._valid_observables:
             raise ValueError(
                 f"observable={self.observable} is invalid. "
                 f"Choose from {self._valid_observables}"
             )
 
-    def _run_cv(self, X, y, **fit_params):
+    def _run_cv(self, X: TSCDataFrame, y=None, **fit_params):
         cv = check_cv(self.cv, y, classifier=is_classifier(self.estimator))
         # n_splits = self.cv.get_n_splits(X, y, groups=None)
 
         parallel = Parallel(
             n_jobs=self.n_jobs, verbose=self.verbose, pre_dispatch=self.pre_dispatch
         )
 
-        results: Dict[str, Any] = {}
+        results: dict[str, Any] = {}
         X_validate: Optional[TSCDataFrame] = None
         err_timeseries: Optional[TSCDataFrame] = None
         best_estimator: Optional[EDMD] = None
         with parallel:
 
             def evaluate_cv_splits():
                 nonlocal X_validate
@@ -1907,15 +2543,15 @@
                 if len(ret) < 1:
                     raise ValueError(
                         "No fits were performed. "
                         "Was the CV iterator empty? "
                         "Were there no candidates?"
                     )
 
-                scores: np.ndarray = np.asarray([r["test_score"] for r in ret])
+                scores = np.asarray([r["test_score"] for r in ret])
                 best_estimator_idx = np.argmax(scores)
                 best_estimator = ret[best_estimator_idx]["edmd"]
 
                 X_validate = TSCDataFrame.from_frame_list([r["X_test"] for r in ret])
                 err_timeseries = TSCDataFrame.from_frame_list(
                     [r["err_timeseries"] for r in ret]
                 )
@@ -1929,15 +2565,14 @@
         return X_validate, err_timeseries, best_estimator
 
     def fit_transform(self, X: TSCDataFrame, y=None, **fit_params):
         """Computes the post observables and alters the EDMD estimator.
 
         Parameters
         ----------
-
         X
             Training time series data.
 
         y: None
             ignored
 
         **fit_params : Dict[str, object]
@@ -1966,7 +2601,107 @@
         self.final_estimator_ = self._adapt_edmd_model(
             edmd=self.final_estimator_,
             X_validate=X_validate,
             abserr_timeseries=abserr_timeseries,
         )
 
         return self.final_estimator_
+
+
+@warn_experimental_class
+class HAVOK(BaseEstimator, TSCPredictMixin):  # pragma: no cover
+    def __init__(self, delays, rank=None) -> None:
+        self.rank = rank
+        self.delays = delays
+
+    def transform(self, X: TSCDataFrame):
+        X = self._delay_embedding.transform(X)
+
+        X_svd = (
+            # np.linalg.inv(np.diag(self.svals[: self.svd_rank - 1]))
+            # @
+            np.linalg.pinv(self._ur)
+            @ X.to_numpy().T
+        ).T
+
+        X_svd = TSCDataFrame.from_same_indices_as(
+            X, values=X_svd, except_columns=[f"svd{i}" for i in range(self.rank - 1)]
+        )
+
+        return X_svd
+
+    def fit(self, X: TSCDataFrame, y=None):
+        # TODO: instead of using numpy here, use sciki-learn TruncatedSVD class
+        # TODO: if rank is None, then use the scipy svd
+        # TODO: data validation!
+
+        from datafold import TSCFiniteDifference, TSCTakensEmbedding
+
+        self.dt_ = X.delta_time
+
+        if X.n_timeseries != 1:
+            raise NotImplementedError(
+                "Currently only single time series are supported. Implementation welcome"
+            )
+
+        self._delay_embedding = TSCTakensEmbedding(delays=self.delays).fit(X)
+        X = self._delay_embedding.transform(X)
+
+        U, S, Vh = np.linalg.svd(X.to_numpy().T, full_matrices=False)
+
+        Vr = Vh[: self.rank, :].T
+        Ur = U[:, : self.rank]
+        Sr = S[: self.rank]
+
+        Vr = TSCDataFrame.from_array(
+            Vr,
+            time_values=X.index.get_level_values(TSCDataFrame.tsc_time_idx_name),
+            feature_names=[f"svd{i}" for i in range(self.rank)],
+        )
+        dVr = TSCFiniteDifference(diff_order=1, accuracy=2).fit_transform(
+            Vr.iloc[:, :-1]
+        )
+
+        # account for samples that are lost when computing the finite difference
+        Vr = Vr.loc[dVr.index, :]
+
+        M = np.linalg.lstsq(Vr.to_numpy(), dVr.to_numpy(), rcond=None)[0].T
+
+        assert M.shape == (self.rank - 1, self.rank)
+
+        self.forcing_signal = Vr.iloc[:, [-1]]
+        self.state_matrix = M[:, :-1]
+        self.control_matrix = M[:, [-1]]
+
+        self.svals = S
+
+        from datafold.utils.general import mat_dot_diagmat
+
+        self._ur = mat_dot_diagmat(Ur[:, :-1], Sr[:-1])
+
+        eigenvalues, eigenvectors = np.linalg.eig(self.state_matrix)
+        eigenvalues = np.exp(eigenvalues * self.dt_)
+        self.unnormalized_modes = self._ur @ eigenvectors
+        self._tmp_compute_psi = np.linalg.inv(eigenvectors) @ self._ur.T
+        return self
+
+    def fit_predict(self, X: TSCDataFrame):  # type: ignore
+        self.fit(X=X)
+
+        X_ic = X.initial_states(n_samples=self.delays + 1)
+        X_ic = self.transform(X_ic)
+
+        from datafold.dynfold.dynsystem import LinearDynamicalSystem
+
+        system = LinearDynamicalSystem(
+            is_controlled=True, sys_type="differential", sys_mode="matrix"
+        )
+        system.setup_matrix_system(
+            system_matrix=self.state_matrix, control_matrix=self.control_matrix
+        )
+        X_pred = system.evolve_system(
+            initial_conditions=X_ic.to_numpy().T,
+            control_input=self.forcing_signal.to_numpy()[:, np.newaxis],
+            time_values=self.forcing_signal.time_values()[:-1],
+        )
+
+        return X_pred
```

### Comparing `datafold-1.1.6/datafold/dynfold/__init__.py` & `datafold-2.0.0/datafold/dynfold/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,30 +25,40 @@
 2. Models subclassing :class:`sklearn.base.RegressorMixin`:
    These models interpolate/regress general function values on manifolds. An important
    scenario to use the methods is to provide a mapping (image and pre-image) for
    non-linear manifold learning methods. An example model is the
    :class:`LaplacianPyramidsInterpolator`.
 
 2. Models subclassing :py:class:`.TSCPredictMixin`:
-   On this level this tpye of model are mainly variants of the Dynamic Mode
+   On this level this type of model are mainly variants of the Dynamic Mode
    Decomposition algorithm (:class:`.DMDBase`). These models fit time series data,
    meaning the input is restricted to :class:`TSCDataFrame` input. A fitted model
    defines a linear dynamical system which can be used to predict time series.
 """
 
 from datafold.dynfold.compose import TSCColumnTransformer
-from datafold.dynfold.dmap import DiffusionMaps, LocalRegressionSelection
-from datafold.dynfold.dmd import DMDBase, DMDEco, DMDFull, PyDMDWrapper, gDMDFull
+from datafold.dynfold.dmap import DiffusionMaps, LocalRegressionSelection, Roseland
+from datafold.dynfold.dmd import (
+    DMDBase,
+    DMDControl,
+    DMDStandard,
+    OnlineDMD,
+    PyDMDWrapper,
+    StreamingDMD,
+    gDMDAffine,
+    gDMDFull,
+)
 from datafold.dynfold.outofsample import (
     GeometricHarmonicsInterpolator,
     LaplacianPyramidsInterpolator,
 )
 from datafold.dynfold.transform import (
     TSCApplyLambdas,
     TSCFeaturePreprocess,
     TSCFiniteDifference,
     TSCIdentity,
     TSCPolynomialFeatures,
     TSCPrincipalComponent,
     TSCRadialBasis,
+    TSCSampledNetwork,
     TSCTakensEmbedding,
 )
```

### Comparing `datafold-1.1.6/datafold/dynfold/base.py` & `datafold-2.0.0/datafold/dynfold/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 #!/usr/bin/env python3
 
-from typing import Any, Callable, List, Optional, Tuple, Union
+from datetime import datetime
+from typing import Any, Callable, Optional, Union
 
 import numpy as np
+import numpy.testing as nptest
 import pandas as pd
-import pandas.testing as pdtest
 from pandas.api.types import is_datetime64_dtype
-from sklearn.base import TransformerMixin
+from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.exceptions import NotFittedError
 from sklearn.utils.validation import check_array, check_is_fitted
 
 from datafold.pcfold import InitialCondition, TSCDataFrame, TSCMetric, TSCScoring
 from datafold.pcfold.timeseries.collection import TSCException
-from datafold.utils.general import if1dim_rowvec
+from datafold.utils.general import if1dim_rowvec, is_df_same_index
 
 # types allowed for transformation
 TransformType = Union[TSCDataFrame, np.ndarray]
 
 # types allowed for time predictions
 TimePredictType = TSCDataFrame
 InitialConditionType = Union[TSCDataFrame, np.ndarray]
 
 
-class TSCBaseMixin(object):
+class TSCBase:
     """Base class for Mixin's in *datafold*.
 
     See Also
     --------
     :py:class:`.TSCTransformerMixin`
     :py:class:`.TSCPredictMixin`
     """
 
+    def get_feature_names_out(self, input_features=None):
+        raise NotImplementedError(
+            "class has not implemented 'get_feature_names_out' method"
+        )
+
     def _has_feature_names(self, _obj):
         # True, for pandas.DataFrame or TSCDataFrame
         return isinstance(_obj, pd.DataFrame)
 
-    def _read_fit_params(self, attrs: Optional[List[Tuple[str, Any]]], fit_params):
+    def _read_fit_params(self, attrs: Optional[list[tuple[str, Any]]], fit_params):
         return_values = []
 
         if attrs is not None:
-            for attr in attrs:
-                return_values.append(fit_params.pop(attr[0], attr[1]))
+            for a in attrs:
+                return_values.append(fit_params.pop(a[0], a[1]))
 
         if fit_params != {}:
-            raise KeyError(f"fit_params.keys = {fit_params.keys()} not supported")
+            raise KeyError(f"{fit_params.keys()=} are not supported")
 
         if len(return_values) == 0:
             return None
         elif len(return_values) == 1:
             return return_values[0]
         else:
             return return_values
@@ -73,282 +79,267 @@
                 f"{check_attributes} are not available for estimator {self}. "
                 f"Please report bug."
             )
 
     def _validate_datafold_data(
         self,
         X: Union[TSCDataFrame, np.ndarray],
+        *,
+        ensure_np: bool = False,
         ensure_tsc: bool = False,
+        force_all_finite: bool = True,
+        ensure_min_samples: int = 1,
+        ensure_min_features: int = 1,
         array_kwargs: Optional[dict] = None,
         tsc_kwargs: Optional[dict] = None,
     ):
         """Provides a general function to validate data that is input to datafold
         functions -- it can be overwritten if a concrete implementation requires
         different checks.
 
         This function is very close to scikit-learn BaseEstimator._validate_data (which
         was introduced in  0.23.1).
 
         Parameters
         ----------
         X
-        ensure_feature_name_type
+        ensure_np
+        ensure_tsc
         array_kwargs
         tsc_kwargs
 
         Returns
         -------
 
         """
-
         # defaults to empty dictionary if None
         array_kwargs = array_kwargs or {}
         tsc_kwargs = tsc_kwargs or {}
 
-        if ensure_tsc and not isinstance(X, TSCDataFrame):
-            raise TypeError(
-                f"Input 'X' is of type {type(X)} but a TSCDataFrame is required."
-            )
+        if ensure_np + ensure_tsc == 2:
+            raise ValueError("only 'ensure_np' or 'ensure_tsc' can be True")
+
+        if self._has_feature_names(X):
+            if X.columns.ndim != 1:
+                raise ValueError(
+                    f"The feature columns of X must be 1-dim. Got {X.columns.ndim=}"
+                )
 
         if type(X) != TSCDataFrame:
             # Currently, everything that is not strictly a TSCDataFrame will go the
-            # path of an usual array format. This includes:
+            # path of a usual array format. This includes:
             #  * sparse scipy matrices
             #  * numpy ndarray
             #  * memmap
-            #  * pandas.DataFrame (Note a TSCDataFrame is also a pandas.DataFrame,
-            #                      but not strictly)
+            #  * pd.DataFrame (Note that TSCDataFrame is also a pd.DataFrame,
+            #                  but not in a strict sense)
+
+            if ensure_tsc:
+                raise TypeError(
+                    f"Found type {type(X)=} but type TSCDataFrame is required."
+                )
 
             tsc_kwargs = {}  # no need to check -> overwrite to empty dict
 
             if type(X) == pd.DataFrame:
+                if ensure_np:
+                    TypeError(f"Found type {type(X)=} but type np.ndarray is required.")
+
                 # special handling of pandas.DataFrame (strictly, not including
                 # TSCDataFrame) --> keep the type (recover after validation).
                 assert isinstance(X, pd.DataFrame)  # mypy checking
                 revert_to_data_frame = True
                 idx, col = X.index, X.columns
+
             else:
                 revert_to_data_frame = False
                 idx, col = [None] * 2
 
             X = check_array(
                 X,
                 accept_sparse=array_kwargs.pop("accept_sparse", False),
                 accept_large_sparse=array_kwargs.pop("accept_large_sparse", False),
                 dtype=array_kwargs.pop("dtype", "numeric"),
                 order=array_kwargs.pop("order", None),
                 copy=array_kwargs.pop("copy", False),
-                force_all_finite=array_kwargs.pop("force_all_finite", True),
+                force_all_finite=force_all_finite,
                 ensure_2d=array_kwargs.pop("ensure_2d", True),
                 allow_nd=array_kwargs.pop("allow_nd", False),
-                ensure_min_samples=array_kwargs.pop("ensure_min_samples", 1),
-                ensure_min_features=array_kwargs.pop("ensure_min_features", 1),
+                ensure_min_samples=ensure_min_samples,
+                ensure_min_features=ensure_min_features,
                 estimator=self,
             )
 
             if revert_to_data_frame:
                 X = pd.DataFrame(X, index=idx, columns=col)
 
-        else:
+        else:  # isinstance(X, TSCDataFrame)
+            if ensure_np:
+                raise TypeError(
+                    f"Input 'X' is of type {type(X)} but a numpy format is required."
+                )
 
             array_kwargs = {}  # no need to check -> overwrite to empty dict
 
             X = X.tsc.check_tsc(
-                ensure_all_finite=tsc_kwargs.pop("ensure_all_finite", True),
-                ensure_min_samples=tsc_kwargs.pop("ensure_min_samples", None),
+                ensure_all_finite=force_all_finite,
+                ensure_min_samples=ensure_min_samples,
                 ensure_same_length=tsc_kwargs.pop("ensure_same_length", False),
                 ensure_const_delta_time=tsc_kwargs.pop(
                     "ensure_const_delta_time", False
                 ),
                 ensure_delta_time=tsc_kwargs.pop("ensure_delta_time", None),
                 ensure_same_time_values=tsc_kwargs.pop(
                     "ensure_same_time_values", False
                 ),
                 ensure_normalized_time=tsc_kwargs.pop("ensure_normalized_time", False),
                 ensure_n_timeseries=tsc_kwargs.pop("ensure_n_timeseries", None),
+                ensure_n_timesteps=tsc_kwargs.pop("ensure_n_timesteps", None),
                 ensure_min_timesteps=tsc_kwargs.pop("ensure_min_timesteps", None),
                 ensure_no_degenerate_ts=tsc_kwargs.pop(
                     "ensure_no_degenerate_ts", False
                 ),
+                ensure_dtype_time=tsc_kwargs.pop("ensure_dtype_time", None),
             )
 
-        if array_kwargs != {} or tsc_kwargs != {}:
-            # validate_kwargs have to be empty and must only contain key-values that can
-            # be handled to check_array / check_tsc
+        if array_kwargs or tsc_kwargs:
+            # validation kwargs have to be empty at this point (after "kwargs.pop()" above)
 
             left_over_keys = list(array_kwargs.keys()) + list(tsc_kwargs.keys())
             raise ValueError(
-                f"{left_over_keys} are no valid validation keys. Please report bug."
+                f"{left_over_keys} are no valid keys arguments. Please report bug."
             )
 
         return X
 
 
-class TSCTransformerMixin(TSCBaseMixin, TransformerMixin):
+class TSCTransformerMixin(TSCBase, TransformerMixin):
     """Mixin to provide functionality for point cloud and time series transformations.
 
     Generally, the following input/output types are supported.
 
     * :class:`numpy.ndarray`
     * :class:`pandas.DataFrame` no restriction on the frame's index and column format
     * :class:`.TSCDataFrame` as a special data frame for time series collections
 
     The parameters should be set in during `fit` in a subclass.
 
-    .. note::
-
-        The scikit-learn project heavily discusses on how to handle feature names. There
-        are many proposed solutions. The solution that datafold uses is
-        `SLEP007 <https://scikit-learn-enhancement-proposals.readthedocs.io/en/latest/slep007/proposal.html>`__
+    Discussions in the scikit-learn project, which are followed in datafold:
 
-        However, this is only a proposal and may have to be changed later.
+    * `SLEP 007 <https://scikit-learn-enhancement-proposals.readthedocs.io/en/latest/slep007/proposal.html>`__
+    * `SLEP 010 <https://scikit-learn-enhancement-proposals.readthedocs.io/en/latest/slep010/proposal.html>`__
 
-        Other resources:
+    Other related discussions (also proposing different solutions):
 
-        * `new array (SLEP012) <https://scikit-learn-enhancement-proposals.readthedocs.io/en/latest/slep012/proposal.html>`__
-        * `discussion (SLEP008) <https://github.com/scikit-learn/enhancement_proposals/pull/18/>`__
+    * `new array (SLEP012) <https://scikit-learn-enhancement-proposals.readthedocs.io/en/latest/slep012/proposal.html>`__
+    * `discussion (SLEP008) <https://github.com/scikit-learn/enhancement_proposals/pull/18/>`__
 
     Parameters
     ----------
-
     n_features_in_: int
-        Number of features of input during `fit`.
+        Number of features in input `X` during `fit`. The same number of features are
+        required for `transform`.
 
-    n_features_in_: Optional[pd.Index]
-        Feature names during `fit` if the input is indexed. The feature names
-        are used as output in `inverse_transform` and for validation in `transform`.
+    feature_names_in_: Optional[np.array]
+        Feature names passed in input `X` in `fit`. The attribute is only set if the input is
+        a pandas object. The feature names are used for validation of input in `transform` and
+        as output feature names in `inverse_transform`.
 
     n_features_out_: int
-        Number of features of output during `fit`.
-
-    features_out_: Optional[pd.Index]
-        Feature names during `fit` if the input is indexed. The feature names
-        are used as output in `transform` and for validation in `inverse_transform`.
+        Number of features in output of `transform`.
     """
 
-    _feature_attrs = [
-        "n_features_in_",
-        "n_features_out_",
-        "feature_names_in_",
-        "feature_names_out_",
-    ]
-
-    def _setup_feature_attrs_fit(self, X, features_out):
-
-        if isinstance(features_out, str):
-            assert features_out == "like_features_in"
-
-        if self._has_feature_names(X):
+    def _setup_feature_attrs_fit(
+        self: Union[BaseEstimator, "TSCTransformerMixin"],
+        X,
+        n_features_out: Optional[int] = None,
+    ) -> None:
+        if not hasattr(self, "n_features_in_"):
+            # sklearn function to set n_features_in_
+            self._check_n_features(X, reset=True)
+
+        if not hasattr(self, "feature_names_in_"):
+            if isinstance(X, TSCDataFrame) and type(X.columns[0]) != str:
+                # workaround for datafold to support non-str feature names
+                # sklearn does only support feature names of type str
+                # Note that there is a guarantee for TSCDataFrame that the feature names have
+                # same type
+                self.feature_names_in_ = X.columns.to_numpy()
+            else:
+                # sklearn function to set feature_names_in_
+                self._check_feature_names(X, reset=True)
 
-            if isinstance(features_out, str) and features_out == "like_features_in":
-                features_out = X.columns
+        # TODO: set features out implemented in alignment to SLEO013, but this proposal was
+        #  rejected -- think of removing n_features_out (check how often and where it is used)
+        # https://scikit-learn-enhancement-proposals.readthedocs.io/en/latest/slep013/proposal.html  # noqa
+        if not hasattr(self, "n_features_out_"):
+            if n_features_out is None:
+                feature_out = self.get_feature_names_out()
+                self.n_features_out_: int = len(feature_out)
+            else:
+                self.n_features_out_ = n_features_out
 
-            if isinstance(features_out, (list, np.ndarray)):
-                # For convenience features_out can be given as a list
-                # (better code readability than pd.Index)
-                features_out = pd.Index(
-                    features_out,
-                    dtype=np.str_,
-                    name=TSCDataFrame.tsc_feature_col_name,
-                )
+    def _validate_feature_input(
+        self: Union[BaseEstimator, "TSCTransformerMixin"], X: TransformType, direction
+    ) -> None:
+        self._check_attributes_set_up(["n_features_in_", "n_features_out_"])
+
+        if direction == "transform":
+            self._check_n_features(X, reset=False)
+            self._check_feature_names(X, reset=False)
+        else:  # direction == inverse_transform
+            should_n_features = self.n_features_out_
 
-            if X.columns.has_duplicates or features_out.has_duplicates:
+            if should_n_features != X.shape[1]:
                 raise ValueError(
-                    "duplicated indices detected. \n"
-                    f"features_in={X.columns.duplicated()} \n"
-                    f"features_out={features_out.duplicated()}"
+                    f"The number of features (={X.shape[1]}) do not match. "
+                    f"Required: {should_n_features}"
                 )
 
-            if X.columns.ndim != 1 or features_out.ndim != 1:
-                raise ValueError("feature names must be 1-dim.")
-
-            self.n_features_in_: int = len(X.columns)
-            self.n_features_out_: int = len(features_out)
-            self.feature_names_in_: Optional[pd.Index] = X.columns
-            self.feature_names_out_: Optional[pd.Index] = features_out
-
-        else:
-
-            if isinstance(features_out, str) and features_out == "like_features_in":
-                features_out = X.shape[1]
-            elif isinstance(features_out, int):
-                assert features_out > 0
-            else:
-                # if list or pd.Index use the number of features out
-                features_out = len(features_out)
+            if self._has_feature_names(X):
+                should_features = self.get_feature_names_out()
+                try:
+                    nptest.assert_array_equal(should_features, X.columns.to_numpy())
+                except AssertionError:
+                    raise ValueError(
+                        f"The features names do not match. "
+                        f"Required: {should_features}."
+                    )
 
-            # do not store names, because they are not available
-            self.n_features_in_ = X.shape[1]
-            self.n_features_out_ = features_out
-            self.feature_names_in_ = None
-            self.feature_names_out_ = None
-
-    def _validate_feature_input(self, X: TransformType, direction):
-
-        self._check_attributes_set_up(self._feature_attrs)
-
-        if not self._has_feature_names(X) or self.feature_names_out_ is None:
-            # Either
-            # * X has no feature names, or
-            # * during fit X had no feature names given.
-            # --> Only check if shape is correct and trust user with the rest
-
-            if direction == "transform":
-                _check_shape = self.n_features_in_
-            else:  # direction == "inverse_transform"
-                _check_shape = self.n_features_out_
+    def _more_tags(self) -> dict:
+        """Add tag to scikit-learn tags to indicate whether the original states in `X` are
+        preserved during the transformation.
 
-            if _check_shape != X.shape[1]:
-                raise ValueError(
-                    f"Shape mismatch: expected {self.n_features_out_} "
-                    f"features (number of columns in 'X') but got {X.shape[1]}."
-                )
-        else:  # self._has_feature_names(X)
-            # Now X has features and during fit features were given. So now we can
-            # check if feature names of X match with data during fit:
-
-            if direction == "transform":
-                _check_features = self.feature_names_in_
-            elif direction == "inverse_transform":
-                _check_features = self.feature_names_out_
-            else:
-                raise RuntimeError(
-                    f"'direction'={direction} not known. Please report bug."
-                )
-
-            if isinstance(X, pd.Series):
-                # if X is a Series, then the columns of the original data are in a
-                # Series this usually happens if X.iloc[0, :] --> returns a Series
-                pdtest.assert_index_equal(right=_check_features, left=X.index)
-            else:
-                pdtest.assert_index_equal(right=_check_features, left=X.columns)
+        Defaults to False and can be overwritten by transformers.
+        """
+        return dict(tsc_contains_orig_states=False)
 
     def _same_type_X(
-        self, X: TransformType, values: np.ndarray, feature_names: pd.Index
+        self,
+        X: TransformType,
+        values: np.ndarray,
+        feature_names: Union[pd.Index, np.ndarray],
     ) -> Union[pd.DataFrame, TransformType]:
-        """Chooses the same type for input as type of `X`.
+        """Return object with the same type as for input `X`.
 
         Parameters
         ----------
         X
-            Object from which the type will be inferred.
+            Object from which the type is inferred.
 
         values
             Data to transform in the same format as `X`.
 
         feature_names
             Feature names in case `X` is a :class:`pandas.DataFrame`.
 
         Returns
         -------
 
         """
-
-        _type = type(X)
-
         if isinstance(X, TSCDataFrame):
             # NOTE: order is important here TSCDataFrame is also a DataFrame, so first
             # check for the special case, then for the more general case.
 
             return TSCDataFrame.from_same_indices_as(
                 X, values=np.asarray(values), except_columns=feature_names
             )
@@ -383,29 +374,46 @@
         Returns
         -------
         numpy.ndarray, pandas.DataFrame, TSCDataFrame
             Transformed array of shape `(n_samples, n_transformed_features)` and of same
             type as input `X`.
         """
         # This is only to overwrite the datafold documentation from scikit-learns docs
-        return super(TSCTransformerMixin, self).fit_transform(X=X, y=y, **fit_params)
+        return super().fit_transform(X=X, y=y, **fit_params)
+
+    def partial_fit_transform(
+        self, X: TransformType, y=None, **fit_params
+    ) -> TransformType:
+        """TODO.
+
+        Parameters
+        ----------
+        X
+        y
+        fit_params.
 
+        Returns
+        -------
 
-class TSCPredictMixin(TSCBaseMixin):
+        """
+        self.partial_fit: Callable
+        return self.partial_fit(X, y=y, **fit_params).transform(X)
+
+
+class TSCPredictMixin(TSCBase):
     """Mixin to provide functionality for models that train on time series data.
 
     The attribute should be set during `fit` and used to validate during `predict`.
 
     Parameters
     ----------
-
     n_features_in_: int
         Number of features during `fit`.
 
-    feature_names_in_: pd.Index
+    feature_names_in_: np.ndarray
         The feature names during `fit`.
 
     time_values_in_: numpy.ndarray
         Time values with all time values observed during `fit`. Note, that because in a
         time series collection not all time series must share the same time
         values, a time value to be recorded in `time_values_in_` must at least appear
         in one time series.
@@ -413,188 +421,394 @@
     dt_: Union[float, pd.Series]
         Time sampling rate in the time series data during `fit`.
     """
 
     _cls_feature_attrs = [
         "n_features_in_",
         "feature_names_in_",
-        "time_values_in_",
         "dt_",
     ]
 
-    @property
-    def time_interval_(self):
-        self._check_attributes_set_up(check_attributes="time_values_in_")
-        return (self.time_values_in_[0], self.time_values_in_[-1])
-
     def _setup_default_tsc_metric_and_score(self):
         self.metric_eval = TSCMetric(metric="rmse", mode="feature", scaling="min-max")
         self._score_eval = TSCScoring(self.metric_eval)
 
-    def _setup_features_and_time_attrs_fit(self, X: TSCDataFrame):
-
+    def _validate_and_setup_fit_attrs(
+        self: Union[BaseEstimator, "TSCPredictMixin"],
+        X: TSCDataFrame,
+        U: Optional[TSCDataFrame] = None,
+    ):
         if not isinstance(X, TSCDataFrame):
-            raise TypeError("Only TSCDataFrame can be used for 'X'.")
+            raise TypeError(
+                f"Only TSCDataFrame can be used for system data (got {type(U)=})."
+            )
+
+        is_controlled = U is not None
+
+        if is_controlled and not isinstance(X, TSCDataFrame):
+            raise TypeError(
+                f"Only TSCDataFrame can be used for control data (got {type(U)=})."
+            )
+
+        self.n_features_in_ = X.shape[1]
+        self.feature_names_in_ = X.columns
+
+        if is_controlled:
+            self.n_control_in_ = U.shape[1]  # type: ignore
+            self.control_names_in_ = U.columns  # type: ignore
 
         time_values = X.time_values()
-        features_in = X.columns
+        time_values = self._validate_time_values_format(time_values=time_values)
+
+        req_last_control_state = getattr(self, "_requires_last_control_state", False)
+
+        if is_controlled and not is_df_same_index(
+            X.tsc.drop_last_n_samples(1) if not req_last_control_state else X,
+            U,
+            check_column=False,
+            check_names=False,
+            handle=None,
+        ):
+            msg = "(except the last state) " if not req_last_control_state else ""
+
+            raise ValueError(
+                f"For each system state {msg}in `X`, there must be a matching "
+                "control input in `U` (i.e. corresponding ID and time value)."
+            )
 
-        time_values = self._validate_time_values(time_values=time_values)
-        self.time_values_in_ = time_values
-        self.n_features_in_ = len(features_in)
-        self.feature_names_in_ = features_in
         self.dt_ = X.delta_time
 
-        if isinstance(self.dt_, pd.Series) or np.isnan(
-            self.dt_
-        ):  # Series if dt_ is not the same across multiple time series.
+        if isinstance(self.dt_, pd.Series) or np.isnan(self.dt_):
+            # Series if dt_ is not the same for all time series in the data.
             raise NotImplementedError(
                 "Currently, all algorithms assume a constant time "
-                f"delta. Got X.time_delta={X.time_delta}"
+                f"delta. Got {X.time_delta=}."
             )
 
         # TODO: check this closer why are there 5 decimals required?
         assert (
             np.around(
-                (self.time_interval_[1] - self.time_interval_[0]) / self.dt_, decimals=5
+                (np.max(time_values) - np.min(time_values)) / self.dt_, decimals=5
             )
             % 1
             == 0
         )
 
-    def _validate_time_values(self, time_values: np.ndarray):
+    def _validate_and_set_time_values_predict(
+        self,
+        time_values: Optional[np.ndarray],
+        X: Union[TSCDataFrame, np.ndarray],
+        U: Optional[Union[TSCDataFrame, np.ndarray]],
+        dt=None,
+    ):
+        # comparing time values in floating points is sometimes a bit tricky, because two
+        # effectively equal values have a tiny difference -- this parameter is used within
+        # this function as a tolerance value
+        _numerical_tol = 1e-14
+        _numerical_tol = 0
+
+        if dt is None:
+            try:
+                dt = self.dt_
+            except AttributeError:
+                raise NotFittedError(
+                    "The time sampling dt needs to be either"
+                    "passed by argument or in attribute self.dt_."
+                )
+
+        is_controlled = U is not None
+        req_last_control_state = getattr(self, "_requires_last_control_state", False)
+
+        if isinstance(X, TSCDataFrame):
+            reference = X.final_states(n_samples=1).time_values()
+            reference = np.unique(reference)
+            if np.size(reference) != 1:
+                raise ValueError(
+                    "All initial conditions must have the same time reference. "
+                    f"Got {reference=}."
+                )
+            else:
+                reference = reference[0]
+        else:
+            if is_controlled and isinstance(U, TSCDataFrame):
+                reference = U.time_values()[0]
+            else:
+                if isinstance(dt, np.timedelta64):
+                    reference = np.datetime64(datetime.now())
+                else:
+                    reference = 0
+
+        if time_values is None:
+            if is_controlled:
+                if callable(U):
+                    raise ValueError(
+                        "If `U` is a control input function (callable), then the "
+                        "parameter 'time_values' cannot be None."
+                    )
 
+                if isinstance(U, TSCDataFrame):
+                    time_values = U.time_values()
+
+                    if not req_last_control_state:
+                        time_values = np.append(time_values, time_values[-1] + dt)
+
+                    # the -1E-14 is needed to avoid that numerical noise removes the actual
+                    # reference point from the time values
+                    time_values = time_values[time_values >= reference - _numerical_tol]
+
+                    if time_values.size == 0:
+                        raise ValueError(
+                            f"There are no time values in 'U' that are greater "
+                            f"than the {reference=} time value in 'X'. No time "
+                            f"values for prediction could be obtained."
+                        )
+
+                else:
+                    time_values = np.arange(
+                        reference,
+                        reference
+                        + _numerical_tol
+                        + (U.shape[0] + int(not req_last_control_state))  # type: ignore
+                        * dt,
+                        dt,
+                    )
+            else:
+                time_values = np.array([reference, reference + dt])
+        else:
+            time_values = self._validate_time_values_format(time_values=time_values)
+
+            if is_controlled:
+                if isinstance(U, np.ndarray):
+                    if len(time_values) != U.shape[0] + int(not req_last_control_state):
+                        str_req_control_states = (
+                            f"{U.shape[0]-1=}"
+                            if int(not req_last_control_state)
+                            else f"{U.shape[0]=}"
+                        )
+
+                        raise ValueError(
+                            f"The length of time values ({len(time_values)=}) "
+                            "does not match the number of control states "
+                            f"(required: {str_req_control_states}, got: {U.shape[0]=})."
+                        )
+                elif isinstance(U, TSCDataFrame):
+                    req_time_values = U.time_values()
+                    req_time_values = req_time_values[
+                        req_time_values >= reference - _numerical_tol
+                    ]
+
+                    if not req_last_control_state:
+                        req_time_values = np.append(
+                            req_time_values, req_time_values[-1] + dt
+                        )
+
+                    if (
+                        time_values.shape != req_time_values.shape
+                        or not (
+                            np.array(time_values - req_time_values) <= _numerical_tol
+                        ).all()
+                    ):
+                        raise ValueError(
+                            "The two parameters ('U' and 'time_values') provide mismatching "
+                            "time information for the current prediction. It is recommended "
+                            "to only provide the control input 'U'."
+                        )
+                elif callable(U):
+                    pass  # nothing to do for now ...
+                else:
+                    raise TypeError(
+                        f"Invalid type of control input 'U' (got {type(U)=}."
+                    )
+
+            if isinstance(X, TSCDataFrame):
+                if (time_values < reference - _numerical_tol).any():
+                    smaller_time_values = time_values[time_values < reference]
+                    if len(smaller_time_values) > 4:
+                        n_values = len(smaller_time_values)
+                        smaller_time_values = smaller_time_values[:4]
+                        msg = f"{smaller_time_values=} [...] ({n_values=})"
+                    else:
+                        msg = f"{smaller_time_values}"
+
+                    raise ValueError(
+                        "The time values must not contain any value that is smaller than the "
+                        f"time reference of the initial condition ({reference=})\n"
+                        f"Invalid values found: {msg}"
+                    )
+
+                if np.abs(reference - time_values[0]) > _numerical_tol:
+                    time_values = np.append(reference, time_values)
+        return time_values
+
+    def _validate_time_values_format(self, time_values: np.ndarray) -> np.ndarray:
         try:
             time_values = np.asarray(time_values)
         except Exception:
-            raise TypeError("Cannot convert 'time_values' to array.")
+            raise TypeError(
+                f"Cannot convert 'time_values' to NumPy array. "
+                f"Got {type(time_values)=}."
+            )
 
-        if not isinstance(time_values, np.ndarray):
-            raise TypeError("time_values has to be a NumPy array")
+        if time_values.ndim != 1:
+            raise ValueError("'time_values' must be be an 1-dim. array")
 
         if time_values.dtype.kind not in "iufM":
             # see for dtype.kind values:
             # https://docs.scipy.org/doc/numpy/reference/generated/numpy.dtype.kind.html
-            raise TypeError(f"time_values.dtype {time_values.dtype} not supported")
+            raise TypeError(f"{time_values.dtype=} not supported")
 
         if not is_datetime64_dtype(time_values) and (time_values < 0).any():
             # "datetime" cannot be negative and raises error when checked with "< 0"
             raise ValueError("In 'time_values' all values must be non-negative.")
 
         if not np.isfinite(time_values).all():
             raise ValueError("'time_values' contains invalid numbers (inf/nan).")
 
-        if time_values.ndim != 1:
-            raise ValueError("'time_values' must be be an 1-dim. array")
-
         if not (np.diff(time_values).astype(float) > 0).all():
             # as "float64" is required in case of datetime where the differences are in
             # terms of "np.timedelta"
             raise ValueError(
-                "'time_values' must be sorted with increasing unique values"
+                "'time_values' must be sorted with increasing (unique) numeric values"
             )
 
         return time_values
 
     def _validate_delta_time(self, delta_time):
         self._check_attributes_set_up(check_attributes=["dt_"])
 
         if isinstance(delta_time, pd.Series):
             raise NotImplementedError(
-                "Currently, all methods assume that dt_ is const."
+                "Currently, all methods require that dt_ is constant. "
             )
 
-        if delta_time != self.dt_:
+        if np.abs(delta_time - self.dt_) > 1e-14:
             raise TSCException(
-                f"delta_time during fit was {self.dt_}, now it is {delta_time}"
+                f"delta_time during fit was {self.dt_=}, now it is {delta_time=} "
+                f"({np.abs(delta_time - self.dt_)=} with set tolerance 1e-14) "
             )
 
-    def _validate_feature_names(self, X: TransformType, require_all=True):
-        self._check_attributes_set_up(check_attributes=["feature_names_in_"])
+    def _validate_feature_names(
+        self: Union[BaseEstimator, "TSCPredictMixin"],
+        X: TSCDataFrame,
+        U: Optional[TSCDataFrame] = None,
+    ):
+        if not self._has_feature_names(X):
+            raise TypeError(
+                "only types that are indexed with time and states are supported"
+            )
+
+        self._check_n_features(X, reset=False)  # type: ignore
 
         try:
-            if require_all:
-                pdtest.assert_index_equal(
-                    right=self.feature_names_in_, left=X.columns, check_names=False
+            # alternative check in datafold to sklearn
+            # self._check_feature_names(reset=False)
+            # Reason: in datafold there are also non-string feature names allowed
+            nptest.assert_array_equal(
+                np.asarray(X.columns), np.asarray(self.feature_names_in_)
+            )
+        except AssertionError:
+            raise ValueError(
+                f"model was fit with feature names\n{self.feature_names_in_.tolist()}\n"
+                f"but got\n{X.columns.tolist()}"
+            )
+
+        if U is not None:
+            try:
+                # alternative check in datafold to sklearn
+                # self._check_feature_names(reset=False)
+                # Reason: in datafold there are also non-string feature names allowed
+                nptest.assert_array_equal(
+                    np.asarray(U.columns), np.asarray(self.control_names_in_)
+                )
+            except AssertionError:
+                raise ValueError(
+                    f"model was fit with feature names\n{self.control_names_in_.tolist()}\n"
+                    f"but got\n{U.columns.tolist()}"
                 )
-            else:
-                if not np.isin(X.columns, self.feature_names_in_).all():
-                    raise AssertionError(
-                        f"feature names in X are invalid "
-                        f"{X.columns[np.isin(self.feature_names_in_,X.columns)]}"
-                    )
-        except AssertionError as e:
-            raise ValueError(e.args[0])
 
-    def _validate_qois(self, qois, valid_feature_names) -> np.ndarray:
+            if self.n_control_in_ != U.shape[1]:
+                raise ValueError(
+                    f"The number of set control states ({self.n_control_in_=}) does not fit "
+                    f"the current number in the control input {U.shape[1]=}."
+                )
 
+    def _validate_qois(self, qois, valid_feature_names) -> np.ndarray:
         if qois is not None:
             try:
                 qois = np.asarray(qois)
-            except:
-                raise TypeError("parameter 'qois' must be list-like")
+            except Exception:
+                raise TypeError(
+                    f"Parameter 'qois' must be list-like. Got {type(qois)=}"
+                )
 
             if qois.ndim != 1:
                 raise ValueError(
-                    f"'qois' must be a 1-dim. array. " f"Got qois.ndim={qois.ndim}"
+                    f"Parameter 'qois' must be a 1-dim. array. Got {qois.ndim=}"
                 )
 
             mask_valid_qois = np.isin(qois, valid_feature_names)
 
             if not mask_valid_qois.all():
                 raise ValueError(
-                    f"The qois={qois[~mask_valid_qois]} are invalid. Valid "
+                    f"qois={qois[~mask_valid_qois]} are invalid. Valid "
                     f"feature names are {valid_feature_names}."
                 )
 
         return qois
 
     def _validate_features_and_time_values(
-        self, X: TSCDataFrame, time_values: Optional[np.ndarray]
+        self,
+        X: TSCDataFrame,
+        U: Optional[TSCDataFrame],
+        time_values: Optional[np.ndarray],
     ):
+        self._validate_feature_names(X=X, U=U)
+        self._validate_time_values_format(time_values=time_values)
 
-        self._check_attributes_set_up(check_attributes=["time_values_in_"])
-
-        if time_values is None:
-            time_values = self.time_values_in_
-
-        if not self._has_feature_names(X):
-            raise TypeError("only types that support feature names are supported")
-
-        time_values = self._validate_time_values(time_values=time_values)
-        self._validate_feature_names(X)
-
-        return X, time_values
+        return X, U, time_values
 
     def predict(
         self,
         X: InitialConditionType,
+        *,
+        U: Optional[Union[np.ndarray, TSCDataFrame, Callable]] = None,
         time_values: Optional[np.ndarray] = None,
         **predict_params,
-    ):
-        # intended for duck-typing, but provides method layout
+    ) -> TSCDataFrame:
+        # intended for duck-typing, but provides argument layout
         raise NotImplementedError("method not implemented")
 
     def fit_predict(
         self,
         X: InitialConditionType,
+        *,
+        U=None,
         y=None,
         **fit_params,
     ) -> TSCDataFrame:
-        # overwrite if necessary
+        """Standard fit_predict method. Overwrite if necessary."""
         self.fit: Callable
-        return self.fit(X, **fit_params).predict(X.initial_states())
+
+        # TODO: it is likely that this fails for U is not None, as predict also requires U
+        return self.fit(X, U=U, y=y, **fit_params).predict(X.initial_states(), U=U)
 
     def reconstruct(
         self,
         X: TSCDataFrame,
-        qois: Optional[Union[np.ndarray, pd.Index, List[str]]] = None,
+        *,
+        U: Optional[TSCDataFrame] = None,
+        qois: Optional[Union[np.ndarray, pd.Index, list[str]]] = None,
     ):
+        """Standard reconstruct method. Overwrite if necessary."""
         X_reconstruct_ts = []
 
         for X_ic, time_values in InitialCondition.iter_reconstruct_ic(
             X, n_samples_ic=1
         ):
-            X_ts = self.predict(X=X_ic, time_values=time_values)
+            X_ts = self.predict(
+                X=X_ic,
+                U=U.loc[pd.IndexSlice[X_ic.ids, :], :] if U is not None else None,
+                time_values=time_values,
+            )
             X_reconstruct_ts.append(X_ts)
 
         return pd.concat(X_reconstruct_ts, axis=0)
```

### Comparing `datafold-1.1.6/datafold/dynfold/compose.py` & `datafold-2.0.0/datafold/dynfold/compose.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env python3
 
-from typing import List, Tuple
 
-import numpy as np
 import pandas as pd
-import sklearn.compose as compose
-import sklearn.pipeline as pipeline
+from sklearn import compose, pipeline
 from sklearn.utils.validation import check_is_fitted
 
 from datafold.dynfold.base import TransformType, TSCTransformerMixin
 
 
 class TSCPipeline(pipeline.Pipeline, TSCTransformerMixin):  # pragma: no cover
-    @property
-    def feature_names_in_(self):
-        return self.steps[0][1].feature_names_in_
+    # @property # Note: this property is handled in the super class
+    # def feature_names_in_(self):
+    #    return self.steps[0][1].feature_names_in_
 
     @property
     def n_features_out_(self):
         return self.steps[-1][1].n_features_out_
 
     @property
     def feature_names_out_(self):
@@ -28,85 +25,67 @@
 class TSCColumnTransformer(compose.ColumnTransformer, TSCTransformerMixin):
     """A column transformer for time series data.
 
     This class is a wrapper class of scikit-learn's ColumnTransformer and adopted for
     :py:class:`TSCDataFrame` in the pipeline.
 
     For the undocumented attributes please go to the base class documentation
-    `ColumnTransformer <https://scikit-learn.org/stable/modules/generated/sklearn.compose.ColumnTransformer.html>`__
+    `ColumnTransformer <https://scikit-learn.org/stable/modules/generated/sklearn.compose.ColumnTransformer.html>`__.
 
     .. note::
         The parameter ``sparse_threshold`` of the super class is not supported.
 
     Parameters
     ----------
     transformers
         All transformers included in the list must be able to process
         :py:class:`TSCDataFrame`. See base class for the detailed specification of
         the tuple.
     """
 
     def __init__(
         self,
-        transformers: List[Tuple],
+        transformers: list[tuple],
         *,
         remainder="drop",
         n_jobs=None,
         transformer_weights=None,
-        verbose=False
+        verbose=False,
+        verbose_feature_names_out=True
     ):
-        super(TSCColumnTransformer, self).__init__(
+        super().__init__(
             transformers=transformers,
             remainder=remainder,
-            sparse_threshold=0.3,  # default value, will be ignored
+            sparse_threshold=0.3,  # default value, parameter ignored in TSCColumnTransformer
             transformer_weights=transformer_weights,
             n_jobs=n_jobs,
             verbose=verbose,
+            verbose_feature_names_out=verbose_feature_names_out,
         )
 
-    # @property
-    # def n_features_in_(self):
-    #     # this is only to make it explicit that this is already handled by the super class
-    #     return super(TSCColumnTransformer, self).n_features_in_
-
-    @property
-    def feature_names_in_(self):
-        check_is_fitted(self, "transformers_")
-        return self.transformers_[0][1].feature_names_in_
-
     @property
     def n_features_out_(self):
         check_is_fitted(self, "transformers_")
-        return sum([tr.n_features_out_ for _, tr, _ in self.transformers_])
-
-    @property
-    def feature_names_out_(self):
-        check_is_fitted(self, "transformers_")
-        indices = [tr.feature_names_out_ for _, tr, _ in self.transformers_]
-
-        for i in range(1, len(indices)):
-            indices[0] = indices[0].append(indices[i])
-            indices[i] = None
-
-        return indices[0]
+        return sum(tr.n_features_out_ for _, tr, _ in self.transformers_)
 
     def _hstack(self, Xs):
         if self.sparse_output_:
             raise NotImplementedError(
-                "Currently there is no support for sparse output in TSCColumnsTransformer"
+                "Currently there is no support for sparse output in TSCColumnTransformer."
             )
 
-        all_columns = pd.Index(np.hstack([df.columns.to_numpy() for df in Xs]))
-
-        if all_columns.has_duplicates:
-            # handle feature names in case of conflict
-            for i in range(len(self.transformers_)):
-                Xs[i] = Xs[i].add_prefix(self.transformers_[i][0] + "__")
-
         # dropna(axis=0) removes all rows that were dropped during transform
         # (i.e. transformations that require multiple timesteps).
-        return pd.concat(Xs, axis=1).dropna(axis=0)
+        Xs = pd.concat(Xs, axis=1, sort=True, ignore_index=True).dropna(axis=0)
+        Xs.columns = pd.Index(self.get_feature_names_out())
+        return Xs
 
     def fit(self, X: TransformType, y=None, **fit_params):
         X = self._validate_datafold_data(X)
         self._read_fit_params(attrs=None, fit_params=fit_params)
-        return super(TSCColumnTransformer, self).fit(X)
+        return super().fit(X)
+
+    def partial_fit(self, X, y=None, **fit_params):
+        if not hasattr(self, "transformers_"):
+            return self.fit(X, y, **fit_params)
+        else:
+            return self
```

### Comparing `datafold-1.1.6/datafold/dynfold/dmap.py` & `datafold-2.0.0/datafold/dynfold/dmap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 import sys
 import warnings
-from typing import List, Optional, Tuple, Union
+from copy import deepcopy
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import scipy.linalg
 import scipy.sparse
 import scipy.sparse.linalg
 import scipy.spatial
 from sklearn.base import BaseEstimator
 from sklearn.utils import resample
 from sklearn.utils.validation import check_is_fitted, check_scalar
 
 from datafold.dynfold.base import TransformType, TSCTransformerMixin
-from datafold.pcfold import DmapKernelFixed, PCManifold, TSCDataFrame
-from datafold.pcfold.eigsolver import NumericalMathError, compute_kernel_eigenpairs
+from datafold.pcfold import DmapKernelFixed, TSCDataFrame
+from datafold.pcfold.eigsolver import (
+    NumericalMathError,
+    compute_kernel_eigenpairs,
+    compute_kernel_svd,
+)
 from datafold.pcfold.kernels import (
-    BaseManifoldKernel,
     DmapKernelVariable,
     GaussianKernel,
     KernelType,
     PCManifoldKernel,
+    RoselandKernel,
     TSCManifoldKernel,
 )
 from datafold.utils.general import (
     df_type_and_indices_from,
     diagmat_dot_mat,
-    if1dim_colvec,
     mat_dot_diagmat,
     random_subsample,
 )
 
 
 class _DmapKernelAlgorithms:
     """Collection of re-useable algorithms that appear in models that have a diffusion
     map kernel.
 
     See Also
     --------
-
     :class:`.DiffusionMaps`
     :class:`.DiffusionMapsVariable`
     :class:`.GeometricHarmonicsInterpolator`
     """
 
     @staticmethod
     def solve_eigenproblem(
+        kernel,
         kernel_matrix: KernelType,
         n_eigenpairs: int,
-        is_symmetric: bool,
-        is_stochastic: bool,
-        basis_change_matrix: Optional[scipy.sparse.dia_matrix],
         index_from: Optional[TSCDataFrame] = None,
-    ) -> Tuple[np.ndarray, Union[np.ndarray, TSCDataFrame]]:
-
+    ) -> tuple[np.ndarray, Union[np.ndarray, TSCDataFrame]]:
         if isinstance(kernel_matrix, pd.DataFrame):
             kernel_matrix = kernel_matrix.to_numpy()
 
         try:
             eigvals, eigvect = compute_kernel_eigenpairs(
+                kernel=kernel,
                 kernel_matrix=kernel_matrix,  # from here on only ndarray
                 n_eigenpairs=n_eigenpairs,
-                is_symmetric=is_symmetric,
-                is_stochastic=is_stochastic,
                 # only normalize after potential basis change
                 normalize_eigenvectors=False,
                 backend="scipy",
+                validate_matrix=False,
             )
 
         except NumericalMathError:
             # re-raise with more details for DMAP kernel
             raise_numerical_error = True
         else:
             max_imag_eigvect = np.abs(np.imag(eigvect)).max()
@@ -87,16 +87,16 @@
                 f"parameter 'symmetrize_kernel=True' (improves numerical stability) and "
                 f"only if this is not working adjust kernel settings."
             )
         else:
             eigvals = np.real(eigvals)
             eigvect = np.real(eigvect)
 
-        if basis_change_matrix is not None:
-            eigvect = basis_change_matrix @ eigvect
+        if kernel.basis_change_matrix_ is not None:
+            eigvect = kernel.basis_change_matrix_ @ eigvect
 
         eigvect /= np.linalg.norm(eigvect, axis=0)[np.newaxis, :]
 
         if index_from is not None:
             eigvect = TSCDataFrame.from_same_indices_as(
                 index_from,
                 eigvect,
@@ -112,41 +112,39 @@
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Transform a kernel matrix obtained from a symmetric conjugate
         transformation to the diffusion kernel matrix.
 
         The conjugate relationship is as follows
 
         .. math::
-            A = D^{1/2} K D^{-1/2}
+            A = D^{1/2} K D^{-1/2},
 
-        , where :math:`A` is the symmetric matrix, conjugate to the "true" Markov
-        matrix :math:`K`. To recover :math:`K` the following operation is performed
+        where matrix :math:`A` is the symmetric matrix, conjugate to the "true" stochastic
+        Markov matrix :math:`K`. To recover :math:`K` the following operation is performed
 
         .. math::
             K = D^{-1/2} A D^{1/2}
 
-        Note, that the ``basis_change_matrix``, is already :math:`D^{-1/2}`.
-        See also reference :cite:`rabin_heterogeneous_2012` and function
-        :py:meth:`_conjugate_stochastic_kernel_matrix` in ``kernels.py`` for further
-        infos.
+        Note, that the ``basis_change_matrix`` is already :math:`D^{-1/2}`.
+        See also reference :cite:`rabin-2012` and function
+        :py:meth:`_conjugate_stochastic_kernel_matrix` in ``kernels.py``.
 
         Parameters
         ----------
         kernel_matrix
             Symmetric conjugate kernel matrix of shape `(n_samples, n_samples)`
 
         basis_change_matrix
             Diagonal elements of basis change matrix :math:`D^{-1/2}`
 
         Returns
         -------
         numpy.ndarray
             Generally non-symmetric matrix of same shape and type as `kernel_matrix`.
         """
-
         if isinstance(kernel_matrix, TSCDataFrame):
             row_idx, col_idx = kernel_matrix.index, kernel_matrix.columns
         else:
             row_idx, col_idx = None, None
 
         inv_basis_change_matrix = scipy.sparse.diags(
             np.reciprocal(basis_change_matrix.data.ravel())
@@ -182,71 +180,64 @@
 
     time_exponent
         The time of the diffusion process (exponent of eigenvalues in embedding). The
         value can be changed after the model is fit.
 
     is_stochastic
         If True, the diffusion kernel matrix is normalized (row stochastic). In the
-        standard definition this has to be True.
+        standard definition of diffusion maps the parameter has to be True.
 
     alpha
         The degree of re-normalization between `(0,1)`. Setting ``alpha=1`` corrects
         the sampling density in the data as an artifact of the collection process.
-        Special values are (see :cite:`coifman_diffusion_2006`)
+        Special values are (see :cite:t:`coifman-2006`)
 
         * `alpha=0` Graph Laplacian,
         * `alpha=0.5` Fokker-Plank operator,
         * `alpha=1` Laplace-Beltrami operator
 
         Note, that ``is_stochastic=True`` is required in all three cases.
 
     symmetrize_kernel
         If True, a symmetric conjugate transformation is performed, if the kernel
         matrix is non-symmetric (otherwise the parameter has no effect). The symmetric
         conjugate improves numerical stability when solving the eigenvectors, because it
         allows using algorithms designed for (sparse) Hermitian matrices.
 
-    dist_kwargs
-        Keyword arguments passed to the internal distance matrix computation. See
-        :py:meth:`datafold.pcfold.distance.compute_distance_matrix` for parameter
-        arguments.
 
     Attributes
     ----------
-
-    X_fit_: Untion[PCManifold, TSCDataFrame]
-        The training data during fit. The data is required for out-of-sample mappings;
-        the object is equipped with kernel :py:class:`DmapKernelFixed`;
-        ``np.asarray(X_fit_)`` casts the object to a standard numpy array.
+    X_fit_: Union[numpy.ndarray, pandas.DataFrame, TSCDataFrame]
+        The training data `X` passed during `fit`. The data is required for out-of-sample
+        mappings in the Nyström extension.
 
     eigenvalues_ : numpy.ndarray
         The eigenvalues of diffusion kernel matrix in decreasing order.
 
-    eigenvectors_: TSCDataFrame, pandas.DataFrame, numpy.ndarray
+    eigenvectors_: Union[np.ndarray, pd.DataFrame, TSCDataFrame]
         The eigenvectors of the kernel matrix.
 
     target_coords_: numpy.ndarray
         The coordinate indices to map to when transforming the data. The target point
         dimension equals the number of indices included in `target_coords_`. Note that the
-        attributes `eigenvectors_` and `eigenvalues_` sill contain *all* computed
+        attributes `eigenvectors_` and `eigenvalues_` still contain *all* computed
         eigenpairs.
 
     inv_coeff_matrix_: numpy.ndarray
         The coefficient matrix to map points from embedding space back to state space.
         The computation is delayed until `inverse_transform` is called for the first
         time (only then the attribute is available).
 
     kernel_matrix_ : Union[numpy.ndarray, scipy.sparse.csr_matrix]
         The computed kernel matrix; the matrix is only stored if
         ``store_kernel_matrix=True`` is set during :py:meth:`.fit`.
 
     References
     ----------
-    :cite:`lafon_diffusion_2004`
-    :cite:`coifman_diffusion_2006`
+    :cite:`lafon-2004,coifman-2006`
     """
 
     _cls_valid_operator_names = (
         "laplace_beltrami",
         "fokker_planck",
         "graph_laplacian",
         "rbf",
@@ -257,24 +248,21 @@
         kernel: Optional[Union[PCManifoldKernel, TSCManifoldKernel]] = None,
         *,  # keyword-only
         n_eigenpairs: int = 10,
         time_exponent: float = 0,
         is_stochastic: bool = True,
         alpha: float = 1,
         symmetrize_kernel: bool = True,
-        dist_kwargs=None,
     ) -> None:
-
         self.kernel = kernel
         self.n_eigenpairs = n_eigenpairs
         self.time_exponent = time_exponent
         self.is_stochastic = is_stochastic
         self.alpha = alpha
         self.symmetrize_kernel = symmetrize_kernel
-        self.dist_kwargs = dist_kwargs
 
         # mypy
         self.eigenvalues_: np.ndarray
         self.eigenvectors_: np.ndarray
 
     @classmethod
     def laplace_beltrami(
@@ -361,45 +349,44 @@
             max_val=1,
         )
 
     def _get_default_kernel(self):
         return GaussianKernel(epsilon=1.0)
 
     def _nystrom(self, kernel_cdist, eigvec, eigvals, index_from):
-
         if isinstance(kernel_cdist, pd.DataFrame):
             _kernel_cdist = kernel_cdist.to_numpy()
         else:
             _kernel_cdist = kernel_cdist
 
         _magic_tol = 1e-15  # need to adapt if not sufficient
         if (np.abs(eigvals) < _magic_tol).any():
             warnings.warn(
                 "Diffusion map eigenvalues are close to zero, which can cause "
-                "numerical instabilities when applying the Nystroem extension."
+                "numerical instabilities when applying the Nystroem extension.",
+                stacklevel=2,
             )
 
         # Nystroem approximation
         approx_eigenvectors = _kernel_cdist @ mat_dot_diagmat(
             eigvec, np.reciprocal(eigvals)
         )
 
         if index_from is not None:
             approx_eigenvectors = df_type_and_indices_from(
                 index_from,
                 values=approx_eigenvectors,
-                except_columns=[f"ev{i}" for i in range(self.n_eigenpairs)],
+                except_columns=self.get_feature_names_out(),
             )
 
         return approx_eigenvectors
 
     def _perform_dmap_embedding(
         self, eigenvectors: Union[np.ndarray, pd.DataFrame]
     ) -> Union[np.ndarray, pd.DataFrame]:
-
         check_scalar(
             self.time_exponent,
             "time_exponent",
             target_type=(float, np.floating, int, np.integer),
         )
 
         if self.time_exponent == 0:
@@ -408,77 +395,53 @@
             eigvals_time = np.power(self.eigenvalues_, self.time_exponent)
             dmap_embedding = mat_dot_diagmat(np.asarray(eigenvectors), eigvals_time)
 
         if isinstance(eigenvectors, pd.DataFrame):
             dmap_embedding = df_type_and_indices_from(
                 indices_from=eigenvectors,
                 values=dmap_embedding,
-                except_columns=self.feature_names_out_,
+                except_columns=self.get_feature_names_out(),
             )
 
         return dmap_embedding
 
-    def _feature_names(self):
-        if hasattr(self, "target_coords_"):
-            feature_names = pd.Index(
-                [f"dmap{i}" for i in self.target_coords_],
-                name=TSCDataFrame.tsc_feature_col_name,
-            )
-        else:
-            feature_names = pd.Index(
-                [f"dmap{i}" for i in range(self.n_eigenpairs)],
-                name=TSCDataFrame.tsc_feature_col_name,
-            )
-
-        return feature_names
-
-    def _setup_default_dist_kwargs(self):
-        from copy import deepcopy
-
-        self.dist_kwargs_ = deepcopy(self.dist_kwargs) or {}
-        self.dist_kwargs_.setdefault("cut_off", np.inf)
-        self.dist_kwargs_.setdefault("kmin", 0)
-        self.dist_kwargs_.setdefault("backend", "guess_optimal")
-
     def _select_eigenpairs_target_coords(self):
         """Returns either
         * all eigenpairs, or
-        * the ones that were selected during set_target_coords
+        * the ones that were selected during set_target_coords.
 
         It is assumed that the model is already fit.
         """
-
         if hasattr(self, "target_coords_"):
             if isinstance(self.eigenvectors_, pd.DataFrame):
                 eigvec = self.eigenvectors_.iloc[:, self.target_coords_]
             else:
                 eigvec = self.eigenvectors_[:, self.target_coords_]
 
             eigvals = self.eigenvalues_[self.target_coords_]
         else:
             eigvec, eigvals = self.eigenvectors_, self.eigenvalues_
         return eigvec, eigvals
 
     def set_target_coords(
-        self, indices: Union[np.ndarray, List[int]]
+        self, indices: Union[np.ndarray, list[int]]
     ) -> "DiffusionMaps":
         """Set eigenvector coordinates for parsimonious mapping.
 
         Parameters
         ----------
         indices
             Index values of eigenpairs (``eigenvalues_`` and ``eigenvectors_``) to map
             new points to.
 
         Returns
         -------
         DiffusionMaps
             self
         """
-
         indices = np.asarray(indices)
         indices = np.sort(indices)
 
         if indices.dtype != int:
             raise TypeError(f"The indices must be integers. Got type {indices.dtype}.")
 
         if indices[0] < 0 or indices[-1] >= self.n_eigenpairs:
@@ -486,26 +449,32 @@
                 f"Indices {indices} are out of bound. Only integer values "
                 f"in [0, {self.n_eigenpairs}] are allowed."
             )
 
         self.target_coords_ = indices
 
         self.n_features_out_ = len(self.target_coords_)
-        if hasattr(self, "feature_names_out_") and self.feature_names_out_ is not None:
-            self.feature_names_out_ = self._feature_names()
 
         return self
 
+    def get_feature_names_out(self, input_features=None):
+        if hasattr(self, "target_coords_"):
+            feature_names = np.array([f"dmap{i}" for i in self.target_coords_])
+        else:
+            feature_names = np.array([f"dmap{i}" for i in range(self.n_eigenpairs)])
+
+        return feature_names
+
     def fit(
         self,
         X: TransformType,
         y=None,
         **fit_params,
     ) -> "DiffusionMaps":
-        """Compute diffusion kernel matrix and its' eigenpairs.
+        """Fit the model by computing the eigenpairs of the diffusion kernel matrix.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data of shape `(n_samples, n_features)`.
 
         y: None
@@ -520,105 +489,84 @@
         DiffusionMaps
             self
         """
         self._validate_settings()
 
         X = self._validate_datafold_data(
             X=X,
-            array_kwargs=dict(ensure_min_samples=max(2, self.n_eigenpairs)),
-            tsc_kwargs=dict(ensure_min_samples=max(2, self.n_eigenpairs)),
+            ensure_min_samples=max(2, self.n_eigenpairs),
         )
 
-        self._setup_feature_attrs_fit(X, features_out=self._feature_names())
+        self._setup_feature_attrs_fit(X)
 
-        store_kernel_matrix = self._read_fit_params(
-            attrs=[("store_kernel_matrix", False)],
+        store_kernel_matrix, kernel_kwargs = self._read_fit_params(
+            attrs=[("store_kernel_matrix", False), ("kernel_kwargs", {})],
             fit_params=fit_params,
         )
 
-        self._setup_default_dist_kwargs()
-
-        # Note the DmapKernel is a kernel that wraps another kernel to provides the
-        # DMAP specific functionality.
+        # The DmapKernel is a meta-kernel that wraps another (internal) kernel to provide
+        # the specific normalizations in Diffusion Maps.
+        # deepcopy to performed to not mutate the original self.kernel attribute (this is
+        # according to sklearn's rules)
+        # TODO: no default kernel? Or use np.median for default kernel...
         internal_kernel = (
-            self.kernel if self.kernel is not None else self._get_default_kernel()
+            deepcopy(self.kernel)
+            if self.kernel is not None
+            else self._get_default_kernel()
         )
 
         self._dmap_kernel = DmapKernelFixed(
             internal_kernel=internal_kernel,
             is_stochastic=self.is_stochastic,
             alpha=self.alpha,
             symmetrize_kernel=self.symmetrize_kernel,
         )
 
-        if isinstance(X, TSCDataFrame):
-            self.X_fit_ = TSCDataFrame(
-                X, kernel=self._dmap_kernel, dist_kwargs=self.dist_kwargs_
-            )
-        elif isinstance(X, (np.ndarray, pd.DataFrame)):
-            self.X_fit_ = PCManifold(
-                X,
-                kernel=self._dmap_kernel,
-                dist_kwargs=self.dist_kwargs_,
-            )
-
-        kernel_output = self.X_fit_.compute_kernel_matrix()
-        (
-            kernel_matrix_,
-            self._cdist_kwargs,
-            ret_extra,
-        ) = PCManifoldKernel.read_kernel_output(kernel_output=kernel_output)
-
-        # if key is not present, this is a bug. The value for the key can also be None.
-        basis_change_matrix = ret_extra["basis_change_matrix"]
+        self.X_fit_ = X
+        kernel_matrix_ = self._dmap_kernel(X=X, **kernel_kwargs)
 
         # choose object to copy time information from, if applicable
         if isinstance(kernel_matrix_, TSCDataFrame):
             # if possible take time index from kernel_matrix (especially
             # dynamics-adapted kernels can drop samples from X)
             index_from: Optional[TSCDataFrame] = kernel_matrix_
         elif (
             isinstance(self.X_fit_, TSCDataFrame)
             and kernel_matrix_.shape[0] == self.X_fit_.shape[0]
         ):
             # if kernel is numpy.ndarray or scipy.sparse.csr_matrix, but X_fit_ is a time
-            # series, then take incides from X_fit_ -- this only works if no samples are
-            # dropped in the kernel computation.
+            # series, then take indexes from X_fit_ -- this only works if no samples are
+            # dropped in the kernel computation (such as in ConeKernel where the time
+            # derivative is computed)
             index_from = self.X_fit_
         else:
             index_from = None
 
         (
             self.eigenvalues_,
             self.eigenvectors_,
         ) = _DmapKernelAlgorithms.solve_eigenproblem(
+            kernel=self._dmap_kernel,
             kernel_matrix=kernel_matrix_,
             n_eigenpairs=self.n_eigenpairs,
-            is_symmetric=self._dmap_kernel.is_symmetric,
-            is_stochastic=self.is_stochastic,
-            basis_change_matrix=basis_change_matrix,
             index_from=index_from,
         )
 
-        # TODO: warning if less self.eigenvalues_ than n_eigenpairs?
-        #  happens if square kernel has less entries than n_eigenpairs
-
-        if self._dmap_kernel.is_symmetric_transform() and store_kernel_matrix:
+        if self._dmap_kernel.is_conjugate and store_kernel_matrix:
             kernel_matrix_ = _DmapKernelAlgorithms.unsymmetric_kernel_matrix(
                 kernel_matrix=kernel_matrix_,
-                basis_change_matrix=basis_change_matrix,
+                basis_change_matrix=self._dmap_kernel.basis_change_matrix_,
             )
 
         if store_kernel_matrix:
             self.kernel_matrix_ = kernel_matrix_
 
         return self
 
     def transform(self, X: TransformType) -> TransformType:
-
         r"""Embed out-of-sample points with Nyström extension.
 
         From solving the eigenproblem of the diffusion kernel :math:`K`
         (:class:`.DmapKernelFixed`)
 
         .. math::
             K(X,X) \Psi = \Psi \Lambda
@@ -628,44 +576,41 @@
         .. math::
             K(X, Y) \Psi \Lambda^{-1} = \Psi
 
         where :math:`K(X, Y)` is a component-wise evaluation of the kernel.
 
         Note, that the Nyström mapping can be used for image mappings irrespective of
         whether the computed kernel matrix :math:`K(X,X)` is symmetric.
-        For details on this see :cite:`fernandez_diffusion_2015` (especially equation 5).
+        For details on this see :cite:t:`fernandez-2015` (especially Eq. 5).
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Data points of shape `(n_samples, n_features)` to be embedded.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_coords)`
         """
         check_is_fitted(self, ("X_fit_", "eigenvalues_", "eigenvectors_"))
 
-        X = self._validate_datafold_data(X, array_kwargs=dict(ensure_min_samples=1))
+        X = self._validate_datafold_data(X)
         self._validate_feature_input(X, direction="transform")
 
-        kernel_output = self.X_fit_.compute_kernel_matrix(X, **self._cdist_kwargs)
-        kernel_matrix_cdist, _, _ = PCManifoldKernel.read_kernel_output(
-            kernel_output=kernel_output
-        )
+        kernel_matrix_cdist = self._dmap_kernel(self.X_fit_, X)
 
-        # choose object to copy time information from, if applicable
+        # choose object to copy time information from
         if isinstance(kernel_matrix_cdist, TSCDataFrame):
             # if possible take time index from kernel_matrix (especially
             # dynamics-adapted kernels can drop samples from X)
             index_from: Optional[TSCDataFrame] = kernel_matrix_cdist
         elif isinstance(X, TSCDataFrame) and kernel_matrix_cdist.shape[0] == X.shape[0]:
             # if kernel is numpy.ndarray or scipy.sparse.csr_matrix, but X_fit_ is a time
-            # series, then take incides from X_fit_ -- this only works if no samples are
+            # series, then take indices from X_fit_ -- this only works if no samples are
             # dropped in the kernel computation.
             index_from = X
         else:
             index_from = None
 
         eigvec, eigvals = self._select_eigenpairs_target_coords()
 
@@ -675,15 +620,15 @@
             eigvals=eigvals,
             index_from=index_from,
         )
 
         return self._perform_dmap_embedding(eigvec_nystroem)
 
     def fit_transform(self, X: TransformType, y=None, **fit_params) -> TransformType:
-        """Compute diffusion map from data and apply embedding on same data.
+        """Fit model with data and apply embedding on same data.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data of shape `(n_samples, n_features)`
 
         y: None
@@ -693,23 +638,22 @@
             See `fit` method for additional parameter.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_eigenpairs)`
         """
-
-        X = self._validate_datafold_data(X, array_kwargs=dict(ensure_min_samples=2))
+        X = self._validate_datafold_data(X, ensure_min_samples=2)
         self.fit(X=X, y=y, **fit_params)
 
         eigvec, _ = self._select_eigenpairs_target_coords()
         return self._perform_dmap_embedding(eigvec)
 
     def inverse_transform(self, X: TransformType) -> TransformType:
-        """Pre-image from embedding space back to original (ambient) space.
+        """Perform pre-image by mapping data from embedding space back to ambient space.
 
         .. note::
             Currently, this is only a linear map in a least squares sense. Overwrite
             this function for more advanced pre-image mappings.
 
         Parameters
         ----------
@@ -718,15 +662,14 @@
             map from embedding space to original space.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape (`n_samples, n_features)`
         """
-
         check_is_fitted(self)
         X = self._validate_datafold_data(X)
         self._validate_feature_input(X, direction="inverse_transform")
 
         if not hasattr(self, "inv_coeff_matrix_"):
             if isinstance(self.X_fit_, pd.DataFrame):
                 # happens if samples were dropped during kernel fit
@@ -737,43 +680,45 @@
             eigvec, _ = self._select_eigenpairs_target_coords()
 
             self.inv_coeff_matrix_ = scipy.linalg.lstsq(
                 np.asarray(eigvec), _X, cond=None
             )[0]
 
         X_orig_space = np.asarray(X) @ self.inv_coeff_matrix_
-        return self._same_type_X(
-            X, values=X_orig_space, feature_names=self.feature_names_in_
-        )
+
+        try:
+            feature_names = self.feature_names_in_
+        except AttributeError:
+            feature_names = None
+
+        return self._same_type_X(X, values=X_orig_space, feature_names=feature_names)
 
 
 class DiffusionMapsVariable(BaseEstimator, TSCTransformerMixin):  # pragma: no cover
     """(experimental, not documented)
     .. warning::
         This class is not documented. Contributions are welcome
             * documentation
-            * unit- or functional-testing
+            * unit- or functional-testing.
 
     References
     ----------
-    :cite:`berry_nonparametric_2015`
-    :cite:`berry_variable_2016`
+    :cite:`berry-2015,berry-2016`
 
     """
 
     def __init__(
         self,
         epsilon=1.0,
         *,  # keyword-only
         n_eigenpairs=10,
         nn_bandwidth=10,
         expected_dim=2,
         beta=-0.5,
         symmetrize_kernel=False,
-        dist_kwargs=None,
     ):
         self.epsilon = epsilon
         self.n_eigenpairs = n_eigenpairs
         self.expected_dim = expected_dim
         self.beta = beta
         self.nn_bandwidth = nn_bandwidth
 
@@ -784,116 +729,542 @@
             epsilon=self.epsilon,
             k=nn_bandwidth,
             expected_dim=expected_dim,
             beta=beta,
             symmetrize_kernel=symmetrize_kernel,
         )
         self.alpha = self.dmap_kernel_.alpha  # is computed (depends on beta) in kernel
-        self.dist_kwargs = dist_kwargs
 
     @property
     def peq_est_(self):
         """Estimation of the equilibrium density (p_eq)."""
-
         #  TODO: there are different suggestions,
         #    q_eps_s as noted pdfp. 5,  OR  eq. (2.3) pdfp 4 rho \approx peq^(-1/2)
 
-        nr_samples = self.q_eps_s_.shape[0]
-        return self.q_eps_s_ / (
+        nr_samples = self.dmap_kernel_.q_eps_s_.shape[0]
+        return self.dmap_kernel_.q_eps_s_ / (
             nr_samples * (4 * np.pi * self.epsilon) ** (self.expected_dim / 2)
         )
 
-    def fit(self, X: TransformType, y=None, **fit_params):
-
-        X = self._validate_datafold_data(X, array_kwargs=dict(ensure_min_samples=2))
-
-        self._setup_feature_attrs_fit(
-            X, features_out=[f"dmap{i}" for i in range(self.n_eigenpairs)]
-        )
+    def get_feature_names_out(self, input_features=None):
+        return np.array([f"dmap{i}" for i in range(self.n_eigenpairs)])
 
+    def fit(self, X: TransformType, y=None, **fit_params):
+        X = self._validate_datafold_data(X, ensure_min_samples=2)
+        self._setup_feature_attrs_fit(X)
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
-        self.dist_kwargs = self.dist_kwargs or {}
-        self.dist_kwargs.setdefault("cut_off", np.inf)
-        self.dist_kwargs.setdefault("kmin", self.nn_bandwidth)
-        self.dist_kwargs.setdefault("backend", "guess_optimal")
-
-        pcm = PCManifold(
-            X,
-            kernel=self.dmap_kernel_,
-            dist_kwargs=self.dist_kwargs,
-        )
-
-        # basis_change_matrix is None if not required
-        (
-            self.operator_matrix_,
-            _basis_change_matrix,
-            self.rho0_,
-            self.rho_,
-            self.q0_,
-            self.q_eps_s_,
-        ) = pcm.compute_kernel_matrix()
+        self.generator_matrix_ = self.dmap_kernel_(X=X)
 
         (
             self.eigenvalues_,
             self.eigenvectors_,
         ) = _DmapKernelAlgorithms.solve_eigenproblem(
-            kernel_matrix=self.operator_matrix_,
+            kernel=self.dmap_kernel_,
+            kernel_matrix=self.generator_matrix_,
             n_eigenpairs=self.n_eigenpairs,
-            is_symmetric=self.dmap_kernel_.is_symmetric,
-            is_stochastic=True,
-            basis_change_matrix=_basis_change_matrix,
         )
 
         # TODO: note here the kernel is actually NOT the kernel but the operator matrix
         #  ("L") -> see "Variable bandwidth diffusion maps" by Berry et al.
         #  Maybe think about a way to transform this?
 
         if self.dmap_kernel_.is_symmetric_transform(is_pdist=True):
-            self.operator_matrix_ = _DmapKernelAlgorithms.unsymmetric_kernel_matrix(
-                kernel_matrix=self.operator_matrix_,
-                basis_change_matrix=_basis_change_matrix,
+            self.generator_matrix_ = _DmapKernelAlgorithms.unsymmetric_kernel_matrix(
+                kernel_matrix=self.generator_matrix_,
+                basis_change_matrix=self.dmap_kernel_.basis_change_matrix_,
             )
 
         # TODO: transformation to match eigenvalues with true kernel matrix.
         self.eigenvalues_ = np.power(
             self.eigenvalues_, 1 / self.epsilon, out=self.eigenvalues_
         )
 
         # assumes that the eigenvectors are already normed to 1
         #   (which is the default)
         self.eigenvectors_ = np.multiply(
             self.eigenvectors_, np.sqrt(X.shape[0]), out=self.eigenvectors_
         )
 
         self.eigenvectors_ = self._same_type_X(
-            X, values=self.eigenvectors_, feature_names=self.feature_names_out_
+            X, values=self.eigenvectors_, feature_names=self.get_feature_names_out()
         )
 
         return self
 
     def transform(self, X: TransformType):
         raise NotImplementedError(
             "A transform for out-of-sample points is currently "
             "not supported. This requires to implement the "
             "'cdist' case for the variable bandwidth diffusion "
             "maps kernel."
         )
 
     def fit_transform(self, X: TransformType, y=None, **fit_params):
         self.fit(X=X, y=y, **fit_params)
-        return self._same_type_X(X, self.eigenvectors_, self.feature_names_out_)
+        return self._same_type_X(X, self.eigenvectors_, self.get_feature_names_out())
+
+
+class Roseland(BaseEstimator, TSCTransformerMixin):
+    """Define a diffusion process on a point cloud by using a landmark set to find meaningful
+    geometric descriptions.
+
+    The model can be used for
+
+    * non-linear dimensionality reduction
+    * spectral clustering
+
+    Parameters
+    ----------
+    kernel
+        The kernel to describe similarity between points. A landmark-set affinity (kernel)
+        matrix is computed using it. The normalized kernel matrix is used to define the
+        diffusion process. Defaults to :py:class:`.GaussianKernel` with bandwidth `epsilon=1`.
+
+    n_svdtriplet
+        The number of singular value decomposition pairs (left singular vector, singular
+        value) to be computed from the normalized landmark-set affinity matrix.
+        The right singular vectors are also computed and their number is governed by
+        ``n_svdpairs``.
+
+    time_exponent
+        The time of the diffusion process (exponent of the singular values in the
+        embedding). The value can be changed after the model is fitted.
+
+    landmarks
+        The landmark set used for computing the landmark-set affinity matrix.
+        The strategy of how to choose the landmarks is determined by the type:
+
+        * a float in the interval (0,1] -- proportion of random set from `X` during
+          :py:meth:`fit`
+        * an integer > 1 -- the number of random samples from `X` during :py:meth:`fit`
+        * a `np.ndarray` containing the final landmark points
+
+    alpha
+        Normalization of the sampling density, indicated by a float in [0,1]. The
+        parameter corresponds to `alpha` in :py:meth:`DiffusionMaps`.
+
+        .. note::
+            The parameter is not covered in the original Roseland paper (corresponding to
+            `alpha=0`). Enabling the additional normalization (`alpha>0`) should therefore
+            be used with care.
+
+    random_state
+        Random seed for the selection of the landmark set. If provided when `Y` is also
+        given, it is ignored. When `Y` is not provided it is used for the subsampling of
+        the landmarks.
+
+    Attributes
+    ----------
+    landmarks_: np.ndarray
+        The final landmark data used. It is required for both in-sample and
+        out-of-sample embeddings.
+
+    svdvalues_ : numpy.ndarray
+        The singular values of the diffusion kernel matrix in decreasing order.
+
+    svdvec_left_: numpy.ndarray
+        The left singular vectors of the kernel matrix.
+
+    svdvec_right_: numpy.ndarray
+        The right singular vectors of the diffusion kernel matrix
+
+    target_coords_: numpy.ndarray
+        The coordinate indices to map to when transforming the data. The target point
+        dimension equals the number of indices included in `target_coords_`. Note that the
+        attributes `svdvalues_`, `svdvec_left_`, and `svdvec_right_` still contain *all*
+        computed `n_svdtriplet`.
+
+    kernel_matrix_ : Union[numpy.ndarray, scipy.sparse.csr_matrix]
+        The computed kernel matrix; the matrix is only stored if
+        ``store_kernel_matrix=True`` is set during :py:meth:`fit`.
+
+    References
+    ----------
+    :cite:`shen-2020`
+    """
+
+    def __init__(
+        self,
+        kernel: Optional[PCManifoldKernel] = None,
+        *,  # keyword-only
+        n_svdtriplet: int = 10,
+        time_exponent: float = 0,
+        landmarks: Union[float, int, np.ndarray] = 0.25,
+        alpha: float = 0,
+        random_state: Optional[int] = None,
+    ) -> None:
+        self.kernel = kernel
+        self.n_svdtriplet = n_svdtriplet
+        self.time_exponent = time_exponent
+        self.landmarks = landmarks
+        self.alpha = alpha
+        self.random_state = random_state
+
+        self.svdvalues_: np.ndarray
+        self.svdvec_left_: np.ndarray
+        self.svdvec_right_: np.ndarray
+
+    def _validate_setting(self, n_samples):
+        if isinstance(self.kernel, TSCManifoldKernel):
+            raise NotImplementedError(
+                "Kernels of type 'TSCManifoldKernel' are not supported yet"
+            )
+
+        check_scalar(
+            self.n_svdtriplet, "n_svdtriplet", target_type=(int, np.integer), min_val=1
+        )
+
+        check_scalar(
+            self.time_exponent,
+            "time_exponent",
+            target_type=(float, int, np.floating, np.integer),
+        )
+
+        if isinstance(self.landmarks, float):
+            check_scalar(
+                self.landmarks,
+                "landmarks",
+                target_type=float,
+                min_val=0.0,
+                max_val=1.0,
+                include_boundaries="right",
+            )
+        elif isinstance(self.landmarks, int):
+            check_scalar(
+                self.landmarks,
+                "landmarks",
+                target_type=int,
+                min_val=1,
+                max_val=n_samples,
+            )
+        elif isinstance(self.landmarks, np.ndarray):
+            pass  # will get checked later
+        else:
+            raise TypeError(
+                f"Type of parameter landmarks (={type(self.landmarks)}) "
+                "is not supported"
+            )
+
+    def _get_default_kernel(self):
+        return GaussianKernel(epsilon=1.0)
+
+    def _subsample_landmarks(self, X: Union[np.ndarray, TSCDataFrame]):
+        """Subsample landmarks from training data `X` when no `landmarks` are
+        provided.
+        """
+        if isinstance(self.landmarks, float):
+            n_landmarks = int(X.shape[0] * self.landmarks)
+        else:  # isinstance(self.landmarks, int):
+            n_landmarks = self.landmarks
+
+        if n_landmarks <= 1:
+            raise ValueError(
+                "The landmark set must contain at least two samples."
+                f"Got {n_landmarks} samples."
+            )
+
+        if n_landmarks == X.shape[0]:
+            landmarks = X.to_numpy() if isinstance(X, TSCDataFrame) else X
+        else:
+            landmarks, _ = random_subsample(
+                X.to_numpy() if isinstance(X, TSCDataFrame) else X,
+                n_landmarks,
+                random_state=self.random_state,
+            )
+
+        return landmarks
+
+    def _compute_kernel_svd(
+        self,
+        kernel_matrix: KernelType,
+        n_svdtriplet: int,
+        normalize_diagonal: Optional[np.ndarray] = None,
+        index_from: Optional[TSCDataFrame] = None,
+    ) -> tuple[np.ndarray, Union[np.ndarray, TSCDataFrame], np.ndarray]:
+        svdvec_left, svdvals, svdvec_right = compute_kernel_svd(
+            kernel_matrix=kernel_matrix, n_svdtriplet=n_svdtriplet
+        )
+
+        if normalize_diagonal is not None:
+            # Change coordinates of the left singular vectors by using the diagonal matrix
+            svdvec_left = diagmat_dot_mat(normalize_diagonal, svdvec_left)
+
+        if index_from is not None:
+            svdvec_left = TSCDataFrame.from_same_indices_as(
+                index_from,
+                svdvec_left,
+                except_columns=[f"sv{i}" for i in range(n_svdtriplet)],
+            )
+
+        # transpose such that the right SVD vectors (typically denoted as V) are row-wise
+        svdvec_right = svdvec_right.T
+        return svdvec_left, svdvals, svdvec_right
+
+    def _select_svdpairs_target_coords(self):
+        """Returns either
+        * all svd-triplets, or
+        * the ones that were selected during set_target_coords.
+
+        It is assumed that the model is already fit.
+        """
+        if hasattr(self, "target_coords_"):
+            svdvec_left = self.svdvec_left_[:, self.target_coords_]
+            svdvec_right = self.svdvec_right_[:, self.target_coords_]
+            svdvals = self.svdvalues_[self.target_coords_]
+        else:
+            svdvec_left, svdvals, svdvec_right = (
+                self.svdvec_left_,
+                self.svdvalues_,
+                self.svdvec_right_,
+            )
+        return svdvec_left, svdvals, svdvec_right
+
+    def _nystrom(self, kernel_cdist, svdvec_right, svdvals, normalize_diagonal):
+        _magic_tol = 1e-14  # tolerance to raise a warning
+
+        if (np.abs(svdvals) < _magic_tol).any():
+            warnings.warn(
+                "Roseland singular values are close to zero, which can cause "
+                "numerical instabilities when applying the Nystroem extension.",
+                stacklevel=2,
+            )
+
+        # Interpolate the svdvec_left with:
+        #    K = U @ S @ V^T
+        # --> U = K @ V @ S^{-1}
+        # Note that transposing V is sufficient for the inverse because the vectors in
+        # SVD are orthonormal
+        svdvec_left_interp = kernel_cdist @ mat_dot_diagmat(
+            svdvec_right, np.reciprocal(svdvals)
+        )
+
+        svdvec_left_interp = diagmat_dot_mat(normalize_diagonal, svdvec_left_interp)
+
+        return svdvec_left_interp
+
+    def _perform_roseland_embedding(
+        self, svdvectors: Union[np.ndarray, pd.DataFrame], svdvalues: np.ndarray
+    ) -> Union[np.ndarray, pd.DataFrame]:
+        check_scalar(
+            self.time_exponent,
+            "time_exponent",
+            target_type=(float, np.floating, int, np.integer),
+        )
+
+        if self.time_exponent == 0:
+            roseland_embedding = svdvectors
+        else:
+            svdvals_time = np.power(svdvalues, 2 * self.time_exponent)
+            roseland_embedding = mat_dot_diagmat(svdvectors, svdvals_time)
+
+        return roseland_embedding
+
+    def get_feature_names_out(self, input_features=None):
+        if hasattr(self, "target_coords_"):
+            feature_names = np.array([f"rose{i}" for i in self.target_coords_])
+        else:
+            feature_names = np.array([f"rose{i}" for i in range(self.n_svdtriplet)])
+
+        return feature_names
+
+    def set_target_coords(self, indices: Union[np.ndarray, list[int]]) -> "Roseland":
+        """Set specific singular vector coordinates for a parsimonious mapping.
+
+        Parameters
+        ----------
+        indices
+            Index values of svdpairs (``svdvalues_`` and ``svdvectors_``) to map
+            new points to.
+
+        Returns
+        -------
+        Roseland
+            self
+        """
+        indices = np.sort(np.asarray(indices))
+
+        if indices.dtype != int:
+            raise TypeError(f"The indices must be integers. Got type {indices.dtype}.")
+
+        if indices[0] < 0 or indices[-1] >= self.n_svdtriplet:
+            raise ValueError(
+                f"Indices {indices} are out of bound. Only integer values "
+                f"in [0, {self.n_svdtriplet}] are allowed."
+            )
+
+        self.target_coords_ = indices
+        self.n_features_out_ = len(self.target_coords_)
+
+        return self
+
+    def fit(
+        self,
+        X: TransformType,
+        y=None,
+        **fit_params,
+    ) -> "Roseland":
+        """Compute the Roseland kernel matrix and its singular vectors and values.
+
+        Parameters
+        ----------
+        X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
+            Training data.
+
+        y: None
+
+        **fit_params: Dict[str, object]
+            - store_kernel_matrix: ``bool``
+                If True, store the kernel matrix in attribute ``kernel_matrix``.
+
+        Returns
+        -------
+        Roseland
+            self
+        """
+        X = self._validate_datafold_data(
+            X=X, ensure_min_samples=max(2, self.n_svdtriplet)
+        )
+
+        store_kernel_matrix = self._read_fit_params(
+            attrs=[("store_kernel_matrix", False)],
+            fit_params=fit_params,
+        )
+
+        self._validate_setting(n_samples=X.shape[0])
+        self._setup_feature_attrs_fit(X)
+
+        if isinstance(self.landmarks, (int, float)):
+            self.landmarks_ = self._subsample_landmarks(X=X)
+        else:
+            self.landmarks_ = self.landmarks.view()
+
+        self.landmarks_ = self._validate_datafold_data(
+            X=self.landmarks_,
+            ensure_np=True,
+            ensure_min_samples=2,
+        )
+
+        if self.kernel is None:
+            self.kernel = self._get_default_kernel()
+
+        self.rose_kernel_ = RoselandKernel(
+            internal_kernel=self.kernel, alpha=self.alpha
+        )
+
+        kernel_matrix = self.rose_kernel_(self.landmarks_, X)
+
+        (
+            self.svdvec_left_,
+            self.svdvalues_,
+            self.svdvec_right_,
+        ) = self._compute_kernel_svd(
+            kernel_matrix=kernel_matrix,
+            n_svdtriplet=self.n_svdtriplet,
+            normalize_diagonal=self.rose_kernel_.normalize_diagonal_,
+            index_from=X if isinstance(X, TSCDataFrame) else None,
+        )
+
+        if store_kernel_matrix:
+            self.kernel_matrix_ = kernel_matrix
+
+        return self
+
+    def transform(self, X: TransformType) -> TransformType:
+        r"""Embed out-of-sample points with the Nyström extension:
+
+        .. math::
+
+            K(Y, X) V \Lambda^{-1} = U_{new}
+
+        where :math:`K(Y, X)` is a component-wise evaluation of the new kernel matrix,
+        :math:`V` the right singular vectors associated with the fitted model,
+        :math:`\Lambda` the singular values of the fitted model, and
+        :math:`U_{new}` the approximated left singular vectors of the (normalized) new
+        kernel matrix.
+
+        Parameters
+        ----------
+        X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
+            Out-of-sample points to embed.
+
+        Returns
+        -------
+        TSCDataFrame, pandas.DataFrame, numpy.ndarray
+            the new coordinates of the points in `X`
+        """
+        check_is_fitted(
+            self, ("landmarks_", "svdvalues_", "svdvec_left_", "svdvec_right_")
+        )
+
+        X = self._validate_datafold_data(X)
+        self._validate_feature_input(X, direction="transform")
+
+        kernel_matrix_cdist = self.rose_kernel_(self.landmarks_, X)
+
+        _, svdvals, svdvec_right = self._select_svdpairs_target_coords()
+
+        svdvec_left_interp = self._nystrom(
+            kernel_matrix_cdist,
+            svdvec_right=svdvec_right,
+            svdvals=svdvals,
+            normalize_diagonal=self.rose_kernel_.normalize_diagonal_,
+        )
+
+        roseland_embedding = self._perform_roseland_embedding(
+            svdvec_left_interp, svdvals
+        )
+
+        if isinstance(X, TSCDataFrame) and kernel_matrix_cdist.shape[0] == X.shape[0]:
+            roseland_embedding = TSCDataFrame.from_same_indices_as(
+                indices_from=X,
+                values=roseland_embedding,
+                except_columns=self.get_feature_names_out(),
+            )
+
+        return roseland_embedding
+
+    def fit_transform(self, X: TransformType, y=None, **fit_params) -> np.ndarray:
+        """Compute Roseland fit from data and apply embedding on the same data.
+
+        Parameters
+        ----------
+        X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
+            Training data.
+
+        y: None
+
+        **fit_params: Dict[str, object]
+            See `fit` method for additional parameter.
+
+        Returns
+        -------
+        TSCDataFrame, pandas.DataFrame, numpy.ndarray
+            the new coordinates of the points in X
+
+        """
+        self.fit(X=X, **fit_params)
+        svdvec_left, svdvals, _ = self._select_svdpairs_target_coords()
+
+        if isinstance(X, TSCDataFrame):
+            svdvec_left = TSCDataFrame.from_same_indices_as(
+                indices_from=X,
+                values=svdvec_left,
+                except_columns=self.get_feature_names_out(),
+            )
+
+        return svdvec_left
 
 
 class LocalRegressionSelection(BaseEstimator, TSCTransformerMixin):
     """Automatic selection of functional independent geometric harmonic vectors for
     parsimonious data manifold embedding.
 
-    To measure the functional dependency a local regression regression is performed: The
-    larger the residuals between eigenvetor sets the more information they add and are
+    To measure the functional dependency a local regression is performed: The
+    larger the residuals between eigenvector sets the more information they add and are
     therefore more likely to be considered in an embedding.
 
     The kernel used for the local linear regression has a scale of
 
     .. code::
 
         scale = bandwidth_type(distances) / eps_med_scale
@@ -928,23 +1299,21 @@
         "median" or "mean"
 
     random_state
         seed for random generator if the data is subsampled
 
     Attributes
     ----------
-
     evec_indices_
 
     residuals_
 
     References
     ----------
-
-    :cite:`dsilva_parsimonious_2018`
+    :cite:`dsilva-2018`
 
     """
 
     _cls_valid_strategy = ("dim", "threshold")
     _cls_valid_bandwidth = ("median", "mean")
 
     def __init__(
@@ -954,42 +1323,38 @@
         n_subsample=np.inf,
         strategy="dim",
         intrinsic_dim=2,
         regress_threshold=0.9,
         bandwidth_type="median",
         random_state: Optional[int] = None,
     ):
-
         self.strategy = strategy
 
         self.intrinsic_dim = intrinsic_dim
         self.regress_threshold = regress_threshold
         self.bandwidth_type = bandwidth_type
         self.random_state = random_state
 
         self.eps_med_scale = eps_med_scale
         self.n_subsample = n_subsample
 
     def _validate_parameter(self, num_eigenvectors):
-
         check_scalar(
             self.eps_med_scale,
             name="eps_med_scale",
             target_type=(float, np.floating, int, np.integer),
-            min_val=np.finfo(float).eps,  # exclusive zero
-            max_val=np.inf,
+            min_val=0,
         )
 
         if not np.isinf(self.n_subsample):
             check_scalar(
                 self.n_subsample,
                 name="n_subsample",
                 target_type=(int, np.integer),
                 min_val=1,
-                max_val=np.inf,
             )
 
         if self.strategy not in self._cls_valid_strategy:
             raise ValueError(f"strategy={self.strategy} is invalid.")
 
         if self.strategy == "dim":
             check_scalar(
@@ -1001,16 +1366,17 @@
             )
 
         if self.strategy == "threshold":
             check_scalar(
                 self.regress_threshold,
                 name="regress_threshold",
                 target_type=(float, np.floating),
-                min_val=np.finfo(float).eps,
-                max_val=1 - np.finfo(float).eps,
+                min_val=0,
+                max_val=1,
+                include_boundaries="neither",
             )
 
         if self.bandwidth_type not in self._cls_valid_bandwidth:
             raise ValueError(
                 f"Valid options for 'locregress_bandwidth_type' are "
                 f"{self._cls_valid_bandwidth}. Got: {self.bandwidth_type}"
             )
@@ -1119,22 +1485,21 @@
         #     (target_eigenvector - estimated_target_values) / error_scale))) /
         #     target_stddev
         # END
         ######
 
         # residual according to paper, equation 12  (also used in PCM code)
         residual = np.sqrt(
-            np.sum(np.square((target_eigenvector - estimated_target_values)))
+            np.sum(np.square(target_eigenvector - estimated_target_values))
             / np.sum(np.square(target_eigenvector))
         )
 
         return residual
 
     def _set_indices(self):
-
         # For the strategies numerical values are required. Therefore, set the first
         # residual (nan) here to the invalid value -1. This value makes sure, that
         # the first coordinate is always chosen.
         residuals = self.residuals_.copy()
         residuals[0] = -1
 
         # Strategy 1, according to user input:
@@ -1150,19 +1515,28 @@
                     np.argpartition(-residuals, self.intrinsic_dim)[
                         : self.intrinsic_dim
                     ]
                 )
 
         # User provides a threshold for the residuals. All eigenfunctions above this value
         # are included to parametrize the manifold.
-        else:  #  self.strategy == "threshold":
+        else:  # self.strategy == "threshold":
             self.evec_indices_ = np.sort(
                 np.where(residuals > self.regress_threshold)[0]
             )
 
+    def get_feature_names_out(self, input_features=None):
+        if input_features is None and not hasattr(self, "feature_names_in_"):
+            return np.array(self.evec_indices_, dtype=str)
+        else:
+            if input_features is not None:
+                return input_features[self.evec_indices_]
+            else:
+                return self.feature_names_in_[self.evec_indices_]
+
     def fit(self, X: TransformType, y=None, **fit_params) -> "LocalRegressionSelection":
         """Select indices according to strategy.
 
         Parameters
         ----------
         X
             Eigenvectors of shape `(n_samples, n_eigenvectors)` to make selection on.
@@ -1182,24 +1556,25 @@
         # are 2 loops, the inner loop runs over all samples, which could be
         # parallelized in a future work or by using numba.
 
         # NOTE: this saves self._transform_columns = X.columns
         # Later on not all of these columns are required because of the selection
         # performed.
 
-        X = self._validate_datafold_data(X, array_kwargs=dict(ensure_min_features=2))
+        X = self._validate_datafold_data(X, ensure_min_features=2)
         num_eigenvectors = X.shape[1]
 
         self._validate_parameter(num_eigenvectors)
 
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
         if not np.isinf(self.n_subsample):
+            X_numpy = X.to_numpy() if isinstance(X, TSCDataFrame) else X
             eigvec = resample(
-                X,
+                X_numpy,
                 replace=False,
                 n_samples=self.n_subsample,
                 random_state=self.random_state,
             )
         else:
             eigvec = np.asarray(X)
 
@@ -1210,57 +1585,49 @@
 
         for i in range(2, num_eigenvectors):
             self.residuals_[i] = self._single_residual_local_regression(
                 domain_eigenvectors=eigvec[:, 1:i], target_eigenvector=eigvec[:, i]
             )
 
         self._set_indices()
-
-        self._setup_feature_attrs_fit(
-            X,
-            features_out=X.columns[self.evec_indices_]
-            if isinstance(X, pd.DataFrame)
-            else len(self.evec_indices_),
-        )
+        self._setup_feature_attrs_fit(X)
 
         return self
 
     def transform(self, X: TransformType) -> TransformType:
         """Select parsimonious representation of full set of eigenvectors.
 
         Parameters
         ----------
-
         X
             Eigenvectors of shape `(n_samples, n_eigenvectors)` to carry out selection.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_evec_indices)`
         """
-
         X = self._validate_datafold_data(X)
         self._validate_feature_input(X, direction="transform")
 
         # choose eigenvectors
         X_selected = self._same_type_X(
             X,
             np.asarray(X)[:, self.evec_indices_],
-            feature_names=self.feature_names_out_,
+            feature_names=self.get_feature_names_out(),
         )
 
         return X_selected
 
     def inverse_transform(self, X: TransformType):
-        """
+        """n/a.
+
         .. warning::
             Not implemented.
         """
-
         # TODO: the inverse_transform should map
         #   \Psi_selected -> \Psi_full
         #  However this is usually not what we are interested in. Instead it is more
         #  likely that someone wants to do the inverse_transform like in DMAP:
         #   \Psi_selected -> X (original data).
 
         raise NotImplementedError(
```

### Comparing `datafold-1.1.6/datafold/dynfold/jsf.py` & `datafold-2.0.0/datafold/dynfold/jsf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,415 +1,352 @@
-from typing import Dict, List, Optional, Tuple, Union
+from copy import deepcopy
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import scipy.linalg
 import scipy.sparse
 import scipy.sparse.linalg
 from sklearn.base import BaseEstimator
+from sklearn.utils import check_scalar
 from sklearn.utils.validation import check_is_fitted
 
 from datafold.dynfold.base import TransformType, TSCTransformerMixin
-from datafold.pcfold import PCManifold, TSCDataFrame
-from datafold.pcfold.eigsolver import compute_kernel_eigenpairs
-from datafold.pcfold.kernels import GaussianKernel, PCManifoldKernel
+from datafold.pcfold import TSCDataFrame
+from datafold.pcfold.eigsolver import compute_kernel_eigenpairs, compute_kernel_svd
+from datafold.pcfold.kernels import BaseManifoldKernel
 from datafold.utils.general import mat_dot_diagmat
 
 
-# TODO: replace with datafold.utils.general.sort_eigenpairs
-#  -- Note that one sorts abs. values, the other complex values directly
-def sort_eigensystem(eigenvalues, eigenvectors):
-    idx = np.argsort(np.abs(eigenvalues))[::-1]
-    sorted_eigenvalues = eigenvalues[idx]
-    if isinstance(eigenvectors, pd.DataFrame):
-        sorted_eigenvectors = eigenvectors.iloc[:, idx]
-    else:
-        sorted_eigenvectors = eigenvectors[:, idx]
-    return sorted_eigenvalues, sorted_eigenvectors
-
-
-class JsfDataset:
-    """`JsfDataset` does the slicing of multimodal data. This is needed, as `.fit`,
-    `.transform`, and `.fit_transform` of `JointlySmoothFunctions` accept a single
-    data array `X`. Thus, the multimodal data is passed in as a single array and is
-    then separated inside the methods.
+class JointlySmoothFunctions(BaseEstimator, TSCTransformerMixin):
+    """Compute jointly smooth functions on multimodal data.
 
     Parameters
     ----------
-    name
-        The name of the dataset.
-
-    columns
-        The columns that correspond to the dataset.
-
-    kernel
-        The (optional) kernel for the dataset.
-
-    result_scaling
-        The (optional) result scaling for the parameter optimization.
-
-    dist_kwargs
-        Keyword arguments passed to the internal distance matrix computation. See
-        :py:meth:`datafold.pcfold.distance.compute_distance_matrix` for parameter
-        arguments.
-    """
-
-    def __init__(
-        self,
-        name: Optional[str] = None,
-        columns: Optional[slice] = None,
-        kernel: Optional[PCManifoldKernel] = None,
-        result_scaling: float = 1.0,
-        **dist_kwargs,
-    ):
-        self.name = name
-        self.columns = columns
-        self.kernel = kernel
-        self.result_scaling = result_scaling
-        self.dist_kwargs = dist_kwargs
-
-    def extract_from(self, X: TransformType) -> Union[TSCDataFrame, PCManifold]:
-        if self.columns:
-            if isinstance(X, pd.DataFrame) or isinstance(X, TSCDataFrame):
-                data = X.iloc[:, self.columns]
-            else:
-                data = X[:, self.columns]
-        else:
-            data = X
-
-        if isinstance(data, TSCDataFrame):
-            if self.kernel is None:
-                self.kernel = GaussianKernel()
-            data = TSCDataFrame(data, kernel=self.kernel, dist_kwargs=self.dist_kwargs)
-        elif isinstance(data, (np.ndarray, pd.DataFrame)):
-            data = PCManifold(
-                data=data, kernel=self.kernel, dist_kwargs=self.dist_kwargs
-            )
-            if self.kernel is None:
-                data.optimize_parameters(
-                    inplace=True, result_scaling=self.result_scaling
-                )
-
-        return data
-
-
-class _ColumnSplitter:
-    """Uses a `JsfDataset` list to split up a single data array X into a `PCManifold` list.
-
-    Parameters
-    ----------
-    datasets
-        The `JsfDataset`s used to split up the array X.
-    """
-
-    def __init__(self, datasets: Optional[List[JsfDataset]] = None):
-        self.datasets = datasets
-
-    def split(self, X: TransformType, y=None) -> List[Union[TSCDataFrame, PCManifold]]:
-        if not self.datasets:
-            dataset = JsfDataset()
-            return [dataset.extract_from(X)]
-
-        X_split: List[Union[TSCDataFrame, PCManifold]] = []
-
-        for dataset in self.datasets:
-            X_split.append(dataset.extract_from(X))
-
-        return X_split
-
-
-class JointlySmoothFunctions(TSCTransformerMixin, BaseEstimator):
-    """Calculate smooth functions on multimodal data/observations.
-
-    Parameters
-    ----------
-    datasets
-        The :py:class:`JsfDataset`s used to split up the multimodal data.
+    data_splits:
+        List of tuples with (name: str, kernel: `BaseManifoldKernel`, indices: slice) to
+        describe the splits on the multimodal data in `X`. For each data split a new kernel is
+        computed.
 
     n_kernel_eigenvectors
-        The number of eigenvectors to compute from the kernel matrices.
+        The number of eigenvectors to compute from each kernel per split.
 
     n_jointly_smooth_functions
-        The number of jointly smooth functions to compute from the eigenvectors of the
-        kernel matrices.
+        The number of jointly smooth functions to compute with a singular value decomposition.
 
     kernel_eigenvalue_cut_off
         The kernel eigenvectors with a eigenvalue smaller than or equal to
-        ``kernel_eigenvalue_cut_off`` will not be included in the calculation of the
-        jointly smooth functions.
+        the cut-off will not be included in the computation of the jointly smooth functions.
 
     eigenvector_tolerance
         The relative accuracy for eigenvalues, i.e. the stopping criterion. A value of
-        0 implies machine precision.
+        zero implies machine precision.
+
+    svd_solver_kwargs
+        Keyword arguments passed to the SciPy
+        `SVD solver <https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.svds.html>`__.
 
     Attributes
     ----------
-    observations_: List[PCManifold]
-        The :py:class:`PCManifolds` containing the separated observations with the
-        specified, corresponding :py:class:`PCManifoldKernel`.
-
-    kernel_matrices_: List[scipy.spars.csr_matrix]
-        The computed kernel matrices.
-
-    _cdist_kwargs_: List[Dict]
-        The cdist_kwargs returned during the kernel calculation. This is required for the
-        out-of-sample extension.
-
-    kernel_eigenvectors_: List[scipy.sparse.csr_matrix]
-        The kernel eigenvectors used to calculate the jointly smooth functions.
+    X_fit_
+        The data `X` passed during `fit`. The data is required to extend the
+        ``jointly_smooth_vectors_`` with the Nyström extension for new samples in `transform`.
+
+    kernel_content_: dict
+        The computed kernel matrix and data required for the Nyström embedding. The key of
+        the dictionary corresponds to the name given in parameter ``data_splits``. (Note that
+        the kernel matrix is only stored of ``store_kernel_matrix=True`` during fit).
+
+    kernel_eigenvectors_: Dict
+        The kernel eigenvectors for each split. The key of the dictionary corresponds to
+        the name given in parameter ``data_splits``. The eigenvectors are used to compute
+        and extend the jointly smooth functions.
+
+    kernel_eigenvalues_: Dict
+        The kernel eigenvalues for each split. The key of the dictionary corresponds to
+        the name given in parameter ``data_splits``. The eigenvalues are used to compute
+        and extend the jointly smooth functions.
+
+    jointly_smooth_vectors_: Union[numpy.ndarray, TSCDataFrame]
+        The jointly smooth functions evaluated at the training data `X` during `fit`.
+        Shape `(n_samples, n_jointly_smooth_functions)`.
 
-    kernel_eigenvalues_ List[scipy.sparse.csr_matrix]
-        The kernel eigenvalues used to calculate the out-of-sample extension.
-
-    _jointly_smooth_functions_: np.ndarray
-        The calculated jointly smooth functions of shape
-        `(n_samples, n_jointly_smooth_functions)`.
-
-    _eigenvalues_: np.ndarray
-        The eigenvalues of the jointly smooth functions of shape `(n_samples)`
+    eigenvalues_: numpy.ndarray
+        The eigenvalues of the jointly smooth functions.
 
     References
     ----------
-    :cite:`TODO enter paper reference`
+    :cite:t:`dietrich-2022`
+
     """
 
+    _required_parameters = ["data_splits"]
+
     def __init__(
         self,
-        datasets: Optional[List[JsfDataset]] = None,
+        data_splits: list[tuple],
+        *,
         n_kernel_eigenvectors: int = 100,
         n_jointly_smooth_functions: int = 10,
         kernel_eigenvalue_cut_off: float = 0,
         eigenvector_tolerance: float = 1e-6,
+        svd_solver_kwargs: Optional[dict] = None,
     ) -> None:
+        self.data_splits = data_splits
         self.n_kernel_eigenvectors = n_kernel_eigenvectors
         self.n_jointly_smooth_functions = n_jointly_smooth_functions
-        self.datasets = datasets
         self.kernel_eigenvalue_cut_off = kernel_eigenvalue_cut_off
         self.eigenvector_tolerance = eigenvector_tolerance
+        self.svd_solver_kwargs = svd_solver_kwargs
+
+        self.X_fit_: Union[TSCDataFrame, pd.DataFrame, np.ndarray]
+        self.kernel_content_: dict
+        self.kernel_eigenvectors_: dict
+        self.kernel_eigenvalues_: dict
+        self.jointly_smooth_vectors_: np.ndarray
+        self.eigenvalues_: np.ndarray
+
+    def _validate_parameter(self):
+        if (
+            not isinstance(self.data_splits, list)
+            or not np.array([isinstance(a, tuple) for a in self.data_splits]).all()
+        ):
+            raise TypeError("parameter 'data_splits' must be a list of tuples")
+
+        if len(self.data_splits) <= 1:
+            raise ValueError("parameter 'data_splits' must at least contain two splits")
+
+        if len({n[0] for n in self.data_splits}) != len(self.data_splits):
+            raise ValueError("the names in 'data_splits' must be unique")
+
+        for a in self.data_splits:
+            if (
+                len(a) != 3
+                or not isinstance(a[0], str)
+                or not isinstance(a[1], BaseManifoldKernel)
+                or not isinstance(a[2], (slice, np.ndarray, list))
+            ):
+                raise TypeError(
+                    f"Each tuple must contain three elements with name (type str), "
+                    f"kernel (BaseManifoldKernel) and indices (slice or np.ndarray). Got {a}"
+                )
+
+        check_scalar(
+            self.n_kernel_eigenvectors,
+            "n_kernel_eigenvectors",
+            target_type=int,
+            min_val=1,
+        )
+
+        check_scalar(
+            self.n_jointly_smooth_functions,
+            "n_kernel_eigenvectors",
+            target_type=int,
+            min_val=1,
+        )
+
+        check_scalar(
+            self.kernel_eigenvalue_cut_off,
+            "kernel_eigenvalue_cut_off",
+            target_type=(int, float),
+            min_val=0,
+        )
+
+    def _compute_kernel_eigenpairs(self, X, kernel_content):
+        ret_eigenvectors = dict()
+        ret_eigenvalues = dict()
+
+        for name in kernel_content:
+            kernel_matrix = kernel_content[name]["kernel_matrix"]
+            kernel = kernel_content[name]["kernel"]
 
-        self.ending_points_: List[int]
-        self.observations_: List[Union[TSCDataFrame, PCManifold]]
-        self.kernel_matrices_: List[scipy.sparse.csr_matrix]
-        self._cdist_kwargs_: List[Dict]
-        self.kernel_eigenvectors_: List[scipy.sparse.csr_matrix]
-        self.kernel_eigenvalues_: List[scipy.sparse.csr_matrix]
-        self._jointly_smooth_functions_: np.ndarray
-        self._eigenvalues_: np.ndarray
-
-    @property
-    def jointly_smooth_functions(self) -> TransformType:
-        return self._jointly_smooth_functions_
-
-    @property
-    def eigenvalues(self) -> np.ndarray:
-        return self._eigenvalues_
-
-    def _calculate_kernel_matrices(self):
-        self._cdist_kwargs_ = []
-        self.kernel_matrices_ = []
-        for observation in self.observations_:
-            kernel_output = observation.compute_kernel_matrix()
-            kernel_matrix, cdist_kwargs, _ = PCManifoldKernel.read_kernel_output(
-                kernel_output
-            )
-            self._cdist_kwargs_.append(cdist_kwargs)
-            sparse_kernel_matrix = scipy.sparse.csr_matrix(
-                kernel_matrix, dtype=np.float64
-            )
-            self.kernel_matrices_.append(sparse_kernel_matrix)
-
-    def _calculate_kernel_eigensystem(self):
-        self.kernel_eigenvectors_ = []
-        self.kernel_eigenvalues_ = []
-        for i, kernel_matrix in enumerate(self.kernel_matrices_):
-            is_symmetric = np.alltrue(kernel_matrix.A == kernel_matrix.T.A)
-            ones_row = np.ones(kernel_matrix.shape[0])
-            ones_col = np.ones(kernel_matrix.shape[1])
-            is_stochastic = np.alltrue(kernel_matrix @ ones_col == ones_row)
             kernel_eigenvalues, kernel_eigenvectors = compute_kernel_eigenpairs(
-                kernel_matrix,
+                kernel=kernel,
+                kernel_matrix=kernel_matrix,
                 n_eigenpairs=self.n_kernel_eigenvectors,
-                is_symmetric=is_symmetric,
-                is_stochastic=is_stochastic,
             )
 
-            if isinstance(kernel_matrix, TSCDataFrame):
-                index_from = kernel_matrix
-            elif (
-                isinstance(self.observations_[i], TSCDataFrame)
-                and kernel_matrix.shape[0] == self.observations_[i].shape[0]
-            ):
-                index_from = self.observations_[i]
-            else:
-                index_from = None
-
-            if index_from is not None:
+            if isinstance(X, pd.DataFrame) and kernel_matrix.shape[0] == X.shape[0]:
                 kernel_eigenvectors = TSCDataFrame.from_same_indices_as(
-                    index_from,
-                    kernel_eigenvectors,
+                    indices_from=X,
+                    values=kernel_eigenvectors,
                     except_columns=[
-                        f"kev{i}" for i in range(self.n_kernel_eigenvectors)
+                        f"ev{i}" for i in range(self.n_kernel_eigenvectors)
                     ],
                 )
 
-            kernel_eigenvalues, kernel_eigenvectors = sort_eigensystem(
-                kernel_eigenvalues, kernel_eigenvectors
-            )
+            bool_evals_cutoff = kernel_eigenvalues > self.kernel_eigenvalue_cut_off
+            ret_eigenvalues[name] = kernel_eigenvalues[bool_evals_cutoff]
+
             if isinstance(kernel_eigenvectors, TSCDataFrame):
-                kernel_eigenvectors = kernel_eigenvectors.iloc[
-                    :, kernel_eigenvalues > self.kernel_eigenvalue_cut_off
-                ]
+                ret_eigenvectors[name] = kernel_eigenvectors.iloc[:, bool_evals_cutoff]
             else:
-                kernel_eigenvectors = kernel_eigenvectors[
-                    :, kernel_eigenvalues > self.kernel_eigenvalue_cut_off
-                ]
-            kernel_eigenvalues = kernel_eigenvalues[
-                kernel_eigenvalues > self.kernel_eigenvalue_cut_off
-            ]
-            self.kernel_eigenvectors_.append(kernel_eigenvectors)
-            self.kernel_eigenvalues_.append(kernel_eigenvalues)
-
-    def _calculate_jointly_smooth_functions(self) -> Tuple[np.ndarray, np.ndarray]:
-        eigenvectors_matrix = scipy.sparse.csr_matrix(
-            np.column_stack([eigenvector for eigenvector in self.kernel_eigenvectors_])
-        )
+                ret_eigenvectors[name] = kernel_eigenvectors[:, bool_evals_cutoff]
 
-        tsc_flag = isinstance(self.kernel_eigenvectors_[0], TSCDataFrame)
-        if tsc_flag:
-            index_from = self.kernel_eigenvectors_[0]
-        else:
-            index_from = None
+        return ret_eigenvalues, ret_eigenvectors
+
+    def _compute_jointly_smooth_vectors(
+        self, X, kernel_eigenvectors
+    ) -> tuple[np.ndarray, np.ndarray]:
+        stacked_eigenvectors = np.column_stack(list(kernel_eigenvectors.values()))
 
-        rng = np.random.default_rng(seed=1)
         if len(self.kernel_eigenvectors_) == 2:
-            ev0 = self.kernel_eigenvectors_[0]
-            ev1 = self.kernel_eigenvectors_[1]
+            # cf. Algorithm 4.1 in https://arxiv.org/pdf/2004.04386.pdf
+            W1, W2 = list(kernel_eigenvectors.values())
+
+            # turn to numpy arrays in case of DataFrame
+            W1, W2 = np.asarray(W1), np.asarray(W2)
+
             n_jointly_smooth_functions = min(
-                [self.n_jointly_smooth_functions, ev0.shape[1] - 1, ev1.shape[1] - 1]
+                [self.n_jointly_smooth_functions, W1.shape[1] - 1, W2.shape[1] - 1]
             )
-            if tsc_flag:
-                evs = ev0.to_numpy().T @ ev1.to_numpy()
-            else:
-                evs = ev0.T @ ev1
-            min_ev_shape = min(evs.shape)
-            v0 = rng.normal(loc=0, scale=1 / min_ev_shape, size=min_ev_shape)
-            Q, eigenvalues, R_t = scipy.sparse.linalg.svds(
-                evs,
-                k=n_jointly_smooth_functions,
-                which="LM",
-                tol=self.eigenvector_tolerance,
-                v0=v0,
-            )
-            center = np.row_stack(
-                [np.column_stack([Q, Q]), np.column_stack([R_t.T, -R_t.T])]
-            )
-            right = np.diag(
-                np.power(np.concatenate([1 + eigenvalues, 1 - eigenvalues]), -1 / 2)
+
+            # compute full SVD
+            Q, singular_vals, Rt = scipy.linalg.svd(W1.T @ W2, full_matrices=False)
+
+            center_blockmatrix = np.row_stack(
+                [np.column_stack([Q, Q]), np.column_stack([Rt.T, -Rt.T])]
             )
+
+            # reduce the elements to the number of functions we actually need
+            center_blockmatrix = center_blockmatrix[:, :n_jointly_smooth_functions]
+
+            # diagonal matrix with 1 +/- singular_vals (Gamma in algorithm)
+            diagonal_elements = np.concatenate([1 + singular_vals, 1 - singular_vals])
+            diagonal_elements = diagonal_elements[:n_jointly_smooth_functions]
+            diagonal_elements = np.sqrt(diagonal_elements, out=diagonal_elements)
+            diagonal_elements = np.reciprocal(diagonal_elements, out=diagonal_elements)
+
             jointly_smooth_functions = (
-                1 / np.sqrt(2) * eigenvectors_matrix @ center @ right
-            )[:, :n_jointly_smooth_functions]
+                1.0
+                / np.sqrt(2.0)
+                * stacked_eigenvectors
+                @ mat_dot_diagmat(center_blockmatrix, diagonal_elements)
+            )
         else:
+            # cf. Algorithm 4.2 in https://arxiv.org/pdf/2004.04386.pdf
             n_jointly_smooth_functions = min(
-                [self.n_jointly_smooth_functions, eigenvectors_matrix.shape[1]]
+                [self.n_jointly_smooth_functions, stacked_eigenvectors.shape[1]]
             )
-            min_ev_shape = min(eigenvectors_matrix.shape)
-            v0 = rng.normal(loc=0, scale=1 / min_ev_shape, size=min_ev_shape)
-            jointly_smooth_functions, eigenvalues, _ = scipy.sparse.linalg.svds(
-                eigenvectors_matrix,
-                k=n_jointly_smooth_functions,
-                which="LM",
-                tol=self.eigenvector_tolerance,
-                v0=v0,
+
+            jointly_smooth_functions, singular_vals, _ = compute_kernel_svd(
+                stacked_eigenvectors,
+                n_svdtriplet=n_jointly_smooth_functions,
+                **(self.svd_solver_kwargs or {}),
             )
 
-        if index_from is not None:
+        if isinstance(X, TSCDataFrame):
             jointly_smooth_functions = TSCDataFrame.from_same_indices_as(
-                index_from,
+                X,
                 jointly_smooth_functions,
-                except_columns=[f"jsf{i}" for i in range(n_jointly_smooth_functions)],
+                except_columns=self.get_feature_names_out(),
             )
 
-        eigenvalues, jointly_smooth_functions = sort_eigensystem(
-            eigenvalues, jointly_smooth_functions
-        )
-
-        return jointly_smooth_functions, eigenvalues
-
-    def nystrom(self, new_indexed_observations: Dict[int, TransformType]):
-        """Embed out-of-sample points with Nyström.
+        return singular_vals, jointly_smooth_functions
 
-        (see transform of dmap for Nyström documentation)
+    def _nystrom(self, X):
+        """Embed out-of-sample points with Nyström extension.
 
         Parameters
         ----------
-        new_indexed_observations: Dict[int, List[Union[TSCDataFrame, pandas.DataFrame, numpy.ndarray]]
-             A dict containing out-of-sample points for (not necessarily all) observations.
-             The keys are the indexes of the observations. The values are the observations
-             of shape `(n_samples, *n_features_of_observation*)`.
+        X: Union[TSCDataFrame, pandas.DataFrame]
+             The out-of-sample data with shape `(n_samples, n_features_in_)`.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
-            same type as the values of shape `(n_samples, n_jointly_smooth_functions)`.
+            same type as `X` of shape `(n_samples, n_jointly_smooth_functions)`
         """
-        eigenvectors = []
-        alphas = []
-        for index, new_observation in new_indexed_observations.items():
-            kernel_eigenvectors = self.kernel_eigenvectors_[index]
-            if isinstance(kernel_eigenvectors, TSCDataFrame):
-                kernel_eigenvectors = kernel_eigenvectors.to_numpy()
-            if isinstance(self._jointly_smooth_functions_, TSCDataFrame):
-                alpha = (
-                    kernel_eigenvectors.T @ self._jointly_smooth_functions_.to_numpy()
-                )
+        kernel_matrices: dict = self._kernel_content_transform(X)
+        eigenvectors = dict()
+        alphas = dict()
+
+        for name in kernel_matrices:
+            kernel_evec = self.kernel_eigenvectors_[name]
+
+            if isinstance(kernel_evec, TSCDataFrame):
+                kernel_evec = kernel_evec.to_numpy()
+
+            if isinstance(self.jointly_smooth_vectors_, TSCDataFrame):
+                alpha = kernel_evec.T @ self.jointly_smooth_vectors_.to_numpy()
             else:
-                alpha = kernel_eigenvectors.T @ self._jointly_smooth_functions_
-            alphas.append(alpha)
-            observation = self.observations_[index]
-            kernel_output = observation.compute_kernel_matrix(
-                new_observation, **self._cdist_kwargs_[index]
-            )
-            kernel_matrix, _, _ = PCManifoldKernel.read_kernel_output(
-                kernel_output=kernel_output
-            )
-            approx_eigenvectors = kernel_matrix @ mat_dot_diagmat(
-                kernel_eigenvectors,
-                np.reciprocal(self.kernel_eigenvalues_[index]),
-            )
-
-            if isinstance(kernel_matrix, TSCDataFrame):
-                index_from: Optional[TSCDataFrame] = kernel_matrix
-            elif (
-                isinstance(new_observation, TSCDataFrame)
-                and kernel_matrix.shape[0] == new_observation.shape[0]
-            ):
-                index_from = new_observation
+                alpha = kernel_evec.T @ self.jointly_smooth_vectors_
+
+            alphas[name] = alpha
+
+            eigenvectors[name] = kernel_matrices[name] @ mat_dot_diagmat(
+                kernel_evec,
+                np.reciprocal(self.kernel_eigenvalues_[name]),
+            )
+
+        _dtype_probe = list(alphas.values())[0].dtype
+        f_m_star = np.zeros(
+            [X.shape[0], self.n_jointly_smooth_functions], dtype=_dtype_probe
+        )
+        tmp = np.zeros_like(f_m_star)
+
+        for name in eigenvectors:
+            f_m_star += np.dot(eigenvectors[name], alphas[name], out=tmp)
+
+        f_m_star /= len(self.data_splits)  # divide by number of splits
+
+        if isinstance(X, TSCDataFrame) and hasattr(self, "feature_names_in_"):
+            f_m_star = TSCDataFrame.from_same_indices_as(
+                X, f_m_star, except_columns=self.get_feature_names_out()
+            )
+
+        return f_m_star
+
+    def _kernel_content_fit(self, X: TransformType):
+        return_content: dict[str, dict] = dict()
+
+        for _, split in enumerate(self.data_splits):
+            name, kernel, indices = split
+
+            # copy kernels to not mutate the original attribute(sklearn conform)
+            kernel = deepcopy(kernel)
+
+            if isinstance(X, pd.DataFrame):
+                kernel_matrix = kernel(X.iloc[:, indices])
             else:
-                index_from = None
+                kernel_matrix = kernel(X[:, indices])
 
-            if index_from is not None:
-                approx_eigenvectors = TSCDataFrame.from_same_indices_as(
-                    index_from,
-                    approx_eigenvectors,
-                    except_columns=[
-                        f"aev{i}"
-                        for i in range(self.kernel_eigenvectors_[index].shape[1])
-                    ],
+            return_content[name] = dict()
+            return_content[name]["kernel_matrix"] = kernel_matrix
+            return_content[name]["kernel"] = kernel
+
+        return return_content
+
+    def _kernel_content_transform(self, X):
+        return_content = dict()
+
+        for _, split in enumerate(self.data_splits):
+            name, _, indices = split
+            kernel = self.kernel_content_[name]["kernel"]
+
+            if isinstance(X, pd.DataFrame):
+                kernel_matrix = kernel(
+                    self.X_fit_.iloc[:, indices],
+                    X.iloc[:, indices],
+                )
+            else:
+                kernel_matrix = kernel(
+                    self.X_fit_[:, indices],
+                    X[:, indices],
                 )
 
-            eigenvectors.append(approx_eigenvectors)
-        f_m_star = 0.0
-        for i in range(len(alphas)):
-            f_m_star += eigenvectors[i] @ alphas[i]
-        f_m_star /= len(alphas)
-        return f_m_star
+            return_content[name] = kernel_matrix
+
+        return return_content
+
+    def get_feature_names_out(self, input_features=None):
+        return np.array([f"jsf{i}" for i in range(self.n_jointly_smooth_functions)])
 
     def fit(self, X: TransformType, y=None, **fit_params) -> "JointlySmoothFunctions":
-        """Compute the jointly smooth functions.
+        """Compute the jointly smooth functions on training data `X`.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.Dataframe, numpy.ndarray
             Training data of shape `(n_samples, n_features)`
 
         y: None
@@ -419,94 +356,77 @@
             ignored
 
         Returns
         -------
         JointlySmoothFunctions
             self
         """
-        X = self._validate_datafold_data(
-            X=X,
-            array_kwargs=dict(
-                ensure_min_samples=max(2, self.n_kernel_eigenvectors + 1)
-            ),
-            tsc_kwargs=dict(ensure_min_samples=max(2, self.n_kernel_eigenvectors + 1)),
-        )
-
-        self._setup_feature_attrs_fit(
-            X=X,
-            features_out=[f"jsf{i}" for i in range(self.n_jointly_smooth_functions)],
+        self.X_fit_ = self._validate_datafold_data(
+            X=X, ensure_min_samples=max(2, self.n_kernel_eigenvectors + 1)
         )
 
-        column_splitter = _ColumnSplitter(self.datasets)
-        self.observations_ = column_splitter.split(X)
+        self._validate_parameter()
 
-        self._calculate_kernel_matrices()
+        store_kernel_matrix = self._read_fit_params(
+            attrs=[("store_kernel_matrix", False)],
+            fit_params=fit_params,
+        )
 
-        self._calculate_kernel_eigensystem()
+        self._setup_feature_attrs_fit(X=X)
+        self.kernel_content_ = self._kernel_content_fit(self.X_fit_)
+        (
+            self.kernel_eigenvalues_,
+            self.kernel_eigenvectors_,
+        ) = self._compute_kernel_eigenpairs(X, self.kernel_content_)
+
+        if not store_kernel_matrix:
+            # release storage by deleting kernel matrix
+            for name in self.kernel_content_:
+                del self.kernel_content_[name]["kernel_matrix"]
 
         (
-            self._jointly_smooth_functions_,
-            self._eigenvalues_,
-        ) = self._calculate_jointly_smooth_functions()
+            self.eigenvalues_,
+            self.jointly_smooth_vectors_,
+        ) = self._compute_jointly_smooth_vectors(X, self.kernel_eigenvectors_)
 
         return self
 
     def transform(self, X: TransformType) -> TransformType:
-        """Embed out-of-sample points with the Nyström extension.
-
-        (see transform of dmap for Nyström documentation)
+        """Evaluate jointly smooth functions for out-of-sample data with Nyström extension.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
-            Data points of shape `(n_samples, n_features)` to be embedded.
+            Data points of shape `(n_samples, n_features)` to be mapped.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_jointly_smooth_functions)`
         """
         check_is_fitted(
             self,
             (
-                "observations_",
-                "kernel_matrices_",
-                "_cdist_kwargs_",
+                "kernel_content_",
                 "kernel_eigenvectors_",
                 "kernel_eigenvalues_",
-                "_jointly_smooth_functions_",
-                "_eigenvalues_",
+                "jointly_smooth_vectors_",
+                "eigenvalues_",
             ),
         )
 
-        X = self._validate_datafold_data(
-            X=X,
-            array_kwargs=dict(ensure_min_samples=1),
-            tsc_kwargs=dict(ensure_min_samples=1),
-        )
-
-        if X.shape[1] != self.n_features_in_:
-            raise ValueError(
-                "X must have the same number of features as the data with which fit was called."
-                "If you want to call it with fewer observations, you have to call nystrom"
-            )
-
+        X = self._validate_datafold_data(X=X)
         self._validate_feature_input(X, direction="transform")
 
-        column_splitter = _ColumnSplitter(self.datasets)
-        new_observations = column_splitter.split(X)
-
-        indices = list(range(len(self.observations_)))
-        indexed_observations = dict(zip(indices, new_observations))
-        f_m_star = self.nystrom(indexed_observations)
+        f_m_star = self._nystrom(X)
 
         return f_m_star
 
     def fit_transform(self, X: TransformType, y=None, **fit_params) -> TransformType:
-        """Compute jointly smooth functions and return them.
+        """Compute and return jointly smooth functions evaluated at training data `X`.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data of shape `(n_samples, n_features)`
 
         y: None
@@ -517,77 +437,83 @@
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_jointly_smooth_functions)`
         """
         X = self._validate_datafold_data(
-            X,
-            array_kwargs=dict(ensure_min_samples=max(2, self.n_kernel_eigenvectors)),
-            tsc_kwargs=dict(ensure_min_samples=max(2, self.n_kernel_eigenvectors)),
+            X, ensure_min_samples=max(2, self.n_kernel_eigenvectors)
         )
         self.fit(X=X, y=y, **fit_params)
 
-        return self._jointly_smooth_functions_
+        return self.jointly_smooth_vectors_
 
     def score_(self, X, y):
         """Compute a score for hyperparameter optimization.
 
         Returns
         -------
         float
             The sum of the truncated energies.
         """
-        return self.calculate_truncated_energies().sum()
+        return self._compute_truncated_energies().sum()
 
-    def calculate_truncated_energies(self) -> np.ndarray:
+    def _compute_truncated_energies(self) -> np.ndarray:
         """Compute the truncated energy for each kernel eigenvector.
 
         Returns
         -------
         np.ndarray
             The truncated energies of shape `(n_observations, n_jointly_smooth_functions)`.
         """
-        truncated_energies = []
-        for kernel_eigenvector in self.kernel_eigenvectors_:
-            truncated_energy = (
-                np.linalg.norm(
-                    kernel_eigenvector.T @ self.jointly_smooth_functions, axis=0
-                )
-                ** 2
+        truncated_energies = dict()
+        for name in self.kernel_eigenvectors_:
+            truncated_energy = np.linalg.norm(
+                np.asarray(self.kernel_eigenvectors_[name]).T
+                @ self.jointly_smooth_vectors_,
+                axis=0,
             )
-            truncated_energies.append(truncated_energy)
-        return np.array(truncated_energies)
+            truncated_energies[name] = truncated_energy**2
+
+        return np.array(truncated_energies.values())
 
-    def calculate_E0(self) -> float:
+    def compute_E0(self) -> float:
         """Compute a threshold for the eigenvalues of the jointly smooth functions.
 
         Returns
         -------
         float
-            The E0 threshold value from :cite:`TODO enter paper reference`
+            The E0 threshold value from :cite:t:`dietrich-2022`.
         """
-        noisy = self.kernel_eigenvectors_[-1].copy()
-        np.random.shuffle(noisy)
+        kernel_evecs = list(self.kernel_eigenvectors_.values())
 
-        kernel_eigenvectors = self.kernel_eigenvectors_[:-1]
+        noisy = kernel_evecs[-1].copy()
+
+        rng = np.random.default_rng(1)  # expose seed to user if required
+        rng.shuffle(noisy)
+
+        kernel_eigenvectors = kernel_evecs[:-1]
         kernel_eigenvectors.append(noisy)
 
-        eigenvectors_matrix = scipy.sparse.csr_matrix(
-            np.column_stack([eigenvector for eigenvector in kernel_eigenvectors])
-        )
+        eigenvectors_matrix = np.column_stack(kernel_evecs)
 
         if len(kernel_eigenvectors) == 2:
             ev0 = kernel_eigenvectors[0]
             ev1 = kernel_eigenvectors[1]
-            _, Gamma, _ = scipy.sparse.linalg.svds(
-                ev0.T @ ev1, k=self.n_jointly_smooth_functions, which="LM"
+
+            gamma = scipy.sparse.linalg.svds(
+                ev0.T @ ev1,
+                k=self.n_jointly_smooth_functions,
+                which="LM",
+                return_singular_vectors=False,
             )
         else:
-            _, Gamma, _ = scipy.sparse.linalg.svds(
-                eigenvectors_matrix, k=self.n_jointly_smooth_functions, which="LM"
+            gamma = scipy.sparse.linalg.svds(
+                eigenvectors_matrix,
+                k=self.n_jointly_smooth_functions,
+                which="LM",
+                return_singular_vectors=False,
             )
 
-        Gamma.sort()
-        gamma2 = Gamma[-2]
-        E0 = (1 + gamma2) / 2
+        gamma = np.sort(gamma)[::-1]
+        E0 = (1 + gamma[2]) / 2  # page 6 in https://arxiv.org/pdf/2004.04386.pdf
         return E0
```

### Comparing `datafold-1.1.6/datafold/dynfold/outofsample.py` & `datafold-2.0.0/datafold/dynfold/outofsample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import enum
-from typing import Optional, Union
+from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.sparse
 from sklearn.base import BaseEstimator, MultiOutputMixin, RegressorMixin
 from sklearn.metrics import mean_squared_error
 from sklearn.utils import check_array, check_consistent_length, check_X_y
 from sklearn.utils.validation import check_is_fitted, check_scalar
 
 from datafold._decorators import warn_known_bug
 from datafold.dynfold.dmap import _DmapKernelAlgorithms
-from datafold.pcfold import PCManifold
 from datafold.pcfold.distance import compute_distance_matrix
 from datafold.pcfold.kernels import DmapKernelFixed, GaussianKernel, PCManifoldKernel
 from datafold.utils.general import mat_dot_diagmat
 
 
 class GeometricHarmonicsInterpolator(RegressorMixin, MultiOutputMixin, BaseEstimator):
     """Interpolation of function values on high dimensional data with manifold assumption.
@@ -40,23 +39,17 @@
     symmetrize_kernel
         If True, a conjugate transformation is performed if the current settings would
         lead to a non-symmetric kernel matrix. This improves numerical stability when
         solving the eigenvectors of the kernel matrix as it allows algorithms designed
         for (sparse) Hermitian matrices to be used. If the kernel matrix is symmetric
         already (`is_stochastic=False`), then the parameter has no effect.
 
-    dist_kwargs
-        Keyword arguments passed to the internal distance matrix computation. See
-        :py:meth:`datafold.pcfold.distance.compute_distance_matrix` for parameter
-        arguments.
-
     Attributes
     ----------
-
-    X_: PCManifold
+    X_fit_: np.ndarray
         Training data during fit of shape `(n_samples, n_features)`. The data is required
         to be stored to perform out-of-sample interpolations. Equipped with kernel
         :py:class:`DmapKernelFixed`.
 
     y_: numpy.ndarray
         Target function values of shape `(n_samples, n_targets)`, can be multi-dimensional.
 
@@ -67,41 +60,39 @@
         Eigenvectors of the kernel matrix. Corresponds to the geometric harmonics.
 
     kernel_matrix_ : Union[numpy.ndarray, scipy.sparse.csr_matrix]
         Computed kernel matrix, stored if `store_kernel_matrix=True` during fit.
 
     References
     ----------
+    :cite:`coifman-2006a`
 
-    :cite:`coifman_geometric_2006`
+    See :cite:t:`evangelou-2022` for using geometric harmonics to map between ambient and
+    latent space variables (diffusion coordinates).
 
     See Also
     --------
-
     :class:`.LaplacianPyramidsInterpolator`
 
     """
 
     def __init__(
         self,
         kernel: Optional[PCManifoldKernel] = None,
         *,  # keyword-only
         n_eigenpairs: int = 10,
         is_stochastic: bool = False,
         alpha: float = 1,
         symmetrize_kernel=True,
-        dist_kwargs=None,
     ) -> None:
-
         self.kernel = kernel
         self.n_eigenpairs = n_eigenpairs
         self.is_stochastic = is_stochastic
         self.alpha = alpha
         self.symmetrize_kernel = symmetrize_kernel
-        self.dist_kwargs = dist_kwargs
 
     def _precompute_aux(self) -> None:
         # TODO: [style, minor] "aux" should get a better name
 
         # Alternative/legacy way of computing self._aux
         # a little bit faster than  legacy "n^3"
         # self._aux = (ev.T * (1. / ew)) @ (ev @ self.values)
@@ -143,27 +134,20 @@
         # see "check_regressors_train" in sklearn/estimator_checks.py
         # GHI computes the negated root mean squared error and therefore would
         # always fail because of this assert in the test:
         #     regressor.score(X, y_) > 0.5
         return {"requires_y": True, "multioutput": True, "poor_score": True}
 
     def _get_tags(self):
-        return super(GeometricHarmonicsInterpolator, self)._get_tags()
+        # TODO: check if this function can be removed, as it anyway only calls super class
+        return super()._get_tags()
 
     def _get_default_kernel(self):
         return GaussianKernel(epsilon=1.0)
 
-    def _setup_default_dist_kwargs(self):
-        from copy import deepcopy
-
-        self.dist_kwargs_ = deepcopy(self.dist_kwargs) or {}
-        self.dist_kwargs_.setdefault("cut_off", np.inf)
-        self.dist_kwargs_.setdefault("kmin", 0)
-        self.dist_kwargs_.setdefault("backend", "guess_optimal")
-
     def fit(
         self, X: np.ndarray, y: np.ndarray, store_kernel_matrix: bool = False
     ) -> "GeometricHarmonicsInterpolator":
         """Fit model with training data.
 
         Parameters
         ----------
@@ -177,82 +161,67 @@
             If True, store the kernel matrix in attribute ``kernel_matrix_``.
 
         Returns
         -------
         GeometricHarmonicsInterpolator
             self
         """
-
         # function provided by sklearn
         # internally sets attribute n_features_in_
         X, y = self._validate_data(
             X=X,
             y=y,
             reset=True,
             validate_separately=False,
             **self._validate_kwargs(X, ensure_min_samples=2, during_fit=True),
         )
         if isinstance(y, np.ndarray) and y.ndim == 1:
             y = y[:, np.newaxis]
         check_consistent_length(X, y)
 
-        self._setup_default_dist_kwargs()
-
         internal_kernel = (
             self.kernel if self.kernel is not None else self._get_default_kernel()
         )
 
         self._dmap_kernel = DmapKernelFixed(
             internal_kernel=internal_kernel,
             is_stochastic=self.is_stochastic,
             alpha=self.alpha,
             symmetrize_kernel=self.symmetrize_kernel,
         )
 
-        self.X_ = PCManifold(
-            X,
-            kernel=self._dmap_kernel,
-            dist_kwargs=self.dist_kwargs_,
-        )
+        self.X_fit_ = X
         self.y_ = y
 
         check_scalar(
             self.n_eigenpairs,
             "n_eigenpairs",
             target_type=(int, np.integer),
             min_val=1,
-            max_val=self.X_.shape[0] - 1,
+            max_val=self.X_fit_.shape[0] - 1,
         )
 
-        kernel_output = self.X_.compute_kernel_matrix()
-        (
-            kernel_matrix_,
-            self._cdist_kwargs,
-            ret_extra,
-        ) = PCManifoldKernel.read_kernel_output(kernel_output=kernel_output)
-        basis_change_matrix = ret_extra["basis_change_matrix"]
+        kernel_matrix_ = self._dmap_kernel(X=X)
 
         (
             self.eigenvalues_,
             self.eigenvectors_,
         ) = _DmapKernelAlgorithms.solve_eigenproblem(
+            kernel=self._dmap_kernel,
             kernel_matrix=kernel_matrix_,
             n_eigenpairs=self.n_eigenpairs,
-            is_symmetric=self._dmap_kernel.is_symmetric,
-            is_stochastic=self.is_stochastic,
-            basis_change_matrix=basis_change_matrix,
         )
 
         self._precompute_aux()
 
         if store_kernel_matrix:
-            if self._dmap_kernel.is_symmetric_transform():
+            if self._dmap_kernel.is_conjugate:
                 self.kernel_matrix_ = _DmapKernelAlgorithms.unsymmetric_kernel_matrix(
                     kernel_matrix=kernel_matrix_,
-                    basis_change_matrix=basis_change_matrix,
+                    basis_change_matrix=self._dmap_kernel.basis_change_matrix_,
                 )
             else:
                 self.kernel_matrix_ = kernel_matrix_
 
         return self
 
     def predict(self, X: np.ndarray) -> np.ndarray:
@@ -264,25 +233,20 @@
             Points of shape `(n_samples, n_features)`.
 
         Returns
         -------
         numpy.ndarray
             The interpolated function values of shape `(n_samples, n_targets)`.
         """
-
         check_is_fitted(self)
         X = check_array(
             X, **self._validate_kwargs(X, ensure_min_samples=1, during_fit=False)
         )
 
-        kernel_output = self.X_.compute_kernel_matrix(Y=X, **self._cdist_kwargs)
-        kernel_matrix_, _, _ = PCManifoldKernel.read_kernel_output(
-            kernel_output=kernel_output
-        )
-
+        kernel_matrix_ = self._dmap_kernel(self.X_fit_, X)
         return np.squeeze(kernel_matrix_ @ self._aux)
 
     @warn_known_bug(gitlab_issue=16)
     def gradient(self, X: np.ndarray, vcol: Optional[int] = None) -> np.ndarray:
         """Evaluate gradient of interpolator at the given points.
 
         .. warning::
@@ -299,25 +263,24 @@
             Has to be given for multivariate interpolation.
 
         Returns
         -------
         np.ndarray
             Gradients (row-wise)
         """
-
         # TODO: generalize to all columns (if required...). Note that this will be a
         #  tensor then.
 
         from sklearn.utils.validation import check_array
 
         X = check_array(
             X, self._validate_kwargs(X, ensure_min_samples=1, during_fit=False)
         )
 
-        assert self.X_ is not None and self.y_ is not None  # prevents mypy warnings
+        assert self.X_fit_ is not None and self.y_ is not None  # prevents mypy warnings
 
         if vcol is None and self.y_.ndim > 1 and self.y_.shape[1] > 1:
             raise NotImplementedError(
                 "Currently vcol has to be provided to indicate for which values to get "
                 "the gradient. Jacobi matrix is currently not supported."
             )
 
@@ -328,36 +291,30 @@
             )
 
         if vcol is not None:
             values = self.y_[:, vcol]
         else:
             values = self.y_[:, 0]
 
-        kernel_output = self.X_.compute_kernel_matrix(X)
-        kernel_matrix, _, _sanity_check = PCManifoldKernel.read_kernel_output(
-            kernel_output=kernel_output
-        )
-
-        assert _sanity_check == {}
+        kernel_matrix = self._dmap_kernel(self.X_fit_, X)
 
         # TODO: see issue #54 the to_ndarray() kills memory, when many points
         #  (xi.shape[0]) are requested
-
         if isinstance(kernel_matrix, scipy.sparse.coo_matrix):
             kernel_matrix = np.squeeze(kernel_matrix.toarray())
         elif isinstance(kernel_matrix, scipy.sparse.csr_matrix):
             kernel_matrix = kernel_matrix.toarray()
 
         # Gradient computation
         ki_psis = kernel_matrix * values
 
         grad = np.zeros_like(X)
-        v = np.empty_like(self.X_)
+        v = np.empty_like(self.X_fit_)
         for p in range(X.shape[0]):
-            np.subtract(X[p, :], self.X_, out=v)
+            np.subtract(X[p, :], self.X_fit_, out=v)
             np.matmul(v.T, ki_psis[p, :], out=grad[p, :])
         return grad
 
     def score(
         self,
         X: np.ndarray,
         y: np.ndarray,
@@ -422,67 +379,61 @@
         return -1 * np.sqrt(score)
 
 
 @NotImplementedError
 class MultiScaleGeometricHarmonicsInterpolator(
     GeometricHarmonicsInterpolator
 ):  # pragma: no cover
-    """
-    .. warning::
-        This class is not documented and in experimental state. Contributions are welcome:
-            * documentation
-            * write unit tests
-            * improve code
+    """.. warning::
+    This class is not documented and in experimental state. Contributions are welcome:
+    * documentation
+    * write unit tests
+    * improve code.
     """
 
     def __init__(
         self,
         initial_scale=1.0,
         n_eigenpairs: int = 11,
         condition=1.0,  # nu
         admissible_error=1.0,  # tau
         is_stochastic: bool = False,
         alpha: float = 1,
         symmetrize_kernel=False,
-        dist_kwargs=None,
     ):
+        """TODO: This is a work in progress algorithm.
+        See: Chiavazzo et al. Reduced Models in Chemical Kinetics via Nonlinear
+        Data-Mining.
         """
-        TODO: This is a work in progress algorithm.
-         See: Chiavazzo et al. Reduced Models in Chemical Kinetics via Nonlinear
-              Data-Mining
-        """
-        super(MultiScaleGeometricHarmonicsInterpolator, self).__init__(
+        super().__init__(
             kernel=GaussianKernel(),
             n_eigenpairs=n_eigenpairs,
             is_stochastic=is_stochastic,
             alpha=alpha,
             symmetrize_kernel=symmetrize_kernel,
-            dist_kwargs=dist_kwargs,
         )
 
         self.condition = condition
         self.admissible_error = admissible_error
         self.initial_scale = initial_scale
 
     def _multi_scale_optimize(self, X, y):
-
         scale = self.initial_scale
         error_not_in_range = True
 
         from scipy.sparse.linalg import eigsh
 
         from datafold.pcfold import PCManifold
         from datafold.pcfold.kernels import GaussianKernel
         from datafold.utils.general import diagmat_dot_mat, sort_eigenpairs
 
         mu_l_ = None
         phi_l_ = None
 
         while error_not_in_range:
-
             kernel = GaussianKernel(epsilon=scale)
             X = PCManifold(X, kernel)
 
             kernel_matrix = X.compute_kernel_matrix()
 
             mu, phi = eigsh(kernel_matrix, k=300, which="LM")
             mu, phi = np.real(mu), np.real(phi)
@@ -490,15 +441,15 @@
 
             # use orthogonality to solve phi c = y
             coeff_ = phi.T @ y
 
             ratio_eigenvalues = mu[0] / mu
             max_l = np.argmax(~(ratio_eigenvalues < self.condition))
 
-            coeff_l_, coeff_l_err_ = (coeff_[:max_l], coeff_[max_l:])
+            _, coeff_l_err_ = (coeff_[:max_l], coeff_[max_l:])
 
             mu_l_ = mu[:max_l]
             phi_l_ = phi[:, :max_l]
 
             error = np.sqrt(np.sum(np.abs(coeff_l_err_) ** 2))
 
             print(f"scale={scale}  --  error={error} -- max_l={max_l}")
@@ -529,34 +480,32 @@
 
         self._multi_scale_optimize(X, y)
         # self._precompute_aux()
 
         return self
 
     def score(self, X, y, sample_weight=None, multioutput="uniform_average") -> float:
-
         if y is None:
             y = self.eigenvectors_  # target functions
 
-        return super(MultiScaleGeometricHarmonicsInterpolator, self).score(
+        return super().score(
             X=X, y=y, sample_weight=sample_weight, multioutput=multioutput
         )
 
 
 class LaplacianPyramidsInterpolator(RegressorMixin, MultiOutputMixin, BaseEstimator):
     """Laplacian pyramids interpolation of function values on data manifold using
     kernels with different scales.
 
     The model implementation is generalized to vector valued targets: The kernel scales
     are decreased (i.e. a new kernel with lower scale is computed) until for each target
     function the corresponding stopping criteria is reached (based on the residual).
 
     Parameters
     ----------
-
     initial_epsilon
         The scale of kernel in first iteration.
 
     mu
         The factor by which epsilon is decreased in every iteration
         :code:`(new_epsilon = old_epsilon / mu)`. Must be a strictly larger than one.
 
@@ -570,31 +519,28 @@
 
     alpha
         A parameter handled to the diffusion maps kernel that in internally used
         (see :py:class:`DmapKernelFixed`).
 
     Attributes
     ----------
-
     X_: numpy.ndarray
         The point cloud during fit. Must be stored into memory to be able to perform
         out-of-sample interpolations.
 
     level_: int
         The number of levels and kernels used in the model.
 
     n_targets_: int
         The number of target functions during fit. (Note, the target values are not
         stored in the model).
 
     References
     ----------
-
-    :cite:`fernandez_auto-adaptative_2014`
-    :cite:`rabin_heterogeneous_2012`
+    :cite:`fernandez-2014,rabin-2012`
 
     """
 
     # Internal Enum class to indicate the state of a function in the loop during fit
     class _LoopCond(enum.Enum):
         NO_TERMINATION = 0
         BELOW_RES_TOL = 1
@@ -607,48 +553,44 @@
         *,  # keyword-only
         initial_epsilon: float = 10.0,
         mu: float = 2.0,
         residual_tol: Optional[float] = None,
         auto_adaptive: bool = False,
         alpha: float = 0,
     ):
-
         self.initial_epsilon = initial_epsilon
         self.mu = mu
         self.residual_tol = residual_tol
         self.auto_adaptive = auto_adaptive
         self.alpha = alpha
 
     @property
     def level_(self):
         return 0 if self._level_tracker == {} else max(self._level_tracker.keys())
 
     def _validate(self, X, y, ensure_y, ensure_min_samples):
-
         if self.residual_tol is None and not self.auto_adaptive:
             raise ValueError(
                 "Need to specify a stopping criteria by either providing a "
                 "residual tolerance or enabling auto adaptive termination."
             )
 
         if self.residual_tol is not None:
             check_scalar(
                 self.residual_tol,
                 name="residual_tol",
                 target_type=(float, np.floating),
                 min_val=0,
-                max_val=np.inf,
             )
 
         check_scalar(
             self.mu,
             "mu",
             target_type=(int, np.integer, float, np.floating),
-            min_val=1 + np.finfo(float).eps,
-            max_val=np.inf,
+            min_val=1,
         )
 
         if isinstance(X, np.memmap):
             copy = True
         else:
             copy = False
 
@@ -676,15 +618,15 @@
 
         return X, y
 
     def _setup(self):
         self._level_tracker = dict()
 
     def _get_tags(self):
-        _tags = super(LaplacianPyramidsInterpolator, self)._get_tags()
+        _tags = super()._get_tags()
         _tags["multioutput"] = True
         return _tags
 
     def _termination_rules_single(self, current_residual_norm, last_residual_norm):
         signal = self._LoopCond.NO_TERMINATION
 
         if self.auto_adaptive:
@@ -710,15 +652,14 @@
         ):
             # Stop in any configuration, below this threshold
             signal = self._LoopCond.TINY_RES
 
         return signal
 
     def _terminate_condition_loop(self, current_residual_norm, last_residual_norm):
-
         assert current_residual_norm.ndim == 1
         assert current_residual_norm.shape == last_residual_norm.shape
 
         nr_tests = current_residual_norm.shape[0]
         signals = np.array([self._LoopCond.NO_TERMINATION] * nr_tests)
 
         for i in range(nr_tests):
@@ -739,32 +680,26 @@
     def _get_next_level_(self):
         if self._level_tracker == {}:
             return 0
         else:
             return max(self._level_tracker.keys()) + 1
 
     def _track_new_level(
-        self,
-        kernel,
-        target_values,
-        residual_norm,
-        active_func_indices,
-        row_sums_fit_alpha,
+        self, kernel, target_values, residual_norm, active_func_indices
     ):
         new_level = self._get_next_level_()
 
         assert new_level not in self._level_tracker.keys()
         assert active_func_indices.shape[0] == target_values.shape[1]
 
         self._level_tracker[new_level] = {
             "kernel": kernel,
             "target_values": target_values,
             "residual_norm": residual_norm,
             "active_indices": active_func_indices,
-            "row_sums_fit_alpha": row_sums_fit_alpha,
         }
 
     def _remove_increase_loocv_indices(
         self,
         active_func_indices,
         loop_condition,
         target_values,
@@ -782,15 +717,14 @@
     def _remove_residual_based_indices(
         self,
         active_func_indices,
         loop_condition,
         current_residual,
         current_residual_norm,
     ):
-
         # remove LOOCV-termination reason as it is handeled separately
         loop_condition = loop_condition[
             loop_condition != self._LoopCond.LOOCV_INCREASES
         ]
 
         bool_idx = np.logical_or(
             loop_condition == self._LoopCond.BELOW_RES_TOL,
@@ -807,31 +741,27 @@
         dmap_kernel = DmapKernelFixed(
             internal_kernel=GaussianKernel(epsilon),
             is_stochastic=True,
             alpha=self.alpha,
             symmetrize_kernel=False,
         )
 
-        kernel_output = dmap_kernel.eval(distance_matrix=distance_matrix, is_pdist=True)
-        kernel_matrix, cdist_kwargs, _check = PCManifoldKernel.read_kernel_output(
-            kernel_output=kernel_output
+        kernel_matrix = dmap_kernel.evaluate(
+            distance_matrix=distance_matrix, is_pdist=True
         )
 
-        row_sums_alpha_fit = cdist_kwargs["row_sums_alpha_fit"]
-
-        assert (
-            _check["basis_change_matrix"] is None
-        ), "no symmetrize of kernel supported"
+        if dmap_kernel.is_conjugate:
+            raise NotImplementedError("no symmetric conjugation of kernel supported")
 
         if self.auto_adaptive:
             # inplace: set diagonal to zero to obtain LOOCV estimation
             # TODO: this requires special handling for a sparse kernel matrix
             np.fill_diagonal(kernel_matrix, 0)
 
-        return dmap_kernel, kernel_matrix, row_sums_alpha_fit
+        return dmap_kernel, kernel_matrix
 
     def _compute_residual(
         self, y, func_approx, active_func_indices, current_residual_norm
     ):
         current_residual = np.subtract(
             y[:, active_func_indices], func_approx[:, active_func_indices]
         )
@@ -840,15 +770,14 @@
             current_residual_norm,
             np.linalg.norm(current_residual, axis=0),
         )
 
         return current_residual, current_residual_norm, last_residual_norm
 
     def _laplacian_pyramid(self, X, y):
-
         func_approx = np.zeros_like(y, dtype=float)
 
         # compute once and only apply eval
         distance_matrix = self._distance_matrix(X)
 
         # set up variables for first iteration
         target_values = y
@@ -858,20 +787,17 @@
 
         # at least one iteration
         func_loop_conditions = np.array(
             [self._LoopCond.NO_TERMINATION] * self.n_targets_
         )
 
         while self._LoopCond.NO_TERMINATION in func_loop_conditions:
-
-            (
-                dmap_kernel,
-                kernel_matrix,
-                row_sums_fit_alpha,
-            ) = self._prepare_kernel_and_matrix(distance_matrix, epsilon)
+            (dmap_kernel, kernel_matrix) = self._prepare_kernel_and_matrix(
+                distance_matrix, epsilon
+            )
 
             # improve function approximation
             func_approx[:, active_func_indices] += kernel_matrix @ target_values
 
             (
                 current_residual,
                 current_residual_norm,
@@ -910,15 +836,14 @@
                 # insert all information about this run
                 # (mainly required for function evaluation in __call__ !)
                 self._track_new_level(
                     kernel=dmap_kernel,
                     target_values=target_values,
                     residual_norm=current_residual_norm,
                     active_func_indices=active_func_indices,
-                    row_sums_fit_alpha=row_sums_fit_alpha,
                 )
 
                 # Remove all indices now that fulfill the residual criteria and do not
                 # need another loop.
                 (
                     active_func_indices,
                     current_residual,
@@ -929,15 +854,14 @@
                     current_residual,
                     current_residual_norm,
                 )
 
             if self._LoopCond.NO_TERMINATION in curr_loop_conditions:
                 # prepare for next loop iteration
                 epsilon = epsilon / self.mu
-                current_residual_norm = current_residual_norm
                 target_values = current_residual
 
         return self
 
     def fit(
         self, X: np.ndarray, y: np.ndarray, **fit_params
     ) -> "LaplacianPyramidsInterpolator":
@@ -972,40 +896,35 @@
             Out-of-sample data of shape `(n_samples, n_features)`.
 
         Returns
         -------
         numpy.ndarray
             Predicted function values of shape `(n_samples, n_targets_)`.
         """
-
         X, _ = self._validate(X, y=None, ensure_y=False, ensure_min_samples=1)
 
         check_is_fitted(self)
 
         # allocate memory for return
         y_hat = np.zeros([X.shape[0], self.n_targets_])
         distance_matrix = self._distance_matrix(X=self.X_, Y=X)
 
-        for level, level_content in self._level_tracker.items():
-
-            kernel_matrix, _, _ = level_content["kernel"].eval(
-                distance_matrix, row_sums_alpha_fit=level_content["row_sums_fit_alpha"]
-            )
+        for _, level_content in self._level_tracker.items():
+            kernel_matrix = level_content["kernel"].evaluate(distance_matrix)
 
             active_indices = level_content["active_indices"]
             y_hat[:, active_indices] += kernel_matrix @ level_content["target_values"]
 
         if self.n_targets_ == 1:
             y_hat = y_hat.flatten()
 
         return y_hat
 
     def plot_eps_vs_residual(self) -> None:  # pragma: no cover
         """Plot residuals versus kernel scales (epsilon) from model fit."""
-
         check_is_fitted(self)
 
         norm_residuals = np.zeros([self.level_ + 1, self.n_targets_]) * np.nan
 
         for i, info in enumerate(self._level_tracker.values()):
             residuals = np.linalg.norm(info["target_values"], axis=0)
             norm_residuals[i, info["active_indices"]] = residuals
```

### Comparing `datafold-1.1.6/datafold/dynfold/transform.py` & `datafold-2.0.0/datafold/dynfold/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 #!/usr/bin/env python3
 
 import itertools
-from typing import Optional, Union
+from typing import Literal, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, clone
-from sklearn.decomposition import PCA
+from sklearn.decomposition import PCA, IncrementalPCA
+from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MinMaxScaler, PolynomialFeatures, StandardScaler
-from sklearn.utils.validation import check_is_fitted, check_scalar
+from sklearn.utils.validation import NotFittedError, check_is_fitted, check_scalar
 
 from datafold.dynfold.base import TransformType, TSCTransformerMixin
-from datafold.pcfold import MultiquadricKernel, PCManifold, TSCDataFrame
-from datafold.pcfold.kernels import PCManifoldKernel
+from datafold.pcfold import TSCDataFrame
 from datafold.pcfold.timeseries.collection import TSCException
 
 
 class TSCFeaturePreprocess(BaseEstimator, TSCTransformerMixin):
     """Wrapper of a scikit-learn preprocess algorithms to allow time series
     collections as input and output.
 
     Often scikit-learn performs "pandas.DataFrame in -> numpy.ndarray out". This wrapper
     makes sure to have "pandas.DataFrame in -> pandas.DataFrame out".
 
     Parameters
     ----------
-
     sklearn_transformer
-        See `here <https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing>`_
-        for a list of possible preprocessing algorithms.
+        See `here <https://scikit-learn.org/stable/modules/classes.html#module-sklearn.
+        preprocessing>`__ for a list of possible preprocessing algorithms.
     """
 
     _cls_valid_scale_names = ("min-max", "standard")
     # flag from scikit-learn -- need to set that check_estimator is valid
     _required_parameters = ["sklearn_transformer"]
 
     def __init__(self, sklearn_transformer):
@@ -61,14 +60,19 @@
         elif name == "standard":
             return cls(StandardScaler(copy=True, with_mean=True, with_std=True))
         else:
             raise ValueError(
                 f"name='{name}' is not known. Choose from {cls._cls_valid_scale_names}"
             )
 
+    def get_feature_names_out(self, input_features=None):
+        return self.sklearn_transformer_fit_.get_feature_names_out(
+            input_features=input_features
+        )
+
     def fit(self, X: TransformType, y=None, **fit_params) -> "TSCFeaturePreprocess":
         """Calls fit of internal transform ``sklearn`` object.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data of shape `(n_samples, n_features)`.
@@ -80,29 +84,25 @@
             `None`
 
         Returns
         -------
         TSCFeaturePreprocess
             self
         """
-
         if not hasattr(self.sklearn_transformer, "transform"):
             raise AttributeError("sklearn object has no 'transform' attribute")
-
-        X = self._validate_datafold_data(X)
-        self._setup_feature_attrs_fit(X, features_out="like_features_in")
-
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
         self.sklearn_transformer_fit_ = clone(
             estimator=self.sklearn_transformer, safe=True
         )
+        self._validate_datafold_data(X)
 
-        X_intern = self._X_to_numpy(X)
-        self.sklearn_transformer_fit_.fit(X_intern)
+        self.sklearn_transformer_fit_.fit(X)
+        self._setup_feature_attrs_fit(X)
 
         return self
 
     def transform(self, X: TransformType):
         """Calls transform of internal transform ``sklearn`` object.
 
         Parameters
@@ -111,52 +111,53 @@
             Data to transform of shape `(n_samples, n_features)`.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type and shape as `X`
         """
-
         check_is_fitted(self, "sklearn_transformer_fit_")
 
         X = self._validate_datafold_data(X)
         self._validate_feature_input(X, direction="transform")
 
-        X_intern = self._X_to_numpy(X)
-        values = self.sklearn_transformer_fit_.transform(X_intern)
+        values = self.sklearn_transformer_fit_.transform(X)
         return self._same_type_X(
-            X=X, values=values, feature_names=self.feature_names_out_
+            X=X,
+            values=values,
+            feature_names=self.get_feature_names_out(),
         )
 
     def fit_transform(self, X: TransformType, y=None, **fit_params):
-        """Calls fit_transform of internal transform ``sklearn`` object..
+        """Calls fit_transform of internal transform ``sklearn`` object.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data to transform of shape `(n_samples, n_features)`.
 
         y: None
             ignored
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type and shape as `X`
         """
-
         X = self._validate_datafold_data(X)
 
-        self._setup_feature_attrs_fit(X, features_out="like_features_in")
-
         self.sklearn_transformer_fit_ = clone(self.sklearn_transformer)
         values = self.sklearn_transformer_fit_.fit_transform(X)
 
+        self._setup_feature_attrs_fit(X)
+
         return self._same_type_X(
-            X=X, values=values, feature_names=self.feature_names_out_
+            X=X,
+            values=values,
+            feature_names=self.get_feature_names_out(),
         )
 
     def inverse_transform(self, X: TransformType):
         """Calls `inverse_transform` of internal transform ``sklearn`` object.
 
         Parameters
         ----------
@@ -164,25 +165,81 @@
             Data to map back of shape `(n_samples, n_features)`.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type and shape as `X`
         """
-
         if not hasattr(self.sklearn_transformer, "inverse_transform"):
             raise AttributeError("sklearn object has no 'inverse_transform' attribute")
 
-        X_intern = self._X_to_numpy(X)
-        values = self.sklearn_transformer_fit_.inverse_transform(X_intern)
+        values = self.sklearn_transformer_fit_.inverse_transform(X)
         return self._same_type_X(
             X=X, values=values, feature_names=self.feature_names_in_
         )
 
 
+class TSCFeatureSelect(BaseEstimator, TSCTransformerMixin):
+    """A simple class to select features by name or index.
+
+    Parameters
+    ----------
+    features
+
+
+    """
+
+    def __init__(self, features: np.ndarray):
+        self.features = features
+
+    def get_feature_names_out(self, input_features=None):
+        if input_features is None and not hasattr(self, "feature_names_in_"):
+            return self.features
+        else:
+            return self.features
+
+    def fit(self, X: TransformType, y=None, **fit_params) -> "TSCFeatureSelect":
+        """Fit the model.
+
+        Parameters
+        ----------
+        X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
+            Training data of shape `(n_samples, n_features)`.
+
+        y: None
+            ignored
+
+        **fit_params: Dict[str, object]
+            `None`
+        """
+        if (
+            not isinstance(self.features, np.ndarray)
+            or self.features.ndim != 1
+            or self.features.dtype.type is not np.str_
+        ):
+            raise ValueError(
+                "parameter 'features' must be a 1-dim. array with feature names"
+            )
+        self._validate_datafold_data(X, ensure_tsc=True)
+        self._setup_feature_attrs_fit(X, n_features_out=self.features.shape[0])
+
+        try:
+            X.loc[:, self.features]
+        except KeyError:
+            raise ValueError("all features must be contained in X")
+
+        return self
+
+    def transform(self, X):
+        X = self._validate_datafold_data(X, ensure_tsc=True)
+        self._validate_feature_input(X, direction="transform")
+
+        return X.loc[:, self.features]
+
+
 class TSCIdentity(BaseEstimator, TSCTransformerMixin):
     """Transformer as a "passthrough" placeholder and/or attaching a constant feature.
 
     Parameters
     ----------
     include_const
         If True, a constant (all ones) column is attached to the data.
@@ -196,14 +253,37 @@
         True if fit has been called.
     """
 
     def __init__(self, *, include_const: bool = False, rename_features: bool = False):
         self.include_const = include_const
         self.rename_features = rename_features
 
+    def get_feature_names_out(self, input_features=None):
+        if input_features is None and hasattr(self, "feature_names_in_"):
+            features_out = self.feature_names_in_
+        else:
+            features_out = input_features
+
+        if features_out is not None:
+            if self.rename_features:
+                features_out = np.array(
+                    [f"{col}_id" for col in features_out], dtype=object
+                )
+
+            if self.include_const:
+                features_out = np.append(features_out, ["const"])
+
+        return features_out
+
+    def _more_tags(self):
+        if not self.rename_features:
+            return dict(tsc_contains_orig_states=True)
+        else:
+            return dict(tsc_contains_orig_states=False)
+
     def fit(self, X: TransformType, y=None, **fit_params):
         """Passthrough data and set internals for validation.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Data of shape `(n_samples, n_features)`.
@@ -218,32 +298,29 @@
         -------
         TSCIdentity
             self
         """
         X = self._validate_datafold_data(X)
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
-        if self._has_feature_names(X):
-            if self.rename_features:
-                features_out = np.asarray([f"{col}_id" for col in X.columns])
-            else:
-                features_out = X.columns
-
-            if self.include_const:
-                features_out = np.append(features_out, ["const"])
-        else:
-            features_out = "like_features_in"
-
-        self._setup_feature_attrs_fit(X, features_out=features_out)
+        self._setup_feature_attrs_fit(
+            X, n_features_out=X.shape[1] + int(self.include_const)
+        )
 
         # Dummy attribute to indicate that fit was called
         self.is_fit_ = True
 
         return self
 
+    def partial_fit(self, X, y=None, **fit_transform):
+        if not hasattr(self, "feature_names_in_"):
+            return self.fit(X, y, **fit_transform)
+        else:
+            return self
+
     def transform(self, X: TransformType) -> TransformType:
         """Passthrough data and validate feature.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Data of shape `(n_samples, n_features)` to passthrough.
@@ -295,25 +372,58 @@
                 X = X.drop("const", axis=1)
             else:
                 X = X[:, :-1]
 
         return X
 
 
+class TSCIncrementalPCA(IncrementalPCA, TSCTransformerMixin):  # pragma: no cover
+    # TODO: docu, tests
+
+    def __init__(self, n_components, *, whiten=False, copy=False, batch_size=None):
+        super().__init__(
+            n_components=n_components, whiten=whiten, copy=copy, batch_size=batch_size
+        )
+
+    def get_feature_names_out(self, input_features=None):
+        return np.array([f"pca{i}" for i in range(self.n_components_)], dtype=object)
+
+    def partial_fit(self, X, y=None, check_input=True):
+        super().partial_fit(X, y=y)
+
+        if self.n_samples_seen_ == X.shape[0]:
+            self._setup_feature_attrs_fit(X)
+        return self
+
+    def transform(self, X):
+        check_is_fitted(self)
+        X = self._validate_datafold_data(X)
+
+        self._validate_feature_input(X, direction="transform")
+        pca_data = super(IncrementalPCA, self).transform(X)
+        return self._same_type_X(
+            X, values=pca_data, feature_names=self.get_feature_names_out()
+        )
+
+
 class TSCPrincipalComponent(PCA, TSCTransformerMixin):
     """Compute principal components from data.
 
     This is a subclass of scikit-learn's ``PCA``  to generalize the
     input and output of :class:`pandas.DataFrames` and :class:`.TSCDataFrame`. All input
     parameters remain the same. For documentation please visit:
 
-    * `PCA docu <https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html>`_
-    * `PCA user guide <https://scikit-learn.org/stable/modules/decomposition.html#pca>`_
+    * `PCA docu <https://scikit-learn.org/stable/modules/generated/sklearn.
+      decomposition.PCA.html>`__
+    * `PCA user guide <https://scikit-learn.org/stable/modules/decomposition.html#pca>`__
     """
 
+    def get_feature_names_out(self, input_features=None):
+        return np.array([f"pca{i}" for i in range(self.n_components_)], dtype=object)
+
     def fit(self, X: TransformType, y=None, **fit_params) -> "PCA":
         """Compute the principal components from training data.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data of shape `(n_samples, n_features)`.
@@ -325,25 +435,20 @@
             None
 
         Returns
         -------
         TSCPrincipalComponent
             self
         """
-
         X = self._validate_datafold_data(X)
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
-        # validation happens here:
-        super(TSCPrincipalComponent, self).fit(self._X_to_numpy(X), y=y)
-
-        self._setup_feature_attrs_fit(
-            X, features_out=[f"pca{i}" for i in range(self.n_components_)]
-        )
-
+        # validation happens in super.fit()
+        super().fit(X, y=y)
+        self._setup_feature_attrs_fit(X)
         return self
 
     def transform(self, X: TransformType):
         """Apply dimension reduction by projecting the data on principal components.
 
         Parameters
         ----------
@@ -352,22 +457,22 @@
             reduction on.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_components_)`
         """
-
         check_is_fitted(self)
         X = self._validate_datafold_data(X)
 
         self._validate_feature_input(X, direction="transform")
-        pca_data = super(TSCPrincipalComponent, self).transform(self._X_to_numpy(X))
+        pca_data = super().transform(X)
+
         return self._same_type_X(
-            X, values=pca_data, feature_names=self.feature_names_out_
+            X, values=pca_data, feature_names=self.get_feature_names_out()
         )
 
     def fit_transform(self, X: TransformType, y=None, **fit_params) -> TransformType:
         """Compute principal components from data and reduce dimension on same data.
 
         Parameters
         ----------
@@ -378,27 +483,20 @@
             ignored
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_components_)`
         """
-
         X = self._validate_datafold_data(X)
-
-        pca_values = super(TSCPrincipalComponent, self).fit_transform(
-            self._X_to_numpy(X), y=y
-        )
-
-        self._setup_feature_attrs_fit(
-            X, features_out=[f"pca{i}" for i in range(self.n_components_)]
-        )
+        pca_values = super().fit_transform(X, y=y)
+        self._setup_feature_attrs_fit(X)
 
         return self._same_type_X(
-            X, values=pca_values, feature_names=self.feature_names_out_
+            X, values=pca_values, feature_names=self.get_feature_names_out()
         )
 
     def inverse_transform(self, X: TransformType):
         """Map data from the reduced space back to the original space.
 
         Parameters
         ----------
@@ -407,108 +505,100 @@
             original space.
 
         Returns
         -------
         TSCDataFrame, pandas.DataFrame, numpy.ndarray
             same type as `X` of shape `(n_samples, n_features)`
         """
-
         self._validate_feature_input(X, direction="inverse_transform")
 
-        X_intern = self._X_to_numpy(X)
-        data_orig_space = super(TSCPrincipalComponent, self).inverse_transform(X_intern)
+        data_orig_space = super().inverse_transform(X)
 
         return self._same_type_X(
             X, values=data_orig_space, feature_names=self.feature_names_in_
         )
 
 
 class TSCTakensEmbedding(BaseEstimator, TSCTransformerMixin):
     r"""Perform Takens time delay embedding on time series collection data.
 
     Parameters
     ----------
-
     delays
         Number for time delays to embed.
 
     lag
         Number of time steps to lag before embedding starts.
 
     frequency
         Time step frequency to emebd (e.g. to embed every sample or only every second
         or third).
 
     kappa
         Weight of exponential factor in delayed coordinates
         :math:`e^{-d \cdot \kappa}(x_{-d})` with :math:`d = 0, \ldots delays` being the
-        delay index. Adapted from :cite:`berry_time-scale_2013`, Eq. 2.1).
+        delay index. Adapted from :cite:t:`berry-2013`, Eq. 2.1).
 
     Attributes
     ----------
-
     delay_indices_ : numpy.ndarray
         Delay indices (backwards in time) assuming a fixed time delta in the time series.
 
     min_timesteps_: int
         Minimum required time steps for each time series to have a single embedding
         vector.
 
     delta_time_fit_
         Time delta measured during model fit. This is primarily used to check that
         `transform` or `inverse_transform` data still have the same time delta for
         consistency.
 
     References
     ----------
-
-    * Original paper from Takens :cite:`takens_detecting_1981`
-    * Generalized to multiple observation :cite:`deyle_generalized_2011`
-    * time delay embedding in the context of Koopman operator, e.g.
-      :cite:`arbabi_ergodic_2017` or :cite:`champion_discovery_2019` or
+    * Original paper from :cite:t:`takens-1981`
+    * Generalized to multiple observation in :cite:`deyle-2011`
+    * time delay embedding in the context of Koopman operator theory, e.g.
+      :cite:t:`arbabi-2017` or :cite:t:`champion-2019`.
     """
 
     def __init__(
         self, delays: int = 10, *, lag: int = 0, frequency: int = 1, kappa: float = 0
     ):
         self.lag = lag
         self.delays = delays
         self.frequency = frequency
         self.kappa = kappa
 
-    def _validate_parameter(self):
+    def _more_tags(self):
+        return dict(tsc_contains_orig_states=True)
 
-        check_scalar(
-            self.lag, name="lag", target_type=(int, np.integer), min_val=0, max_val=None
-        )
+    def _validate_parameter(self):
+        check_scalar(self.lag, name="lag", target_type=(int, np.integer), min_val=0)
 
         # TODO also allow 0 delays? This would only "passthrough",
         #  but makes it is easier in pipelines etc.
         check_scalar(
             self.delays,
             name="delays",
             target_type=(int, np.integer),
             min_val=1,
-            max_val=None,
         )
 
         check_scalar(
             self.frequency,
             name="delays",
             target_type=(int, np.integer),
             min_val=1,
-            max_val=None,
         )
 
         check_scalar(
             self.kappa,
             name="kappa",
             target_type=(int, np.integer, float, np.floating),
             min_val=0.0,
-            max_val=None,
         )
 
         if self.frequency > 1 and self.delays <= 1:
             raise ValueError(
                 f"If frequency (={self.frequency} is larger than 1, "
                 f"then number for delays (={self.delays}) has to be larger "
                 "than 1)."
@@ -525,26 +615,31 @@
     def _columns_to_type_str(self, X):
         # in case the column in not string it is important to transform it here to
         # string. Otherwise, There are mixed types (e.g. int and str), because the
         # delayed columns are all strings to indicate the delay number.
         X.columns = X.columns.astype(np.str_)
         return X
 
-    def _expand_all_delay_columns(self, cols):
+    def get_feature_names_out(self, input_features=None):
+        if input_features is None:
+            input_features = self.feature_names_in_
+
         def expand():
             delayed_columns = list()
             for delay_idx in self.delay_indices_:
                 # rename columns: [column_name]:d[delay_index]
-                _cur_delay_columns = [f"{col}:d{delay_idx}" for col in cols.astype(str)]
+                _cur_delay_columns = [
+                    f"{col}:d{delay_idx}" for col in input_features.astype(str)
+                ]
                 delayed_columns.append(_cur_delay_columns)
             return delayed_columns
 
         # the name of the original indices is not changed, therefore append the delay
         # indices to
-        columns_names = cols.tolist() + list(itertools.chain(*expand()))
+        columns_names = input_features.tolist() + list(itertools.chain(*expand()))
 
         return pd.Index(
             columns_names,
             dtype=np.str_,
             copy=False,
             name=TSCDataFrame.tsc_feature_col_name,
         )
@@ -589,17 +684,45 @@
         )
 
         X = self._columns_to_type_str(X)
 
         # save delta time during fit to check that time series collections in
         # transform have the same delta time
         self.delta_time_fit_ = X.delta_time
+        self._setup_feature_attrs_fit(X)
+
+        return self
+
+    def partial_fit(
+        self, X: TransformType, y=None, **fit_params
+    ) -> "TSCTakensEmbedding":
+        """# TODO.
+
+        Parameters
+        ----------
+        X
+        y
+        fit_params
+
+        Returns
+        -------
 
-        features_out = self._expand_all_delay_columns(X.columns)
-        self._setup_feature_attrs_fit(X, features_out=features_out)
+        """
+        try:
+            check_is_fitted(self)
+            # there is no real model update needed, just check if the data still complies with
+            # the data used during the initial fit
+            self._validate_datafold_data(
+                X,
+                ensure_tsc=True,
+                tsc_kwargs=dict(ensure_delta_time=self.delta_time_fit_),
+            )
+        except NotFittedError:
+            # fit the model
+            self.fit(X, y, **fit_params)
 
         return self
 
     def transform(self, X: TSCDataFrame) -> TSCDataFrame:
         """Perform Takens time delay embedding for each time series in the collection.
 
         Parameters
@@ -618,31 +741,29 @@
         Raises
         ------
         TSCException
             Time series collection requirements in `X`: (1) time delta must be constant
             (2) all time series must have the minimum number of time samples to obtain
             one sample in the time delay embedding.
         """
-
         X = self._validate_datafold_data(
             X,
             tsc_kwargs={
                 # must be same time delta as during fit
                 "ensure_delta_time": self.delta_time_fit_,
                 "ensure_min_timesteps": self.min_timesteps_,
             },
             ensure_tsc=True,
         )
 
         X = self._columns_to_type_str(X)
         self._validate_feature_input(X, direction="transform")
 
-        #################################
-        ### Implementation using pandas by using shift()
-        ### This implementation is better readable, and is for many cases similarly
+        # Implementation using pandas by using shift()
+        # This implementation is better readable, and is for many cases similarly
         # fast to the numpy version (below), but has a performance drop for
         # high-dimensions (dim>500)
         # id_groupby = X.groupby(TSCDataFrame.IDX_ID_NAME)
         # concat_dfs = [X]
         #
         # for delay_idx in self.delay_indices_:
         #     shifted_data = id_groupby.shift(delay_idx, fill_value=np.nan)
@@ -652,16 +773,15 @@
         # X = pd.concat(concat_dfs, axis=1)
 
         # if self.fillin_handle == "remove":
         #     # _TODO: use pandas.dropna()
         #     bool_idx = np.logical_not(np.sum(pd.isnull(X), axis=1).astype(np.bool))
         #     X = X.loc[bool_idx]
 
-        # Implementation using numpy functions.
-
+        # Implementation using numpy functions:
         # pre-allocate list
         delayed_timeseries = [pd.DataFrame([])] * len(X.ids)
 
         max_delay = max(self.delay_indices_)
 
         if self.kappa > 0:
             # only the delayed coordinates are multiplied with the exp factor
@@ -670,15 +790,14 @@
             # the np.repeat assumes the following pattern:
             # (a,b), (a:d1, b:d1), (a:d2, b:d2), ...
             kappa_vec = np.repeat(kappa_vec, self.n_features_in_)
         else:
             kappa_vec = None
 
         for idx, (_, df) in enumerate(X.groupby(TSCDataFrame.tsc_id_idx_name)):
-
             # use time series numpy block
             time_series_numpy = df.to_numpy()
 
             # max_delay determines the earliest sample that has no fill-in
             original_data = time_series_numpy[max_delay:, :]
 
             # select the data (row_wise) for each delay block
@@ -695,17 +814,16 @@
                 delayed_data = delayed_data.astype(float)
                 delayed_data *= kappa_vec
 
             # go back to DataFrame, and adapt the index by excluding removed indices
             df = pd.DataFrame(
                 np.hstack([original_data, delayed_data]),
                 index=df.index[max_delay:],
-                columns=self.feature_names_out_,
+                columns=self.get_feature_names_out(self.feature_names_in_),
             )
-
             delayed_timeseries[idx] = df
 
         X = TSCDataFrame(pd.concat(delayed_timeseries, axis=0))
         return X
 
     def inverse_transform(self, X: TransformType) -> TransformType:
         """Remove time delayed feature columns of time delay embedded time series
@@ -725,71 +843,274 @@
 
         X = self._validate_datafold_data(X, ensure_tsc=True)
         self._validate_feature_input(X, direction="inverse_transform")
 
         return X.loc[:, self.feature_names_in_]
 
 
+class TSCSampledNetwork(BaseEstimator, TSCTransformerMixin):  # pragma: no cover
+    """
+    This is a simple wrapper for sampled neural networks.
+
+    Parameters
+    ----------
+    nn
+        A sklearn pipeline that represents the neural network (containing ``Dense``, ``Linear``
+        layers, etc. from the ``swimnetwork`` Python package). Note the pipleline
+        should not be fitted yet.
+
+
+    References
+    ----------
+    See :cite:t:`bolager-2023` for the paper on sampled networks and the
+    gitlab repository `swimnetworks <https://gitlab.com/felix.dietrich/swimnetworks>`__
+
+    To install the package run
+
+    .. code-block::
+
+        pip install git+https://github.com/https://gitlab.com/felix.dietrich/swimnetworks
+
+    """
+
+    def __init__(
+        self,
+        nn: Pipeline,
+    ):
+        self.nn = nn
+
+    def __repr__(self):
+        # TODO: somehow the repr of the original implementation is quite costly
+        #    (investigate why and propose a fix)
+        return "SWIM NETWORK"
+
+    def get_feature_names_out(self, input_features=None):
+        n_features_out = self.nn[-1].weights.shape[1]
+        return [f"w{i}" for i in range(n_features_out)]
+
+    def fit(self, X: TSCDataFrame) -> "TSCSampledNetwork":
+        self._validate_datafold_data(X=X)
+
+        if self.nn[-1].weights is None:
+            Xm, Xp = X.tsc.shift_matrices(snapshot_orientation="row")
+            self.nn = self.nn.fit(Xm, Xp)
+        else:
+            pass
+
+        # must be setup only *after* the network is fitted
+        self._setup_feature_attrs_fit(X)
+        return self
+
+    def transform(self, X: TSCDataFrame):
+        self._validate_feature_input(X=X, direction="transform")
+
+        X_return = self.nn.transform(X.to_numpy())
+        X_return = TSCDataFrame.from_same_indices_as(
+            X, X_return, except_columns=self.get_feature_names_out()
+        )
+
+        return X_return
+
+
+class FourierRBF(BaseEstimator, TSCTransformerMixin):  # pragma: no cover
+    def __init__(self, n_features=100, sigma=1):
+        self.n_features = n_features
+        self.sigma = sigma
+
+    def get_feature_names_out(self, input_features=None):
+        sin = [f"sin{i}" for i in range(self.n_features)]
+        cos = [f"cos{i}" for i in range(self.n_features)]
+        return pd.Index(sin + cos)
+
+    def fit(self, X, y=None, **fit_params):
+        self._setup_feature_attrs_fit(X, n_features_out=2 * self.n_features)
+
+        # sample features components
+        self.fourier_components_ = np.zeros([X.shape[1], self.n_features])
+
+        mean = np.zeros(X.shape[1])
+        cov = np.identity(X.shape[1]) / self.sigma**2
+
+        rng = np.random.default_rng(1)
+
+        for d in range(self.n_features):
+            self.fourier_components_[:, d] = rng.multivariate_normal(mean, cov)
+
+        return self
+
+    def partial_fit(self, X, y, **fit_params):
+        if not hasattr(self, "fourier_components_"):
+            return self.fit(X, y, **fit_params)
+        else:
+            return self
+
+    def transform(self, X):
+        mc_samples = np.dot(X.to_numpy(), self.fourier_components_)
+        all_samples = np.zeros([X.shape[0], 2 * self.n_features])
+        all_samples[:, : self.n_features] = np.sin(mc_samples)
+        all_samples[:, self.n_features :] = np.cos(mc_samples)
+
+        return TSCDataFrame.from_same_indices_as(
+            indices_from=X,
+            values=all_samples,
+            except_columns=self.get_feature_names_out(),
+        )
+
+
+class TSCMovingAverage(BaseEstimator, TSCTransformerMixin):
+    """Compute the moving average for each feature of a time series.
+
+    window
+        The window size on which the moving average is computed.
+
+    # TODO: this is not official
+    # TODO: could wrap functionality of https://github.com/cerlymarco/tsmoothie
+    #   here to smooth time series
+    """
+
+    def __init__(self, window: int = 3):
+        self.window = window
+
+    def get_feature_names_out(self, input_features=None):
+        if input_features is None:
+            try:
+                input_features = self.feature_names_in_
+            except AttributeError:
+                raise NotFittedError
+
+        return [f"{n}_ma{self.window}" for n in input_features]
+
+    def fit(self, X: TSCDataFrame, **fit_params):
+        """Fit the model.
+
+        Parameters
+        ----------
+        X
+            Time series collection data
+
+        **fit_params
+            None
+
+        Returns
+        -------
+        self
+        """
+        check_scalar(self.window, "window", target_type=int, min_val=1)
+
+        self._read_fit_params(attrs=None, fit_params=fit_params)
+        self._validate_datafold_data(
+            X,
+            ensure_tsc=True,
+            ensure_min_samples=self.window,
+            tsc_kwargs=dict(ensure_const_delta_time=True),
+        )
+        self._setup_feature_attrs_fit(X, n_features_out=len(X.columns))
+
+        return self
+
+    def transform(self, X: TSCDataFrame):
+        """Transform time series data.
+
+        Parameters
+        ----------
+        X
+            Time series collection data.
+
+        Returns
+        -------
+        TSCDataFrame
+            The number of samples in each time series reduce according to the ``window``
+            parameter.
+        """
+        self._validate_datafold_data(
+            X,
+            ensure_tsc=True,
+            ensure_min_samples=self.window,
+            tsc_kwargs=dict(ensure_const_delta_time=True),
+        )
+        self._validate_feature_input(X, direction="transform")
+
+        X_new = (
+            pd.DataFrame(X)
+            .groupby(TSCDataFrame.tsc_id_idx_name)
+            .rolling(window=self.window)
+            .mean()
+            .dropna()
+        )
+        X_new = TSCDataFrame(X_new.droplevel(0))
+        X_new.columns = pd.Index(self.get_feature_names_out())
+
+        return X_new
+
+
 class TSCRadialBasis(BaseEstimator, TSCTransformerMixin):
     """Represent data in coefficients of radial basis functions.
 
     Parameters
     ----------
-
     kernel
         Radial basis kernel to compute the coefficients with. Defaults to
         :code:`MultiquadricKernel(epsilon=1.0)`.
 
     center_type
         Selection of what to take as centers during fit.
 
         * `all_data` - all data points during fit are used as centers
+        * `random` - subsample `n_samples` samples from the dataset and use as
+           centers.
         * `fit_params` - set the center points with keyword arguments during fit
         * `initial_condition` - take the initial condition states as centers.
            Note for this option the data `X` during fit must be of
            type :class:`.TSCDataFrame`.
 
+    n_samples
+        Number of sub-samples to use. Parameter is only considered if `center_type=random`.
+
     exact_distance
         An inexact distance computation increases computational performance at the cost of
         numerical inaccuracies (~1e-7 for Euclidean distance, and ~1 e-14 for squared
         Eucledian distance).
 
     Attributes
     ----------
-
     centers_: numpy.ndarray
         The center points of the radial basis functions.
 
     inv_coeff_matrix_: numpy.ndarray
         Matrix to map radial basis coefficients to original space. Computation is
         delayed until `inverse_transform` is called for the first time.
     """
 
-    _cls_valid_center_types = ["all_data", "fit_params", "initial_condition"]
+    _cls_valid_center_types = ["all_data", "random", "fit_params", "initial_condition"]
+    _required_parameters = ["kernel"]
 
     def __init__(
         self,
-        kernel: Optional[PCManifoldKernel] = None,
+        kernel,
         *,  # keyword-only
-        center_type: str = "all_data",
+        center_type: Literal[
+            "all_data", "random", "fit_params", "inital_condition"
+        ] = "all_data",
+        n_samples: int = 100,
         exact_distance=True,
     ):
         self.kernel = kernel
         self.center_type = center_type
+        self.n_samples = n_samples
         self.exact_distance = exact_distance
 
     def _validate_center_type(self, center_type):
         if center_type not in self._cls_valid_center_types:
             raise ValueError(
                 f"center_type={center_type} not valid. Choose from "
                 f"{self._cls_valid_center_types} "
             )
 
-    def _get_default_kernel(self):
-        return MultiquadricKernel(epsilon=1.0)
+    def get_feature_names_out(self, feature_names_in=None):
+        return np.array([f"rbf{i}" for i in range(self.centers_.shape[0])])
 
     def fit(self, X: TransformType, y=None, **fit_params) -> "TSCRadialBasis":
         """Set the point centers of the radial basis functions.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
@@ -805,64 +1126,67 @@
                 `center_type="fit_params"` must be set during initialization.
 
         Returns
         -------
         TSCRadialBasis
             self
         """
-
         X = self._validate_datafold_data(X)
         self._validate_center_type(center_type=self.center_type)
         _centers = self._read_fit_params(
             attrs=[("centers", None)], fit_params=fit_params
         )
 
         if self.center_type == "all_data":
             if _centers is not None:
-                raise ValueError("center points were passed but center_type='all_data'")
+                raise ValueError(
+                    "center points were passed but center_type='all_data'"
+                    "was set during model init"
+                )
 
             self.centers_ = self._X_to_numpy(X)
-        elif self.center_type == "fit_params":
+        elif self.center_type == "random":
+            if self.n_samples > X.shape[0]:
+                raise ValueError(
+                    f"{self.n_samples=} is greater than the number of samples in the "
+                    f"dataset ({X.shape[0]=})"
+                )
 
+            rng = np.random.default_rng(1)  # TODO: possibly make a parameter
+            idx_samples = rng.choice(
+                range(0, X.shape[0]), size=self.n_samples, replace=False
+            )
+            self.centers_ = self._X_to_numpy(X)[idx_samples, :]
+
+        elif self.center_type == "fit_params":
             if _centers is None:
                 raise ValueError("The center points were not provided in 'fit_params'.")
 
             try:
                 self.centers_ = np.asarray(_centers).astype(float)
             except TypeError:
                 raise TypeError(
                     "centers were not passed to fit_params or not array-like."
                 )
 
             if self.centers_.ndim != 2 or self.centers_.shape[1] != X.shape[1]:
                 raise ValueError(
-                    "The center points must be a matrix with same point "
-                    "dimension than 'X'."
+                    f"The center points (={self.centers_.shape[1]}) must be a two dimensional "
+                    f"array with the same point dimension in 'X' (={X.shape[1]})."
                 )
         elif self.center_type == "initial_condition":
             if not isinstance(X, TSCDataFrame):
                 raise TypeError("'X' must be of type TSCDataFrame.")
             self.centers_ = X.initial_states().to_numpy()
         else:
             raise RuntimeError(
                 "center_type was not checked correctly. Please report bug."
             )
 
-        set_kernel = (
-            self.kernel if self.kernel is not None else self._get_default_kernel()
-        )
-
-        self.centers_ = PCManifold(
-            self.centers_,
-            kernel=set_kernel,
-            dist_kwargs=dict(backend="brute", exact_numeric=self.exact_distance),
-        )
-
-        n_centers = self.centers_.shape[0]
-        self._setup_feature_attrs_fit(X, [f"rbf{i}" for i in range(n_centers)])
+        self._setup_feature_attrs_fit(X)
 
         return self
 
     def transform(self, X: TransformType) -> TransformType:
         """Transform data to radial basis functions coefficients.
 
         Parameters
@@ -876,18 +1200,18 @@
             same type as `X` of shape `(n_samples, n_centers)`
         """
         check_is_fitted(self, attributes=["centers_"])
         X = self._validate_datafold_data(X)
         self._validate_feature_input(X, direction="transform")
 
         X_intern = self._X_to_numpy(X)
-        rbf_coeff = self.centers_.compute_kernel_matrix(Y=X_intern)
+        rbf_coeff = self.kernel(self.centers_, X_intern)
 
         return self._same_type_X(
-            X, values=rbf_coeff, feature_names=self.feature_names_out_
+            X, values=rbf_coeff, feature_names=self.get_feature_names_out()
         )
 
     def fit_transform(self, X, y=None, **fit_params):
         """Set the data as centers and transform to radial basis coefficients.
 
         Parameters
         ----------
@@ -905,21 +1229,21 @@
         """
         self.fit(X, **fit_params)
         X_intern = self._X_to_numpy(X)
         self._validate_center_type(center_type=self.center_type)
 
         if self.center_type == "all_data":
             # compute pdist distance matrix, which is often more efficient
-            rbf_coeff = self.centers_.compute_kernel_matrix()
+            rbf_coeff = self.kernel(X)
         else:  # self.center_type in ["initial_condition", "fit_params"]:
-            rbf_coeff = self.centers_.compute_kernel_matrix(Y=X_intern)
+            rbf_coeff = self.kernel(self.centers_, X_intern)
 
         # import matplotlib.pyplot as plt; plt.matshow(rbf_coeff)
         return self._same_type_X(
-            X=X, values=rbf_coeff, feature_names=self.feature_names_out_
+            X=X, values=rbf_coeff, feature_names=self.get_feature_names_out()
         )
 
     def inverse_transform(self, X: TransformType):
         """Transform radial basis coefficients back to the original function values.
 
         Parameters
         ----------
@@ -937,15 +1261,15 @@
         if self._has_feature_names(X):
             rbf_coeff = X.to_numpy()
         else:
             rbf_coeff = X
 
         if not hasattr(self, "inv_coeff_matrix_"):
             # save inv_coeff_matrix_
-            center_kernel = self.centers_.compute_kernel_matrix()
+            center_kernel = self.kernel(self.centers_)
             self.inv_coeff_matrix_ = np.linalg.lstsq(
                 center_kernel, self.centers_, rcond=None
             )[0]
 
         X_inverse = rbf_coeff @ self.inv_coeff_matrix_
         return self._same_type_X(
             X, values=X_inverse, feature_names=self.feature_names_in_
@@ -957,54 +1281,58 @@
 
     This is a subclass of ``PolynomialFeatures`` from scikit-learn to generalize the
     input and output of :class:`pandas.DataFrames` and :class:`.TSCDataFrame`.
 
     This class adds the parameter `include_first_order` to choose whether to include the
     identity states. For all other parameters please visit the super class
     documentation of
-    `PolynomialFeatures <https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.PolynomialFeatures.html>`_.
+    `PolynomialFeatures <https://scikit-learn.org/stable/modules/generated/sklearn.
+    preprocessing.PolynomialFeatures.html>`__.
     """
 
     def __init__(
         self,
         degree: int = 2,
         *,  # keyword-only
         interaction_only: bool = False,
         include_bias: bool = False,
         include_first_order=False,
     ):
         self.include_first_order = include_first_order
 
-        super(TSCPolynomialFeatures, self).__init__(
+        super().__init__(
             degree=degree,
             interaction_only=interaction_only,
             include_bias=include_bias,
             order="C",
         )
 
     @property
     def powers_(self):
-        powers = super(TSCPolynomialFeatures, self).powers_
+        powers = super().powers_
         if self.include_first_order:
             return powers
         else:
             return powers[powers.sum(axis=1) != 1, :]
 
+    def _more_tags(self):
+        return dict(tsc_contains_orig_states=self.include_first_order)
+
     def _get_poly_feature_names(self, X, input_features=None):
         # Note: get_feature_names function is already provided by super class
         if self._has_feature_names(X):
-            feature_names = self.get_feature_names(
+            feature_names = self.get_feature_names_out(
                 input_features=X.columns.astype(np.str_)
             )
         else:
             feature_names = self.get_feature_names()
         return feature_names
 
     def _non_id_state_mask(self):
-        powers = super(TSCPolynomialFeatures, self).powers_
+        powers = super().powers_
         return powers.sum(axis=1) != 1
 
     def fit(self, X: TransformType, y=None, **fit_params) -> "TSCPolynomialFeatures":
         """Compute number of output features.
 
         Parameters
         ----------
@@ -1021,23 +1349,26 @@
         -------
         TSCPolynomialFeatures
             self
         """
         X = self._validate_datafold_data(X)
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
-        super(TSCPolynomialFeatures, self).fit(X, y=y)
-
-        self._setup_feature_attrs_fit(
-            X,
-            features_out=self._get_poly_feature_names(X),
-        )
+        super().fit(X, y=y)
+        self._setup_feature_attrs_fit(X)
 
         return self
 
+    def partial_fit(self, X: TransformType, y=None, **fit_params):
+        if not hasattr(self, "feature_names_in_"):
+            # is fit already
+            return self.fit(X, y=None, **fit_params)
+        else:
+            return self
+
     def transform(self, X: TransformType) -> TransformType:
         """Transform data to polynomial features.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             The data of shape `(n_samples, n_features)` to transform.
@@ -1048,21 +1379,25 @@
             Transformed data of shape `(n_samples, n_polynomials)` and with same type
             as `X`.
         """
         check_is_fitted(self)
         X = self._validate_datafold_data(X)
         self._validate_feature_input(X, direction="transform")
 
-        poly_data = super(TSCPolynomialFeatures, self).transform(X)
+        poly_data = super().transform(X)
 
         if not self.include_first_order:
             poly_data = poly_data[:, self._non_id_state_mask()]
 
         poly_data = self._same_type_X(
-            X, values=poly_data, feature_names=self._get_poly_feature_names(X)
+            X,
+            values=poly_data,
+            feature_names=self.get_feature_names_out(
+                input_features=self.feature_names_in_
+            ),
         )
 
         return poly_data
 
 
 class TSCApplyLambdas(BaseEstimator, TSCTransformerMixin):
     """Transform data in an element-by-element fashion with lambda functions.
@@ -1089,18 +1424,30 @@
 
     def __init__(self, lambdas):
         self.lambdas = lambdas
 
     def _not_implemented_numpy_arrays(self, X):
         if isinstance(X, np.ndarray):
             raise NotImplementedError(
-                "Currently not implemented for numpy.ndarray. If this is required please "
+                "Currently not implemented for np.ndarray. If this is required please "
                 "open an issue on Gitlab."
             )
 
+    def get_feature_names_out(self, feature_names_in=None):
+        if feature_names_in is None:
+            feature_names_in = self.feature_names_in_
+
+        return np.array(
+            [
+                f"{feature_name}_lambda{i}"
+                for feature_name in feature_names_in
+                for i in range(len(self.lambdas))
+            ]
+        )
+
     def fit(self, X: TransformType, y=None, **fit_params) -> "TSCApplyLambdas":
         """Set internal feature information.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Training data.
@@ -1116,21 +1463,15 @@
         TSCApplyLambdas
             self
         """
         self._not_implemented_numpy_arrays(X)
         X = self._validate_datafold_data(X, ensure_tsc=True)
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
-        features_out = [
-            f"{feature_name}_lambda{i}"
-            for feature_name in X.columns
-            for i in range(len(self.lambdas))
-        ]
-
-        self._setup_feature_attrs_fit(X, features_out=features_out)
+        self._setup_feature_attrs_fit(X)
         return self
 
     def transform(self, X: TransformType) -> TransformType:
         """Transform data with specified lambda functions.
 
         Parameters
         ----------
@@ -1148,15 +1489,14 @@
         check_is_fitted(self)
         X = self._validate_datafold_data(X, ensure_tsc=True)
         self._validate_feature_input(X, direction="transform")
 
         lambdas_applied = list()
 
         for i, _lambda in enumerate(self.lambdas):
-
             lambda_result = X.apply(func=_lambda, axis=0, raw=True)
             lambda_result.columns = pd.Index(
                 [f"{feature_name}_lambda{i}" for feature_name in X.columns]
             )
 
             lambdas_applied.append(lambda_result)
 
@@ -1175,49 +1515,56 @@
     .. note::
         The class internally uses the Python package findiff, which currently is
         optional in *datafold*. The class raises an `ImportError` if findiff is not
         installed.
 
     Parameters
     ----------
-
     spacing: Union[str, float]
         The time difference between samples. If "dt" (str) then the time sampling
         frequency of a :meth:`.TSCDataFrame.delta_time` is used during fit.
 
+    scheme
+        The finite difference scheme to apply, "center", "backward" or "forward".
+
     diff_order
         The derivative order.
 
     accuracy
         The convergence order of the finite difference scheme.
 
     Attributes
     ----------
-
     spacing_
         The resolved time difference between samples. Equals the parameter
         input if it was of type :class`float`.
 
     See Also
     --------
     `findiff documentation <https://findiff.readthedocs.io/en/latest/>`_
     """
 
     def __init__(
         self,
         *,  # keyword-only
-        spacing: Union[str, float] = "dt",
+        spacing: Union[Literal["dt"], float] = "dt",
+        scheme: Literal["backward", "center", "forward"] = "center",
         diff_order: int = 1,
         accuracy: int = 2,
     ):
-
         self.spacing = spacing
+        self.scheme = scheme
         self.diff_order = diff_order
         self.accuracy = accuracy
 
+    def get_feature_names_out(self, input_features=None):
+        if input_features is None:
+            input_features = self.feature_names_in_
+        return [f"{col}_dot" for col in input_features]
+
     def fit(self, X: TransformType, y=None, **fit_params) -> "TSCFiniteDifference":
         """Set and validate time spacing between samples.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Data of shape `(n_samples, n_features)`.
@@ -1238,80 +1585,76 @@
         TSCException
             If time series data has not a constant time delta or the input `X` has not
             the same value as specified in `spacing` during initialization.
 
         """
         X = self._validate_datafold_data(
             X,
-            ensure_tsc=False,
+            ensure_tsc=True,
             tsc_kwargs=dict(
                 ensure_delta_time=self.spacing
                 if isinstance(self.spacing, float)
                 else None
             ),
         )
 
         self._read_fit_params(attrs=None, fit_params=fit_params)
 
-        if self._has_feature_names(X):
-            features_out = [f"{col}_dot" for col in X.columns]
-        else:
-            features_out = X.shape[1]
-
-        self._setup_feature_attrs_fit(X=X, features_out=features_out)
+        self._setup_feature_attrs_fit(X=X)
 
         if self.spacing == "dt":
             if not isinstance(X, TSCDataFrame):
                 raise TypeError(
                     "For input 'spacing=dt' a time series collections is required."
                 )
 
             self.spacing_ = X.delta_time
 
             if isinstance(self.spacing_, pd.Series) or np.isnan(self.spacing_):
                 raise TSCException.not_const_delta_time(actual_delta_time=self.spacing_)
         else:
+            check_scalar(
+                x=self.spacing,
+                target_type=(float, int),
+                min_val=0,
+                include_boundaries="right",
+            )
             self.spacing_ = self.spacing
 
-            if (
-                isinstance(X, TSCDataFrame)
-                and np.asarray(self.spacing_ != X.delta_time).all()
-            ):
-                raise ValueError(
-                    f"A spacing of {self.spacing} was specified, but the time series "
-                    f"collection has a time delta of {X.delta_time}"
-                )
-
         check_scalar(
             self.spacing_,
             "spacing",
             target_type=(int, np.integer, float, np.floating),
-            min_val=np.finfo(float).eps,
-            max_val=None,
+            min_val=0,
+            include_boundaries="neither",
         )
         self.spacing_ = float(self.spacing_)
 
         check_scalar(
             self.diff_order,
             "diff_order",
             target_type=(int, np.integer),
             min_val=1,
-            max_val=None,
         )
 
         check_scalar(
             self.accuracy,
             name="accuracy",
             target_type=(int, np.integer),
             min_val=1,
-            max_val=None,
         )
 
         return self
 
+    def partial_fit(self, X: TransformType, y=None, **fit_params) -> TransformType:
+        if not hasattr(self, "feature_names_in_"):
+            return self.fit(X, y, **fit_params)
+        else:
+            return self
+
     def transform(self, X: TransformType) -> TransformType:
         """Compute the finite difference values.
 
         Parameters
         ----------
         X: TSCDataFrame, pandas.DataFrame, numpy.ndarray
             Data of shape `(n_samples, n_features)`.
@@ -1332,14 +1675,14 @@
             ensure_tsc=True,
             tsc_kwargs=dict(ensure_delta_time=self.spacing_),
         )
 
         self._validate_feature_input(X=X, direction="transform")
 
         time_derivative = X.tsc.time_derivative(
-            scheme="center",
+            scheme=self.scheme,
             diff_order=self.diff_order,
             accuracy=self.accuracy,
             shift_index=True,
         )
         time_derivative = time_derivative.add_suffix(f"_dot{self.diff_order}")
         return time_derivative
```

### Comparing `datafold-1.1.6/datafold/pcfold/__init__.py` & `datafold-2.0.0/datafold/pcfold/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from datafold.pcfold.kernels import (
     ConeKernel,
     ContinuousNNKernel,
     CubicKernel,
     DmapKernelFixed,
     GaussianKernel,
     InverseMultiquadricKernel,
+    InverseQuadraticKernel,
     MultiquadricKernel,
     PCManifoldKernel,
     QuinticKernel,
 )
 from datafold.pcfold.pointcloud import (
     PCManifold,
     estimate_cutoff,
```

### Comparing `datafold-1.1.6/datafold/pcfold/distance.py` & `datafold-2.0.0/datafold/pcfold/distance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
-
 import abc
-from typing import Optional, Sequence, Type, Union
+import inspect
+from copy import deepcopy
+from typing import Optional, Union
 
 import numpy as np
 import scipy.sparse
 import scipy.spatial
 from scipy.spatial.distance import cdist, pdist, squareform
 from sklearn.metrics import pairwise_distances
-from sklearn.neighbors import BallTree, NearestNeighbors
+from sklearn.neighbors import BallTree, KNeighborsTransformer, NearestNeighbors
+from sklearn.utils.validation import check_scalar
 
 from datafold.utils.general import if1dim_colvec, if1dim_rowvec, is_integer
 
 try:
     # rdist is an optional distance algorithm backend -- an import error is raised only
     # when one attempts to use rdist and the import was not successful
     import rdist
@@ -27,53 +29,183 @@
     """Abstract base class for distance matrix algorithms (dense or sparse).
 
     Important aspects and conventions for the distance algorithms:
 
     * The terms "pair-wise" (pdist) and "component-wise" (cdist) are
       adapted from the scipy's distance matrix computations
       :class:`scipy.sparse.spatial.pdist` and :class:`scipy.sparse.spatial.cdist`
-    * A sparse distance matrix with a distance cut-off value does not store distance
-      values *above* the cut-off. Importantly, this means that the sparse matrix
-      **must** store real distance zeros (duplicates or self-distances in case of
-      `pdist`) and treat the zeros not stored in the sparse matrix as "distance
-      values out of range".
+    * A sparse distance matrix with a distance (either `k`-neighbors or with a radius cut-off)
+      does not store all distance pairs. Importantly, this means that the sparse matrix
+      **must** store "real distance zeros" (introduced by duplicate points or self-distances
+      in case of `pdist`). This sometimes requires a workaround in matrix operations, so that
+      stored distance-zeros are not removed.
 
     Parameters
     ----------
     metric
         distance metric to compute
+
+    is_symmetric
+        indicate whether the distance matrix is symmetric (typically the standard
+        k-nearest-neighbor is not symmetric)
+
+    k
+        * for k-nearest-neighbors the number of neighbors
+        * for radius-based distance algorithms, there is a follow-up routine to make sure that
+          each sample has at least ``kmin`` neighbors (including distance pairs that are
+          larger than radius)
     """
 
-    # distances cannot be negative, therefore choose an easy to identify negative value
+    # distances cannot be negative - an easy to identify negative value
     _invalid_dist_value = -999
 
-    def __init__(self, metric):
-        try:
-            getattr(self, "backend_name")
-        except AttributeError:
-            raise NotImplementedError(
-                f"Attribute 'backend_name' is missing in subclass {type(self)}."
-            )
+    def __init__(
+        self,
+        metric: str,
+        is_symmetric: bool,
+        cut_off: Optional[float] = None,
+        k: Optional[float] = None,
+    ) -> None:
+        assert hasattr(
+            self, "name"
+        ), f"Attribute 'name' is missing in subclass {type(self)}."
+        self.name: str
 
         self.metric = metric
+        self.is_symmetric = is_symmetric
+
+        if cut_off is not None:
+            self._set_attrs_range(cut_off=cut_off, kmin=k)
+
+        if k is not None:
+            self._set_attrs_knn(k)
 
-    def _check_valid_metric(self, valid, metric):
+    def _set_attrs_range(self, cut_off, kmin):
+        if kmin is not None and not is_integer(kmin):
+            raise TypeError(
+                f"parameter 'kmin' must be an integer type or None. Got: {type(kmin)}"
+            )
+
+        check_scalar(
+            cut_off,
+            "cut_off",
+            target_type=(float, int),
+            min_val=0,
+            include_boundaries="neither",
+        )
+
+        if self.metric == "sqeuclidean":
+            if cut_off is not None:
+                # NOTE: this is a special case. Usually the cut_off is represented in the
+                # respective metric. However, for the 'sqeuclidean' case we use the
+                # 'euclidean' metric for the cut-off.
+                cut_off = cut_off**2
+
+        self.cut_off = cut_off
+        self.kmin = kmin
+
+    @property
+    def dist_type(self):
+        if hasattr(self, "cut_off"):
+            return "range-nn"
+        elif hasattr(self, "k"):
+            return "knn"
+        else:
+            return "full"
+
+    def _set_attrs_knn(self, k):
+        if k <= 0:
+            raise ValueError(f"parameter '{k=}' must be a positive integer")
+        self.k = k
+
+    def __repr__(self):
+        _name = self.__class__.__name__
+
+        if self.dist_type == "range-nn":
+            return (
+                _name + f"({self.metric=}, {self.is_symmetric=}, {self.is_sparse=}, "
+                f"{self.cut_off=}, {self.kmin=})".replace("self.", "")
+            )
+        elif self.dist_type == "knn":
+            return (
+                _name + f"({self.metric=}, {self.is_symmetric=}, {self.is_sparse=}, "
+                f"{self.k=})".replace("self.", "")
+            )
+        else:
+            return _name + f"({self.metric=}, {self.is_symmetric=})".replace(
+                "self.", ""
+            )
+
+    @property
+    def is_sparse(self):
+        if self.dist_type == "range-nn":
+            return self.cut_off is not None
+        elif self.dist_type == "knn":
+            return self.k < np.inf
+        else:
+            return False
+
+    def _validate_cut_off(self, cut_off):
+        if cut_off is None or np.isinf(cut_off):
+            cut_off = None  # default to None and use dense case if np.isinf(cut_off)
+        else:
+            try:
+                cut_off = float(cut_off)  # make sure to only deal with Python built-in
+            except ValueError:
+                raise TypeError(f"type(cut_off)={type(cut_off)} must be of type float")
+
+            if cut_off <= 0:
+                raise ValueError(
+                    f"cut_off={cut_off} must be a positive number number of "
+                    f"type 'float'"
+                )
+        if self.metric == "sqeuclidean":
+            if cut_off is not None:
+                # NOTE: this is a special case. Usually the cut_off is represented in the
+                # respective metric. However, for the 'sqeuclidean' case we use the
+                # 'euclidean' metric for the cut-off.
+                cut_off = cut_off**2
+
+        return cut_off
+
+    def _validate_X_Y(self, X, Y):
+        X = np.asarray(X)
+        X = if1dim_colvec(X)
+
+        if X.shape[0] <= 1:
+            raise ValueError("Number of samples has to be greater than 1.")
+
+        is_pdist = Y is None
+
+        if not is_pdist:
+            Y = np.asarray(Y)
+            Y = if1dim_rowvec(Y)
+
+            if X.shape[1] != Y.shape[1]:
+                raise ValueError(
+                    f"Mismatch in point dimension: "
+                    f"X.shape[1]={X.shape[1]} != Y.shape[1]={Y.shape[1]} "
+                )
+        return X, Y, is_pdist
+
+    def _validate_metric(self, valid, metric):
         if metric not in valid:
             raise ValueError(
                 f"Distance algorithm has invalid metric = {metric}. Valid metrics "
                 f"are = {valid}."
             )
 
-    def _numeric_cut_off(self, cut_off):
-        if cut_off is not None:
-            return cut_off
-        else:
-            return np.inf
+    def _sparse2dense_matrix(self, distance_matrix):
+        if scipy.sparse.issparse(distance_matrix) and self.cut_off is None:
+            # dense case stored in a sparse distance matrix -> convert to np.ndarray
+            distance_matrix = distance_matrix.toarray()
+
+        return distance_matrix
 
-    def _set_zeros_sparse_diagonal(self, distance_matrix):
+    def _set_zeros_diagonal_sparse(self, distance_matrix):
         # This function sets the diagonal to zero of a sparse matrix.
 
         # Some algorithms don't store the zeros on the diagonal for the pdist case.
         # However, this is critical if afterwards the kernel is applied
         # kernel(distance_matrix).
         #   -> kernel(distance)=0 but correct is kernel(distance)=1
         #      (for a stationary kernel)
@@ -111,836 +243,846 @@
         distance_matrix[distance_matrix == 0] = self._invalid_dist_value
         distance_matrix[distance_matrix >= cut_off] = 0
         distance_matrix = scipy.sparse.csr_matrix(distance_matrix)
         distance_matrix.data[distance_matrix.data == self._invalid_dist_value] = 0
 
         return distance_matrix
 
-    def __call__(
-        self,
+    @staticmethod  # static, so that it can be overwritten
+    def _ensure_kmin_nearest_neighbor(
         X: np.ndarray,
-        Y: Optional[np.ndarray] = None,
-        *,
-        cut_off: Optional[float] = None,
-        **backend_options,
-    ):
-        """Abstract method to compute the distance matrix.
+        Y: Optional[np.ndarray],
+        metric: str,
+        kmin: int,
+        distance_matrix: scipy.sparse.csr_matrix,
+    ) -> scipy.sparse.csr_matrix:
+        """Computes `kmin` nearest neighbors for all points that in the current distance
+        matrix have not at least `kmin` neighbors, yet.
 
-        Attributes
-        ----------
+        This function is especially useful to make sure that a neighborhood graph (
+        described by a distance matrix) is fully connected. If outlier have no
+        (or only self neighbor), then this can have unwanted side effects in some
+        applications.
 
+        Internally, the k-NN query is carried out using :class:`sklearn.neighbors.BallTree`.
+
+        Parameters
+        ----------
         X
-            Reference dataset.
+            Point cloud of shape `(n_samples_X, n_features_X)`.
 
         Y
-            Query dataset. If set then the computation is component-wise (cf. ``cdist``
-            function scipy) and if ``None``, the reference dataset is set to the query
-            (cf. ``pdist`` function in scipy)
-
-        cut_off
-            All distance pairs larger than this value are not stored in the resulting
-            sparse distance matrix (CSR format).
+            Query Point cloud of shape `(n_samples_Y, n_features_Y)`. If not given,
+            then `Y=X` (pdist case).
+
+        metric
+            distance metric
+
+        kmin
+            Minimum number of neighbors. Note, for the `pdist` case, `kmin==1` is already
+            fulfilled by the diagonal line (self-distances).
+
+        distance_matrix
+            Current distance matrix to which the missin distance pairs are inserted.
 
-        **backend_options
-            Additional kwargs for the method.
+        Returns
+        -------
+        scipy.sparse.csr_matrix
+            distance matrix with shape `(n_samples_Y, n_samples_X)`
         """
+        current_nnz = distance_matrix.getnnz(axis=1)
+        knn_query_indices = np.where(current_nnz < kmin)[0]
+        is_pdist = Y is None
+
+        if len(knn_query_indices) != 0:
+            if is_pdist:
+                Y = X.view()
+            else:
+                assert isinstance(Y, np.ndarray)
+                if (
+                    Y.shape[0] != distance_matrix.shape[0]
+                    or X.shape[0] != distance_matrix.shape[1]
+                ):
+                    raise ValueError("Mismatch between dataset and distance matrix.")
+
+            _ball_tree = BallTree(X, leaf_size=40, metric="euclidean")
+            distances, columns_indices = _ball_tree.query(
+                Y[knn_query_indices, :],
+                k=kmin,
+                return_distance=True,
+                dualtree=False,
+                breadth_first=False,
+                sort_results=False,
+            )
 
-        if Y is None:
-            return self.pdist(X, cut_off=cut_off, **backend_options)
-        else:
-            return self.cdist(X, Y, cut_off=cut_off, **backend_options)
+            distances = np.reshape(
+                distances, newshape=np.prod(distances.shape), order="C"
+            )
 
-    @abc.abstractmethod
-    def pdist(
-        self, X: np.ndarray, cut_off: Optional[float] = None, **backend_options
-    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
-        """Abstract method to compute the distance matrix pair-wise from the dataset.
+            # Note: duplicates and trivial self-distances in the pdist are assumed to already
+            # covered by the DistanceAlgorithm (always contained in the radius!)
+            nnz_distance_mask = (distances != 0).astype(bool)
+            distances = distances[nnz_distance_mask]
+
+            knn_query_indices = np.repeat(knn_query_indices, kmin)[nnz_distance_mask]
+
+            columns_indices = np.reshape(
+                columns_indices, newshape=np.prod(columns_indices.shape), order="C"
+            )[nnz_distance_mask]
+
+            if is_pdist:
+                knn_query_indices, columns_indices, distances = np.unique(
+                    np.vstack(
+                        [
+                            np.column_stack(
+                                [knn_query_indices, columns_indices, distances]
+                            ),
+                            np.column_stack(
+                                [columns_indices, knn_query_indices, distances]
+                            ),
+                        ]
+                    ),
+                    axis=0,
+                ).T
+
+            kmin_elements_csr = scipy.sparse.csr_matrix(
+                (distances, (knn_query_indices, columns_indices)),
+                shape=distance_matrix.shape,
+            )
 
-        In a pair-wise computation the query and reference data are the same. From this
-        the following distance matrix properties follow:
+            # TODO: This changes the sparsity structure and raises a warning. I am not sure
+            #  how to make this right. For this attempt the tests fail:
+            #  distance_matrix.tolil(copy=False)[
+            #      kmin_elements_csr.nonzero()
+            #  ] = kmin_elements_csr.data
+            #  maybe the best is to combine the elements of kmin_elements_csr and distance
+            #  matrix into one set (sorting out the upper triangle for pdist) and then
+            #  create a new sparse matrix...
+            distance_matrix[kmin_elements_csr.nonzero()] = kmin_elements_csr.data
+
+        return distance_matrix.tocsr()
+
+    def _handle_kmin(self, X, Y, distance_matrix):
+        """Use only for radius/range based algorithms."""
+        is_pdist = Y is None
 
-        * square
-        * diagonal contains distance to itself and are therefore zero
-        * symmetric
-        """
+        distance_matrix = self._validate_final_sparse_matrix(
+            distance_matrix=distance_matrix
+        )
+
+        # only for the sparse case we care about kmin:
+        apply_kmin_procedure = self.kmin is not None and (
+            (self.kmin > 0 and not is_pdist) or (self.kmin > 1 and is_pdist)
+        )
+
+        if apply_kmin_procedure:
+            # kmin == 1 and is_pdist does not need treatment because the diagonal is set.
+            distance_matrix = self._ensure_kmin_nearest_neighbor(
+                X,
+                Y,
+                metric=self.metric,
+                kmin=self.kmin,
+                distance_matrix=distance_matrix,
+            )
+
+        return distance_matrix
+
+    def _validate_final_sparse_matrix(self, distance_matrix):
+        # actually return a dense matrix
+        if scipy.sparse.issparse(distance_matrix) and np.isinf(self.cut_off):
+            # dense case stored in a sparse distance matrix -> convert to np.ndarray
+            distance_matrix = distance_matrix.toarray()
+        elif not isinstance(distance_matrix, scipy.sparse.csr_matrix):
+            # Currently, we only return a sparse matrix in CSR format.
+            distance_matrix = distance_matrix.tocsr()
+
+        if scipy.sparse.issparse(distance_matrix):
+            # sort_indices returns immediately if indices are already sorted.
+            # If not sorted, the call could be costly (depending on nnz), but is better for
+            # follow-up computations.
+            distance_matrix.sort_indices()
+
+        return distance_matrix
 
     @abc.abstractmethod
-    def cdist(
+    def __call__(
         self,
         X: np.ndarray,
-        Y: np.ndarray,
-        cut_off: Optional[float] = None,
-        **backend_options,
+        Y: Optional[np.ndarray] = None,
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
-        """Abstract method to compute the distance matrix component-wise.
+        """Compute distance matrix.
 
-        The dataset `X` refers to the reference dataset, and the distances are
-        computed component-wise for the query dataset `Y`. From this the general
-        matrix properties follow:
+        If only the reference dataset (`X`) is given, then the distances are pair-wise. From
+        this the following distance matrix properties follow:
+
+        * square
+        * diagonal contains distance to itself and are therefore zero
+        * symmetric
+
+        If an additional query dataset is given, then the distance matrix properties follow:
 
         * rectangular matrix of shape `(n_samples_Y, n_samples_X)`
-        * outlier points can lead to zero columns / rows
-        * only duplicated between `X` and `Y` have zero entries
+        * outlier points can lead to columns / rows of zero
+        * duplicated points between `X` and `Y` have zero entries on the diagonal
+
+
+        Attributes
+        ----------
+        X
+            Reference dataset of shape `(n_samples_X, n_features)`.
+
+        Y
+            Query dataset of shape `(n_samples_Y, n_features)`. If set then the computation
+            is component-wise and if ``None``, the reference dataset is taken as the query
+            points (i.e. `Y=X`).
         """
 
 
 class BruteForceDist(DistanceAlgorithm):
     """Computes all distance pairs in the distance matrix.
 
-    Chooses either
-
-        * `scipy.pdist <https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html>`_ \
-           and
-           `scipy.cdist <https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.cdist.html>`_
-        * `sklearn.pairwise_distances <https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise_distances.html>`_
+    Based on parameter `metric` and argument `exact_numeric` either backend is used:
 
-        Depending on the parameter `metric` and argument `exact_numeric`.
+        * SciPy with `scipy.pdist <https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html>`__ and
+          `scipy.cdist <https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.cdist.html>`__
+        * scikit-learn with `sklearn.pairwise_distances <https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise_distances.html>`__
 
-        For an explanation of how `exact_numeric = False` is beneficial, see the
-        `scikit-learn` `documentation <https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.euclidean_distances.html>`_
+    For an explanation of how `exact_numeric = False` is beneficial, see the
+    `scikit-learn documentation <https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.euclidean_distances.html>`__
 
     Parameters
     ----------
     metric
-        Metric to compute, see documentation of backend algorithms what metrics for
-        supported options.
-    """
-
-    backend_name = "brute"
-
-    def __init__(self, metric: str):
-        super(BruteForceDist, self).__init__(metric=metric)
-
-    def pdist(
-        self,
-        X: np.ndarray,
-        cut_off: Optional[float] = None,
-        exact_numeric: bool = True,
-        **backend_options,
-    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
-        """Pair-wise distance matrix computation.
-
-        Parameters
-        ----------
-        X
-            Point cloud of shape `(n_samples, n_features)`.
+        Metric to compute, see documentation of backend algorithms what metrics are supported.
 
-        cut_off
-            distances larger than `cut_off` are set to zero
+    exact_numeric
+        If False, computes Euclidean distances more efficiently
+        t the cost of introducing numerical noise. Empirically `~1e-14` for "sqeuclidean"
+        metric and `~1e-7` for "euclidean" metric.
 
-            .. note::
-                Distances with larger distance are removed after a full memory
-                allocation of the distance matrix. It is recommended to use
-                distance algorithms that directly integrate a cut-off sparsity.
-
-        exact_numeric
-            If False, computes Euclidean distances more efficiently
-            at the cost of introducing numerical noise. Empirically `~1e-14` for
-            "sqeuclidean" and `~1e-7` for "euclidean" metric.
-
-        **backend_options
-            Keyword arguments handled to the executing backend.
+    cut_off
+        distances larger than `cut_off` are set to zero
 
-        Returns
-        -------
-        Union[numpy.ndarray, scipy.sparse.csr_matrix]
-            distance matrix of shape `(n_samples, n_samples)`
-        """
-        if exact_numeric:
-            X = np.array(X)
-            _pdist = pdist(X, metric=self.metric)
-            distance_matrix = squareform(_pdist)
-        else:
-            # sklearn uses an numeric inexact but faster implementation
-            distance_matrix = pairwise_distances(
-                X, metric=self.metric, **backend_options
-            )
+        .. note::
 
-        if cut_off is not None:
-            distance_matrix = self._dense2csr_matrix(distance_matrix, cut_off=cut_off)
+            Distances with larger distance are removed after a full memory
+            allocation of the distance matrix. It is recommended to use
+            distance algorithms that directly reduce the number of computations.
+
+    **backend_options
+        Keyword arguments handled to the executing backend (depending on ``exact_numeric``
+        parameter).
+    """  # noqa: E501
 
-        return distance_matrix
+    name = "brute"
 
-    def cdist(
+    def __init__(
         self,
-        X: np.ndarray,
-        Y: np.ndarray,
-        cut_off: Optional[float] = None,
+        metric: str,
         exact_numeric: bool = True,
+        cut_off: Optional[Union[float, int]] = np.inf,
         **backend_options,
-    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
-        """Component-wise distance matrix computation.
+    ):
+        self.exact_numeric = exact_numeric
+        self.backend_options = backend_options
+        super().__init__(metric=metric, is_symmetric=True, cut_off=cut_off or np.inf)
+
+    @classmethod
+    def is_symmetric(cls):
+        return True
 
-        For undocumented parameters look at :meth:`.pdist`.
+    def __call__(
+        self,
+        X: np.ndarray,
+        Y: Optional[np.ndarray] = None,
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        """Compute distance matrix.
 
         Parameters
         ----------
         X
-            Point cloud of shape `(n_samples_X, n_features_X)`.
+            Reference dataset of shape `(n_samples_X, n_features)`.
 
         Y
-            Point cloud of shape `(n_samples_Y, n_features_Y)`.
+            Query dataset of shape `(n_samples_Y, n_features)`. If set then the computation
+            is component-wise and if ``None``, the reference dataset is taken as the query
+            points (i.e. `Y=X`).
 
         Returns
         -------
-        Union[numpy.ndarray, scipy.sparse.csr_matrix]
-            distance matrix of shape `(n_samples_Y, n_samples_X)`
+        np.ndarray, scipy.sparse.csr_matrix
+            distance matrix
         """
+        X, Y, is_pdist = self._validate_X_Y(X, Y)
 
-        if exact_numeric:
-            distance_matrix = cdist(Y, X, metric=self.metric, **backend_options)
+        if is_pdist:
+            if self.exact_numeric:
+                _pdist = pdist(X, metric=self.metric, **self.backend_options)
+                distance_matrix = squareform(_pdist)
+            else:
+                # sklearn uses a numeric inexact but faster implementation
+                distance_matrix = pairwise_distances(
+                    X, metric=self.metric, **self.backend_options
+                )
         else:
-            distance_matrix = pairwise_distances(
-                Y, X, metric=self.metric, **backend_options
+            if self.exact_numeric:
+                distance_matrix = cdist(
+                    Y, X, metric=self.metric, **self.backend_options
+                )
+            else:
+                distance_matrix = pairwise_distances(
+                    Y, X, metric=self.metric, **self.backend_options
+                )
+
+        if not np.isinf(self.cut_off):
+            distance_matrix = self._dense2csr_matrix(
+                distance_matrix, cut_off=self.cut_off
             )
 
-        if cut_off is not None:
-            # remove distances > cut_off and convert to sparse matrix
-            distance_matrix = self._dense2csr_matrix(distance_matrix, cut_off=cut_off)
+            distance_matrix = self._validate_final_sparse_matrix(distance_matrix)
 
         return distance_matrix
 
 
 class RDist(DistanceAlgorithm):
     """Sparse distance matrix algorithm rdist, for point clouds with manifold assumption.
 
     .. note::
-        The dependency on the Python package is optional. The package is currentl not
+        The dependency on the Python package is optional. The package is currently not
         published.
 
     Parameters
     ----------
-
     metric
         "euclidean" or "sqeuclidean"
 
+    cut_off
+        Distance values (always Euclidean metric) that are larger are not stored in
+        distance matrix.
+
     Raises
     ------
-
     ImportError
         if rdist is not installed, but selected as backend
 
     References
     ----------
-
     .. todo::
         include own paper if published
 
     """
 
-    backend_name = "rdist" if IS_IMPORTED_RDIST else None
+    name = "rdist" if IS_IMPORTED_RDIST else None  # type: ignore
 
-    def __init__(self, metric):
+    def __init__(self, cut_off, kmin=None, metric="euclidean", **backend_options):
         if not IS_IMPORTED_RDIST:
             raise ImportError("Could not import rdist. Check if it is installed.")
+        self.backend_options = backend_options
+        self._validate_metric(valid=["euclidean", "sqeuclidean"], metric=metric)
+        super().__init__(metric=metric, is_symmetric=True, cut_off=cut_off, k=kmin)
+
+    @classmethod
+    def is_symmetric(cls):
+        return True
 
-        self._check_valid_metric(valid=["euclidean", "sqeuclidean"], metric=metric)
-        super(RDist, self).__init__(metric=metric)
-
-    def _adapt_correct_metric_max_distance(self, max_distance):
+    def _adapt_radius(self):
         # Generally: the cut-off is represented like self.metric. The scipy.kdtree can
         # only compute Euclidean distances. Therefore, undo the squaring of cut-off.
         # For sqeuclidean distance, the squaring has to be done after the
         # distance matrix was computed.
 
         if self.metric == "sqeuclidean":
-            max_distance = np.sqrt(
-                max_distance
-            )  # note if max_distance==np.inf, the it is still np.inf
-
-        return max_distance
+            return np.sqrt(self.cut_off)
+        else:
+            return self.cut_off
 
     def _get_dist_options(self):
         return {"max_incr_radius": 0, "kmin": 0}
 
-    def pdist(
-        self, X: np.ndarray, cut_off: Optional[float] = None, **backend_options
-    ) -> scipy.sparse.csr_matrix:
-        """Pair-wise distance matrix computation.
-
-        Parameters
-        ----------
-        X
-            Point cloud of shape `(n_samples, n_features)`.
-
-        cut_off
-            Distance values (always Euclidean metric) that are larger are not stored in
-            distance matrix.
-
-        **backend_options
-            keywords handled to build
-
-        Returns
-        -------
-        scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples, n_samples)`
-        """
-
-        max_distance = self._numeric_cut_off(cut_off)
-        max_distance = self._adapt_correct_metric_max_distance(max_distance)
-
-        assert rdist is not None
-
-        # build tree, currently not stored, backend options are handled to here.
-        _rdist = rdist.Rdist(X, **backend_options)
-
-        # compute distance matrix, these options are not accessible from outside at the
-        # moment.
-        distance_matrix = _rdist.sparse_pdist(
-            r=max_distance, rtype="radius", **self._get_dist_options()
-        )
-
-        if self.metric == "euclidean":
-            distance_matrix.data = np.sqrt(distance_matrix.data)
-
-        return distance_matrix
-
-    def cdist(
+    def __call__(
         self,
         X: np.ndarray,
-        Y: np.ndarray,
-        cut_off: Optional[float] = None,
-        **backend_options,
+        Y: Optional[np.ndarray] = None,
     ) -> scipy.sparse.csr_matrix:
-        """Component-wise distance matrix computation.
-
-        For undocumented parameters look at :meth:`.pdist`.
+        """Compute distance matrix.
 
         Parameters
         ----------
         X
-            Point cloud of shape `(n_samples_X, n_features_X)`.
+            Reference dataset of shape `(n_samples_X, n_features)`.
 
         Y
-            Point cloud of shape `(n_samples_Y, n_features_Y)`.
+            Query dataset of shape `(n_samples_Y, n_features)`. If set then the computation
+            is component-wise and if ``None``, the reference dataset is taken as the query
+            points (i.e. `Y=X`).
 
         Returns
         -------
         scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples_Y, n_samples_X)`
+            distance matrix
         """
+        is_pdist = Y is None
 
-        assert rdist is not None
+        radius = self._adapt_radius()
 
-        max_distance = self._numeric_cut_off(cut_off)
-        max_distance = self._adapt_correct_metric_max_distance(max_distance)
+        if is_pdist or not hasattr(self, "rdist_"):
+            self.rdist_ = rdist.Rdist(X, **self.backend_options)
 
-        _rdist = rdist.Rdist(X, **backend_options)
-        distance_matrix = _rdist.sparse_cdist(
-            req_points=Y, r=max_distance, rtype="radius", **self._get_dist_options()
-        )
+        if is_pdist:
+            distance_matrix = self.rdist_.sparse_pdist(
+                r=radius, rtype="radius", **self._get_dist_options()
+            )
+        else:
+            distance_matrix = self.rdist_.sparse_cdist(
+                req_points=Y, r=radius, rtype="radius", **self._get_dist_options()
+            )
 
         if self.metric == "euclidean":
-            distance_matrix.data = np.sqrt(distance_matrix.data)
+            distance_matrix.data = np.sqrt(
+                distance_matrix.data, out=distance_matrix.data
+            )
 
-        return distance_matrix
+        return self._handle_kmin(X, Y, distance_matrix)
 
 
 class ScipyKdTreeDist(DistanceAlgorithm):
     """Sparse distance matrix computation using scipy's kd-tree implementation.
 
     Parameters
     ----------
-    metric
+    cut_off: float
+        Distance values (always Euclidean metric) that are larger are not stored in
+        distance matrix.
+
+    metric: str
         "euclidean" or "sqeuclidean"
 
+    kmin: int
+        store at least ``kmin`` samples per sample
+
+    backend_options
+        key word arguments passed to `cKDTree <https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.cKDTree.html>`__
+
     References
     ----------
-
     :class:`scipy.spatial.cKDTree`
     :meth:`scipy.spatial.KDTree.sparse_distance_matrix`
-
     """
 
-    backend_name = "scipy.kdtree"
+    name = "scipy.kdtree"
+
+    def __init__(self, cut_off, metric="euclidean", kmin=None, **backend_options):
+        self.backend_options = backend_options
+        self._validate_metric(valid=["euclidean", "sqeuclidean"], metric=metric)
+        super().__init__(
+            metric=metric, is_symmetric=True, cut_off=cut_off or np.inf, k=kmin
+        )
 
-    def __init__(self, metric):
-        self._check_valid_metric(valid=["euclidean", "sqeuclidean"], metric=metric)
-        super(ScipyKdTreeDist, self).__init__(metric=metric)
+    @classmethod
+    def is_symmetric(cls):
+        return True
 
-    def _adapt_correct_metric_max_distance(self, max_distance):
+    def _get_max_distance(self):
         # Generally: the cut-off is represented like self.metric. The scipy.kdtree can
         # only compute Euclidean distances. Therefore, undo the squaring of cut-off.
         # For sqeuclidean distance, the squaring has to be done after the
         # distance matrix was computed.
 
         if self.metric == "sqeuclidean":
-            # note if max_distance==np.inf, the it is still np.inf
-            max_distance = np.sqrt(max_distance)
-
-        return max_distance
-
-    def pdist(
-        self, X: np.ndarray, cut_off: Optional[float] = None, **backend_options
-    ) -> scipy.sparse.csr_matrix:
-        """Pair-wise distance computation.
-
-        Parameters
-        ----------
-        X
-            Point cloud of shape `(n_samples, n_features)`.
-
-        cut_off
-            Distance values (always Euclidean metric) that are larger are not stored in
-            distance matrix.
-
-        **backend_options
-            key word arguments handled to `cKDTree`
-
-        Returns
-        -------
-        scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples, n_samples)`
-        """
-
-        # TODO: if necessary there are build_options and compute_options required,
-        #  currently no options to sparse_distance_matrix are handed
-        max_distance = self._numeric_cut_off(cut_off)
-        max_distance = self._adapt_correct_metric_max_distance(max_distance)
-
-        kdtree = scipy.spatial.cKDTree(X, **backend_options)
-        dist_matrix = kdtree.sparse_distance_matrix(
-            kdtree, max_distance=max_distance, output_type="coo_matrix"
-        )
-
-        if self.metric == "sqeuclidean":
-            dist_matrix.data = np.square(dist_matrix.data)
-
-        return dist_matrix.tocsr()
+            # note if max_distance==np.inf, it is still np.inf
+            return np.sqrt(self.cut_off)
+        else:
+            return self.cut_off
 
-    def cdist(
+    def __call__(
         self,
         X: np.ndarray,
-        Y: np.ndarray,
-        cut_off: Optional[float] = None,
-        **backend_options,
+        Y: Optional[np.ndarray] = None,
     ) -> scipy.sparse.csr_matrix:
-        """Component-wise distance matrix computation.
+        """Compute distance matrix.
 
         Parameters
         ----------
         X
-            Point cloud of shape `(n_samples_X, n_features_X)`.
+            Reference dataset of shape `(n_samples_X, n_features)`.
 
         Y
-            Point cloud of shape `(n_samples_Y, n_features_Y)`.
+            Query dataset of shape `(n_samples_Y, n_features)`. If set then the computation
+            is component-wise and if ``None``, the reference dataset is taken as the query
+            points (i.e. `Y=X`).
 
         Returns
         -------
         scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples_Y, n_samples_X)`
+            distance matrix
         """
-        max_distance = self._numeric_cut_off(cut_off)
-        max_distance = self._adapt_correct_metric_max_distance(max_distance)
+        X, Y, is_pdist = self._validate_X_Y(X, Y)
 
-        kdtree_x = scipy.spatial.cKDTree(X, **backend_options)
-        kdtree_y = scipy.spatial.cKDTree(Y, **backend_options)
+        if is_pdist or not hasattr(self, "kdtree_x_"):
+            self.kdtree_x_ = scipy.spatial.cKDTree(X, **self.backend_options)
 
-        dist_matrix = kdtree_y.sparse_distance_matrix(
-            kdtree_x, max_distance=max_distance, output_type="coo_matrix"
-        )
+        if is_pdist:
+            distance_matrix = self.kdtree_x_.sparse_distance_matrix(
+                self.kdtree_x_,
+                max_distance=self._get_max_distance(),
+                output_type="coo_matrix",
+            )
+        else:
+            if not hasattr(self, "kdtree_x_"):
+                # else reuse from pdist call
+                self.kdtree_x_ = scipy.spatial.cKDTree(X, **self.backend_options)
+
+            kdtree_y = scipy.spatial.cKDTree(Y, **self.backend_options)
+
+            distance_matrix = kdtree_y.sparse_distance_matrix(
+                self.kdtree_x_,
+                max_distance=self._get_max_distance(),
+                output_type="coo_matrix",
+            )
 
         if self.metric == "sqeuclidean":
-            dist_matrix.data = np.square(dist_matrix.data)
+            distance_matrix.data = np.square(distance_matrix.data)
 
-        return dist_matrix.tocsr()
+        return self._handle_kmin(X, Y, distance_matrix=distance_matrix)
 
 
 class SklearnBalltreeDist(DistanceAlgorithm):
     """Distance matrix using ball tree implementation from scikit-learn.
 
     Parameters
     ----------
+    cut_off
+        Distance values (always Euclidean metric) that are larger are not stored in
+        distance matrix.
+
     metric
-        see `NeaestNeighors` documentation (reference)
+        see `metric parameter in `sklearn.NearestNeighbor <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html>`__
 
-    References
-    ----------
+    kmin
+        store at least ``kmin`` samples per sample
+
+    **backend_options
+        key word arguments passed to `sklearn.NearestNeighbors <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html>`__
 
+    See Also
+    --------
     :class:`sklearn.neighbors.NearestNeighbors`
     """
 
-    backend_name = "sklearn.balltree"
+    name = "sklearn.balltree"
 
-    def __init__(self, metric):
-        super(SklearnBalltreeDist, self).__init__(metric=metric)
+    def __init__(
+        self,
+        cut_off,
+        metric: str = "euclidean",
+        kmin: Optional[int] = None,
+        **backend_options,
+    ):
+        self.backend_options = backend_options
+        self._validate_metric(valid=["euclidean", "sqeuclidean"], metric=metric)
+        super().__init__(
+            metric=metric, is_symmetric=True, cut_off=cut_off or np.inf, k=kmin
+        )
 
-    def _map_metric_and_cut_off(self, cut_off):
+    @classmethod
+    def is_symmetric(cls):
+        return True
+
+    def _map_metric_and_radius(self):
         if self.metric == "sqeuclidean":
-            if cut_off is not None:
-                cut_off = np.sqrt(cut_off)
-            return "euclidean", cut_off
+            return "euclidean", np.sqrt(self.cut_off)
         else:
-            return self.metric, cut_off
+            return self.metric, self.cut_off
 
-    def pdist(
-        self, X: np.ndarray, cut_off: Optional[float] = None, **backend_options
-    ) -> scipy.sparse.csr_matrix:
-        """Pair-wise distance matrix computation.
-
-        Parameters
-        ----------
-        X
-            Point cloud of shape `(n_samples, n_features)`.
-
-        cut_off
-            Distance values (always Euclidean metric) that are larger are not stored in
-            distance matrix. (see also :class:`sklearn.neighbors.NearestNeighbors`
-            documentation)
-
-        **backend_options
-            handled to `NearestNeighbor`
-
-        Returns
-        -------
-        scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples, n_samples)`
-        """
-        metric, cut_off = self._map_metric_and_cut_off(cut_off)
-
-        max_distance = self._numeric_cut_off(cut_off)
+    def _fit_nearest_neighbor(self, X):
+        metric, radius = self._map_metric_and_radius()
         nn = NearestNeighbors(
-            radius=max_distance, algorithm="ball_tree", metric=metric, **backend_options
+            radius=radius, algorithm="ball_tree", metric=metric, **self.backend_options
         )
         nn.fit(X)
-        distance_matrix = nn.radius_neighbors_graph(mode="distance")
-
-        if self.metric == "sqeuclidean":
-            distance_matrix.data = np.square(
-                distance_matrix.data, out=distance_matrix.data
-            )
 
-        distance_matrix = self._set_zeros_sparse_diagonal(distance_matrix)
+        return nn
 
-        return distance_matrix
-
-    def cdist(
+    def __call__(
         self,
         X: np.ndarray,
-        Y: np.ndarray,
-        cut_off: Optional[float] = None,
-        **backend_options,
+        Y: Optional[np.ndarray] = None,
     ) -> scipy.sparse.csr_matrix:
-        """Component-wise distance matrix computation.
-
-        For undocumented parameters look at :meth:`.pdist`.
+        """Compute distance matrix.
 
         Parameters
         ----------
         X
-            Point cloud of shape `(n_samples_X, n_features_X)`.
+            Reference dataset of shape `(n_samples_X, n_features)`.
 
         Y
-            Point cloud of shape `(n_samples_Y, n_features_Y)`.
+            Query dataset of shape `(n_samples_Y, n_features)`. If set then the computation
+            is component-wise and if ``None``, the reference dataset is taken as the query
+            points (i.e. `Y=X`).
 
         Returns
         -------
         scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples_Y, n_samples_X)`
+            distance matrix
         """
-        metric, cut_off = self._map_metric_and_cut_off(cut_off)
+        X, Y, is_pdist = self._validate_X_Y(X, Y)
 
-        max_distance = self._numeric_cut_off(cut_off)
-        nn = NearestNeighbors(
-            radius=max_distance, algorithm="ball_tree", metric=metric, **backend_options
-        )
-        nn.fit(X)
-        distance_matrix = nn.radius_neighbors_graph(Y, mode="distance")
+        if is_pdist or not hasattr(self, "nn_"):
+            self.nn_ = self._fit_nearest_neighbor(X)
+
+        if is_pdist:
+            distance_matrix = self.nn_.radius_neighbors_graph(mode="distance")
+        else:
+            distance_matrix = self.nn_.radius_neighbors_graph(Y, mode="distance")
 
         if self.metric == "sqeuclidean":
             distance_matrix.data = np.square(
                 distance_matrix.data, out=distance_matrix.data
             )
 
-        return distance_matrix
+        if is_pdist:
+            distance_matrix = self._set_zeros_diagonal_sparse(distance_matrix)
 
+        return self._handle_kmin(X, Y, distance_matrix)
 
-class GuessOptimalDist(DistanceAlgorithm):
-    """Tries to guess a suitable algorithm based on sparsity, metric and installed
-    backends algorithms.
 
-    Parameters
-    ----------
-    metric
-        distance metric
+class SklearnKNN(DistanceAlgorithm):
+    name = "sklearn.knn"
 
-    """
+    def __init__(self, metric, k, **backend_options):
+        self.backend_options = backend_options
+        super().__init__(metric=metric, is_symmetric=False, k=k)
 
-    backend_name = "guess_optimal"
+    @classmethod
+    def is_symmetric(cls):
+        return False
 
-    def __init__(self, metric):
-        super(GuessOptimalDist, self).__init__(metric=metric)
+    def __call__(self, X, Y=None):
+        X, Y, is_pdist = self._validate_X_Y(X, Y=Y)
 
-    def _guess_optimal_backend(self, cut_off):
+        if is_pdist or not hasattr(self, "nn_"):
+            self.nn_ = KNeighborsTransformer(
+                mode="distance",
+                n_neighbors=self.k,
+                metric=self.metric,
+                **self.backend_options,
+            )
+            self.nn_.fit(X)
 
-        if cut_off is None:  # dense case
-            backend_str = BruteForceDist.backend_name
+        if is_pdist:
+            # here, the connection to self is not computed (but inserted below)
+            distance_matrix = self.nn_.kneighbors_graph(
+                n_neighbors=self.k - 1, mode="distance"
+            )
+            distance_matrix = self._set_zeros_diagonal_sparse(distance_matrix)
         else:
-            if IS_IMPORTED_RDIST and self.metric in ["euclidean", "sqeuclidean"]:
-                backend_str = RDist.backend_name
-                # backend_str = ScipyKdTreeDist.backend_name
-                assert backend_str is not None
-
-            elif self.metric in ["euclidean", "sqeuclidean"]:
-                backend_str = ScipyKdTreeDist.backend_name
-            else:
-                backend_str = BruteForceDist.backend_name
-
-        backend_class = get_backend_distance_algorithm(backend_str)
-        return backend_class(self.metric)  # initialize and return as object
-
-    def pdist(
-        self, X: np.ndarray, cut_off: Optional[float] = None, **backend_options
-    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
-        """Pair-wise distance matrix computation.
-
-        Parameters
-        ----------
-        X
-            Point cloud of shape `(n_samples, n_features)`.
-
-        cut_off
-            Distance values (always Euclidean metric) that are larger are not stored in
-            distance matrix.
-
-        **backend_options
-            Keyword arguments passed to :meth:`DistanceAlgorithm.pdist`
-
-        Returns
-        -------
-        scipy.sparse.csr_matrix
-            distance matrix of shape `(n_samples, n_samples)`
-        """
-        return self._guess_optimal_backend(cut_off).pdist(X, cut_off, **backend_options)
-
-    def cdist(
-        self,
-        X: np.ndarray,
-        Y: np.ndarray,
-        cut_off: Optional[float] = None,
-        **backend_options,
-    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
-        """Component-wise distance matrix computation.
-
-        For undocumented parameters look at :meth:`.pdist`.
-
-        Parameters
-        ----------
-        X
-            Point cloud of shape `(n_samples_X, n_features_X)`.
-
-        Y
-            Point cloud of shape `(n_samples_Y, n_features_Y)`.
-
-        Returns
-        -------
-        Union[numpy.ndarray, scipy.sparse.csr_matrix]
-            distance matrix of shape `(n_samples_Y, n_samples_X)`
-        """
-        return self._guess_optimal_backend(cut_off).cdist(
-            X, Y, cut_off, **backend_options
-        )
+            distance_matrix = self.nn_.kneighbors_graph(
+                Y, n_neighbors=self.k, mode="distance"
+            )
 
+        return distance_matrix
 
-def _ensure_kmin_nearest_neighbor(
-    X: np.ndarray,
-    Y: Optional[np.ndarray],
-    metric: str,
-    kmin: int,
-    distance_matrix: scipy.sparse.csr_matrix,
-) -> scipy.sparse.csr_matrix:
-    """Computes `kmin` nearest neighbors for all points that in the current distance
-    matrix have not at least `kmin` neighbors, yet.
-
-    This function is especially useful to make sure that a neighborhood graph (
-    described by a distance matrix) is fully connected. If outlier have no
-    (or only self neighbor), then this can have unwanted side effects in some
-    applications.
 
-    Internally, the k-NN query is carried out using :class:`sklearn.neighbors.BallTree`.
+class GuessOptimalDist(DistanceAlgorithm):
+    """Tries to guess a suitable algorithm based on sparsity, metric and installed
+    backends algorithms.
 
     Parameters
     ----------
-    X
-        Point cloud of shape `(n_samples_X, n_features_X)`.
-
-    Y
-        Query Point cloud of shape `(n_samples_Y, n_features_Y)`. If not given,
-        then `Y=X` (pdist case).
-
     metric
-        distance metric
+        distance metric to compute
 
-    kmin
-        Minimum number of neighbors. Note, for the `pdist` case, `kmin==1` is already
-        fulfilled by the diagonal line (self-distances).
+    is_symmetric
+        Whether it is required to compute a symmetric matrix (if True this excludes
+        sparse `k`-nearest-neighbor algorithms)
 
-    distance_matrix
-        Current distance matrix to which the missin distance pairs are inserted.
+    cut_off
+        If a valid float, then compute a sparse (symmetric) radius-based distance matrix.
+
+    k
+        Compute `k`-nearest-neighbor if non-symmetric sparse matrix or provide at least `k`
+        neighbors in a radius-based sparse matrix.
 
-    Returns
-    -------
-    scipy.sparse.csr_matrix
-        distance matrix with shape `(n_samples_Y, n_samples_X)`
     """
 
-    current_nnz = distance_matrix.getnnz(axis=1)
-    knn_query_indices = np.where(current_nnz < kmin)[0]
-    is_pdist = Y is None
+    name = "guess_optimal"
 
-    if len(knn_query_indices) != 0:
+    def __new__(cls, metric="euclidean", is_symmetric=True, cut_off=np.inf, kmin=None):
+        cut_off = cut_off or np.inf
+        cls.is_symmetric = lambda: is_symmetric
 
-        if is_pdist:
-            Y = X.view()
+        if np.isinf(cut_off):  # dense case
+            backend_class = BruteForceDist(cut_off=cut_off, metric=metric)
         else:
-            assert isinstance(Y, np.ndarray)
-            if (
-                Y.shape[0] != distance_matrix.shape[0]
-                or X.shape[0] != distance_matrix.shape[1]
-            ):
-                raise ValueError("Mismatch between dataset and distance matrix.")
-
-        _ball_tree = BallTree(X, leaf_size=40, metric="euclidean")
-        distances, columns_indices = _ball_tree.query(
-            Y[knn_query_indices, :],
-            k=kmin,
-            return_distance=True,
-            dualtree=False,
-            breadth_first=False,
-            sort_results=False,
-        )
-
-        distances = np.reshape(
-            distances, newshape=np.product(distances.shape), order="C"
-        )
-
-        # Note: duplicates and trivial self-distances in the pdist are assumed to already
-        # covered by the DistanceAlgorithm (always contained in the radius!)
-        nnz_distance_mask = (distances != 0).astype(bool)
-        distances = distances[nnz_distance_mask]
-
-        knn_query_indices = np.repeat(knn_query_indices, kmin)[nnz_distance_mask]
-
-        columns_indices = np.reshape(
-            columns_indices, newshape=np.product(columns_indices.shape), order="C"
-        )[nnz_distance_mask]
-
-        if is_pdist:
-
-            knn_query_indices, columns_indices, distances = np.unique(
-                np.vstack(
-                    [
-                        np.column_stack(
-                            [knn_query_indices, columns_indices, distances]
-                        ),
-                        np.column_stack(
-                            [columns_indices, knn_query_indices, distances]
-                        ),
-                    ]
-                ),
-                axis=0,
-            ).T
-
-        kmin_elements_csr = scipy.sparse.csr_matrix(
-            (distances, (knn_query_indices, columns_indices)),
-            shape=distance_matrix.shape,
-        )
+            if IS_IMPORTED_RDIST and metric in ["euclidean", "sqeuclidean"]:
+                backend_class = RDist(cut_off=cut_off, metric=metric, kmin=kmin)
+                assert backend_class is not None
+
+            elif metric in ["euclidean", "sqeuclidean"]:
+                backend_class = ScipyKdTreeDist(
+                    cut_off=cut_off, metric=metric, kmin=kmin
+                )
+            else:
+                backend_class = BruteForceDist(cut_off=cut_off, metric=metric)
 
-        # TODO: This changes the sparsity structure and raises a warning. I am not sure
-        #  how to make this right. For this attempt the tests fail:
-        #  distance_matrix.tolil(copy=False)[
-        #      kmin_elements_csr.nonzero()
-        #  ] = kmin_elements_csr.data
-        #  maybe the best is to combine the elements of kmin_elements_csr and distance
-        #  matrix into one set (sorting out the upper triangle for pdist) and then
-        #  create a new sparse matrix...
-        distance_matrix[kmin_elements_csr.nonzero()] = kmin_elements_csr.data
+        return backend_class
 
-    return distance_matrix.tocsr()
 
+def _all_available_distance_algorithm(require_symmetric: bool = False):
+    """Searches for valid subclasses of :py:class:`DistanceAlgorithm`.
 
-def _all_available_distance_algorithm():
-    """Searches for valid subclasses of :py:class:`DistanceAlgorithm`
+    Parameters
+    ----------
+    require_symmetric
+        Only return ``DistanceAlgorithm`` that compute a symmetric distance matrix.
 
     Returns
     -------
     list
         all valid subclasses
     """
-
-    all_backends: Sequence[type] = DistanceAlgorithm.__subclasses__()
+    all_backends = DistanceAlgorithm.__subclasses__()
 
     return_backends = list()
     # This is the case if backend is given as a str, now we look for the matching
-    # DistanceAlgorithm.backend_name
+    # DistanceAlgorithm.name
     for b in all_backends:
         # Tests are only for security that all algorithms have the mandatory (static)
         # attribute set.
 
         try:
             # Attribute error is raised here if 'backend_name' does not exist
             # If 'backend_name' is set to none, then the implementation is not
             # considered e.g. because dependencies are not met in case of rdist.
-            if isinstance(b.backend_name, str):
-                return_backends.append(b)
-        except AttributeError or AssertionError:
+            if isinstance(b.name, str):
+                if require_symmetric and b.is_symmetric():  # type: ignore
+                    return_backends.append(b)
+                elif not require_symmetric:
+                    return_backends.append(b)
+        except AttributeError:
             raise NotImplementedError(
-                f"Bug: class {type(b)} has no 'backend_name' attribute or it is not of "
+                f"Bug: class {type(b)} has no 'name' attribute or it is not of "
                 f"type 'str'. Check implementation."
             )
 
     return return_backends
 
 
-def get_backend_distance_algorithm(backend) -> Type[DistanceAlgorithm]:
+def get_backend_distance_algorithm(
+    backend, require_symmetric=False
+) -> type[DistanceAlgorithm]:
     """Selects and validates the backend class for distance matrix computation.
 
     Parameters
     ----------
     backend
         * ``str`` - maps to the algorithms
         * ``DistanceAlgorithm`` - returns same object if valid
 
+    require_symmetric
+        If True only return ``DistanceAlgorithm`` classes that compute a symmetric distance
+        matrix.
+
     Returns
     -------
     DistanceAlgorithm
     """
-
     if backend is None:
         raise ValueError("backend cannot be None")
 
-    all_backends = _all_available_distance_algorithm()
+    all_backends = _all_available_distance_algorithm(require_symmetric)
 
-    # This is the case if a user chooses backend by object instead of "backend_name"
+    # This is the case if a user chooses backend by object instead of "name"
     # attribute.
     if backend in all_backends:
         return backend
 
+    selected_backend = None
     for b in all_backends:
         # look up for the backend algorithm with the name implemented
-        if b.backend_name == backend:
-            return b
+        if b.name == backend:
+            selected_backend = b
+            break
     else:
         raise ValueError(f"Could not find backend {backend}")
 
+    return selected_backend
+
+
+def init_distance_algorithm(
+    backend="guess_optimal",
+    metric="euclidean",
+    cut_off=None,
+    k=None,
+    **backend_options,
+) -> DistanceAlgorithm:
+    """Initialize a distance matrix by name and keywords.
+
+    Parameters
+    ----------
+    backend: str
+        Backend to compute distance matrix.
+
+    metric
+        Distance metric. Needs to be supported by backend.
+
+    cut_off
+        Distances larger than `cut_off` are set to zero. The parameter controls the
+        degree of sparsity in the distance matrix.
+
+        .. note::
+            The pseudo-metric "sqeuclidean" is handled differently in a way that the
+            cut-off must be stated in in Eucledian distance (not squared cut-off).
+
+    k
+        Minimum number of neighbors per point. Ignored if `cut_off=np.inf` to indicate
+        a dense distance matrix, where all distance pairs are computed.
+
+    **backend_options
+        Keyword arguments handled to selected backend.
+
+    Returns
+    -------
+    Union[numpy.ndarray, scipy.sparse.csr_matrix]
+        distance matrix of shape `(n_samples_X, n_samples_X)` if `Y=None`, \
+        else of shape `(n_samples_Y, n_samples_X)`
+    """
+    backend_class = get_backend_distance_algorithm(backend)
+
+    backend_init_args = inspect.signature(backend_class).parameters.keys()
+
+    kwargs = {
+        "metric": metric,
+        "cut_off": cut_off,
+        "kmin": k,
+        "backend_options": backend_options,
+    }
+    keys = deepcopy(list(kwargs.keys()))
+
+    for a in keys:
+        if a not in backend_init_args:
+            kwargs.pop(a)
+
+    backend_options = kwargs.pop("backend_options", {})
+    return backend_class(**kwargs, **backend_options)
+
 
 def compute_distance_matrix(
     X: np.ndarray,
     Y: Optional[np.ndarray] = None,
     metric: str = "euclidean",
     cut_off: Optional[float] = None,
-    kmin: int = 0,
-    backend: Union[str, Type[DistanceAlgorithm]] = "brute",
+    k: Optional[int] = None,
+    backend: Union[str, type[DistanceAlgorithm]] = "guess_optimal",
     **backend_kwargs,
 ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
     """Compute distance matrix with different settings and backends.
 
     Parameters
     ----------
-
     X
         Point cloud of shape `(n_samples_X, n_features_X)`.
 
     Y
         Reference point cloud for component-wise computation of shape \
         `(n_samples_Y, n_features_Y)`. If not given, then `Y=X` (pairwise computation)
 
@@ -951,15 +1093,15 @@
         Distances larger than `cut_off` are set to zero. The parameter controls the
         degree of sparsity in the distance matrix.
 
         .. note::
             The pseudo-metric "sqeuclidean" is handled differently in a way that the
             cut-off must be stated in in Eucledian distance (not squared cut-off).
 
-    kmin
+    k
         Minimum number of neighbors per point. Ignored if `cut_off=np.inf` to indicate
         a dense distance matrix, where all distance pairs are computed.
 
     backend
         Backend to compute distance matrix.
 
     **backend_kwargs
@@ -967,125 +1109,15 @@
 
     Returns
     -------
     Union[numpy.ndarray, scipy.sparse.csr_matrix]
         distance matrix of shape `(n_samples_X, n_samples_X)` if `Y=None`, \
         else of shape `(n_samples_Y, n_samples_X)`
     """
-
-    if not isinstance(X, np.ndarray):
-        X = np.asarray(X)
-
-    X = if1dim_colvec(X)
-
-    is_pdist = Y is None
-
-    if cut_off is None or np.isinf(cut_off):
-        cut_off = None  # default to None and use dense case if np.isinf(cut_off)
-        is_sparse = False
-    else:
-        try:
-            cut_off = float(cut_off)  # make sure to only deal with Python built-in
-        except ValueError:
-            raise TypeError(f"type(cut_off)={type(cut_off)} must be of type float")
-        is_sparse = True
-
-    if not is_pdist and not isinstance(Y, np.ndarray):
-        Y = np.asarray(Y)
-
-    if not is_pdist:
-        assert Y is not None
-        Y = if1dim_rowvec(Y)
-
-        if X.shape[1] != Y.shape[1]:
-            raise ValueError(
-                f"Mismatch in point dimension: "
-                f"X.shape[1]={X.shape[1]} != Y.shape[1]={Y.shape[1]} "
-            )
-
-    if X.shape[0] <= 1:
-        raise ValueError(f"Number of samples has to be greater than 1.")
-
-    if is_sparse:
-        assert isinstance(cut_off, float)
-
-        if cut_off <= 0:
-            raise ValueError(
-                f"cut_off={cut_off} must be a positive number number of "
-                f"type 'float'"
-            )
-
-        kmin = int(kmin)  # use Python built-in
-        if not is_integer(kmin):
-            raise TypeError(f"kmin must be an integer type. Got: {type(kmin)}")
-
-        if kmin >= X.shape[0]:
-            raise ValueError(
-                "kmin must be smaller than the number of points available. "
-                f"Got {kmin} and X.shape[0]={X.shape[0]}"
-            )
-
-    if metric == "sqeuclidean":
-        if cut_off is not None:
-            # NOTE: this is a special case. Usually the cut_off is represented in the
-            # respective metric. However, for the 'sqeuclidean' case we use the
-            # 'euclidean' metric for the cut-off.
-            cut_off = cut_off ** 2
-
-    backend_class = get_backend_distance_algorithm(backend)
-    distance_method = backend_class(metric=metric)
-    distance_matrix = distance_method(X, Y, cut_off=cut_off, **backend_kwargs)
-
-    if scipy.sparse.issparse(distance_matrix) and cut_off is None:
-        # dense case stored in a sparse distance matrix -> convert to np.ndarray
-        distance_matrix = distance_matrix.toarray()
-
-    if is_sparse:
-
-        if not scipy.sparse.issparse(distance_matrix):
-            raise RuntimeError(
-                "Distance_matrix is expected to be sparse but DistanceAlgorithm "
-                f"{backend} returned dense matrix. Please report bug."
-            )
-
-        if not isinstance(distance_matrix, scipy.sparse.csr_matrix):
-            # Currently, we only return a sparse matrix in CSR format.
-            distance_matrix = distance_matrix.tocsr()
-
-        # only for the sparse case we care about kmin:
-        if (kmin > 0 and not is_pdist) or (kmin > 1 and is_pdist):
-            # kmin == 1 and is_pdist does not need treatment because the diagonal is set.
-            distance_matrix = _ensure_kmin_nearest_neighbor(
-                X,
-                Y,
-                metric=metric,
-                kmin=kmin,
-                distance_matrix=distance_matrix,
-            )
-
-        # sort_indices returns immediately if indices are already sorted.
-        # If not sorted, the call could be costly (depending on nnz), but is better for
-        # follow-up computations.
-        distance_matrix.sort_indices()
-
-        # n_elements_stored = (
-        #     distance_matrix.nnz
-        #     + len(distance_matrix.indptr)
-        #     + len(distance_matrix.indices)
-        # )
-
-        # There are also other reasons than memory savings for sparse matrices --
-        # therefore the warning is comment out for now.
-
-        # if n_elements_stored > np.product(distance_matrix.shape):
-        #     warnings.warn(
-        #         f"cut_off={cut_off} value does not lead to reduced memory requirements "
-        #         f"with sparse matrix. The sparse matrix stores {n_elements_stored} "
-        #         f"which exceeds a dense matrix by "
-        #         f"{n_elements_stored - np.product(distance_matrix.shape)} elements."
-        #     )
-
-    return distance_matrix
+    backend_class = init_distance_algorithm(
+        backend, metric, cut_off, k, **backend_kwargs
+    )
+    return backend_class(X, Y)
 
 
 if __name__ == "__main__":
     print(_all_available_distance_algorithm())
```

### Comparing `datafold-1.1.6/datafold/pcfold/eigsolver.py` & `datafold-2.0.0/datafold/pcfold/eigsolver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,318 @@
 import sys
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Union
 
 import numpy as np
 import scipy.sparse
 import scipy.sparse.linalg
 
-from datafold.utils.general import is_symmetric_matrix, sort_eigenpairs
+from datafold.utils.general import is_matrix, is_symmetric_matrix, sort_eigenpairs
+
+_valid_eigsolver_backends = ["scipy"]
+_valid_svd_backends = ["scipy"]
 
 
 class NumericalMathError(Exception):
     """Use for numerical problems/issues, such as singular matrices or too large
-    imaginary part."""
+    imaginary part.
+    """
 
     def __init__(self, message):
-        super(NumericalMathError, self).__init__(message)
+        super().__init__(message)
 
 
 def scipy_eigsolver(
-    kernel_matrix: Union[np.ndarray, scipy.sparse.csr_matrix],
-    n_eigenpairs: int,
-    is_symmetric: bool,
-    is_stochastic: bool,
+    kernel, kernel_matrix: Union[np.ndarray, scipy.sparse.csr_matrix], n_eigenpairs: int
 ):
     """Compute eigenpairs of kernel matrix with scipy backend.
 
     The scipy solver is selected based on the number of eigenpairs to compute. Note
     that also for dense matrix cases a sparse solver is selected. There are two reasons
-    for this decsision:
+    for this decision:
 
     1. General dense matrix eigensolver only allow *all* eigenpairs to be computed. This
        is computational more costly than handling a dense matrix to a sparse solver
        which can also solve for `k` eigenvectors.
     2. The hermitian (symmetric) `eigh` solver would also allow a partial computation of
        eigenpairs, but it showed to be slower in microbenchmark tests than the sparse
        solvers for dense matrices.
 
     Internal selection of backend:
 
     * If :code:`n_eigenpairs == n_samples` (for dense / sparse):
-      * symmetric `eigh <https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.eigh.html#scipy.linalg.eigh>`_
-      * non-symmetric `eig  <https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.eig.html#scipy.linalg.eig>`_
+
+      * symmetric `eigh <https://docs.scipy.org/doc/scipy/reference/generated/scipy.
+        linalg.eigh.html#scipy.linalg.eigh>`__
+      * non-symmetric `eig <https://docs.scipy.org/doc/scipy/reference/generated/scipy.
+        linalg.eig.html#scipy.linalg.eig>`__
 
     * If :code:`n_eigenpairs < n_samples` (for dense / sparse):
-      * symmetric `eigsh <https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.eigsh.html>`_
-      * non-symmetric `eigs <https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.eigs.html#scipy.sparse.linalg.eigs>`_
+
+      * symmetric `eigsh <https://docs.scipy.org/doc/scipy/reference/generated/scipy.
+        sparse.linalg.eigsh.html>`__
+      * non-symmetric `eigs <https://docs.scipy.org/doc/scipy/reference/generated/scipy.
+        sparse.linalg.eigs.html#scipy.sparse.linalg.eigs>`__
 
     Parameters
     ----------
-
     kernel_matrix
         Matrix of shape `(n_samples, n_samples)`.
 
     n_eigenpairs
         Number of eigenpairs to compute.
 
-    is_symmetric
-        True if matrix is symmetric. Note that there is no check and also numerical
-        noise that breaks the symmetry can lead to instabilities.
-
-     is_stochastic
-        If True, the kernel matrix is assumed to be row-stochastic. This enables
-        setting a `sigma` close to 1 to accelerate convergence.
-
     Returns
     -------
     numpy.ndarray
         eigenvalues of shape `(n_eigenpairs,)`
 
     numpy.ndarray
         eigenvectors of shape `(n_samples, n_eigenpairs)`
     """
-
     n_samples, n_features = kernel_matrix.shape
 
     # check only for n_eigenpairs == n_features and n_eigenpairs < n_features
     # wrong parametrized n_eigenpairs are catched in scipy functions
     if n_eigenpairs == n_features:
-        if is_symmetric:
+        if kernel._is_symmetric_kernel:
             scipy_eigvec_solver = scipy.linalg.eigh
         else:
             scipy_eigvec_solver = scipy.linalg.eig
 
-        solver_kwargs: Dict[str, object] = {
+        solver_kwargs: dict[str, object] = {
             "check_finite": False
-        }  # should be already checked
+        }  # should be checked already
 
     else:  # n_eigenpairs < matrix.shape[1]
-        if is_symmetric:
+        if kernel.is_symmetric:
             scipy_eigvec_solver = scipy.sparse.linalg.eigsh
         else:
             scipy_eigvec_solver = scipy.sparse.linalg.eigs
 
         solver_kwargs = {
             "k": n_eigenpairs,
             "which": "LM",
             "v0": np.ones(n_samples),
             "tol": 1e-14,
         }
 
         # The selection of sigma is a result of a microbenchmark
-        if is_symmetric and is_stochastic:
+        if kernel.is_symmetric and kernel.is_stochastic:
             # NOTE: it turned out that for self.kernel_.is_symmetric=False (-> eigs),
             # setting sigma=1 resulted into a slower computation.
             NUMERICAL_EXACT_BREAKER = 0.1
             solver_kwargs["sigma"] = 1.0 + NUMERICAL_EXACT_BREAKER
             solver_kwargs["mode"] = "normal"
         else:
+            # NOTE: it turned out that for self.kernel_.is_symmetric=False (-> eigs),
+            # setting sigma=1 resulted into a slower computation.
             solver_kwargs["sigma"] = None
 
         # the scipy solvers only work on floating points
         if scipy.sparse.issparse(
             kernel_matrix
         ) and kernel_matrix.data.dtype.kind not in ["fdFD"]:
             kernel_matrix = kernel_matrix.asfptype()
-        elif isinstance(kernel_matrix, np.ndarray) and kernel_matrix.dtype != "f":
+        elif isinstance(kernel_matrix, np.ndarray) and kernel_matrix.dtype.kind != "f":
             kernel_matrix = kernel_matrix.astype(float)
 
     eigvals, eigvects = scipy_eigvec_solver(kernel_matrix, **solver_kwargs)
 
     return eigvals, eigvects
 
 
-_valid_backends = ["scipy"]
+def scipy_svdsolver(
+    kernel_matrix, n_svdvtriplets, **kwargs
+) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """Decompose a (possibly rectangular) kernel matrix into singular value components.
+
+    Compute
+
+    .. math::
+
+        K = U S V^T
+
+    where, :math:`K` is the kernel matrix, :math:`U` and :math:`V` are the left and right
+    singular vectors and :math:`S` the diagonal singular matrix.
+
+    Parameters
+    ----------
+    kernel_matrix
+        Kernel matrix of shape `(n_samples_data, n_samples_reference)`, where
+        `n_samples_reference` can be the size of a reference/landmark set.
+
+    n_svdvtriplets
+        The number of SVD vectors and values to compute. Must be smaller than
+        `min(n_samples_data, n_samples_reference)`. If all triplets are computed, then a
+        sparse kernel may be cast to a dense matrix.
+
+    Returns
+    -------
+        svdvec_left
+            matrix :math:`U`
+        svdvals
+            array of singular values :math:`S`
+        svdvec_right
+            matrix :math:`V`
+    """
+    max_n_triplets = np.min(kernel_matrix.shape)
+
+    if n_svdvtriplets < max_n_triplets:
+        random_state = kwargs.pop("random_state", 3)
+        which = kwargs.pop("which", "LM")
+
+        svdvec_left, svdvals, svdvec_right = scipy.sparse.linalg.svds(
+            kernel_matrix,
+            k=n_svdvtriplets,
+            which=which,
+            random_state=random_state,
+            **kwargs,
+        )
+    else:  # n_svdvtriplets == max_n_triplets:
+        if scipy.sparse.isspmatrix(kernel_matrix):
+            # must be a dense matrix for the solver -- TODO: maybe raise warning?
+            kernel_matrix = kernel_matrix.toarray()
+        svdvec_left, svdvals, svdvec_right = scipy.linalg.svd(
+            kernel_matrix, full_matrices=False
+        )
+
+    return svdvec_left, svdvals, svdvec_right
 
 
 def compute_kernel_eigenpairs(
+    kernel,
     kernel_matrix: Union[np.ndarray, scipy.sparse.csr_matrix],
     n_eigenpairs: int,
-    is_symmetric: bool = False,
-    is_stochastic: bool = False,
     normalize_eigenvectors: bool = False,
     backend: str = "scipy",
-) -> Tuple[np.ndarray, np.ndarray]:
+    validate_matrix: bool = False,
+) -> tuple[np.ndarray, np.ndarray]:
     """Compute eigenvalues and -vectors from kernel matrix with consideration of matrix
     properties.
 
     Parameters
     ----------
     kernel_matrix
         Kernel matrix of shape `(n_samples, n_samples)`.
 
     n_eigenpairs
         Number of eigenpairs to compute.
 
-    is_symmetric
-        If True, this allows using specialized algorithms for symmetric matrices and
-        enables an additional numerical sanity check that all eigenvalues are real-valued.
-
-    is_stochastic
-        If True, this allows convergence to be improved because the trivial first
-        eigenvalue is known and all following eigenvalues are smaller.
-
     normalize_eigenvectors
-        If True, all eigenvectors are normalized to Eucledian norm 1.
+        If True, all eigenvectors are normalized to length 1.
 
     backend
         Valid backends:
             * "scipy"
 
+    validate_matrix
+        Validate matrix that it fulfills the specified properties (primarily used for
+        testing).
+
     Returns
     -------
     numpy.ndarray
         Eigenvalues in ascending order (absolute value).
 
     numpy.ndarray
         Eigenvectors (not necessarily normalized) in the same order to eigenvalues.
     """
-
-    if kernel_matrix.ndim != 2 or kernel_matrix.shape[0] != kernel_matrix.shape[1]:
-        raise ValueError(
-            f"kernel matrix must be a square. "
-            f"Got kernel_matrix.shape={kernel_matrix.shape}"
-        )
+    is_matrix(kernel_matrix, "kernel_matrix", square=True, allow_sparse=True)
 
     err_nonfinite = ValueError(
-        "kernel_matrix must only contain finite values (no np.nan " "or np.inf)"
+        "kernel_matrix must only contain finite values (no np.nan or np.inf)"
     )
     if (
-        isinstance(kernel_matrix, scipy.sparse.spmatrix)
+        scipy.sparse.issparse(kernel_matrix)
         and not np.isfinite(kernel_matrix.data).all()
     ):
         raise err_nonfinite
     elif isinstance(kernel_matrix, np.ndarray) and not np.isfinite(kernel_matrix).all():
         raise err_nonfinite
 
-    assert not is_symmetric or (is_symmetric and is_symmetric_matrix(kernel_matrix))
-
-    # BEGIN experimental code
-    # test_sparsify_experimental = False
-    # if test_sparsify_experimental:
-    #
-    #     SPARSIFY_CUTOFF = 1e-14
-    #
-    #     if scipy.sparse.issparse(kernel_matrix):
-    #         kernel_matrix.data[np.abs(kernel_matrix.data) < SPARSIFY_CUTOFF] = 0
-    #         kernel_matrix.eliminate_zeros()
-    #     else:
-    #         kernel_matrix[np.abs(kernel_matrix) < SPARSIFY_CUTOFF] = 0
-    #         kernel_matrix = scipy.sparse.csr_matrix(kernel_matrix)
-    # END experimental
+    if kernel_matrix.dtype == bool:
+        # cast bools to float64, otherwise the resulting vectors are in float32
+        kernel_matrix = kernel_matrix.astype(np.float64)
+
+    if validate_matrix:
+        if kernel.is_symmetric and not is_symmetric_matrix(kernel_matrix):
+            raise ValueError("kernel_matrix is not symmetric")
+
+        # TODO: include this after kernel refactor is carried out in #149
+        # if kernel_content.is_symmetric and not is_stochastic_matrix(kernel_matrix, axis=1):
+        #      raise ValueError("kernel_matrix is not stochastic")
 
     if backend == "scipy":
         eigvals, eigvects = scipy_eigsolver(
+            kernel=kernel,
             kernel_matrix=kernel_matrix,
             n_eigenpairs=n_eigenpairs,
-            is_symmetric=is_symmetric,
-            is_stochastic=is_stochastic,
         )
     else:
         raise ValueError(f"backend {backend} not known.")
 
     if not np.isfinite(eigvals).all() or not np.isfinite(eigvects).all():
         raise NumericalMathError(
             "eigenvalues or eigenvectors contain 'NaN' or 'inf' values."
         )
 
-    if is_symmetric:
+    if kernel._is_symmetric_kernel:
         if np.any(eigvals.imag > 1e2 * sys.float_info.epsilon):
             raise NumericalMathError(
                 "Eigenvalues have non-negligible imaginary part (larger than "
                 f"{1e2 * sys.float_info.epsilon})."
             )
 
         # algorithm can include numerical noise in imaginary part
         eigvals = np.real(eigvals)
         eigvects = np.real(eigvects)
 
     if normalize_eigenvectors:
         eigvects /= np.linalg.norm(eigvects, axis=0)[np.newaxis, :]
 
     return sort_eigenpairs(eigvals, eigvects)
+
+
+def compute_kernel_svd(
+    kernel_matrix: Union[np.ndarray, scipy.sparse.csr_matrix],
+    n_svdtriplet: int,
+    backend: str = "scipy",
+    **backend_kwargs,
+):
+    if n_svdtriplet > np.min(kernel_matrix.shape):
+        raise ValueError(
+            f"{n_svdtriplet} is larger than the maximum number of SVD triplets available "
+            f"(={np.min(kernel_matrix.shape)})"
+        )
+
+    if backend == "scipy":
+        svdvec_left, svdvals, svdvec_right = scipy_svdsolver(
+            kernel_matrix, n_svdvtriplets=n_svdtriplet, **backend_kwargs
+        )
+    else:
+        raise ValueError(
+            f"SVD backend {backend} is not available. "
+            f"Choose from {_valid_svd_backends}"
+        )
+
+    if np.iscomplexobj(svdvec_left) or np.iscomplexobj(svdvec_right):
+        # Note that the singular values are guaranteed to be real-valued
+
+        max_imag_entry = max(
+            np.abs(np.imag(svdvec_left)).max(), np.abs(np.imag(svdvec_right)).max()
+        )
+
+        if max_imag_entry > 1e2 * sys.float_info.epsilon:
+            raise NumericalMathError(
+                "SVD eigenvectors have non-negligible imaginary part (larger than "
+                f"{1e2 * sys.float_info.epsilon})."
+            )
+        else:
+            svdvec_left = np.real(svdvec_left)
+            svdvec_right = np.real(svdvec_right)
+
+    # Note: it is correct that left/right is opposite here
+    svdvals, svdvec_left, svdvec_right = sort_eigenpairs(
+        svdvals, right_eigenvectors=svdvec_left, left_eigenvectors=svdvec_right
+    )
+
+    return svdvec_left, svdvals, svdvec_right
```

### Comparing `datafold-1.1.6/datafold/pcfold/estimators.py` & `datafold-2.0.0/datafold/pcfold/estimators.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from datafold.pcfold.kernels import _kth_nearest_neighbor_dist
 
 
 def _warn_if_not_gaussian_kernel(kernel):
     if not isinstance(kernel, GaussianKernel):
         warnings.warn(
             "There is no guarantee that the method works with a kernel other than the "
-            "GaussianKernel"
+            "GaussianKernel",
+            stacklevel=2,
         )
 
 
 def estimate_cutoff(
     pcm,
     n_subsample: int = 1000,
     k: int = 10,
@@ -46,19 +47,17 @@
         sets :code:`np.random.default_rng(random_state)`
 
     distance_matrix
         pre-computed distance matrix instead of using the internal `cdist` method
 
     See Also
     --------
-
     :py:class:`datafold.pcfold.kernels.GaussianKernel`
 
     """
-
     from datafold.utils.general import is_integer
 
     if k <= 1 and not is_integer(k):
         raise ValueError("Parameter 'k' must be an integer greater than 1.")
     else:
         k = int(k)
 
@@ -75,15 +74,15 @@
         perm_indices_all = np.random.default_rng(random_state).permutation(n_points)
 
         distance_matrix = compute_distance_matrix(
             pcm[perm_indices_all[:n_subsample], :],
             pcm,
             metric="euclidean",
             backend="brute",
-            kmin=k,
+            k=k,
             # for estimation it is okay to be not exact and compute faster
             **dict(exact_numeric=False)
         )
 
         k = np.min([k, distance_matrix.shape[1]])
         # need to transpose the matrix here to correctly work with
         # _kth_nearest_neighbor_dist
@@ -112,17 +111,19 @@
 
     cut_off
         The `tol` parameter is ignored and the cut-off is used directly
 
     **estimate_cutoff_params
         Parameters to handle to method :py:meth:`estimate_cutoff` if ``cut_off is None``.
     """
-
-    _warn_if_not_gaussian_kernel(pcm.kernel)
+    try:
+        _warn_if_not_gaussian_kernel(pcm.kernel)
+    except AttributeError:
+        pass
 
     if cut_off is None:
         cut_off = estimate_cutoff(pcm, **estimate_cutoff_params)
 
     # this formula is derived by solving for epsilon in
     # tol >= exp(-cut_off**2 / epsilon)
-    eps0 = cut_off ** 2 / (-np.log(tol))
+    eps0 = cut_off**2 / (-np.log(tol))
     return float(eps0)
```

### Comparing `datafold-1.1.6/datafold/pcfold/kernels.py` & `datafold-2.0.0/datafold/pcfold/kernels.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import abc
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+import warnings
+from typing import Any, Callable, Optional, Union
 
 import numexpr as ne
 import numpy as np
 import pandas as pd
 import scipy.sparse
 import scipy.spatial
 from sklearn.gaussian_process.kernels import Kernel
 from sklearn.preprocessing import normalize
 from sklearn.utils import check_scalar
 
-from datafold.pcfold.distance import compute_distance_matrix
+from datafold.pcfold.distance import DistanceAlgorithm, init_distance_algorithm
 from datafold.pcfold.timeseries.accessor import TSCAccessor
 from datafold.utils.general import (
     df_type_and_indices_from,
     diagmat_dot_mat,
     is_df_same_index,
     is_float,
     is_integer,
@@ -36,36 +37,36 @@
     else:
         kernel = kernel_function(distance_matrix)
 
     return kernel
 
 
 def _apply_kernel_function_numexpr(distance_matrix, expr, expr_dict=None):
-
     expr_dict = expr_dict or {}
     assert "D" not in expr_dict.keys()
 
     if scipy.sparse.issparse(distance_matrix):
         # copy because the distance matrix may be used further by the user
         distance_matrix = distance_matrix.copy()
         expr_dict["D"] = distance_matrix.data
         ne.evaluate(expr, expr_dict, out=distance_matrix.data)
-        return distance_matrix  # returns actually the kernel
+        return distance_matrix  # returns actually the kernel matrix
     else:
         expr_dict["D"] = distance_matrix
         return ne.evaluate(expr, expr_dict)
 
 
 def _symmetric_matrix_division(
     matrix: Union[np.ndarray, scipy.sparse.spmatrix],
     vec: np.ndarray,
+    is_symmetric: bool,
     vec_right: Optional[np.ndarray] = None,
     scalar: float = 1.0,
     value_zero_division: Union[str, float] = "raise",
-) -> Union[np.ndarray, scipy.sparse.csr_matrix,]:
+) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
     r"""Symmetric division, often appearing in kernels.
 
     .. math::
         \frac{M_{i, j}}{a v^(l)_i v^(r)_j}
 
     where :math:`M` is a (kernel-) matrix and its elements are divided by the
     (left and right) vector elements :math:`v` and scalar :math:`a`.
@@ -94,48 +95,50 @@
     scalar
         Scalar ``a`` in the denominator.
 
     Returns
     -------
 
     """
-
     if matrix.ndim != 2:
         raise ValueError("Parameter 'matrix' must be a two dimensional array.")
 
     if matrix.shape[0] != matrix.shape[1] and vec_right is None:
         raise ValueError(
             "If 'matrix' is non-square, then 'vec_right' must be provided."
         )
 
     vec = vec.astype(float)
+    zero_idx_vec = vec == 0.0
 
-    if (vec == 0.0).any():
+    if zero_idx_vec.any():
         if value_zero_division == "raise":
             raise ZeroDivisionError(
-                f"Encountered zero values in division in {(vec == 0).sum()} points."
+                f"Encountered zero values in division in {zero_idx_vec.sum()} points."
             )
         else:
             # division results into 'nan' without raising a ZeroDivisionWarning. The
             # nan values will be replaced later
-            vec[vec == 0.0] = np.nan
+            vec[zero_idx_vec] = np.nan
 
     vec_inv_left = np.reciprocal(vec)
 
     if vec_right is None:
         vec_inv_right = vec_inv_left.view()
     else:
         vec_right = vec_right.astype(float)
-        if (vec_right == 0.0).any():
+        zero_idx_vec = vec_right == 0.0
+
+        if zero_idx_vec.any():
             if value_zero_division == "raise":
                 raise ZeroDivisionError(
-                    f"Encountered zero values in division in {(vec == 0).sum()}"
+                    f"Encountered zero values in division in {zero_idx_vec.sum()}"
                 )
             else:
-                vec_right[vec_right == 0.0] = np.inf
+                vec_right[zero_idx_vec] = np.nan
 
         vec_inv_right = np.reciprocal(vec_right.astype(float))
 
     if vec_inv_left.ndim != 1 or vec_inv_left.shape[0] != matrix.shape[0]:
         raise ValueError(
             f"Invalid input: 'vec.shape={vec.shape}' is not compatible with "
             f"'matrix.shape={matrix.shape}'."
@@ -144,28 +147,20 @@
     if vec_inv_right.ndim != 1 or vec_inv_right.shape[0] != matrix.shape[1]:
         raise ValueError(
             f"Invalid input: 'vec_right.shape={vec_inv_right.shape}' is not compatible "
             f"with 'matrix.shape={matrix.shape}'."
         )
 
     if scipy.sparse.issparse(matrix):
-        left_inv_diag_sparse = scipy.sparse.spdiags(
-            vec_inv_left, 0, m=matrix.shape[0], n=matrix.shape[0]
-        )
-        right_inv_diag_sparse = scipy.sparse.spdiags(
-            vec_inv_right, 0, m=matrix.shape[1], n=matrix.shape[1]
-        )
-
-        # The performance of DIA-sparse matrices is good if the matrix is actually
-        # sparse. I.e. the performance drops for a sparse-dense-sparse multiplication.
-
         # The zeros are removed in the matrix multiplication, but because 'matrix' is
         # usually a distance matrix we need to preserve the "true zeros"!
         matrix.data[matrix.data == 0] = np.inf
-        matrix = left_inv_diag_sparse @ matrix @ right_inv_diag_sparse
+
+        matrix = mat_dot_diagmat(matrix, vec_inv_right)
+        matrix = diagmat_dot_mat(vec_inv_left, matrix)
 
         matrix.data[np.isinf(matrix.data)] = 0
 
         # this imposes precedence order
         #    --> np.inf/np.nan -> np.nan
         # i.e. for cases with 0/0, set 'value_zero_division'
         if isinstance(value_zero_division, (int, float)):
@@ -177,27 +172,27 @@
         matrix = diagmat_dot_mat(vec_inv_left, matrix, out=matrix)
         matrix = mat_dot_diagmat(matrix, vec_inv_right, out=matrix)
 
         if isinstance(value_zero_division, (int, float)):
             matrix[np.isnan(matrix)] = value_zero_division
 
     # sparse and dense
-    if vec_right is None:
+    if is_symmetric and vec_right is None:
         matrix = remove_numeric_noise_symmetric_matrix(matrix)
 
     if scalar != 1.0:
         scalar = 1.0 / scalar
         matrix = np.multiply(matrix, scalar, out=matrix)
 
     return matrix
 
 
 def _conjugate_stochastic_kernel_matrix(
     kernel_matrix: Union[np.ndarray, scipy.sparse.spmatrix]
-) -> Tuple[Union[np.ndarray, scipy.sparse.spmatrix], scipy.sparse.dia_matrix]:
+) -> tuple[Union[np.ndarray, scipy.sparse.spmatrix], scipy.sparse.dia_matrix]:
     r"""Conjugate transformation to obtain symmetric (conjugate) kernel matrix with same
     spectrum properties.
 
     Rabin et al. :cite:`rabin_heterogeneous_2012` states in equation Eq. 3.1 \
     (notation adapted):
 
     .. math::
@@ -232,57 +227,57 @@
     Parameters
     ----------
     kernel_matrix
         non-symmetric kernel matrix
 
     Returns
     -------
-    Tuple[Union[np.ndarray, scipy.sparse.spmatrix], scipy.sparse.dia_matrix]
-        conjugate matrix (tpye as `kernel_matrix`) and (sparse) diagonal matrix to recover
+    Tuple[Union[np.ndarray, scipy.sparse.csr_matrix], scipy.sparse.dia_matrix]
+        conjugate matrix (type as `kernel_matrix`) and (sparse) diagonal matrix to recover
         eigenvectors
 
     References
     ----------
-    :cite:`rabin_heterogeneous_2012`
+    :cite:`rabin-2012`
 
     """
-
     left_vec = kernel_matrix.sum(axis=1)
 
     if scipy.sparse.issparse(kernel_matrix):
-        # to np.ndarray in case it is depricated format np.matrix
+        # to np.ndarray in case it is deprecated format np.matrix
         left_vec = left_vec.A1
 
     if left_vec.dtype.kind != "f":
         left_vec = left_vec.astype(float)
 
     left_vec = np.sqrt(left_vec, out=left_vec)
 
     kernel_matrix = _symmetric_matrix_division(
-        kernel_matrix, vec=left_vec, vec_right=None
+        kernel_matrix, vec=left_vec, is_symmetric=True, vec_right=None
     )
 
     # This is D^{-1/2} in sparse matrix form.
     basis_change_matrix = scipy.sparse.diags(np.reciprocal(left_vec, out=left_vec))
-
     return kernel_matrix, basis_change_matrix
 
 
 def _stochastic_kernel_matrix(kernel_matrix: Union[np.ndarray, scipy.sparse.spmatrix]):
-    """Normalizes matrix rows.
+    """Normalizes a matrix to a row-stochastic matrix.
 
-    This function performs
+    Mathematically,
 
     .. math::
+
         M = D^{-1} K
 
-    where matrix :math:`M` is the row-normalized kernel from :math:`K` by the
-    matrix :math:`D` with the row sums of :math:`K` on the diagonal.
+    where matrix :math:`M` is the row-normalized (kernel) matrix from :math:`K`. The matrix
+    :math:`D` has the row sums of :math:`K` on the diagonal.
 
     .. note::
+
         If the kernel matrix is evaluated component wise (points compared to reference
         points), then outliers can have a row sum close to zero. In this case the
         respective element on the diagonal is set to zero. For a pairwise kernel
         (pdist) this can not happen, as the diagonal element must be non-zero.
 
     Parameters
     ----------
@@ -295,15 +290,14 @@
         normalized kernel matrix with type same as `kernel_matrix`
     """
     if scipy.sparse.issparse(kernel_matrix):
         # in a microbenchmark this turned out to be the fastest solution for sparse
         # matrices
         kernel_matrix = normalize(kernel_matrix, copy=False, norm="l1")
     else:  # dense
-
         normalize_diagonal = np.sum(kernel_matrix, axis=1)
 
         with np.errstate(divide="ignore", over="ignore"):
             # especially in cdist computations there can be far away outliers
             # (or very small scale/epsilon). This results in elements near 0 and
             #  the reciprocal can then
             #     - be inf
@@ -332,32 +326,30 @@
     distance_matrix
         Distance matrix of shape `(n_samples_Y, n_samples_X)` from which to find the
         `k`-th nearest neighbor and its corresponding distance to return. If the matrix is
         sparse each point must have a minimum number of `k` neighbours (i.e. non-zero
         elements per row).
 
     k
-        The distance of the `k`-th nearest neighbor.
+        The distance to the `k`-th nearest neighbor.
 
     Returns
     -------
     numpy.ndarray
         distance values
     """
-
     if not is_integer(k):
-        raise ValueError(f"parameter 'k={k}' must be a positive integer")
+        raise ValueError(f"parameter {k=} must be a positive integer")
     else:
         # make sure we deal with Python built-in
         k = int(k)
 
-    if not (0 <= k <= distance_matrix.shape[1]):
+    if not (0 < k <= distance_matrix.shape[1]):
         raise ValueError(
-            "'k' must be an integer between 1 and "
-            f"distance_matrix.shape[1]={distance_matrix.shape[1]}"
+            f"{k=} must be an integer between 1 and {distance_matrix.shape[1]=}"
         )
 
     if isinstance(distance_matrix, np.ndarray):
         dist_knn = np.partition(distance_matrix, k - 1, axis=1)[:, k - 1]
     elif isinstance(distance_matrix, scipy.sparse.csr_matrix):
         # see mircobenchmark_kth_nn.py for a comparison of implementations for the
         # sparse case
@@ -394,195 +386,171 @@
     else:
         raise TypeError(f"type {type(distance_matrix)} not supported")
 
     return dist_knn
 
 
 class BaseManifoldKernel(Kernel):
+    def __init__(
+        self,
+        is_symmetric: bool = True,
+        is_stochastic: bool = False,
+        distance: Optional[Union[dict, DistanceAlgorithm]] = None,
+    ):
+        """Initialize new kernel.
+
+        Parameters
+        ----------
+        is_symmetric
+            Indicate whether the resulting kernel matrix is symmetric. A kernel may be
+            symmetric but computed with a `k` nearest-neighbor algorithm, ending in a
+            non-symmetric sparse matrix.
+
+        is_stochastic
+            Indicate whether the pairwise kernel matrix is stochastic. The typical case is
+            that the rows sum up to one (but columns-wise or double-stochastic matrix could
+            also be possible).
+        """
+        self._is_symmetric_kernel = is_symmetric
+        self.is_stochastic = is_stochastic
+
+        if distance is None or isinstance(distance, dict):
+            self.distance: DistanceAlgorithm = init_distance_algorithm(
+                **(distance or {})
+            )
+        else:
+            self.distance = distance
+
+    @property
+    def metric(self):
+        """Distance metric in the kernel."""
+        return self.distance.metric
+
+    @property
+    def is_symmetric(self):
+        """Indicates whether a pairwise kernel matrix is symmetric.
+
+        Note that a kernel matrix to be symmetric, also the distance matrix must be symmetric
+        (especially for k-nearest-neighbor this is often not the case).
+        """
+        return self.distance.is_symmetric and self._is_symmetric_kernel
+
     @abc.abstractmethod
-    def __call__(self, X, Y=None, *, dist_kwargs=None, **kernel_kwargs):
+    def __call__(
+        self, X, Y=None, **kernel_kwargs
+    ) -> Union[np.ndarray, scipy.sparse.spmatrix]:
         """Compute kernel matrix.
 
         If `Y=None`, then the pairwise-kernel is computed with `Y=X`. If `Y` is given,
         then the kernel matrix is computed component-wise with `X` being the reference
-        and `Y` the query point cloud.
-
-        Because the kernel can return a variable number of return values, this is
-        unified with :meth:`PCManifoldKernel.read_kernel_output`.
+        and `Y` the query points.
 
         Parameters
         ----------
-        args
+        Args:
+        ----
         kwargs
             See parameter documentation in subclasses.
 
         Returns
         -------
+        Union[np.ndarray, scipy.sparse.spmatrix]
+            Kernel matrix of shape `(n_samples_Y, n_samples_X)`. If cut-off is
+            specified in `dist_kwargs`, then the matrix is sparse.
+
         """
 
     def diag(self, X):
-        """(Not implemented, not used in datafold)
+        """(Not implemented, not used in datafold).
 
         Raises
         ------
         NotImplementedError
             this is only to overwrite abstract method in super class
         """
-
         raise NotImplementedError("base class")
 
     def is_stationary(self):
-        """(Not implemented, not used in datafold)
+        """(Not implemented, not used in datafold).
 
         Raises
         ------
         NotImplementedError
             this is only to overwrite abstract method in super class
         """
-
         # in datafold there is no handling of this attribute, if required this has to
         # be implemented
         raise NotImplementedError("base class")
 
-    def __repr__(self):
+    def __repr__(self, print_distance=True):
+        from copy import deepcopy
 
-        param_str = ", ".join(
-            [f"{name}={val}" for name, val in self.get_params().items()]
-        )
-        return f"{self.__class__.__name__}({param_str})"
+        _params = deepcopy(self.get_params())
+        _params.pop("distance", None)
 
-    def _read_kernel_kwargs(self, attrs: Optional[List[str]], kernel_kwargs: dict):
+        param_str = ", ".join([f"{name}={val}" for name, val in _params.items()])
 
-        return_values: List[Any] = []
+        if print_distance:
+            _distance = f"\n\t{self.distance=}".replace("self.", "")
+        else:
+            _distance = ""
+
+        return f"{self.__class__.__name__}({_distance}\n\t{param_str}\n)"
+
+    def _read_kernel_kwargs(self, attrs: Optional[list[str]], kernel_kwargs: dict):
+        return_values: list[Any] = []
 
         if attrs is not None:
             for attr in attrs:
                 return_values.append(kernel_kwargs.pop(attr, None))
 
         if kernel_kwargs != {}:
             raise KeyError(
-                f"kernel_kwargs.keys = {kernel_kwargs.keys()} are not " f"supported"
+                f"kernel_kwargs.keys = {kernel_kwargs.keys()} are not supported"
             )
 
         if len(return_values) == 0:
             return None
         elif len(return_values) == 1:
             return return_values[0]
         else:
             return return_values
 
-    @staticmethod
-    def read_kernel_output(
-        kernel_output: Union[Union[np.ndarray, scipy.sparse.csr_matrix], Tuple]
-    ) -> Tuple[Union[np.ndarray, scipy.sparse.csr_matrix], Dict, Dict]:
-        """Unifies kernel output for all possible return scenarios of a kernel.
-
-        This is required for models that allow generic kernels to be set where the
-        number of outputs of the internal kernel are not known *apriori*.
-
-        A kernel must return a computed kernel matrix in the first position. The two
-        other places are optional:
-
-        2. A dictionary containing keys that are required for a component-wise kernel
-           computation (and set in `**kernel_kwargs`, see also below). Examples are
-           computed density values.
-        3. A dictionary that containes additional information computed during the
-           computation. These extra information must always be at the third return
-           position.
-
-        .. code-block:: python
-
-            # we don't know how the exact kernel and therefore not how many return
-            # values are contained in kernel_output
-            kernel_output = compute_kernel_matrix(X)
-
-            # we read the output and obtain the three psossible places
-            kernel_matrix, cdist_kwargs, extra_info = \
-                PCManifold.read_kernel_output(kernel_output)
-
-            # we can compute a follow up component-wise kernel matrix
-            cdist_kernel_output = compute_kernel_matrix(X,Y, **cdist_kwargs)
-
-        Parameters
-        ----------
-        kernel_output
-            Output from an generic kernel, from which we don't know if it contains one,
-            two or three return values.
-
-        Returns
-        -------
-        Union[numpy.ndarray, scipy.sparse.csr_matrix]
-            Kernel matrix.
-
-        Dict
-            Data required for follow-up component-wise computation. The dictionary
-            should contain keys that can be included as `**kernel_kwargs` to the follow-up
-            ``__call__``. Dictionary is empty if no data is contained in kernel output.
-
-        Dict
-            Quantities of interest with keys specific of the respective kernel.
-            Dictionary is empty if no data is contained in kernel output.
-        """
-
-        if isinstance(
-            kernel_output, (pd.DataFrame, np.ndarray, scipy.sparse.csr_matrix)
-        ):
-            # easiest case, we simply return the kernel matrix
-            kernel_matrix, ret_cdist, ret_extra = [kernel_output, None, None]
-        elif isinstance(kernel_output, tuple):
-            if len(kernel_output) == 1:
-                kernel_matrix, ret_cdist, ret_extra = [kernel_output[0], None, None]
-            elif len(kernel_output) == 2:
-                kernel_matrix, ret_cdist, ret_extra = (
-                    kernel_output[0],
-                    kernel_output[1],
-                    None,
-                )
-            elif len(kernel_output) == 3:
-                kernel_matrix, ret_cdist, ret_extra = kernel_output
+    def _required_attrs(self, attrs: list, is_fit):
+        for a in attrs:
+            if is_fit:
+                if hasattr(self, a):
+                    raise AttributeError(
+                        f"Attribute {a} is already set from a previous "
+                        f"pairwise kernel evaluation. The attributes cannot "
+                        f"be reset, use a new kernel object."
+                    )
             else:
-                raise ValueError(
-                    "kernel_output must has more than three elements. "
-                    "Please report bug"
-                )
-        else:
-            raise TypeError(
-                "'kernel_output' must be either pandas.DataFrame (incl. TSCDataFrame), "
-                "numpy.ndarray or tuple. Please report bug."
-            )
-
-        ret_cdist = ret_cdist or {}
-        ret_extra = ret_extra or {}
-
-        if not isinstance(
-            kernel_matrix, (pd.DataFrame, np.ndarray, scipy.sparse.csr_matrix)
-        ):
-            raise TypeError(
-                f"Illegal type of kernel_matrix (type={type(kernel_matrix)}. "
-                f"Please report bug."
-            )
-
-        return kernel_matrix, ret_cdist, ret_extra
+                if not hasattr(self, a):
+                    raise AttributeError(
+                        f"Attribute {a} is missing in kernel. It is required to "
+                        f"first compute the pairwise kernel matrix "
+                        f"(i.e. :code:`kernel(X)`) to set the attributes."
+                    )
 
 
 class PCManifoldKernel(BaseManifoldKernel):
-    """Abstract base class for kernels acting on point clouds.
+    """Abstract base class for kernels evaluated on static point clouds or time series.
 
     See Also
     --------
     :py:class:`PCManifold`
+    :py:class:`TSCDataFrame`
     """
 
     @abc.abstractmethod
     def __call__(
         self,
         X: np.ndarray,
         Y: Optional[np.ndarray] = None,
-        *,
-        dist_kwargs: Optional[Dict[str, object]] = None,
         **kernel_kwargs,
     ):
         """Abstract method to compute the kernel matrix from a point cloud.
 
         Parameters
         ----------
         X
@@ -613,61 +581,59 @@
         Optional[Dict]
             If the kernel computes quantities of interest, then these quantities can be
             included in this dictionary. If this is returned, then this
             must be at the third return position (with a possible `None` return at the
             second position). If a kernel has no such values, this can be empty (i.e. not
             even `None` is returned).
         """
-
         raise NotImplementedError("base class")
 
     @abc.abstractmethod
-    def eval(
+    def evaluate(
         self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Evaluate kernel on pre-computed distance matrix.
 
         For return values see :meth:`.__call__`.
 
         .. note::
 
             In this function there are no checks of whether the distance matrix was
             computed with the correct metric required by the kernel.
 
         Parameters
         ----------
-
         distance_matrix
             Matrix of shape `(n_samples_Y, n_samples_X)`. For the sparse matrix case note
             that the kernel acts only on stored data, i.e. distance values with
             exactly zero (duplicates and self distance) must be stored explicitly in the
             matrix. Only large distance values exceeding a cut-off should not be stored.
 
         Returns
         -------
 
         """
         raise NotImplementedError("base class")
 
 
 class TSCManifoldKernel(BaseManifoldKernel):
-    """Abstract base class for kernels acting on time series collections.
+    """Abstract base class for kernels evaluating exclusively on time series.
 
     See Also
     --------
     :py:class:`.TSCDataFrame`
     """
 
     @abc.abstractmethod
     def __call__(
         self,
         X: pd.DataFrame,
         Y: Optional[pd.DataFrame] = None,
         *,
-        dist_kwargs: Optional[Dict[str, object]] = None,
+        dist_kwargs: Optional[dict[str, object]] = None,
         **kernel_kwargs,
     ):
         """Abstract method to compute the kernel matrix from a time series collection.
 
         Parameters
         ----------
         X
@@ -700,89 +666,101 @@
         Optional[Dict]
             If the kernel computes quantities of interest, then these quantities can be
             included in this dictionary. If this is returned, then this
             must be at the third return position (with a possible `None` return at the
             second position). If a kernel has no such values, this can be empty (i.e. not
             even `None` is returned).
         """
-
         raise NotImplementedError("base class")
 
 
 class RadialBasisKernel(PCManifoldKernel, metaclass=abc.ABCMeta):
     """Abstract base class for radial basis kernels.
 
     "A radial basis function (RBF) is a real-valued function whose value depends \
-    only on the distance between the input and some fixed point." from
-    `Wikipedia <https://en.wikipedia.org/wiki/Radial_basis_function>`_
+    only on the distance between the input and some fixed point." (taken from
+    `Wikipedia <https://en.wikipedia.org/wiki/Radial_basis_function>`__)
 
     Parameters
     ----------
-    distance_metric
+    required_metric
         metric required for kernel
     """
 
-    def __init__(self, distance_metric):
-        self.distance_metric = distance_metric
-        super(RadialBasisKernel, self).__init__()
+    def __init__(
+        self,
+        required_metric: str,
+        distance: Optional[Union[dict, DistanceAlgorithm]] = None,
+    ):
+        _metric_mismatch = ValueError(
+            "The metric is fixed for radial basis kernel and should not set in "
+            "dist_kwargs"
+        )
+
+        if distance is None:
+            distance = {"metric": required_metric}
+        elif isinstance(distance, DistanceAlgorithm):
+            if distance.metric != required_metric:
+                raise _metric_mismatch
+        elif isinstance(distance, dict):
+            _exist_metric = distance.pop("metric", None)
+
+            if _exist_metric is None or _exist_metric == required_metric:
+                distance["metric"] = required_metric
+            else:
+                raise _metric_mismatch
+
+        super().__init__(distance=distance)
 
     @classmethod
     def _check_bandwidth_parameter(cls, parameter, name) -> float:
         check_scalar(
             parameter,
             name=name,
             target_type=(float, np.floating, int, np.integer),
-            min_val=np.finfo(float).eps,
+            min_val=0,
+            include_boundaries="neither",
         )
         return float(parameter)
 
     def __call__(
-        self, X, Y=None, *, dist_kwargs=None, **kernel_kwargs
+        self, X, Y=None, **kernel_kwargs
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Compute kernel matrix.
 
         Parameters
         ----------
         X
             Reference point cloud of shape `(n_samples_X, n_features_X)`.
 
         Y
             Query point cloud of shape `(n_samples_Y, n_features_Y)`. If not given,
             then `Y=X`.
 
-        dist_kwargs,
-            Keyword arguments passed to the distance matrix computation. See
-            :py:meth:`datafold.pcfold.compute_distance_matrix` for parameter arguments.
-
         **kernel_kwargs
             None
 
         Returns
         -------
         Union[np.ndarray, scipy.sparse.csr_matrix]
             Kernel matrix of shape `(n_samples_Y, n_samples_X)`. If cut-off is
             specified in `dist_kwargs`, then the matrix is sparse.
         """
-
         self._read_kernel_kwargs(attrs=None, kernel_kwargs=kernel_kwargs)
 
         X = np.atleast_2d(X)
 
-        if Y is not None:
-            Y = np.atleast_2d(Y)
+        is_pdist = Y is None
 
-        distance_matrix = compute_distance_matrix(
-            X,
-            Y,
-            metric=self.distance_metric,
-            **dist_kwargs or {},
-        )
+        if not is_pdist:
+            Y = np.atleast_2d(Y)
 
-        kernel_matrix = self.eval(distance_matrix)
+        distance_matrix = self.distance(X, Y)
 
+        kernel_matrix = self.evaluate(distance_matrix)
         return kernel_matrix
 
 
 class GaussianKernel(RadialBasisKernel):
     r"""Gaussian radial basis kernel.
 
     .. math::
@@ -792,48 +770,48 @@
 
     See also super classes :class:`RadialBasisKernel` and :class:`PCManifoldKernel`
     for more functionality and documentation.
 
     Parameters
     ----------
     epsilon
-        The kernel scale as a positive float value. Alternatively, a a
-        callable can be passed. After computing the distance matrix, the distance matrix
-        will be passed to this function i.e. ``function(distance_matrix)``. The result
-        of this function must be a again a positive float to describe the kernel scale.
+        The kernel scale as a positive float value. Alternatively, a
+        callable can be passed to which the distance matrix is
+        (i.e. ``function(distance_matrix)``). The return value of this function must be a
+        positive float that is used as the epsilon.
     """
 
-    def __init__(self, epsilon: Union[float, Callable] = 1.0):
+    def __init__(self, epsilon: Union[float, Callable] = 1.0, distance=None):
         self.epsilon = epsilon
-        super(GaussianKernel, self).__init__(distance_metric="sqeuclidean")
+        super().__init__(required_metric="sqeuclidean", distance=distance)
 
-    def eval(
+    def evaluate(
         self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Evaluate the kernel on pre-computed distance matrix.
 
         Parameters
         ----------
         distance_matrix
             Matrix of pairwise distances of shape `(n_samples_Y, n_samples_X)`.
 
         Returns
         -------
         Union[np.ndarray, scipy.sparse.csr_matrix]
             Kernel matrix of same shape and type as `distance_matrix`.
         """
-
         # Security copy, the distance matrix is maybe required again (for gradient,
         # or other computations...)
 
         if callable(self.epsilon):
             if isinstance(distance_matrix, scipy.sparse.csr_matrix):
                 self.epsilon = self.epsilon(distance_matrix.data)
             elif isinstance(distance_matrix, np.ndarray):
                 self.epsilon = self.epsilon(distance_matrix)
+                print(self.epsilon)
             else:
                 raise TypeError(
                     f"Invalid type: type(distance_matrix)={type(distance_matrix)}."
                     f"Please report bug."
                 )
 
         self.epsilon = self._check_bandwidth_parameter(
@@ -859,37 +837,36 @@
 
     See also super classes :class:`RadialBasisKernel` and :class:`PCManifoldKernel`
     for more functionality and documentation.
 
     Parameters
     ----------
     epsilon
-        kernel scale
+        Positive float to scale the kernel weights.
     """
 
-    def __init__(self, epsilon: float = 1.0):
+    def __init__(self, epsilon: float = 1.0, distance: Optional[dict] = None):
         self.epsilon = epsilon
-        super(MultiquadricKernel, self).__init__(distance_metric="sqeuclidean")
+        super().__init__(required_metric="sqeuclidean", distance=distance)
 
-    def eval(
+    def evaluate(
         self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Evaluate the kernel on pre-computed distance matrix.
 
         Parameters
         ----------
         distance_matrix
             Matrix of pairwise distances of shape `(n_samples_Y, n_samples_X)`.
 
         Returns
         -------
         Union[np.ndarray, scipy.sparse.csr_matrix]
             Kernel matrix of same shape and type as `distance_matrix`.
         """
-
         self.epsilon = self._check_bandwidth_parameter(
             parameter=self.epsilon, name="epsilon"
         )
 
         return _apply_kernel_function_numexpr(
             distance_matrix,
             expr="sqrt(1.0 / (2*eps) * D + 1.0)",
@@ -907,64 +884,127 @@
 
     See also super classes :class:`RadialBasisKernel` and :class:`PCManifoldKernel`
     for more functionality and documentation.
 
     Parameters
     ----------
     epsilon
-        kernel scale
+        Positive float to scale the kernel weights.
     """
 
-    def __init__(self, epsilon: float = 1.0):
+    def __init__(self, epsilon: float = 1.0, distance=None):
         self.epsilon = epsilon
-        super(InverseMultiquadricKernel, self).__init__(distance_metric="sqeuclidean")
+        super().__init__(required_metric="sqeuclidean", distance=distance)
 
-    def eval(
+    def evaluate(
         self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Evaluate the kernel on pre-computed distance matrix.
 
         Parameters
         ----------
         distance_matrix
             Matrix of pairwise distances of shape `(n_samples_Y, n_samples_X)`.
 
         Returns
         -------
         Union[np.ndarray, scipy.sparse.csr_matrix]
             Kernel matrix of same shape and type as `distance_matrix`.
         """
-
         self.epsilon = self._check_bandwidth_parameter(
             parameter=self.epsilon, name="epsilon"
         )
 
         return _apply_kernel_function_numexpr(
             distance_matrix,
             expr="1.0 / sqrt(1.0 / (2*eps) * D + 1.0)",
             expr_dict={"eps": self.epsilon},
         )
 
 
+class InverseQuadraticKernel(RadialBasisKernel):
+    r"""Inverse quadratic radial basis kernel.
+
+    .. math::
+        K = (\frac{1}{2\varepsilon} \cdot D + 1)^{-1}
+
+    where :math:`D` is the squared Euclidean distance matrix.
+
+    See also super classes :class:`RadialBasisKernel` and :class:`PCManifoldKernel`
+    for more functionality and documentation.
+
+    Parameters
+    ----------
+    epsilon
+        kernel scale
+    """
+
+    def __init__(self, epsilon: float = 1.0):
+        self.epsilon = epsilon
+        super().__init__(required_metric="sqeuclidean")
+
+    def evaluate(
+        self,
+        distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix],
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        """Evaluate the kernel on pre-computed distance matrix.
+
+        Parameters
+        ----------
+        distance_matrix
+            Matrix of pairwise distances of shape `(n_samples_Y, n_samples_X)`.
+
+        Returns
+        -------
+        Union[np.ndarray, scipy.sparse.csr_matrix]
+            Kernel matrix of same shape and type as `distance_matrix`.
+        """
+        self.epsilon = self._check_bandwidth_parameter(
+            parameter=self.epsilon, name="epsilon"
+        )
+
+        return _apply_kernel_function_numexpr(
+            distance_matrix,
+            expr="1.0 / (1.0 / (2*eps) * D + 1.0)",
+            expr_dict={"eps": self.epsilon},
+        )
+
+
+class ThinplateKernel(RadialBasisKernel):
+    r"""Thinplate radial basis kernel."""
+
+    def __init__(self, distance=None):
+        super().__init__(required_metric="euclidean", distance=distance)
+
+    def evaluate(
+        self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        kernel_matrix = _apply_kernel_function_numexpr(
+            distance_matrix, expr="D**2 * log(D)"
+        )
+        kernel_matrix[np.isnan(kernel_matrix)] = 0
+        return kernel_matrix
+
+
 class CubicKernel(RadialBasisKernel):
     r"""Cubic radial basis kernel.
 
     .. math::
         K= D^{3}
 
     where :math:`D` is the Euclidean distance matrix.
 
     See also super classes :class:`RadialBasisKernel` and :class:`PCManifoldKernel`
     for more functionality and documentation.
     """
 
-    def __init__(self):
-        super(CubicKernel, self).__init__(distance_metric="euclidean")
+    def __init__(self, distance=None):
+        super().__init__(required_metric="euclidean", distance=distance)
 
-    def eval(
+    def evaluate(
         self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Evaluate the kernel on pre-computed distance matrix.
 
         Parameters
         ----------
         distance_matrix
@@ -987,18 +1027,18 @@
 
     where :math:`D` is the Euclidean distance matrix.
 
     See also super classes :class:`RadialBasisKernel` and :class:`PCManifoldKernel`
     for more functionality and documentation.
     """
 
-    def __init__(self):
-        super(QuinticKernel, self).__init__(distance_metric="euclidean")
+    def __init__(self, distance=None):
+        super().__init__(required_metric="euclidean", distance=distance)
 
-    def eval(
+    def evaluate(
         self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]
     ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
         """Evaluate the kernel on pre-computed distance matrix.
 
         Parameters
         ----------
         distance_matrix
@@ -1012,77 +1052,131 @@
         # r**5
         return _apply_kernel_function_numexpr(distance_matrix, "D ** 5")
 
 
 class ContinuousNNKernel(PCManifoldKernel):
     """Compute the continuous `k` nearest-neighbor adjacency graph.
 
-    The continuous `k` nearest neighbor (C-kNN) graph is an adjacency (i.e. unweighted)
-    graph for which the (un-normalized) graph Laplacian converges spectrally to a
-    Laplace-Beltrami operator on the manifold in the large data limit.
+    The continuous `k` nearest neighbor (C-kNN) graph is an adjacency graph (i.e. weights are
+    only one or zero). This (un-normalized) graph Laplacian converges spectrally to the
+    Laplace-Beltrami operator on the manifold in the large data limit (see reference).
 
     Parameters
     ----------
     k_neighbor
-        For each point the distance to the `k_neighbor` nearest neighbor is computed.
+        For each point the distance to the ``k_neighbor`` nearest neighbor is computed.
         If a sparse matrix is computed (with cut-off distance), then each point must
-        have a minimum of `k` stored neighbors. (see `kmin` parameter in
+        have a minimum of `k` neighbors. (see `kmin` parameter in
         :meth:`pcfold.distance.compute_distance_matrix`).
 
     delta
         Unit-less scale parameter.
 
-    References
+    Attributes
     ----------
+    reference_dist_knn_
+        The `k`-th nearest neighbors stored for the reference dataset in a pairwise
+        computation. The data is required for component-wise evaluation.
 
-    :cite:`berry_consistent_2019`
+    References
+    ----------
+    :cite:t:`berry-2019`
     """
 
-    def __init__(self, k_neighbor: int, delta: float):
-
-        if not is_integer(k_neighbor):
-            raise TypeError("n_neighbors must be an integer")
-        else:
-            # make sure to only use Python built-in
-            self.k_neighbor = int(k_neighbor)
-
+    def __init__(self, k_neighbor: int, delta: float, distance=None):
         if not is_float(delta):
             if is_integer(delta):
                 self.delta = float(delta)
             else:
                 raise TypeError("delta must be of type float")
         else:
             # make sure to only use Python built-in
             self.delta = float(delta)
 
-        if self.k_neighbor < 1:
-            raise ValueError(
-                f"parameter 'k_neighbor={self.k_neighbor}' must be a positive integer"
-            )
-
         if self.delta <= 0.0:
-            raise ValueError(
-                f"parrameter 'delta={self.delta}' must be a positive float"
-            )
+            raise ValueError(f"parameter '{self.delta=}' must be a positive float")
 
-        super(ContinuousNNKernel, self).__init__()
+        if k_neighbor < 1:
+            raise ValueError(f"parameter '{k_neighbor=}' must be a positive integer")
+
+        if not is_integer(k_neighbor):
+            raise TypeError(f"k_neighbor must be an integer (got {type(k_neighbor)=})")
+        else:
+            # make sure to only use Python built-in
+            self.k_neighbor = int(k_neighbor)
+
+        if distance is None or isinstance(distance, dict):
+            distance = distance or {}
+            distance.setdefault("kmin", self.k_neighbor)
+            distance.setdefault("metric", "euclidean")
+            distance = init_distance_algorithm(backend="guess_optimal", **distance)
+        elif isinstance(distance, DistanceAlgorithm) and distance.dist_type == "knn":
+            if distance.k < self.k_neighbor:
+                raise ValueError(
+                    f"{self.distance=} must have at least {self.k_neighbor=} neighbors"
+                )
+        elif (
+            isinstance(distance, DistanceAlgorithm) and distance.dist_type == "range-nn"
+        ):
+            if distance.kmin < self.k_neighbor:
+                raise ValueError(
+                    f"{self.distance=} must assure that each point has at least "
+                    f"{self.k_neighbor=} neighbors (set kmin)"
+                )
+        else:
+            raise TypeError(f"{type(self.distance)=} not understood")
+        self.distance = distance
+        self.reference_dist_knn_: np.ndarray
+        super().__init__(distance=distance)
 
     def _validate_reference_dist_knn(self, is_pdist, reference_dist_knn):
         if is_pdist and reference_dist_knn is None:
             raise ValueError("For the 'cdist' case 'reference_dist_knn' must be given")
 
+    def _validate(self, distance_matrix, is_pdist):
+        if distance_matrix.ndim != 2:
+            raise ValueError("distance_matrix must be a two-dimensional array")
+
+        n_samples_Y, n_samples_X = distance_matrix.shape
+
+        if is_pdist:
+            if n_samples_Y != n_samples_X:
+                raise ValueError(
+                    f"If {is_pdist=}, the distance matrix must be square and symmetric."
+                )
+
+            if isinstance(distance_matrix, np.ndarray):
+                diagonal = np.diag(distance_matrix)
+            else:
+                diagonal = np.asarray(distance_matrix.diagonal(0))
+
+            if (diagonal != 0).all():
+                raise ValueError(
+                    f"If {is_pdist=}, distance_matrix must have zeros on diagonal."
+                )
+        else:
+            if self.k_neighbor < 1 or self.k_neighbor > n_samples_X - 1:
+                raise ValueError(
+                    f"{self.k_neighbor=}' must be in a range between 1 to the number of "
+                    f"samples ({distance_matrix.shape[1]=})"
+                )
+
+            if self.reference_dist_knn_.shape[0] != n_samples_X:
+                raise ValueError(
+                    f"{self.reference_dist_knn_.shape[0]} "
+                    f"must have {distance_matrix.shape[1]=} samples"
+                )
+
     def __call__(
         self,
         X: np.ndarray,
         Y: Optional[np.ndarray] = None,
-        *,
-        dist_kwargs: Optional[Dict] = None,
         **kernel_kwargs,
     ):
-        """Compute (sparse) adjacency graph to describes a point neighborhood.
+        """Compute (sparse) adjacency graph to describe point neighborhood.
 
         Parameters
         ----------
         X
             Reference point cloud of shape `(n_samples_X, n_features_X)`.
 
         Y
@@ -1090,249 +1184,379 @@
             then `Y=X`.
 
         dist_kwargs
             Keyword arguments passed to the internal distance matrix computation. See
             :py:meth:`datafold.pcfold.compute_distance_matrix` for parameter arguments.
 
         **kernel_kwargs: Dict[str, object]
-            - reference_dist_knn: Optional[np.ndarray]
-                Distances to the `k`-th nearest neighbor for each point in `X`. The
-                parameter is mandatory if `Y` is not `None`.
+            ignored
 
         Returns
         -------
         scipy.sparse.csr_matrix
             Sparse adjacency matrix describing the unweighted, undirected continuous
             nearest neighbor graph.
 
         Optional[Dict[str, numpy.ndarray]]
             For a pair-wise kernel evaluation, a dictionary with key
             `reference_dist_knn` with the `k`-the nearest neighbors for each point is
             returned.
         """
-
+        self._read_kernel_kwargs(attrs=None, kernel_kwargs=kernel_kwargs)
         is_pdist = Y is None
 
-        reference_dist_knn = self._read_kernel_kwargs(
-            attrs=["reference_dist_knn"], kernel_kwargs=kernel_kwargs
-        )
-
-        dist_kwargs = dist_kwargs or {}
-        # minimum number of neighbors required in sparse case!
-        dist_kwargs.setdefault("kmin", self.k_neighbor)
-
-        distance_matrix = compute_distance_matrix(
-            X, Y, metric="euclidean", **dist_kwargs
-        )
-
-        return self.eval(
-            distance_matrix, is_pdist=is_pdist, reference_dist_knn=reference_dist_knn
-        )
-
-    def _validate(self, distance_matrix, is_pdist, reference_dist_knn):
-        if distance_matrix.ndim != 2:
-            raise ValueError("distance_matrix must be a two-dimensional array")
-
-        n_samples_Y, n_samples_X = distance_matrix.shape
-
-        if is_pdist:
-            if n_samples_Y != n_samples_X:
-                raise ValueError(
-                    "If is_pdist=True, the distance matrix must be square and symmetric."
-                )
-
-            if isinstance(distance_matrix, np.ndarray):
-                diagonal = np.diag(distance_matrix)
-            else:
-                diagonal = np.asarray(distance_matrix.diagonal(0))
-
-            if (diagonal != 0).all():
-                raise ValueError(
-                    "If is_pdist=True, distance_matrix must have zeros on diagonal."
-                )
-        else:
-            if reference_dist_knn is None:
-                raise ValueError(
-                    "If is_pdist=False, 'reference_dist_knn' (=None) must be provided."
-                )
-
-            if not isinstance(reference_dist_knn, np.ndarray):
-                raise TypeError("cdist_reference_k_nn must be of type numpy.ndarray")
-
-            if reference_dist_knn.ndim != 1:
-                raise ValueError("cdist_reference_k_nn must be 1 dim.")
+        distance_matrix = self.distance(X, Y)
+        return self.evaluate(distance_matrix, is_pdist=is_pdist)
 
-            if reference_dist_knn.shape[0] != n_samples_X:
-                raise ValueError(
-                    f"len(cdist_reference_k_nn)={reference_dist_knn.shape[0]} "
-                    f"must be distance.shape[1]={n_samples_X}"
-                )
-
-            if self.k_neighbor < 1 or self.k_neighbor > n_samples_X - 1:
-                raise ValueError(
-                    "'n_neighbors' must be in a range between 1 to the number of samples."
-                )
-
-    def eval(
-        self, distance_matrix, is_pdist=False, reference_dist_knn=None
-    ) -> Tuple[scipy.sparse.csr_matrix, Optional[Dict[Any, np.ndarray]]]:
+    def evaluate(self, distance_matrix, is_pdist=False) -> scipy.sparse.csr_matrix:
         """Evaluate kernel on pre-computed distance matrix.
 
         For return values see :meth:`.__call__`.
 
         Parameters
         ----------
         distance_matrix
             Pre-computed matrix.
 
         is_pdist
             If True, the `distance_matrix` is assumed to be symmetric and with zeros on
             the diagonal (self distances). Note, that there are no checks to validate
             the distance matrix.
-
-        reference_dist_knn
-            An input is required for a component-wise evaluation of the kernel. This is
-            the case if the distance matrix is rectangular or non-symmetric (i.e.,
-            ``is_pdist=False``). The required values are returned for a pre-evaluation
-            of the pair-wise evaluation.
         """
-
-        self._validate(
-            distance_matrix=distance_matrix,
-            is_pdist=is_pdist,
-            reference_dist_knn=reference_dist_knn,
-        )
+        self._validate(distance_matrix=distance_matrix, is_pdist=is_pdist)
+        self._required_attrs(["reference_dist_knn_"], is_fit=is_pdist)
 
         dist_knn = _kth_nearest_neighbor_dist(distance_matrix, self.k_neighbor)
 
         distance_factors = _symmetric_matrix_division(
             distance_matrix,
             vec=np.sqrt(dist_knn),
-            vec_right=np.sqrt(reference_dist_knn)
-            if reference_dist_knn is not None
-            else None,
+            is_symmetric=self.distance.is_symmetric,
+            vec_right=np.sqrt(self.reference_dist_knn_) if not is_pdist else None,
         )
 
         if isinstance(distance_factors, np.ndarray):
             kernel_matrix = scipy.sparse.csr_matrix(
                 distance_factors < self.delta, dtype=bool
             )
         else:
             assert isinstance(distance_factors, scipy.sparse.csr_matrix)
             distance_factors.data = (distance_factors.data < self.delta).astype(bool)
             distance_factors.eliminate_zeros()
             kernel_matrix = distance_factors
 
-        # return dist_knn, which is required for cdist_k_nearest_neighbor in
-        # order to do a follow-up cdist request (then as reference_dist_knn as input).
         if is_pdist:
-            ret_cdist: Optional[Dict[str, np.ndarray]] = dict(
-                reference_dist_knn=dist_knn
+            self.reference_dist_knn_ = dist_knn
+
+        return kernel_matrix
+
+
+class MahalanobisKernel(PCManifoldKernel):  # pragma: no cover
+    """# TODO - description
+    # TODO - citations.
+
+    Parameters
+    ----------
+    epsilon
+        The kernel bandwidth. If "None" (default), it will be estimated from the
+        mahalanobis distance matrix, using the median of 10-th nearest neighbor distances.
+    distance_metric
+        distance metric to use in the pre-computation of the neighborhoods.
+        Default: "euclidean"
+    cov_matrices
+        N*m*m array of N covariance matrices of shape m*m each.
+    """
+
+    def __init__(self, epsilon=None, distance=None):
+        warnings.warn(
+            f"Class '{MahalanobisKernel}' is marked as experimental. This means "
+            f"the intended functionality may not be complete and there is no sufficient "
+            f"testing. Use class with caution!",
+            stacklevel=2,
+        )
+
+        self.epsilon = epsilon
+        super().__init__(is_symmetric=True, distance=distance)
+
+    def __call__(
+        self, X, Y=None, **kernel_kwargs
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        """Compute kernel matrix.
+
+        Parameters
+        ----------
+        X
+            Reference point cloud of shape `(n_samples_X, n_features_X)`.
+
+        Y
+            Query point cloud of shape `(n_samples_Y, n_features_Y)`. If not given,
+            then `Y=X`.
+
+        dist_kwargs,
+            Keyword arguments passed to the distance matrix computation. See
+            :py:meth:`datafold.pcfold.compute_distance_matrix` for parameter arguments.
+
+        kernel_kwargs
+            not supplied
+
+        Returns
+        -------
+        Union[np.ndarray, scipy.sparse.csr_matrix]
+            Kernel matrix of shape `(n_samples_Y, n_samples_X)`. If cut-off is
+            specified in `dist_kwargs`, then the matrix is sparse.
+        """
+        # if not("covariance_matrices" in kernel_kwargs):
+        #    raise ValueError(f"invalid kwargs {kernel_kwargs}, must have covariance_matrices")
+
+        X = np.atleast_2d(X)
+
+        if Y is not None:
+            Y = np.atleast_2d(Y)
+
+        # TODO: Can they also be computed within the kernel?
+        cov_matrices = self._read_kernel_kwargs(
+            attrs=["cov_matrices"], kernel_kwargs=kernel_kwargs
+        )
+
+        distance_matrix = self.distance(X, Y)
+
+        # TODO: the kernel can not handle the out-of-sample case if Y is not None
+        kernel_matrix = self.evaluate(distance_matrix, X, cov_matrices)
+        return kernel_matrix
+
+    def evaluate(
+        self, distance_matrix, X=None, cov_matrices=None
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        """Replace the given distance_matrix with the mahalanobis kernel matrix."""
+        assert X is not None and cov_matrices is not None
+
+        # TODO: efficiency
+        #    -- only compute upper triangle from symmetric distance matrix?
+        #    -- possible to vectorize the inner loop in evaluate()?
+        #    -- parallelize / use numba
+        #    -- efficiently compute cov-matrices?
+        # TODO: out-of-sample property is currently missing
+        # TODO: compute and store cov-matrices for training data within kernel?
+        # TODO: avoid to *only* consider sparse distance matrices -> make it a case
+        #       distinction between dense and sparse
+        # TODO: require epsilon (no additional routine for estimating epsilon)
+
+        # Need only connectivity matrix, NOT distance matrix!!
+        distance_matrix = scipy.sparse.csr_matrix(distance_matrix)
+
+        for row_idx in range(distance_matrix.shape[0]):
+            row = distance_matrix.getrow(row_idx)
+
+            row_point = X[row_idx, :]
+            row_cov_matrix = cov_matrices[row_idx, :, :]
+
+            # iterate through non-zero entries in data
+            for data_index in range(len(row.data)):
+                col_idx = row.indices[data_index]
+                if col_idx != row_idx:
+                    col_point = X[col_idx, :]
+                    col_cov_matrix = cov_matrices[col_idx, :, :]
+
+                    point_diff = row_point - col_point
+
+                    # dist = np.sqrt(0.5 * ||x-y|| @ (V_x + V_y) @ ||x-y||)
+                    mahalanobis_distance = np.sqrt(
+                        0.5
+                        * point_diff
+                        @ (row_cov_matrix + col_cov_matrix)
+                        @ point_diff.T
+                    )
+
+                    # TODO: the indexing could be improved!
+                    distance_matrix.data[
+                        distance_matrix.indptr[row_idx] : distance_matrix.indptr[
+                            row_idx + 1
+                        ]
+                    ][data_index] = mahalanobis_distance
+
+        _epsilon = self.epsilon
+        if _epsilon is None:
+            from datafold.pcfold.estimators import estimate_cutoff, estimate_scale
+
+            cut_off = estimate_cutoff(X, k=25, distance_matrix=distance_matrix)
+            _epsilon = estimate_scale(X, cut_off=cut_off)
+
+        # convert distance to kernel
+        # distance_matrix.data = np.exp(-np.square(distance_matrix.data) / (2 * _epsilon))
+        # TODO: check: above we have sqrt around the mahalanobis_distance, here we have
+        #  a square -- shouldn't this cancel out?
+        distance_matrix.data = np.square(distance_matrix.data, out=distance_matrix.data)
+        kernel_matrix = _apply_kernel_function_numexpr(
+            distance_matrix=distance_matrix,
+            expr="exp((- 1. / (2*eps)) * D)",
+            expr_dict={"eps": _epsilon},
+        )
+
+        # TODO: this operation fails for a k-NN sparse matrix (one that is not symmetric)
+        # make it symmetric
+        kernel_matrix = scipy.sparse.lil_matrix(kernel_matrix)
+        kernel_matrix = scipy.sparse.csr_matrix(0.5 * (kernel_matrix + kernel_matrix.T))
+
+        return kernel_matrix
+
+    def eval2(
+        self, X, distance_matrix, cov_matrices, dist_kwargs
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        """Replace the given distance_matrix with the mahalanobis kernel matrix."""
+        distance_matrix = scipy.sparse.csr_matrix(distance_matrix)
+
+        for row in range(distance_matrix.shape[0]):
+            r = distance_matrix.getrow(row)
+
+            p1 = X[row, :]
+            c1 = cov_matrices[row, :, :]
+            for d_index in range(len(r.data)):
+                col = r.indices[d_index]
+                if col != row:
+                    p2 = X[col, :]
+                    c2 = cov_matrices[col, :, :]
+                    diff = p1 - p2
+                    M_distance = np.sqrt(1 / 2 * diff @ (c1 + c2) @ diff.T)
+
+                    distance_matrix.data[
+                        distance_matrix.indptr[row] : distance_matrix.indptr[row + 1]
+                    ][d_index] = M_distance
+
+        if dist_kwargs is None:
+            dist_kwargs = {}
+
+        _epsilon = self.epsilon
+        if _epsilon is None:
+            from datafold.pcfold.estimators import estimate_cutoff, estimate_scale
+
+            cut_off = estimate_cutoff(
+                X, k=dist_kwargs.get("kmin", 25), distance_matrix=distance_matrix
             )
-        else:
-            ret_cdist = None
+            _epsilon = estimate_scale(X, cut_off=cut_off)
+
+        # convert distance to kernel
+        distance_matrix.data = np.exp(
+            -np.power(distance_matrix.data, 2) / (2 * _epsilon)
+        )
+
+        # make it symmetric
+        distance_matrix = scipy.sparse.lil_matrix(distance_matrix)
+        distance_matrix = scipy.sparse.csr_matrix(
+            0.5 * (distance_matrix + distance_matrix.T)
+        )
 
-        return kernel_matrix, ret_cdist
+        return distance_matrix
 
 
 class DmapKernelFixed(BaseManifoldKernel):
     """Diffusion map kernel with fixed kernel bandwidth.
 
-    This kernel wraps an kernel to describe a diffusion process.
+    This (meta) kernel wraps another kernel to describe a diffusion process.
 
     Parameters
     ----------
-
     internal_kernel
         Kernel that describes the proximity between data points.
 
     is_stochastic
-        If True, the kernel matrix is row-normalized.
+        If True, the kernel matrix is normalized such that the rows sum up to one.
 
     alpha
-        Degree of re-normalization of sampling density in point cloud. `alpha` must be
-        inside the interval [0, 1] (inclusive).
+        Degree of re-normalization of sampling density in point cloud. The parameter ``alpha``
+        must be a float in [0, 1].
 
     symmetrize_kernel
-        If True, performs a conjugate transformation which can improve numerical
-        stability for matrix operations (such as computing eigenpairs). The matrix to
-        change the basis back is provided as a quantity of interest (see
-        possible return values in :meth:`PCManifoldKernel.__call__`).
+        If True, perform a conjugate transformation which can improve numerical
+        stability for follow-up operations (such as computing the kernel eigenpairs). The
+        matrix to change the basis back is stored in the object attribute
+        ``basis_change_matrix_``.
+
+    Attributes
+    ----------
+    row_sums_alpha_: Optional[np.ndarray]
+        Row sum values computed for the re-normalization during an initial pair-wise kernel
+        computation. The parameter is mandatory for the component-wise kernel
+        evaluation and if `alpha>0`.
+
+    basis_change_matrix_: Optional[scipy.sparse.dia_matrix]
+        Basis change matrix (sparse diagonal) if `is_symmetrize=True` and only
+        set if the kernel matrix is a symmetric conjugate of the true
+        diffusion kernel matrix. Required to recover the diffusion map eigenvectors
+        from the eigenvectors of the symmetric conjugate matrix (see :cite:t:`rabin-2012`).
 
     See Also
     --------
     :py:class:`DiffusionMaps`
 
     References
     ----------
-    :cite:`coifman_diffusion_2006`
+    :cite:t:`coifman-2006,rabin-2012`
     """
 
     def __init__(
         self,
-        internal_kernel: PCManifoldKernel = GaussianKernel(epsilon=1.0),
+        internal_kernel: PCManifoldKernel,
+        *,
         is_stochastic: bool = True,
         alpha: float = 1.0,
         symmetrize_kernel: bool = True,
     ):
+        check_scalar(
+            alpha,
+            name="alpha",
+            target_type=(np.integer, int, np.floating, float),
+            min_val=0,
+            max_val=1,
+        )
 
-        self.is_stochastic = is_stochastic
-
-        if not (0 <= alpha <= 1):
-            raise ValueError(f"alpha has to be between [0, 1]. Got alpha={alpha}")
         self.alpha = alpha
         self.symmetrize_kernel = symmetrize_kernel
-
         self.internal_kernel = internal_kernel
 
-        # i) not stochastic -> if the kernel is symmetric the kernel is always
-        # symmetric
-        # `symmetrize_kernel` indicates if the user wants the kernel to use
-        # similarity transformations to solve the
-        # eigenproblem on a symmetric kernel (if required).
-
-        # NOTE: a necessary condition to symmetrize the kernel is that the kernel
-        # is evaluated pairwise
-        #  (i.e. is_pdist = True)
-        #     self._is_symmetric = True
-        # else:
-        #     self._is_symmetric = False
+        is_symmetric = symmetrize_kernel or not is_stochastic
+        super().__init__(is_symmetric=is_symmetric, is_stochastic=is_stochastic)
 
-        self.row_sums_init = None
+    def __repr__(self):
+        return super().__repr__(print_distance=False)
 
-        super(DmapKernelFixed, self).__init__()
+    @property  # type: ignore
+    def distance(self):
+        return self.internal_kernel.distance
+
+    @distance.setter
+    def distance(self, d):
+        # do not use distance here (but forward the distance from the internal kernel
+        return None
 
     @property
-    def is_symmetric(self):
-        return self.symmetrize_kernel or not self.is_stochastic
-
-    def is_symmetric_transform(self) -> bool:
-        """Indicates whether a symmetric conjugate kernel matrix was computed.
-
-        Returns
-        -------
-
+    def is_conjugate(self) -> bool:
+        """Indicates whether a symmetric matrix is computed that is conjugate to a
+        (non-symmetric) stochastic kernel matrix.
         """
-
         # If the kernel is made stochastic, it looses the symmetry, if symmetric_kernel
-        # is set to True, then apply the the symmetry transformation
-        return self.is_stochastic and self.is_symmetric
+        # is set to True, then apply a symmetry transformation
+        return (
+            self.is_stochastic
+            and self._is_symmetric_kernel
+            and self.distance.is_symmetric
+        )
 
     def _normalize_sampling_density(
-        self,
-        kernel_matrix: Union[np.ndarray, scipy.sparse.csr_matrix],
-        row_sums_alpha_fit: np.ndarray,
-    ) -> Tuple[Union[np.ndarray, scipy.sparse.csr_matrix], Optional[np.ndarray]]:
+        self, kernel_matrix: Union[np.ndarray, scipy.sparse.csr_matrix], is_pdist: bool
+    ) -> tuple[Union[np.ndarray, scipy.sparse.csr_matrix], Optional[np.ndarray]]:
         """Normalize (sparse/dense) kernels with positive `alpha` value. This is also
-        referred to a 'renormalization' of sampling density."""
+        referred to a 'renormalization' of sampling density.
+        """
+        if not is_pdist:
+            row_sums_alpha_fit = self.row_sums_alpha_
 
-        if row_sums_alpha_fit is None:
-            assert is_symmetric_matrix(kernel_matrix)
+            if self.row_sums_alpha_.shape[0] != kernel_matrix.shape[1]:
+                raise ValueError("'kernel_matrix' does not have the correct shape")
         else:
-            assert row_sums_alpha_fit.shape[0] == kernel_matrix.shape[1]
+            row_sums_alpha_fit = None
 
         row_sums = kernel_matrix.sum(axis=1)
 
         if scipy.sparse.issparse(kernel_matrix):
             # np.matrix to np.ndarray
             # (np.matrix is deprecated but still used in scipy.sparse)
             row_sums = row_sums.A1
@@ -1346,237 +1570,405 @@
             row_sums_alpha = np.power(row_sums, self.alpha, out=row_sums)
         else:  # no need to power with 1
             row_sums_alpha = row_sums
 
         normalized_kernel = _symmetric_matrix_division(
             matrix=kernel_matrix,
             vec=row_sums_alpha,
+            is_symmetric=self.distance.is_symmetric,
             vec_right=row_sums_alpha_fit,
         )
 
-        if row_sums_alpha_fit is not None:
+        if not is_pdist:
             # Set row_sums_alpha to None for security, because in a cdist-case (if
             # row_sums_alpha_fit) there is no need to further process row_sums_alpha, yet.
             row_sums_alpha = None
 
         return normalized_kernel, row_sums_alpha
 
     def _normalize(
         self,
-        internal_kernel: KernelType,
-        row_sums_alpha_fit: np.ndarray,
+        kernel_matrix: KernelType,
         is_pdist: bool,
     ):
-
-        # only required for symmetric kernel, return None if not used
+        # defaults to None -- only required for a symmetric conjugate kernel matrix
         basis_change_matrix = None
 
-        # required if alpha>0 and _normalize is called later for a cdist case
-        # set in the pdist, alpha > 0 case
+        # defaults ot None -- only required if alpha>0 and normalize is called later for a
+        # cdist case
         row_sums_alpha = None
 
         if self.is_stochastic:
-
             if self.alpha > 0:
                 # if pdist: kernel is still symmetric after this function call
-                (internal_kernel, row_sums_alpha,) = self._normalize_sampling_density(
-                    internal_kernel, row_sums_alpha_fit
-                )
+                (
+                    kernel_matrix,
+                    row_sums_alpha,
+                ) = self._normalize_sampling_density(kernel_matrix, is_pdist)
 
-            if is_pdist and self.is_symmetric_transform():
+            if is_pdist and self.is_conjugate:
                 # Increases numerical stability when solving the eigenproblem
                 # Note1: when using the (symmetric) conjugate matrix, the eigenvectors
                 #        have to be transformed back to match the original
                 # Note2: the similarity transform only works for the is_pdist case
                 #        (for cdist, there is no symmetric kernel in the first place,
                 #        because it is generally rectangular and does not include self
                 #        points)
                 (
-                    internal_kernel,
+                    kernel_matrix,
                     basis_change_matrix,
-                ) = _conjugate_stochastic_kernel_matrix(internal_kernel)
+                ) = _conjugate_stochastic_kernel_matrix(kernel_matrix)
             else:
-                internal_kernel = _stochastic_kernel_matrix(internal_kernel)
+                kernel_matrix = _stochastic_kernel_matrix(kernel_matrix)
 
             # check that if     "is symmetric pdist" -> require basis change
             #            else   no basis change
             assert not (
-                (is_pdist and self.is_symmetric_transform())
-                ^ (basis_change_matrix is not None)
+                (is_pdist and self.is_conjugate) ^ (basis_change_matrix is not None)
             )
 
-        if is_pdist and self.is_symmetric:
-            assert is_symmetric_matrix(internal_kernel)
-
-        return internal_kernel, basis_change_matrix, row_sums_alpha
+        return kernel_matrix, basis_change_matrix, row_sums_alpha
 
-    def _validate_row_alpha_fit(self, is_pdist, row_sums_alpha_fit):
-        if (
-            self.is_stochastic
-            and self.alpha > 0
-            and not is_pdist
-            and row_sums_alpha_fit is None
-        ):
-            raise ValueError(
-                "cdist request can not be carried out, if 'row_sums_alpha_fit=None'"
-                "Please consider to report bug."
-            )
-
-    def _eval(self, kernel_output, is_pdist, row_sums_alpha_fit):
-
-        self._validate_row_alpha_fit(
-            is_pdist=is_pdist, row_sums_alpha_fit=row_sums_alpha_fit
-        )
-
-        kernel_matrix, internal_ret_cdist, _ = PCManifoldKernel.read_kernel_output(
-            kernel_output=kernel_output
+    def _eval_kernel_matrix(self, kernel_matrix, is_pdist):
+        self._required_attrs(
+            attrs=["row_sums_alpha_", "basis_change_matrix_"], is_fit=is_pdist
         )
 
         if isinstance(kernel_matrix, pd.DataFrame):
             # store indices and cast to same type later
             _type = type(kernel_matrix)
             rows_idx, columns_idx = kernel_matrix.index, kernel_matrix.columns
             kernel_matrix = kernel_matrix.to_numpy()
         else:
             _type, rows_idx, columns_idx = None, None, None
 
         kernel_matrix, basis_change_matrix, row_sums_alpha = self._normalize(
             kernel_matrix,
-            row_sums_alpha_fit=row_sums_alpha_fit,
             is_pdist=is_pdist,
         )
 
         if rows_idx is not None and columns_idx is not None:
             kernel_matrix = _type(kernel_matrix, index=rows_idx, columns=columns_idx)
 
         if is_pdist:
-            ret_cdist = dict(
-                row_sums_alpha_fit=row_sums_alpha,
-                internal_kernel_kwargs=internal_ret_cdist,
-            )
-            ret_extra = dict(basis_change_matrix=basis_change_matrix)
-        else:
-            # no need for row_sums_alpha or the basis change matrix in the cdist case
-            ret_cdist = None
-            ret_extra = None
+            self.row_sums_alpha_ = row_sums_alpha
+            self.basis_change_matrix_ = basis_change_matrix
 
-        return kernel_matrix, ret_cdist, ret_extra
+        return kernel_matrix
 
     def __call__(
         self,
         X: np.ndarray,
         Y: Optional[np.ndarray] = None,
-        *,
-        dist_kwargs: Optional[Dict] = None,
         **kernel_kwargs,
-    ) -> Tuple[
-        Union[np.ndarray, scipy.sparse.csr_matrix], Optional[Dict], Optional[Dict]
-    ]:
-        """Compute the diffusion map kernel.
+    ) -> Union[np.ndarray, scipy.sparse.csr_matrix]:
+        """Compute kernel matrix.
+
+        .. note::
+            Before evaluating the component-wise kernel matrix (with :code:`kernel(X,Y)`) it
+            is first required to evaluate the pairwise kernel matrix (with :code:`kernel(X)`)
+            to set necessary attributes from the reference points.
 
         Parameters
         ----------
         X
             Reference point cloud of shape `(n_samples_X, n_features_X)`.
 
         Y
             Query point cloud of shape `(n_samples_Y, n_features_Y)`. If not given,
             then `Y=X`.
 
-        dist_kwargs
-            Keyword arguments passed to the internal distance matrix computation. See
-            :py:meth:`datafold.pcfold.compute_distance_matrix` for parameter arguments.
-
-        **kernel_kwargs: Dict[str, object]
-            - internal_kernel_kwargs: Optional[Dict]
-                Keyword arguments passed to the set internal kernel.
-            - row_sums_alpha_fit: Optional[np.ndarray]
-                Row sum values during re-normalization computed during pair-wise kernel
-                computation. The parameter is mandatory for the compontent-wise kernel
-                computation and if `alpha>0`.
+        **kernel_kwargs
+            passed to `kernel_kwargs` of internal kernel
 
         Returns
         -------
-        numpy.ndarray`, `scipy.sparse.csr_matrix`
-            kernel matrix (or conjugate of it) with same type and shape as
+        `numpy.ndarray`, `scipy.sparse.csr_matrix`
+            kernel matrix (or symmetric conjugate of it) with same type and shape as
             `distance_matrix`
-
-        Optional[Dict[str, numpy.ndarray]]
-            Row sums from re-normalization in key 'row_sums_alpha_fit', only returned for
-            pairwise computations. The values are required for follow up out-of-sample
-            kernel evaluations (`Y is not None`).
-
-        Optional[Dict[str, scipy.sparse.dia_matrix]]
-            Basis change matrix (sparse diagonal) if `is_symmetrize=True` and only
-            returned if the kernel matrix is a symmetric conjugate of the true
-            diffusion kernel matrix. Required to recover the diffusion map eigenvectors
-            from the symmetric conjugate matrix.
         """
-
         is_pdist = Y is None
 
-        internal_kernel_kwargs, row_sums_alpha_fit = self._read_kernel_kwargs(
-            attrs=["internal_kernel_kwargs", "row_sums_alpha_fit"],
-            kernel_kwargs=kernel_kwargs,
-        )
-
-        kernel_output = self.internal_kernel(
-            X, Y=Y, dist_kwargs=dist_kwargs or {}, **internal_kernel_kwargs or {}
-        )
+        if is_pdist:
+            kernel_matrix = self.internal_kernel(X, **kernel_kwargs)
+        else:
+            kernel_matrix = self.internal_kernel(X, Y, **kernel_kwargs)
 
-        return self._eval(
-            kernel_output=kernel_output,
-            is_pdist=is_pdist,
-            row_sums_alpha_fit=row_sums_alpha_fit,
-        )
+        return self._eval_kernel_matrix(kernel_matrix=kernel_matrix, is_pdist=is_pdist)
 
-    def eval(
+    def evaluate(
         self,
         distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix],
         is_pdist=False,
-        row_sums_alpha_fit=None,
     ):
         """Evaluate kernel on pre-computed distance matrix.
 
         For return values see :meth:`.__call__`.
 
         Parameters
         ----------
-
         distance_matrix
             Matrix of shape `(n_samples_Y, n_samples_X)`.
 
         is_pdist:
             If True, the distance matrix must be square
 
         Returns
         -------
+        `numpy.ndarray`, `scipy.sparse.csr_matrix`
+            Kernel matrix with same shape and type of distance matrix.
         """
+        kernel_matrix = self.internal_kernel.evaluate(distance_matrix)
 
-        kernel_output = self.internal_kernel.eval(distance_matrix)
-        return self._eval(
-            kernel_output=kernel_output,
+        return self._eval_kernel_matrix(
+            kernel_matrix=kernel_matrix,
             is_pdist=is_pdist,
-            row_sums_alpha_fit=row_sums_alpha_fit,
         )
 
 
+class RoselandKernel(PCManifoldKernel):
+    """Roseland kernel to describe a diffusion process with respect to landmarks on a point
+    cloud.
+
+    This kernel wraps a kernel that describes the point neighborhood. Note that the kernel
+    matrix is usually not square because there are less landmarks than points.
+
+    Parameters
+    ----------
+    internal_kernel
+        Kernel that describes the proximity between data points.
+
+    alpha
+        Degree of re-normalization of sampling density in point cloud. The parameter ``alpha``
+        must be a float inside the interval [0, 1].
+
+    Attributes
+    ----------
+    landmark_density_: Optional[np.ndarray]
+        Point density values at the reference points in a pairwise kernel evaluation. This
+        attribute is only set if ``alpha>0``. The values are required for follow-up
+        component-wise kernel evaluations.
+
+    stochastic_normalization_: np.ndarray
+        Diagonal elements of the normalization matrix for the refrence points in a pairwise
+        kernel evaluation. The values are required for follow-up component-wise kernel
+        evaluations.
+
+    References
+    ----------
+    :cite:t:`shen-2020`
+    """
+
+    def __init__(self, internal_kernel, alpha=0):
+        self.internal_kernel = internal_kernel
+
+        check_scalar(
+            alpha,
+            "alpha",
+            target_type=(np.integer, int, np.floating, float),
+            min_val=0,
+            max_val=1,
+        )
+        self.alpha = alpha
+        super().__init__(is_symmetric=False, is_stochastic=False)
+
+    def _cast_array(self, obj, is_sparse):
+        # Scipy's sparse matrices use the deprecated matrix module from Numpy
+        # The attribute A1 turns a matrix object to an array
+        return obj.A1 if is_sparse else obj
+
+    def _normalize_density(self, kernel_matrix, is_fit):
+        is_sparse = scipy.sparse.spmatrix(kernel_matrix)
+
+        if is_fit:
+            landmark_density = self._cast_array(kernel_matrix.sum(axis=0), is_sparse)
+        else:
+            landmark_density = self.landmark_density_
+
+        data_density = self._cast_array(kernel_matrix.sum(axis=1), is_sparse)
+
+        normalized_kernel_matrix = _symmetric_matrix_division(
+            kernel_matrix,
+            vec=data_density,
+            is_symmetric=False,
+            vec_right=landmark_density,
+        )
+
+        return normalized_kernel_matrix, landmark_density
+
+    def _compute_normalize_diagonal(self, kernel_matrix, is_fit):
+        """This function computes.
+
+        .. code::
+
+            normalize_diagonal = np.sqrt((kernel_matrix @ kernel_matrix.T).sum(axis=1))
+
+        without evaluating :code:`kernel_matrix @ kernel_matrix.T`.
+
+        In the paper this is the diagonal of :math:`D^{-1/2}`.
+        """
+        is_sparse = scipy.sparse.issparse(kernel_matrix)
+
+        if is_fit:
+            stochastic_normalization = self._cast_array(
+                kernel_matrix.sum(axis=0), is_sparse
+            )
+        else:
+            stochastic_normalization = self.stochastic_normalization_
+
+        # Alternative computation,
+        #   normalize_diagonal = np.sqrt((kernel_matrix @ kernel_matrix.T).sum(axis=1))
+        # However, this does not separate the "stochastic_normalization" part,
+        # which is required later for an out-of-sample embedding.
+
+        kernel_matrix_adapted = mat_dot_diagmat(kernel_matrix, stochastic_normalization)
+
+        normalize_diagonal = self._cast_array(
+            np.sqrt(np.sum(kernel_matrix_adapted, axis=1)), is_sparse
+        )
+
+        with np.errstate(divide="ignore"):
+            # The reciprocal can be inf when a landmark has no neighbors.
+            # These cases are treated separately in 'bool_invalid' below
+            normalize_diagonal = np.reciprocal(
+                normalize_diagonal, out=normalize_diagonal
+            )
+
+            bool_invalid = np.logical_or(
+                np.isinf(normalize_diagonal), normalize_diagonal < 0
+            )
+            normalize_diagonal[bool_invalid] = 0
+
+        return stochastic_normalization, normalize_diagonal
+
+    def _eval_kernel_matrix(self, kernel_matrix):
+        """Normalizes the kernel matrix.
+
+        This function performs
+
+        .. math::
+
+            M = D^{-1/2} K
+
+        where matrix :math:`M` is the normalized kernel matrix from :math:`K` by the
+        diagonal matrix :math:`D`.
+
+        Parameters
+        ----------
+        kernel_matrix
+            kernel matrix (square or rectangular) to normalize
+
+        Returns
+        -------
+        Union[np.ndarray, scipy.sparse.spmatrix]
+            normalized kernel matrix with type same as `kernel_matrix`
+        """
+        # indicates whether the kernel has been executed for pairwise before
+        is_fit = not hasattr(self, "stochastic_normalization_") or not hasattr(
+            self, "landmark_density_"
+        )
+
+        self._required_attrs(
+            attrs=["stochastic_normalization_", "landmark_density_"], is_fit=is_fit
+        )
+
+        if self.alpha > 0:
+            kernel_matrix, landmark_density = self._normalize_density(
+                kernel_matrix, is_fit=is_fit
+            )
+        else:
+            landmark_density = None
+
+        (
+            stochastic_normalization,
+            normalize_diagonal,
+        ) = self._compute_normalize_diagonal(kernel_matrix=kernel_matrix, is_fit=is_fit)
+
+        kernel_matrix = diagmat_dot_mat(
+            normalize_diagonal, kernel_matrix, out=kernel_matrix
+        )
+
+        if is_fit:
+            self.stochastic_normalization_ = stochastic_normalization
+            self.landmark_density_ = landmark_density
+
+        self.normalize_diagonal_ = normalize_diagonal
+
+        return kernel_matrix
+
+    def __call__(
+        self,
+        X: np.ndarray,
+        Y: Optional[np.ndarray] = None,
+        **kernel_kwargs,
+    ):
+        """Compute kernel matrix.
+
+        Parameters
+        ----------
+        X
+            Landmark points of shape `(n_samples_X, n_features_X)`.
+
+        Y
+            Query point cloud of shape `(n_samples_Y, n_features_Y)`. Note that `Y` is not
+            optional here.
+
+        **kernel_kwargs
+            None
+
+        Returns
+        -------
+        `numpy.ndarray`, `scipy.sparse.csr_matrix`
+            kernel matrix (or symmetric conjugate of it) with same type and shape of
+            `(n_samples_X, n_samples_Y)`.
+        """
+        if Y is None:
+            raise ValueError(
+                "For the landmarked kernel parameter Y must always be provided"
+            )
+
+        kernel_matrix = self.internal_kernel(X, Y=Y)
+        return self._eval_kernel_matrix(kernel_matrix=kernel_matrix)
+
+    def evaluate(
+        self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix], is_fit=False
+    ):
+        """Evaluate kernel on pre-computed distance matrix.
+
+        Parameters
+        ----------
+        distance_matrix
+            Matrix of shape `(n_samples_Y, n_samples_X)`.
+
+        is_fit:
+            If True,
+
+        Returns
+        -------
+        `np.ndarray`, `scipy.sparse.csr_matrix`
+            kernel matrix with same type and shape as distance matrix
+        """
+        kernel_matrix = self.internal_kernel.evaluate(distance_matrix)
+        return self._eval_kernel_matrix(kernel_matrix=kernel_matrix)
+
+
 class ConeKernel(TSCManifoldKernel):
-    r"""Compute a dynamics adapted cone kernel for time series collection data.
+    r"""Compute a dynamically adapted cone kernel on time series collection data.
 
     The equations below describe the kernel evaluation and are taken from the referenced
     paper below.
 
-    A single kernel evaluation between samples :math:`x` and :math:`y` is computed with
+    A single kernel evaluation between time series samples :math:`x` and :math:`y` is computed
+    with
 
     .. math::
         K(x, y) = \exp
         \left(
         -\frac{\vert\vert \omega_{ij}\vert\vert^2}
-        {\varepsilon \delta t^2 \vert\vert \xi_i \vert\vert \vert\vert \xi_j \vert\vert }
+        {\varepsilon \Delta t^2 \vert\vert \xi_i \vert\vert \vert\vert \xi_j \vert\vert }
         \left[ (1-\zeta \cos^2 \theta_i)(1-\zeta \cos^2 \theta_j) \right]^{0.5}
         \right)
 
     where,
 
     .. math::
         \cos \theta_i =
@@ -1587,47 +1979,46 @@
 
     .. math::
         \omega_{ij} = y - x
 
     is a difference vector between the point pairs,
 
     .. math::
-        \delta t
+        \Delta t
 
     is the (constant) time sampling in the time series,
 
     .. math::
         \varepsilon
 
     is an additional scaling parameter of the kernel bandwidth,
 
     .. math::
         \zeta
 
     is the parameter to control the angular influence, and
 
     .. math::
-        \xi_i = \delta_p x_i = \sum_{j=-p/2}^{p/2} w_j x_{i+j}
+        \xi_i = \Delta_p x_i = \sum_{j=-p/2}^{p/2} w_j x_{i+j}
 
     is the approximation of the dynamical vector field. The approximation is carried
-    out with :math:`\delta_p`, a :math:`p`-th order accurate central finite difference
-    (in a sense that :math:`\frac{\xi}{\delta t} + \mathcal{O}(\delta t^p)`) with
+    out with :math:`\Delta_p`, a :math:`p`-th order accurate central finite difference
+    (in a sense that :math:`\frac{\xi}{\Delta t} + \mathcal{O}(\Delta t^p)`) with
     associated weights :math:`w`.
 
     .. note::
         In the centered finite difference the time values are shifted such that no
         samples are taken from the future. For exmaple, for the scheme
         :math:`x_{t+1} - x_{t-1}`, at time :math:`t`, then the new assigned time value
         is `t+1`. See also :py:meth:`.TSCAccessor.time_derivative`.
 
     Parameters
     ----------
-
     zeta
-        A scalar between :math:`[0, 1)` that controls the angular influence . The
+        A scalar between :math:`[0, 1)` to control the angular influence. The
         weight from one point to a neighboring point is increased if the relative
         displacement vector is aligned with the dynamical flow. The special case of
         `zeta=0`, corresponds to the so-called "Non-Linear Laplacian Spectral
         Analysis" kernel (NLSA).
 
     epsilon
         An additional scaling parameter with which the kernel scale can be adapted to
@@ -1636,53 +2027,82 @@
     fd_accuracy
         The accuracy of the centered finite difference scheme (:math:`p`
         in the description). Note, that the higher the order the more smaples are
         required in a warm-up phase, where the centered scheme cannot be evaluated with
         the given accuracy. All samples from this warm-up phase are dropped in the
         kernel evaluation.
 
-    References
+    Attributes
     ----------
+    timederiv_X_: np.ndarray
+        The time derivative from the finite difference scheme for the reference data `X`.
+        Required for the component-wise evaluation and only available after a pairse
+        evaluation of the kernel.
+
+    norm_timederiv_X_: np.ndarray
+        Norm of the time derivative for the reference data `X`. Required for the
+        component-wise evaluation and only available after a pairse evaluation of the kernel.
 
-    :cite:`giannakis_dynamics-adapted_2015` (the equations are taken from the
+    References
+    ----------
+    :cite:t:`giannakis-2015` (the equations are taken from the
     `arXiv version <https://arxiv.org/abs/1403.0361>`__)
     """
 
-    def __init__(self, zeta: float = 0.0, epsilon: float = 1.0, fd_accuracy: int = 4):
+    def __init__(
+        self,
+        zeta: float = 0.0,
+        epsilon: float = 1.0,
+        fd_accuracy: int = 4,
+        distance=None,
+    ):
         self.zeta = zeta
         self.epsilon = epsilon
         self.fd_accuracy = fd_accuracy
 
-    def _validate_setting(self, X, Y):
+        distance = distance or {}
+
+        distance.setdefault("metric", "sqeuclidean")
 
+        cut_off = distance.get("cut_off", None)
+        if cut_off is not None and not np.isinf(cut_off):
+            raise NotImplementedError(
+                "Sparse kernel matrix (by setting cut_off) is currently not implemented!"
+            )
+
+        self.timederiv_X_: np.ndarray
+        self.norm_timederiv_X_: np.ndarray
+
+        super().__init__(distance=distance)
+
+    def _validate_parameter(self, X, Y):
         # cannot import in top of file, because this creates circular imports
-        from datafold.pcfold.timeseries.collection import TSCDataFrame, TSCException
+        from datafold.pcfold.timeseries.collection import TSCDataFrame
 
         check_scalar(
             self.zeta,
             name="zeta",
             target_type=(float, np.floating, int, np.integer),
             min_val=0.0,
-            max_val=1.0 - np.finfo(float).eps,
+            max_val=1.0,
+            include_boundaries="left",
         )
 
         check_scalar(
             self.epsilon,
             name="epsilon",
             target_type=(float, np.floating, int, np.integer),
-            min_val=np.finfo(float).eps,
-            max_val=None,
+            min_val=0,
         )
 
         check_scalar(
             self.fd_accuracy,
             "fd_accuracy",
             target_type=(int, np.integer),
             min_val=1,
-            max_val=None,
         )
 
         # make sure to only deal with Python built-in types
         self.zeta = float(self.zeta)
         self.epsilon = float(self.epsilon)
         self.fd_accuracy = int(self.fd_accuracy)
 
@@ -1713,15 +2133,14 @@
         self,
         Y_numpy: np.ndarray,
         timederiv_Y: np.ndarray,
         norm_timederiv_Y: np.ndarray,
         X_numpy: Optional[np.ndarray] = None,
         distance_matrix=None,
     ):
-
         if X_numpy is None:
             X_numpy = Y_numpy
 
         is_compute_distance = distance_matrix is None
 
         # pre-allocate cosine- and distance-matrix
         cos_matrix = np.zeros((Y_numpy.shape[0], X_numpy.shape[0]))
@@ -1783,61 +2202,45 @@
 
         return timederiv, norm_timederiv
 
     def __call__(
         self,
         X: pd.DataFrame,
         Y: Optional[pd.DataFrame] = None,
-        *,
-        dist_kwargs: Optional[Dict[str, object]] = None,
         **kernel_kwargs,
     ):
         """Compute kernel matrix.
 
         Parameters
         ----------
         X
             The reference time series collection of shape `(n_samples_X, n_features_X)`.
         Y
             The query time series collection of shape `(n_samples_Y, n_features_Y)`. If
             `Y` is not provided, then ``Y=X``.
 
-        dist_kwargs
-            ignored `(The distance matrix is computed as part of the kernel evaluation.
-            For now this can only be a dense matrix).`
-
-        **kernel_kwargs: Dict[str, object]
-            - timederiv_X
-                The time derivative from a finite difference scheme. Required for a
-                component-wise evaluation.
-            - norm_timederiv_X
-                Norm of the time derivative. Required for a component-wise evaluation.
+        **kernel_kwargs
+            None
 
         Returns
         -------
         TSCDataFrame
             The kernel matrix with time information.
         """
+        delta_time = self._validate_parameter(X, Y)
+        is_pdist = Y is None
 
-        delta_time = self._validate_setting(X, Y)
-
-        timederiv_X, norm_timederiv_X = self._read_kernel_kwargs(
-            attrs=["timederiv_X", "norm_timederiv_X"], kernel_kwargs=kernel_kwargs
+        compute_attributes = is_pdist or (
+            not hasattr(self, "timederiv_X_") or not hasattr(self, "norm_timederiv_X_")
         )
 
-        is_pdist = Y is None
-
-        if is_pdist:
+        if compute_attributes:
             timederiv_X, norm_timederiv_X = self._approx_dynflow(X=X)
         else:
-            if timederiv_X is None or norm_timederiv_X is None:
-                raise ValueError(
-                    "For component wise computation the parameters 'timederiv_X' "
-                    "and 'norm_timederiv_X' must be provided. "
-                )
+            timederiv_X, norm_timederiv_X = self.timederiv_X_, self.norm_timederiv_X_
 
         # NOTE: samples are dropped here which are at the time series boundaries. How
         # many, depends on the accuracy level of the time derivative.
         X_numpy = X.loc[timederiv_X.index].to_numpy()
 
         if is_pdist:
             timederiv_Y = timederiv_X
@@ -1855,22 +2258,23 @@
                 cos_matrix = np.multiply(
                     cos_matrix_Y_X, cos_matrix_Y_X.T, out=cos_matrix_Y_X
                 )
                 cos_matrix = np.sqrt(cos_matrix, out=cos_matrix)
                 # squared Euclidean metric
                 distance_matrix = np.square(distance_matrix, out=distance_matrix)
             else:
-                distance_matrix = compute_distance_matrix(X_numpy, metric="sqeuclidean")
+                distance_matrix = self.distance(X=X_numpy)
                 cos_matrix = np.ones((X_numpy.shape[0], X_numpy.shape[0]))
 
             factor_matrix = _symmetric_matrix_division(
                 cos_matrix,
                 vec=norm_timederiv_X.to_numpy().ravel(),
+                is_symmetric=True,
                 vec_right=None,
-                scalar=(delta_time ** 2) * self.epsilon,
+                scalar=(delta_time**2) * self.epsilon,
                 value_zero_division=0,
             )
 
         else:
             assert isinstance(Y, pd.DataFrame)  # mypy
 
             timederiv_Y, norm_timederiv_Y = self._approx_dynflow(X=Y)
@@ -1902,24 +2306,23 @@
                 cos_matrix = np.multiply(
                     cos_matrix_Y_X, cos_matrix_X_Y.T, out=cos_matrix_Y_X
                 )
                 cos_matrix = np.sqrt(cos_matrix, out=cos_matrix)
                 # squared Euclidean metric
                 distance_matrix = np.square(distance_matrix, out=distance_matrix)
             else:
-                distance_matrix = compute_distance_matrix(
-                    X_numpy, Y_numpy, metric="sqeuclidean"
-                )
+                distance_matrix = self.distance(X_numpy, Y_numpy)
                 cos_matrix = np.ones((Y_numpy.shape[0], X_numpy.shape[0]))
 
             factor_matrix = _symmetric_matrix_division(
                 cos_matrix,
                 vec=norm_timederiv_Y.to_numpy().ravel(),
+                is_symmetric=False,
                 vec_right=norm_timederiv_X.to_numpy().ravel(),
-                scalar=(delta_time ** 2) * self.epsilon,
+                scalar=(delta_time**2) * self.epsilon,
                 value_zero_division=0,
             )
 
         assert np.isfinite(factor_matrix).all()
 
         kernel_matrix = _apply_kernel_function_numexpr(
             distance_matrix=distance_matrix,
@@ -1929,63 +2332,56 @@
 
         kernel_matrix = df_type_and_indices_from(
             indices_from=timederiv_Y,
             values=kernel_matrix,
             except_columns=[f"X{i}" for i in np.arange(X_numpy.shape[0])],
         )
 
-        if is_pdist:
-            ret_cdist: Optional[Dict[str, Any]] = dict(
-                timederiv_X=timederiv_X, norm_timederiv_X=norm_timederiv_X
-            )
-        else:
-            ret_cdist = None
+        if compute_attributes:
+            self.timederiv_X_ = timederiv_X
+            self.norm_timederiv_X_ = norm_timederiv_X
 
-        return kernel_matrix, ret_cdist
+        return kernel_matrix
 
 
 class DmapKernelVariable(BaseManifoldKernel):  # pragma: no cover
     """Diffusion maps kernel with variable kernel bandwidth.
 
     .. warning::
         This class is not documented. Contributions are welcome
             * documentation
             * unit- or functional-testing
 
     References
     ----------
-    :cite:`berry_nonparametric_2015`
-    :cite:`berry_variable_2016`
+    :cite:`berry-2015,berry-2016`
 
     See Also
     --------
     :py:class:`DiffusionMapsVariable`
 
     """
 
-    def __init__(self, epsilon, k, expected_dim, beta, symmetrize_kernel):
+    def __init__(
+        self, epsilon, k, expected_dim, beta, symmetrize_kernel, distance=None
+    ):
         if expected_dim <= 0 and not is_integer(expected_dim):
             raise ValueError("expected_dim has to be a non-negative integer.")
 
         if epsilon < 0 and not not is_float(expected_dim):
             raise ValueError("epsilon has to be positive float.")
 
         if k <= 0 and not is_integer(expected_dim):
             raise ValueError("k has to be a non-negative integer.")
 
         self.beta = beta
         self.epsilon = epsilon
         self.k = k
         self.expected_dim = expected_dim  # variable 'd' in paper
 
-        if symmetrize_kernel:  # allows to later on include a stochastic option...
-            self.is_symmetric = True
-        else:
-            self.is_symmetric = False
-
         self.alpha = -self.expected_dim / 4
         c2 = (
             1 / 2
             - 2 * self.alpha
             + 2 * self.expected_dim * self.alpha
             + self.expected_dim * self.beta / 2
             + self.beta
@@ -1994,31 +2390,44 @@
         if c2 >= 0:
             raise ValueError(
                 "Theory requires c2 to be negative:\n"
                 "c2 = 1/2 - 2 * alpha + 2 * expected_dim * alpha + expected_dim * "
                 f"beta/2 + beta \n but is {c2}"
             )
 
+        # TODO: this overwrites the user input -- also allow type DistanceAlgorithm
+        #  (e.g. sparse matrix)
+        distance = {}
+        distance["backend"] = "brute"
+        distance["metric"] = "sqeuclidean"
+        distance["cut_off"] = None
+
+        # TODO: currently the kernel computes the LB generator (i.e. is_stochastic must be
+        #  False, if the operator is computed, then max(eigval)==1
+        super().__init__(
+            is_symmetric=symmetrize_kernel, is_stochastic=False, distance=distance
+        )
+
     def is_symmetric_transform(self, is_pdist):
         # If the kernel is made stochastic, it looses the symmetry, if symmetric_kernel
-        # is set to True, then apply the the symmetry transformation
-        return is_pdist and self.is_symmetric
+        # is set to True, then apply the symmetry transformation
+        return is_pdist and self._is_symmetric_kernel
 
     def _compute_rho0(self, distance_matrix):
         """Ad hoc bandwidth function."""
         nr_samples = distance_matrix.shape[1]
 
         # both modes are equivalent, MODE=1 allows to easier compare with ref3.
         MODE = 1
         if MODE == 1:  # according to Berry code
             # keep only nearest neighbors
             distance_matrix = np.sort(np.sqrt(distance_matrix), axis=1)[
                 :, 1 : self.k + 1
             ]
-            rho0 = np.sqrt(np.mean(distance_matrix ** 2, axis=1))
+            rho0 = np.sqrt(np.mean(distance_matrix**2, axis=1))
         else:  # MODE == 2:  , more performant if required
             if self.k < nr_samples:
                 # TODO: have to revert setting the inf
                 #   -> check that the diagonal is all zeros
                 #   -> set to inf
                 #   -> after computation set all infs back to zero
                 #   -> this is also very similar to continous-nn in PCManifold
@@ -2050,58 +2459,57 @@
             # suffices
             rho0 = np.sqrt(np.nanmean(distance_matrix, axis=1))
 
         return rho0
 
     def _compute_q0(self, distance_matrix, rho0):
         """The sampling density."""
-
         meanrho0 = np.mean(rho0)
         rho0tilde = rho0 / meanrho0
 
         # TODO: eps0 could also be optimized (see Berry Code + paper ref2)
-        eps0 = meanrho0 ** 2
+        eps0 = meanrho0**2
 
         expon_matrix = _symmetric_matrix_division(
-            matrix=-distance_matrix, vec=rho0tilde, scalar=2 * eps0
+            matrix=-distance_matrix, vec=rho0tilde, is_symmetric=True, scalar=2 * eps0
         )
 
         nr_samples = distance_matrix.shape[0]
 
         # according to eq. (10) in ref1
         q0 = (
             np.power(2 * np.pi * eps0, -self.expected_dim / 2)
             / (np.power(rho0, self.expected_dim) * nr_samples)
             * np.sum(np.exp(expon_matrix), axis=1)
         )
 
         return q0
 
     def _compute_rho(self, q0):
-        """The bandwidth function for K_eps_s"""
+        """The bandwidth function for K_eps_s."""
         rho = np.power(q0, self.beta)
 
         # Division by rho-mean is not in papers, but in berry code (ref3)
         return rho / np.mean(rho)
 
     def _compute_kernel_eps_s(self, distance_matrix, rho):
         expon_matrix = _symmetric_matrix_division(
-            matrix=distance_matrix, vec=rho, scalar=-4 * self.epsilon
+            matrix=distance_matrix, vec=rho, is_symmetric=True, scalar=-4 * self.epsilon
         )
         kernel_eps_s = np.exp(expon_matrix, out=expon_matrix)
         return kernel_eps_s
 
     def _compute_q_eps_s(self, kernel_eps_s, rho):
         rho_power_dim = np.power(rho, self.expected_dim)[:, np.newaxis]
         q_eps_s = np.sum(kernel_eps_s / rho_power_dim, axis=1)
         return q_eps_s
 
     def _compute_kernel_eps_alpha_s(self, kernel_eps_s, q_eps_s):
         kernel_eps_alpha_s = _symmetric_matrix_division(
-            matrix=kernel_eps_s, vec=np.power(q_eps_s, self.alpha)
+            matrix=kernel_eps_s, vec=np.power(q_eps_s, self.alpha), is_symmetric=True
         )
 
         return kernel_eps_alpha_s
 
     def _compute_matrix_l(self, kernel_eps_alpha_s, rho):
         rhosq = np.square(rho)[:, np.newaxis]
         n_samples = rho.shape[0]
@@ -2109,70 +2517,53 @@
         return matrix_l
 
     def _compute_matrix_s_inv(self, rho, q_eps_alpha_s):
         s_diag = np.reciprocal(rho * np.sqrt(q_eps_alpha_s))
         return scipy.sparse.diags(s_diag)
 
     def _compute_matrix_l_conjugate(self, kernel_eps_alpha_s, rho, q_eps_alpha_s):
-
         basis_change_matrix = self._compute_matrix_s_inv(rho, q_eps_alpha_s)
 
         p_sq_inv = scipy.sparse.diags(np.reciprocal(np.square(rho)))
 
         matrix_l_hat = (
             basis_change_matrix @ kernel_eps_alpha_s @ basis_change_matrix
             - (p_sq_inv - scipy.sparse.diags(np.ones(kernel_eps_alpha_s.shape[0])))
         )
 
         matrix_l_hat = remove_numeric_noise_symmetric_matrix(matrix_l_hat)
 
         return matrix_l_hat, basis_change_matrix
 
-    def __call__(self, X, Y=None, *, dist_kwargs=None, **kernel_kwargs):
-
-        dist_kwargs = dist_kwargs or {}
-        cut_off = dist_kwargs.pop("cut_off", None)
-
+    def __call__(self, X, Y=None, **kernel_kwargs):
         self._read_kernel_kwargs(attrs=None, kernel_kwargs=kernel_kwargs)
 
-        if cut_off is not None and not np.isinf(cut_off):
-            raise NotImplementedError("Handling sparsity is currently not implemented!")
-
         if Y is not None:
             raise NotImplementedError("cdist case is currently not implemented!")
 
         if self.k > X.shape[0]:
             raise ValueError(
                 f"nr of nearest neighbors (self.k={self.k}) "
                 f"is larger than number of samples (={X.shape[0]})"
             )
 
-        distance_matrix = compute_distance_matrix(
-            X,
-            Y,
-            metric="sqeuclidean",
-            **dist_kwargs,
-        )
-
-        operator_l_matrix, basis_change_matrix, rho0, rho, q0, q_eps_s = self.eval(
-            distance_matrix
-        )
+        distance_matrix = self.distance(X, Y)
 
-        # TODO: this is not yet aligned to the kernel_matrix, cdist_dict, extra_dict
-        return (
+        (
             operator_l_matrix,
-            basis_change_matrix,
-            rho0,
-            rho,
-            q0,
-            q_eps_s,
-        )
+            self.basis_change_matrix_,
+            self.rho0_,
+            self.rho_,
+            self.q0_,
+            self.q_eps_s_,
+        ) = self.evaluate(distance_matrix)
 
-    def eval(self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]):
+        return operator_l_matrix
 
+    def evaluate(self, distance_matrix: Union[np.ndarray, scipy.sparse.csr_matrix]):
         if scipy.sparse.issparse(distance_matrix):
             raise NotImplementedError(
                 "Currently DmapKernelVariable is only implemented to handle a dense "
                 "distance matrix."
             )
 
         assert (
@@ -2186,15 +2577,15 @@
         kernel_eps_s = self._compute_kernel_eps_s(distance_matrix, rho)
         q_eps_s = self._compute_q_eps_s(kernel_eps_s, rho)
         kernel_eps_alpha_s = self._compute_kernel_eps_alpha_s(kernel_eps_s, q_eps_s)
 
         # can be expensive
         assert is_symmetric_matrix(kernel_eps_alpha_s)
 
-        if self.is_symmetric:
+        if self._is_symmetric_kernel:
             q_eps_alpha_s = kernel_eps_alpha_s.sum(axis=1)
             operator_l_matrix, basis_change_matrix = self._compute_matrix_l_conjugate(
                 kernel_eps_alpha_s, rho, q_eps_alpha_s
             )
         else:
             basis_change_matrix = None
             operator_l_matrix = self._compute_matrix_l(kernel_eps_alpha_s, rho)
```

### Comparing `datafold-1.1.6/datafold/pcfold/pointcloud.py` & `datafold-2.0.0/datafold/pcfold/pointcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 #!/usr/bin/env python
 
 import copy
-from typing import Optional, Tuple, Union
+from typing import Optional, Union
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy.sparse
 
 from datafold.pcfold import GaussianKernel, PCManifoldKernel
-from datafold.pcfold.distance import (
-    compute_distance_matrix,
-    get_backend_distance_algorithm,
-)
+from datafold.pcfold.distance import compute_distance_matrix
 from datafold.pcfold.estimators import estimate_cutoff, estimate_scale
 
 
 class PCManifold(np.ndarray):
     """Represent a point cloud lying near a manifold with a kernel.
 
     ``PCManifold`` is derived from NumPy's ``ndarray``. It attaches a kernel that is
@@ -36,15 +32,14 @@
     dist_kwargs
         Keyword arguments passed to the internal distance matrix computation. See
         :py:meth:`datafold.pcfold.distance.compute_distance_matrix` for parameter
         arguments.
 
     See Also
     --------
-
     :class:`numpy.ndarray`
     :class:`numpy.array`
     """
 
     def __new__(
         cls,
         data: Union[np.ndarray, pd.DataFrame],
@@ -80,15 +75,15 @@
             raise ValueError("Point cloud must be finite (no 'nan' or 'inf' values).")
 
         if dist_kwargs is not None and not isinstance(dist_kwargs, dict):
             raise TypeError("Parameter 'dist_kwargs' must be of type 'dict'.")
 
         # Set the kernel according to user input
         obj.kernel = kernel
-        obj.dist_kwargs = dist_kwargs or {}
+        obj.distance = dist_kwargs or {}
 
         return obj
 
     def __array_finalize__(self, obj):
         # Gets called for all three ways of object creation
         # 1) explicit construction (PCManifold(...)) --> obj is None
         # 2) view casting -->  obj can be an instance of any subclass of ndarray,
@@ -123,25 +118,24 @@
         attributes_line = " | ".join(
             [
                 f"kernel={self.kernel}",
                 f"dist_kwargs={str(self.dist_kwargs)}",
             ]
         )
 
-        repr = "\n".join([attributes_line, super(PCManifold, self).__repr__()])
-        return repr
+        return "\n".join([attributes_line, super().__repr__()])
 
     def __reduce__(self):
         # __reduce__ and __setstate__ are required for pickling (required if a model
         # such as DiffusionMaps that holds a PCManifold object is pickled)
         # The solution is from Mike McKerns' answer:
         # https://stackoverflow.com/a/26599346
 
         # Get the parent's __reduce__ tuple
-        pickled_state = super(PCManifold, self).__reduce__()
+        pickled_state = super().__reduce__()
 
         # Create own tuple to pass to __setstate__ (see below)
         new_state = pickled_state[2] + (
             self.kernel,
             self.dist_kwargs,
         )  # -2  # -1
 
@@ -150,15 +144,15 @@
 
     def __setstate__(self, state, *args, **kwargs):
         # Set own attributes attached to every np.ndarray
         self.kernel = state[-2]
         self.dist_kwargs = state[-1]
 
         # Call the parent's __setstate__ with the other tuple elements.
-        super(PCManifold, self).__setstate__(state[0:-2])
+        super().__setstate__(state[0:-2])
 
     @property
     def cut_off(self) -> float:
         """Larger distance values are not set in a distance matrix computation. The
         corresponding kernel value is then treated as zero.
 
         The cut-off value is part of the dist_kwargs.
@@ -231,30 +225,29 @@
         Union[np.ndarray, scipy.sparse.csr_matrix]
             kernel matrix of shape `(n_samples_Y, n_samples_self)`
 
         Optional
             A kernel can return further values see :meth:`PCManifoldKernel.__call__`
             for details.
         """
-        return self.kernel(X=self, Y=Y, dist_kwargs=self.dist_kwargs, **kernel_kwargs)
+        return self.kernel(X=self, Y=Y, **kernel_kwargs)
 
     def optimize_parameters(
         self,
         n_subsample: int = 1000,
         tol: float = 1e-8,
         k: int = 25,
         random_state: Optional[int] = None,
         result_scaling: float = 1.0,
         inplace: bool = True,
-    ) -> Tuple[float, float]:
+    ) -> tuple[float, float]:
         """Estimates ``cut_off`` and kernel bandwidth ``epsilon`` for a Gaussian kernel.
 
         Parameters
         ----------
-
         n_subsample
             Number of samples to use for cut-off estimation.
 
         tol
             Tolerance below which the Gaussian kernel is assumed to be zero.
 
         k
@@ -274,15 +267,14 @@
         Returns
         -------
         float
             cut-off
         float
             epsilon
         """
-
         if not isinstance(self.kernel, GaussianKernel):
             raise TypeError("kernel must be of type GaussianKernel")
 
         if not hasattr(self.kernel, "epsilon"):
             # fails if kernel has no epsilon parameter
             raise AttributeError(
                 f"Kernel {type(self.kernel)} has no epsilon parameter to optimize."
@@ -310,15 +302,14 @@
     min_distance: Optional[float] = None,
     min_added_per_iteration=1,
 ):
     """Subsample a manifold point cloud with a uniform sample density.
 
     Parameters
     ----------
-
     pcm
         Point cloud to subsample.
 
     n_samples
         Block size for iteration.
 
     min_distance
@@ -336,26 +327,27 @@
     numpy.ndarray
         subsampled indices of the original dataset
 
     See Also
     --------
     :py:meth:`datafold.utils.math.random_subsample`
     """
-
     if min_distance is None and pcm.cut_off is not None:
         min_distance = pcm.cut_off * 2
 
     if min_distance is None:
         raise ValueError(
             "'cut_off' cannot be None. Either provide in 'min_distance' or 'pcm.cut_off'."
         )
 
     n_samples_pcm = pcm.shape[0]
 
-    all_indices = np.random.permutation(n_samples_pcm)
+    rng = np.random.default_rng(1)
+    all_indices = rng.permutation(n_samples_pcm)
+
     indices_splits = np.array_split(all_indices, n_samples_pcm // n_samples + 1)
 
     # choose first block of random samples as a basis
     subsample_indices = indices_splits[0]
     subsample_points = pcm[subsample_indices, :]
 
     # block-wise iteration of other blocks
@@ -397,26 +389,24 @@
 
 def pcm_remove_outlier(pcm: PCManifold, kmin: int, cut_off: float):
     """Remove all points that have not a minimum number of neighbors insinde the
     distance range.
 
     Parameters
     ----------
-
     pcm
         Point cloud.
 
     kmin
         The minimum number of a point to be not treated as an outlier.
 
     cut_off
         The distance range (Euclidean) in which to count the neighbours for
         each point.
     """
-
     if kmin <= 0 or not isinstance(kmin, int):
         raise ValueError("kmin must be a positive integer")
 
     distance_matrix = compute_distance_matrix(
         pcm, metric="sqeuclidean", cut_off=cut_off, backend="guess_optimal"
     )
```

### Comparing `datafold-1.1.6/datafold/pcfold/timeseries/accessor.py` & `datafold-2.0.0/datafold/pcfold/timeseries/accessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 #!/usr/bin/env python3
 
 import warnings
-from typing import Generator, Optional, Tuple, Union
+from collections.abc import Generator
+from typing import Optional, Union
 
 import findiff.diff
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.testing as nptest
 import pandas as pd
 import pandas.testing as pdtest
 from scipy.stats import multivariate_normal
 
 from datafold.pcfold.timeseries.collection import TSCDataFrame, TSCException
-from datafold.utils.general import is_integer
+from datafold.utils.general import is_df_same_index, is_integer
 
 
 @pd.api.extensions.register_dataframe_accessor("tsc")
-class TSCAccessor(object):
+class TSCAccessor:
     """Extension functions for TSCDataFrame.
 
-    See `documentation <https://pandas.pydata.org/pandas-docs/stable/development/extending.html?highlight=accessor>`_
-    for regular pandas accessors.
+    See `documentation <https://pandas.pydata.org/pandas-docs/stable/development/
+    extending.html?highlight=accessor>`__ for regular pandas accessors.
 
     The functions are available through the accessor `tsc`, for example,
 
     .. code::
 
             tsc_object.tsc.normalize_time()
 
     Parameters
     ----------
-
     tsc_df
         time series collection data to carry out accessor functions on
     """
 
     def __init__(self, tsc_df: TSCDataFrame):
-
         # NOTE: cannot call TSCDataFrame(tsc_df) here to transform in case it is a normal
         # DataFrame. This is because the accessor has to know when updating this object.
         if not isinstance(tsc_df, TSCDataFrame):
             raise TypeError(
                 "The 'tsc' extension only works for type TSCDataFrame (convert before)."
             )
 
         self._tsc_df = tsc_df
 
     def check_tsc(
         self,
         *,
         ensure_all_finite: bool = True,
-        ensure_min_samples: Optional[int] = None,
+        ensure_min_samples: int = 1,
+        ensure_min_features: int = 1,
         ensure_same_length: bool = False,
         ensure_const_delta_time: bool = True,
         ensure_delta_time: Optional[float] = None,
         ensure_same_time_values: bool = False,
         ensure_normalized_time: bool = False,
         ensure_n_timeseries: Optional[int] = None,
         ensure_min_timesteps: Optional[int] = None,
         ensure_n_timesteps: Optional[int] = None,
         ensure_no_degenerate_ts: bool = True,
+        ensure_dtype_time=None,
     ) -> TSCDataFrame:
         """Validate time series properties.
 
         This summarises the single check functions also contained in `TSCAccessor`.
 
         Parameters
         ----------
@@ -99,27 +100,27 @@
             If provided, check if every time series has the required minimum of time
             steps.
 
         ensure_no_degenerate_ts
             If True, make sure that no degenerate (single sampled) time series are
             present.
 
+        ensure_dtype_time
+            Check the data type of the time index.
+
         Returns
         -------
         TSCDataFrame
             validated time series collection (without changes)
         """
-
-        # TODO: allow handle_fail="raise | warn | return"?
-
         if ensure_all_finite:
             self.check_finite()
 
-        if ensure_min_samples is not None:
-            self.check_min_samples(min_samples=ensure_min_samples)
+        self.check_min_samples(min_samples=ensure_min_samples)
+        self.check_min_features(min_features=ensure_min_features)
 
         if ensure_same_length:
             self.check_timeseries_same_length()
 
         if ensure_const_delta_time:
             self.check_const_time_delta()
 
@@ -140,51 +141,83 @@
 
         if ensure_min_timesteps is not None:
             self.check_required_min_timesteps(ensure_min_timesteps)
 
         if ensure_no_degenerate_ts:
             self.check_no_degenerate_ts()
 
+        if ensure_dtype_time is not None:
+            self.check_dtype_time(ensure_dtype_time)
+
         return self._tsc_df
 
     def check_finite(self) -> None:
         """Check if all values are finite (i.e. does not contain `nan` or `inf`)."""
         if not self._tsc_df.is_finite():
             raise TSCException.not_finite()
 
     def check_min_samples(self, min_samples) -> None:
-        """Check if there is a minimum number of samples included."""
+        """Check if there is a minimum number of samples included in the collection."""
         if self._tsc_df.shape[0] < min_samples:
             raise TSCException.not_min_samples(min_samples=min_samples)
 
+    def check_min_features(self, min_features) -> None:
+        """Check if there is a minimum number of features included in the collection."""
+        if self._tsc_df.shape[1] < min_features:
+            raise TSCException.not_min_features(min_features=min_features)
+
     def check_timeseries_same_length(self) -> None:
         """Check if time series in the collection have the same length."""
         if not self._tsc_df.is_equal_length():
             raise TSCException.not_same_length(
                 actual_lengths=self._tsc_df.is_equal_length()
             )
 
     def check_const_time_delta(self) -> Union[pd.Series, float]:
         """Check if all time series have the same time-delta."""
         delta_time = self._tsc_df.delta_time
-        if not self._tsc_df.is_const_delta_time():
-            raise TSCException.not_const_delta_time(self._tsc_df.delta_time)
+        if not self._tsc_df.is_const_delta_time(delta_time):
+            raise TSCException.not_const_delta_time(delta_time)
         return delta_time
 
+    def check_const_timesteps(self) -> int:
+        """Check that all time series have the same number of timesteps. The time values itself
+        can differ between the time series.
+        """
+        n_timesteps = self._tsc_df.n_timesteps
+        if isinstance(n_timesteps, pd.Series):
+            raise TSCException.not_const_timesteps()
+        else:
+            return n_timesteps
+
     def check_equal_timevalues(self) -> None:
-        """Check if all time series in the collection share the same time values."""
+        """Check if all time series in the collection have identical time values."""
         if not self._tsc_df.is_same_time_values():
             raise TSCException.not_same_time_values()
 
+    def check_contain_required_ids(self, required_ids, check_order=False):
+        """Check that the time series collection contains exactly the required IDs."""
+        required_ids = np.asarray(required_ids)
+
+        if check_order:
+            X_ids = self._tsc_df.initial_states(1).index.get_level_values(
+                TSCDataFrame.tsc_id_idx_name
+            )
+        else:
+            required_ids = np.sort(required_ids)
+            X_ids = np.asarray(self._tsc_df.ids)  # already sorted
+
+        if X_ids.shape != required_ids.shape or (X_ids != required_ids).any():
+            raise TSCException.not_match_required_ids(required_ids)
+
     def check_normalized_time(self) -> None:
         """Check if time series collection has normalized time.
 
         See Also
         --------
-
         :py:meth:`TSCAccessor.normalize_time`
 
         """
         if not self._tsc_df.is_normalized_time():
             raise TSCException.not_normalized_time()
 
     def check_required_time_delta(
@@ -193,15 +226,14 @@
         """Check if time series collection has required time-delta.
 
         Parameters
         ----------
         required_time_delta
             single value or per time series
         """
-
         try:
             delta_times = np.asarray(self._tsc_df.delta_time)
 
             if self._tsc_df.is_datetime_index():
                 if (delta_times != required_time_delta).any():
                     raise AttributeError
             else:
@@ -259,14 +291,19 @@
                 actual_n_timesteps=_n_timesteps,
             )
 
     def check_no_degenerate_ts(self):
         if self._tsc_df.has_degenerate():
             raise TSCException.has_degenerate_ts()
 
+    def check_dtype_time(self, dtype):
+        _is = self._tsc_df.index.get_level_values(TSCDataFrame.tsc_time_idx_name).dtype
+        if _is != dtype:
+            raise TSCException.has_wrong_time_dtype(got=_is, expected=dtype)
+
     def check_non_overlapping_timeseries(self) -> None:
         """Check if all time series have disjoint time values (do not overlap).
 
         Returns
         -------
 
         """
@@ -276,15 +313,15 @@
         )
         if (counts > 1).any():
             raise TSCException("time series are required to be non-overlapping")
 
     @classmethod
     def check_equal_delta_time(
         cls, X: TSCDataFrame, Y: TSCDataFrame, atol=1e-15, require_const=False
-    ) -> Tuple[Union[float, pd.Series], Union[float, pd.Series]]:
+    ) -> tuple[Union[float, pd.Series], Union[float, pd.Series]]:
         """Check if two time series collections have the same delta times.
 
         Parameters
         ----------
         X
             First time series collection.
         Y
@@ -340,57 +377,51 @@
             First delta time.
 
         dt2
             Second delta time.
 
         atol
             Acceptable absolute tolerance between the two delta times. This is
-            relevant for floating delta times that have "numerical noise" when
-            equally spaced.
+            relevant for delta times with floating point arithmetic which can introduce
+            "numerical noise" (breaking the exact equidistant spacing).
 
         Returns
         -------
         bool
         """
         return np.abs(dt1 - dt2) <= atol
 
     def iter_timevalue_window(
         self,
         window_size: int,
         offset: int,
         per_time_series: bool = False,
-        strictly_sequential: bool = True,
     ) -> Generator[TSCDataFrame, None, None]:
-        """Iterator over time series intervals (window).
+        """Iterator over time series windows.
 
         Parameters
         ----------
         window_size
             The number of samples for each window. Note that the `blocksize` is not
             guaranteed and is usually shorter in last iterations if the number of samples
             are not a multiple of `blocksize`.
 
         offset
             A positive integer value that indicates by how much the next window should be
             shifted. If ``offset=blocksize``, then the windows are non-overlapping.
 
         per_time_series
-            If True, the windows are generated for each time series separately. This is
-            recommended for time series a collection consists where the time series are
-            disjoint (i.e. non-overlapping time intervals).
-
-        strictly_sequential
-            TODO
+            Treat every time series separately when iterating. This is recommended if the time
+            series in a collection have disjoint time values.
 
         Returns
         -------
         Generator[TSCDataFrame]
             An iterator for the windowed time series data.
         """
-
         self.check_const_time_delta()
 
         if not is_integer(window_size):
             raise TypeError(
                 f"The parameter 'window_size={window_size}' must be of type integer. "
                 f"Got {type(window_size)}"
             )
@@ -403,76 +434,212 @@
 
         if window_size <= 0:
             raise ValueError(
                 f"The parameter 'window_size={window_size}' must be positive."
                 f"Got {type(window_size)}"
             )
 
-        if offset <= 0:
+        if not is_integer(offset) or offset <= 0:
             raise ValueError(
-                f"The parameter 'offset={offset}' must be positive."
-                f"Got {type(window_size)}"
+                f"The parameter '{offset=}' must be a positive integer."
+                f"Got {type(offset)=}"
             )
 
         if per_time_series:
             _iter_timeseries_collection = self._tsc_df.groupby(
                 by=self._tsc_df.tsc_id_idx_name
             )
         else:
             # This mimics a single element of the "groupby" function -- the first element
-            # is the time series id, but not required here and therefore None
+            # is the time series ID (but not required here and therefore set to None)
             _iter_timeseries_collection = [(None, self._tsc_df)]
 
         for _, current_tsc in _iter_timeseries_collection:
             time_values = current_tsc.time_values()
             start = 0
             end = start + window_size
 
             while end <= time_values.shape[0]:
                 selected_time_values = time_values[start:end]
 
                 start = start + offset
                 end = start + window_size
 
-                _ret = current_tsc.select_time_values(selected_time_values)
+                yield current_tsc.select_time_values(selected_time_values)
 
-                if strictly_sequential and isinstance(_ret.n_timesteps, pd.Series):
-                    pass
-                else:
-                    yield _ret
-
-    def shift_time(self, shift_t: float):
+    def shift_time_by_delta(self, shift_t: float):
         """Shift all time values from the time series by a constant value.
 
         Parameters
         ----------
         shift_t
             positive or negative time shift value
 
         Returns
         -------
         TSCDataFrame
             same shape as input
         """
-
-        if shift_t == 0:
+        if shift_t == 0:  # no shift
             return self._tsc_df
 
-        convert_times = self._tsc_df.index.get_level_values(1) + shift_t
+        convert_times = (
+            self._tsc_df.index.get_level_values(TSCDataFrame.tsc_time_idx_name)
+            + shift_t
+        )
         convert_times = pd.Index(convert_times, name=TSCDataFrame.tsc_time_idx_name)
 
         new_tsc_index = pd.MultiIndex.from_arrays(
-            [self._tsc_df.index.get_level_values(0), convert_times]
+            [
+                self._tsc_df.index.get_level_values(TSCDataFrame.tsc_id_idx_name),
+                convert_times,
+            ]
         )
 
         self._tsc_df.index = new_tsc_index
-        self._tsc_df._validate()
-
         return self._tsc_df
 
+    # def shift_time_by_index(self, idx):
+    #     """Shift the time index for samples.
+    #
+    #     For example, if idx=1 then the second row gets the first index, the third the second
+    #     and so on. The first index is dropped.
+    #
+    #
+    #     Parameters
+    #     ----------
+    #     idx
+    #         Positive or negative integer value by how much to shift the time index.
+    #
+    #     Returns
+    #     -------
+    #     TSCDataFrame
+    #         data with shifted time index
+    #     """
+    #
+    #     new_index = self._tsc_df.groupby(TSCDataFrame.tsc_id_idx_name)
+    #        .tail(self._tsc_df.n_timesteps - idx).index
+    #     return self._tsc_df.set_index(new_index)
+
+    def expand_time_values(self, time_values, fill_value=0.0):
+        # implementation required to remove this restriction
+        if self._tsc_df.n_timeseries == 1:
+            pad_data = np.ones([len(time_values), self._tsc_df.n_features]) * fill_value
+            pad_data = TSCDataFrame.from_array(
+                pad_data,
+                time_values=time_values,
+                feature_names=self._tsc_df.columns,
+                ts_id=self._tsc_df.ids[0],
+            )
+            return pd.concat([self._tsc_df, pad_data], axis=0)
+        else:
+            self.check_equal_timevalues()
+
+            tensor_data = self._tsc_df.to_numpy().reshape(
+                [
+                    self._tsc_df.n_timeseries,
+                    self._tsc_df.n_timesteps,
+                    self._tsc_df.n_features,
+                ]
+            )
+            new_time_values = np.append(self._tsc_df.time_values(), time_values)
+            tensor_data = np.pad(
+                tensor_data,
+                ((0, 0), (0, len(time_values)), (0, 0)),
+                mode="constant",
+                constant_values=fill_value,
+            )
+            return TSCDataFrame.from_tensor(
+                tensor=tensor_data,
+                time_series_ids=self._tsc_df.ids,
+                time_values=new_time_values,
+                feature_names=self._tsc_df.columns,
+            )
+
+    def shift_time_per_time_series(
+        self,
+        shift_values: Optional[pd.Series] = None,
+        ensure_identical_values=False,
+        return_shift_values=False,
+    ):
+        """
+        Shift each time series by a value given in shift_values. If ``shift_values is None``
+        then each time series is normalized to zero. This may be beneficial when dealing with
+        time series data from autonomous systems.
+
+        Parameters
+        ----------
+        shift_values:
+            If provided, then the series must contain the shift value for each time series.
+            If ``None`` then the shift values are computed such that each time series has an
+            initial time value of zero.
+
+        ensure_identical_values
+            A flag that performs an extra routine that counteracts numerical noise after the
+            time values are shifted. Note that this is only possible if the time series
+            collection is equally spaced (otherwise the parameter is ignored).
+
+        reutrn_shift_values:
+            If True the applied shift_values are returned. This is useful if the parameter
+            ``shift_values is None``.
+
+        Returns
+        -------
+        TSCDataFrame, pd.Series
+           shifted time series collection and shift_values (optional)
+
+        """
+        n_timesteps = self._tsc_df.n_timesteps
+        if isinstance(n_timesteps, pd.Series):
+            n_timesteps = n_timesteps.to_numpy()
+
+        if shift_values is None:
+            shift_values = self._tsc_df.initial_states(1).index
+            shift_values = pd.Series(
+                # -1 to normalize it to zero
+                -1 * shift_values.get_level_values(TSCDataFrame.tsc_time_idx_name),
+                shift_values.get_level_values(TSCDataFrame.tsc_id_idx_name),
+            )
+        else:
+            if not isinstance(shift_values, pd.Series):
+                raise TypeError(
+                    f"shift_values must be of type pd.Series. Got {type(shift_values)=}"
+                )
+
+            if not (shift_values.index == self._tsc_df.ids).all():
+                raise ValueError(
+                    "The ids in shift_values must match the ones in TSCDataFrame."
+                )
+
+        if np.any(shift_values != 0):
+            time_shift_expanded = np.repeat(shift_values.to_numpy(), n_timesteps)
+
+            normalized_time_values = (
+                self._tsc_df.index.get_level_values("time") + time_shift_expanded
+            )
+            new_index = pd.MultiIndex.from_arrays(
+                [self._tsc_df.index.get_level_values("ID"), normalized_time_values]
+            )
+
+            if ensure_identical_values:
+                dt = self._tsc_df.delta_time
+                corrected_values = (
+                    np.round(new_index.get_level_values("time") / dt) * dt
+                )
+                new_index = pd.MultiIndex.from_arrays(
+                    [new_index.get_level_values("ID"), corrected_values]
+                )
+
+            self._tsc_df.index = new_index
+
+        if return_shift_values:
+            return self._tsc_df, shift_values
+        else:
+            return self._tsc_df
+
     def normalize_time(self):
         """Normalize time in time series collection.
 
         A :py:class:`TSCDataFrame` with normalized time has the following properties:
 
         * the global time starts at zero
         * delta_time is constant one
@@ -485,15 +652,14 @@
             normalized data with same shape as input
 
         Raises
         ------
         TSCException
             If time delta between all time series is not constant.
         """
-
         convert_times = self._tsc_df.index.get_level_values(
             TSCDataFrame.tsc_time_idx_name
         )
         min_time, _ = self._tsc_df.time_interval()
         delta_time = self._tsc_df.delta_time
 
         if not self._tsc_df.is_const_delta_time():
@@ -516,14 +682,29 @@
         self._tsc_df.index = new_tsc_index
         self._tsc_df._validate()
 
         assert self._tsc_df.is_normalized_time()
 
         return self._tsc_df
 
+    def drop_last_n_samples(self, n_samples: int):
+        """Drop last `n` samples per time series in the collection.
+
+        n_samples
+            Number of samples to drop.
+
+        Returns
+        -------
+        TSCDataFrame
+            reduced time series collection
+        """
+        self.check_required_min_timesteps(n_samples)
+        drop_idx = self._tsc_df.groupby(by="ID").tail(n_samples).index
+        return self._tsc_df.drop(drop_idx)
+
     def time_derivative(
         self,
         scheme="center",
         diff_order: int = 1,
         accuracy: int = 2,
         shift_index: bool = False,
     ) -> Union[pd.DataFrame, TSCDataFrame]:
@@ -555,15 +736,15 @@
         Returns
         -------
         Union[pd.DataFrame, TSCDataFrame]
             The finite difference time series. The boundary samples are removed,
             i.e. the number of samples decrease accordingly.
         """
 
-        class InternalDiff(findiff.diff.Diff):
+        class _InternalDiff(findiff.diff.Diff):
             """Overwrites the behaviour of the findiff superclass."""
 
             def diff(
                 self,
                 data: Union[np.ndarray, pd.DataFrame],
                 spacing: float,
                 accuracy: int,
@@ -594,15 +775,15 @@
 
                 self._apply_to_array(
                     data_dt, data_numpy, weights, off_slices, ref_slice, self.axis
                 )
 
                 data_dt = data_dt[start_sample:end_sample, :]
 
-                h_inv = 1.0 / spacing ** self.order
+                h_inv = 1.0 / spacing**self.order
                 data_dt *= h_inv
 
                 if scheme in ["center", "forward"] and shift_index:
                     # NOTE: Only the first samples of the time values are dropped. This
                     # means that the time is shifted to the finite difference offset that
                     # lies furthest in the future.
                     lost_samples = data.shape[0] - data_dt.shape[0]
@@ -621,17 +802,17 @@
 
         self.check_const_time_delta()
         spacing = self._tsc_df.delta_time
 
         min_samples = np.inf
         time_derivative = list()
 
-        dt_func = InternalDiff(axis=0, order=diff_order)
+        dt_func = _InternalDiff(axis=0, order=diff_order)
 
-        for ts_id, time_series in self._tsc_df.itertimeseries():
+        for _, time_series in self._tsc_df.itertimeseries():
             time_series_dt = dt_func.diff(
                 data=time_series,
                 spacing=spacing,
                 accuracy=accuracy,
             )
             min_samples = min(min_samples, time_series_dt.shape[0])
 
@@ -648,15 +829,14 @@
         Note, that this operation is inplace and overwrites the existing time series IDs.
 
         Returns
         -------
         TSCDataFrame
             The data with time series IDs in sequential order.
         """
-
         self._tsc_df.index = self._tsc_df.index.remove_unused_levels()
         # levels[0] = IDs, levels[1] = time
         n_timeseries = len(self._tsc_df.index.levels[0])
 
         self._tsc_df.index = self._tsc_df.index.set_levels(
             np.arange(n_timeseries), level=0
         )
@@ -680,16 +860,16 @@
         train_indices
             The indices to indicate which samples are included in the training set.
 
         test_indices
             The indices to indicate which samples are included in the test set.
 
         return_dropped
-            If True, a DataFrame is returned in the third return value which includes
-            all samples that were neigher included in the training indices nor the test
+            If True, a DataFrame is returned to the third return value which includes
+            all samples that were neither included in the training indices nor the test
             indices.
 
         Returns
         -------
         TSCDataFrame
             The time series collection for training.
 
@@ -700,15 +880,15 @@
             The dropped samples; only returned if ``return_dropped_samples=True``.
         """
 
         def _test_array(_array):
             bool_dim = _array.ndim == 1
             bool_positive = np.all(_array >= 0)
             bool_sorted = np.all(_array[:-1] < _array[1:])
-            bool_type = _array.dtype == int
+            bool_type = np.issubdtype(_array.dtype, np.integer)
 
             if not (bool_dim and bool_positive and bool_sorted and bool_type):
                 raise ValueError(
                     "The arrays 'train_indices' and 'test_indices' must be sorted 1-dim. "
                     "array of non-negative and unique integer values."
                 )
 
@@ -739,29 +919,30 @@
         ).astype(bool)
 
         # iii) detect switch of dropped indices
         mask_dropped = np.ones(self._tsc_df.shape[0], dtype=bool)
         mask_dropped[train_indices] = False
         mask_dropped[test_indices] = False
 
-        # cumulative sum of on or the other change and reassign IDs
+        # cumulative sum of one or the other change and reassign IDs
         id_cum_sum_mask = np.logical_or(
             np.logical_or(change_fold_indicator, change_id_indicator),
             mask_dropped,
         )
         new_ids = np.cumsum(id_cum_sum_mask)
 
         reassigned_ids_idx = pd.MultiIndex.from_arrays(
             arrays=(
                 new_ids,
                 self._tsc_df.index.get_level_values(TSCDataFrame.tsc_time_idx_name),
             )
         )
 
         # See also gitlab issue #105 (if addressed, can use TSCDataFrame)
+        # TODO: #105 is possible now, can adapt.
         splitted_df = pd.DataFrame(
             data=self._tsc_df.to_numpy(),
             index=reassigned_ids_idx,
             columns=self._tsc_df.columns,
         )
 
         train_tsc = splitted_df.iloc[train_indices, :]
@@ -909,21 +1090,20 @@
 
                 return local_tsc_df.set_index(reassigned_ids_idx)
 
         result_dfs = list()
 
         min_id = 0
         for _id, timeseries_df in self._tsc_df.groupby(by=TSCDataFrame.tsc_id_idx_name):
-
             if pd.isnull(timeseries_df.delta_time):
                 new_df = split_irregular_time_series(timeseries_df, min_id=min_id)
             else:
                 # reset time series ID
                 new_df = timeseries_df
-                new_df.index = new_df.index.set_levels([min_id], 0)
+                new_df.index = new_df.index.set_levels([min_id], level=0)
 
             if new_df is not None:
                 min_id = max(new_df.ids) + 1
                 result_dfs.append(new_df)
             else:
                 if not drop_samples:
                     raise RuntimeError(
@@ -934,38 +1114,94 @@
             self._tsc_df = pd.concat(result_dfs, axis=0)
             self._tsc_df = self._tsc_df.tsc.assign_ids_sequential()
 
             if np.isnan(np.asarray(self._tsc_df.delta_time)).any():
                 warnings.warn(
                     "The function 'assign_ids_const_delta' was unsuccessful "
                     "to remove all irregular time series. Please "
-                    "consider to report case."
+                    "consider to report case.",
+                    stacklevel=2,
                 )
 
             return self._tsc_df
         else:
             return None
 
+    def fill_timeseries_with_last_state(self, n_timesteps):
+        """Fills the time series with less than `n_timesteps` to a length with `n_timesteps`
+        by filling the last available state.
+        """
+        if self._tsc_df.n_timeseries != 1:
+            raise NotImplementedError(
+                "Currently this function is only implemented for a single time series"
+            )
+
+        if self._tsc_df.n_timesteps >= n_timesteps:
+            df = self._tsc_df
+            raise TSCException(
+                f"The time series must contain less timesteps ({df.n_timesteps=}) than "
+                f"the required {n_timesteps=}"
+            )
+
+        dt = self.check_const_time_delta()
+
+        # number of states to attach:
+        n_attach = n_timesteps - self._tsc_df.shape[0]
+
+        last_state = self._tsc_df.iloc[[-1], :].to_numpy()
+        first_time = self._tsc_df.time_values()[-1] + dt
+
+        attach_states = np.tile(last_state, (n_attach, 1))
+        attach_time = np.arange(first_time, first_time + n_attach * dt - 1e-15, dt)
+        tsc_attach = TSCDataFrame.from_array(
+            attach_states, time_values=attach_time, feature_names=self._tsc_df.columns
+        )
+        return pd.concat([self._tsc_df, tsc_attach], axis=0)
+
+    def augment_control_input(self, U: TSCDataFrame):
+        # TODO: validation
+        # X and U need to have same structure
+        #   n_elements per time series
+        #   same ID axis
+
+        X_ids = self._tsc_df.index.get_level_values(TSCDataFrame.tsc_id_idx_name)
+        mask_all_except_first = np.logical_not(
+            np.diff(X_ids, prepend=True).astype(bool)
+        )
+        mask_all_except_last = np.append(
+            np.logical_not((X_ids[:-1] - X_ids[1:]).astype(bool)), False
+        )
+
+        is_df_same_index(self._tsc_df.loc[mask_all_except_last], U, check_column=False)
+
+        U = U.copy(deep=True)  # append new data without changing the old
+        # make that time values are identical
+        U.index = self._tsc_df.loc[mask_all_except_first].index
+        return pd.concat([self._tsc_df, U], axis=1)
+
     def shift_matrices(
-        self, snapshot_orientation: str = "col"
-    ) -> Tuple[np.ndarray, np.ndarray]:
+        self, snapshot_orientation: str = "col", validate: bool = True
+    ) -> tuple[np.ndarray, np.ndarray]:
         """Computes shift matrices from time series data.
 
-        Both shift matrices have same shape with `(n_features, n_snapshots-1)` or
+        Both shift matrices have the same shape with `(n_features, n_snapshots-1)` or
         `(n_snapshots-1, n_features)`, depending on `snapshot_orientation`.
 
         Parameters
         ----------
         snapshot_orientation
             Orientation of snapshots (system states at time) either in rows ("row") or
             column-wise ("col")
 
+        validate
+            If True, validation steps (constant sampling and that each time series has at
+            least two samples) are performed.
+
         Returns
         -------
-
         :class:`numpy.ndarray`
             shift matrix for time steps `(0,1,2,...,N-1)`
 
         :class:`numpy.ndarray`
             shift matrix for time steps `(1,2,...,N)`
 
         Raises
@@ -974,69 +1210,61 @@
             If time series collection has no constant time delta.
 
         See Also
         --------
         :py:class:`DMDFull`
 
         """
+        if validate:
+            self.check_required_min_timesteps(required_min_timesteps=2)
+            self.check_const_time_delta()
 
-        self.check_const_time_delta()
-
-        # can be implemented if required:
-        self.check_required_min_timesteps(required_min_timesteps=2)
-
-        ts_counts = self._tsc_df.n_timesteps
-
-        if is_integer(ts_counts):
-            ts_counts = pd.Series(
-                np.ones(self._tsc_df.n_timeseries, dtype=int) * ts_counts,
-                index=self._tsc_df.ids,
-            )
-
-        assert isinstance(ts_counts, pd.Series)  # for mypy
-
-        n_shift_snapshots = (ts_counts.subtract(1)).sum()
-        insert_indices = np.append(0, (ts_counts.subtract(1)).cumsum().to_numpy())
+        # Note that the copy() operations are important here to avoid that the data within the
+        # shift matrices do not point to the original memory (not having the copies led to
+        # incorrect results in other tests
+        if self._tsc_df.n_timeseries == 1:
+            # fast return for a single time series
+            values = self._tsc_df.to_numpy()
+            left, right = values[:-1].copy(), values[1:].copy()
+        else:
+            ts_counts = self._tsc_df.n_timesteps
+            values = self._tsc_df.to_numpy()
+            if isinstance(ts_counts, int):
+                # single snapshot pairs case
+                # this improves computational performance for streaming settings
+                if ts_counts == 2:
+                    left, right = values[0::2, :].copy(), values[1::2, :].copy()
+                else:
+                    idx = np.arange(values.shape[0])
+                    idx_del_left = idx[ts_counts - 1 :: ts_counts]
+                    left = np.delete(values.copy(), idx_del_left, axis=0)
+
+                    idx_del_right = idx[::ts_counts]
+                    right = np.delete(values.copy(), idx_del_right, axis=0)
+
+            elif isinstance(ts_counts, pd.Series):
+                idx = np.append(0, ts_counts.to_numpy()).cumsum()
+                idx_del_left = (idx - 1)[1:]
+                idx_del_right = idx[:-1]
 
-        assert len(insert_indices) == self._tsc_df.n_timeseries + 1
+                left = np.delete(values.copy(), idx_del_left, axis=0)
+                right = np.delete(values.copy(), idx_del_right, axis=0)
+            else:
+                raise TypeError(
+                    f"{type(ts_counts)} is not understood -- please report bug"
+                )
 
         if snapshot_orientation == "col":
-            shift_left = np.zeros([self._tsc_df.n_features, n_shift_snapshots])
+            return left.T, right.T
         elif snapshot_orientation == "row":
-            shift_left = np.zeros([n_shift_snapshots, self._tsc_df.n_features])
+            return left, right
         else:
-            raise ValueError(f"snapshot_orientation={snapshot_orientation} not known")
-
-        shift_right = np.zeros_like(shift_left)
-
-        # NOTE: if this has performance issues or memory issues, then it may be beneficial
-        # to do the whole thing with boolean indexing
-
-        # TODO: maybe three is a better readable code using pandas' functionatlity?
-        #  e.g. shift https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.shift.html
-        #  could also be more efficient than cmp to itertimeseries()
-        for i, (id_, ts_df) in enumerate(self._tsc_df.itertimeseries()):
-            if snapshot_orientation == "col":
-                # start from 0 and exclude last snapshot
-                shift_left[:, insert_indices[i] : insert_indices[i + 1]] = ts_df.iloc[
-                    :-1, :
-                ].T
-                # exclude 0 and go to last snapshot
-                shift_right[:, insert_indices[i] : insert_indices[i + 1]] = ts_df.iloc[
-                    1:, :
-                ].T
-            else:  # "row"
-                shift_left[insert_indices[i] : insert_indices[i + 1], :] = ts_df.iloc[
-                    :-1, :
-                ]
-                shift_right[insert_indices[i] : insert_indices[i + 1], :] = ts_df.iloc[
-                    1:, :
-                ]
-
-        return shift_left, shift_right
+            raise ValueError(
+                f"{snapshot_orientation=} not known (choose either 'row' or 'col')"
+            )
 
     def time_values_overview(self) -> pd.DataFrame:
         """Generate table with overview of time values.
 
         Example of how the table looks:
         .. Comment: generated with https://truben.no/table/
 
@@ -1051,15 +1279,14 @@
         +----------------+------------+----------+----+
 
         Returns
         -------
         pandas.DataFrame
             overview
         """
-
         table = pd.DataFrame(
             [self._tsc_df.time_interval(_id) for _id in self._tsc_df.ids],
             index=self._tsc_df.ids,
             columns=["start", "end"],
         )
 
         table["delta_time"] = self._tsc_df.delta_time
@@ -1097,15 +1324,14 @@
             covariance of Gaussian bells
 
         Returns
         -------
         matplotlib object
             axis handle
         """
-
         if len(self._tsc_df.columns) != 2:
             raise ValueError("Density can only be plotted for 2D time series.")
 
         if covariance is None:
             covariance = np.eye(2)
 
         df = self._tsc_df.select_time_values(time_values=time)
@@ -1151,16 +1377,15 @@
         ax1.set_yticklabels(
             [round(ymin, float_precision), round(ymax, float_precision)]
         )
 
         return heatmap_plot
 
     def _generate_2d_meshgrid(self, xdim, ydim):
-        """
-        Both parameters must be a tuple consisting of three values (min, max, resolution
+        """Both parameters must be a tuple consisting of three values (min, max, resolution
         Return a n x 2 vector representing the grid.
         """
         x = np.linspace(*xdim)
         y = np.linspace(*ydim)
 
         xx, yy = np.meshgrid(x, y)
         grid = np.c_[xx.ravel(), yy.ravel()]
```

### Comparing `datafold-1.1.6/datafold/pcfold/timeseries/collection.py` & `datafold-2.0.0/datafold/pcfold/timeseries/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,106 @@
+from collections.abc import Generator
+from functools import partial
 from numbers import Number
-from typing import Generator, List, Optional, Tuple, Union
+from typing import Optional, Union
 
 import matplotlib.colors as mclrs
 import numpy as np
 import pandas as pd
-import scipy.sparse
-from pandas.api.types import is_datetime64_dtype, is_numeric_dtype
+from pandas.api.types import is_datetime64_dtype, is_numeric_dtype, is_timedelta64_dtype
 from pandas.core.indexing import _iLocIndexer, _LocIndexer
 
-from datafold.pcfold.distance import compute_distance_matrix
 from datafold.utils.general import (
     df_type_and_indices_from,
+    if1dim_colvec,
     is_df_same_index,
     is_integer,
 )
 
-ColumnType = Union[pd.Index, List[str]]
+ColumnType = Union[pd.Index, list[str], np.ndarray]
 NumericalTimeType = Union[int, float, np.datetime64]
 
 
 class TSCException(Exception):
     """Error raised if TSC is not correct."""
 
     def __init__(self, message):
-        super(TSCException, self).__init__(message)
+        super().__init__(message)
 
     @classmethod
     def not_finite(cls):
-        return cls(f"Numeric values are not finite (nan or inf values present).")
+        return cls("Numeric values are not finite (nan or inf values present).")
 
     @classmethod
     def not_min_samples(cls, min_samples):
         return cls(f"A minimum number of {min_samples} samples is required.")
 
     @classmethod
+    def not_min_features(cls, min_features):
+        return cls(f"A minimum number of {min_features} features is required.")
+
+    @classmethod
     def not_same_length(cls, actual_lengths):
         return cls(f"Time series have not the same length. Got {actual_lengths}")
 
     @classmethod
     def not_required_n_timesteps(cls, required_length, actual_length):
         return cls(
             "One or more time series do not meet the minimum number of required time "
             f"samples. Required {required_length} time values but got \n{actual_length}."
         )
 
     @classmethod
-    def not_const_delta_time(cls, actual_delta_time=None):
-        msg = (
-            "The time sampling ('delta_time') is not constant. \n"
-            "Note: If the time values are numerical floating points and were generated "
-            "with numpy.linspace, then this can introduce numerical noise breaking "
-            "the equal spacing."
-        )
-
+    def not_const_delta_time(cls, actual_delta_time=None, add_float_note=False):
         if actual_delta_time is not None:
-            msg += f"\n {actual_delta_time}"
+            msg_dt = f"delta_time={actual_delta_time}"
+        else:
+            msg_dt = "delta_time"
+
+        if add_float_note:
+            msg_note = (
+                "\nNote: If the time values are numerical floating points and were "
+                "generated with numpy.linspace, then this can introduce numerical "
+                "noise breaking the equal spacing."
+            )
+        else:
+            msg_note = ""
 
+        msg = f"The time sampling is not constant ({msg_dt}).{msg_note}"
         return cls(msg)
 
     @classmethod
-    def not_required_delta_time(cls, required_delta_time, actual_delta_time):
+    def not_const_timesteps(cls, actual_timesteps=None):
+        a = ""
+        if actual_timesteps is not None:
+            a = f"Got\n{actual_timesteps}"
+
+        msg = (
+            f"It is required that all time series have the same number of timesteps.{a}"
+        )
+        return cls(msg)
+
+    @classmethod
+    def not_match_required_ids(cls, required_ids):
         return cls(
-            f"The required delta_time (={required_delta_time}) does not match the "
-            f"actual delta time {actual_delta_time}."
+            "The time series collection does not contain all required time "
+            f"series IDs  {required_ids=}."
         )
 
     @classmethod
+    def not_required_delta_time(cls, required_delta_time, actual_delta_time):
+        return cls(f"{required_delta_time=} does not match the {actual_delta_time=}.")
+
+    @classmethod
     def not_same_time_values(cls):
-        return cls("The time series have not the same time values.")
+        return cls("The time series in the collection have not the same time values.")
 
     @classmethod
     def not_normalized_time(cls):
-        return cls("The time values are not normalized.")
+        return cls("The time values in the time series are not normalized.")
 
     @classmethod
     def not_required_n_timeseries(cls, required_n_timeseries, actual_n_timeseries):
         return cls(
             f"There are {actual_n_timeseries} time series present. "
             f"Required: {required_n_timeseries}"
         )
@@ -86,102 +111,97 @@
             f"The minimum number of required timesteps (={required_n_timesteps}) is not "
             f"met. Got: \n{actual_n_timesteps}"
         )
 
     @classmethod
     def not_n_timesteps(cls, required: int):
         return cls(
-            f"Invalid format: The time series collection has the requirement of"
-            f" {required} samples per time series."
+            f"Invalid TSCDataFrame format. Each time series in the collection must have "
+            f"exactly {required} {'samples' if required > 1 else 'sample'}."
         )
 
     @classmethod
     def has_degenerate_ts(cls):
         return cls(
             "One or more time series are degenerated (i.e. have only a single sample)."
         )
 
     @classmethod
-    def no_kernel(cls):
-        return cls("No kernel is set.")
+    def has_wrong_time_dtype(cls, got, expected):
+        return cls(f"The time index has a wrong dtype={got}. Expected dtype={expected}")
 
 
 def _is_numeric_dtype(obj):
     if isinstance(obj, Number):
         # this includes np.nan and np.inf
         return True
-    elif isinstance(obj, pd.Series) or isinstance(obj, np.ndarray):
+    elif isinstance(obj, (np.ndarray, pd.Series)):
         # call is_numeric_dtype from pandas
         return is_numeric_dtype(obj)
     elif isinstance(obj, pd.DataFrame):
         return np.all([is_numeric_dtype(ty) for ty in obj.dtypes])
     else:
         return False
 
 
 class _LocTSCIndexer(_LocIndexer):
-    """Required for overwriting the behavior of :meth:`TSCDataFrame.loc`.
-    `iloc` is currently not supported, see #61"""
+    """Required for overwriting the behavior of :meth:`TSCDataFrame.loc`."""
 
     def __getitem__(self, item):
-        sliced = super(_LocTSCIndexer, self).__getitem__(item)
+        sliced = super().__getitem__(item)
         _type = type(sliced)
 
         try:
             # there is no "TSCSeries", so always use TSCDataFrame, even when
             # sliced has only 1 column and is a pd.Series.
             if isinstance(sliced, pd.Series):
-                # raises attribute error if not possible
+                # raises attribute error if this does not work
                 sliced = TSCDataFrame(sliced)
-            else:
-                sliced._validate()
 
         except AttributeError:
             # Fallback if the sliced is not a valid TSC anymore
             # returns to pd.Series or pd.DataFrame (depending on what the
             # sliced object of a standard pd.DataFrame is).
             if _type == TSCDataFrame:
                 sliced = pd.DataFrame(sliced)
 
         return sliced
 
     def __setitem__(self, key, value):
         if not _is_numeric_dtype(value):
             raise AttributeError("Data in TSCDataFrame must be numeric.")
-        return super(_LocTSCIndexer, self).__setitem__(key, value)
+        return super().__setitem__(key, value)
 
 
 class _iLocTSCIndexer(_iLocIndexer):
     def __getitem__(self, item):
         sliced = super(_iLocIndexer, self).__getitem__(item)
         _type = type(sliced)
 
         try:
             # NOTE: this is different to loc -- here a pd.Series remains a pd.Series!
-            # This is because pandas internal testing requires this
+            # This is because pandas' internal testing routines require this
             if isinstance(sliced, pd.Series):
                 # TODO: see issue #61
                 #  https://gitlab.com/datafold-dev/datafold/-/issues/61
                 raise AttributeError
-            else:
-                sliced._validate()
 
         except AttributeError:
             # Fallback if the sliced is not a valid TSC anymore
             # returns to pd.Series or pd.DataFrame (depending on what the
             # sliced object of a standard pd.DataFrame is).
             if _type == TSCDataFrame:
                 sliced = pd.DataFrame(sliced)
 
         return sliced
 
     def __setitem__(self, key, value):
         if not _is_numeric_dtype(value):
             raise AttributeError("Data in TSCDataFrame must be numeric.")
-        return super(_iLocTSCIndexer, self).__setitem__(key, value)
+        return super().__setitem__(key, value)
 
 
 class TSCDataFrame(pd.DataFrame):
     """Data frame to store time series collections.
 
     The class inherits from pandas' data structure :class:`pandas.DataFrame` and provides
     additional functionality to manipulate and analyze a time series collection. The
@@ -189,15 +209,16 @@
 
     * The row index must be a multi index of two levels, where the first indicates
       the time series ID (integer), and the second contains the time values of the time
       series (non-negative and finite numerical values)
     * The column must be a one-dimensional column index that contains the feature
       names (accounting to the spatial axis)
     * There are no duplicates in both row and column index allowed (the flag
-      `allows_duplicate_labels <https://pandas.pydata.org/docs/reference/api/pandas.Flags.allows_duplicate_labels.html>`__
+      `allows_duplicate_labels
+      <https://pandas.pydata.org/docs/reference/api/pandas.Flags.allows_duplicate_labels.html>`__
       is set to True). Note, that this disables inplace operations on the labels (e.g.
       :code:`tsc.set_index(new_index, inplace=True` raises an error).
     * All time series values must be of a numeric dtype (`nan` or `inf` are allowed).
 
     A single time series typically consists of two or more samples with unequal
     time values. However, it is also possible to store "degenerated time series",
     which only contain a single sample. In some situations this is useful, such as when
@@ -218,15 +239,14 @@
         Currently, there is no corresponding ``TSCSeries``, which results in
         inconsistencies in `iloc` indexing. For example, ``tsc.iloc[:, 0]`` returns a
         ``pandas.Series`` instead of a ``TSCDataFrame``. It is encouraged to use slices
         that return a data frame, i.e. ``tsc.iloc[:, [0]]``.
 
     Examples
     --------
-
     An example ``TSCDataFrame`` with three time series and two features (columns). The
     first two time series share the same time values (rows). The third time series
     contains only a single sample (degenerated time series).
 
     +-------------+---------------+-----------+-----------+
     | feature     |               | sin       | cos       |
     +=============+===============+===========+===========+
@@ -282,82 +302,100 @@
         arguments.
     """
 
     tsc_id_idx_name = "ID"
     tsc_time_idx_name = "time"
     tsc_feature_col_name = "feature"
 
-    def __init__(self, *args, **kwargs):
-
-        # remove specific attributes from kwargs first into local attributes
-        kernel = kwargs.pop("kernel", None)
-        dist_kwargs = kwargs.pop("dist_kwargs", dict())
+    def __init__(self, *args, fixed_delta=None, validate=True, **kwargs):
+        # TODO: potential
+        # TODO: write an index extension?
+        # TODO: include fixed_delta in constructors?
+        # TODO: adapt delta_time
+        # TODO: test that delta_time only accepts float and setting integer time values
+        # TODO: test that there can be diverse
 
         # NOTE: do not move this call after other setters "self.attribute = ...".
         # Otherwise, there is an infinite recursion because pandas handles the
         # __getattr__ magic function.
-        super(TSCDataFrame, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-        self.kernel = kernel
+        self.flags.allows_duplicate_labels = False
 
-        dist_kwargs.setdefault("cut_off", np.inf)
-        dist_kwargs.setdefault("kmin", 0)
-        dist_kwargs.setdefault("backend", "guess_optimal")
-        self.attrs["dist_kwargs"] = dist_kwargs
+        if not hasattr(self, "is_validate"):
+            self.is_validate = validate
 
-        try:
-            # In validate an AttributeError is raised, follow-up changes to the data
-            # are dealt with the flag (introduced in pandas v. 1.2.0)
-            self.flags.allows_duplicate_labels = False
-            self._validate()
-        except AttributeError as e:
-            # This is a special case of input, where the fallback is a cast to
-            # pd.DataFrame.
-            # Internally of pandas the __init__ is called like this:
-            # df._constructor(res)
-            # --> df._constructor is TSCDataFrame
-            # --> res is a BlockManager (pandas internal type)
-            # If a BlockManager slices the index, then no AttributeError is raised,
-            # but instead self casted to DataFrame
-            # (case was necessary with changes introduced in pandas==1.2.0)
-            _is_blockmanager_input = len(args) > 0 and isinstance(
-                args[0], pd.core.internals.managers.BlockManager
-            )
-
-            if _is_blockmanager_input and self.index.nlevels != 2:
-                # TODO: this seems dangerous... maybe there are better ways to deal
-                #  with this?
-                self = pd.DataFrame(self)
+        if not hasattr(self, "fixed_delta"):
+            if fixed_delta is None or (
+                isinstance(fixed_delta, float) and fixed_delta > 0
+            ):
+                self.fixed_delta = fixed_delta
             else:
-                raise e
+                raise TypeError(
+                    "Parameter 'fixed_delta' must be None or positive float. "
+                    f"Got: {type(fixed_delta)=} and {fixed_delta=}"
+                )
+
+        # This is a special case of input with fallback to cast to pd.DataFrame:
+        # In pandas the __init__ is called like this:
+        # df._constructor(res)
+        # --> df._constructor is TSCDataFrame
+        # --> res is a BlockManager (pandas internal type)
+        # If a BlockManager slices the index, then no AttributeError is raised,
+        # but is instead cast to DataFrame
+        # (case was necessary with changes introduced in pandas==1.2.0)
+        _is_blockmanager_input = len(args) > 0 and isinstance(
+            args[0], pd.core.internals.managers.BlockManager
+        )
+
+        if _is_blockmanager_input and self.index.nlevels != 2:
+            # TODO: this seems dangerous... maybe there are better ways to deal
+            #  with this?
+            self = pd.DataFrame(self)
+        else:
+            if self.is_validate:
+                self._validate()
 
     def __setattr__(self, key, value):
-        if key == "index":
+        if key == "index" and self.is_validate:
             value = self._validate_index(value)
-        elif key == "columns":
+        elif key == "columns" and self.is_validate:
             value = self._validate_columns(value)
 
         # Note: validation of data is not necessary here because this is done
         # in _LocTSCIndexer and _iLocTSCIndexer
-        return super(TSCDataFrame, self).__setattr__(key, value)
+        return super().__setattr__(key, value)
+
+    def __repr__(self, with_fixed_delta=True):
+        if not with_fixed_delta and self.fixed_delta is not None:
+            _time = TSCDataFrame.tsc_time_idx_name
+            _adapt_time_values = self.index.get_level_values(_time) * self.fixed_delta
+            _repr_index = self.index.set_levels(
+                _adapt_time_values, level=_time, verify_integrity=False
+            )
+            return pd.DataFrame(
+                self.to_numpy(), index=_repr_index, columns=self.columns
+            ).__repr__()
+        else:
+            return super().__repr__()
 
     @classmethod
     def from_tensor(
         cls,
         tensor: np.ndarray,
-        time_series_ids: Optional[np.ndarray] = None,
-        columns: Optional[Union[pd.Index, list]] = None,
+        time_series_ids: Optional[Union[np.ndarray, pd.Index]] = None,
+        feature_names: Optional[Union[pd.Index, list]] = None,
         time_values: Optional[np.ndarray] = None,
     ) -> "TSCDataFrame":
-        """Create a ``TSCDataFrame`` from a three dimensional tensor.
+        """Create a ``TSCDataFrame`` from a three-dimensional tensor.
 
         Parameters
         ----------
         tensor
-            The time series data of shape `(n_timeseries, n_timesteps, n_feature,)`.
+            The time series data of shape `(n_timeseries, n_timesteps, n_feature)`.
 
         time_series_ids
             The IDs of shape `(n_timeseries,)` to assign for the respective time
             series. Defaults to `(0,1,2,..., n_timeseries-1)`.
 
         columns
             The feature names of shape `(n_feature,)`. Defaults to
@@ -368,15 +406,14 @@
             `(0,1,2, ..., n_timesteps-1)`.
 
         Returns
         -------
         TSCDataFrame
             new instance
         """
-
         if tensor.ndim != 3:
             raise ValueError(
                 "Input tensor has to be of dimension 3. Index (1) denotes the time "
                 "series, (2) time and (3) the quantity of interest. "
                 f"Got tensor.ndim={tensor.ndim}"
             )
 
@@ -398,66 +435,75 @@
                     f"n_timeseries={n_timeseries}."
                 )
             if len(np.unique(time_series_ids)) != len(time_series_ids):
                 raise ValueError("time_series_ids must be unique")
 
             time_series_ids = time_series_ids.repeat(n_timesteps)
 
-        if columns is None:
-            columns = pd.Index(
+        if feature_names is None:
+            feature_names = pd.Index(
                 [f"feature{i}" for i in range(n_feature)],
                 name=TSCDataFrame.tsc_feature_col_name,
             )
 
         if time_values is None:
             time_values = np.arange(n_timesteps)
+        elif len(time_values) != tensor.shape[1]:
+            raise ValueError(
+                f"{len(time_values)=} does not match the time series length "
+                f"in {tensor.shape[1]=}"
+            )
 
         # entire column, repeating for every time series
         col_time_values = np.resize(time_values, n_timeseries * n_timesteps)
         idx = pd.MultiIndex.from_arrays([time_series_ids, col_time_values])
 
         data = tensor.reshape(n_timeseries * n_timesteps, n_feature)
 
         # Sorting index here, handles cases where time values are not sorted in the input.
-        data = pd.DataFrame(data=data, index=idx, columns=columns)
-        data.sort_index(axis=0, level=0, inplace=True)
+        data = pd.DataFrame(data=data, index=idx, columns=feature_names)
+        data = data.sort_index(axis=0, level=0)
         return cls(data)
 
     @classmethod
     def from_shift_matrices(
         cls,
         left_matrix,
         right_matrix,
+        *,
+        time_values=(0, 1),
         snapshot_orientation: str = "col",
         columns: Optional[Union[pd.Index, list]] = None,
     ) -> "TSCDataFrame":
         """Create ``TSCDataFrame`` from shift matrices.
 
         Parameters
         ----------
         left_matrix
             Time series values at time "now".
 
         right_matrix
             Time series values at time "next".
 
+        time_values
+            Two time values to highlight the time step size.
+
         snapshot_orientation
             Indicate whether the snapshots (states) are in rows ("row") or columns
             ("col").
 
         columns
             Feature names of shape `(n_feature,)`. Defaults to
             `feature[0,1,2,..., n_feature-1]`.
 
         Returns
         -------
         TSCDataFrame
             new instance
         """
-
         snapshot_orientation = snapshot_orientation.lower()
 
         if snapshot_orientation == "col":
             left_matrix, right_matrix = left_matrix.T, right_matrix.T
         elif snapshot_orientation == "row":
             pass
         else:
@@ -465,33 +511,31 @@
                 f"snapshot_orientation={snapshot_orientation} not known. "
                 f"Choose either 'row' or 'col'"
             )
 
         if left_matrix.shape != right_matrix.shape:
             raise ValueError(
                 "The matrix shapes are not the same. "
-                f"left_matrix.shape={left_matrix.shape}"
-                f"right_matrix.shape={right_matrix.shape}"
+                f"{left_matrix.shape=} "
+                f"{right_matrix.shape=}."
             )
 
         n_timeseries, n_features = left_matrix.shape
 
         # allocate memory
         zipped_values = np.zeros([n_timeseries * 2, n_features])
         # copy for safety
         zipped_values[0::2, :] = left_matrix.copy()
         zipped_values[1::2, :] = right_matrix.copy()
 
         id_idx = np.repeat(np.arange(n_timeseries), 2)
-        time_values = np.array([0, 1] * n_timeseries)
+        time_values = np.array([time_values[0], time_values[1]] * n_timeseries)
         index = pd.MultiIndex.from_arrays([id_idx, time_values])
 
-        tsc = cls(data=zipped_values, index=index, columns=columns)
-        tsc._validate()
-        return tsc
+        return cls(data=zipped_values, index=index, columns=columns)
 
     @classmethod
     def from_same_indices_as(
         cls,
         indices_from: "TSCDataFrame",
         values: Union[np.ndarray, pd.DataFrame, "TSCDataFrame"],
         except_index: Optional[ColumnType] = None,
@@ -517,15 +561,14 @@
             set together with `except_index`.
 
         Returns
         -------
         TSCDataFrame
             new instance
         """
-
         if not isinstance(indices_from, TSCDataFrame):
             raise TypeError("Parameter 'indices_from' must be of type 'TSCDataFrame'")
 
         return df_type_and_indices_from(
             indices_from=indices_from,
             values=values,
             except_index=except_index,
@@ -550,41 +593,73 @@
             ID of initial time series.
 
         Returns
         -------
         TSCDataFrame
             new instance
         """
+        df = df.copy()  # to not change original data
 
         if isinstance(df, TSCDataFrame) or df.index.nlevels > 1:
             # Handling of TSCDataFrame can be implemented if required.
-            raise TypeError("The row index must only contain time values.")
+            raise TypeError(
+                "The row index must be one-dimensional and only contain time values."
+            )
 
         if ts_id is None:
             ts_id = 0
 
         if isinstance(df, pd.Series):
             if df.name is None:
                 df.name = cls.tsc_feature_col_name
             df = pd.DataFrame(df)
 
         # The time values must be sorted.
-        df.sort_index(axis=0, inplace=True)
+        df = df.sort_index(axis=0)
 
         df[cls.tsc_id_idx_name] = ts_id
-        df.set_index(cls.tsc_id_idx_name, append=True, inplace=True)
+        df = df.set_index(cls.tsc_id_idx_name, append=True)
         df = df.reorder_levels([cls.tsc_id_idx_name, df.index.names[0]])
 
         return cls(df)
 
     @classmethod
+    def from_array(cls, array, time_values=None, feature_names=None, ts_id=None):
+        """Create ``TSCDataFrame`` from an array (describing a single time series).
+
+        Parameters
+        ----------
+        array
+            Time series data (2-dim. array) with snapshots in rows.
+
+        time_values
+            Time values to apply. Must have :code:`data.shape[0]` elements.
+            Defaults to `0, 1, 2, ...`.
+
+        ts_id
+            An integer of for The ID of a single time series (if timesteps is None). Or the
+
+        Returns
+        -------
+        TSCDataFrame
+            new instance
+        """
+        if time_values is not None:
+            time_values = np.atleast_1d(time_values)
+
+        df = pd.DataFrame(
+            np.atleast_2d(array), index=time_values, columns=feature_names
+        )
+        return cls.from_single_timeseries(df, ts_id=ts_id)
+
+    @classmethod
     def from_frame_list(
         cls,
-        frame_list: List[pd.DataFrame],
-        ts_ids: Optional[Union[np.ndarray, pd.Index, List[int]]] = None,
+        frame_list: list[pd.DataFrame],
+        ts_ids: Optional[Union[np.ndarray, pd.Index, list[int]]] = None,
     ) -> "TSCDataFrame":
         """Create ``TSCDataFrame`` from a list of time series.
 
         Parameters
         ----------
         frame_list
             Data frames with :code:`index=time_values` and :code:`columns=feature_names`.
@@ -616,15 +691,15 @@
                 check_index=False,
                 check_column=True,
                 check_names=False,
                 handle="raise",
             )
 
         # prepare list
-        final_list: List[pd.DataFrame] = []
+        final_list: list[pd.DataFrame] = []
 
         for df in frame_list:
             # >= 2 to raise error for invalid DataFrames
             if df.index.nlevels >= 2 and not isinstance(df, TSCDataFrame):
                 try:
                     df = TSCDataFrame(df)
                 except AttributeError:
@@ -632,15 +707,17 @@
                         f"Cannot process entry check that the format is correct. \n {df}"
                     )
 
             if isinstance(df, TSCDataFrame):
                 if len(df.ids) > 1:
                     df = [e[1] for e in list(df.itertimeseries())]
                 else:
-                    df = pd.DataFrame(df)
+                    # copy in case there are multiple df with the same reference in the list
+                    # see test "test_from_frame_list04"
+                    df = pd.DataFrame(df).copy()
                     df.index = df.index.get_level_values(TSCDataFrame.tsc_time_idx_name)
 
             if isinstance(df, list):
                 final_list += df
             else:
                 final_list.append(df)
 
@@ -659,152 +736,93 @@
             raise ValueError(
                 "Parameter 'ts_ids' must contain unique time series IDs with same "
                 "length than 'frame_list'"
             )
 
         tsc_list = list()
         for _id, df in zip(ts_ids, final_list):
-            # TODO: can be done without loop and would be more efficient
+            # TODO: could be done without loop and would be more efficient
+            df = df.copy(
+                deep=True
+            )  # there can be dfs in the list that are actually the same
             df.index = pd.MultiIndex.from_product([[_id], df.index.to_numpy()])
             tsc_list.append(TSCDataFrame(df))
 
         return cls(pd.concat(tsc_list, axis=0))
 
-    @staticmethod
-    def unique_delta_times(
-        delta_times: Union[np.ndarray, pd.Series], rtol=1e-11, atol=1e-15
-    ) -> np.ndarray:
-        """Returns unique (within tolerances) delta time values.
-
-        The tolerances are required for floating point time values. For example,
-
-        .. code::
-
-            np.unique(np.diff(np.linspace(0,2, 4)))
-
-        prints :code:`array([0.6666666666666666, 0.6666666666666667])`.
-
-        The default tolerance values are adjusted in test_linspace_unique_delta_times so
-        that a wide range of time_values generated with ``np.linspace`` are considered
-        equally spaced (despite the numerical noise that breaks the equality).
-
-        Parameters
-        ----------
-        delta_times
-            Array of delta times between samples of a time series.
-
-        rtol
-            Relative tolerance of the largest versus the smallest delta time.
-
-        atol
-            Absolute tolerance between the delta times to be considered unique.
-
-        Returns
-        -------
-        numpy.ndarray
-            Unique (in tolerance levels) delta times.
-        """
-
-        unique_delta_times = np.unique(np.asarray(delta_times))
-
-        if unique_delta_times.dtype == float and len(unique_delta_times) > 1:
-            # Note: unique_delta_times is already sorted by np.unique
-            max_step = np.diff(unique_delta_times)
-            rel_step = max_step / unique_delta_times[1:]
-
-            # print(f"max_step={max_step} | rel_step={rel_step}")
-
-            abs_groups = max_step <= atol
-            rel_groups = rel_step <= rtol
-
-            groups = np.logical_not(np.logical_or(abs_groups, rel_groups)).cumsum()
-            groups = np.append(0, groups)
-
-            n_groups = groups[-1] + 1  # +1 because 0 is also a group
-            _unique_dt = np.zeros(n_groups)
-
-            for group in range(n_groups):
-                _unique_dt[group] = np.mean(unique_delta_times[groups == group])
-
-            unique_delta_times = _unique_dt
-
-        return unique_delta_times
-
     def to_csv(self, *args, **kwargs) -> Optional[str]:
         """Write object to a comma-separated values (csv) file.
 
         Internaly, the method casts the object (self) to pd.Dataframe before the csv is
         written. The reason is that for larger files it could be observed that the
         internals of ``to_csv`` could lead to invalid TSCDataFrame objects (which
         raise an error).
 
         Parameters
         ----------
         **kwargs
             All keyword arguments are passed to the super class. See
-            `docu <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html>`__
+            `docu <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html>`__.
 
         Returns
         -------
         None or str
             If path is None, returns the resulting csv format as a
             string. Otherwise returns None.
 
         """
-
         return pd.DataFrame(self).to_csv(*args, **kwargs)
 
     @classmethod
     def from_csv(cls, filepath, **kwargs) -> "TSCDataFrame":
         """Initialize time series collection from csv file.
 
         Parameters
         ----------
         filepath
             The file path to the csv file.
 
         **kwargs
             keyword arguments handled to
-            `pandas.read_csv <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`_
+            `pandas.read_csv <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`__
 
         Returns
         -------
         TSCDataFrame
             new instance
         """
         # NOTE: Overwrites the super class method (which is deprecated since version 0.21
         # Here the csv is read from a csv file that was a
         # TSCDataFrame, i.e. tscdf.to_csv("filename.csv") and therefore should be valid.
         df = pd.read_csv(filepath, index_col=[0, 1], header=[0], **kwargs)
         return cls(df)
 
     @property
     def _constructor(self):
-        return TSCDataFrame
+        return partial(TSCDataFrame, validate=self.is_validate)
 
     @property
     def _constructor_expanddim(self):
-        raise NotImplementedError("expanddim is not supported for TSCDataFrame")
+        raise NotImplementedError("The dimension of TSCDataFrame cannot be expanded")
 
     def _validate_index(self, index: Union[pd.MultiIndex, pd.Index]) -> pd.MultiIndex:
-
         if not isinstance(index, pd.MultiIndex):
             raise AttributeError("index must be of type pd.MultiIndex")
 
         if index.nlevels != 2:
             # must exactly have two levels [ID, time]
             raise AttributeError(
-                "Index has to be a 'MultiIndex' with two levels (index.nlevels == 2). "
+                "Index has to be a 'MultiIndex' with two levels (index.nlevels = 2). "
                 "First level for the time series ID, "
-                f"second level for the time values. Got: {index.nlevels}"
+                f"second level for the time values. Got: {index.nlevels=}"
             )
 
         if index.duplicated().any():
             raise AttributeError(
-                f"Duplicated indices found: " f"{index[index.duplicated()].to_numpy()}"
+                f"Duplicated indices found: {index[index.duplicated()].to_numpy()}"
             )
 
         # Insert required index names:
         #  -- Note: this overwrites potential previous names.
         index.names = [self.tsc_id_idx_name, self.tsc_time_idx_name]
 
         ids_index = index.get_level_values(self.tsc_id_idx_name)
@@ -816,93 +834,113 @@
             if (ids_index.astype(int) == ids_index).all():
                 index = index.set_levels(
                     index.levels[0].astype(int),
                     level=self.tsc_id_idx_name,
                 )
             else:
                 raise AttributeError(
-                    "Time series IDs must be of type integer. "
-                    f"Got dtype={ids_index.dtype}"
+                    f"Time series IDs must be integers. Got dtype={ids_index.dtype}"
                 )
 
         if (ids_index < 0).any():
-            unique_negative_ids = np.unique(ids_index < 0)
+            unique_negative_ids = np.unique(ids_index[ids_index < 0])
             raise AttributeError(
-                f"All time series IDs have to be non-negative integer values. "
-                f"Got invalid time series IDs: {unique_negative_ids}"
+                f"All time series IDs have to be non-negative unique integers. "
+                f"Got invalid negative time series IDs: {unique_negative_ids}"
             )
 
-        if time_index.dtype.kind in "bcmOSUV":
+        if self.fixed_delta is not None:
+            _allowed_dtypes = "iu"
+        else:
+            _allowed_dtypes = "iufM"
+
+        if time_index.dtype.kind not in _allowed_dtypes:
             # See further info for 'kind'-codes:
             # https://docs.scipy.org/doc/numpy/reference/generated/numpy.dtype.kind.html
             raise AttributeError(
                 f"Time values have to be numeric and real-valued. "
-                f"Got dtype={time_index.dtype}"
+                f"Got {time_index.dtype=} with {time_index.dtype.kind=}"
             )
         else:
             assert (
                 time_index.dtype.kind in "uifM"
-            ), f"Numpy dtype.kind={time_index.dtype.kind} not handled, please report bug."
+            ), f"Numpy dtype.kind={time_index.dtype.kind} not allowed in TSCDataFrame."
 
         # u - unsigned integer | i - signed integer | f - floating point
         # do not perform this check for:
         # M - datetime (bc. the second condition raises an error)
         if time_index.dtype.kind in "uif" and (time_index < 0).any():
             raise AttributeError(
                 "Time values have to be non-negative. "
-                f"Found invalid time values {(time_index[time_index < 0])}"
+                f"Found invalid time values {time_index[time_index < 0]}"
             )
 
         # bool index to the start of new IDs
         bool_new_id = np.append(1, np.diff(index.codes[0])).astype(bool)
         _ids = ids_index[bool_new_id]
 
         if len(np.unique(_ids)) != len(_ids):
-            raise AttributeError("Time series IDs appear multiple times.")
+            raise AttributeError("The time series must have a unique ID.")
 
-        ts_internal_codes = np.append(0, np.diff(index.codes[1]))
-        if np.any(ts_internal_codes[~bool_new_id] <= 0):
-            raise AttributeError("The time values of each time series must be sorted.")
+        if is_datetime64_dtype(time_index):
+            _time_index_num = time_index.view(np.int64)
+        else:
+            _time_index_num = time_index.view()
+
+        cond_not_sorted = np.logical_and(
+            ~np.diff(ids_index).astype(bool),
+            np.diff(_time_index_num) <= 0.0,
+        )
 
+        if np.any(cond_not_sorted):
+            raise AttributeError(
+                "The time values of each time series in the collection must be sorted."
+            )
         return index
 
     def _validate_columns(self, columns: pd.Index) -> pd.Index:
-
         if not isinstance(columns, pd.Index):
             raise AttributeError("columns must be of type pd.Index")
 
         if columns.nlevels != 1:
-            # must exactly have two levels [ID, time]
             raise AttributeError(
                 f"Columns must be single level (columns.nlevels == 1).  "
                 f"Got: columns.nlevels={columns.nlevels}"
             )
 
+        col_types = sorted(t.__qualname__ for t in {type(v) for v in columns})
+
+        if len(col_types) > 1:
+            raise AttributeError(
+                f"There are mixed types in the columns {col_types}. "
+                f"Use a consistent type over all column names."
+            )
+
         if columns.duplicated().any():
             raise AttributeError(
-                f"Duplicated columns found: "
+                f"Duplicated column names found: "
                 f"{columns[columns.duplicated()].to_numpy()}"
             )
 
         columns.name = self.tsc_feature_col_name
         return columns
 
     def _validate_data(self) -> None:
         if not _is_numeric_dtype(self):
-            raise AttributeError("All feature columns must have a numeric dtype")
+            raise AttributeError(f"All data types must be numeric. Got {self.dtypes=}")
 
     def _validate(self) -> bool:
+        if self.is_validate:
+            # just for security remove unused levels --
+            # disable validate to avoid infinite recursion
+            self.index: pd.Index = self._validate_index(self.index)
+            self.index = self.index.remove_unused_levels()
 
-        # just for security remove unused levels --
-        # disable validate to avoid infinite recursion
-        self.index: pd.Index = self._validate_index(self.index)
-        self.index = self.index.remove_unused_levels()
-
-        self.columns: pd.Index = self._validate_columns(self.columns)
-        self._validate_data()
+            self.columns: pd.Index = self._validate_columns(self.columns)
+            self._validate_data()
         return True
 
     @property
     def n_timeseries(self) -> int:
         """Number of time series in the collection."""
         return len(self.ids)
 
@@ -915,231 +953,259 @@
     def ids(self) -> pd.Index:
         """The time series IDs in the collection."""
         # update index by removing potentially unused levels
         self.index = self.index.remove_unused_levels()
         return self.index.levels[0]
 
     @property
-    def delta_time(self) -> Union[pd.Series, float]:
-        """Time sampling frequency.
+    def delta_time(self) -> Union[pd.Series, int, float, np.timedelta64]:
+        """Time deltas (i.e. sampling frequency) for each time series or the entire collection.
+
+        Unevenly spaced time series have a ``delta_time=nan``. If all time series in the
+        collection have the same time delta (including `nan`), then a single value is returned.
+
+        .. warning::
+
+            If the time values type are floating points, then there are typically
+            numerical discrepancies in time differences that can lead to unintended results
+            (i.e. wrongly considered as equal or unequal).
 
-        Collects for each time series the time delta. Irregular frequencies are marked
-        with `nan`. If all time series are consistent (i.e., all have same time delta,
-        including `nan`), then a single float is returned.
+            For example,
+
+            .. code::
+
+                np.unique(np.diff(np.linspace(0, 2, 4)))
+
+            prints :code:`array([0.6666666666666666, 0.6666666666666667])`. The discrepancies
+            can vary depending on the order and range of time values in a time series.
+            While there are carefully adjusted tolerances set in this function within which
+            time deltas are considered equal, it is always safer to use integers as time
+            values if time values are multiples of a fixed time delta.
 
         Returns
         -------
+        pd.Series, int, float, np.timedelata64
+            Scalar value of same type than the time values if `delta_time` is identical in all
+            time series, otherwise a pd.Series indicating the `delta_time` for each time
+            series.
         """
-
         _index_name_series = "delta_time"
 
         if self.is_datetime_index():
-            # TODO: are there ways to better deal with timedeltas?
-            #  E.g. could cast internally to float64
             # NaT = Not a Time (cmp. to NaN)
             dt_result_series = pd.Series(
                 np.timedelta64("NaT"), index=self.ids, name=_index_name_series
             )
             dt_result_series = dt_result_series.astype("timedelta64[ns]")
         else:
-            # initialize all with nan values (which essentially is np.floag64.
+            # initialize all with nan values (which essentially is np.float64.
             # return back to same dtype than time_values if all values are finite,
             # otherwise the type stays as float.
             dt_result_series = pd.Series(
                 np.nan, index=self.ids, name=_index_name_series
             )
 
         diff_times = np.diff(self.index.get_level_values(self.tsc_time_idx_name))
         id_indexer = self.index.get_level_values(self.tsc_id_idx_name)
 
-        for timeseries_id in self.ids:
-            _id_dt = diff_times[id_indexer.get_indexer_for([timeseries_id])[:-1]]
-            _id_unique_dt = self.unique_delta_times(_id_dt)
+        n_timesteps = self.n_timesteps
 
-            if len(_id_unique_dt) == 1:
-                dt_result_series[timeseries_id] = _id_unique_dt[0]
+        # tolerances at which to consider two delta time vales the same:
+        # this is actually a tricky task to find well-suited tolernaces. The
+        # rtol=5e-12
+        # atol=1e-16
+        # are tested in a wider range of time values however it still may failure for cases
+        # (even if time values are generated with np.linspace)
+        # TODO: this actually calls for a feature in TSCDataFrame to set a global time delta
+        #  and internally work with integers (which makes everything much easier here!)
+        rtol = 3e-12
+        atol = 1e-16
+
+        if isinstance(n_timesteps, int):
+            if n_timesteps == 1:
+                dt_result_series[:] = np.nan
+            else:
+                n_timeseries = self.n_timeseries
 
-        if not np.isnan(dt_result_series).all():
+                # faster evaluation if all time series have the same number of time steps
+                idx_mask = np.ones(n_timesteps, dtype=bool)
+                idx_mask[-1] = 0
+
+                # the :-1 is here because in the np.diff above,
+                # there is no diff value for the last
+                diff_times = diff_times[np.tile(idx_mask, n_timeseries)[:-1]]
+                diff_times = np.reshape(diff_times, (n_timeseries, n_timesteps - 1))
+
+                if diff_times.shape[1] == 1:
+                    # special case when n_timesteps==2
+                    dt_result_series[:] = diff_times.flatten()
+                else:
+                    # need to check if all values are the same
+                    if diff_times.dtype == float:
+                        result = np.min(diff_times, axis=1)[:, np.newaxis]
+                        abs_diff = np.abs(diff_times[:, 1:] - result)
+
+                        within_atol = np.all(abs_diff < atol, axis=1)
+                        within_rtol = np.all(
+                            np.divide(abs_diff, result, out=abs_diff) < rtol, axis=1
+                        )
+                        equal_dt = np.logical_or(within_atol, within_rtol)
+                        result[~equal_dt] = np.nan
+                    else:
+                        result = diff_times[:, [0]]
+                        equal_dt = np.all(diff_times[:, 1:] == result, axis=1)
+
+                        if not equal_dt.all():
+                            if not is_timedelta64_dtype(result):
+                                result = result.astype(float)
+                                result[~equal_dt] = np.nan
+                            else:
+                                result[~equal_dt] = np.timedelta64("NaT")
 
-            _unique_result_series = self.unique_delta_times(
-                dt_result_series, rtol=0, atol=1e-15
-            )
+                    dt_result_series[:] = result.flatten()
+        else:
+            for timeseries_id in self.ids:
+                # TODO: this can be potentially faster by using views on the diff_times
+                #  instead of using get indexer for
+                _id_dt = diff_times[id_indexer.get_indexer_for([timeseries_id])[:-1]]
 
-            n_different_dts = len(_unique_result_series)
+                if is_timedelta64_dtype(_id_dt) or _id_dt.dtype == int:
+                    _is_unique_dt = len(np.unique(np.asarray(_id_dt))) == 1
+                else:
+                    _is_unique_dt = np.allclose(
+                        np.min(_id_dt), _id_dt, atol=atol, rtol=rtol
+                    )
+
+                if _is_unique_dt:
+                    dt_result_series[timeseries_id] = _id_dt[0]
+
+        if not np.isnan(dt_result_series).all():
+            if is_timedelta64_dtype(dt_result_series) or dt_result_series.dtype == int:
+                is_global_unique = len(np.unique(dt_result_series))
+            else:
+                is_global_unique = np.allclose(
+                    np.min(dt_result_series), dt_result_series, atol=atol, rtol=rtol
+                )
 
             if not np.isnan(dt_result_series).any():
                 # TODO: here it may be interesting to check the new "Null" types of
                 #  pandas. They allow to also have nan by still keeping other dtypes
-                #  than float (--> only float has a nan representation in Numpy types)
+                #  than float (--> only float has a nan representation in Numpy dtypes)
                 dt_result_series = dt_result_series.astype(diff_times.dtype)
 
         else:
             # all nan (i.e. irregular sampling), treat as all "identical
             # irregular sampled"
-            n_different_dts = 1
+            is_global_unique = 1
 
-        if self.n_timeseries == 1 or n_different_dts == 1:
+        if self.n_timeseries == 1 or is_global_unique:
             single_value = dt_result_series.iloc[0]
 
             if isinstance(single_value, pd.Timedelta):
                 # Somehow single_value gets turned into pd.Timedelta when calling .iloc[0]
                 single_value = single_value.to_timedelta64()
+            elif dt_result_series.dtype.kind == "m" and pd.isna(single_value):
+                # Somehow single_value gets turned into pd.NaT when calling .iloc[0]
+                single_value = np.timedelta64("NaT")
 
-            return single_value
+            if self.fixed_delta is None:
+                return single_value
+            else:
+                return single_value * self.fixed_delta
         else:
-            # return series listing delta_time per time series
-            return dt_result_series
+            if self.fixed_delta is None:
+                # return series listing delta_time per time series
+                return dt_result_series
+            else:
+                return dt_result_series.astype(float) * self.fixed_delta
 
     @property
     def n_timesteps(self) -> Union[int, pd.Series]:
         """Number of time steps per time series.
 
         Collects for each time series the number of time steps. If all time series are
         consistent (all have same time steps), then a single float is returned.
 
         Returns
         -------
         """
-        n_time_elements = self.index.get_level_values(0).value_counts()
-        n_unique_elements = len(np.unique(n_time_elements))
+        vals, counts = np.unique(
+            self.index.get_level_values(self.tsc_id_idx_name), return_counts=True
+        )
 
-        if self.n_timeseries == 1 or n_unique_elements == 1:
-            return int(n_time_elements.iloc[0])
+        if self.n_timeseries == 1 or len(np.unique(counts)) == 1:
+            return int(counts[0])
         else:
-            n_time_elements.index.name = self.tsc_id_idx_name
-            # seems not to be sorted in the first place.
-            n_time_elements = n_time_elements.sort_index()
-            n_time_elements.name = "counts"
-            return n_time_elements
-
-    @property
-    def kernel(self):
-        """The kernel to describe the proximity between samples.
-
-        Returns
-        -------
-
-        :py:class:`.BaseManifoldKernel`
-        """
-        if "kernel" not in self.attrs:
-            self.attrs["kernel"] = None
-
-        return self.attrs["kernel"]
-
-    @kernel.setter
-    def kernel(self, kernel) -> None:
-        """Set a new kernel.
-
-        Parameters
-        ----------
-        kernel
-            The new kernel to be set.
-
-        Returns
-        -------
-
-        """
-
-        from datafold.pcfold.kernels import BaseManifoldKernel
-
-        if kernel is not None and not isinstance(kernel, BaseManifoldKernel):
-            raise TypeError(
-                f"Kernel must be a subclass of type BaseManifoldKernel. Got "
-                f"type {type(kernel)}."
-            )
-        self.attrs["kernel"] = kernel
-
-    @property
-    def dist_kwargs(self) -> dict:
-        """Keyword arguments passed to the internal distance matrix computation.
-
-        See :py:meth:`datafold.pcfold.compute_distance_matrix` for parameter arguments.
-
-        Returns
-        -------
-
-        """
-        if "dist_kwargs" not in self.attrs:
-            self.attrs["dist_kwargs"] = dict()
-
-        return self.attrs["dist_kwargs"]
-
-    @dist_kwargs.setter
-    def dist_kwargs(self, dist_kwargs: Optional[dict]) -> None:
-        """Set new keyword arguments for the distance matrix computation.
-
-        Parameters
-        ----------
-        dist_kwargs
-            The new arguments passed to the distance matrix backend. To set the default
-            keywords pass ``None``.
-
-        Returns
-        -------
-
-        """
-
-        if dist_kwargs is not None and not isinstance(dist_kwargs, dict):
-            raise TypeError(
-                f"Keyword arguments for distance computation must be a dictionary or "
-                f"None. Got type {type(dist_kwargs)}."
+            return pd.Series(
+                counts, index=pd.Index(vals, name=self.tsc_id_idx_name), name="counts"
             )
 
-        dist_kwargs = {} or dist_kwargs
-
-        assert dist_kwargs is not None  # for mypy
-
-        dist_kwargs.setdefault("cut_off", np.inf)
-        dist_kwargs.setdefault("kmin", 0)
-        dist_kwargs.setdefault("backend", "guess_optimal")
-
-        self.attrs["dist_kwargs"] = dist_kwargs
-
     @property
     def loc(self):
         """Label-based indexing.
 
         Please visit
-        `pd.DataFrame.loc <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.loc.html#pandas.DataFrame.loc>`_
-        for full documentation.
+        `pd.DataFrame.loc <https://pandas.pydata.org/pandas-docs/stable/reference/api/
+        pandas.DataFrame.loc.html#pandas.DataFrame.loc>`__ for full documentation.
 
         Returns
         -------
 
         """
         return _LocTSCIndexer("loc", self)
 
     @property
     def iloc(self):
         """Index-based indexing.
 
-        Visit
-        `pd.DataFrame.iloc <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.iloc.html#pandas.DataFrame.iloc>`_
-        for documentation of how to index DataFrame.
+        Visit `pd.DataFrame.iloc <https://pandas.pydata.org/pandas-docs/stable/reference/
+        api/pandas.DataFrame.iloc.html#pandas.DataFrame.iloc>`__ for documentation of how
+        to index DataFrame.
 
         .. warning::
             For single column slices (e.g. ``tsc.iloc[:, 0]``), the type
             changes to ``pandas.Series``, use ``tsc.iloc[:, [0]]`` instead to maintain a
             ``TSCDataFrame``.
 
         Returns
         -------
 
         """
         return _iLocTSCIndexer("iloc", self)
 
+    def transpose(self, *args, copy: bool = False) -> pd.DataFrame:
+        """Overwrite transpose of super class.
+
+        Because the index and column are swapped the resulting type cannot be of type
+        `TSCDataFrame` anymore. Instead, the transpose is of type `DataFrame`.
+
+        Parameters
+        ----------
+        *args
+        copy
+            Whether to copy the data after transposing, even for DataFrames with a single
+            dtype. Note that a copy is always required for mixed dtype DataFrames, or for
+            DataFrames with any extension types.
+
+        Returns
+        -------
+        pd.DataFrame
+            the transposed data structure
+        """
+        return pd.DataFrame(self).transpose(*args, copy=copy)
+
     def set_index(
         self,
         keys,
         drop=True,
         append=False,
         inplace=False,
         verify_integrity=False,
     ):
-        result = super(TSCDataFrame, self).set_index(
+        result = super().set_index(
             keys=keys,
             drop=drop,
             append=append,
             inplace=inplace,
             verify_integrity=verify_integrity,
         )
 
@@ -1158,39 +1224,39 @@
         self, key, axis=0, level=None, drop_level: bool = True
     ) -> Union[pd.DataFrame, pd.Series]:
         """Overwrites cross section to provide fall back solution in case the result
         is not a valid ``TSCDataFrame`` anymore.
 
         Parameters
         ----------
-        args
+        Args:
+        ----
             see docu
-            `DataFrame.xs <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.xs.html#pandas.DataFrame.xs>`_
+            `DataFrame.xs <https://pandas.pydata.org/pandas-docs/stable/reference/api/
+            pandas.DataFrame.xs.html#pandas.DataFrame.xs>`_
 
         Returns
         -------
         Union[TSCDataFrame, pandas.DataFrame, pandas.Series]
             Cross section of ``TSCDataFrame``. The type is determined by the resulting
             slice.
         """
-
         _slice = pd.DataFrame(self).xs(
             key, axis=axis, level=level, drop_level=drop_level
         )
 
         try:
-            _slice = TSCDataFrame(_slice)
+            _slice = TSCDataFrame(_slice, validate=self.is_validate)
         except AttributeError:
             pass
 
         return _slice
 
     def __getitem__(self, key):
-
-        _slice = super(TSCDataFrame, self).__getitem__(key=key)
+        _slice = super().__getitem__(key=key)
 
         try:
             if isinstance(_slice, pd.Series):
                 # try to convert to TSCDataFrame
                 _slice = TSCDataFrame(_slice)
             else:
                 _slice._validate()
@@ -1200,66 +1266,82 @@
 
         return _slice
 
     def is_datetime_index(self) -> bool:
         """Indicates whether 'time' index is datetime format."""
         return is_datetime64_dtype(self.index.get_level_values(self.tsc_time_idx_name))
 
-    def itertimeseries(self) -> Generator[Tuple[int, pd.DataFrame], None, None]:
+    def itertimeseries(
+        self, valid_tsc=False
+    ) -> Generator[tuple[int, pd.DataFrame], None, None]:
         """Generator of contained time series.
 
         Each iteration returns the time series ID and the corresponding
         time series (a :class:`pd.DataFrame` instead of a ``TSCDataFrame``).
 
+        Parameters
+        ----------
+        valid_tsc
+            If True return a valid format of ``TSCDataFrame`` (i.e. the time series ID is
+            element in the index).
+
         Yields
         ------
-        Tuple[int, pandas.DataFrame]
-            Time series ID and corresponding time series.
+        Tuple[int, pandas.DataFrame] or TSCDataFrame
+            Time series ID and corresponding time series or time series
         """
         for i, ts in self.groupby(level=self.tsc_id_idx_name):
-            # cast single time series back to DataFrame
-            yield i, pd.DataFrame(ts.loc[i, :])
+            if valid_tsc:
+                yield ts
+            else:
+                # cast single time series back to DataFrame
+                yield i, pd.DataFrame(ts.loc[i, :])
 
     def is_equal_length(self) -> bool:
         """Indicates if all time series in the collection have the same number of
         time steps.
         """
         return len(np.unique(self.n_timesteps)) == 1
 
-    def is_const_delta_time(self) -> bool:
-        """Indicates if all time series in the collection have the same time delta."""
+    def is_const_delta_time(self, delta_time=None) -> bool:
+        """Indicates if all time series in the collection have the same time delta.
 
-        # If dt is a Series it means it shows "dt per ID" (because it is not constant).
-        _dt = self.delta_time
+        Parameters
+        ----------
+        delta_time
+            Pass ``delta_time`` if it is already available.
+        """
+        if delta_time is None:
+            # If dt is a Series it means it shows "dt per ID" (because it is not constant).
+            delta_time = self.delta_time
 
-        if isinstance(_dt, pd.Series):
+        if isinstance(delta_time, pd.Series):
             return False
 
         # pd.isnull is better than np.finite because it also checks for
         # NaT (Not a Time[-delta])
-        return not pd.isnull(_dt)
+        return not pd.isnull(delta_time)
 
     def is_same_time_values(self) -> bool:
         """Indicates if all time series in the collection share the same time values."""
-
         if self.n_timeseries == 1:
-            # trivial case early
+            # return trivial case early
             return True
 
         length_time_series = self.n_timesteps
 
         if isinstance(length_time_series, pd.Series):
             return False
         else:
             # Check:
             # If every time series is as long as all (unique) index levels, then they
             # are all the same.
 
             # This call is important, as the levels are usually not updated (even if
-            # they not appear in in the index).
+            # they not appear in the index).
             # See: https://stackoverflow.com/a/43824296
             self.index = self.index.remove_unused_levels()
             n_time_level_values = len(self.index.levels[1])
             return length_time_series == n_time_level_values
 
     def is_normalized_time(self) -> bool:
         """Indicates if the time values are normalized.
@@ -1271,25 +1353,24 @@
         """
         if not self.is_const_delta_time():
             return False
         return self.time_interval()[0] == 0 and self.delta_time == 1
 
     def is_finite(self) -> bool:
         """Indicates if all feature values are finite (i.e. neither NaN nor inf)."""
-        return np.isfinite(self).all().all()
+        return np.isfinite(self.to_numpy()).all().all()
 
     def degenerate_ids(self) -> Optional[pd.Index]:
         """Return the degenerate time series IDs.
 
         Degenerate time series consist only of a single sample.
 
         Returns
         -------
         """
-
         n_timesteps = self.n_timesteps
         _ids = None
 
         if isinstance(n_timesteps, pd.Series):
             _ids = n_timesteps[n_timesteps == 1].index
             if len(_ids) == 0:
                 _ids = None
@@ -1303,226 +1384,113 @@
         """Indicates whether degenerate time series are present in the collection.
 
         Returns
         -------
         """
         return self.degenerate_ids() is not None
 
-    def compute_distance_matrix(
-        self, Y: Optional[Union["TSCDataFrame", np.ndarray]] = None, metric="euclidean"
-    ) -> Union["TSCDataFrame", np.ndarray]:
-        """Compute distance matrix on time series collection.
-
-        Internally calls :py:meth:`datafold.pcfold.distance.compute_distance_matrix`
-        and adds time information if possible.
-
-        No time information is added when
-
-           * the query matrix `Y` is a numpy matrix
-           * the distance matrix is sparse due to ``dist_kwargs`` settings.
-
-        Parameters
-        ----------
-        Y
-            Query point cloud of shape (n_samples_Y, n_features). If provided, compute
-            the distance matrix component-wise, else `Y=self` (pair-wise). For further
-            details see also :class:`.DistanceAlgorithm`.
-
-        metric
-            Distance metric. The backend algorithm set in ``dist_kwargs`` must support
-            the metric.
-
-        Returns
-        -------
-        Union[np.ndarray, scipy.sparse.csr_matrix, TSCDataFrame]
-            Distance matrix.
-        """
-
-        if Y is not None:
-            is_attach_time = isinstance(Y, pd.DataFrame)
-        else:
-            is_attach_time = True
-
-        distance_matrix = compute_distance_matrix(
-            X=self,
-            Y=Y,
-            metric=metric,
-            **self.dist_kwargs,
-        )
-
-        if is_attach_time and not isinstance(distance_matrix, scipy.sparse.spmatrix):
-            time_idx_from = self if Y is None else Y
-
-            distance_matrix = df_type_and_indices_from(
-                time_idx_from,
-                distance_matrix,
-                except_columns=[f"X{i}" for i in np.arange(self.shape[0])],
-            )
-
-        return distance_matrix
-
-    def compute_kernel_matrix(
-        self, Y: Optional[Union[np.ndarray, "TSCDataFrame"]] = None, **kernel_kwargs
-    ) -> pd.DataFrame:
-        """Compute the kernel matrix with the specified kernel.
-
-        Parameters
-        ----------
-        Y
-            Query point cloud or other time series collection of shape
-            `(n_samples_Y, n_features)`. If provided, it computes
-            the kernel matrix component-wise, else `Y=self` for a pair-wise kernel
-            matrix.
-
-        kernel_kwargs
-            Keyword arguments passed passed to the kernel.
-
-        Returns
-        -------
-        Union[numpy.ndarray, pandas.DataFrame, TSCDataFrame]
-            If the kernel is of type :class:`PCManifoldKernel` (i.e. acts on
-            point clouds), the time information is added in this routine. If the time
-            information. For :class:`.TSCManifoldKernel` (i.e. kernels natively act on
-            time series data), the result is directly returned from the kernel.
-
-        Optional
-            The specified kernel can return further objects, which are all forwarded
-            by this function. See :meth:`PCManifoldKernel.__call__`,
-            :meth:`TSCManifoldKernel.__call__` or the respective kernel for details.
-        """
-
-        if self.kernel is None:
-            raise TSCException.no_kernel()
-
-        if Y is not None:
-            is_attach_time = isinstance(Y, pd.DataFrame)
-        else:
-            is_attach_time = True
-
-        kernel_output = self.kernel(
-            X=self,
-            Y=Y,
-            dist_kwargs=self.dist_kwargs,
-            **kernel_kwargs,
-        )
-
-        if isinstance(kernel_output, (tuple, list)):
-            ty_kernel_matrix = type(kernel_output[0])
-        else:
-            ty_kernel_matrix = type(kernel_output)
-
-        def _pcmkernel2tsc(kernel_matrix, indices_from):
-            return df_type_and_indices_from(
-                indices_from,
-                kernel_matrix,
-                except_columns=[f"X{i}" for i in np.arange(self.shape[0])],
-            )
-
-        if is_attach_time and ty_kernel_matrix == np.ndarray:
-            time_idx_from = self if Y is None else Y
-
-            if isinstance(kernel_output, (tuple, list)):
-                kernel_output = list(kernel_output)
-                kernel_output[0] = _pcmkernel2tsc(kernel_output[0], time_idx_from)
-                kernel_output = tuple(kernel_output)
-            else:
-                kernel_output = _pcmkernel2tsc(kernel_output, time_idx_from)
-
-        return kernel_output
-
     def insert_ts(
         self, df: pd.DataFrame, ts_id: Optional[int] = None
     ) -> "TSCDataFrame":
-        """Inserts new time series to current collection.
+        """Inserts new time series to the current collection.
 
         Parameters
         ----------
         df
-            New time series, with same features (column names) as the existing.
-            If ``df`` is of type ``pd.DataFrame``, the row index must contain time
+            New time series. The column names have to match the existing collection.
+            If ``df`` is of type ``pd.DataFrame``, the index must contain time
             values.
         ts_id
-            Dedicated ID of new time series (must not be present in current collection).
+            Unique ID for new time series. Defaulting to increase the largest present ID by 1.
 
         Returns
         -------
         TSCDataFrame
             self
         """
         if ts_id is None:
-            ts_id = self.ids.max() + 1  # is unique and positive
+            ts_id = self.ids.max() + 1  # unique and positive
 
         if ts_id in self.ids:
-            raise ValueError(f"ID {ts_id} already present.")
+            raise ValueError(f"ID {ts_id} already in the existing collection.")
 
         if not is_integer(ts_id):
-            raise ValueError(f"ts_id has to be an integer type. Got={type(ts_id)}.")
+            raise ValueError(f"ts_id has to be an integer type. Got: {type(ts_id)=}.")
 
         if self.n_features != df.shape[1] or not (self.columns == df.columns).all():
             raise ValueError(
                 "Column names do not match. "
                 f"Expected \n{self.columns} "
                 f"but got \n{df.columns} "
             )
 
         if df.index.nlevels == 1:
             _index = df.index
         elif df.index.nlevels == 2 and isinstance(df, TSCDataFrame):
             _index = df.index.get_level_values(self.tsc_time_idx_name)
         else:
-            raise ValueError("The input parameter 'df' is of wrong format.")
+            raise ValueError("The input parameter 'df' has an incompatible format.")
 
         if self.is_datetime_index() ^ np.issubdtype(_index.dtype, np.datetime64):
+            existing_type = self.index.get_level_values(
+                TSCDataFrame.tsc_time_idx_name
+            ).dtype
             raise ValueError(
-                "If the existing index is datetime64, but the new time "
-                f"series has dype={_index.dtype} for time values."
+                f"Cannot attach time values with dtype={existing_type} to a "
+                f"collection with dtype={_index.dtype}."
             )
 
-        # Add the id to the first level of the MultiIndex
+        # Add the ID to the first level of the MultiIndex
         df.index = pd.MultiIndex.from_arrays(
             [np.ones(df.shape[0], dtype=int) * ts_id, _index],
             names=[self.tsc_id_idx_name, self.tsc_time_idx_name],
         )
 
         # 'self' has to appear first to keep TSCDataFrame type.
         return pd.concat([self, df.copy(deep=True)], sort=False, axis=0)
 
     def time_interval(
         self, ts_id: Optional[int] = None
-    ) -> Tuple[NumericalTimeType, NumericalTimeType]:
-        """Time interval (start, end) for all or single time series in
-        the collection.
+    ) -> tuple[NumericalTimeType, NumericalTimeType]:
+        """Time interval (start, end) covered by the collection or a specific time series.
 
         Parameters
         ----------
         ts_id
-            Time series ID. If not provided, the interval is over all time series
-            in the collection.
+            Time series ID. Defaults to the interval in the collection.
         """
-
         if ts_id is None:
             time_values = self.time_values()
         else:
             time_values = self.loc[ts_id, :].index
 
         return np.min(time_values), np.max(time_values)
 
-    def time_values(self) -> np.ndarray:
+    def time_values(self, with_fixed_delta: bool = True) -> np.ndarray:
         """All time values that appear in at least one time series of the collection.
 
+        Attributes
+        ----------
+        with_fixed_delta
+            If True return the actual time values according to a set `fixed_delta`.
+
         Returns
         -------
-
+        np.ndarray
+            all time values that appear in the collection
         """
         self.index = self.index.remove_unused_levels()
-        return np.asarray(self.index.levels[1])
+        ret_idx = np.asarray(self.index.levels[1])
+        if self.fixed_delta is not None and with_fixed_delta:
+            ret_idx = ret_idx.astype(float)
+            ret_idx *= self.fixed_delta
+        return ret_idx
 
-    def time_values_delta_time(self) -> np.ndarray:
-        """All time values between `(start, end)` interval with constant time
-        delta.
+    def const_sampled_time_values(self) -> np.ndarray:
+        """All time values between `(start, end)` interval with constant time delta.
 
         Potential gaps between time series are closed so that a constant delta time is
         maintained in returned time array.
 
         Returns
         -------
         numpy.ndarray
@@ -1530,15 +1498,14 @@
 
         Raises
         ------
         TSCException
             if `delta_time` is not constant
 
         """
-
         if not self.is_const_delta_time():
             raise TSCException.not_const_delta_time()
 
         start, end = self.time_interval()
 
         if self.is_datetime_index():
             return np.arange(start, end + np.timedelta64(1, "ns"), self.delta_time)
@@ -1572,18 +1539,17 @@
 
         Raises
         ------
         TSCException
             If time series in the collection have not identical time values.
 
         """
-
         if feature is None and self.shape[1] > 1:
             raise ValueError(
-                "parameter 'feature' must be provided if there are " "multiple features"
+                "parameter 'feature' must be provided if there are multiple features"
             )
         elif feature is None:
             feature = self.columns[0]
 
         if not self.is_same_time_values():
             raise TSCException.not_same_time_values()
 
@@ -1617,38 +1583,38 @@
         return self.loc[idx[:, time_values], :]
 
     def initial_states(self, n_samples: int = 1) -> "TSCDataFrame":
         """Get initial state of each time series in the collection.
 
         Parameters
         ----------
-
         n_samples
             Number of samples required for an initial state.
 
         Returns
         -------
         TSCDataFrame
             Initial states of shape `(n_samples * n_timeseries, n_features)`.
 
         Raises
         ------
         TSCException
             If there is a time series in the collection that has less time values
-            than than the required number of samples.
+            than the required number of samples.
         """
-
         if not is_integer(n_samples) or n_samples < 1:
             raise ValueError(
-                "The parameter 'n_samples' must be a positive integer value."
+                f"The parameter 'n_samples' must be a positive integer value. "
+                f"Got {n_samples=} with {type(n_samples)=}"
             )
 
         self.tsc.check_required_min_timesteps(required_min_timesteps=n_samples)
-
-        return self.groupby(by="ID", axis=0, level=0).head(n=n_samples)
+        return self.groupby(by=TSCDataFrame.tsc_id_idx_name, axis=0, level=0).head(
+            n=n_samples
+        )
 
     def final_states(self, n_samples: int = 1) -> "TSCDataFrame":
         """Get the final states of each time series in the collection.
 
         Parameters
         ----------
         n_samples
@@ -1661,31 +1627,35 @@
 
         Raises
         ------
         TSCException
             If there is a time series with less than the required number of samples.
 
         """
-
         if not is_integer(n_samples) or n_samples < 1:
-            raise ValueError("Parameter 'n_samples' must be a positive integer.")
+            raise ValueError(
+                f"Parameter 'n_samples' must be a positive integer. "
+                f"Got: {type(n_samples)=} and {n_samples=}"
+            )
 
         self.tsc.check_required_min_timesteps(required_min_timesteps=n_samples)
-
-        return self.groupby(by="ID", axis=0, level=0).tail(n=n_samples)
+        return self.groupby(by=TSCDataFrame.tsc_id_idx_name, axis=0, level=0).tail(
+            n=n_samples
+        )
 
     def plot(self, **kwargs):
         """Plots time series.
 
         Parameters
         ----------
         **kwargs
             Key word arguments handled to each time series
-            `pandas.DataFrame.plot() <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.plot.html?highlight=plot#pandas.DataFrame.plot>`_
-            call.
+            `pandas.DataFrame.plot()
+            <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.
+            plot.html?highlight=plot#pandas.DataFrame.plot>`__ call.
 
         Returns
         -------
         matplotlib object
             axes handle
         """
         ax = kwargs.pop("ax", None)
@@ -1695,18 +1665,20 @@
 
         if color is not None and c is not None:
             raise TypeError(
                 "Got both 'color' and 'c', which are aliases of one another."
             )
         elif c is not None:
             color = c
+        else:
+            color = "black"
 
         first = True
 
-        for i, ts in self.itertimeseries():
+        for _, ts in self.itertimeseries():
             kwargs["ax"] = ax
 
             if first:
                 # there may be already lines in it, set color of *new* lines
                 exist_lines = len(ax.lines) if ax is not None else 0
 
                 ax = ts.plot(color=color, legend=legend, **kwargs)
@@ -1719,15 +1691,15 @@
                 first = False
             else:
                 ax = ts.plot(color=color, legend=False, **kwargs)
 
         return ax
 
 
-class InitialCondition(object):
+class InitialCondition:
     """Helper functions to create and validate initial conditions for time series
     predictions.
 
     Initial conditions are internally described with ``TSCDataFrame`` objects.
 
     In general, initial conditions are required in models that train on time series
     data, see for example in :py:meth:`EDMD.predict`. An initial condition can consist of
@@ -1735,58 +1707,99 @@
     the case if model transformations require multiple time values to define the
     transformed state (such as :py:class:`.TSCTakensEmbedding` or
     :py:class:`TSCFiniteDifference`).
     """
 
     @classmethod
     def from_array(
-        cls, X: np.ndarray, columns: Union[pd.Index, List[str]]
+        cls,
+        X: np.ndarray,
+        time_value: Union[float, int],
+        feature_names: Union[pd.Index, list[str]],
+        ts_ids: Optional[np.ndarray] = None,
     ) -> TSCDataFrame:
         """Build initial conditions object from a NumPy array.
 
         Note that the assumption is that each row is a new initial condition. All time
         values are set to zero.
 
         Parameters
         ----------
         X
             Initial condition of shape `(n_ic, n_features)`.
 
-        columns
+        time_value
+            Time value associated to the initial condition.
+
+        feature_names
             Feature names in model during fit (they can be accessed with
             :code:`model_obj.features_in_[1]`.
 
+        ts_ids
+            Time series ids.  Defaults to range(0, n_initial_condition).
+
         Returns
         -------
         TSCDataFrame
             initial condition
         """
-
-        if isinstance(columns, list):
+        # TODO: generalize array also for tensors (where an IC is a time series with a fixed
+        #  number of time steps)
+        if isinstance(feature_names, list):
             # feature name is not enforced for initial conditions
-            columns = pd.Index(columns, name=TSCDataFrame.tsc_feature_col_name)
+            feature_names = pd.Index(
+                feature_names, name=TSCDataFrame.tsc_feature_col_name
+            )
 
         if X.ndim == 1:
-            # make a "row-matrix"
+            # turn to matrix with row-oriented states
             X = X[np.newaxis, :]
-
-        if X.ndim > 2:
+        elif X.ndim > 2:
             raise ValueError(
-                "Cannot convert arrays with dimension larger than 2. Got "
-                f"X.ndim={X.ndim}"
+                f"Cannot convert array with dimension larger than 2. Got {X.ndim=}."
             )
 
         n_ic = X.shape[0]
-        index = pd.MultiIndex.from_arrays([np.arange(n_ic), np.zeros(n_ic)])
+        if ts_ids is None:
+            ts_ids = np.arange(n_ic)
+
+        index = pd.MultiIndex.from_arrays([ts_ids, np.repeat(time_value, n_ic)])
 
-        ic_df = TSCDataFrame(X, index=index, columns=columns)
+        ic_df = TSCDataFrame(X, index=index, columns=feature_names)
         InitialCondition.validate(ic_df, n_samples_ic=1, dt=None)
         return ic_df
 
     @classmethod
+    def from_array_control(
+        cls,
+        U,
+        *,
+        control_names,
+        dt: Optional[Union[float, int]] = None,
+        time_values: Optional[np.ndarray] = None,
+        ts_id: Optional[int] = None,
+    ) -> TSCDataFrame:
+        if not isinstance(U, np.ndarray):
+            raise TypeError("")
+
+        U = if1dim_colvec(U)
+
+        if (dt is None) + (time_values is None) == 2:
+            raise ValueError("")
+
+        if time_values is None:
+            time_values = np.arange(0, U.shape[0] * dt, dt)
+
+        U = TSCDataFrame.from_array(
+            U, time_values=time_values, feature_names=control_names, ts_id=ts_id
+        )
+
+        return U
+
+    @classmethod
     def from_tsc(cls, X: TSCDataFrame, n_samples_ic: int = 1) -> pd.DataFrame:
         """Extract initial states from a ``TSCDataFrame``.
 
         Parameters
         ----------
         X
             The time series data to extract initial states from.
@@ -1795,53 +1808,55 @@
             The number of time steps per initial condition.
 
         Returns
         -------
         TSCDataFrame
             initial condition
         """
-
         ic_df = X.initial_states(n_samples=n_samples_ic)
         InitialCondition.validate(
             ic_df,
             n_samples_ic=n_samples_ic,
             dt=X.delta_time if n_samples_ic > 1 else None,
         )
         return ic_df
 
     @classmethod
     def iter_reconstruct_ic(
-        cls, X: TSCDataFrame, n_samples_ic: int = 1
-    ) -> Generator[Tuple[TSCDataFrame, np.ndarray], None, None]:
+        cls, X: TSCDataFrame, U: Optional[TSCDataFrame] = None, n_samples_ic: int = 1
+    ) -> Generator[tuple[TSCDataFrame, np.ndarray], None, None]:
         """Extract and iterate over initial conditions over groups of time series that
         have identical time values.
 
-        This iterator is particulary usefule to reconstruct time series.
+        This iterator is useful for reconstructing time series.
 
         Parameters
         ----------
         X
             The time series collection to extract initial states from.
 
+        U
+            The control input acting on the states. If they are provided, these are used to
+            identify the time values of the prediction horizon.
+
         n_samples_ic
             The number of time steps per initial condition.
 
         Returns
         -------
         iterator Tuple[TSCDataFrame, numpy.ndarray]
             Each iteration returns the initial states for each time series of the group
             and the associate time values.
         """
-
         X.tsc.check_required_min_timesteps(n_samples_ic)
         time_series_table = X.tsc.time_values_overview()
 
         if np.isnan(time_series_table["delta_time"]).any():
             raise NotImplementedError(
-                "Currently, only constant delta times are " "implemented."
+                "Currently, only constant delta times are implemented."
             )
 
         for (_, _, _), df in time_series_table.groupby(
             by=["start", "end", "delta_time"], axis=0
         ):
             grouped_ids = df.index
             grouped_tsc: TSCDataFrame = X.loc[grouped_ids, :]
@@ -1859,33 +1874,40 @@
     @classmethod
     def validate(
         cls,
         X_ic: TSCDataFrame,
         n_samples_ic: Optional[int] = None,
         dt: Optional[float] = None,
     ) -> bool:
-        """Validate the initial condition format of a :py:class:`-TSCDataFrame`.
+        """Validate the initial condition format of a :py:class:`TSCDataFrame`.
 
         Parameters
         ----------
         X_ic
             The initial condition to validate.
 
         n_samples_ic
             If provided, then validate that each initial condition has the set number of
             samples.
 
         dt
             If provided, then validate that the time series have the set constant delta
             time sampling. The parameter ``n_samples_ic`` must be given at the same time.
 
+        Raises
+        ------
+        TypeError, ValueError
+            If initial condition is not valid
+
         Returns
         -------
-        """
+        bool
+            True if the the initial condition is valid
 
+        """
         if not isinstance(X_ic, TSCDataFrame):
             raise TypeError(
                 "The initial condition to be validated must be of type TSCDataFrame."
             )
 
         if n_samples_ic is None and dt is not None:
             raise ValueError(
@@ -1895,29 +1917,40 @@
 
         if n_samples_ic == 1 and dt is not None:
             raise ValueError(
                 "Cannot check the time sampling rate, when at the same "
                 "time only one sample is required per initial condition."
             )
 
-        # all the usual restrictions for TSCDataFrame apply
-        assert X_ic._validate()
-
         X_ic.tsc.check_tsc(
             ensure_const_delta_time=np.array(X_ic.n_timesteps > 1).any(),
             ensure_no_degenerate_ts=False,
             ensure_same_length=True,
             ensure_all_finite=True,
             ensure_same_time_values=True,
             ensure_n_timesteps=n_samples_ic,
             ensure_delta_time=dt,
         )
 
         return True
 
+    @classmethod
+    def validate_control(cls, X_ic: TSCDataFrame, U: TSCDataFrame):
+        X_ic.tsc.check_contain_required_ids(required_ids=U.ids, check_order=True)
+        U.tsc.check_equal_timevalues()
+
+        last_state_time = X_ic.final_states(1).time_values()[0]
+        first_control_time = U.initial_states(1).time_values()[0]
+
+        if (last_state_time != first_control_time).any():
+            raise TSCException(
+                f"The last time value of X (={last_state_time}) must match the "
+                f"first time value of the control input (={first_control_time})."
+            )
+
 
 def allocate_time_series_tensor(n_time_series, n_timesteps, n_feature):
     """Allocate a time series tensor that complies with
     :py:meth:`TSCDataFrame.from_tensor()`.
 
     Allocated three-dimensional ``numpy.ndarray`` is C-aligned and can be accessed with
```

### Comparing `datafold-1.1.6/datafold/pcfold/timeseries/metric.py` & `datafold-2.0.0/datafold/pcfold/timeseries/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-#!/usr/bin/env python3
-
 import abc
+from collections.abc import Generator
 from functools import partial
-from typing import Generator, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from sklearn import metrics
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import MinMaxScaler, Normalizer, StandardScaler
 
 from datafold.pcfold import TSCDataFrame
 from datafold.utils.general import is_df_same_index, is_integer, series_if_applicable
 
 
-class TSCMetric(object):
+class TSCMetric:
     """Compute metrics for time series collection data.
 
     Parameters
     ----------
-
     metrics
 
         * "rmse" - root mean squared error,
         * "rrmse" - relative root mean squared error
         * "mse" - mean squared error,
         * "mae" - mean absolute error,
         * "max" maximum error,
@@ -39,25 +37,28 @@
         * "id" - no scaling,
         * "min-max" - each feature is scaled into (0, 1) range,
         * "standard" - remove mean and scale to unit variance for each feature,
         * "l2_normalize" - divide each feature by Euclidean norm
 
     References
     ----------
-
-    "rrmse" is taken from :cite:`le_clainche_higher_2017`
+    "rrmse" is taken from :cite:t:`leclainche-2017`
 
     """
 
     _cls_valid_modes = ["timeseries", "timestep", "feature"]
     _cls_valid_metrics = ["rmse", "rrmse", "mse", "mape", "mae", "medae", "max", "l2"]
     _cls_valid_scaling = ["id", "min-max", "standard", "l2_normalize"]
 
-    def __init__(self, metric: str, mode: str, scaling: str = "id"):
-
+    def __init__(
+        self,
+        metric: Literal["rmse", "rrmse", "mse", "mape", "mae", "medae", "max", "l2"],
+        mode: Literal["timeseries", "timestep", "feature"],
+        scaling: Literal["id", "min-max", "standard", "l2_normalize"] = "id",
+    ):
         mode = mode.lower()
         metric = metric.lower()
 
         if metric in self._cls_valid_metrics:
             self.metric = self._metric_from_str_input(metric)
         else:
             raise ValueError(
@@ -70,47 +71,44 @@
             raise ValueError(
                 f"Invalid mode='{mode}'. Choose from {self._cls_valid_modes}"
             )
 
         self.scaling = self._select_scaling(name=scaling)
 
     def _select_scaling(self, name):
-
         if name == "id":
             return None
         elif name == "min-max":
             return MinMaxScaler()
         elif name == "standard":
             return StandardScaler()
         elif name == "l2_normalize":
             return Normalizer(norm="l2")
         else:
             raise ValueError(
                 f"scaling={name} is not known. Choose from {self._cls_valid_scaling}"
             )
 
     def _scaling(self, y_true: TSCDataFrame, y_pred: TSCDataFrame):
-
         # it is checked before that y_true and y_pred indices/columns are identical
         index, columns = y_true.index, y_true.columns
 
         # first normalize y_true, afterwards (with the same factors from y_true!) y_pred
         if self.scaling is not None:  # is None if scaling is identity
             y_true = self.scaling.fit_transform(y_true)
-            y_pred = self.scaling.transform(y_pred.to_numpy())
+            y_pred = self.scaling.transform(y_pred)
 
             y_true = TSCDataFrame(y_true, index=index, columns=columns)
             y_pred = TSCDataFrame(y_pred, index=index, columns=columns)
 
         return y_true, y_pred
 
     def _l2_metric(
         self, y_true, y_pred, sample_weight=None, multioutput="uniform_average"
     ):
-
         diff = y_true - y_pred
 
         if sample_weight is not None:
             diff = sample_weight[:, np.newaxis] * diff
 
         l2_norm = np.linalg.norm(diff, axis=0)
 
@@ -119,15 +117,14 @@
 
         return l2_norm
 
     def _medae_metric(
         self, y_true, y_pred, sample_weight=None, multioutput="uniform_average"
     ):
         """Median absolute error."""
-
         if sample_weight is not None:
             raise ValueError("Median absolute error does not support sample_weight.")
 
         return metrics.median_absolute_error(
             y_true=y_true, y_pred=y_pred, multioutput=multioutput
         )
 
@@ -161,16 +158,15 @@
     #     if multioutput == "uniform_average":
     #         error = np.mean(error)
     #     return error
 
     def _rrmse_metric(
         self, y_true, y_pred, sample_weight=None, multioutput="uniform_average"
     ):
-        """Metric from :cite:`le_clainche_higher_2017`"""
-
+        """Metric from :cite:`le_clainche_higher_2017`."""
         if multioutput == "uniform_average":
             norm_ = np.sum(np.square(np.linalg.norm(y_true, axis=1)))
         else:  # multioutput == "raw_values":
             norm_ = np.sum(np.square(y_true), axis=0)
 
         if (np.asarray(norm_) <= 1e-14).any():
             raise RuntimeError(
@@ -186,20 +182,18 @@
 
     def _max_error(
         self, y_true, y_pred, sample_weight=None, multioutput="uniform_average"
     ):
         """Wrapper for :class:`sklean.metrics.max_error` to allow `sample_weight` and
         `multioutput` arguments (both have not effect).
         """
-
         # fails if y is multioutput
         return metrics.max_error(y_true=y_true, y_pred=y_pred)
 
     def _metric_from_str_input(self, error_metric: str):
-
         error_metric = error_metric.lower()
         from typing import Callable
 
         error_metric_handle: Callable
         if error_metric == "rmse":  # root mean squared error
             error_metric_handle = partial(metrics.mean_squared_error, squared=False)
         elif error_metric == "rrmse":  # relative root mean squared error
@@ -233,15 +227,14 @@
             scalar_score = False
 
         else:
             raise ValueError(f"Illegal argument multioutput='{multioutput}'")
         return scalar_score
 
     def _single_column_name(self, multioutput) -> list:
-
         assert self._is_scalar_multioutput(multioutput)
 
         if isinstance(multioutput, str) and multioutput == "uniform_average":
             column = ["metric_uniform_average"]
         elif isinstance(multioutput, np.ndarray):
             column = ["metric_user_weights"]
         else:
@@ -252,15 +245,14 @@
     def _metric_per_timeseries(
         self,
         y_true: TSCDataFrame,
         y_pred: TSCDataFrame,
         sample_weight=None,
         multioutput="uniform_average",
     ) -> Union[pd.Series, pd.DataFrame]:
-
         if sample_weight is not None:
             # same length of time series to have mapping
             # sample_weight -> time step of time series (can be a different time value)
             y_true.tsc.check_timeseries_same_length()
 
             if sample_weight.shape[0] != y_true.n_timesteps:
                 raise ValueError(
@@ -329,50 +321,48 @@
     def _metric_per_timestep(
         self,
         y_true: TSCDataFrame,
         y_pred: TSCDataFrame,
         sample_weight=None,
         multioutput="uniform_average",
     ):
-
         if sample_weight is not None:
             # sample weights -> each time series has a different weight
 
             # Currently, all time series must have the same time values to have the same
             # length for each time step
             y_true.tsc.check_timeseries_same_length()
 
             # the weight, must be as long as the time series
             if sample_weight.shape[0] != y_true.n_timeseries:
                 raise ValueError(
                     f"'sample_weight' shape (={sample_weight.shape[0]}) "
                     f"does not match the number of time series (={y_true.n_timeseries})."
                 )
 
-        time_indices = pd.Index(y_true.time_values(), name="time")
+        time_values = pd.Index(y_true.time_values(), name="time")
 
         if self._is_scalar_multioutput(multioutput=multioutput):
             column = self._single_column_name(multioutput=multioutput)
 
             # Make in both cases a DataFrame and later convert to Series in the scalar
             # case this allows to use .loc[i, :] in the loop
-            metric_per_time = pd.DataFrame(np.nan, index=time_indices, columns=column)
+            metric_per_time = pd.DataFrame(np.nan, index=time_values, columns=column)
 
         else:
             metric_per_time = pd.DataFrame(
-                np.nan, index=time_indices, columns=y_true.columns.to_list()
+                np.nan, index=time_values, columns=y_true.columns.to_list()
             )
 
         metric_per_time.index = metric_per_time.index.set_names(
             TSCDataFrame.tsc_time_idx_name
         )
 
         idx_slice = pd.IndexSlice
-        for t in time_indices:
-
+        for t in time_values:
             y_true_t = pd.DataFrame(y_true.loc[idx_slice[:, t], :])
             y_pred_t = pd.DataFrame(y_pred.loc[idx_slice[:, t], :])
 
             metric_per_time.loc[t, :] = self.metric(
                 y_true_t,
                 y_pred_t,
                 sample_weight=sample_weight,
@@ -428,15 +418,14 @@
 
         Raises
         ------
         TSCException
             If not all values are finite in `y_true` or `y_pred` or if \
             :class:`TSCDataFrame` properties do not allow for a `sample_weight` argument.
         """
-
         if sample_weight is not None:
             sample_weight = np.asarray(sample_weight)
 
             if sample_weight.ndim != 1:
                 raise ValueError("'sample_weight' must be an 1-dim. array")
 
         # checks:
@@ -485,15 +474,15 @@
             raise RuntimeError(
                 f"Unknown return type {type(metric_result)}. Please report bug."
             )
 
         return metric_result
 
 
-class TSCScoring(object):
+class TSCScoring:
     """Create scoring function from :class:`.TSCMetric`.
 
     Parameters
     ----------
     tsc_metric
         Time series collections metric.
 
@@ -550,15 +539,14 @@
             * `TSCMetric.mode=time` - weight array of shape `(n_timesteps,)`
 
         Returns
         -------
         :class:`float`
             score
         """
-
         eval_tsc_metric: pd.Series = self.tsc_metric(
             y_true=y_true,
             y_pred=y_pred,
             sample_weight=self.metric_kwargs.get("sample_weight", None),
             multioutput=self.metric_kwargs.get("multioutput", "uniform_average"),
         )
 
@@ -630,15 +618,15 @@
     ):
         self.kfold_splitter = KFold(
             n_splits=n_splits, shuffle=shuffle, random_state=random_state
         )
 
     def split(
         self, X: TSCDataFrame, y=None, groups=None
-    ) -> Generator[Tuple[np.ndarray, np.ndarray], None, None]:
+    ) -> Generator[tuple[np.ndarray, np.ndarray], None, None]:
         """Yields k-folds of training and test indices of time series collection.
 
         Parameters
         ----------
         X
             The time series collection to split.
 
@@ -710,15 +698,14 @@
     also consist of only a single time series. Note that if a block is taken from
     testing, then this results in more training series as in the original time series
     collection. For example, for a single time series this would result in two training
     time series and one test time series.
 
     Parameters
     ----------
-
     n_splits
         The number of splits.
     """
 
     def __init__(self, n_splits: int = 3):
         self.kfold_splitter = KFold(n_splits=n_splits, shuffle=False, random_state=None)
 
@@ -799,15 +786,14 @@
       no overlapping. If the next window within a time series cannot be placed,
       then these samples will not be included in any test set.
     * If a time series has less samples than ``test_window_length``, then this time
       series will not be considered for testing.
 
     Parameters
     ----------
-
     test_window_length
         The length of a window for samples included in testing.
 
     window_offset
         The offset to next possible test window. In a single long time series the offset
         equals the gap between windows.
 
@@ -819,15 +805,14 @@
 
     def __init__(
         self,
         test_window_length: int,
         window_offset: int = 0,
         train_min_timesteps: Optional[int] = None,
     ):
-
         if not is_integer(test_window_length) or test_window_length <= 0:
             raise ValueError(
                 f"The parameter 'test_window_length={test_window_length}' must be a "
                 f"positive integer."
             )
 
         if not is_integer(window_offset) or window_offset < 0:
@@ -902,15 +887,14 @@
         X.tsc.check_const_time_delta()
 
         for test_tsc in indices_tsc.copy().tsc.iter_timevalue_window(
             window_size=self.test_window_length,
             offset=self.test_window_length + self.test_offset,
             per_time_series=True,
         ):
-
             train_tsc = indices_tsc.copy().drop(test_tsc.index, axis=0)
 
             # it is important to reassign the ids to keep the same sub-sampling and
             # assign two IDs, if the test window is somewhere in between
             # a longer time series.
             train_tsc, test_tsc = indices_tsc.copy().tsc.assign_ids_train_test(
                 train_indices=train_tsc.time_values(),
@@ -955,15 +939,14 @@
 
         groups
             ignored
 
         Returns
         -------
         """
-
         if X is None:
             raise ValueError("'X' must be provided to compute the number of splits.")
 
         return len(list(self.split(X)))
 
     def plot_splits(self, X: TSCDataFrame, test_set=None) -> None:
         """Plot the test, training and dropped samples.
@@ -993,15 +976,14 @@
 
         f, ax = plt.subplots(n_splits, 1, sharex=True, sharey=True)
 
         time_name = TSCDataFrame.tsc_time_idx_name
         id_name = TSCDataFrame.tsc_id_idx_name
 
         for i, (train_indices, test_indices) in enumerate(self.split(X)):
-
             train_tsc, test_tsc, dropped_samples = X.tsc.assign_ids_train_test(
                 train_indices, test_indices, return_dropped=True
             )
 
             if n_splits == 1:
                 _ax = ax
             else:
```

### Comparing `datafold-1.1.6/datafold/utils/_systems.py` & `datafold-2.0.0/datafold/utils/plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,340 +1,336 @@
 #!/usr/bin/env python3
 
-import abc
+import warnings
+from typing import Optional
 
+import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
-from scipy.integrate import odeint, solve_ivp
 
-from datafold.pcfold import TSCDataFrame
+from datafold._decorators import warn_experimental_function
 
 
-# TODO: could be a TSCPredictMixin
-class DynamicalSystem(metaclass=abc.ABCMeta):
-    @abc.abstractmethod
-    def predict(self, initial_conditions, time_values, **kwargs):
-        raise NotImplementedError("base class")
+def plot_eigenvalues(
+    eigenvalues: np.ndarray,
+    *,
+    plot_unit_circle: bool = False,
+    semilogy: bool = False,
+    ax=None,
+    subplot_kwargs: Optional[dict[str, object]] = None,
+    plot_kwargs: Optional[dict[str, object]] = None,
+):
+    """Plots eigenvalue distribution.
+
+    Parameters
+    ----------
+    eigenvalues
+        Complex or real eigenvalues.
+
+    plot_unit_circle
+        If True, include unit circle on complex plane.
+
+    semilogy
+        Enable logarithmic y-axis. Parameter is ignored for complex eigenvalues.
+
+    ax
+        Plot in existing matplotlib axes object. ``subplot_kwargs`` are ignored then.
 
+    subplot_kwargs
+        Keyword arguments passed to ``plt.subplot``.
 
-class LimitCycle(DynamicalSystem):
-    def __init__(self, eps=1, analytical=True):
-        self.obs = None
-        self.eps = eps
-        self.analytical = analytical
+    plot_kwargs
+        Keyword arguments passed to ``ax.plot(**plot_kwargs)``
 
-    def _compute_angle(self, x1, x2):
-        e_vec = np.array([1, 0])
-        vec = np.array([x1, x2])
-
-        norm_vec = np.linalg.norm(vec)
-
-        if norm_vec < 1e-15:
-            return 0
-
-        if x2 < 0:
-            angle = 2 * np.pi - np.arccos(np.dot(e_vec, vec) / norm_vec)
-        else:
-            angle = np.arccos(np.dot(e_vec, vec) / norm_vec)
+    Returns
+    -------
+    """
+    if ax is None:
+        _, ax = plt.subplots(**({} if subplot_kwargs is None else subplot_kwargs))
 
-        return angle
+    plot_kwargs = plot_kwargs or {}
+    plot_kwargs.setdefault("marker", "+")
+    plot_kwargs.setdefault("linewidth", 0)
+
+    if eigenvalues.dtype == complex:
+        ax.plot(np.real(eigenvalues), np.imag(eigenvalues), **plot_kwargs)
+
+        if plot_unit_circle:
+            circle_values = np.linspace(0, 2 * np.pi, 3000)
+            ax.plot(np.cos(circle_values), np.sin(circle_values), "-", color="gray")
+            ax.set_aspect("equal")
+
+        with plt.rc_context(rc={"text.usetex": True}):
+            ax.set_xlabel("$\\Re(\\lambda)$")
+            ax.set_ylabel("$\\Im(\\lambda)$")
+
+    elif eigenvalues.dtype == float:
+        if plot_unit_circle:
+            warnings.warn(
+                "eigenvalues are real-valued, 'plot_unit_circle=True' is ignored",
+                stacklevel=2,
+            )
 
-    def _as_cartesian_coordinates(self, ang, rad):
-        vals = rad * np.exp(0 + 1j * ang)
-        return np.real(vals), np.imag(vals)
-
-    def predict(self, **kwargs):
-
-        if "t_eval" in kwargs:
-            kwargs["nr_steps"] = len(kwargs["t_eval"])
-            t_diff = np.diff(kwargs["t_eval"])
-            assert (
-                len(np.unique(np.round(t_diff, decimals=10))) == 1
-            )  # TODO only equidistant is supported at the moment!
-            kwargs["dt"] = t_diff[0]
-            del kwargs["t_eval"]
+        eigenvalues = np.sort(eigenvalues.copy())[::-1]
 
-        if self.analytical:
-            return self.eval_analytical(**kwargs)
+        _ylabel_text = "eigenvalue $\\lambda$"
+        if semilogy:
+            ax.semilogy(np.arange(len(eigenvalues)), eigenvalues, **plot_kwargs)
+            _ylabel_text = _ylabel_text + " (log scale)"
         else:
-            return self.eval_finite_differences(**kwargs)
+            ax.plot(np.arange(len(eigenvalues)), eigenvalues, **plot_kwargs)
 
-    def eval_finite_differences(self, x1, x2, dt, nr_steps):
-        # use Euler, could also be solved analytically
-        # diss, p. 52 t_end=10^-3 and nr_steps=10, eps=1E-2
-        t = np.linspace(0, dt * (nr_steps - 1), nr_steps)
-        r0 = np.linalg.norm(np.array([x1, x2]))
-        a0 = self._compute_angle(x1=x1, x2=x2)
-
-        a_vals = np.zeros(nr_steps)
-        a_vals[0] = a0
-
-        r_vals = np.zeros(nr_steps)
-        r_vals[0] = r0
-
-        for i in range(1, nr_steps):
-            a_vals[i] = a_vals[i - 1] + dt * 1 / self.eps
-            r_vals[i] = r_vals[i - 1] + dt * ((-r_vals[i - 1] ** 2 + 1) * r_vals[i - 1])
-
-        # x, y = self._as_cartesian_coordinates(rad=r_vals, ang=a_vals)
-        self.obs = pd.DataFrame(
-            np.vstack([a_vals, r_vals]).T, index=t, columns=["alpha", "radius"]
-        )
-        return self.obs
-
-    def eval_analytical(self, x1, x2, dt, nr_steps):
-        t = np.linspace(0, dt * (nr_steps - 1), nr_steps)
-
-        a0 = self._compute_angle(x1=x1, x2=x2)
-        r0 = (
-            np.linalg.norm(np.array([x1, x2])) + 1e-10
-        )  # add a small number to avoid division by zero
+        with plt.rc_context(rc={"text.usetex": True}):
+            ax.set_ylabel(_ylabel_text)
 
-        a_vals = 1 / self.eps * t + a0
+        ax.set_xlabel("index eigenvalue")
 
-        r_vals = np.exp(t) / np.sqrt(-1 + np.exp(2 * t) + 1 / r0 ** 2)
-
-        # x, y = self._as_cartesian_coordinates(rad=r_vals, ang=a_vals)
-        self.obs = pd.DataFrame(
-            np.vstack([a_vals, r_vals]).T, index=t, columns=["alpha", "radius"]
-        )
-        return self.obs
+    return ax
 
 
-class HopfSystem(DynamicalSystem):
-    """
-    Lawrence Perko. Differential equations and dynamical systems, volume 7. Springer Science & Business
-    Media, 2013. page 350
+def plot_eigenvalues_time(
+    time_values: np.ndarray,
+    eigenvalues: np.ndarray,
+    *,
+    system_type="flowmap",
+    delta_time: Optional[float] = None,
+    ax=None,
+    subplots_kwargs=None,
+    plot_kwargs=None,
+):
+    r"""Plot eigenvalues over time.
+
+    The eigenvalues :math:`\lambda_k` (y-axis) are plot with respect to the
+    ``system_type``:
+
+    * "flowmap" - requires to set ``delta_time``
+        .. math::
+            \vert \lambda_k^{t / \Delta t} \vert
+
+    * "differential"
+        .. math::
+            \exp( \lambda_k \cdot t )
+
+    For linear dynamical system, the plot is informative to show the
+    eigenvalues contribution over the time horizon of ``time_values``. Eigenpairs with
+    :math:`\lambda < 1` have a decaying contribution over time, eigenpairs with
+    :math:`\lambda > 1` lead to exponential growth and prohibit long time term
+    predictions.
+
+    Parameters
+    ----------
+    time_values
+        The time values on the x-axis.
+
+    eigenvalues
+        Eigenvalues to plot on the y-axis.
+
+    system_type
+        There are two modes to describe a linear dynamical system (see also
+        :py:class:`.LinearDynamicalSystem`)
+        * "flowmap" - discrete system
+        * "differential" - continuous system
+
+    delta_time
+        Reference system time of type "flowmap".
+
+    ax
+        Matplotlib ``Axes`` object to plot in.
+
+    subplots_kwargs
+        Keyword arguments passed to ``matplotlib.pyplot.subpplot``. Ignored if
+        ``ax`` is not ``None``.
+
+    plot_kwargs
+        Keyword arguments passed to ``ax.plot(**kwargs)``.
+
+    Returns
+    -------
+    matplotlib axes object
 
-    https://link.springer.com/book/10.1007/978-1-4613-0003-8
     """
+    n_timesteps = len(time_values)
 
-    def __init__(self, mu: float = 1, return_xx: bool = True, return_rt: bool = True):
-
-        self.mu = mu
-        self.return_xx = return_xx
-        self.return_rt = return_rt
-
-        if not self.return_xx and not return_rt:
-            raise ValueError("Cannot have both return_xx=False and return_rt=False")
-
-    def hopf_system(self, t, y):
-        """Autonmous, planar ODE System"""
-
-        y_dot = np.zeros(2)
-        factor = self.mu - y[0] ** 2 - y[1] ** 2
-
-        y_dot[0] = -y[1] + y[0] * factor
-        y_dot[1] = y[0] + y[1] * factor
-        return y_dot
-
-    def predict(self, initial_conditions, time_values, ic_type="xx"):
-
-        assert ic_type in ["xx", "rt"]
-        assert initial_conditions.ndim == 2
-        assert initial_conditions.shape[1] == 2
-
-        if ic_type == "rt":
-            new_ic = np.copy(initial_conditions)
-            new_ic[:, 0] = initial_conditions[:, 0] * np.cos(initial_conditions[:, 1])
-            new_ic[:, 1] = initial_conditions[:, 0] * np.sin(initial_conditions[:, 1])
-            initial_conditions = new_ic
-
-        tsc_dfs = []
-
-        for _id, ic in enumerate(initial_conditions):
-            solution = solve_ivp(
-                self.hopf_system,
-                t_span=(time_values[0], time_values[-1]),
-                y0=ic,
-                t_eval=time_values,
-            )
-            current_solution = solution["y"].T
-            theta = np.arctan2(current_solution[:, 1], current_solution[:, 0])
-            radius = current_solution[:, 0] / np.cos(theta)
-
-            current_solution = np.column_stack([current_solution, radius, theta])
-
-            solution = pd.DataFrame(
-                data=current_solution,
-                index=pd.MultiIndex.from_arrays(
-                    [np.ones(len(solution["t"])) * _id, solution["t"]]
-                ),
-                columns=["x1", "x2", "r", "theta"],
+    if system_type == "flowmap":
+        if delta_time is None:
+            raise ValueError(
+                "For 'system_type=flowmap', the parameter 'delta_time' must be provided."
             )
 
-            tsc_dfs.append(solution)
-
-        result = pd.concat(tsc_dfs, axis=0)
-
-        if not self.return_xx:
-            result = result.drop(["x1", "x2"], axis=1)
-        elif not self.return_rt:
-            result = result.drop(["r", "theta"], axis=1)
-
-        # TODO: return as TSCDataFrame
-        return result
-
-
-class ClosedPeriodicalCurve(DynamicalSystem):
-    def __init__(self, consts=(3, 1, 1, 5, 2), noise_std=0):
-        assert len(consts) == 5
-        self.consts = consts
-        self.noise = noise_std
-
-    def _closed_system(self, t_eval):
-
-        if self.noise > 0:
-            noise_x = np.random.default_rng(1).normal(0, self.noise, size=len(t_eval))
-            noise_y = np.random.default_rng(2).normal(0, self.noise, size=len(t_eval))
-            noise_z = np.random.default_rng(3).normal(0, self.noise, size=len(t_eval))
-        else:
-            noise_x, noise_y, noise_z = [0, 0, 0]
-
-        x = noise_x + np.sin(self.consts[0] * t_eval) * np.cos(self.consts[1] * t_eval)
-        y = noise_y + np.sin(self.consts[2] * t_eval) * np.sin(self.consts[3] * t_eval)
-        z = noise_z + np.sin(self.consts[4] * t_eval)
-
-        return pd.DataFrame(
-            np.column_stack([x, y, z]), index=t_eval, columns=["x", "y", "z"]
+        values_matrix = np.abs(
+            np.power(
+                np.outer(eigenvalues, np.ones(n_timesteps)),
+                time_values[np.newaxis, :] / delta_time,
+            )
+        )
+    elif system_type == "differential":
+        values_matrix = np.abs(np.exp(np.outer(eigenvalues, time_values)))
+    else:
+        raise ValueError(
+            f"system_type={system_type} not known. Choose between "
+            f"[flowmap, differential]."
         )
 
-    def predict(self, initial_conditions, time_values, **kwargs):
-        assert initial_conditions is None
-        return self._closed_system(time_values)
+    if ax is None:
+        f, ax = plt.subplots(**({} if subplots_kwargs is None else subplots_kwargs))
 
+    plot_kwargs = plot_kwargs or {}
+    plot_kwargs.setdefault("linestyle", "-")
+    plot_kwargs.setdefault("color", "black")
+
+    ax.plot(time_values, values_matrix.T, **plot_kwargs)
+
+    with plt.rc_context(rc={"text.usetex": True}):
+        ax.set_xlabel("time ($t$)")
+
+        if system_type == "flowmap":
+            ax.set_ylabel("$\\vert \\lambda^{t / \\Delta t} \\vert$")
+        else:  # continuous
+            ax.set_ylabel("$\\vert \\exp(\\lambda \\cdot t) \\vert$")
+
+    return ax
+
+
+def plot_pairwise_eigenvector(
+    eigenvectors: np.ndarray,
+    n: int,
+    idx_start=0,
+    label=r"\Psi",
+    scatter_params: Optional[dict] = None,
+    fig_params: Optional[dict] = None,
+):
+    """Plot scatter plot of n-th eigenvector on x-axis and remaining eigenvectors on
+    y-axis.
+
+    Parameters
+    ----------
+    eigenvectors
+        Eigenvectors of the kernel matrix of shape `(n_samples, n_eigenvectors)`. The
+        eigenvectors are assumed to be sorted by the index.
+
+    n
+        eigenvector index (in columns) to plot on x-axis
+
+    idx_start
+        is the eigenvector index of the first columns (useful when trivial constant
+        eigenvectors are removed before, then set `idx_start=1`).
 
-class Pendulum(DynamicalSystem):
-    """
-    System explained:
-    https://towardsdatascience.com/a-beginners-guide-to-simulating-dynamical-systems-with-python-a29bc27ad9b1
+    scatter_params
+        keyword arguments handled to  `matplotlib.pyplot.scatter()`
 
+    fig_params
+        keyword arguments handled to `matplotlib.pyplot.figure()`
     """
+    eigenvectors = np.asarray(eigenvectors)
 
-    def __init__(self, mass_kg=1, length_rod_m=1, friction=0, gravity=9.81):
-        self.mass_kg = mass_kg
-        self.rod_length_m = length_rod_m
-        self.friction = friction
-        self.gravity = gravity
+    # -1 because the trivial case "n versus n" is skipped
+    n_eigenvectors = eigenvectors.shape[1] - 1
 
-    def _integrate_pendulum_sim(self, theta_init, t):
-        theta_dot_1 = theta_init[1]
-        theta_dot_2 = -self.friction / self.mass_kg * theta_init[
-            1
-        ] - self.gravity / self.rod_length_m * np.sin(theta_init[0])
-        return theta_dot_1, theta_dot_2
+    fig_params = {} if fig_params is None else fig_params
 
-    def _compute_cart_parameters(self):
+    ncols = fig_params.pop("ncols", 2)
+    nrows = fig_params.pop("nrows", int(np.ceil(n_eigenvectors / 2)))
+    sharex = fig_params.pop("sharex", True)
+    sharey = fig_params.pop("sharey", True)
 
-        # 10 * circle_area = mass -- the 10 is artificial
-        self.radius_mass_ = np.sqrt(self.mass_kg / np.pi) / 10
+    f, ax = plt.subplots(
+        nrows=nrows, ncols=ncols, sharex=sharex, sharey=sharey, **fig_params
+    )
 
-        self.fixation_point_ = np.array([0, self.rod_length_m], dtype=float)
-        self.equilibrium_point_ = np.array([0, 0])
+    correct_one = 0
 
-    def _convert_cartesian(self, theta_position):
-        x = self.rod_length_m * np.cos(theta_position - np.pi / 2)
-        y = self.rod_length_m * np.sin(theta_position - np.pi / 2)
-
-        return self.fixation_point_ + np.column_stack([x, y])
-
-    def predict(self, initial_conditions, time_values, **kwargs):
-        # initial_conditions = theta_0 -- theta_1
-
-        self._compute_cart_parameters()
+    for i, idx_eigvec in enumerate(range(n_eigenvectors + 1)):
+        if i == n:
+            correct_one = 1
+            continue
+        else:
+            i = i - correct_one
 
-        initial_conditions = np.asarray(initial_conditions)
+        current_row = i // ncols
+        current_col = i - current_row * ncols
 
-        if initial_conditions.ndim == 1:
-            initial_conditions = initial_conditions[np.newaxis, :]
+        if nrows == 1:
+            _ax = ax[current_col]
+        elif ncols == 1:
+            _ax = ax[current_row]
+        else:
+            _ax = ax[current_row, current_col]
 
-        solution_frames = []
+        _ax.scatter(
+            eigenvectors[:, n],
+            eigenvectors[:, idx_eigvec],
+            **{} if scatter_params is None else scatter_params,
+        )
 
-        for ic_idx in range(initial_conditions.shape[0]):
-            theta_coord = odeint(
-                self._integrate_pendulum_sim, initial_conditions[ic_idx, :], time_values
-            )
+        _ax.set_title(
+            rf"${label}_{{{n + idx_start}}}$ vs. ${label}_{{{idx_eigvec + idx_start}}}$"
+        )
 
-            cartesian_coord = self._convert_cartesian(theta_coord[:, 0].copy())
+    return f, ax
 
-            theta_coord = pd.DataFrame(
-                theta_coord, index=time_values, columns=["theta", "dot_theta"]
-            )
-            cartesian_coord = pd.DataFrame(
-                cartesian_coord, index=time_values, columns=["x", "y"]
-            )
 
-            solution_frames.append(pd.concat([theta_coord, cartesian_coord], axis=1))
+@warn_experimental_function
+def plot_scales(pcm, scale_range=(1e-5, 1e3), n_scale_tests=20) -> None:
+    """Plots for varying scales.
 
-        tsc_df = TSCDataFrame.from_frame_list(solution_frames)
+    .. warning::
 
-        return tsc_df
+    Parameters
+    ----------
+    pcm
+        point cloud manifold
 
+    scale_range
+        lower and upper limit of scale
 
-# TODO:
-#  include benchmark systems from: https://arxiv.org/pdf/2008.12874.pdf
-
-
-# if __name__ == "__main__":
-#
-#     from datafold.dynfold import DiffusionMaps
-#     from datafold.pcfold import GaussianKernel
-#     from datafold.utils.plot import plot_pairwise_eigenvector
-#
-#     import matplotlib.pyplot as plt
-#     from datafold.pcfold import TSCDataFrame
-#     from mpl_toolkits.mplot3d import Axes3D
-#
-#     t_eval = np.sort(np.random.default_rng(1).uniform(0, np.pi, size=(1000,)))
-#     t_eval_oos = np.linspace(0, np.pi, 5000)
-#     X = ClosedPeriodicalCurve((3, 1, 1, 5, 2), noise_std=0.05).eval(None, t_eval=t_eval)
-#     X_oos = ClosedPeriodicalCurve((3, 1, 1, 5, 2)).eval(None, t_eval=t_eval_oos)
-#
-#     X = TSCDataFrame.from_single_timeseries(X)
-#     X_oos = TSCDataFrame.from_single_timeseries(X_oos)
-#
-#     fig = plt.figure()
-#     ax = fig.gca(projection="3d")
-#     ax.scatter(
-#         X["x"].to_numpy().ravel(),
-#         X["y"].to_numpy().ravel(),
-#         X["z"].to_numpy().ravel(),
-#         label="parametric curve",
-#         c=t_eval,
-#         cmap=plt.cm.Spectral,
-#     )
-#     ax.legend()
-#
-#     dmap = DiffusionMaps(
-#         kernel=GaussianKernel(epsilon=0.01),
-#         n_eigenpairs=5,
-#         # dist_kwargs=dict(cut_off=0.2),
-#     ).fit(X)
-#
-#     Y = dmap.transform(X)
-#     Y_oos = dmap.transform(X_oos)
-#
-#     f, ax = plt.subplots()
-#
-#     ax.scatter(
-#         Y["dmap1"].to_numpy(), Y["dmap2"].to_numpy(), c=t_eval, cmap=plt.cm.Spectral,
-#     )
-#
-#     ax.axis("equal")
-#
-#     f, ax = plt.subplots()
-#
-#     ax.scatter(
-#         Y_oos["dmap1"].to_numpy(),
-#         Y_oos["dmap2"].to_numpy(),
-#         c=t_eval_oos,
-#         cmap=plt.cm.Spectral,
-#     )
-#     ax.axis("equal")
-#
-#     Y_oos.loc[:, ("dmap1", "dmap2")].plot()
-#
-#     # plot_pairwise_eigenvector(
-#     #     dmap.eigenvectors_, n=1, scatter_params=dict(c=t_eval, cmap=plt.cm.Spectral)
-#     # )
-#
-#     plt.show()
+    n_scale_tests
+        number of points
+    """
+    scales = np.exp(
+        np.linspace(np.log(scale_range[0]), np.log(scale_range[1]), n_scale_tests)
+    )
+    scale_sum = np.zeros_like(scales)
+
+    distance_matrix = pcm.compute_distance_matrix()
+
+    fig, ax = plt.subplots(1, 1, figsize=(6, 4))
+
+    save_eps = pcm.kernel.epsilon
+
+    for i, scale in enumerate(scales):
+        pcm.kernel.epsilon = scale
+        kernel_matrix_scale = pcm.kernel.evaluate(distance_matrix=distance_matrix)
+        kernel_sum = kernel_matrix_scale.sum()
+
+        scale_sum[i] = kernel_sum / (kernel_matrix_scale.shape[0] ** 2)
+
+    # ax.loglog(scales, scale_sum, 'k-', label='points')
+    pcm.kernel.epsilon = save_eps
+
+    gradient = np.exp(
+        np.gradient(np.log(scale_sum), np.log(scales)[1] - np.log(scales)[0])
+    )
+    ax.semilogx(scales, gradient, "k-", label="points")
+
+    igmax = np.argmax(gradient)
+
+    eps = scales[igmax]
+    dimension = gradient[igmax] - 1 / 2
+
+    ax.semilogx(
+        [scales[igmax], scales[igmax]],
+        [np.min(gradient), np.max(gradient)],
+        "r-",
+        label=r"max at $\epsilon=%.5f$" % (eps),
+    )
+    ax.semilogx(
+        [np.min(scales), np.max(scales)],
+        [gradient[igmax], gradient[igmax]],
+        "b-",
+        label=r"dimension $\approx %.1f$" % (dimension),
+    )
+
+    ax.set_xlabel(r"$\epsilon$")
+    ax.set_ylabel(r"$\mathbb{E}_\epsilon$")
+    # ax.loglog(scales, 1*scales, 'r--', label='dim=1')
+    # ax.loglog(scales, 2*scales, 'g--', label='dim=2')
+    ax.legend()
+    fig.tight_layout()
```

### Comparing `datafold-1.1.6/datafold/utils/general.py` & `datafold-2.0.0/datafold/utils/general.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
-import warnings
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Union
 
 import numpy as np
 import numpy.testing as nptest
 import pandas as pd
 import pandas.testing as pdtest
 import scipy.sparse
-from sklearn.utils.validation import check_array, check_scalar
+from sklearn.utils.validation import check_scalar
 
 
 def series_if_applicable(ds: Union[pd.Series, pd.DataFrame]):
     """Turns a DataFrame with only one column into a :class:`pandas.Series`."""
     import datafold.pcfold
 
     if isinstance(ds, pd.Series):
@@ -46,30 +45,30 @@
 
 def is_df_same_index(
     df_left: pd.DataFrame,
     df_right: pd.DataFrame,
     check_index=True,
     check_column=True,
     check_names=True,
-    handle="raise",
+    handle: Optional[str] = "raise",
 ):
-
+    """Check that two data frames have the same properties (index, columns, names)."""
     assert check_index + check_column >= 1
 
     is_index_same = True
     is_columns_same = True
 
     if check_index:
         try:
             pdtest.assert_index_equal(
                 df_left.index, df_right.index, check_names=check_names
             )
-        except AssertionError:
+        except AssertionError as e:
             if handle == "raise":
-                raise
+                raise e
             is_index_same = False
 
     if check_column:
         try:
             pdtest.assert_index_equal(
                 df_left.columns, df_right.columns, check_names=check_names
             )
@@ -113,15 +112,14 @@
 
     Returns
     -------
     bool
         True if `n` is a float.
 
     """
-
     return isinstance(n, (float, np.floating))
 
 
 def is_scalar(n: object):
     """Checks if `n` is a scalar.
 
     Parameters
@@ -134,122 +132,220 @@
     bool
         True if `n` is a scalar.
 
     """
     return is_float(n) or is_integer(n)
 
 
+def is_matrix(
+    matrix,
+    name="matrix",
+    square=False,
+    allow_sparse=False,
+    handle: Optional[str] = "raise",
+):
+    # TODO: also include allowed dtype kind?
+    if isinstance(matrix, np.ndarray):
+        if matrix.ndim != 2:
+            if handle == "raise":
+                raise ValueError(
+                    f"The matrix '{name}' must have two dimensions. Got {matrix.ndim=}."
+                )
+            else:
+                return False
+    elif allow_sparse and scipy.sparse.issparse(matrix):
+        pass
+    else:
+        if handle == "raise":
+            raise TypeError(
+                f"The parameter '{name}' is not a valid matrix format. Got {type(matrix)=}."
+            )
+        else:
+            return False
+
+    if square and matrix.shape[0] != matrix.shape[1]:
+        if handle == "raise":
+            raise ValueError(
+                f"The parameter '{name}' must be a square matrix. Got {matrix.shape=}"
+            )
+        else:
+            return False
+
+    return True
+
+
+def is_vector(
+    vector,
+    name="vector",
+    handle: Optional[str] = "raise",
+):
+    if isinstance(vector, np.ndarray):
+        if vector.ndim != 1 or vector.shape[0] < 1:
+            if handle == "raise":
+                raise ValueError(
+                    f"The vector '{name}' must be one dimensional and have at least one "
+                    f"element. Got {vector.ndim=} and {vector.shape=}."
+                )
+            else:
+                return False
+    else:
+        if handle == "raise":
+            raise TypeError(
+                f"The parameter '{name}' is not a valid matrix format. Got {type(vector)=}."
+            )
+        else:
+            return False
+
+    return True
+
+
 def if1dim_colvec(vec: np.ndarray) -> np.ndarray:
     if vec.ndim == 1:
         return vec[:, np.newaxis]
     else:
         return vec
 
 
 def if1dim_rowvec(vec: np.ndarray) -> np.ndarray:
     if vec.ndim == 1:
         return vec[np.newaxis, :]
     else:
         return vec
 
 
-def projection_matrix_from_features(
+def projection_matrix_from_feature_names(
     features_all: pd.Index, features_select: pd.Index
 ) -> scipy.sparse.csr_matrix:
-    r"""Compute a sparse projection matrix that maps that selects columns from a matrix.
+    r"""Compute a sparse projection matrix which maps to selected columns from a matrix.
 
     .. math::
         A \cdot P = A^*
 
     If matrix :math:`A` has a set of features (column-oriented), then the projection
     matrix :math:`P` selects the requested sub-selection of features in matrix
     :math:`A^*` (by performing the matrix multiplication).
 
     Parameters
     ----------
     features_all
-        All features in the original matrix.
+        All original feature names.
 
     features_select
-        The features to include in the final matrix after the projection.
+        The (partial or re-ordered) feature names after the projection
 
     Returns
     -------
     scipy.sparse.csr_matrix
-        The projection matrix.
+        projection matrix
     """
     project_indices = np.where(np.isin(features_all, features_select))[0]
 
     if len(project_indices) != len(features_select):
         raise ValueError(
             "Not all features from 'feature_select' are contained in 'features_all'."
         )
 
     project_matrix = scipy.sparse.lil_matrix((len(features_all), len(features_select)))
     project_matrix[project_indices, np.arange(len(features_select))] = 1
     return project_matrix.tocsr()
 
 
 def sort_eigenpairs(
-    eigenvalues: np.ndarray, eigenvectors: np.ndarray, ascending: bool = False
-) -> Tuple[np.ndarray, np.ndarray]:
-    """Sort eigenpairs according to magnitude (absolute value) of corresponding
+    eigenvalues: np.ndarray,
+    right_eigenvectors: np.ndarray,
+    *,
+    left_eigenvectors=None,
+    ascending: bool = False,
+):
+    r"""Sort eigenpairs according to magnitude (absolute value) of corresponding
     eigenvalue.
 
+    The right eigenvectors :math:`\Psi_r` are given by the standard eigenproblem
+
+    .. math::
+
+        A \Psi_r = \Psi_r \Lambda
+
+    The left eigenvectors :math:`\Psi_l` are from the transposed eigenproblem
+
+    .. math::
+
+        \Psi_l A  = \Lambda \Psi_l
+
+    By convention the right eigenvectors are column wise in :math:`\Psi_r` and the left
+    eigenvectors are column-wise in :math:`\Psi_l`.
+
     Parameters
     ----------
-
     eigenvalues
         complex or real-valued
 
-    eigenvectors
-        vectors, column wise
+    right_eigenvectors
+        vectors, column-wise
+
+    left_eigenvectors
+        vectors, row-wise
 
     ascending
         If True, sort from low magnitude to high magnitude.
 
     Returns
     -------
     Tuple[np.ndarray, np.ndarray]
         sorted eigenvalues and -vectors
     """
-    if eigenvalues.ndim != 1 or eigenvectors.ndim != 2:
+    is_left_eigvec = left_eigenvectors is not None
+
+    if eigenvalues.ndim != 1:
+        raise ValueError("Parameter 'eigenvalues' must be a one dimensional array")
+
+    is_matrix(right_eigenvectors, "right_eigenvectors")
+
+    if is_left_eigvec:
+        is_matrix(left_eigenvectors, "left_eigenvectors")
+
+    if eigenvalues.shape[0] != right_eigenvectors.shape[1]:
         raise ValueError(
-            "eigenvalues have to be 1-dim and eigenvectors "
-            "2-dim np.ndarray respectively"
+            f"The number of eigenvalues (={eigenvalues.shape[0]}) does not match the "
+            f"number of eigenvectors (={right_eigenvectors.shape[1]})"
         )
 
-    if eigenvalues.shape[0] != eigenvectors.shape[1]:
+    if is_left_eigvec and eigenvalues.shape[0] != left_eigenvectors.shape[0]:
         raise ValueError(
-            f"the number of eigenvalues (={eigenvalues.shape[0]}) does not match the "
-            f"number of eigenvectors (={eigenvectors.shape[1]})"
+            f"The number of eigenvalues (={eigenvalues.shape[0]}) does not match the "
+            f"number of left eigenvectors (={left_eigenvectors.shape[0]})"
         )
 
     # Sort eigenvectors according to (complex) value of eigenvalue
     #  -- NOTE: sorting according to complex values is preferred over sorting
     #           absolute complex value here. This is because complex conjugate eigenvalues
     #           have the same absolute value which makes sorting unstable (i.e.
     #           there can be two equivalent absolute values but the associate complex
     #           values are at different places after separate sorting)
     idx = np.argsort(eigenvalues)
 
     if not ascending:
-        # creates a view on array and is most efficient way for reversing order
+        # creates a view on array and is the most efficient way for reversing order
         # see: https://stackoverflow.com/q/6771428
         idx = idx[::-1]
 
-    return eigenvalues[idx], eigenvectors[:, idx]
+    if is_left_eigvec:
+        return eigenvalues[idx], right_eigenvectors[:, idx], left_eigenvectors[idx, :]
+    else:
+        return eigenvalues[idx], right_eigenvectors[:, idx]
 
 
 def mat_dot_diagmat(
-    matrix: np.ndarray, diag_elements: np.ndarray, out: Optional[np.ndarray] = None
-) -> np.ndarray:
-    """Efficient computation of "matrix times diagonal matrix".
+    matrix: Union[np.ndarray, scipy.sparse.spmatrix],
+    diag_elements: np.ndarray,
+    out: Optional[np.ndarray] = None,
+) -> Union[np.ndarray, scipy.sparse.spmatrix]:
+    """Efficient computation of "(sparse/dense) matrix times diagonal matrix".
 
-    This computes
+    Compute the often common but inefficient way
 
     .. code::
         matrix @ np.diag(diag_elements)
 
     by using element-wise computations.
 
     Parameters
@@ -257,174 +353,236 @@
     matrix
         Dense matrix of shape `(I,J)`.
 
     diag_elements
         Diagonal elements in 1 dim. array of `J` elements.
 
     out
-        Select where to write the result. Usual choice is setting it to the full matrix
-        input for better memory efficient.
+        Select NumPy ndarray (with shape ``(I,J)`` to write the result into. A usual choice is
+        setting it to the same matrix as in the argument input. This can improve memory
+        efficient as no new memory needs to be allocated. Ignored if matrix is sparse.
 
     Returns
     -------
     """
-    assert diag_elements.ndim == 1 and matrix.ndim == 2
-    return np.multiply(diag_elements, matrix, out=out)
+    assert diag_elements.ndim == 1 and is_matrix(matrix, "matrix", allow_sparse=True)
 
+    if scipy.sparse.issparse(matrix):
+        # out is ignored here, because it is not supported by scipy sparse
+        return matrix @ scipy.sparse.diags(diagonals=diag_elements)
+    else:
+        return np.multiply(diag_elements, matrix, out=out)
 
-def diagmat_dot_mat(diag_elements: np.ndarray, matrix: np.ndarray, out=None):
-    """Efficient computation of "diagonal matrix times matrix".
 
-    This computes
+def diagmat_dot_mat(
+    diag_elements: Union[np.ndarray, scipy.sparse.spmatrix],
+    matrix: np.ndarray,
+    out=None,
+) -> Union[np.ndarray, scipy.sparse.spmatrix]:
+    """Efficient computation of "diagonal matrix times (sparse/dense) matrix".
+
+    Compute the often common but inefficient way
 
     .. code::
         np.diag(diag_elements) @ matrix
 
     by using element-wise computations.
 
     Parameters
     ----------
     diag_elements
-         Diagonal elements in 1 dim. array of `I` elements.
+         Diagonal elements in 1 dim. array of ``I`` elements.
 
     matrix
-        Dense matrix of shape `(I,J)`.
+        Dense matrix of shape ``(I,J)``.
 
     out
-        Select where to write the result. Usual choice is setting it to the full matrix
-        input for better memory efficient.
+        Select NumPy ndarray (with shape ``(I,J)`` to write the result into. A usual choice is
+        setting it to the same matrix as in the argument input. This can improve memory
+        efficient as no new memory needs to be allocated. Ignored if matrix is sparse.
 
     Returns
     -------
     """
-    assert diag_elements.ndim == 1 and matrix.ndim == 2
-    return np.multiply(matrix, diag_elements[:, np.newaxis], out=out)
+    assert diag_elements.ndim == 1 and is_matrix(matrix, "matrix", allow_sparse=True)
+
+    if scipy.sparse.issparse(matrix):
+        # out is not supported by scipy sparse dot
+        # sparse.diags does not fill memory with zeros
+        return scipy.sparse.diags(diag_elements) @ matrix
+    else:
+        return np.multiply(matrix, diag_elements[:, np.newaxis], out=out)
+
+
+def generate_2d_regular_mesh(
+    low=(-1, -1), high=(1, 1), n_xvalues=10, n_yvalues=10, feature_names=None
+):
+    x_values = np.linspace(low[0], high[0], num=n_xvalues)
+    y_values = np.linspace(low[1], high[1], num=n_yvalues)
+
+    x_mesh, y_mesh = np.meshgrid(x_values, y_values)
+    X = np.column_stack((x_mesh.ravel(), y_mesh.ravel()))
+
+    if feature_names is not None:
+        # import here to avoid circular imports
+        from datafold import InitialCondition
+
+        X = InitialCondition.from_array(X, time_value=0, feature_names=feature_names)
+
+    return X
 
 
 def df_type_and_indices_from(
     indices_from: pd.DataFrame,
     values: Union[np.ndarray, pd.DataFrame],
-    except_index: Optional[Union[pd.Index, List[str]]] = None,
-    except_columns: Optional[Union[pd.Index, List[str]]] = None,
+    except_index: Optional[Union[pd.Index, list[str]]] = None,
+    except_columns: Optional[Union[pd.Index, list[str]]] = None,
 ):
     # import here to prevent circular imports
     from datafold.pcfold import TSCDataFrame
 
     if except_index is not None and except_columns is not None:
         raise ValueError(
-            "'except_index' and 'except_columns' are both given. "
-            "Cannot copy neither index nor column from existing TSCDataFrame if both "
-            "is excluded."
+            "Both parameters 'except_index' and 'except_columns' are provided. For this "
+            "function provide none or one of the optional parameters."
         )
 
     # view input as array (allows for different input, which is
     # compatible with numpy.ndarray
     values = np.asarray(values)
 
     if except_index is None:
-        index = indices_from.index  # type: ignore  # mypy cannot infer type here
+        index = indices_from.index
     else:
         index = except_index
 
     if except_columns is None:
         columns = indices_from.columns
     else:
         columns = except_columns
 
     if isinstance(indices_from, TSCDataFrame):
         return TSCDataFrame(data=values, index=index, columns=columns)
     elif isinstance(indices_from, pd.DataFrame):
         return pd.DataFrame(data=values, index=index, columns=columns)
     else:
-        raise TypeError(
-            f"The argument type 'type(indices_from)={type(indices_from)} is invalid."
-        )
+        raise TypeError(f"The argument type {type(indices_from)=} is invalid.")
 
 
 def is_symmetric_matrix(
     matrix: Union[np.ndarray, scipy.sparse.csr_matrix], tol: float = 0
 ) -> bool:
-    """Checks whether a matrix is symmetric.
+    """Check whether a matrix is symmetric.
 
     Parameters
     ----------
     matrix
        A square matrix to be checked for symmetry.
     tol
-       The maximum allowed absolute deviation between corresponding elements.
+       The tolerance of absolute deviation between corresponding elements
+       (k[i,j] and k[j,i]).
 
     Returns
     -------
     bool
-        True if symmetric.
+        True if symmetric else False.
     """
-
-    if matrix.ndim != 2:
-        raise ValueError("matrix has to be 2-dim.")
-    if matrix.shape[0] != matrix.shape[1]:
-        raise ValueError("matrix has to be square")
-
+    is_matrix(matrix, "matrix", square=True, allow_sparse=True)
     max_abs_deviation = np.max(np.abs(matrix - matrix.T))
     return max_abs_deviation <= tol
 
 
+def is_stochastic_matrix(
+    matrix: Union[np.ndarray, scipy.sparse.csr_matrix], axis=1, tol=1e-15
+) -> bool:
+    """Check whether a matrix is stochastic.
+
+    A matrix is stochastic if either the columns (axis=1) or the rows (axis=0) sum up to 1.
+
+    Parameters
+    ----------
+    matrix
+         The matrix to be checked for stochasticity.
+
+    axis
+       The axis along which to check the stochasticity (0 or row and 1 for column).
+
+    tol
+       The tolerance of absolute deviation from the row or column sum from 1.
+
+    Returns
+    -------
+    bool
+        True if matrix is stochastic else False
+    """
+    is_matrix(matrix, "matrix", allow_sparse=True)
+
+    sum_array = matrix.sum(axis=axis)
+
+    if scipy.sparse.issparse(matrix):
+        sum_array = sum_array.A1
+
+    return (np.abs(sum_array - 1) <= tol).all()
+
+
 def remove_numeric_noise_symmetric_matrix(
     matrix: Union[np.ndarray, scipy.sparse.spmatrix]
 ) -> Union[np.ndarray, scipy.sparse.spmatrix]:
     r"""Remove numerical noise from (almost) symmetric matrix.
 
     Even symmetric operations can sometimes introduce noise. The
     operations are often executed in different order, for example, evaluations such as in
 
     .. math::
-        D^{-1} M D^{-1}
 
-    where :math:`D` is a diagonal matrix. This can then break the exact floating point
-    symmetry in the matrix.
+        D^{-1} M D^{-1},
 
-    This function is intended to make recover an exact symmetry of "almost" symmetric
-    matrices, such as in the following situation:
+    where :math:`D` is a diagonal matrix can break exact floating point symmetry in a
+    symmetric matrix :math:`M`.
+
+    This function recovers an exact symmetry of an "almost symmetric" matrix, such as in the
+    following situation:
 
     .. code::
         np.max(np.abs(matrix - matrix.T)) # 1.1102230246251565e-16
 
-    The symmetry is removed with:
+    The symmetry is recovered with:
 
     .. math::
         M_{sym} = \frac{M + M^T}{2}
 
     Parameters
     ----------
     matrix
         square matrix (dense/sparse) to remove numerical noise from
 
     Returns
     -------
     Union[numpy.ndarray, scipy.sparse.csr_matrix]
         symmetric matrix without noise
     """
-
-    # A faster way would be to truncate the floating values of the matrix to a certain
-    # precision, but NumPy does not seem to provide anything for this?
+    is_matrix(matrix, "matrix", square=True, allow_sparse=True)
 
     if scipy.sparse.issparse(matrix):
-        # need to preserve of explicit stored zeros (-> distance matrix)
+        # need to preserve stored zeros (e.g. in case of distance matrices)
+        # NOTE: there is no check that the sparse structure is symmetric, this leads to
+        # wrong results if the symmetric value of a (non-negative) value is not there.
         matrix.data[matrix.data == 0] = np.nan
         matrix = (matrix + matrix.T) / 2.0
         matrix.data[np.isnan(matrix.data)] = 0
     else:
         matrix = np.add(matrix, matrix.T, out=matrix)
         matrix = np.divide(matrix, 2.0, out=matrix)
 
     return matrix
 
 
 def random_subsample(
     data: np.ndarray, n_samples: int, random_state: Optional[int] = None
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Random uniform subsample without replacement of data.
 
     Parameters
     ----------
     data
         point cloud
 
@@ -439,29 +597,23 @@
     -------
     numpy.ndarray
         subsampled array
 
     numpy.ndarray
         indices in the subsample from the original array
     """
-
-    data = check_array(
-        data,
-        force_all_finite=False,
-        ensure_min_samples=2,
-    )
-    assert isinstance(data, np.ndarray)  # for mypy
+    is_matrix(data, "data", allow_sparse=False)
 
     n_samples_data = data.shape[0]
 
     check_scalar(
         n_samples,
         name="n_samples",
         target_type=int,
         min_val=1,
         max_val=n_samples_data - 1,
     )
 
-    indices = np.random.default_rng(seed=random_state).permutation(n_samples_data)[
-        :n_samples
-    ]
+    indices = np.random.default_rng(seed=random_state).permutation(n_samples_data)
+    indices = indices[:n_samples]
+
     return data[indices, :], indices
```

### Comparing `datafold-1.1.6/datafold.egg-info/PKG-INFO` & `datafold-2.0.0/datafold.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,268 +1,270 @@
 Metadata-Version: 2.1
 Name: datafold
-Version: 1.1.6
+Version: 2.0.0
 Summary: Operator-theoretic models to identify dynamical systems and parametrize point cloud geometry
 Home-page: https://datafold-dev.gitlab.io/datafold
+Download-URL: https://pypi.org/project/datafold/
 Author: datafold development team
-Author-email: daniel.lehmberg@hm.edu
+Author-email: d.lehmberg@tum.de
 License: MIT
-Download-URL: https://pypi.org/project/datafold/
-Description: Quick links
-        ^^^^^^^^^^^
-        
-        `Source repository <https://gitlab.com/datafold-dev/datafold>`__ |
-        `Contributing and feedback <https://datafold-dev.gitlab.io/datafold/contributing.html>`__ |
-        `PyPI <https://pypi.org/project/datafold/>`__ |
-        `Documentation <https://datafold-dev.gitlab.io/datafold/>`__ |
-        `Tutorials <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__ |
-        `Scientific literature <https://datafold-dev.gitlab.io/datafold/references.html>`__
-        
-        What is *datafold*?
-        ====================
-        
-        *datafold* is a `MIT-licensed <https://gitlab.com/datafold-dev/datafold/-/blob/master/LICENSE>`__
-        Python package containing operator-theoretic, data-driven models to identify dynamical
-        systems from time series data and to infer geometrical structures in point clouds.
-        
-        The package includes:
-        
-        * Data structures to handle point clouds on manifolds (``PCManifold``) and time series
-          collections (``TSCDataFrame``). The data structures are used both internally and for
-          model input/outputs. In contrast to solutions found in other projects, such as
-          lists of Numpy arrays, ``TSCDataFrame`` makes it much easier to describe many forms of
-          time series data in a single object.
-        * An efficient implementation of the ``DiffusionMaps`` model to infer geometric
-          meaningful structures from data, such as the eigenfunctions of the
-          Laplace-Beltrami operator. As a distinguishing factor to other implementations, the
-          model can handle a sparse kernel matrix and allows setting an arbitrary kernel,
-          including the standard Gaussian kernel,
-          `continuous k-nearest neighbor kernel <https://arxiv.org/abs/1606.02353>`__, or
-          `dynamics-adapted cone kernel <https://cims.nyu.edu/~dimitris/files/Giannakis15_cone_kernels.pdf>`__.
-        * Out-of-sample extensions for the Diffusion Maps model, such as the (auto-tuned)
-          Laplacian Pyramids or Geometric Harmonics to interpolate general function values on a
-          point cloud manifold.
-        * An implementation of the (Extended-) Dynamic Mode Decomposition (e.g. model ``DMDFull``
-          or ``EDMD``) as data-driven methods to identify dynamical systems from time series
-          collection data. ``EDMD`` subclasses from the flexible scikit-learn
-          `Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`__,
-          which allows setting up and transforming time series collection data to a more suitable
-          feature state (cf. Koopman operator theory).
-        * ``EDMDCV`` allows model parameters to be optimized with cross-validation splittings that
-          account for the temporal order in time series collections.
-        
-        See also `this introduction page <https://datafold-dev.gitlab.io/datafold/intro.html>`__.
-        For a mathematical thorough introduction, we refer to the `scientific literature
-        <https://datafold-dev.gitlab.io/datafold/references.html>`__.
-        
-        .. note::
-            The project is under active development in a research-driven environment.
-        
-            * Code quality varies from "experimental/early stage" to "well-tested". Well tested
-              code is listed in the
-              `software documentation <https://datafold-dev.gitlab.io/datafold/api.html>`__
-              and are directly accessible through the package levels ``pcfold``, ``dynfold`` or
-              ``appfold`` (e.g. :code:`from datafold.dynfold import ...`). Experimental code is
-              only accessible via "deep imports"
-              (e.g. :code:`from datafol.dynfold.outofsample import ...`) and may raise a warning
-              when using it.
-            * There is no deprecation cycle. Backwards compatibility is indicated by the
-              package version, where we use a `semantic versioning <https://semver.org/>`__
-              policy `[major].[minor].[patch]`, i.e.
-        
-                 * `major` - making incompatible changes in the (documented) API
-                 * `minor` - adding functionality in a backwards-compatible manner
-                 * `patch` - backwards-compatible bug fixes
-        
-              We do not intend to indicate a feature complete milestone with version `1.0`.
-        
-        
-        Cite
-        ====
-        
-        If you use *datafold* in your research, please cite
-        `this paper <https://joss.theoj.org/papers/10.21105/joss.02283>`__ published in the
-        *Journal of Open Source Software* (`JOSS <https://joss.theoj.org/>`__).
-        
-        *Lehmberg et al., (2020). datafold: data-driven models for point clouds and time series on
-        manifolds. Journal of Open Source Software, 5(51), 2283,* https://doi.org/10.21105/joss.02283
-        
-        BibTeX:
-        
-        .. code-block:: latex
-        
-            @article{Lehmberg2020,
-                     doi       = {10.21105/joss.02283},
-                     url       = {https://doi.org/10.21105/joss.02283},
-                     year      = {2020},
-                     publisher = {The Open Journal},
-                     volume    = {5},
-                     number    = {51},
-                     pages     = {2283},
-                     author    = {Daniel Lehmberg and Felix Dietrich and Gerta K{\"o}ster and Hans-Joachim Bungartz},
-                     title     = {datafold: data-driven models for point clouds and time series on manifolds},
-                     journal   = {Journal of Open Source Software}}
-        
-        How to get it?
-        ==============
-        
-        Installation requires `Python>=3.7 <https://www.python.org/>`__ with
-        `pip <https://pip.pypa.io/en/stable/>`__ and
-        `setuptools <https://setuptools.readthedocs.io/en/latest/>`__ installed. Both
-        packages usually ship with a standard Python installation. The package dependencies
-        install automatically. The main dependencies and their role in *datafold* are listed below
-        in "Dependencies".
-        
-        There are two ways to install *datafold*:
-        
-        1. From PyPI
-        ------------
-        
-        This is the standard way for users. The package is hosted on the official Python package
-        index (PyPI) and installs the core package (excluding tutorials and tests). The tutorial
-        files can be downloaded separately
-        `here <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__.
-        
-        To install the package and its dependencies with :code:`pip`, run
-        
-        .. code-block:: bash
-        
-           python -m pip install datafold
-        
-        .. note::
-        
-            If you run Python in an Anaconda environment you can use pip from within ``conda``.
-            See also
-            `official instructions <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages>`__.
-        
-            .. code-block:: bash
-        
-                conda activate venv
-                conda install pip
-                pip install datafold
-        
-        
-        2. From source
-        --------------
-        
-        This way is recommended if you want to access the latest (but potentially unstable)
-        development, run tests or wish to contribute (see section "Contributing" for details).
-        Download or git-clone the source code repository.
-        
-        1. Download the repository
-        
-           a. If you wish to contribute code, it is required to have
-              `git <https://git-scm.com/>`__ installed. Clone the repository with
-        
-              .. code-block:: bash
-        
-                git clone https://gitlab.com/datafold-dev/datafold.git
-        
-           b. If you only want access to the source code (current ``master`` branch), download one
-              of the compressed files
-              (`zip <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.zip>`__,
-              `tar.gz <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.gz>`__,
-              `tar.bz2 <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.bz2>`__,
-              `tar <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar>`__)
-        
-        2. Install the package from the downloaded repository
-        
-           .. code-block:: bash
-        
-               python -m pip install .
-        
-        
-        Contributing
-        ============
-        
-        Any contribution (code/tutorials/documentation improvements), question or feedback is
-        very welcome. Either use the
-        `issue tracker <https://gitlab.com/datafold-dev/datafold/-/issues>`__ or
-        `Email <incoming+datafold-dev-datafold-14878376-issue-@incoming.gitlab.com>`__.
-        Instructions to set up *datafold* for development can be found
-        `here <https://datafold-dev.gitlab.io/datafold/contributing.html>`__.
-        
-        Dependencies
-        ============
-        
-        The dependencies of the core package are managed in the file
-        `requirements.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements.txt>`__
-        and install with *datafold*. The tests, tutorials, documentation and code analysis
-        require additional dependencies which are managed in
-        `requirements-dev.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements-dev.txt>`__.
-        
-        *datafold* integrates with common packages from the
-        `Python scientific computing stack <https://www.scipy.org/about.html>`__:
-        
-        * `NumPy <https://numpy.org/>`__
-           The data structure ``PCManifold`` subclasses from NumPy's
-           `ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`__. The
-           class attaches an kernel object to the data to describe point similarity.
-           NumPy is used throughout *datafold* and is the default package for numerical
-           data and algorithms.
-        
-        * `pandas <https://pandas.pydata.org/pandas-docs/stable/index.html>`__
-           *datafold* uses pandas'
-           `DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`__
-           as a base class for ``TSCDataFrame``, which captures time series data and
-           collections thereof. The data structure indexes time, time series ID and
-           one-or-many spatial features. It includes specific time series collection functionality
-           and is compatible with pandas rich functionality.
-        
-        * `scikit-learn <https://scikit-learn.org/stable/>`__
-           All *datafold* algorithms that are part of the "machine learning pipeline" align
-           to the scikit-learn `API <https://scikit-learn.org/stable/developers/develop.html>`__.
-           This is done by deriving the models from
-           `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
-           and appropriate `MixIns`. *datafold* defines own `MixIns` that align with the
-           API in a duck-typing fashion to allow identifying dynamical systems from temporal data
-           in ``TSCDataFrame``.
-        
-        * `SciPy <https://docs.scipy.org/doc/scipy/reference/index.html>`__
-           The package is used for elementary numerical algorithms and data structures in
-           conjunction with NumPy. This includes (sparse) linear least
-           square regression, (sparse) eigenpairs solver and sparse matrices as
-           optional data structure for kernel matrices.
-        
-        How does it compare to other software?
-        ======================================
-        
-        *The selection only includes other Python packages.*
-        
-        * `scikit-learn <https://scikit-learn.org/stable/>`__
-           provides algorithms and models along the entire machine learning pipeline, with a
-           strong focus on static data (i.e. without temporal context). *datafold* integrates
-           into scikit-learn' API and all data-driven models are subclasses of
-           `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
-           An important contribution of *datafold* is the ``DiffusionMaps`` model as popular
-           framework for manifold learning, which is not contained in scikit-learn's `set of
-           algorithms <https://scikit-learn.org/stable/auto_examples/manifold/plot_compare_methods
-           .html#sphx-glr-auto-examples-manifold-plot-compare-methods-py>`__.
-           Furthermore, *datafold* includes dynamical systems as a new model class that is
-           operable with scikit-learn - the attributes align to supervised learning tasks.
-           The key differences are that a model processes data of type ``TSCDataFrame``
-           and instead of a one-to-one relation in the model's input/output, the model can return
-           arbitrary many output samples (a time series) for a single input
-           (an initial condition).
-        
-        * `PyDMD <https://mathlab.github.io/PyDMD/build/html/index.html>`__
-           provides many variants of the `Dynamic Mode Decomposition (DMD) <https://en.wikipedia.org/wiki/Dynamic_mode_decomposition>`__.
-           *datafold* provides a wrapper to make models of ``PyDMD`` accessible. However, a
-           limitation of ``PyDMD`` is that it only processes single coherent time series, see
-           `PyDMD issue 86 <https://github.com/mathLab/PyDMD/issues/86>`__. The DMD models that
-           are directly included in *datafold* utilize the functionality of the data
-           structure ``TSCDataFrame`` and can therefore process time
-           series collections - in an extreme case only containing snapshot pairs.
-        
-        * `PySINDy <https://pysindy.readthedocs.io/en/latest/>`__
-           specializes on a *sparse* system identification of nonlinear dynamical systems to
-           infer governing equations.
-        
 Keywords: mathematics, machine learning, dynamical system, data-driven, time series, regression, forecasting, manifold learning, diffusion map, koopman operator, nonlinear
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: LICENSES_bundled
+
+Quick links
+^^^^^^^^^^^
+
+`Source repository <https://gitlab.com/datafold-dev/datafold>`__ |
+`Contributing and feedback <https://datafold-dev.gitlab.io/datafold/contributing.html>`__ |
+`PyPI <https://pypi.org/project/datafold/>`__ |
+`Documentation <https://datafold-dev.gitlab.io/datafold/>`__ |
+`Tutorials <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__ |
+`Scientific literature <https://datafold-dev.gitlab.io/datafold/references.html>`__
+
+What is *datafold*?
+====================
+
+*datafold* is a `MIT-licensed <https://gitlab.com/datafold-dev/datafold/-/blob/master/LICENSE>`__
+Python package containing operator-theoretic, data-driven models to identify dynamical
+systems from time series data and to infer geometrical structures in point clouds.
+
+The package includes:
+
+* An efficient implementation of the ``DiffusionMaps`` model to infer geometric
+  meaningful structures from data, such as the eigenfunctions of the
+  Laplace-Beltrami operator. As a distinguishing factor to other implementations, the
+  model can handle a sparse kernel matrix and allows setting an arbitrary kernel,
+  including the standard Gaussian kernel,
+  `continuous k-nearest neighbor kernel <https://arxiv.org/abs/1606.02353>`__, or
+  `dynamics-adapted cone kernel <https://cims.nyu.edu/~dimitris/files/Giannakis15_cone_kernels.pdf>`__.
+* Implementations and variants of the Dynamic Mode Decomposition as data-driven methods to
+  identify and analyze dynamical systems from time series collection data. This incldues:
+  * ``DMDFull`` or ``DMDEco`` as standard methods of DMD
+  * ``OnlineDMD`` or ``StreamingDMD`` modify the DMD to handle streaming data
+  * ``DMDControl`` augments the DMD to handle additional control input
+  * ``EDMD`` - The Extended-DMD, which allows setting up a highly flexible dictionary to
+  transform time series data and thereby handle nonlinear dynamics within the Koopman
+  operator framework. The EDMD wraps an arbitrary DMD variation for the decomposition.
+  The key advantage of this is, that the ``EDMD`` directly profits from the above
+  functionalities. ``EDMD`` can be used in control or streaming settings. Furthermore it is
+  possible to learn the dictionary directly from data (commonly referred to EDMD-DL)
+* Handling of cross-validation. The method ``EDMDCV``, for example, allows model parameters to
+  be optimized with cross-validation splittings that account for the temporal order in time
+  series data.
+* Methods to perform Model Predictive Control (MPC) with Koopman operator-based methods (
+  mainly the ``EDMD``). *This is currently still under development and experimental*.
+* Regression models for high-dimensional data (often used for out-of-sample extensions for the
+  Diffusion Maps model), such as the (auto-tuned) Laplacian Pyramids or Geometric Harmonics to
+  interpolate general function values on a point cloud manifold.
+* A data structure ``TSCDataFrame`` to handle time series collection data. It simplifies model
+  inputs/outputs and make it easier to describe various forms of time series data.
+
+See also `this introduction page <https://datafold-dev.gitlab.io/datafold/intro.html>`__.
+For a mathematical thorough introduction, we refer to the `scientific literature
+<https://datafold-dev.gitlab.io/datafold/references.html>`__.
+
+.. note::
+    The project is under active development in a research-driven environment.
+
+    * Code quality varies from "experimental/early stage" to "well-tested". Well tested
+      code is listed in the
+      `software documentation <https://datafold-dev.gitlab.io/datafold/api.html>`__
+      and are directly accessible through the highest module level (e.g.
+      :code:`from datafold import ...`). Experimental code is
+      only accessible via "deep imports" (e.g.
+      :code:`from datafol.dynfold.outofsample import ...`) and may raise a warning when using
+      it.
+    * The interfaces within *datafold* are not stable. The software is **not** intended for
+      production. Nevertheless, if we break something it is intentional and we hope that such
+      adaptations become less over time.
+    * There is no deprecation cycle. The software uses
+      `semantic versioning <https://semver.org/>`__ policy `[major].[minor].[patch]`, i.e.
+
+         * `major` - making incompatible changes in the (documented) API
+         * `minor` - adding functionality in a backwards-compatible manner
+         * `patch` - backwards-compatible bug fixes
+
+      We do not intend to indicate a feature complete milestone with version `1.0`.
+
+Cite
+====
+
+If you use *datafold* in your research, please cite
+`this paper <https://joss.theoj.org/papers/10.21105/joss.02283>`__ published in the
+*Journal of Open Source Software* (`JOSS <https://joss.theoj.org/>`__).
+
+*Lehmberg et al., (2020). datafold: data-driven models for point clouds and time series on
+manifolds. Journal of Open Source Software, 5(51), 2283,* https://doi.org/10.21105/joss.02283
+
+BibTeX:
+
+.. code-block:: latex
+
+    @article{Lehmberg2020,
+             doi       = {10.21105/joss.02283},
+             url       = {https://doi.org/10.21105/joss.02283},
+             year      = {2020},
+             publisher = {The Open Journal},
+             volume    = {5},
+             number    = {51},
+             pages     = {2283},
+             author    = {Daniel Lehmberg and Felix Dietrich and Gerta K{\"o}ster and Hans-Joachim Bungartz},
+             title     = {datafold: data-driven models for point clouds and time series on manifolds},
+             journal   = {Journal of Open Source Software}}
+
+How to get it?
+==============
+
+Installation requires `Python>=3.9 <https://www.python.org/>`__ with
+`pip <https://pip.pypa.io/en/stable/>`__ and
+`setuptools <https://setuptools.pypa.io/en/latest/>`__ installed (both packages ship with a
+standard Python installation). The package dependencies
+install automatically. The main dependencies and their usage in *datafold* are listed
+in the section "Dependencies" below.
+
+There are two ways to install *datafold*:
+
+1. From PyPI
+------------
+
+This is the standard way for users. The package is hosted on the official Python package
+index (PyPI) and installs the core package (excluding tutorials and tests). The tutorial
+files can be downloaded separately
+`here <https://datafold-dev.gitlab.io/datafold/tutorial_index.html>`__.
+
+To install the package and its dependencies with :code:`pip`, run
+
+.. code-block:: bash
+
+   python -m pip install datafold
+
+.. note::
+
+    If you run Python in an Anaconda environment you can use pip from within ``conda``.
+    See also
+    `official instructions <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages>`__.
+
+    .. code-block:: bash
+
+        conda activate venv
+        conda install pip
+        pip install datafold
+
+2. From source
+--------------
+
+This way is recommended if you want to access the latest (but potentially unstable)
+development state, run tests or wish to contribute (see section "Contributing" for details).
+Download or git-clone the source code repository.
+
+1. Download the repository
+
+   a. If you wish to contribute code, it is required to have
+      `git <https://git-scm.com/>`__ installed. Clone the repository with
+
+      .. code-block:: bash
+
+        git clone https://gitlab.com/datafold-dev/datafold.git
+
+   b. If you only want access to the source code (current ``master`` branch), download one
+      of the compressed file types
+      (`zip <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.zip>`__,
+      `tar.gz <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.gz>`__,
+      `tar.bz2 <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar.bz2>`__,
+      `tar <https://gitlab.com/datafold-dev/datafold/-/archive/master/datafold-master.tar>`__)
+
+2. Install the package from the downloaded repository
+
+   .. code-block:: bash
+
+       python -m pip install .
+
+Contributing
+============
+
+Any contribution (code/tutorials/documentation improvements), question or feedback is
+very welcome. Either use the
+`issue tracker <https://gitlab.com/datafold-dev/datafold/-/issues>`__ or
+`Email <incoming+datafold-dev-datafold-14878376-issue-@incoming.gitlab.com>`__ us.
+Instructions to set up *datafold* for development can be found
+`here <https://datafold-dev.gitlab.io/datafold/contributing.html>`__.
+
+Dependencies
+============
+
+The dependencies of the core package are managed in the file
+`requirements.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements.txt>`__
+and install with *datafold*. The tests, tutorials, documentation and code analysis
+require additional dependencies which are managed in
+`requirements-dev.txt <https://gitlab.com/datafold-dev/datafold/-/blob/master/requirements-dev.txt>`__.
+
+*datafold* integrates with common packages from the
+`Python scientific computing stack <https://scipy.org/about/>`__:
+
+* `NumPy <https://numpy.org/>`__
+   NumPy is used throughout *datafold* and is the default package for numerical
+   data and algorithms.
+
+* `pandas <https://pandas.pydata.org/pandas-docs/stable/index.html>`__
+   *datafold* uses pandas'
+   `DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`__
+   as a base class for ``TSCDataFrame`` to capture various forms of time series data. The data
+   It includes specific time series collection functionality and is mostly compatible with
+   pandas' rich functionality.
+
+* `scikit-learn <https://scikit-learn.org/stable/>`__
+   All *datafold* algorithms that are part of the "machine learning pipeline" align
+   to the scikit-learn `API <https://scikit-learn.org/stable/developers/develop.html>`__.
+   This is done by deriving the models from
+   `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
+   and appropriate ``MixIns``. *datafold* defines own ``MixIns`` that align with the
+   API in a duck-typing fashion to allow identifying dynamical systems from temporal data
+   in ``TSCDataFrame``.
+
+* `SciPy <https://docs.scipy.org/doc/scipy/reference/index.html>`__
+   The package is used for elementary numerical algorithms and data structures in
+   conjunction with NumPy. This includes (sparse) linear least
+   square regression, (sparse) eigenpairs solver and sparse matrices as
+   optional data structure for kernel matrices.
+
+How does it compare to other software?
+======================================
+
+*Note: This list covers only Python packages.*
+
+* `scikit-learn <https://scikit-learn.org/stable/>`__
+   provides algorithms and models along the entire machine learning pipeline, with a
+   strong focus on static data (i.e. without temporal context). *datafold* integrates
+   into scikit-learn' API and all data-driven models are subclasses of
+   `BaseEstimator <https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html>`__.
+   An important contribution of *datafold* is the ``DiffusionMaps`` model as popular
+   framework for manifold learning, which is not contained in scikit-learn's `set of
+   algorithms <https://scikit-learn.org/stable/auto_examples/manifold/plot_compare_methods
+   .html#sphx-glr-auto-examples-manifold-plot-compare-methods-py>`__.
+   Furthermore, *datafold* includes dynamical systems as a new model class that is
+   operable with scikit-learn - the attributes align to supervised learning tasks.
+   The key differences are that a model processes data of type ``TSCDataFrame``
+   and instead of a one-to-one relation in the model's input/output, the model can return
+   arbitrary many output samples (a time series) for a single input
+   (an initial condition).
+
+* `PyDMD <https://github.com/PyDMD/PyDMD>`__
+   provides many variants of the `Dynamic Mode Decomposition (DMD)
+   <https://en.wikipedia.org/wiki/Dynamic_mode_decomposition>`__. *datafold* provides a wrapper
+   to make models of ``PyDMD`` accessible. However, a limitation of ``PyDMD`` is that it only
+   processes single coherent time series, see `PyDMD issue 86
+   <https://github.com/PyDMD/PyDMD/issues/86>`__. The DMD models that are directly included
+   in *datafold* utilize the functionality of the data structure ``TSCDataFrame`` and can
+   therefore process time series collections - in an extreme case only containing snapshot
+   pairs.
+
+* `PySINDy <https://pysindy.readthedocs.io/en/latest/>`__
+   specializes on a *sparse* system identification of nonlinear dynamical systems to
+   infer governing equations.
```

