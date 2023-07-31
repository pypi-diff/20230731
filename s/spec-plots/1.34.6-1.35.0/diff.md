# Comparing `tmp/spec_plots-1.34.6.tar.gz` & `tmp/spec_plots-1.35.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spec_plots-1.34.6.tar", last modified: Mon Mar 19 17:21:15 2018, max compression
+gzip compressed data, was "spec_plots-1.35.0.tar", last modified: Mon Jul 31 17:43:58 2023, max compression
```

## Comparing `spec_plots-1.34.6.tar` & `spec_plots-1.35.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      402 2018-03-19 17:21:15.000000 spec_plots-1.34.6/PKG-INFO
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      368 2016-11-28 23:12:28.000000 spec_plots-1.34.6/README.md
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       38 2018-03-19 17:21:15.000000 spec_plots-1.34.6/setup.cfg
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1226 2018-03-16 03:24:26.000000 spec_plots-1.34.6/setup.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      231 2018-03-19 17:19:48.000000 spec_plots-1.34.6/spec_plots/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1613 2018-03-16 03:24:26.000000 spec_plots-1.34.6/spec_plots/__main__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1648 2018-03-16 03:24:26.000000 spec_plots-1.34.6/spec_plots/__main_jwst__.py
--rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    20169 2018-03-19 16:55:13.000000 spec_plots-1.34.6/spec_plots/make_hst_spec_previews.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    16259 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/make_html.py
--rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    14959 2018-03-19 16:55:13.000000 spec_plots-1.34.6/spec_plots/make_jwst_spec_previews.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots/utils/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      180 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/__init__.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots/utils/specutils/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1336 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2333 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/avoidregion.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4601 2018-01-24 21:18:54.000000 spec_plots-1.34.6/spec_plots/utils/specutils/calc_covering_fraction.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3797 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/calc_plot_metrics.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4890 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/debug_oplot.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1957 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/dq_has_flag.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    15392 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/edge_trim.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1693 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/get_flux_stats.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1880 2016-11-28 23:11:25.000000 spec_plots-1.34.6/spec_plots/utils/specutils/is_bad_dq.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1035 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/rms.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4836 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/set_plot_xrange.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4587 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/set_plot_yrange.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1253 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils/specutilserror.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7916 2018-01-24 21:18:54.000000 spec_plots-1.34.6/spec_plots/utils/specutils/stitch_components.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      837 2018-01-24 21:18:54.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3125 2016-11-28 23:11:25.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/check_segments.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7256 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/cosspectrum.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3579 2016-11-28 23:11:25.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/extract_subspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1204 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/get_segment_names.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     5388 2018-01-24 21:18:54.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/make_fits.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17525 2018-03-19 17:02:43.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/plotspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    12465 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils_cos/readspec.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots/utils/specutils_jwst/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      483 2016-11-28 23:11:25.000000 spec_plots-1.34.6/spec_plots/utils/specutils_jwst/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1491 2016-11-28 23:11:25.000000 spec_plots-1.34.6/spec_plots/utils/specutils_jwst/jwstspectrum.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    13335 2018-03-19 17:03:12.000000 spec_plots-1.34.6/spec_plots/utils/specutils_jwst/plotspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2523 2016-11-28 23:11:25.000000 spec_plots-1.34.6/spec_plots/utils/specutils_jwst/readspec.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots/utils/specutils_stis/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      685 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils_stis/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1201 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils_stis/get_association_indices.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17344 2018-03-19 17:02:57.000000 spec_plots-1.34.6/spec_plots/utils/specutils_stis/plotspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2302 2016-11-28 23:02:15.000000 spec_plots-1.34.6/spec_plots/utils/specutils_stis/readspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4897 2016-09-30 20:32:23.000000 spec_plots-1.34.6/spec_plots/utils/specutils_stis/stis1dspectrum.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/dependency_links.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      125 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/entry_points.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2014-12-12 18:16:09.000000 spec_plots-1.34.6/spec_plots.egg-info/not-zip-safe
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      402 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/PKG-INFO
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       59 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/requires.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1860 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/SOURCES.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       11 2018-03-19 17:21:15.000000 spec_plots-1.34.6/spec_plots.egg-info/top_level.txt
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.949343 spec_plots-1.35.0/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      285 2023-07-31 17:43:58.949172 spec_plots-1.35.0/PKG-INFO
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      362 2023-07-31 15:04:45.000000 spec_plots-1.35.0/README.md
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       38 2023-07-31 17:43:58.949400 spec_plots-1.35.0/setup.cfg
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1175 2023-07-31 16:18:05.000000 spec_plots-1.35.0/setup.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.941427 spec_plots-1.35.0/spec_plots/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      231 2023-07-31 15:05:19.000000 spec_plots-1.35.0/spec_plots/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1613 2018-03-16 03:24:26.000000 spec_plots-1.35.0/spec_plots/__main__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1648 2018-03-16 03:24:26.000000 spec_plots-1.35.0/spec_plots/__main_jwst__.py
+-rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    20169 2020-04-05 18:34:12.000000 spec_plots-1.35.0/spec_plots/make_hst_spec_previews.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    16259 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/make_html.py
+-rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    14959 2018-03-19 16:55:13.000000 spec_plots-1.35.0/spec_plots/make_jwst_spec_previews.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.943238 spec_plots-1.35.0/spec_plots/utils/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      180 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/__init__.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.945834 spec_plots-1.35.0/spec_plots/utils/specutils/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1336 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2333 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/avoidregion.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4601 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils/calc_covering_fraction.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3797 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/calc_plot_metrics.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4890 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/debug_oplot.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1957 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/dq_has_flag.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    15392 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/edge_trim.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1693 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/get_flux_stats.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1880 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils/is_bad_dq.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1035 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/rms.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4836 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_xrange.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4587 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_yrange.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1253 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/specutilserror.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7916 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils/stitch_components.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.947299 spec_plots-1.35.0/spec_plots/utils/specutils_cos/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      837 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3125 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/check_segments.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7256 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/cosspectrum.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3579 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/extract_subspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1204 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/get_segment_names.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     5388 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/make_fits.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17530 2023-07-31 16:00:45.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/plotspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    12465 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/readspec.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.948009 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      483 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1491 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/jwstspectrum.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    13340 2023-07-31 16:09:30.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/plotspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2523 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/readspec.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.948924 spec_plots-1.35.0/spec_plots/utils/specutils_stis/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      685 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1201 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/get_association_indices.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17349 2023-07-31 15:57:11.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/plotspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2302 2016-11-28 23:02:15.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/readspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4897 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/stis1dspectrum.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.943037 spec_plots-1.35.0/spec_plots.egg-info/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      285 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/PKG-INFO
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1860 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      124 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/entry_points.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2014-12-12 18:16:09.000000 spec_plots-1.35.0/spec_plots.egg-info/not-zip-safe
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       62 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/requires.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       11 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spec_plots-1.34.6/setup.py` & `spec_plots-1.35.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 from __future__ import absolute_import
 from setuptools import setup
 from spec_plots import __version__
 
 setup(name="spec_plots",
       version=__version__,
       description="Create preview plots of HST or JWST spectra.",
-      classifiers=["Programming Language :: Python :: 2.7",
-                   "Programming Language :: Python :: 3.6"],
-      url="https://github.com/openSAIL/spec_plots",
+      classifiers=["Programming Language :: Python :: 3.9"],
+      url="https://github.com/spacetelescope/spec_plots",
       author="Scott W. Fleming",
       author_email="fleming@stsci.edu",
       license="MIT",
       packages=["spec_plots", "spec_plots.utils", "spec_plots.utils.specutils",
                 "spec_plots.utils.specutils_cos",
                 "spec_plots.utils.specutils_jwst",
                 "spec_plots.utils.specutils_stis"],
-      install_requires=["astropy>=0.4.1", "matplotlib>=1.4.1", "numpy>=1.9.1",
-                        "future>=0.15"],
+      install_requires=["astropy>=5.2.2", "matplotlib>=3.7.1", "numpy>=1.24.3",
+                        "future>=0.18.3"],
       entry_points={"console_scripts" :
                     ["make_hst_spec_previews = spec_plots.__main__:main",
                      "make_jwst_spec_previews = spec_plots.__main_jwst__:main"
                     ]},
       zip_safe=False)
