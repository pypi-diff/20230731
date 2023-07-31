# Comparing `tmp/ecosound-0.0.8.tar.gz` & `tmp/ecosound-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ecosound-0.0.8.tar", last modified: Tue Mar 23 05:59:46 2021, max compression
+gzip compressed data, was "ecosound-0.0.9.tar", last modified: Mon Feb 21 16:27:41 2022, max compression
```

## Comparing `ecosound-0.0.8.tar` & `ecosound-0.0.9.tar`

### file list

```diff
@@ -1,116 +1,144 @@
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:46.348710 ecosound-0.0.8/
--rw-rw-rw-   0        0        0      171 2020-11-20 20:53:27.000000 ecosound-0.0.8/AUTHORS.rst
--rw-rw-rw-   0        0        0       97 2020-11-20 20:53:27.000000 ecosound-0.0.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1548 2020-01-28 22:52:07.000000 ecosound-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      313 2020-12-02 18:37:01.000000 ecosound-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4079 2021-03-23 05:59:46.348710 ecosound-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2618 2021-01-16 02:30:23.000000 ecosound-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:44.855574 ecosound-0.0.8/docs/
--rw-rw-rw-   0        0        0      638 2021-01-16 01:59:15.000000 ecosound-0.0.8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:44.755433 ecosound-0.0.8/docs/build/
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:44.755433 ecosound-0.0.8/docs/build/html/
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.261469 ecosound-0.0.8/docs/build/html/_static/
--rw-rw-rw-   0        0        0   197010 2020-06-18 13:49:29.000000 ecosound-0.0.8/docs/build/html/_static/Detection_example_Snake_Island.png
--rw-rw-rw-   0        0        0    15633 2021-01-16 01:32:41.000000 ecosound-0.0.8/docs/build/html/_static/ecosound_logo.png
--rw-rw-rw-   0        0        0     4832 2021-01-16 02:32:06.000000 ecosound-0.0.8/docs/build/html/_static/ecosound_logo_small.png
--rw-rw-rw-   0        0        0    17672 2021-01-16 01:29:41.000000 ecosound-0.0.8/docs/build/html/_static/ecosound_logo_transparent.png
--rw-rw-rw-   0        0        0      286 2021-01-04 14:40:55.000000 ecosound-0.0.8/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2021-01-04 14:40:55.000000 ecosound-0.0.8/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2021-01-04 14:40:55.000000 ecosound-0.0.8/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      799 2021-01-16 01:59:15.000000 ecosound-0.0.8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.292714 ecosound-0.0.8/docs/source/
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.323966 ecosound-0.0.8/docs/source/_static/
--rw-rw-rw-   0        0        0   197010 2020-06-18 13:49:29.000000 ecosound-0.0.8/docs/source/_static/Detection_example_Snake_Island.png
--rw-rw-rw-   0        0        0    15633 2021-01-16 01:32:41.000000 ecosound-0.0.8/docs/source/_static/ecosound_logo.png
--rw-rw-rw-   0        0        0     4832 2021-01-16 02:32:06.000000 ecosound-0.0.8/docs/source/_static/ecosound_logo_small.png
--rw-rw-rw-   0        0        0    17672 2021-01-16 01:29:41.000000 ecosound-0.0.8/docs/source/_static/ecosound_logo_transparent.png
--rw-rw-rw-   0        0        0     2032 2021-01-16 02:33:20.000000 ecosound-0.0.8/docs/source/conf.py
--rw-rw-rw-   0        0        0     2835 2021-01-16 02:16:18.000000 ecosound-0.0.8/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.346092 ecosound-0.0.8/ecosound/
--rw-rw-rw-   0        0        0       43 2020-11-20 22:39:36.000000 ecosound-0.0.8/ecosound/__init__.py
--rw-rw-rw-   0        0        0       21 2021-03-23 05:46:38.000000 ecosound-0.0.8/ecosound/_version.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.446349 ecosound-0.0.8/ecosound/classification/
--rw-rw-rw-   0        0        0     7564 2020-07-08 04:38:12.000000 ecosound-0.0.8/ecosound/classification/CrossValidation.py
--rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.8/ecosound/classification/__init__.py
--rw-rw-rw-   0        0        0     1897 2020-11-12 22:45:59.000000 ecosound-0.0.8/ecosound/classification/classification.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.524473 ecosound-0.0.8/ecosound/core/
--rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.8/ecosound/core/__init__.py
--rw-rw-rw-   0        0        0    48534 2021-03-23 05:43:05.000000 ecosound-0.0.8/ecosound/core/annotation.py
--rw-rw-rw-   0        0        0    23222 2020-08-06 22:33:20.000000 ecosound-0.0.8/ecosound/core/audiotools.py
--rw-rw-rw-   0        0        0      893 2020-05-15 21:23:39.000000 ecosound-0.0.8/ecosound/core/decorators.py
--rw-rw-rw-   0        0        0     6737 2020-06-30 19:16:43.000000 ecosound-0.0.8/ecosound/core/measurement.py
--rw-rw-rw-   0        0        0     3543 2021-01-14 18:46:09.000000 ecosound-0.0.8/ecosound/core/metadata.py
--rw-rw-rw-   0        0        0    20929 2020-06-07 22:38:07.000000 ecosound-0.0.8/ecosound/core/spectrogram.py
--rw-rw-rw-   0        0        0      355 2020-01-31 20:51:33.000000 ecosound-0.0.8/ecosound/core/timestamp_formats.json
--rw-rw-rw-   0        0        0     5420 2020-12-02 18:17:31.000000 ecosound-0.0.8/ecosound/core/tools.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.524473 ecosound-0.0.8/ecosound/datasets/
--rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.8/ecosound/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.562234 ecosound-0.0.8/ecosound/detection/
--rw-rw-rw-   0        0        0       41 2020-02-22 00:42:41.000000 ecosound-0.0.8/ecosound/detection/__init__.py
--rw-rw-rw-   0        0        0    10497 2021-03-22 19:39:12.000000 ecosound-0.0.8/ecosound/detection/blob_detector.py
--rw-rw-rw-   0        0        0     1905 2020-02-26 18:26:05.000000 ecosound-0.0.8/ecosound/detection/detector_builder.py
--rw-rw-rw-   0        0        0     2136 2020-02-22 00:53:26.000000 ecosound-0.0.8/ecosound/detection/detector_template.py
--rw-rw-rw-   0        0        0     9513 2020-02-07 23:27:32.000000 ecosound-0.0.8/ecosound/detection/kurtosis_detector.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.577860 ecosound-0.0.8/ecosound/localization/
--rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.8/ecosound/localization/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.609106 ecosound-0.0.8/ecosound/measurements/
--rw-rw-rw-   0        0        0       55 2020-04-30 17:04:14.000000 ecosound-0.0.8/ecosound/measurements/__init__.py
--rw-rw-rw-   0        0        0     1900 2020-04-22 18:17:47.000000 ecosound-0.0.8/ecosound/measurements/measurer_builder.py
--rw-rw-rw-   0        0        0     2140 2020-04-22 18:57:43.000000 ecosound-0.0.8/ecosound/measurements/measurer_template.py
--rw-rw-rw-   0        0        0    52219 2021-03-22 20:03:07.000000 ecosound-0.0.8/ecosound/measurements/spectrogram_features.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.640353 ecosound-0.0.8/ecosound/visualization/
--rw-rw-rw-   0        0        0       41 2020-02-22 01:02:45.000000 ecosound-0.0.8/ecosound/visualization/__init__.py
--rw-rw-rw-   0        0        0     1865 2020-02-26 18:24:44.000000 ecosound-0.0.8/ecosound/visualization/grapher_builder.py
--rw-rw-rw-   0        0        0    21918 2020-10-28 23:05:36.000000 ecosound-0.0.8/ecosound/visualization/sound_plotter.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.424220 ecosound-0.0.8/ecosound.egg-info/
--rw-rw-rw-   0        0        0     4079 2021-03-23 05:59:43.000000 ecosound-0.0.8/ecosound.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2021-03-23 05:59:44.000000 ecosound-0.0.8/ecosound.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-23 05:59:43.000000 ecosound-0.0.8/ecosound.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-11-20 21:37:50.000000 ecosound-0.0.8/ecosound.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      191 2021-03-23 05:59:43.000000 ecosound-0.0.8/ecosound.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-03-23 05:59:43.000000 ecosound-0.0.8/ecosound.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-23 05:59:46.348710 ecosound-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1777 2021-03-22 20:24:24.000000 ecosound-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:45.646859 ecosound-0.0.8/tests/
--rw-rw-rw-   0        0        0       39 2020-11-20 20:53:27.000000 ecosound-0.0.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-23 05:59:46.326568 ecosound-0.0.8/tests/old_tests/
--rw-rw-rw-   0        0        0     1836 2020-05-29 04:54:05.000000 ecosound-0.0.8/tests/old_tests/Add_metadat_to_detections.py
--rw-rw-rw-   0        0        0     7053 2020-05-29 05:19:07.000000 ecosound-0.0.8/tests/old_tests/Annot_overlap.py
--rw-rw-rw-   0        0        0     2907 2020-05-29 22:19:30.000000 ecosound-0.0.8/tests/old_tests/Annotations.py
--rw-rw-rw-   0        0        0      674 2020-07-17 23:01:07.000000 ecosound-0.0.8/tests/old_tests/Classify.py
--rw-rw-rw-   0        0        0   153764 2020-12-15 23:42:43.000000 ecosound-0.0.8/tests/old_tests/ConvertDetect2raven.ipynb
--rw-rw-rw-   0        0        0     1935 2020-07-07 21:53:29.000000 ecosound-0.0.8/tests/old_tests/Investigate_detection_difference.py
--rw-rw-rw-   0        0        0     1678 2020-07-07 00:15:00.000000 ecosound-0.0.8/tests/old_tests/Measurements.py
--rw-rw-rw-   0        0        0     2303 2020-10-19 20:54:25.000000 ecosound-0.0.8/tests/old_tests/Troubleshoot_xarray_combine.py
--rw-rw-rw-   0        0        0    20448 2020-10-21 04:32:06.000000 ecosound-0.0.8/tests/old_tests/aTest_Xarray2.ipynb
--rw-rw-rw-   0        0        0     2738 2020-05-16 05:19:35.000000 ecosound-0.0.8/tests/old_tests/atest_dask-image.py
--rw-rw-rw-   0        0        0     3630 2020-05-05 04:21:55.000000 ecosound-0.0.8/tests/old_tests/atest_dask.py
--rw-rw-rw-   0        0        0     5548 2020-05-13 18:31:53.000000 ecosound-0.0.8/tests/old_tests/atest_dask2.py
--rw-rw-rw-   0        0        0     6106 2020-05-15 04:51:33.000000 ecosound-0.0.8/tests/old_tests/atest_dask3.py
--rw-rw-rw-   0        0        0      413 2020-11-20 20:53:27.000000 ecosound-0.0.8/tests/old_tests/atest_ecosound.py
--rw-rw-rw-   0        0        0      556 2021-03-23 05:44:34.000000 ecosound-0.0.8/tests/old_tests/atest_save_pamlab.py
--rw-rw-rw-   0        0        0   113979 2020-10-17 03:15:50.000000 ecosound-0.0.8/tests/old_tests/atest_xarray.ipynb
--rw-rw-rw-   0        0        0     1714 2020-03-02 05:14:37.000000 ecosound-0.0.8/tests/old_tests/atest_xarray.py
--rw-rw-rw-   0        0        0     2505 2020-02-07 18:58:06.000000 ecosound-0.0.8/tests/old_tests/audiotools.py
--rw-rw-rw-   0        0        0     3040 2020-07-07 19:02:14.000000 ecosound-0.0.8/tests/old_tests/blob_detector.py
--rw-rw-rw-   0        0        0      611 2020-11-10 05:12:52.000000 ecosound-0.0.8/tests/old_tests/check_netcdf_valid.py
--rw-rw-rw-   0        0        0    25121 2020-12-09 21:46:37.000000 ecosound-0.0.8/tests/old_tests/classification.py
--rw-rw-rw-   0        0        0     1448 2020-11-05 22:54:43.000000 ecosound-0.0.8/tests/old_tests/classification_datasets.py
--rw-rw-rw-   0        0        0      708 2020-05-13 20:58:12.000000 ecosound-0.0.8/tests/old_tests/dask_tutorial.py
--rw-rw-rw-   0        0        0     7885 2020-11-19 22:10:02.000000 ecosound-0.0.8/tests/old_tests/detector_batch.py
--rw-rw-rw-   0        0        0     6838 2020-10-19 23:01:23.000000 ecosound-0.0.8/tests/old_tests/detector_batch_parralel_run.py
--rw-rw-rw-   0        0        0     2601 2021-01-13 22:00:58.000000 ecosound-0.0.8/tests/old_tests/display_annot_detec.py
--rw-rw-rw-   0        0        0     4778 2021-01-13 23:16:37.000000 ecosound-0.0.8/tests/old_tests/display_annot_detec_documentation.py
--rw-rw-rw-   0        0        0     4931 2020-12-15 19:14:57.000000 ecosound-0.0.8/tests/old_tests/extract_hourly_detec_summary.py
--rw-rw-rw-   0        0        0     4584 2020-12-17 00:03:22.000000 ecosound-0.0.8/tests/old_tests/extract_hourly_detec_summary_raven.py
--rw-rw-rw-   0        0        0     5071 2020-10-21 04:16:35.000000 ecosound-0.0.8/tests/old_tests/extract_hourly_detec_summary_v2.py
--rw-rw-rw-   0        0        0     1967 2020-07-07 19:26:43.000000 ecosound-0.0.8/tests/old_tests/filter_detections.py
--rw-rw-rw-   0        0        0  3114276 2020-11-06 13:05:09.000000 ecosound-0.0.8/tests/old_tests/plot_ambient_sound.ipynb
--rw-rw-rw-   0        0        0     1707 2020-10-06 01:02:18.000000 ecosound-0.0.8/tests/old_tests/plot_timeseries.py
--rw-rw-rw-   0        0        0     3031 2020-12-15 08:01:07.000000 ecosound-0.0.8/tests/old_tests/re_classify_measurements.py
--rw-rw-rw-   0        0        0     2025 2020-11-05 22:46:32.000000 ecosound-0.0.8/tests/old_tests/relabel_FP_as_noise_annot.py
--rw-rw-rw-   0        0        0     1383 2020-05-15 04:46:28.000000 ecosound-0.0.8/tests/old_tests/spectrogram.py
--rw-rw-rw-   0        0        0     7878 2021-03-22 23:18:52.000000 ecosound-0.0.8/tests/old_tests/spectrogram_classifier.py
--rw-rw-rw-   0        0        0     2789 2020-09-23 06:36:54.000000 ecosound-0.0.8/tests/old_tests/spectrogram_measurer.py
--rw-rw-rw-   0        0        0     1855 2021-03-08 07:52:06.000000 ecosound-0.0.8/tests/old_tests/time_series_plotter.py
--rw-rw-rw-   0        0        0     2758 2021-01-05 19:56:11.000000 ecosound-0.0.8/tests/test_core_annotation.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:41.820960 ecosound-0.0.9/
+-rw-rw-rw-   0        0        0      171 2020-11-20 20:53:27.000000 ecosound-0.0.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0       97 2020-11-20 20:53:27.000000 ecosound-0.0.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1548 2020-01-28 22:52:07.000000 ecosound-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      313 2020-12-02 18:37:01.000000 ecosound-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3662 2022-02-21 16:27:41.818961 ecosound-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2618 2021-01-16 02:30:23.000000 ecosound-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:39.878933 ecosound-0.0.9/docs/
+-rw-rw-rw-   0        0        0      638 2021-01-16 01:59:15.000000 ecosound-0.0.9/docs/Makefile
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:39.753003 ecosound-0.0.9/docs/build/
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:39.755002 ecosound-0.0.9/docs/build/html/
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:39.940921 ecosound-0.0.9/docs/build/html/_static/
+-rw-rw-rw-   0        0        0   197010 2020-06-18 13:49:29.000000 ecosound-0.0.9/docs/build/html/_static/Detection_example_Snake_Island.png
+-rw-rw-rw-   0        0        0    15633 2021-01-16 01:32:41.000000 ecosound-0.0.9/docs/build/html/_static/ecosound_logo.png
+-rw-rw-rw-   0        0        0     4832 2021-01-16 02:32:06.000000 ecosound-0.0.9/docs/build/html/_static/ecosound_logo_small.png
+-rw-rw-rw-   0        0        0    17672 2021-01-16 01:29:41.000000 ecosound-0.0.9/docs/build/html/_static/ecosound_logo_transparent.png
+-rw-rw-rw-   0        0        0      286 2021-01-04 14:40:55.000000 ecosound-0.0.9/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2021-01-04 14:40:55.000000 ecosound-0.0.9/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2021-01-04 14:40:55.000000 ecosound-0.0.9/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      799 2021-01-16 01:59:15.000000 ecosound-0.0.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:39.972879 ecosound-0.0.9/docs/source/
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.010858 ecosound-0.0.9/docs/source/_static/
+-rw-rw-rw-   0        0        0   197010 2020-06-18 13:49:29.000000 ecosound-0.0.9/docs/source/_static/Detection_example_Snake_Island.png
+-rw-rw-rw-   0        0        0    15633 2021-01-16 01:32:41.000000 ecosound-0.0.9/docs/source/_static/ecosound_logo.png
+-rw-rw-rw-   0        0        0     4832 2021-01-16 02:32:06.000000 ecosound-0.0.9/docs/source/_static/ecosound_logo_small.png
+-rw-rw-rw-   0        0        0    17672 2021-01-16 01:29:41.000000 ecosound-0.0.9/docs/source/_static/ecosound_logo_transparent.png
+-rw-rw-rw-   0        0        0     2032 2021-01-16 02:33:20.000000 ecosound-0.0.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2835 2021-01-16 02:16:18.000000 ecosound-0.0.9/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.028846 ecosound-0.0.9/ecosound/
+-rw-rw-rw-   0        0        0       43 2020-11-20 22:39:36.000000 ecosound-0.0.9/ecosound/__init__.py
+-rw-rw-rw-   0        0        0       21 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/_version.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.132786 ecosound-0.0.9/ecosound/classification/
+-rw-rw-rw-   0        0        0     7564 2020-07-08 04:38:12.000000 ecosound-0.0.9/ecosound/classification/CrossValidation.py
+-rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.9/ecosound/classification/__init__.py
+-rw-rw-rw-   0        0        0     1897 2020-11-12 22:45:59.000000 ecosound-0.0.9/ecosound/classification/classification.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.340667 ecosound-0.0.9/ecosound/core/
+-rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.9/ecosound/core/__init__.py
+-rw-rw-rw-   0        0        0    48788 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/core/annotation.py
+-rw-rw-rw-   0        0        0    27265 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/core/audiotools.py
+-rw-rw-rw-   0        0        0      893 2020-05-15 21:23:39.000000 ecosound-0.0.9/ecosound/core/decorators.py
+-rw-rw-rw-   0        0        0     1747 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/core/envelop.py
+-rw-rw-rw-   0        0        0     6737 2020-06-30 19:16:43.000000 ecosound-0.0.9/ecosound/core/measurement.py
+-rw-rw-rw-   0        0        0     3543 2021-01-14 18:46:09.000000 ecosound-0.0.9/ecosound/core/metadata.py
+-rw-rw-rw-   0        0        0    20907 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/core/spectrogram.py
+-rw-rw-rw-   0        0        0      462 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/core/timestamp_formats.json
+-rw-rw-rw-   0        0        0     8813 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/core/tools.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.352660 ecosound-0.0.9/ecosound/datasets/
+-rw-rw-rw-   0        0        0        0 2020-01-23 06:16:40.000000 ecosound-0.0.9/ecosound/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.422620 ecosound-0.0.9/ecosound/detection/
+-rw-rw-rw-   0        0        0       41 2020-02-22 00:42:41.000000 ecosound-0.0.9/ecosound/detection/__init__.py
+-rw-rw-rw-   0        0        0    10762 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/detection/blob_detector.py
+-rw-rw-rw-   0        0        0     1905 2020-02-26 18:26:05.000000 ecosound-0.0.9/ecosound/detection/detector_builder.py
+-rw-rw-rw-   0        0        0     2136 2020-02-22 00:53:26.000000 ecosound-0.0.9/ecosound/detection/detector_template.py
+-rw-rw-rw-   0        0        0     9513 2020-02-07 23:27:32.000000 ecosound-0.0.9/ecosound/detection/kurtosis_detector.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.816396 ecosound-0.0.9/ecosound/localization/
+-rw-rw-rw-   0        0        0     4714 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/localization/AnimationHPoptimization.py
+-rw-rw-rw-   0        0        0    20058 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/localization/ArrayOptimization.py
+-rw-rw-rw-   0        0        0     3237 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/localization/ArrayOptimization_plots.py
+-rw-rw-rw-   0        0        0        2 2022-02-21 15:54:08.000000 ecosound-0.0.9/ecosound/localization/__init__.py
+-rw-rw-rw-   0        0        0    48155 2022-02-21 16:08:47.000000 ecosound-0.0.9/ecosound/localization/initial_tes.py
+-rw-rw-rw-   0        0        0    18085 2022-02-21 16:08:47.000000 ecosound-0.0.9/ecosound/localization/initial_tes_exeter.py
+-rw-rw-rw-   0        0        0    44968 2022-02-21 16:08:47.000000 ecosound-0.0.9/ecosound/localization/initial_tes_gridsearch.py
+-rw-rw-rw-   0        0        0    19575 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/localization_batch_run.py
+-rw-rw-rw-   0        0        0    29495 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/localizationlib.py
+-rw-rw-rw-   0        0        0     9149 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plotArrayUncertainties.py
+-rw-rw-rw-   0        0        0     5682 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plotArrayUncertainties_jen.py
+-rw-rw-rw-   0        0        0     9221 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plotArrayUncertainties_mobile_array.py
+-rw-rw-rw-   0        0        0    18497 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results.py
+-rw-rw-rw-   0        0        0    22353 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_LArray_ROV.py
+-rw-rw-rw-   0        0        0    19929 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_lingcod.py
+-rw-rw-rw-   0        0        0    21775 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_lingcod_video.py
+-rw-rw-rw-   0        0        0    23385 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_mini_ROV_video.py
+-rw-rw-rw-   0        0        0    22603 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_mini_copper_video.py
+-rw-rw-rw-   0        0        0    22217 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_mobile_copper2_video.py
+-rw-rw-rw-   0        0        0    21018 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_mobile_copper_video.py
+-rw-rw-rw-   0        0        0    20926 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_mobile_goby_video.py
+-rw-rw-rw-   0        0        0    20145 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_mobile_projector.py
+-rw-rw-rw-   0        0        0    19960 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_quillback.py
+-rw-rw-rw-   0        0        0    19330 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/plot_localization_results_quillback_video.py
+-rw-rw-rw-   0        0        0     3115 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/postprocess_HI07_results.py
+-rw-rw-rw-   0        0        0      923 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/savec_loc_as_csv_tempscript.py
+-rw-rw-rw-   0        0        0     1321 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/tes_movie.py
+-rw-rw-rw-   0        0        0      146 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/localization/untitled0.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.866366 ecosound-0.0.9/ecosound/measurements/
+-rw-rw-rw-   0        0        0       55 2020-04-30 17:04:14.000000 ecosound-0.0.9/ecosound/measurements/__init__.py
+-rw-rw-rw-   0        0        0     1900 2020-04-22 18:17:47.000000 ecosound-0.0.9/ecosound/measurements/measurer_builder.py
+-rw-rw-rw-   0        0        0     2140 2020-04-22 18:57:43.000000 ecosound-0.0.9/ecosound/measurements/measurer_template.py
+-rw-rw-rw-   0        0        0    52219 2021-03-22 20:03:07.000000 ecosound-0.0.9/ecosound/measurements/spectrogram_features.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.906989 ecosound-0.0.9/ecosound/visualization/
+-rw-rw-rw-   0        0        0       41 2020-02-22 01:02:45.000000 ecosound-0.0.9/ecosound/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1865 2020-02-26 18:24:44.000000 ecosound-0.0.9/ecosound/visualization/grapher_builder.py
+-rw-rw-rw-   0        0        0    22453 2022-02-21 15:54:09.000000 ecosound-0.0.9/ecosound/visualization/sound_plotter.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.098806 ecosound-0.0.9/ecosound.egg-info/
+-rw-rw-rw-   0        0        0     3662 2022-02-21 16:27:38.000000 ecosound-0.0.9/ecosound.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4811 2022-02-21 16:27:39.000000 ecosound-0.0.9/ecosound.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-21 16:27:39.000000 ecosound-0.0.9/ecosound.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-11-20 21:37:50.000000 ecosound-0.0.9/ecosound.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      134 2022-02-21 16:27:39.000000 ecosound-0.0.9/ecosound.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-02-21 16:27:39.000000 ecosound-0.0.9/ecosound.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-02-21 16:27:41.822974 ecosound-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2022-02-21 15:54:09.000000 ecosound-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:40.934992 ecosound-0.0.9/tests/
+-rw-rw-rw-   0        0        0       39 2020-11-20 20:53:27.000000 ecosound-0.0.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-21 16:27:41.808968 ecosound-0.0.9/tests/old_tests/
+-rw-rw-rw-   0        0        0     1836 2020-05-29 04:54:05.000000 ecosound-0.0.9/tests/old_tests/Add_metadat_to_detections.py
+-rw-rw-rw-   0        0        0     7053 2020-05-29 05:19:07.000000 ecosound-0.0.9/tests/old_tests/Annot_overlap.py
+-rw-rw-rw-   0        0        0     2907 2020-05-29 22:19:30.000000 ecosound-0.0.9/tests/old_tests/Annotations.py
+-rw-rw-rw-   0        0        0      674 2020-07-17 23:01:07.000000 ecosound-0.0.9/tests/old_tests/Classify.py
+-rw-rw-rw-   0        0        0   153764 2020-12-15 23:42:43.000000 ecosound-0.0.9/tests/old_tests/ConvertDetect2raven.ipynb
+-rw-rw-rw-   0        0        0     1935 2020-07-07 21:53:29.000000 ecosound-0.0.9/tests/old_tests/Investigate_detection_difference.py
+-rw-rw-rw-   0        0        0     1678 2020-07-07 00:15:00.000000 ecosound-0.0.9/tests/old_tests/Measurements.py
+-rw-rw-rw-   0        0        0     2303 2020-10-19 20:54:25.000000 ecosound-0.0.9/tests/old_tests/Troubleshoot_xarray_combine.py
+-rw-rw-rw-   0        0        0    20448 2020-10-21 04:32:06.000000 ecosound-0.0.9/tests/old_tests/aTest_Xarray2.ipynb
+-rw-rw-rw-   0        0        0     2738 2020-05-16 05:19:35.000000 ecosound-0.0.9/tests/old_tests/atest_dask-image.py
+-rw-rw-rw-   0        0        0     3630 2020-05-05 04:21:55.000000 ecosound-0.0.9/tests/old_tests/atest_dask.py
+-rw-rw-rw-   0        0        0     5548 2020-05-13 18:31:53.000000 ecosound-0.0.9/tests/old_tests/atest_dask2.py
+-rw-rw-rw-   0        0        0     6106 2020-05-15 04:51:33.000000 ecosound-0.0.9/tests/old_tests/atest_dask3.py
+-rw-rw-rw-   0        0        0      413 2020-11-20 20:53:27.000000 ecosound-0.0.9/tests/old_tests/atest_ecosound.py
+-rw-rw-rw-   0        0        0      556 2021-03-23 05:44:34.000000 ecosound-0.0.9/tests/old_tests/atest_save_pamlab.py
+-rw-rw-rw-   0        0        0   113979 2020-10-17 03:15:50.000000 ecosound-0.0.9/tests/old_tests/atest_xarray.ipynb
+-rw-rw-rw-   0        0        0     1714 2020-03-02 05:14:37.000000 ecosound-0.0.9/tests/old_tests/atest_xarray.py
+-rw-rw-rw-   0        0        0     2505 2020-02-07 18:58:06.000000 ecosound-0.0.9/tests/old_tests/audiotools.py
+-rw-rw-rw-   0        0        0     3040 2020-07-07 19:02:14.000000 ecosound-0.0.9/tests/old_tests/blob_detector.py
+-rw-rw-rw-   0        0        0      611 2020-11-10 05:12:52.000000 ecosound-0.0.9/tests/old_tests/check_netcdf_valid.py
+-rw-rw-rw-   0        0        0    25121 2020-12-09 21:46:37.000000 ecosound-0.0.9/tests/old_tests/classification.py
+-rw-rw-rw-   0        0        0     1448 2020-11-05 22:54:43.000000 ecosound-0.0.9/tests/old_tests/classification_datasets.py
+-rw-rw-rw-   0        0        0      708 2020-05-13 20:58:12.000000 ecosound-0.0.9/tests/old_tests/dask_tutorial.py
+-rw-rw-rw-   0        0        0     7885 2020-11-19 22:10:02.000000 ecosound-0.0.9/tests/old_tests/detector_batch.py
+-rw-rw-rw-   0        0        0     6838 2020-10-19 23:01:23.000000 ecosound-0.0.9/tests/old_tests/detector_batch_parralel_run.py
+-rw-rw-rw-   0        0        0     2601 2021-01-13 22:00:58.000000 ecosound-0.0.9/tests/old_tests/display_annot_detec.py
+-rw-rw-rw-   0        0        0     4778 2021-01-13 23:16:37.000000 ecosound-0.0.9/tests/old_tests/display_annot_detec_documentation.py
+-rw-rw-rw-   0        0        0     4931 2020-12-15 19:14:57.000000 ecosound-0.0.9/tests/old_tests/extract_hourly_detec_summary.py
+-rw-rw-rw-   0        0        0     4584 2020-12-17 00:03:22.000000 ecosound-0.0.9/tests/old_tests/extract_hourly_detec_summary_raven.py
+-rw-rw-rw-   0        0        0     5071 2020-10-21 04:16:35.000000 ecosound-0.0.9/tests/old_tests/extract_hourly_detec_summary_v2.py
+-rw-rw-rw-   0        0        0     1967 2020-07-07 19:26:43.000000 ecosound-0.0.9/tests/old_tests/filter_detections.py
+-rw-rw-rw-   0        0        0  3114276 2020-11-06 13:05:09.000000 ecosound-0.0.9/tests/old_tests/plot_ambient_sound.ipynb
+-rw-rw-rw-   0        0        0     1707 2020-10-06 01:02:18.000000 ecosound-0.0.9/tests/old_tests/plot_timeseries.py
+-rw-rw-rw-   0        0        0     3031 2020-12-15 08:01:07.000000 ecosound-0.0.9/tests/old_tests/re_classify_measurements.py
+-rw-rw-rw-   0        0        0     2025 2020-11-05 22:46:32.000000 ecosound-0.0.9/tests/old_tests/relabel_FP_as_noise_annot.py
+-rw-rw-rw-   0        0        0     1383 2020-05-15 04:46:28.000000 ecosound-0.0.9/tests/old_tests/spectrogram.py
+-rw-rw-rw-   0        0        0     7878 2021-03-22 23:18:52.000000 ecosound-0.0.9/tests/old_tests/spectrogram_classifier.py
+-rw-rw-rw-   0        0        0     2789 2020-09-23 06:36:54.000000 ecosound-0.0.9/tests/old_tests/spectrogram_measurer.py
+-rw-rw-rw-   0        0        0     1855 2021-03-08 07:52:06.000000 ecosound-0.0.9/tests/old_tests/time_series_plotter.py
+-rw-rw-rw-   0        0        0     2758 2021-01-05 19:56:11.000000 ecosound-0.0.9/tests/test_core_annotation.py
```

### Comparing `ecosound-0.0.8/LICENSE` & `ecosound-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/README.rst` & `ecosound-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/Makefile` & `ecosound-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/build/html/_static/Detection_example_Snake_Island.png` & `ecosound-0.0.9/docs/build/html/_static/Detection_example_Snake_Island.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/build/html/_static/ecosound_logo.png` & `ecosound-0.0.9/docs/build/html/_static/ecosound_logo.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/build/html/_static/ecosound_logo_small.png` & `ecosound-0.0.9/docs/build/html/_static/ecosound_logo_small.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/build/html/_static/ecosound_logo_transparent.png` & `ecosound-0.0.9/docs/build/html/_static/ecosound_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/make.bat` & `ecosound-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/source/_static/Detection_example_Snake_Island.png` & `ecosound-0.0.9/docs/source/_static/Detection_example_Snake_Island.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/source/_static/ecosound_logo.png` & `ecosound-0.0.9/docs/source/_static/ecosound_logo.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/source/_static/ecosound_logo_small.png` & `ecosound-0.0.9/docs/source/_static/ecosound_logo_small.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/source/_static/ecosound_logo_transparent.png` & `ecosound-0.0.9/docs/source/_static/ecosound_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/source/conf.py` & `ecosound-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/docs/source/index.rst` & `ecosound-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/classification/CrossValidation.py` & `ecosound-0.0.9/ecosound/classification/CrossValidation.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/classification/classification.py` & `ecosound-0.0.9/ecosound/classification/classification.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/core/annotation.py` & `ecosound-0.0.9/ecosound/core/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -736,50 +736,54 @@
         for key, value in kwargs.items():
             if key in self.data:
                 self.data[key] = value
             else:
                 raise ValueError('The annotation object has no field: '
                                  + str(key))
 
-    def insert_metadata(self, deployment_info_file):
+    def insert_metadata(self, deployment_info_file, channel=0):
         """
         Insert metadata infortion to the annotation.
 
         Uses the Deployment_info_file to fill in the metadata of the annotation
         . The deployment_info_file must be created using the DeploymentInfo
         class from ecosound.core.metadata using DeploymentInfo.write_template.
 
         Parameters
         ----------
         deployment_info_file : str
             Csv file readable by ecosound.core.meta.DeploymentInfo.read(). It
             contains all the deployment metadata.
+        channel : int
+            Channel number of the recorder for the metadata to insert.
+            Default is 0
 
         Returns
         -------
         None.
 
         """
+        channel = int(channel)
         dep_info = DeploymentInfo()
         dep_info.read(deployment_info_file)
-        self.insert_values(UTC_offset=dep_info.data['UTC_offset'].values[0],
-                           audio_channel=dep_info.data['audio_channel_number'].values[0],
-                           audio_sampling_frequency=dep_info.data['sampling_frequency'].values[0],
-                           audio_bit_depth=dep_info.data['bit_depth'].values[0],
-                           mooring_platform_name = dep_info.data['mooring_platform_name'].values[0],
-                           recorder_type=dep_info.data['recorder_type'].values[0],
-                           recorder_SN=dep_info.data['recorder_SN'].values[0],
-                           hydrophone_model=dep_info.data['hydrophone_model'].values[0],
-                           hydrophone_SN=dep_info.data['hydrophone_SN'].values[0],
-                           hydrophone_depth=dep_info.data['hydrophone_depth'].values[0],
-                           location_name=dep_info.data['location_name'].values[0],
-                           location_lat=dep_info.data['location_lat'].values[0],
-                           location_lon=dep_info.data['location_lon'].values[0],
-                           location_water_depth=dep_info.data['location_water_depth'].values[0],
-                           deployment_ID=dep_info.data['deployment_ID'].values[0],
+        self.insert_values(UTC_offset=dep_info.data['UTC_offset'].values[channel],
+                           audio_channel=dep_info.data['audio_channel_number'].values[channel],
+                           audio_sampling_frequency=dep_info.data['sampling_frequency'].values[channel],
+                           audio_bit_depth=dep_info.data['bit_depth'].values[channel],
+                           mooring_platform_name = dep_info.data['mooring_platform_name'].values[channel],
+                           recorder_type=dep_info.data['recorder_type'].values[channel],
+                           recorder_SN=dep_info.data['recorder_SN'].values[channel],
+                           hydrophone_model=dep_info.data['hydrophone_model'].values[channel],
+                           hydrophone_SN=dep_info.data['hydrophone_SN'].values[channel],
+                           hydrophone_depth=dep_info.data['hydrophone_depth'].values[channel],
+                           location_name=dep_info.data['location_name'].values[channel],
+                           location_lat=dep_info.data['location_lat'].values[channel],
+                           location_lon=dep_info.data['location_lon'].values[channel],
+                           location_water_depth=dep_info.data['location_water_depth'].values[channel],
+                           deployment_ID=dep_info.data['deployment_ID'].values[channel],
                           )
 
     def filter_overlap_with(self, annot, freq_ovp=True,dur_factor_max=None,dur_factor_min=None,ovlp_ratio_min=None,remove_duplicates=False,inherit_metadata=False,filter_deploymentID=True, inplace=False):
         """
         Filter overalaping annotations.
 
         Only keep annotations that overlap in time and/or frequency with the
```

### Comparing `ecosound-0.0.8/ecosound/core/audiotools.py` & `ecosound-0.0.9/ecosound/core/audiotools.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class Sound:
     """
     A class to load and manipulate a sound file
 
     This class can load data from an entire, or part of a, sound file, filter
-    the loaded data, select subsections, and plotteh waveform. Currently a
+    the loaded data, select subsections, and plot the waveform. Currently a
     Sound object can only load data from one channel at a time.
 
     Attributes
     ----------
     file_full_path : str
         Path of the sound file, including file name and extension.
     file_dir : str
@@ -151,15 +151,15 @@
             Remove DC offset of the waveform by subtracting the mean. The
             default is False.
 
         Raises
         ------
         ValueError
             If the chunk list has only 1 value.
-            If the first value in the chunk list is greater or equal to the 
+            If the first value in the chunk list is greater or equal to the
                second one.
             If values in the chunk list exceed the audio file limits.
             If the channel selected does not exist.
             If samp is not set to 'samp' or 'sec'
 
         Returns
         -------
@@ -217,21 +217,21 @@
             raise ValueError(msg)
 
     def filter(self, filter_type, cutoff_frequencies, order=4):
         """
         Filter the audio signal.
 
         Applies low-pass, high-pass, or band-pass scientific filter to the
-        audio signal. The attribute waveform is updated with the filtered 
+        audio signal. The attribute waveform is updated with the filtered
         signal. The same data can only be filtered once.
 
         Parameters
         ----------
         filter_type : str
-            Type of filter. Can be set to 'bandpass', 'lowpass' or 'highpass'.            
+            Type of filter. Can be set to 'bandpass', 'lowpass' or 'highpass'.
         cutoff_frequencies : list
             Cutoff frequencies of the filter, in Hz (float). Must be a list with a
             single float if the filter_type is set to 'lowpass' or 'highpass'.
             Must be a list with two float values (i.e.,[fmin, fmax]) if the
             filter_type is set to 'bandpass'.
         order : int, optional
             Order of the filter. The default is 4.
@@ -248,40 +248,81 @@
             frequencies.
 
         Returns
         -------
         None. Filtered signal in the 'waveform' attribute of the Sound object.
         """
         if self._filter_applied is False:
+
+            # check bandpass cuttoff freq and switch to lowpass.highpass if necessary
+            if (filter_type == 'bandpass') and (min(cutoff_frequencies) <=0):
+                cutoff_frequencies = [max(cutoff_frequencies)]
+                filter_type = 'lowpass'
+                print('Warning: filter type was changed from "bandpass" to "lowpass".')
+            if (filter_type == 'bandpass') and (max(cutoff_frequencies) >=self._waveform_sampling_frequency/2):
+                cutoff_frequencies = [min(cutoff_frequencies)]
+                filter_type = 'highpass'
+                print('Warning: filter type was changed from "bandpass" to "highpass".')
+            # Instantiate filter object
             my_filter = Filter(filter_type, cutoff_frequencies, order)
             self._waveform = my_filter.apply(self._waveform,
                                              self._waveform_sampling_frequency)
             self._filter_applied = True
             self._filter_params = my_filter
         else:
             raise ValueError('This signal has been filtered already. Cannot'
                              + ' filter twice.')
 
-    def plot_waveform(self, unit='sec', newfig=False, title=''):
+    def upsample(self, resolution_sec):
+        """
+        Upsample  waveform
+
+        Increase the number of samples in the waveform and interpolate.
+
+        Parameters
+        ----------
+        resolution_sec : float
+            Sample resolution of the upsampled waveform, in second. The new
+            sampling frequency will be 1/resolution_sec.
+
+        Returns
+        -------
+        None. Updates the waveform of the Sound object.
+
+        """
+        self._waveform, self._waveform_sampling_frequency = upsample(
+            self._waveform,
+            1/ self._waveform_sampling_frequency,
+            resolution_sec)
+
+    def normalize(self, method='amplitude'):
+        if method == 'amplitude':
+            self._waveform = self._waveform / np.max(self._waveform)
+
+    def plot(self, unit='sec', newfig=False, label=[],linestyle='-', marker='',color='black', title=''):
         """
         Plot waveform of the audio signal.
 
         PLots the waveform of the audio signal. Both the plot title and time
-        units can be asjusted. The plot can be displayed on a new or an 
+        units can be asjusted. The plot can be displayed on a new or an
         existing figure.
 
         Parameters
         ----------
         unit : str, optional
             Time units to use. Can be either 'sec' for seconds, or 'samp' for
             samples. The default is 'sec'.
         newfig : bool, optional
             PLots on a new figure if set to True. The default is False.
         title : str, optional
             Title of the plot. The default is ''.
+        linestyle : str, optional
+            Linestyle of the plot. The default is '-'.
+        marker : str, optional
+            Marker of the plot. The default is '-'.
 
         Raises
         ------
         ValueError
             If the waveform attribute is empty.
 
         Returns
@@ -299,36 +340,44 @@
             xlabel = 'Time (sec)'
         elif unit == 'samp':
             axis_t = np.arange(0, len(self._waveform), 1)
             xlabel = 'Time (sample)'
         if newfig:
             plt.figure()
         axis_t = axis_t[0:len(self._waveform)]
-        plt.plot(axis_t, self._waveform, color='black')
+        plt.plot(axis_t, self._waveform,
+                           color=color,
+                           marker = marker,
+                           linestyle = linestyle,
+                           label=label,
+                           )
         plt.xlabel(xlabel)
         plt.ylabel('Amplitude')
         plt.title(title)
         plt.axis([axis_t[0], axis_t[-1],
                   min(self._waveform),
                   max(self._waveform)])
         plt.grid()
         plt.show()
 
-    def select_snippet(self, chunk):
+    def select_snippet(self, chunk, unit='samp'):
         """
         Select section of the loaded waveform.
 
         Create a new Sound object from a section of the sound data laoded.
 
         Parameters
         ----------
         chunk : list
             List of two int values representing the [start time, stop time] of
-            the sound data to select, in samples. Start time must be smaller 
-            than stop time.
+            the sound data to select. Start time must be smaller than stop
+            time.
+        unit : str, optional
+            Time unit of the 'chunk' parameter. Can be set to 'sec' for seconds
+            or 'samp', for samples. The default is 'samp'.
 
         Raises
         ------
         ValueError
             If chunk has only one value
             If the start time is greater tahn the stop time
             If the start or stop times fall outside of the wavform limits.
@@ -338,22 +387,31 @@
         snippet : Sound obj
             Sound object with the selected audio data.
 
         """
         if len(chunk) != 2:
             raise ValueError('Chunk should be a list of with 2 values: '
                              + 'chunk=[t1, t2].')
+        elif unit not in ('samp','sec'):
+           raise ValueError('Invalid unit. Should be set to "sec" or "samp".')
         elif chunk[0] >= chunk[1]:
             raise ValueError('Chunk[0] should be greater than chunk[1].')
-        elif (chunk[0] < 0) | (chunk[0] > self.file_duration_sample):
-            raise ValueError('Invalid chunk start value. The sample value '
+
+        if unit == 'sec':
+            chunk[0] = int(np.floor(chunk[0] * self.waveform_sampling_frequency))
+            chunk[1] = int(np.ceil(chunk[1] * self.waveform_sampling_frequency))
+
+        if (chunk[0] < 0) | (chunk[0] > self.file_duration_sample):
+            raise ValueError('Invalid chunk start value. The start value '
                              + 'chunk[0] is outside of file limit.')
         elif (chunk[1] < 0) | (chunk[1] > self.file_duration_sample):
-            raise ValueError('Invalid chunk stop value. The sample value '
+            raise ValueError('Invalid chunk stop value. The stop value '
                              + 'chunk[1] is outside of file limit.')
+
+
         snippet = copy.deepcopy(self)
         snippet._waveform = self._waveform[chunk[0]:chunk[1]]
         snippet._waveform_stop_sample = snippet._waveform_start_sample + chunk[1]
         snippet._waveform_start_sample = snippet._waveform_start_sample + chunk[0]
         snippet._waveform_duration_sample = len(snippet._waveform)
         snippet._waveform_duration_sec = snippet._waveform_duration_sec / snippet._waveform_sampling_frequency
         return snippet
@@ -370,15 +428,15 @@
         Parameters
         ----------
         energy_percentage : float
             Percentage of the energy the updated waveform should have.
 
         Returns
         -------
-        None. Updates the 'waveform' attribute alomg with all the waveform 
+        None. Updates the 'waveform' attribute alomg with all the waveform
         -related attributes.
 
         """
         chunk = ecosound.core.tools.tighten_signal_limits(self._waveform, energy_percentage)
         snip = self.select_snippet(chunk)
         self.__dict__.update(snip.__dict__)
 
@@ -498,24 +556,24 @@
         Defines coeeficient of the filter.
 
     """
 
     def __init__(self, type, cutoff_frequencies, order=4):
         """
         Initialize the filter.
-        
+
         Parameters
         ----------
         type : {'bandpass', 'lowpass', 'highpass'}
             Type of filter
         cutoff_frequencies : list of float
             Cut-off frequencies of the filter sorted in increasing order (i.e.
-            [lowcut, highcut]). If the filter type is 'bandpass' then 
-            cutoff_frequencies must be a list of 2 floats 
-            cutoff_frequencies=[lowcut, highcut], where lowcut < highcut. 
+            [lowcut, highcut]). If the filter type is 'bandpass' then
+            cutoff_frequencies must be a list of 2 floats
+            cutoff_frequencies=[lowcut, highcut], where lowcut < highcut.
             If the filter type is 'lowpass' or 'highpass' then cutoff_frequencies
             is a list with a single float.
         order : int, optional
             Order of the filter (default is 4)
 
         Raises
         ------