```

### Comparing `spec_plots-1.34.6/spec_plots/__main__.py` & `spec_plots-1.35.0/spec_plots/__main__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/__main_jwst__.py` & `spec_plots-1.35.0/spec_plots/__main_jwst__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/make_hst_spec_previews.py` & `spec_plots-1.35.0/spec_plots/make_hst_spec_previews.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/make_html.py` & `spec_plots-1.35.0/spec_plots/make_html.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/make_jwst_spec_previews.py` & `spec_plots-1.35.0/spec_plots/make_jwst_spec_previews.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/__init__.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/__init__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/avoidregion.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/avoidregion.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/calc_covering_fraction.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/calc_covering_fraction.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/calc_plot_metrics.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/calc_plot_metrics.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/debug_oplot.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/debug_oplot.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/dq_has_flag.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/dq_has_flag.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/edge_trim.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/edge_trim.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/get_flux_stats.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/get_flux_stats.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/is_bad_dq.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/is_bad_dq.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/rms.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/rms.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/set_plot_xrange.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_xrange.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/set_plot_yrange.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_yrange.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/specutilserror.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/specutilserror.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils/stitch_components.py` & `spec_plots-1.35.0/spec_plots/utils/specutils/stitch_components.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/__init__.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/__init__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/check_segments.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/check_segments.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/cosspectrum.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/cosspectrum.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/extract_subspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/extract_subspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/get_segment_names.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/get_segment_names.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/make_fits.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/make_fits.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/plotspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/plotspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,27 +232,27 @@
             covering_fractions[i] = calc_covering_fraction(this_figure,
                                                            these_plotareas, i,
                                                            optimize=optimize)
             # Note: here we remove the line we plotted before, it was only so
             # that calc_covering_fraction would have someting to draw on the
             # canvas and thereby determine which pixels were "blue" (i.e., part
             # of the plotted spectrum vs. background).