@@ -524,33 +582,33 @@
             If the filter type is not set to 'bandpass', 'lowpass', or 'highpass'
             If the cutoff_frequencies has not enough of too much values for the
             filter type selected or are not sorted by increasing frequencies.
         Returns
         -------
         None. Filter object.
 
-        """ 
+        """
         # chech filter type
         if (type == 'bandpass') | (type == 'lowpass') | (type == 'highpass') == 0:
-            raise ValueError('Wrong filter type. Must be "bandpass", "lowpass"' 
+            raise ValueError('Wrong filter type. Must be "bandpass", "lowpass"'
                              +', or "highpass".')
         # chech freq values
         if (type == 'bandpass'):
             if len(cutoff_frequencies) != 2:
                 raise ValueError('The type "bandpass" requires two frepuency '
                                  + 'values: cutoff_frequencies=[lowcut, '
                                  + 'highcut].')
             elif cutoff_frequencies[0] > cutoff_frequencies[1]:
                 raise ValueError('The lowcut value should be smaller than the '
                                  + 'highcut value: cutoff_frequencies=[lowcut,'
                                  + ' highcut].')
         elif (type == 'lowpass') | (type == 'highpass'):
             if len(cutoff_frequencies) != 1:
                 raise ValueError('The type "lowpass" and "highpass" require '
-                                 + 'one frepuency values cutoff_frequencies='
+                                 + 'one frequency value cutoff_frequencies='
                                  + '[cutfreq].')
         self.type = type
         self.cutoff_frequencies = cutoff_frequencies
         self.order = order
 
     def apply(self, waveform, sampling_frequency):
         """
@@ -565,16 +623,18 @@
 
         Returns
         -------
         numpy.ndarray
             Filtered time series.
 
         """
-        b, a = self.coefficients(sampling_frequency)
-        return spsig.lfilter(b, a, waveform)
+        #b, a = self.coefficients(sampling_frequency)
+        #return spsig.sosfiltfilt (b, a, waveform)
+        sos = self.coefficients(sampling_frequency)
+        return spsig.sosfiltfilt (sos, waveform)
 
     def coefficients(self, sampling_frequency):
         """
         Get filter coefficients.
 
         Parameters
         ----------
@@ -589,15 +649,53 @@
             Filter coefficient a.
 
         """
         nyquist = 0.5 * sampling_frequency
         if self.type == 'bandpass':
             low = self.cutoff_frequencies[0] / nyquist
             high = self.cutoff_frequencies[1] / nyquist
-            b, a = spsig.butter(self.order, [low, high], btype='band')
+            #b, a = spsig.butter(self.order, [low, high], btype='band')
+            sos = spsig.butter(self.order, [low, high], btype='band', output='sos')
         elif self.type == 'lowpass':
-            b, a = spsig.butter(self.order,
-                                self.cutoff_frequencies[0]/nyquist, 'low')
+            # b, a = spsig.butter(self.order,
+            #                     self.cutoff_frequencies[0]/nyquist, 'low')
+            sos = spsig.butter(self.order,
+                                self.cutoff_frequencies[0]/nyquist, 'low',output='sos')
         elif self.type == 'highpass':
-            b, a = spsig.butter(self.order,
-                                self.cutoff_frequencies[0]/nyquist, 'high')
-        return b, a
+            # b, a = spsig.butter(self.order,
+            #                     self.cutoff_frequencies[0]/nyquist, 'high')
+            sos = spsig.butter(self.order,
+                                self.cutoff_frequencies[0]/nyquist, 'high',output='sos')
+        return sos
+
+
+def upsample(waveform, current_res_sec, new_res_sec):
+        """
+        Upsample  waveform
+
+        Increase the number of samples in the waveform and interpolate.
+
+        Parameters
+        ----------
+        waveform: 1D array
+            Waveform to upsample
+        current_res_sec : float
+            Time resolution of waveform in seconds. It is the inverse of the
+            sampling frequency.
+        new_res_sec : float
+            New time resolution of waveform after interpolation (in seconds).
+
+        Returns
+        -------
+        waveform: 1D array
+            waveform upsampled to have a time resolution of "new_res_sec".
+
+        """
+        axis_t = np.arange(0, len(waveform)*current_res_sec, current_res_sec)
+        new_fs = round(1/new_res_sec)
+        nb_samp = round(axis_t[-1]*new_fs)
+        new_waveform, new_axis_t = spsig.resample(waveform,
+                                                  nb_samp,
+                                                  t=axis_t,
+                                                  window='hann',
+                                                  )
+        return new_waveform, new_fs
```

### Comparing `ecosound-0.0.8/ecosound/core/decorators.py` & `ecosound-0.0.9/ecosound/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/core/measurement.py` & `ecosound-0.0.9/ecosound/core/measurement.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/core/metadata.py` & `ecosound-0.0.9/ecosound/core/metadata.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/core/spectrogram.py` & `ecosound-0.0.9/ecosound/core/spectrogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     Methods
     -------
     compute(sig, fs)
         Compute spectrogram.
     crop(frequency_min, frequency_max)
         Crop frequencies from the spectrogram.
     denoise(method, **kwargs)
-        Denoise the spectrogram using various methods. 
+        Denoise the spectrogram using various methods.
         Methods implemented:
         METHODS           :    INPUT ARGUMENTS
         'median_equalizer':    window_duration in seconds.
     """
 
     _valid_units = ('samp', 'sec')
     _valid_windows = ('hann',)
@@ -89,15 +89,15 @@
         window_type : str
             Weighting window to teh signal before the FFT. Currently, only
             'hann' is supported.
         fft : float
             Size of the Fast Fourier Transform, in seconds or samples,
             depending on 'unit'.
         step : float
-            Time step between conscutive spectrogram frames. In samples or 
+            Time step between conscutive spectrogram frames. In samples or
             seconds depending on 'unit'.
         sampling_frequency : float
             Sampling frequency of the signal, in Hz.
         unit : str, optional
             Unit used when defining the 'frame' and 'fft' parameters. For
             seconds, use 'sec'. For samples, use 'samp'. The default is 'sec'.
 
@@ -142,14 +142,15 @@
         elif unit == 'samp':
             frame_samp = frame
             fft_samp = adjust_FFT_size(fft)
             step_samp = step
             frame_sec = frame/sampling_frequency
             fft_sec = fft_samp/sampling_frequency
             step_sec = step/sampling_frequency
+
         overlap_samp = frame_samp-step_samp
         overlap_perc = (overlap_samp/frame_samp)*100
         return frame_samp, fft_samp, step_samp, frame_sec, fft_sec, step_sec, overlap_perc,overlap_samp
 
     def _compute_old(self, sig):
         """
         Compute spectrogram.
@@ -334,40 +335,40 @@
                 max_col_idx = self._axis_times.size-1
             else:
                 max_col_idx = max_col_idx[0][0]
         # update spectrogram and axes
         if inplace:
             # self._axis_frequencies = self._axis_frequencies[min_row_idx:max_row_idx]
             # self._axis_times = np.arange(0,(max_col_idx - min_col_idx)*self._time_resolution,self._time_resolution)
-            # self._spectrogram = self._spectrogram[min_row_idx:max_row_idx, min_col_idx:max_col_idx]   
+            # self._spectrogram = self._spectrogram[min_row_idx:max_row_idx, min_col_idx:max_col_idx]
             # out_object = None
             self._axis_frequencies = self._axis_frequencies[min_row_idx:max_row_idx+1]
             self._axis_times = self._axis_times[min_col_idx:max_col_idx+1]-self._axis_times[min_col_idx]
-            self._spectrogram = self._spectrogram[min_row_idx:max_row_idx+1, min_col_idx:max_col_idx+1]   
+            self._spectrogram = self._spectrogram[min_row_idx:max_row_idx+1, min_col_idx:max_col_idx+1]
             out_object = None
         else:
             out_object = copy.copy(self)
             out_object._axis_frequencies = out_object._axis_frequencies[min_row_idx:max_row_idx+1]
             #out_object._axis_times = np.arange(0,(max_col_idx - min_col_idx)*out_object._time_resolution,out_object._time_resolution)
             out_object._axis_times = out_object._axis_times[min_col_idx:max_col_idx+1]-out_object._axis_times[min_col_idx]
-            #out_object._spectrogram = out_object._spectrogram[min_row_idx:max_row_idx, min_col_idx:max_col_idx]   
+            #out_object._spectrogram = out_object._spectrogram[min_row_idx:max_row_idx, min_col_idx:max_col_idx]
             out_object._spectrogram = out_object._spectrogram[min_row_idx:max_row_idx+1, min_col_idx:max_col_idx+1]
             if out_object._spectrogram.shape[1] != len(out_object._axis_times):
                 raise ValueError("Spectrogram axes don't match spectrogram matrix.")
         return out_object
 
     def denoise(self, method, **kwargs):
         """
         Denoise spectrogram.
 
         Denoise the spectrogram using various methods. The methods implemented
         are:
             METHODS           :    INPUT ARGUMENTS
             'median_equalizer':    window_duration in seconds.
-                                   inplace 
+                                   inplace
 
         Parameters
         ----------
         method : str
             DESCRIPTION.
         **kwargs : variable
             Parameters for the methods selected.
@@ -429,15 +430,15 @@
         if inplace:
             self._spectrogram = self._spectrogram-Smed
             self._spectrogram[self._spectrogram < 0] = 0  # floor
             out_object = None
         else:
             out_object = copy.copy(self)
             out_object._spectrogram = out_object._spectrogram-Smed
-            out_object._spectrogram[out_object._spectrogram < 0] = 0  # floor            
+            out_object._spectrogram[out_object._spectrogram < 0] = 0  # floor
         return out_object
 
     @property
     def frame_samp(self):
         """Return the frame_samp attribute."""
         return self._frame_samp
```

### Comparing `ecosound-0.0.8/ecosound/detection/blob_detector.py` & `ecosound-0.0.9/ecosound/detection/blob_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,20 @@
         detec.data['software_name'] = self.name
         detec.data['software_version'] = self.version
         detec.data['entry_date'] = datetime.now()
         detec.data['uuid'] = detec.data.apply(lambda _: str(uuid.uuid4()), axis=1)
         if start_time:
             detec.data['time_min_date']= pd.to_datetime(start_time + pd.to_timedelta(detec.data['time_min_offset'], unit='s'))
             detec.data['time_max_date']= pd.to_datetime(start_time + pd.to_timedelta(detec.data['time_max_offset'], unit='s'))
+        # sort by ascending order
+        detec.data.sort_values('time_min_offset',
+                               ascending=True,
+                               inplace=True,
+                               ignore_index=True,
+                               )
         return detec
 
 @njit()
 def calcVariance2D(buffer):
     """Calculate the 2D variance."""
     return np.var(buffer)
     # return np.median(buffer.ravel())
```

### Comparing `ecosound-0.0.8/ecosound/detection/detector_builder.py` & `ecosound-0.0.9/ecosound/detection/detector_builder.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/detection/detector_template.py` & `ecosound-0.0.9/ecosound/detection/detector_template.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/detection/kurtosis_detector.py` & `ecosound-0.0.9/ecosound/detection/kurtosis_detector.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/measurements/measurer_builder.py` & `ecosound-0.0.9/ecosound/measurements/measurer_builder.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/measurements/measurer_template.py` & `ecosound-0.0.9/ecosound/measurements/measurer_template.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/measurements/spectrogram_features.py` & `ecosound-0.0.9/ecosound/measurements/spectrogram_features.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/visualization/grapher_builder.py` & `ecosound-0.0.9/ecosound/visualization/grapher_builder.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/ecosound/visualization/sound_plotter.py` & `ecosound-0.0.9/ecosound/visualization/sound_plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
     @property
     def version(self):
         """Return version of the grapher."""
         version = '0.1'
         return version
 
-    def add_data(self, *args):
+    def add_data(self, *args, time_offset_sec=0):
         """
         Define sound or spectrogram data to plot.
 
         Add Sound or Spectrogram objects to plot. There is no restriction on
         the number of object to add. Each object will be displayed on a
         different subplot of the same figure. The order in which the objects
         are passed to this method defines the order in which they are displayed
@@ -187,15 +187,16 @@
         -------
         None. Updated grapher object.
 
         """
         if len(args) < 1:
             raise ValueError('There must be at least one input argument')
         # Check  type of each input arguments
-        self._stack_data(args)
+        self._stack_data(args, time_offset_sec=time_offset_sec)
+
 
     def add_annotation(self, annotation, panel=None, label=False, color='red', tag=False, line_width=1):
         """
         Define annotations to display.
 
         When this method is called several times; ANnotation objects are
         appended to the existing list of objects from previous calls.
@@ -308,17 +309,17 @@
         # Plot data
         for idx, data in enumerate(self.data):
             if nb_plots == 1:
                 current_ax = ax
             else:
                 current_ax = ax[idx]
             if data['type'] == 'waveform':
-                self._plot_waveform(data['data'], current_ax, title=titles[idx])
+                self._plot_waveform(data['data'], current_ax, time_offset_sec=data['time_offset_sec'], title=titles[idx])
             elif data['type'] == 'spectrogram':
-                self._plot_spectrogram(data['data'], current_ax, title=titles[idx])
+                self._plot_spectrogram(data['data'], current_ax, time_offset_sec=data['time_offset_sec'], title=titles[idx])
             # only dipslay x label of bottom plot if shared axes
             if self.share_xaxis and (idx != nb_plots-1):
                 current_ax.set_xlabel('')
 
         # Plot annotations
         for idx_annot, annot in enumerate(self.annotations):  # for each set of annotations
             # display annotations on all panels
@@ -343,15 +344,15 @@
 									   line_width = annot['line_width'],
                                        )
                 if annot['label'] is not False:
                     handles, labels = current_ax.get_legend_handles_labels()
                     unique_labels=list(set(labels))
                     new_handles=[]
                     for l in unique_labels:
-                        new_handles.append(handles[labels.index(l)])                        
+                        new_handles.append(handles[labels.index(l)])
                     current_ax.legend(new_handles,unique_labels,loc='upper right')
 
                 if annot['tag'] is True:
                     bbox_props = dict(boxstyle="square", fc="w", ec="w", alpha=0.8)
                     panel_type = self.data[annot['panel'][0]]['type']
                     for index, row in annot['data'].data.iterrows():
                         if self.unit == 'sec':
@@ -366,16 +367,16 @@
                             x = row['time_min_offset']
                             if panel_type == 'spectrogram':
                                 y = row['frequency_max']
                             elif panel_type == 'waveform':
                                 y = max(current_ax.get_ylim())
                             conf = str(round(row['confidence'],2))
                         current_ax.text(x, y, conf, size=8, bbox=bbox_props)
-                    
-                
+
+
         return fig, ax
 
     def to_file(self, filename):
         """
         Save the figure to an image file.
 
         Parameters
@@ -428,45 +429,48 @@
                                  linewidth=line_width,
                                  edgecolor=color,
                                  facecolor=facecolor,
                                  alpha=alpha,
                                  label=label)
             ax.add_patch(rect)
 
-    def _stack_data(self, args):
+    def _stack_data(self, args, time_offset_sec=0):
         """Stack data to be plotted."""
         for idx, arg in enumerate(args):
             if isinstance(arg, Sound):
-                self.data.append({'data': arg, 'type': 'waveform'})
+                self.data.append({'data': arg, 'type': 'waveform', 'time_offset_sec': time_offset_sec})
             elif isinstance(arg, Spectrogram):
-                self.data.append({'data': arg, 'type': 'spectrogram'})
+                self.data.append({'data': arg, 'type': 'spectrogram', 'time_offset_sec': time_offset_sec})
             else:
                 raise ValueError('Type of input argument not recognized.'
                                  'Accepted object types: Spectrogram, Sound')
 
-    def _plot_spectrogram(self, spectro, current_ax, title=None):
+    def _plot_spectrogram(self, spectro, current_ax, time_offset_sec=0, title=None):
         """Plot spectrogram on the current axis"""
         if self.frequency_max is None:
             self.frequency_max = spectro.sampling_frequency/2
         assert len(spectro.spectrogram) > 0, "Spectrogram not computed yet. "
         "Use the .compute() method first."
+        # add time offset if defined
+        spectro._axis_times = spectro.axis_times + time_offset_sec
         if self.unit == 'sec':
             if self.time_max is None:
                 self.time_max = spectro.axis_times[-1]
             current_ax.pcolormesh(spectro.axis_times,
                                   spectro.axis_frequencies,
                                   spectro.spectrogram,
                                   cmap=self.colormap,
                                   vmin=np.percentile(spectro.spectrogram, 50),
                                   vmax=np.percentile(spectro.spectrogram, 99.9),
 								  shading='nearest',
                                   )
             xlabel = 'Time (sec)'
         elif self.unit == 'samp':
             axis_t = np.arange(0, len(spectro.axis_times), 1)
+            axis_t = axis_t + round(time_offset_sec/spectro.time_resolution)
             if self.time_max is None:
                 self.time_max = axis_t[-1]
             current_ax.pcolormesh(axis_t,
                                   spectro.axis_frequencies,
                                   spectro.spectrogram,
                                   cmap=self.colormap,
                                   vmin=np.percentile(spectro.spectrogram, 50),
@@ -484,38 +488,40 @@
         current_ax.set_ylabel('Frequency (Hz)')
         current_ax.set_xlabel(xlabel)
         current_ax.set_title(title)
         # if self.grid:
         #    current_ax.grid()
         return
 
-    def _plot_waveform(self, sound, current_ax, title=None):
+    def _plot_waveform(self, sound, current_ax, time_offset_sec=0, title=None):
         """Plot waveform of a sound object on the current axis."""
         if len(sound._waveform) == 0:
             raise ValueError('Cannot plot, waveform data enpty. Use Sound.read'
                              + ' to load the waveform')
         if self.unit == 'sec':
             axis_t = np.arange(0, sound.waveform_duration_sample
                                / sound.waveform_sampling_frequency, 1
                                / sound.waveform_sampling_frequency)
+            axis_t = axis_t + time_offset_sec
             xlabel = 'Time (sec)'
         elif self.unit == 'samp':
             axis_t = np.arange(0, len(sound._waveform), 1)
+            axis_t = axis_t + (time_offset_sec*sound.waveform_sampling_frequency)
             xlabel = 'Time (sample)'
         else:
             raise ValueError("Keyword 'unit' must be set to either 'sec' or"
                              " 'samp'.")
         if self.time_max is None:
                 self.time_max = axis_t[-1]
         #axis_t = axis_t[0:len(sound._waveform)]
-        current_ax.plot(axis_t, sound._waveform, color='black')
+        current_ax.plot(axis_t[0:len(sound._waveform)], sound._waveform, color='black')
         current_ax.set_xlabel(xlabel)
         current_ax.set_ylabel('Amplitude')
         current_ax.set_title(title)
-        
+
         current_ax.axis([self.time_min,
                          self.time_max,
                          min(sound._waveform),
                          max(sound._waveform)]
         # current_ax.axis([axis_t[0],
         #                  axis_t[-1],
         #                  min(sound._waveform),
```

### Comparing `ecosound-0.0.8/setup.py` & `ecosound-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 	classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: BSD License", 
         "Operating System :: OS Independent",
         "Natural Language :: English",
     ],
-    python_requires='>=3.7.0, <3.9.0',
+    python_requires='>=3.7.0',
 	zip_safe=False,
 )
```

### Comparing `ecosound-0.0.8/tests/old_tests/Add_metadat_to_detections.py` & `ecosound-0.0.9/tests/old_tests/Add_metadat_to_detections.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/Annot_overlap.py` & `ecosound-0.0.9/tests/old_tests/Annot_overlap.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/Annotations.py` & `ecosound-0.0.9/tests/old_tests/Annotations.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/Classify.py` & `ecosound-0.0.9/tests/old_tests/Classify.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/ConvertDetect2raven.ipynb` & `ecosound-0.0.9/tests/old_tests/ConvertDetect2raven.ipynb`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/Investigate_detection_difference.py` & `ecosound-0.0.9/tests/old_tests/Investigate_detection_difference.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/Measurements.py` & `ecosound-0.0.9/tests/old_tests/Measurements.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/Troubleshoot_xarray_combine.py` & `ecosound-0.0.9/tests/old_tests/Troubleshoot_xarray_combine.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/aTest_Xarray2.ipynb` & `ecosound-0.0.9/tests/old_tests/aTest_Xarray2.ipynb`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_dask-image.py` & `ecosound-0.0.9/tests/old_tests/atest_dask-image.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_dask.py` & `ecosound-0.0.9/tests/old_tests/atest_dask.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_dask2.py` & `ecosound-0.0.9/tests/old_tests/atest_dask2.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_dask3.py` & `ecosound-0.0.9/tests/old_tests/atest_dask3.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_save_pamlab.py` & `ecosound-0.0.9/tests/old_tests/atest_save_pamlab.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_xarray.ipynb` & `ecosound-0.0.9/tests/old_tests/atest_xarray.ipynb`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/atest_xarray.py` & `ecosound-0.0.9/tests/old_tests/atest_xarray.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/audiotools.py` & `ecosound-0.0.9/tests/old_tests/audiotools.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/blob_detector.py` & `ecosound-0.0.9/tests/old_tests/blob_detector.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/check_netcdf_valid.py` & `ecosound-0.0.9/tests/old_tests/check_netcdf_valid.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/classification.py` & `ecosound-0.0.9/tests/old_tests/classification.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/classification_datasets.py` & `ecosound-0.0.9/tests/old_tests/classification_datasets.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/dask_tutorial.py` & `ecosound-0.0.9/tests/old_tests/dask_tutorial.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/detector_batch.py` & `ecosound-0.0.9/tests/old_tests/detector_batch.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/detector_batch_parralel_run.py` & `ecosound-0.0.9/tests/old_tests/detector_batch_parralel_run.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/display_annot_detec.py` & `ecosound-0.0.9/tests/old_tests/display_annot_detec.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/display_annot_detec_documentation.py` & `ecosound-0.0.9/tests/old_tests/display_annot_detec_documentation.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/extract_hourly_detec_summary.py` & `ecosound-0.0.9/tests/old_tests/extract_hourly_detec_summary.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/extract_hourly_detec_summary_raven.py` & `ecosound-0.0.9/tests/old_tests/extract_hourly_detec_summary_raven.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/extract_hourly_detec_summary_v2.py` & `ecosound-0.0.9/tests/old_tests/extract_hourly_detec_summary_v2.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/filter_detections.py` & `ecosound-0.0.9/tests/old_tests/filter_detections.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/plot_ambient_sound.ipynb` & `ecosound-0.0.9/tests/old_tests/plot_ambient_sound.ipynb`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/plot_timeseries.py` & `ecosound-0.0.9/tests/old_tests/plot_timeseries.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/re_classify_measurements.py` & `ecosound-0.0.9/tests/old_tests/re_classify_measurements.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/relabel_FP_as_noise_annot.py` & `ecosound-0.0.9/tests/old_tests/relabel_FP_as_noise_annot.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/spectrogram.py` & `ecosound-0.0.9/tests/old_tests/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/spectrogram_classifier.py` & `ecosound-0.0.9/tests/old_tests/spectrogram_classifier.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/spectrogram_measurer.py` & `ecosound-0.0.9/tests/old_tests/spectrogram_measurer.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/old_tests/time_series_plotter.py` & `ecosound-0.0.9/tests/old_tests/time_series_plotter.py`

 * *Files identical despite different names*

### Comparing `ecosound-0.0.8/tests/test_core_annotation.py` & `ecosound-0.0.9/tests/test_core_annotation.py`

 * *Files identical despite different names*