-            this_plotarea.lines.remove(this_line[0])
+            this_line.pop(0).remove()
             # Now we plot the spectrum as a LineCollection so that the
             # transparency will have the desired effect, but, this is not
             # rendered on the canvas inside calc_covering_fraction, hence why we
             # need to plot it both as a regular line first.
             this_collection = this_plotarea.add_collection(
                 plot_metrics[i]["line_collection"])
 
             if covering_fractions[i] > 30.:
                 this_collection.set_alpha(0.1)
 
             # Turn on plot grid lines.
-            this_plotarea.grid(True)
+            this_plotarea.grid(True, linestyle="dashed")
 
             # Add the super title AFTER determining plot transparency (to
             # minimize number of colored pixels).
             if is_bigplot:
                 if i == len(subplot_segment_names)-1:
                     this_figure.suptitle(os.path.basename(
                         cos_spectrum.orig_file), fontsize=18, color='r')
```

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_cos/readspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_cos/readspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_jwst/jwstspectrum.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_jwst/jwstspectrum.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_jwst/plotspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_jwst/plotspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
         covering_fractions = calc_covering_fraction(
             this_figure, numpy.asarray([this_plotarea]), 0, optimize=optimize)
         # Note: here we remove the line we plotted before, it was only
         # so that calc_covering_fraction would have someting to draw on the
         # canvas and thereby determine which pixels were "blue" (i.e., part
         # of the plotted spectrum vs. background).
-        this_plotarea.lines.remove(this_line[0])
+        this_line.pop(0).remove()
         # Now we plot the spectrum as a LineCollection so that the
         # transparency will have the desired effect, but, this is not
         # rendered on the canvas inside calc_covering_fraction, hence why we
         # need to plot it both as a regular line first.
         # Note: because we are re-using a LineCollection object in the
         # array of plot_metrics (specifically, when creating the
         # thumbnail-sized plot), we have to use a copy of the LineCollection
@@ -192,15 +192,15 @@
         this_collection = this_plotarea.add_collection(copy.copy(
             plot_metrics["line_collection"]))
 
         if covering_fractions > 30.:
             this_collection.set_alpha(0.1)
 
         # Turn on plot grid lines.
-        this_plotarea.grid(True)
+        this_plotarea.grid(True, linestyle="dashed")
 
         if is_bigplot:
             this_figure.suptitle(os.path.basename(
                 jwst_spectrum.orig_file), fontsize=18, color='r')
 
         if debug:
             # Overplot points color-coded based on rejection criteria.
```

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_jwst/readspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_jwst/readspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_stis/__init__.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_stis/__init__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_stis/get_association_indices.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_stis/get_association_indices.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_stis/plotspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_stis/plotspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             covering_fractions[i] = calc_covering_fraction(this_figure,
                                                            these_plotareas, i,
                                                            optimize=optimize)
             # Note: here we remove the line we plotted before, it was only
             # so that calc_covering_fraction would have someting to draw on the
             # canvas and thereby determine which pixels were "blue" (i.e., part
             # of the plotted spectrum vs. background).
-            this_plotarea.lines.remove(this_line[0])
+            this_line.pop(0).remove()
             # Now we plot the spectrum as a LineCollection so that the
             # transparency will have the desired effect, but, this is not
             # rendered on the canvas inside calc_covering_fraction, hence why we
             # need to plot it both as a regular line first.
             # Note: because we are re-using a LineCollection object in the
             # array of plot_metrics (specifically, when creating the
             # thumbnail-sized plot), we have to use a copy of the LineCollection
@@ -236,15 +236,15 @@
                 this_collection = this_plotarea.add_collection(
                     plot_metrics[i]["line_collection"])
 
             if covering_fractions[i] > 30.:
                 this_collection.set_alpha(0.1)
 
             # Turn on plot grid lines.
-            this_plotarea.grid(True)
+            this_plotarea.grid(True, linestyle='dashed')
 
             if is_bigplot:
                 if i == len(stitched_spectra)-1:
                     this_figure.suptitle(os.path.basename(
                         stis_spectrum.orig_file), fontsize=18, color='r')
                 else:
                     this_figure.suptitle(os.path.basename(
```

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_stis/readspec.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_stis/readspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots/utils/specutils_stis/stis1dspectrum.py` & `spec_plots-1.35.0/spec_plots/utils/specutils_stis/stis1dspectrum.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.34.6/spec_plots.egg-info/SOURCES.txt` & `spec_plots-1.35.0/spec_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

