# Comparing `tmp/mdata-0.1.1.tar.gz` & `tmp/mdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdata-0.1.1.tar", max compression
+gzip compressed data, was "mdata-0.1.2.tar", max compression
```

## Comparing `mdata-0.1.1.tar` & `mdata-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,94 @@
--rw-r--r--   0        0        0      748 2023-06-12 10:06:57.700377 mdata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      335 2023-05-24 11:21:39.824410 mdata-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 08:17:06.548381 mdata-0.1.1/src/mdata/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 14:47:33.159982 mdata-0.1.1/src/mdata/analysis/__init__.py
--rw-r--r--   0        0        0      159 2023-05-19 08:45:38.105261 mdata-0.1.1/src/mdata/analysis/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      983 2023-05-19 08:57:03.979460 mdata-0.1.1/src/mdata/analysis/__pycache__/frequency.cpython-310.pyc
--rw-r--r--   0        0        0      811 2023-05-19 08:57:03.895576 mdata-0.1.1/src/mdata/analysis/frequency.py
--rw-r--r--   0        0        0        0 2023-05-03 09:02:31.524432 mdata-0.1.1/src/mdata/conversions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 09:02:40.138181 mdata-0.1.1/src/mdata/conversions/ocel/__init__.py
--rw-r--r--   0        0        0      628 2023-05-15 11:42:34.414564 mdata-0.1.1/src/mdata/conversions/ocel/ocel_export.py
--rw-r--r--   0        0        0       93 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/__init__.py
--rw-r--r--   0        0        0      269 2023-06-06 12:51:51.634919 mdata-0.1.1/src/mdata/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      928 2023-05-02 08:49:05.625504 mdata-0.1.1/src/mdata/core/__pycache__/df_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2528 2023-06-09 07:53:36.177943 mdata-0.1.1/src/mdata/core/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0    25359 2023-06-09 09:11:52.707247 mdata-0.1.1/src/mdata/core/__pycache__/machine_data_def.cpython-310.pyc
--rw-r--r--   0        0        0     4554 2023-06-09 07:53:36.194313 mdata-0.1.1/src/mdata/core/__pycache__/raw.cpython-310.pyc
--rw-r--r--   0        0        0     2275 2023-06-06 14:36:56.531531 mdata-0.1.1/src/mdata/core/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0      427 2023-05-02 08:49:05.536425 mdata-0.1.1/src/mdata/core/df_utils.py
--rw-r--r--   0        0        0        0 2023-04-24 11:51:58.667588 mdata-0.1.1/src/mdata/core/extensions/__init__.py
--rw-r--r--   0        0        0      166 2023-05-25 08:35:08.557253 mdata-0.1.1/src/mdata/core/extensions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7266 2023-06-09 08:03:27.599571 mdata-0.1.1/src/mdata/core/extensions/__pycache__/multiplicity.cpython-310.pyc
--rw-r--r--   0        0        0     5949 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/extensions/multiplicity.py
--rw-r--r--   0        0        0     2555 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/factory.py
--rw-r--r--   0        0        0    23958 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/machine_data_def.py
--rw-r--r--   0        0        0     5913 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/raw.py
--rw-r--r--   0        0        0     2034 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/util.py
--rw-r--r--   0        0        0      197 2023-05-17 08:59:22.605542 mdata-0.1.1/src/mdata/file_formats/__init__.py
--rw-r--r--   0        0        0      423 2023-05-17 09:17:42.509792 mdata-0.1.1/src/mdata/file_formats/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2121 2023-05-26 09:19:56.195531 mdata-0.1.1/src/mdata/file_formats/__pycache__/io_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2598 2023-05-04 13:47:40.526847 mdata-0.1.1/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-310.pyc
--rw-r--r--   0        0        0      265 2023-05-04 14:37:13.900246 mdata-0.1.1/src/mdata/file_formats/csv/__init__.py
--rw-r--r--   0        0        0      427 2023-05-04 14:37:18.586529 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3118 2023-06-09 07:53:36.166471 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/checking.cpython-310.pyc
--rw-r--r--   0        0        0     2403 2023-05-11 09:07:39.679690 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/exporting.cpython-310.pyc
--rw-r--r--   0        0        0     2672 2023-06-09 07:53:36.194313 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/importing.cpython-310.pyc
--rw-r--r--   0        0        0      403 2023-05-03 08:54:22.483484 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/shared.cpython-310.pyc
--rw-r--r--   0        0        0     3155 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/csv/checking.py
--rw-r--r--   0        0        0     2317 2023-05-11 09:02:15.344654 mdata-0.1.1/src/mdata/file_formats/csv/exporting.py
--rw-r--r--   0        0        0     3141 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/csv/importing.py
--rw-r--r--   0        0        0      164 2023-05-03 08:54:22.395411 mdata-0.1.1/src/mdata/file_formats/csv/shared.py
--rw-r--r--   0        0        0      145 2023-04-27 12:35:27.078537 mdata-0.1.1/src/mdata/file_formats/hdf/__init__.py
--rw-r--r--   0        0        0      276 2023-04-27 12:35:59.963859 mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1392 2023-06-09 10:14:18.666516 mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-310.pyc
--rw-r--r--   0        0        0     1079 2023-06-09 07:53:36.194313 mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/importing.cpython-310.pyc
--rw-r--r--   0        0        0      190 2023-04-21 14:16:55.019498 mdata-0.1.1/src/mdata/file_formats/hdf/checking.py
--rw-r--r--   0        0        0     1236 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/hdf/exporting.py
--rw-r--r--   0        0        0     1303 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/hdf/importing.py
--rw-r--r--   0        0        0     2183 2023-06-12 10:06:09.254151 mdata-0.1.1/src/mdata/file_formats/io_utils.py
--rw-r--r--   0        0        0     1953 2023-05-04 13:47:40.474562 mdata-0.1.1/src/mdata/file_formats/validity_checking_utils.py
--rw-r--r--   0        0        0      155 2023-05-22 11:21:08.266604 mdata-0.1.1/src/mdata/visualization/__init__.py
--rw-r--r--   0        0        0      355 2023-05-22 11:21:08.475981 mdata-0.1.1/src/mdata/visualization/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1387 2023-06-06 12:53:23.808361 mdata-0.1.1/src/mdata/visualization/__pycache__/matplot.cpython-310.pyc
--rw-r--r--   0        0        0     6654 2023-06-09 10:23:17.455905 mdata-0.1.1/src/mdata/visualization/__pycache__/plotting.cpython-310.pyc
--rw-r--r--   0        0        0     1102 2023-06-12 10:06:09.254151 mdata-0.1.1/src/mdata/visualization/matplot.py
--rw-r--r--   0        0        0     7745 2023-06-12 10:06:09.254151 mdata-0.1.1/src/mdata/visualization/plotting.py
--rw-r--r--   0        0        0      269 2023-04-24 13:27:36.152567 mdata-0.1.1/src/mdata/visualization/textual.py
--rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 mdata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-07-31 08:44:07.626727 mdata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-05-24 11:21:39.824410 mdata-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 08:17:06.548381 mdata-0.1.2/src/mdata/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:47:33.159982 mdata-0.1.2/src/mdata/analysis/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-19 08:45:38.105261 mdata-0.1.2/src/mdata/analysis/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      983 2023-05-19 08:57:03.979460 mdata-0.1.2/src/mdata/analysis/__pycache__/frequency.cpython-310.pyc
+-rw-r--r--   0        0        0      813 2023-07-31 08:42:10.789100 mdata-0.1.2/src/mdata/analysis/frequency.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:02:31.524432 mdata-0.1.2/src/mdata/conversions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:02:40.138181 mdata-0.1.2/src/mdata/conversions/ocel/__init__.py
+-rw-r--r--   0        0        0      628 2023-07-31 08:42:10.790750 mdata-0.1.2/src/mdata/conversions/ocel/ocel_export.py
+-rw-r--r--   0        0        0       94 2023-07-31 08:42:10.790750 mdata-0.1.2/src/mdata/core/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-22 13:03:56.284347 mdata-0.1.2/src/mdata/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      277 2023-07-25 14:46:05.021067 mdata-0.1.2/src/mdata/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      928 2023-05-02 08:49:05.625504 mdata-0.1.2/src/mdata/core/__pycache__/df_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1370 2023-07-21 11:28:35.393077 mdata-0.1.2/src/mdata/core/__pycache__/df_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     2528 2023-06-23 13:21:03.857649 mdata-0.1.2/src/mdata/core/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     5523 2023-07-26 10:44:49.531281 mdata-0.1.2/src/mdata/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     7319 2023-06-23 14:40:43.086571 mdata-0.1.2/src/mdata/core/__pycache__/header.cpython-310.pyc
+-rw-r--r--   0        0        0    16098 2023-07-28 13:46:51.073836 mdata-0.1.2/src/mdata/core/__pycache__/header.cpython-311.pyc
+-rw-r--r--   0        0        0    23541 2023-07-21 09:41:19.548768 mdata-0.1.2/src/mdata/core/__pycache__/machine_data_def.cpython-310.pyc
+-rw-r--r--   0        0        0    47735 2023-07-28 14:58:24.887395 mdata-0.1.2/src/mdata/core/__pycache__/machine_data_def.cpython-311.pyc
+-rw-r--r--   0        0        0     5155 2023-06-23 14:43:21.183472 mdata-0.1.2/src/mdata/core/__pycache__/raw.cpython-310.pyc
+-rw-r--r--   0        0        0     8961 2023-07-25 14:46:04.921635 mdata-0.1.2/src/mdata/core/__pycache__/raw.cpython-311.pyc
+-rw-r--r--   0        0        0     4049 2023-06-22 13:43:35.657351 mdata-0.1.2/src/mdata/core/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0     6522 2023-07-25 14:46:03.911359 mdata-0.1.2/src/mdata/core/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0      427 2023-05-02 08:49:05.536425 mdata-0.1.2/src/mdata/core/df_utils.py
+-rw-r--r--   0        0        0      228 2023-07-31 08:42:10.792010 mdata-0.1.2/src/mdata/core/extensions/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-22 13:15:16.520453 mdata-0.1.2/src/mdata/core/extensions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      249 2023-07-25 14:46:04.036823 mdata-0.1.2/src/mdata/core/extensions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      905 2023-06-22 13:43:35.663453 mdata-0.1.2/src/mdata/core/extensions/__pycache__/annotations.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2023-07-25 14:46:04.040140 mdata-0.1.2/src/mdata/core/extensions/__pycache__/annotations.cpython-311.pyc
+-rw-r--r--   0        0        0     3257 2023-07-21 09:41:19.554851 mdata-0.1.2/src/mdata/core/extensions/__pycache__/metadata.cpython-310.pyc
+-rw-r--r--   0        0        0     8335 2023-07-25 14:46:04.056987 mdata-0.1.2/src/mdata/core/extensions/__pycache__/metadata.cpython-311.pyc
+-rw-r--r--   0        0        0     7266 2023-06-22 12:50:54.230359 mdata-0.1.2/src/mdata/core/extensions/__pycache__/multiplicity.cpython-310.pyc
+-rw-r--r--   0        0        0      565 2023-06-22 13:43:14.287133 mdata-0.1.2/src/mdata/core/extensions/__pycache__/registry.cpython-310.pyc
+-rw-r--r--   0        0        0      726 2023-07-25 14:46:04.014187 mdata-0.1.2/src/mdata/core/extensions/__pycache__/registry.cpython-311.pyc
+-rw-r--r--   0        0        0      583 2023-07-31 08:42:10.792010 mdata-0.1.2/src/mdata/core/extensions/annotations.py
+-rw-r--r--   0        0        0     4693 2023-07-31 08:42:10.793434 mdata-0.1.2/src/mdata/core/extensions/metadata.py
+-rw-r--r--   0        0        0     5921 2023-07-31 08:42:10.793434 mdata-0.1.2/src/mdata/core/extensions/multiplicity.py
+-rw-r--r--   0        0        0      279 2023-07-31 08:42:10.794440 mdata-0.1.2/src/mdata/core/extensions/registry.py
+-rw-r--r--   0        0        0      447 2023-07-31 08:42:10.794440 mdata-0.1.2/src/mdata/core/extensions/segmentation.py
+-rw-r--r--   0        0        0     3273 2023-07-31 08:42:10.795440 mdata-0.1.2/src/mdata/core/factory.py
+-rw-r--r--   0        0        0     7771 2023-07-31 08:42:10.796440 mdata-0.1.2/src/mdata/core/header.py
+-rw-r--r--   0        0        0    25650 2023-07-31 08:42:10.796440 mdata-0.1.2/src/mdata/core/machine_data_def.py
+-rw-r--r--   0        0        0     5637 2023-07-31 08:42:10.797440 mdata-0.1.2/src/mdata/core/raw.py
+-rw-r--r--   0        0        0     3019 2023-07-31 08:42:10.798440 mdata-0.1.2/src/mdata/core/util.py
+-rw-r--r--   0        0        0      183 2023-07-31 08:42:10.798655 mdata-0.1.2/src/mdata/file_formats/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-17 09:17:42.509792 mdata-0.1.2/src/mdata/file_formats/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      485 2023-07-31 08:34:08.712253 mdata-0.1.2/src/mdata/file_formats/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2428 2023-06-22 07:58:14.962611 mdata-0.1.2/src/mdata/file_formats/__pycache__/io_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     5129 2023-07-25 14:46:05.041922 mdata-0.1.2/src/mdata/file_formats/__pycache__/io_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     2845 2023-06-22 07:58:14.975746 mdata-0.1.2/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2023-07-25 14:46:05.074101 mdata-0.1.2/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-311.pyc
+-rw-r--r--   0        0        0      251 2023-07-31 08:42:10.799889 mdata-0.1.2/src/mdata/file_formats/csv/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-04 14:37:18.586529 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      495 2023-07-31 08:34:08.713981 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4401 2023-06-22 13:59:35.522310 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/checking.cpython-310.pyc
+-rw-r--r--   0        0        0     8815 2023-07-31 08:34:08.717223 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/checking.cpython-311.pyc
+-rw-r--r--   0        0        0     3767 2023-06-22 08:30:59.383717 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/exporting.cpython-310.pyc
+-rw-r--r--   0        0        0    11794 2023-07-31 08:34:09.294572 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/exporting.cpython-311.pyc
+-rw-r--r--   0        0        0     4582 2023-06-22 10:03:20.690848 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/importing.cpython-310.pyc
+-rw-r--r--   0        0        0     8639 2023-07-31 08:34:09.286491 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/importing.cpython-311.pyc
+-rw-r--r--   0        0        0      514 2023-06-20 13:51:47.407662 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/shared.cpython-310.pyc
+-rw-r--r--   0        0        0     1134 2023-07-25 14:46:05.041922 mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/shared.cpython-311.pyc
+-rw-r--r--   0        0        0     5263 2023-07-31 08:42:10.799889 mdata-0.1.2/src/mdata/file_formats/csv/checking.py
+-rw-r--r--   0        0        0     5710 2023-07-31 08:42:10.800903 mdata-0.1.2/src/mdata/file_formats/csv/exporting.py
+-rw-r--r--   0        0        0     5963 2023-07-31 08:42:10.800903 mdata-0.1.2/src/mdata/file_formats/csv/importing.py
+-rw-r--r--   0        0        0      483 2023-07-31 08:42:10.801902 mdata-0.1.2/src/mdata/file_formats/csv/shared.py
+-rw-r--r--   0        0        0      145 2023-04-27 12:35:27.078537 mdata-0.1.2/src/mdata/file_formats/hdf/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-27 12:35:59.963859 mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      324 2023-07-21 11:28:35.575053 mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1456 2023-06-20 13:51:47.417660 mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-310.pyc
+-rw-r--r--   0        0        0     4698 2023-07-25 14:46:05.334922 mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-311.pyc
+-rw-r--r--   0        0        0     1079 2023-06-20 13:51:47.415663 mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/importing.cpython-310.pyc
+-rw-r--r--   0        0        0     4696 2023-07-25 14:46:05.313861 mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/importing.cpython-311.pyc
+-rw-r--r--   0        0        0      190 2023-04-21 14:16:55.019498 mdata-0.1.2/src/mdata/file_formats/hdf/checking.py
+-rw-r--r--   0        0        0     2493 2023-07-31 08:42:10.802904 mdata-0.1.2/src/mdata/file_formats/hdf/exporting.py
+-rw-r--r--   0        0        0     3147 2023-07-31 08:42:10.803203 mdata-0.1.2/src/mdata/file_formats/hdf/importing.py
+-rw-r--r--   0        0        0     4829 2023-07-31 08:42:10.803833 mdata-0.1.2/src/mdata/file_formats/header_schema.json
+-rw-r--r--   0        0        0     2818 2023-07-31 08:42:10.804814 mdata-0.1.2/src/mdata/file_formats/io_utils.py
+-rw-r--r--   0        0        0     4530 2023-07-31 08:42:10.805000 mdata-0.1.2/src/mdata/file_formats/schema_template.json
+-rw-r--r--   0        0        0     2218 2023-07-31 08:42:10.806087 mdata-0.1.2/src/mdata/file_formats/validity_checking_utils.py
+-rw-r--r--   0        0        0       32 2023-07-31 08:42:10.806773 mdata-0.1.2/src/mdata/io/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-22 11:21:08.266604 mdata-0.1.2/src/mdata/visualization/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-22 11:21:08.475981 mdata-0.1.2/src/mdata/visualization/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      413 2023-07-21 11:28:35.584583 mdata-0.1.2/src/mdata/visualization/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1387 2023-06-13 11:11:58.321484 mdata-0.1.2/src/mdata/visualization/__pycache__/matplot.cpython-310.pyc
+-rw-r--r--   0        0        0     2514 2023-07-25 14:46:05.390789 mdata-0.1.2/src/mdata/visualization/__pycache__/matplot.cpython-311.pyc
+-rw-r--r--   0        0        0     6665 2023-07-11 10:58:27.205279 mdata-0.1.2/src/mdata/visualization/__pycache__/plotting.cpython-310.pyc
+-rw-r--r--   0        0        0    12465 2023-07-25 14:46:05.342723 mdata-0.1.2/src/mdata/visualization/__pycache__/plotting.cpython-311.pyc
+-rw-r--r--   0        0        0     1102 2023-07-31 08:42:10.807546 mdata-0.1.2/src/mdata/visualization/matplot.py
+-rw-r--r--   0        0        0     7738 2023-07-31 08:42:10.807641 mdata-0.1.2/src/mdata/visualization/plotting.py
+-rw-r--r--   0        0        0      255 2023-07-31 08:42:10.808661 mdata-0.1.2/src/mdata/visualization/textual.py
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 mdata-0.1.2/PKG-INFO
```

### Comparing `mdata-0.1.1/pyproject.toml` & `mdata-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 [tool.poetry]
 name = "mdata"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Leah Tacke genannt Unterberg <leah.tgu@pads.rwth-aachen.de>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["data format", "machine data"]
 exclude = ["files/", "test/"]
 
 [tool.poetry.dependencies]
-pandas = {version = "^1.5"} # after v2.0, extras = ["all"]
-python = "^3.9"
-jupyter = "^1.0"
-matplotlib = "^3.7.1"
+pandas = { version = "^1.5" } # after v2.0, extras = ["all"]
+python = "^3.10"
+immutabledict = "*"
+matplotlib = "*"
 seaborn = "*"
 plotly = "^5.15"
 tsdownsample = "^0.1.2"
-#pm4py = "^2.7.4"
-tables = "^3.8.0"
-numba = "*"
+tables = "*"
+numba = "^0.57"
 numexpr = "*"
 bottleneck = "*"
+llvmlite = "^0.40"
+
+[tool.poetry.group.dev.dependencies]
+pm4py = "^2.7.5"
+jupyter = "^1.0"
 
 [[tool.poetry.source]]
 name = "testpypi"
 url = "https://test.pypi.org/"
-default = false
-secondary = true
+priority = "explicit"
+
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mdata-0.1.1/src/mdata/analysis/__pycache__/frequency.cpython-310.pyc` & `mdata-0.1.2/src/mdata/analysis/__pycache__/frequency.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mdata-0.1.1/src/mdata/analysis/frequency.py` & `mdata-0.1.2/src/mdata/analysis/frequency.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 
 from mdata.core import machine_data_def as mdd
 
 
-def estimate_measurement_frequencies(md: mdd.MachineData) -> dict[mdd.MeasurementTypeKey, float]:
+def estimate_measurement_frequencies(md: mdd.MachineData) -> dict[mdd.MeasurementSpecLabel, float]:
     res = {}
     for m, tsc in md.measurement_series.items():
         diffs = tsc.df[mdd.MDConcepts.Time].diff()
         med = diffs.median()
         values = diffs.sort_values()
         n = len(values)
         inner_values = values.iloc[int(0.05 * n):int(0.95 * n)]
```

### Comparing `mdata-0.1.1/src/mdata/conversions/ocel/ocel_export.py` & `mdata-0.1.2/src/mdata/conversions/ocel/ocel_export.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 
 def create_ocel(md: mdd.MachineData):
     raise NotImplemented
     pd.DataFrame()
     os = md.index_frame[mdd.MDConcepts.Object].unique()
     for mt, tsc in md.measurement_series.items():
         i = 0
-        m_obj = pd.DataFrame(tsc.df, columns=list(tsc.timeseries_type.features))
-        m_obj = m_obj.assign(**{constants.DEFAULT_OBJECT_TYPE: tsc.timeseries_type.label, constants.DEFAULT_OBJECT_ID: i})
+        m_obj = pd.DataFrame(tsc.df, columns=list(tsc.timeseries_spec.features))
+        m_obj = m_obj.assign(**{constants.DEFAULT_OBJECT_TYPE: tsc.timeseries_spec.label, constants.DEFAULT_OBJECT_ID: i})
     for et, tsc in md.event_series.items():
-        tsc.timeseries_type.features
+        tsc.timeseries_spec.features
 
     ...
```

### Comparing `mdata-0.1.1/src/mdata/core/__pycache__/df_utils.cpython-310.pyc` & `mdata-0.1.2/src/mdata/core/__pycache__/df_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mdata-0.1.1/src/mdata/core/__pycache__/factory.cpython-310.pyc` & `mdata-0.1.2/src/mdata/core/__pycache__/factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 07:52:57 2023 UTC, .py size: 2555 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 59da 8264 fb09 0000  o.......Y..d....
+00000000: 6f0d 0d0a 0000 0000 369c 9564 fb09 0000  o.......6..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0173 ca00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
@@ -21,21 +21,21 @@
 00000140: 79da 146f 6e6c 795f 6665 6174 7572 655f  y..only_feature_
 00000150: 636f 6c75 6d6e 73da 1b54 696d 6573 6572  columns..Timeser
 00000160: 6965 7343 6f6c 6c65 6374 696f 6e46 6163  iesCollectionFac
 00000170: 746f 7279 da19 4576 656e 7454 696d 6573  tory..EventTimes
 00000180: 6572 6965 7343 6f6c 6c65 6374 696f 6eda  eriesCollection.
 00000190: 0b4d 6163 6869 6e65 4461 7461 da1f 4d65  .MachineData..Me
 000001a0: 6173 7572 656d 656e 7454 696d 6573 6572  asurementTimeser
-000001b0: 6965 7343 6f6c 6c65 6374 696f 6eda 104d  iesCollection..M
-000001c0: 6163 6869 6e65 4461 7461 5479 7065 73da  achineDataTypes.
+000001b0: 6965 7343 6f6c 6c65 6374 696f 6eda 104f  iesCollection..O
+000001c0: 6273 6572 7661 7469 6f6e 5479 7065 73da  bservationTypes.
 000001d0: 1262 7569 6c64 5f73 6861 7265 645f 696e  .build_shared_in
 000001e0: 6465 7829 03da 1c63 7265 6174 655f 6d61  dex)...create_ma
 000001f0: 6368 696e 655f 6461 7461 5f66 726f 6d5f  chine_data_from_
-00000200: 7261 77da 0d52 6177 4865 6164 6572 5479  raw..RawHeaderTy
-00000210: 7065 da0b 5261 7744 6174 6154 7970 65da  pe..RawDataType.
+00000200: 7261 77da 0d52 6177 4865 6164 6572 5370  raw..RawHeaderSp
+00000210: 6563 da0b 5261 7744 6174 6154 7970 65da  ec..RawDataType.
 00000220: 0264 66fa 0c70 642e 4461 7461 4672 616d  .df..pd.DataFram
 00000230: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
 00000240: 0000 0400 0000 4b00 0001 f316 0000 0074  ......K........t
 00000250: 007c 0066 0164 0174 016a 0269 017c 01a4  .|.f.d.t.j.i.|..
 00000260: 018e 0153 00a9 024e da04 7479 7065 2903  ...S...N..type).
 00000270: da0a 7473 5f66 726f 6d5f 6466 720b 0000  ..ts_from_dfr...
 00000280: 00da 0145 a902 7210 0000 00da 066b 7761  ...E..r......kwa
@@ -80,15 +80,15 @@
 000004f0: 6e64 5f64 6617 0000 0073 1200 0000 0a01  nd_df....s......
 00000500: 0a01 0c01 0e01 0405 0efd 1401 0401 0401  ................
 00000510: 7a25 7473 5f66 726f 6d5f 6466 2e3c 6c6f  z%ts_from_df.<lo
 00000520: 6361 6c73 3e2e 6d61 7463 685f 7370 6563  cals>.match_spec
 00000530: 5f61 6e64 5f64 6672 0100 0000 2901 da08  _and_dfr....)...
 00000540: 6466 5f75 7469 6c73 e901 0000 00e9 0200  df_utils........
 00000550: 0000 e903 0000 0029 1072 0400 0000 da04  .......).r......
-00000560: 5469 6d65 5a0a 6d64 6174 612e 636f 7265  TimeZ.mdata.core
+00000560: 5469 6d65 da0a 6d64 6174 612e 636f 7265  Time..mdata.core
 00000570: 7226 0000 0072 2100 0000 da1b 6372 6561  r&...r!.....crea
 00000580: 7465 5f61 7274 6966 6963 6961 6c5f 6461  te_artificial_da
 00000590: 7465 7261 6e67 65da 064f 626a 6563 74da  terange..Object.
 000005a0: 0454 7970 65da 054c 6162 656c 7205 0000  .Type..Labelr...
 000005b0: 00da 0866 6f72 5f6e 616d 6572 0600 0000  ...for_namer....
 000005c0: 7220 0000 00da 0574 7570 6c65 7207 0000  r .....tupler...
 000005d0: 00da 0866 6f72 5f74 7970 6529 0b72 1000  ...for_type).r..
@@ -110,49 +110,49 @@
 000006d0: 5d24 7d05 6401 7c05 7600 730f 4a00 8201  ]$}.d.|.v.s.J...
 000006e0: 7400 6403 6900 7c05 a401 8e01 7d06 7401  t.d.i.|.....}.t.
 000006f0: 7c06 7402 8302 7221 7c03 a003 7c06 a101  |.t...r!|...|...
 00000700: 0100 7107 7401 7c06 7404 8302 722b 7c04  ..q.t.|.t...r+|.
 00000710: a003 7c06 a101 0100 7107 7405 7406 a007  ..|.....q.t.t...
 00000720: 7c03 7c04 a102 6601 6402 7c00 6901 7c02  |.|...f.d.|.i.|.
 00000730: a401 8e01 7d07 7408 7c03 7c04 7c07 8303  ....}.t.|.|.|...
-00000740: 5300 2904 4e72 1000 0000 7236 0000 0072  S.).Nr....r6...r
+00000740: 5300 2904 4e72 1000 0000 7237 0000 0072  S.).Nr....r7...r
 00000750: 1900 0000 2909 7215 0000 00da 0a69 7369  ....).r......isi
 00000760: 6e73 7461 6e63 6572 0800 0000 da06 6170  nstancer......ap
 00000770: 7065 6e64 720a 0000 0072 0c00 0000 da09  pendr....r......
 00000780: 6974 6572 746f 6f6c 73da 0563 6861 696e  itertools..chain
-00000790: 7209 0000 0029 0872 3600 0000 7237 0000  r....).r6...r7..
+00000790: 7209 0000 0029 0872 3700 0000 7238 0000  r....).r7...r8..
 000007a0: 0072 1800 0000 da03 6574 73da 036d 7473  .r......ets..mts
 000007b0: da02 7364 da03 7473 63da 0b69 6e64 6578  ..sd..tsc..index
 000007c0: 5f66 7261 6d65 7219 0000 0072 1900 0000  _framer....r....
 000007d0: 721a 0000 00da 166d 6163 6869 6e65 5f64  r......machine_d
 000007e0: 6174 615f 6672 6f6d 5f73 7065 6336 0000  ata_from_spec6..
 000007f0: 0073 1600 0000 0a01 0801 0c01 0e01 0a01  .s..............
-00000800: 0c01 0a01 0a01 0280 1c02 0c01 7241 0000  ............rA..
+00000800: 0c01 0a01 0a01 0280 1c02 0c01 7242 0000  ............rB..
 00000810: 0072 0f00 0000 da06 6865 6164 6572 720e  .r......headerr.
 00000820: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
 00000830: 0200 0000 0300 0000 4300 0001 730a 0000  ........C...s...
 00000840: 0074 007c 007c 0183 0253 0029 014e 2901  .t.|.|...S.).N).
-00000850: 720d 0000 0029 0272 1000 0000 7242 0000  r....).r....rB..
+00000850: 720d 0000 0029 0272 1000 0000 7243 0000  r....).r....rC..
 00000860: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
 00000870: da14 6d61 6368 696e 655f 6461 7461 5f66  ..machine_data_f
 00000880: 726f 6d5f 6466 4400 0000 7302 0000 000a  rom_dfD...s.....
-00000890: 0172 4300 0000 2902 7210 0000 0072 1100  .rC...).r....r..
-000008a0: 0000 2902 7237 0000 0072 3400 0000 2904  ..).r7...r4...).
-000008b0: 7210 0000 0072 0f00 0000 7242 0000 0072  r....r....rB...r
+00000890: 0172 4400 0000 2902 7210 0000 0072 1100  .rD...).r....r..
+000008a0: 0000 2902 7238 0000 0072 3500 0000 2904  ..).r8...r5...).
+000008b0: 7210 0000 0072 0f00 0000 7243 0000 0072  r....r....rC...r
 000008c0: 0e00 0000 2920 da0a 5f5f 6675 7475 7265  ....) ..__future
-000008d0: 5f5f 7202 0000 0072 3a00 0000 da06 7479  __r....r:.....ty
+000008d0: 5f5f 7202 0000 0072 3b00 0000 da06 7479  __r....r;.....ty
 000008e0: 7069 6e67 7203 0000 00da 0670 616e 6461  pingr......panda
 000008f0: 73da 0270 645a 1b6d 6461 7461 2e63 6f72  s..pdZ.mdata.cor
 00000900: 652e 6d61 6368 696e 655f 6461 7461 5f64  e.machine_data_d
 00000910: 6566 7204 0000 0072 0500 0000 7206 0000  efr....r....r...
 00000920: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00000930: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000930: 720a 0000 0072 0b00 0000 720c 0000 005a  r....r....r....Z
 00000940: 0e6d 6461 7461 2e63 6f72 652e 7261 7772  .mdata.core.rawr
 00000950: 0d00 0000 720e 0000 0072 0f00 0000 721b  ....r....r....r.
 00000960: 0000 0072 1e00 0000 7215 0000 00da 0944  ...r....r......D
-00000970: 6174 6146 7261 6d65 722c 0000 00da 0373  ataFramer,.....s
-00000980: 7472 722a 0000 0072 2e00 0000 7234 0000  trr*...r....r4..
-00000990: 0072 4100 0000 7243 0000 0072 1900 0000  .rA...rC...r....
+00000970: 6174 6146 7261 6d65 722d 0000 00da 0373  ataFramer-.....s
+00000980: 7472 722a 0000 0072 2f00 0000 7235 0000  trr*...r/...r5..
+00000990: 0072 4200 0000 7244 0000 0072 1900 0000  .rB...rD...r....
 000009a0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
 000009b0: 083c 6d6f 6475 6c65 3e01 0000 0073 1e00  .<module>....s..
 000009c0: 0000 0c00 0802 0c01 0802 2c02 1403 0a03  ..........,.....
 000009d0: 0a04 0a04 041b 1a01 0201 06fe 1005 0e0e  ................
```

### Comparing `mdata-0.1.1/src/mdata/core/__pycache__/raw.cpython-310.pyc` & `mdata-0.1.2/src/mdata/file_formats/csv/__pycache__/checking.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 07:52:57 2023 UTC, .py size: 5913 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,285 +1,276 @@
-00000000: 6f0d 0d0a 0000 0000 59da 8264 1917 0000  o.......Y..d....
+00000000: 6f0d 0d0a 0000 0000 b14c 9464 6c12 0000  o........L.dl...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0173 f400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a03 6400 6402 6c04 5a05 6403 6404 6c06  Z.d.d.l.Z.d.d.l.
-00000050: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
-00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
-00000080: 0100 6509 6a12 6406 6509 6a13 6407 6509  ..e.j.d.e.j.d.e.
-00000090: 6a14 6408 6509 6a15 6409 6904 5a16 6517  j.d.e.j.d.i.Z.e.
-000000a0: 6518 6516 6a19 6509 6a1a 8302 8301 5a1b  e.e.j.e.j.....Z.
-000000b0: 6511 6a1c 640a 6511 6a1d 640b 6902 5a1e  e.j.d.e.j.d.i.Z.
-000000c0: 651f 6518 651e 6a19 6511 6a20 8302 8301  e.e.e.j.e.j ....
-000000d0: 5a21 640c 640d 8400 5a22 6523 650a 650b  Z!d.d...Z"e#e.e.
-000000e0: 6602 1900 5a24 6505 6a25 5a26 6421 6412  f...Z$e.j%Z&d!d.
-000000f0: 6413 8404 5a27 6422 6415 6416 8404 5a28  d...Z'd"d.d...Z(
-00000100: 6422 6417 6418 8404 5a29 6423 641b 641c  d"d.d...Z)d#d.d.
-00000110: 8404 5a2a 6424 641f 6420 8404 5a2b 6402  ..Z*d$d.d ..Z+d.
-00000120: 5300 2925 e900 0000 0029 01da 0b61 6e6e  S.)%.....)...ann
-00000130: 6f74 6174 696f 6e73 4ee9 0100 0000 2901  otationsN.....).
-00000140: da13 6465 7269 7665 5f63 6174 6567 6f72  ..derive_categor
-00000150: 6963 616c 7329 09da 0a4d 4443 6f6e 6365  icals)...MDConce
-00000160: 7074 73da 1154 696d 6573 6572 6965 7354  pts..TimeseriesT
-00000170: 7970 654b 6579 da17 5469 6d65 7365 7269  ypeKey..Timeseri
-00000180: 6573 4665 6174 7572 654c 6162 656c 73da  esFeatureLabels.
-00000190: 0648 6561 6465 72da 1945 7665 6e74 5469  .Header..EventTi
-000001a0: 6d65 7365 7269 6573 436f 6c6c 6563 7469  meseriesCollecti
-000001b0: 6f6e da1f 4d65 6173 7572 656d 656e 7454  on..MeasurementT
-000001c0: 696d 6573 6572 6965 7343 6f6c 6c65 6374  imeseriesCollect
-000001d0: 696f 6eda 0b4d 6163 6869 6e65 4461 7461  ion..MachineData
-000001e0: da1b 5469 6d65 7365 7269 6573 436f 6c6c  ..TimeseriesColl
-000001f0: 6563 7469 6f6e 4661 6374 6f72 79da 104d  ectionFactory..M
-00000200: 6163 6869 6e65 4461 7461 5479 7065 73da  achineDataTypes.
-00000210: 0474 696d 65da 066f 626a 6563 74da 0474  .time..object..t
-00000220: 7970 65da 056c 6162 656c da01 45da 014d  ype..label..E..M
-00000230: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000240: 0005 0000 0043 0000 0173 1800 0000 6401  .....C...s....d.
-00000250: 6402 8400 7400 6403 7c00 6403 1700 8302  d...t.d.|.d.....
-00000260: 4400 8301 5300 2904 4e63 0100 0000 0000  D...S.).Nc......
-00000270: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000280: 0001 7316 0000 0067 007c 005d 077d 0164  ..s....g.|.].}.d
-00000290: 007c 019b 009d 0291 0271 0253 0029 01da  .|.......q.S.)..
-000002a0: 0266 5fa9 0029 02da 022e 30da 0169 7215  .f_..)....0..ir.
-000002b0: 0000 0072 1500 0000 fa39 433a 5c55 7365  ...r.....9C:\Use
-000002c0: 7273 5c4c 6561 685c 5079 6368 6172 6d50  rs\Leah\PycharmP
-000002d0: 726f 6a65 6374 735c 6d64 6174 615c 7372  rojects\mdata\sr
-000002e0: 635c 6d64 6174 615c 636f 7265 5c72 6177  c\mdata\core\raw
-000002f0: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e1c  .py..<listcomp>.
-00000300: 0000 00f3 0200 0000 1600 7a2c 6765 6e5f  ..........z,gen_
-00000310: 6665 6174 7572 655f 636f 6c75 6d6e 5f6e  feature_column_n
-00000320: 616d 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ames.<locals>.<l
-00000330: 6973 7463 6f6d 703e 7203 0000 0029 01da  istcomp>r....)..
-00000340: 0572 616e 6765 2901 da01 6e72 1500 0000  .range)...nr....
-00000350: 7215 0000 0072 1800 0000 da18 6765 6e5f  r....r......gen_
-00000360: 6665 6174 7572 655f 636f 6c75 6d6e 5f6e  feature_column_n
-00000370: 616d 6573 1b00 0000 7302 0000 0018 0172  ames....s......r
-00000380: 1d00 0000 da02 6d64 720b 0000 00da 0672  ......mdr......r
-00000390: 6574 7572 6eda 0d52 6177 4865 6164 6572  eturn..RawHeader
-000003a0: 5479 7065 6301 0000 0000 0000 0000 0000  Typec...........
-000003b0: 0004 0000 0005 0000 0043 0000 0173 2e00  .........C...s..
-000003c0: 0000 6900 7d01 7c00 a000 a100 4400 5d0e  ..i.}.|.....D.].
-000003d0: 7d02 7c02 6a01 7d03 7402 7c03 6a03 8301  }.|.j.}.t.|.j...
-000003e0: 7c01 7c03 a004 a100 3c00 7106 7c01 5300  |.|.....<.q.|.S.
-000003f0: a901 4e29 05da 1369 7465 725f 616c 6c5f  ..N)...iter_all_
-00000400: 7469 6d65 7365 7269 6573 da0f 7469 6d65  timeseries..time
-00000410: 7365 7269 6573 5f74 7970 65da 0574 7570  series_type..tup
-00000420: 6c65 da08 6665 6174 7572 6573 da05 6173  le..features..as
-00000430: 6b65 7929 0472 1e00 0000 da06 6865 6164  key).r......head
-00000440: 6572 da10 7479 7065 645f 7469 6d65 7365  er..typed_timese
-00000450: 7269 6573 da02 7474 7215 0000 0072 1500  ries..ttr....r..
-00000460: 0000 7218 0000 00da 1563 6f6e 7665 7274  ..r......convert
-00000470: 5f74 6f5f 7261 775f 6865 6164 6572 2300  _to_raw_header#.
-00000480: 0000 730a 0000 0004 010c 0106 0114 0104  ..s.............
-00000490: 0172 2a00 0000 da0b 5261 7744 6174 6154  .r*.....RawDataT
-000004a0: 7970 6563 0100 0000 0000 0000 0000 0000  ypec............
-000004b0: 0600 0000 0500 0000 4300 0001 7394 0000  ........C...s...
-000004c0: 0074 0074 0164 0164 0284 007c 00a0 02a1  .t.t.d.d...|....
-000004d0: 0083 0283 017d 0174 036a 047c 006a 0564  .....}.t.j.|.j.d
-000004e0: 0364 048d 027d 0274 066a 077c 0274 087c  .d...}.t.j.|.t.|
-000004f0: 0183 013c 007c 00a0 02a1 0044 005d 217d  ...<.|.....D.]!}
-00000500: 037c 036a 097d 0474 0874 0a7c 036a 0b6a  .|.j.}.t.t.|.j.j
-00000510: 0c83 0183 017d 057c 046a 0d64 0064 0085  .....}.|.j.d.d..
-00000520: 0274 0e7c 036a 0b6a 0c83 0166 0219 006a  .t.|.j.j...f...j
-00000530: 0f7c 026a 0d7c 046a 107c 0566 023c 0071  .|.j.|.j.|.f.<.q
-00000540: 1e74 116a 1274 087c 0183 0117 007c 025f  .t.j.t.|.....|._
-00000550: 137c 0253 0029 054e 6301 0000 0000 0000  .|.S.).Nc.......
-00000560: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00000570: 01f3 0a00 0000 7400 7c00 6a01 8301 5300  ......t.|.j...S.
-00000580: 7221 0000 00a9 02da 036c 656e 7223 0000  r!.......lenr#..
-00000590: 00a9 015a 0d6d 645f 7469 6d65 7365 7269  ...Z.md_timeseri
-000005a0: 6573 7215 0000 0072 1500 0000 7218 0000  esr....r....r...
-000005b0: 00da 083c 6c61 6d62 6461 3e2c 0000 00f3  ...<lambda>,....
-000005c0: 0200 0000 0a00 7a25 636f 6e76 6572 745f  ......z%convert_
-000005d0: 746f 5f72 6177 5f64 6174 612e 3c6c 6f63  to_raw_data.<loc
-000005e0: 616c 733e 2e3c 6c61 6d62 6461 3e54 a901  als>.<lambda>T..
-000005f0: da04 636f 7079 2914 da03 6d61 78da 036d  ..copy)...max..m
-00000600: 6170 7222 0000 00da 0270 64da 0944 6174  apr".....pd..Dat
-00000610: 6146 7261 6d65 da0b 696e 6465 785f 6672  aFrame..index_fr
-00000620: 616d 65da 026e 70da 034e 414e 721d 0000  ame..np..NANr...
-00000630: 00da 0264 6672 2e00 0000 7223 0000 0072  ...dfr....r#...r
-00000640: 2500 0000 da03 6c6f 63da 046c 6973 74da  %.....loc..list.
-00000650: 0676 616c 7565 73da 0569 6e64 6578 7205  .values..indexr.
-00000660: 0000 00da 0c62 6173 655f 636f 6c75 6d6e  .....base_column
-00000670: 73da 0763 6f6c 756d 6e73 2906 721e 0000  s..columns).r...
-00000680: 00da 0c6d 6178 5f66 6561 7475 7265 73da  ...max_features.
-00000690: 0372 6573 da03 7473 6372 3b00 0000 da02  .res..tscr;.....
-000006a0: 6373 7215 0000 0072 1500 0000 7218 0000  csr....r....r...
-000006b0: 00da 1363 6f6e 7665 7274 5f74 6f5f 7261  ...convert_to_ra
-000006c0: 775f 6461 7461 2b00 0000 7312 0000 0016  w_data+...s.....
-000006d0: 0110 080e 010c 0306 0110 012a 0110 0204  ...........*....
-000006e0: 0472 4600 0000 6301 0000 0000 0000 0000  .rF...c.........
-000006f0: 0000 0006 0000 0008 0000 0003 0000 0173  ...............s
-00000700: b000 0000 7400 7401 6401 6402 8400 7c00  ....t.t.d.d...|.
-00000710: a002 a100 8302 8301 7d01 6700 7d02 7c00  ........}.g.}.|.
-00000720: a002 a100 4400 5d2f 7d03 7c03 6a03 7d04  ....D.]/}.|.j.}.
-00000730: 7c03 6a04 8900 8800 6a05 6403 6404 8d01  |.j.....j.d.d...
-00000740: 4400 5d20 8901 7c02 a006 7407 8801 7408  D.] ..|...t...t.
-00000750: 6a09 8302 7407 8801 7408 6a0a 8302 7c04  j...t...t.j...|.
-00000760: 6a0b 7c04 6a0c 6704 8700 8701 6602 6405  j.|.j.g.....f.d.
-00000770: 6406 8408 7c04 6a0d 4400 8301 1700 a101  d...|.j.D.......
-00000780: 0100 711f 7111 740e 6a0f 7c02 7410 7411  ..q.q.t.j.|.t.t.
-00000790: 7c01 8301 1700 6407 8d02 7d05 7c05 6a12  |.....d...}.|.j.
-000007a0: 7413 7408 6a09 1900 6403 6408 8d02 0100  t.t.j...d.d.....
-000007b0: 7c05 5300 2909 4e63 0100 0000 0000 0000  |.S.).Nc........
-000007c0: 0000 0000 0100 0000 0200 0000 5300 0001  ............S...
-000007d0: 722c 0000 0072 2100 0000 722d 0000 0072  r,...r!...r-...r
-000007e0: 2f00 0000 7215 0000 0072 1500 0000 7218  /...r....r....r.
-000007f0: 0000 0072 3000 0000 4500 0000 7231 0000  ...r0...E...r1..
-00000800: 007a 2c63 6f6e 7665 7274 5f74 6f5f 7261  .z,convert_to_ra
-00000810: 775f 6461 7461 5f6c 6567 6163 792e 3c6c  w_data_legacy.<l
-00000820: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e54  ocals>.<lambda>T
-00000830: 2901 723f 0000 0063 0100 0000 0000 0000  ).r?...c........
-00000840: 0000 0000 0200 0000 0500 0000 1300 0001  ................
-00000850: 7320 0000 0067 007c 005d 0c7d 017c 0188  s ...g.|.].}.|..
-00000860: 006a 0076 0072 0274 0188 017c 0183 0291  .j.v.r.t...|....
-00000870: 0271 0253 0072 1500 0000 2902 7241 0000  .q.S.r....).rA..
-00000880: 00da 0767 6574 6174 7472 2902 7216 0000  ...getattr).r...
-00000890: 00da 0166 a902 723b 0000 00da 0374 7570  ...f..r;.....tup
-000008a0: 7215 0000 0072 1800 0000 7219 0000 004d  r....r....r....M
-000008b0: 0000 0073 0800 0000 0600 0201 0802 10fd  ...s............
-000008c0: 7a2e 636f 6e76 6572 745f 746f 5f72 6177  z.convert_to_raw
-000008d0: 5f64 6174 615f 6c65 6761 6379 2e3c 6c6f  _data_legacy.<lo
-000008e0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000008f0: 2901 7241 0000 0029 01da 0769 6e70 6c61  ).rA...)...inpla
-00000900: 6365 2914 7234 0000 0072 3500 0000 7222  ce).r4...r5...r"
-00000910: 0000 0072 2300 0000 723b 0000 00da 0a69  ...r#...r;.....i
-00000920: 7465 7274 7570 6c65 73da 0661 7070 656e  tertuples..appen
-00000930: 6472 4700 0000 7205 0000 00da 0454 696d  drG...r......Tim
-00000940: 65da 064f 626a 6563 7472 1000 0000 7211  e..Objectr....r.
-00000950: 0000 0072 2500 0000 7236 0000 0072 3700  ...r%...r6...r7.
-00000960: 0000 da1d 6261 7365 5f72 6177 5f6d 6163  ....base_raw_mac
-00000970: 6869 6e65 5f64 6174 615f 636f 6c75 6d6e  hine_data_column
-00000980: 7372 1d00 0000 da0b 736f 7274 5f76 616c  sr......sort_val
-00000990: 7565 73da 1043 4f4c 554d 4e5f 4e41 4d45  ues..COLUMN_NAME
-000009a0: 5f44 4943 5429 0672 1e00 0000 7242 0000  _DICT).r....rB..
-000009b0: 00da 0472 6f77 7372 2800 0000 7229 0000  ...rowsr(...r)..
-000009c0: 0072 4300 0000 7215 0000 0072 4900 0000  .rC...r....rI...
-000009d0: 7218 0000 00da 1a63 6f6e 7665 7274 5f74  r......convert_t
-000009e0: 6f5f 7261 775f 6461 7461 5f6c 6567 6163  o_raw_data_legac
-000009f0: 7944 0000 0073 2600 0000 1601 0401 0c01  yD...s&.........
-00000a00: 0601 0601 1001 0401 1801 0401 02ff 0c01  ................
-00000a10: 0402 04fe 02ff 06ff 02ff 1607 1401 0401  ................
-00000a20: 7254 0000 00da 1366 6561 7475 7265 5f64  rT.....feature_d
-00000a30: 6566 696e 6974 696f 6e73 7208 0000 0063  efinitionsr....c
-00000a40: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000a50: 0300 0000 4300 0001 730a 0000 0074 00a0  ....C...s....t..
-00000a60: 017c 00a1 0153 0072 2100 0000 2902 7208  .|...S.r!...).r.
-00000a70: 0000 00da 0866 726f 6d5f 7261 7729 0172  .....from_raw).r
-00000a80: 5500 0000 7215 0000 0072 1500 0000 7218  U...r....r....r.
-00000a90: 0000 00da 1663 7265 6174 655f 6865 6164  .....create_head
-00000aa0: 6572 5f66 726f 6d5f 7261 7756 0000 0073  er_from_rawV...s
-00000ab0: 0200 0000 0a01 7257 0000 00da 0872 6177  ......rW.....raw
-00000ac0: 5f64 6174 61da 0a72 6177 5f68 6561 6465  _data..raw_heade
-00000ad0: 7263 0200 0000 0000 0000 0000 0000 1400  rc..............
-00000ae0: 0000 0700 0000 4300 0001 737e 0100 0074  ......C...s~...t
-00000af0: 007c 0183 017d 0267 0067 0002 027d 037d  .|...}.g.g...}.}
-00000b00: 0474 017c 0074 0274 036a 0474 056a 0674  .t.|.t.t.j.t.j.t
-00000b10: 056a 0774 056a 0867 0383 0283 027d 0564  .j.t.j.g.....}.d
-00000b20: 0164 0284 0074 03a0 09a1 0044 0083 017d  .d...t.....D...}
-00000b30: 0674 0a6a 0b7c 0074 0c64 0364 048d 037d  .t.j.|.t.d.d...}
-00000b40: 077c 076a 0d7c 0664 0364 058d 0201 007c  .|.j.|.d.d.....|
-00000b50: 076a 0e7c 0564 0664 078d 027d 077c 07a0  .j.|.d.d...}.|..
-00000b60: 0f74 0374 056a 0819 0074 0374 056a 0719  .t.t.j...t.t.j..
-00000b70: 0067 02a1 016a 10a0 09a1 0044 005d 5f5c  .g...j.....D.]_\
-00000b80: 027d 087d 097c 085c 027d 0a7d 0b7c 026a  .}.}.|.\.}.}.|.j
-00000b90: 117c 0a7c 0b66 0219 007d 0c7c 0c6a 127d  .|.|.f...}.|.j.}
-00000ba0: 0d74 137c 0d83 017d 0e74 147c 0e83 017d  .t.|...}.t.|...}
-00000bb0: 0f74 0a6a 157c 076a 167c 0974 056a 1766  .t.j.|.j.|.t.j.f
-00000bc0: 0219 007c 006a 167c 097c 0f66 0219 0067  ...|.j.|.|.f...g
-00000bd0: 0264 0364 0864 098d 03a0 187c 09a1 017d  .d.d.d.....|...}
-00000be0: 1064 0a64 0284 0074 197c 0f7c 0d83 0244  .d.d...t.|.|...D
-00000bf0: 0083 017d 117c 106a 0d7c 1164 0364 058d  ...}.|.j.|.d.d..
-00000c00: 0201 0074 1aa0 1b7c 0ca1 017c 1083 017d  ...t...|...|...}
-00000c10: 1274 1c7c 1274 1d83 0272 9c7c 03a0 1e7c  .t.|.t...r.|...|
-00000c20: 12a1 0101 0071 4774 1c7c 1274 1f83 0272  .....qGt.|.t...r
-00000c30: a67c 04a0 1e7c 12a1 0101 0071 4774 2074  .|...|.....qGt t
-00000c40: 217c 076a 2283 01a0 2374 056a 17a1 0183  !|.j"...#t.j....
-00000c50: 017d 137c 076a 247c 1364 0364 058d 0201  .}.|.j$|.d.d....
-00000c60: 0074 257c 037c 047c 0783 0353 0029 0b4e  .t%|.|.|...S.).N
-00000c70: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000c80: 0004 0000 0053 0000 0173 1600 0000 6900  .....S...s....i.
-00000c90: 7c00 5d07 5c02 7d01 7d02 7c02 7c01 9302  |.].\.}.}.|.|...
-00000ca0: 7102 5300 7215 0000 0072 1500 0000 2903  q.S.r....r....).
-00000cb0: 7216 0000 00da 036e 6577 da03 6f6c 6472  r......new..oldr
-00000cc0: 1500 0000 7215 0000 0072 1800 0000 da0a  ....r....r......
-00000cd0: 3c64 6963 7463 6f6d 703e 6200 0000 721a  <dictcomp>b...r.
-00000ce0: 0000 007a 3063 7265 6174 655f 6d61 6368  ...z0create_mach
-00000cf0: 696e 655f 6461 7461 5f66 726f 6d5f 7261  ine_data_from_ra
-00000d00: 772e 3c6c 6f63 616c 733e 2e3c 6469 6374  w.<locals>.<dict
-00000d10: 636f 6d70 3e54 2902 7241 0000 0072 3300  comp>T).rA...r3.
-00000d20: 0000 2902 7241 0000 0072 4b00 0000 4672  ..).rA...rK...Fr
-00000d30: 3200 0000 7203 0000 0029 0272 3300 0000  2...r....).r3...
-00000d40: da04 6178 6973 6301 0000 0000 0000 0000  ..axisc.........
-00000d50: 0000 0003 0000 0004 0000 0053 0000 0173  ...........S...s
-00000d60: 1600 0000 6900 7c00 5d07 5c02 7d01 7d02  ....i.|.].\.}.}.
-00000d70: 7c01 7c02 9302 7102 5300 7215 0000 0072  |.|...q.S.r....r
-00000d80: 1500 0000 2903 7216 0000 0072 5b00 0000  ....).r....r[...
-00000d90: 725a 0000 0072 1500 0000 7215 0000 0072  rZ...r....r....r
-00000da0: 1800 0000 725c 0000 0075 0000 0072 1a00  ....r\...u...r..
-00000db0: 0000 2926 7257 0000 0072 0400 0000 7235  ..)&rW...r....r5
-00000dc0: 0000 0072 5200 0000 da03 6765 7472 0500  ...rR.....getr..
-00000dd0: 0000 724f 0000 00da 054c 6162 656c da04  ..rO.....Label..
-00000de0: 5479 7065 da05 6974 656d 7372 3600 0000  Type..itemsr6...
-00000df0: 7237 0000 0072 5000 0000 da06 7265 6e61  r7...rP.....rena
-00000e00: 6d65 da06 6173 7479 7065 da07 6772 6f75  me..astype..grou
-00000e10: 7062 79da 0667 726f 7570 7372 5500 0000  pby..groupsrU...
-00000e20: 7225 0000 0072 2e00 0000 721d 0000 00da  r%...r....r.....
-00000e30: 0663 6f6e 6361 7472 3c00 0000 7240 0000  .concatr<...r@..
-00000e40: 00da 0973 6574 5f69 6e64 6578 da03 7a69  ...set_index..zi
-00000e50: 7072 0c00 0000 da08 666f 725f 7479 7065  pr......for_type
-00000e60: da0a 6973 696e 7374 616e 6365 7209 0000  ..isinstancer...
-00000e70: 0072 4d00 0000 720a 0000 0072 3d00 0000  .rM...r....r=...
-00000e80: da03 7365 7472 4100 0000 da0a 6469 6666  ..setrA.....diff
-00000e90: 6572 656e 6365 da04 6472 6f70 720b 0000  erence..dropr...
-00000ea0: 0029 1472 5800 0000 7259 0000 0072 2700  .).rX...rY...r'.
-00000eb0: 0000 5a04 6d64 6573 5a04 6d64 6d73 da0a  ..Z.mdesZ.mdms..
-00000ec0: 6361 7465 676f 7269 6573 5a12 6261 7365  categoriesZ.base
-00000ed0: 5f63 6f6c 756d 5f6d 6170 7069 6e67 5a07  _colum_mappingZ.
-00000ee0: 6f76 6572 616c 6cda 0567 726f 7570 da03  overall..group..
-00000ef0: 6964 785a 0374 7079 7211 0000 0072 2300  idxZ.tpyr....r#.
-00000f00: 0000 5a15 6163 7475 616c 5f66 6561 7475  ..Z.actual_featu
-00000f10: 7265 5f6c 6162 656c 735a 0d66 6561 7475  re_labelsZ.featu
-00000f20: 7265 5f63 6f75 6e74 5a1a 706c 6163 6568  re_countZ.placeh
-00000f30: 6f6c 6465 725f 6665 6174 7572 655f 6c61  older_feature_la
-00000f40: 6265 6c73 723b 0000 005a 0d72 656e 616d  belsr;...Z.renam
-00000f50: 696e 675f 6469 6374 5a0d 7473 5f63 6f6c  ing_dictZ.ts_col
-00000f60: 6c65 6374 696f 6eda 1070 6c61 6365 686f  lection..placeho
-00000f70: 6c64 6572 5f63 6f6c 7372 1500 0000 7215  lder_colsr....r.
-00000f80: 0000 0072 1800 0000 da1c 6372 6561 7465  ...r......create
-00000f90: 5f6d 6163 6869 6e65 5f64 6174 615f 6672  _machine_data_fr
-00000fa0: 6f6d 5f72 6177 5a00 0000 733e 0000 0008  om_rawZ...s>....
-00000fb0: 010a 0204 0216 0104 ff12 0310 020e 010e  ................
-00000fc0: 0128 0208 010e 0106 0108 0108 0120 0104  .(........... ..
-00000fd0: 0104 ff06 0102 ff14 070e 020e 010a 010c  ................
-00000fe0: 010a 010a 0102 8016 020e 010c 0272 7200  .............rr.
-00000ff0: 0000 2904 721e 0000 0072 0b00 0000 721f  ..).r....r....r.
-00001000: 0000 0072 2000 0000 2904 721e 0000 0072  ...r ...).r....r
-00001010: 0b00 0000 721f 0000 0072 2b00 0000 2904  ....r....r+...).
-00001020: 7255 0000 0072 2000 0000 721f 0000 0072  rU...r ...r....r
-00001030: 0800 0000 2904 7258 0000 0072 2b00 0000  ....).rX...r+...
-00001040: 7259 0000 0072 2000 0000 292c da0a 5f5f  rY...r ...),..__
-00001050: 6675 7475 7265 5f5f 7202 0000 00da 056e  future__r......n
-00001060: 756d 7079 7239 0000 00da 0670 616e 6461  umpyr9.....panda
-00001070: 7372 3600 0000 da08 6466 5f75 7469 6c73  sr6.....df_utils
-00001080: 7204 0000 00da 106d 6163 6869 6e65 5f64  r......machine_d
-00001090: 6174 615f 6465 6672 0500 0000 7206 0000  ata_defr....r...
-000010a0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-000010b0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-000010c0: 0d00 0000 724e 0000 0072 4f00 0000 7260  ....rN...rO...r`
-000010d0: 0000 0072 5f00 0000 7252 0000 0072 3d00  ...r_...rR...r=.
-000010e0: 0000 7235 0000 0072 5e00 0000 7240 0000  ..r5...r^...r@..
-000010f0: 0072 5000 0000 7212 0000 0072 1300 0000  .rP...r....r....
-00001100: 5a17 4d41 4348 494e 455f 4441 5441 5f54  Z.MACHINE_DATA_T
-00001110: 5950 4553 5f44 4943 5472 6b00 0000 da0a  YPES_DICTrk.....
-00001120: 6261 7365 5f74 7970 6573 da16 7261 775f  base_types..raw_
-00001130: 6d61 6368 696e 655f 6461 7461 5f74 7970  machine_data_typ
-00001140: 6573 721d 0000 00da 0464 6963 7472 2000  esr......dictr .
-00001150: 0000 7237 0000 0072 2b00 0000 722a 0000  ..r7...r+...r*..
-00001160: 0072 4600 0000 7254 0000 0072 5700 0000  .rF...rT...rW...
-00001170: 7272 0000 0072 1500 0000 7215 0000 0072  rr...r....r....r
-00001180: 1500 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
-00001190: 6c65 3e01 0000 0073 2e00 0000 0c00 0802  le>....s........
-000011a0: 0801 0c02 2c01 0606 0601 0601 0601 04fb  ....,...........
-000011b0: 1207 0603 0601 04fe 1204 0803 0c04 0601  ................
-000011c0: 0a03 0a08 0a19 0a12 0e04                 ..........
+00000020: 0007 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6401 6c05 5a05 6400 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
+00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
+00000080: 0100 6407 6408 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
+00000090: 6d11 5a11 0100 6409 640a 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
+000000a0: 0100 6409 640b 6c14 5400 640c 640d 8400  ..d.d.l.T.d.d...
+000000b0: 5a15 640e 640f 8400 5a16 6410 650d 6602  Z.d.d...Z.d.e.f.
+000000c0: 6411 6412 8404 5a17 6410 650d 6602 6413  d.d...Z.d.e.f.d.
+000000d0: 6414 8404 5a18 6513 a019 6500 6a1a a01b  d...Z.e...e.j...
+000000e0: 6500 6a1a a01c 651d a101 6415 6416 a103  e.j...e...d.d...
+000000f0: a101 5a1e 6417 6507 6a1f 6602 6418 6419  ..Z.d.e.j.f.d.d.
+00000100: 8404 5a20 641a 641b 8400 5a21 641c 641d  ..Z d.d...Z!d.d.
+00000110: 8400 5a22 6401 5300 291e e900 0000 004e  ..Z"d.S.)......N
+00000120: 2901 da0b 6465 6661 756c 7464 6963 7429  )...defaultdict)
+00000130: 01da 0f4a 534f 4e44 6563 6f64 6545 7272  ...JSONDecodeErr
+00000140: 6f72 2901 da03 7261 7729 03da 0872 6567  or)...raw)...reg
+00000150: 6973 7472 79da 086d 6574 6164 6174 61da  istry..metadata.
+00000160: 0b61 6e6e 6f74 6174 696f 6e73 2901 da0a  .annotations)...
+00000170: 4461 7461 536f 7572 6365 e901 0000 0029  DataSource.....)
+00000180: 03da 0d72 6561 645f 7261 775f 6461 7461  ...read_raw_data
+00000190: da11 7265 6164 5f6d 6163 6869 6e65 5f64  ..read_machine_d
+000001a0: 6174 61da 2972 6561 645f 6d61 6368 696e  ata.)read_machin
+000001b0: 655f 6461 7461 5f66 726f 6d5f 6361 6e6f  e_data_from_cano
+000001c0: 6e69 6361 6c5f 6261 7365 6e61 6d65 e902  nical_basename..
+000001d0: 0000 0029 01da 0869 6f5f 7574 696c 7329  ...)...io_utils)
+000001e0: 01da 012a 6301 0000 0000 0000 0000 0000  ...*c...........
+000001f0: 0001 0000 0008 0000 0043 0000 0073 2800  .........C...s(.
+00000200: 0000 7a09 7400 7c00 6401 6402 8d02 0100  ..z.t.|.d.d.....
+00000210: 5700 6401 5300 0400 7401 7913 0100 0100  W.d.S...t.y.....
+00000220: 0100 5900 6403 5300 7700 a904 4e54 2901  ..Y.d.S.w...NT).
+00000230: da11 7661 6c69 6469 7479 5f63 6865 636b  ..validity_check
+00000240: 696e 6746 2902 720c 0000 00da 1956 616c  ingF).r......Val
+00000250: 6964 6974 7943 6865 636b 696e 6745 7863  idityCheckingExc
+00000260: 6570 7469 6f6e 2901 da09 6261 7365 5f70  eption)...base_p
+00000270: 6174 68a9 0072 1400 0000 fa4a 433a 5c55  ath..r.....JC:\U
+00000280: 7365 7273 5c4c 6561 685c 5079 6368 6172  sers\Leah\Pychar
+00000290: 6d50 726f 6a65 6374 735c 6d64 6174 615c  mProjects\mdata\
+000002a0: 7372 635c 6d64 6174 615c 6669 6c65 5f66  src\mdata\file_f
+000002b0: 6f72 6d61 7473 5c63 7376 5c63 6865 636b  ormats\csv\check
+000002c0: 696e 672e 7079 da1c 6973 5f76 616c 6964  ing.py..is_valid
+000002d0: 5f63 616e 6f6e 6963 616c 5f66 696c 655f  _canonical_file_
+000002e0: 7061 6972 0f00 0000 730c 0000 0002 010e  pair....s.......
+000002f0: 0104 030c fe06 0102 ff72 1600 0000 6302  .........r....c.
+00000300: 0000 0000 0000 0000 0000 0002 0000 0008  ................
+00000310: 0000 0043 0000 0073 2a00 0000 7a0a 7400  ...C...s*...z.t.
+00000320: 7c00 7c01 6401 6402 8d03 0100 5700 6401  |.|.d.d.....W.d.
+00000330: 5300 0400 7401 7914 0100 0100 0100 5900  S...t.y.......Y.
+00000340: 6403 5300 7700 7210 0000 0029 0272 0b00  d.S.w.r....).r..
+00000350: 0000 7212 0000 0029 02da 0b68 6561 6465  ..r....)...heade
+00000360: 725f 7061 7468 da09 6461 7461 5f70 6174  r_path..data_pat
+00000370: 6872 1400 0000 7214 0000 0072 1500 0000  hr....r....r....
+00000380: da12 6973 5f76 616c 6964 5f66 696c 655f  ..is_valid_file_
+00000390: 7061 6972 1700 0000 730c 0000 0002 0110  pair....s.......
+000003a0: 0104 030c fe06 0102 ff72 1900 0000 da04  .........r......
+000003b0: 6669 6c65 6301 0000 0000 0000 0000 0000  filec...........
+000003c0: 0008 0000 000a 0000 0003 0000 0073 1802  .............s..
+000003d0: 0000 7400 7401 8301 7d01 7a07 7402 a003  ..t.t...}.z.t...
+000003e0: 7c00 a101 7d02 5700 6e14 0400 7404 791f  |...}.W.n...t.y.
+000003f0: 0100 7d03 0100 7a08 7405 6401 7406 7c03  ..}...z.t.d.t.|.
+00000400: 8301 1700 8301 8201 6400 7d03 7e03 7701  ........d.}.~.w.
+00000410: 7700 7407 7c02 6402 6403 8d02 4400 5de3  w.t.|.d.d...D.].
+00000420: 5c02 7d04 8900 8800 6404 1900 7d05 6404  \.}.....d...}.d.
+00000430: 6701 7d06 7c05 7408 6a09 7600 7255 8800  g.}.|.t.j.v.rU..
+00000440: 6402 1900 7d07 7c06 a00a 6402 a101 0100  d...}.|...d.....
+00000450: 7c07 7c01 7c05 1900 7600 724d 7405 6405  |.|.|...v.rMt.d.
+00000460: 7c04 9b00 6406 9d03 8301 8201 7c01 7c05  |...d.......|.|.
+00000470: 1900 a00b 7c07 a101 0100 6e9c 7c05 740c  ....|.....n.|.t.
+00000480: 6a0d 6b02 7270 6407 7c01 7c05 1900 7600  j.k.rpd.|.|...v.
+00000490: 7268 7405 6408 7c04 9b00 6406 9d03 8301  rht.d.|...d.....
+000004a0: 8201 7c01 7c05 1900 a00b 6407 a101 0100  ..|.|.....d.....
+000004b0: 6e81 7c05 740e 6a0d 6b02 72bf 7c06 a00f  n.|.t.j.k.r.|...
+000004c0: 6700 6409 a201 a101 0100 8800 640a 1900  g.d.........d...
+000004d0: 7408 6a09 7600 728c 7410 8800 6402 640b  t.j.v.r.t...d.d.
+000004e0: 8502 1900 8301 7d03 6e1d 8800 640a 1900  ......}.n...d...
+000004f0: 7411 6a0d 6b02 72a1 7410 8800 6402 640c  t.j.k.r.t...d.d.
+00000500: 8502 1900 8301 7d03 7c06 a00a 640c a101  ......}.|...d...
+00000510: 0100 6e08 7405 640d 7c04 9b00 6406 9d03  ..n.t.d.|...d...
+00000520: 8301 8201 7c03 7c01 7c05 1900 7600 72b7  ....|.|.|...v.r.
+00000530: 7405 640e 7c04 9b00 6406 9d03 8301 8201  t.d.|...d.......
+00000540: 7c01 7c05 1900 a00b 7c03 a101 0100 6e32  |.|.....|.....n2
+00000550: 7c05 7411 6a0d 6b02 72e9 7c06 a00f 6700  |.t.j.k.r.|...g.
+00000560: 640f a201 a101 0100 8800 6402 1900 8800  d.........d.....
+00000570: 640a 1900 6602 7d07 7c07 7c01 7c05 1900  d...f.}.|.|.|...
+00000580: 7600 72e1 7405 6410 7c04 9b00 6406 9d03  v.r.t.d.|...d...
+00000590: 8301 8201 7c01 7c05 1900 a00b 7c07 a101  ....|.|.....|...
+000005a0: 0100 6e08 7405 6411 7c04 9b00 6406 9d03  ..n.t.d.|...d...
+000005b0: 8301 8201 7412 8700 6601 6412 6413 8408  ....t...f.d.d...
+000005c0: 7c06 4400 8301 8301 9001 7209 7413 8800  |.D.......r.t...
+000005d0: 8301 0100 7405 6414 7c04 9b00 6406 9d03  ....t.d.|...d...
+000005e0: 8301 8201 7126 6407 5300 2915 4e7a 1055  ....q&d.S.).Nz.U
+000005f0: 6e70 6172 7361 626c 6520 6373 763a 0a72  nparsable csv:.r
+00000600: 0900 0000 2901 da05 7374 6172 7472 0100  ....)...startr..
+00000610: 0000 7a31 4475 706c 6963 6174 6520 6f62  ..z1Duplicate ob
+00000620: 7365 7276 6174 696f 6e20 7479 7065 2073  servation type s
+00000630: 7065 6369 6669 6361 7469 6f6e 2069 6e20  pecification in 
+00000640: 6c69 6e65 20da 012e 547a 2844 7570 6c69  line ...Tz(Dupli
+00000650: 6361 7465 2065 7874 656e 7369 6f6e 2064  cate extension d
+00000660: 6563 6c61 7261 7469 6f6e 2069 6e20 6c69  eclaration in li
+00000670: 6e65 2029 0572 0900 0000 720d 0000 00e9  ne ).r....r.....
+00000680: 0300 0000 e904 0000 00e9 0500 0000 720d  ..............r.
+00000690: 0000 0072 1f00 0000 e906 0000 007a 2f49  ...r.........z/I
+000006a0: 6e76 616c 6964 2073 796d 626f 6c20 696e  nvalid symbol in
+000006b0: 206d 6574 6164 6174 6120 6465 636c 6172   metadata declar
+000006c0: 6174 696f 6e20 696e 206c 696e 6520 7a27  ation in line z'
+000006d0: 4475 706c 6963 6174 6520 6d65 7461 6461  Duplicate metada
+000006e0: 7461 2064 6563 6c61 7261 7469 6f6e 2069  ta declaration i
+000006f0: 6e20 6c69 6e65 2029 0372 0900 0000 720d  n line ).r....r.
+00000700: 0000 0072 1d00 0000 7a29 4475 706c 6963  ...r....z)Duplic
+00000710: 6174 6520 616e 6e6f 7461 7469 6f6e 2064  ate annotation d
+00000720: 6563 6c61 7261 7469 6f6e 2069 6e20 6c69  eclaration in li
+00000730: 6e65 207a 3549 6e76 616c 6964 2073 7065  ne z5Invalid spe
+00000740: 6369 6669 6361 7469 6f6e 2073 796d 626f  cification symbo
+00000750: 6c20 696e 2066 6972 7374 2063 6f6c 756d  l in first colum
+00000760: 6e20 696e 206c 696e 6520 6301 0000 0000  n in line c.....
+00000770: 0000 0000 0000 0002 0000 0003 0000 0033  ...............3
+00000780: 0000 0073 1c00 0000 8100 7c00 5d09 7d01  ...s......|.].}.
+00000790: 8800 7c01 1900 6400 6b02 5600 0100 7102  ..|...d.k.V...q.
+000007a0: 6401 5300 2902 da00 4e72 1400 0000 2902  d.S.)...Nr....).
+000007b0: da02 2e30 da01 69a9 01da 0372 6f77 7214  ...0..i....rowr.
+000007c0: 0000 0072 1500 0000 da09 3c67 656e 6578  ...r......<genex
+000007d0: 7072 3e46 0000 00f3 0400 0000 0280 1a00  pr>F............
+000007e0: 7a3b 6368 6563 6b5f 6966 5f72 6561 6461  z;check_if_reada
+000007f0: 626c 655f 6865 6164 6572 5f64 6566 696e  ble_header_defin
+00000800: 6974 696f 6e5f 6669 6c65 2e3c 6c6f 6361  ition_file.<loca
+00000810: 6c73 3e2e 3c67 656e 6578 7072 3e7a 2649  ls>.<genexpr>z&I
+00000820: 6e63 6f6d 706c 6574 6520 7370 6563 6966  ncomplete specif
+00000830: 6963 6174 696f 6e20 6c69 6e65 2069 6e20  ication line in 
+00000840: 4c69 6e65 2029 1472 0200 0000 da03 7365  Line ).r......se
+00000850: 7472 0e00 0000 da13 7265 6164 5f63 7376  tr......read_csv
+00000860: 5f6c 696e 6573 5f66 726f 6dda 0945 7863  _lines_from..Exc
+00000870: 6570 7469 6f6e da1c 4d61 6c66 6f72 6d65  eption..Malforme
+00000880: 6448 6561 6465 7246 696c 6545 7863 6570  dHeaderFileExcep
+00000890: 7469 6f6e da03 7374 72da 0965 6e75 6d65  tion..str..enume
+000008a0: 7261 7465 da03 6d64 64da 104f 6273 6572  rate..mdd..Obser
+000008b0: 7661 7469 6f6e 5479 7065 73da 0661 7070  vationTypes..app
+000008c0: 656e 64da 0361 6464 7205 0000 00da 0743  end..addr......C
+000008d0: 5356 5f4b 4559 7206 0000 00da 0665 7874  SV_KEYr......ext
+000008e0: 656e 64da 0574 7570 6c65 7207 0000 00da  end..tupler.....
+000008f0: 0361 6e79 da05 7072 696e 7429 0872 1a00  .any..print).r..
+00000900: 0000 da04 7365 656e da0a 6c69 6e65 735f  ....seen..lines_
+00000910: 6672 6f6d da01 65da 016b da0e 726f 775f  from..e..k..row_
+00000920: 6964 656e 7469 6669 6572 da0d 6e6f 6e5f  identifier..non_
+00000930: 656d 7074 795f 6964 78da 056c 6162 656c  empty_idx..label
+00000940: 7214 0000 0072 2400 0000 7215 0000 00da  r....r$...r.....
+00000950: 2863 6865 636b 5f69 665f 7265 6164 6162  (check_if_readab
+00000960: 6c65 5f68 6561 6465 725f 6465 6669 6e69  le_header_defini
+00000970: 7469 6f6e 5f66 696c 651f 0000 0073 5600  tion_file....sV.
+00000980: 0000 0801 0201 0e01 0e01 1001 0880 02ff  ................
+00000990: 1402 0801 0601 0a01 0801 0a01 0c01 1001  ................
+000009a0: 1001 0a01 0c01 1001 1001 0a01 0e01 0e01  ................
+000009b0: 1201 0e01 1001 0c01 1002 0c01 1001 1001  ................
+000009c0: 0a01 0e01 1001 0c01 1001 1001 1002 1801  ................
+000009d0: 0801 1001 02fe 0403 723e 0000 0063 0100  ........r>...c..
+000009e0: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+000009f0: 0000 4300 0000 733e 0000 007a 0a74 006a  ..C...s>...z.t.j
+00000a00: 017c 0064 0164 028d 027d 0157 0064 0453  .|.d.d...}.W.d.S
+00000a10: 0004 0074 0279 1e01 007d 0201 007a 0874  ...t.y...}...z.t
+00000a20: 0364 0374 047c 0283 0117 0083 0182 0164  .d.t.|.........d
+00000a30: 007d 027e 0277 0177 0029 054e 4629 01da  .}.~.w.w.).NF)..
+00000a40: 1273 7761 6c6c 6f77 5f65 7863 6570 7469  .swallow_excepti
+00000a50: 6f6e 737a 1155 6e70 6172 7361 626c 6520  onsz.Unparsable 
+00000a60: 6a73 6f6e 3a0a 5429 0572 0e00 0000 da13  json:.T).r......
+00000a70: 7265 6164 5f6a 736f 6e5f 6469 6374 5f66  read_json_dict_f
+00000a80: 726f 6d72 0300 0000 722b 0000 0072 2c00  romr....r+...r,.
+00000a90: 0000 2903 721a 0000 00da 0164 7239 0000  ..).r......dr9..
+00000aa0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000ab0: da2d 6368 6563 6b5f 6966 5f72 6561 6461  .-check_if_reada
+00000ac0: 626c 655f 6865 6164 6572 5f64 6566 696e  ble_header_defin
+00000ad0: 6974 696f 6e5f 6669 6c65 5f6a 736f 6e4c  ition_file_jsonL
+00000ae0: 0000 0073 0e00 0000 0201 1001 0403 0efe  ...s............
+00000af0: 1001 0880 02ff 7242 0000 007a 022e 2e7a  ......rB...z...z
+00000b00: 1268 6561 6465 725f 7363 6865 6d61 2e6a  .header_schema.j
+00000b10: 736f 6eda 0a72 6177 5f68 6561 6465 7263  son..raw_headerc
+00000b20: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000b30: 0a00 0000 4300 0000 7340 0000 007a 0974  ....C...s@...z.t
+00000b40: 00a0 017c 0074 02a1 0201 0057 0064 0253  ...|.t.....W.d.S
+00000b50: 0004 0074 006a 036a 0479 1f01 007d 0101  ...t.j.j.y...}..
+00000b60: 007a 0874 0564 0174 067c 0183 0117 0083  .z.t.d.t.|......
+00000b70: 0182 0164 007d 017e 0177 0177 0029 034e  ...d.}.~.w.w.).N
+00000b80: 7a1a 5363 6865 6d61 2076 616c 6964 6174  z.Schema validat
+00000b90: 696f 6e20 6661 696c 6564 2e0a 5429 07da  ion failed..T)..
+00000ba0: 0a6a 736f 6e73 6368 656d 61da 0876 616c  .jsonschema..val
+00000bb0: 6964 6174 65da 0d68 6561 6465 725f 7363  idate..header_sc
+00000bc0: 6865 6d61 da0a 6578 6365 7074 696f 6e73  hema..exceptions
+00000bd0: da0f 5661 6c69 6461 7469 6f6e 4572 726f  ..ValidationErro
+00000be0: 7272 2b00 0000 722c 0000 0029 0272 4300  rr+...r,...).rC.
+00000bf0: 0000 7239 0000 0072 1400 0000 7214 0000  ..r9...r....r...
+00000c00: 0072 1500 0000 da19 6368 6563 6b5f 6966  .r......check_if
+00000c10: 5f76 616c 6964 5f72 6177 5f68 6561 6465  _valid_raw_heade
+00000c20: 725c 0000 0073 0e00 0000 0201 0e01 0403  r\...s..........
+00000c30: 12fe 1001 0880 02ff 7249 0000 0063 0100  ........rI...c..
+00000c40: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000c50: 0000 4300 0000 7314 0000 0074 007c 0083  ..C...s....t.|..
+00000c60: 017d 0174 017c 0183 0101 0064 0153 0029  .}.t.|.....d.S.)
+00000c70: 024e 5429 0272 0a00 0000 da17 6368 6563  .NT).r......chec
+00000c80: 6b5f 6966 5f76 616c 6964 5f72 6177 5f64  k_if_valid_raw_d
+00000c90: 6174 6129 02da 0470 6174 68da 0264 6672  ata)...path..dfr
+00000ca0: 1400 0000 7214 0000 0072 1500 0000 da18  ....r....r......
+00000cb0: 6368 6563 6b5f 6966 5f76 616c 6964 5f64  check_if_valid_d
+00000cc0: 6174 615f 6669 6c65 6400 0000 7306 0000  ata_filed...s...
+00000cd0: 0008 0108 0104 0172 4d00 0000 6301 0000  .......rM...c...
+00000ce0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000cf0: 0003 0000 0073 7800 0000 7400 8700 6601  .....sx...t...f.
+00000d00: 6401 6402 8408 7401 6a02 4400 8301 8301  d.d...t.j.D.....
+00000d10: 721c 7403 6403 7404 7401 6a02 8301 7404  r.t.d.t.t.j...t.
+00000d20: 8800 6a05 8301 1800 9b00 6404 9d03 8301  ..j.......d.....
+00000d30: 8201 7406 8800 8301 0100 7407 8800 8301  ..t.......t.....
+00000d40: 7d01 7408 7409 7c01 8301 8301 7d02 7400  }.t.t.|.....}.t.
+00000d50: 6405 6402 8400 740a 7c01 7c02 8302 4400  d.d...t.|.|...D.
+00000d60: 8301 8301 723a 7403 6406 8301 8201 6407  ....r:t.d.....d.
+00000d70: 5300 2908 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000d80: 0000 0200 0000 0300 0000 3300 0000 731a  ..........3...s.
+00000d90: 0000 0081 007c 005d 087d 017c 0188 006a  .....|.].}.|...j
+00000da0: 0076 0156 0001 0071 0264 0053 00a9 014e  .v.V...q.d.S...N
+00000db0: 2901 da07 636f 6c75 6d6e 7329 0272 2200  )...columns).r".
+00000dc0: 0000 da01 63a9 0172 4c00 0000 7214 0000  ....c..rL...r...
+00000dd0: 0072 1500 0000 7226 0000 006b 0000 0073  .r....r&...k...s
+00000de0: 0400 0000 0280 1800 7a2a 6368 6563 6b5f  ........z*check_
+00000df0: 6966 5f76 616c 6964 5f72 6177 5f64 6174  if_valid_raw_dat
+00000e00: 612e 3c6c 6f63 616c 733e 2e3c 6765 6e65  a.<locals>.<gene
+00000e10: 7870 723e 7a20 4461 7461 2069 7320 6d69  xpr>z Data is mi
+00000e20: 7373 696e 6720 6261 7365 2063 6f6c 756d  ssing base colum
+00000e30: 6e28 7329 3a20 721c 0000 0063 0100 0000  n(s): r....c....
+00000e40: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000e50: 7300 0000 731c 0000 0081 007c 005d 095c  s...s......|.].\
+00000e60: 027d 017d 027c 017c 026b 0356 0001 0071  .}.}.|.|.k.V...q
+00000e70: 0264 0053 0072 4e00 0000 7214 0000 0029  .d.S.rN...r....)
+00000e80: 0372 2200 0000 da01 61da 0162 7214 0000  .r".....a..br...
+00000e90: 0072 1400 0000 7215 0000 0072 2600 0000  .r....r....r&...
+00000ea0: 7100 0000 7227 0000 007a 3350 6c61 6365  q...r'...z3Place
+00000eb0: 686f 6c64 6572 2066 6561 7475 7265 2063  holder feature c
+00000ec0: 6f6c 756d 6e73 2068 6176 6520 756e 6578  olumns have unex
+00000ed0: 7065 6374 6564 206c 6162 656c 732e 5429  pected labels.T)
+00000ee0: 0b72 3500 0000 da0a 4d44 436f 6e63 6570  .r5.....MDConcep
+00000ef0: 7473 da0c 6261 7365 5f63 6f6c 756d 6e73  ts..base_columns
+00000f00: da1a 4d61 6c66 6f72 6d65 6444 6174 6146  ..MalformedDataF
+00000f10: 696c 6545 7863 6570 7469 6f6e 7228 0000  ileExceptionr(..
+00000f20: 0072 4f00 0000 da11 6368 6563 6b5f 7469  .rO.....check_ti
+00000f30: 6d65 5f63 6f6c 756d 6eda 1467 6574 5f70  me_column..get_p
+00000f40: 6c61 6365 686f 6c64 6572 5f63 6f6c 73da  laceholder_cols.
+00000f50: 1867 656e 5f66 6561 7475 7265 5f63 6f6c  .gen_feature_col
+00000f60: 756d 6e5f 6e61 6d65 73da 036c 656e da03  umn_names..len..
+00000f70: 7a69 7029 0372 4c00 0000 da10 706c 6163  zip).rL.....plac
+00000f80: 6568 6f6c 6465 725f 636f 6c73 da0a 746f  eholder_cols..to
+00000f90: 5f62 655f 636f 6c73 7214 0000 0072 5100  _be_colsr....rQ.
+00000fa0: 0000 7215 0000 0072 4a00 0000 6a00 0000  ..r....rJ...j...
+00000fb0: 7314 0000 0018 0102 011a 0104 ff08 0208  s...............
+00000fc0: 010c 0118 0108 0104 0172 4a00 0000 2923  .........rJ...)#
+00000fd0: da02 6f73 da0b 636f 6c6c 6563 7469 6f6e  ..os..collection
+00000fe0: 7372 0200 0000 da04 6a73 6f6e 7203 0000  sr......jsonr...
+00000ff0: 0072 4400 0000 da0a 6d64 6174 612e 636f  .rD.....mdata.co
+00001000: 7265 7204 0000 00da 156d 6461 7461 2e63  rer......mdata.c
+00001010: 6f72 652e 6578 7465 6e73 696f 6e73 7205  ore.extensionsr.
+00001020: 0000 0072 0600 0000 7207 0000 00da 1b6d  ...r....r......m
+00001030: 6461 7461 2e66 696c 655f 666f 726d 6174  data.file_format
+00001040: 732e 696f 5f75 7469 6c73 7208 0000 00da  s.io_utilsr.....
+00001050: 0969 6d70 6f72 7469 6e67 720a 0000 0072  .importingr....r
+00001060: 0b00 0000 720c 0000 0072 2100 0000 720e  ....r....r!...r.
+00001070: 0000 00da 1776 616c 6964 6974 795f 6368  .....validity_ch
+00001080: 6563 6b69 6e67 5f75 7469 6c73 7216 0000  ecking_utilsr...
+00001090: 0072 1900 0000 723e 0000 0072 4200 0000  .r....r>...rB...
+000010a0: 7240 0000 0072 4b00 0000 da04 6a6f 696e  r@...rK.....join
+000010b0: da07 6469 726e 616d 65da 085f 5f66 696c  ..dirname..__fil
+000010c0: 655f 5f72 4600 0000 da0d 5261 7748 6561  e__rF.....RawHea
+000010d0: 6465 7253 7065 6372 4900 0000 724d 0000  derSpecrI...rM..
+000010e0: 0072 4a00 0000 7214 0000 0072 1400 0000  .rJ...r....r....
+000010f0: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
+00001100: 756c 653e 0100 0000 7324 0000 0008 000c  ule>....s$......
+00001110: 010c 0108 020c 0214 010c 0114 010c 0108  ................
+00001120: 0108 0308 080e 080e 2d1e 0d10 0308 080c  ........-.......
+00001130: 06                                       .
```

### Comparing `mdata-0.1.1/src/mdata/core/extensions/__pycache__/multiplicity.cpython-310.pyc` & `mdata-0.1.2/src/mdata/core/extensions/__pycache__/multiplicity.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 08:03:26 2023 UTC, .py size: 5949 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cedc 8264 3d17 0000  o..........d=...
+00000000: 6f0d 0d0a 0000 0000 11ee 8664 3d17 0000  o..........d=...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5400 6501 4700 6402 6403 8400  d.l.T.e.G.d.d...
 00000040: 6403 6502 6503 1900 8303 8301 5a04 6501  d.e.e.......Z.e.
 00000050: 4700 6404 6405 8400 6405 6504 6505 1900  G.d.d...d.e.e...
 00000060: 8303 8301 5a06 6501 4700 6406 6407 8400  ....Z.e.G.d.d...
 00000070: 6407 6504 6507 1900 8303 8301 5a08 6509  d.e.e.......Z.e.
```

### Comparing `mdata-0.1.1/src/mdata/core/extensions/multiplicity.py` & `mdata-0.1.2/src/mdata/core/extensions/multiplicity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from ..machine_data_def import *
 
 
 @dataclass
-class IndexedMachineDataTimeseries(MachineDataTimeseries[TSType]):
+class IndexedMachineDataTimeseries(MachineDataTimeseries[TSSpec]):
     indices: Collection[int]
 
 
 @dataclass
-class IndexedEventSeries(IndexedMachineDataTimeseries[EventTimeseriesType]):
+class IndexedEventSeries(IndexedMachineDataTimeseries[EventTimeseriesSpec]):
     pass
 
 
 @dataclass
-class IndexedMeasurementSeries(IndexedMachineDataTimeseries[MeasurementTimeseriesType]):
+class IndexedMeasurementSeries(IndexedMachineDataTimeseries[MeasurementTimeseriesSpec]):
     pass
 
 
 TSI = TypeVar('TSI', bound=IndexedMachineDataTimeseries)
 
 
-class TypedIndexedTimeseriesCollection(Generic[TSType, TS, TSI], TypedTimeseriesCollection[TSType, TS]):
+class TypedIndexedTimeseriesCollection(Generic[TSSpec, TS, TSI], TypedTimeseriesCollection[TSSpec, TS]):
     _tsi_cls: type[TSI] = None
 
-    def __init__(self, timeseries_type: TSType, df: pd.DataFrame) -> None:
-        super().__init__(timeseries_type, df)
+    def __init__(self, timeseries_spec: TSSpec, df: pd.DataFrame) -> None:
+        super().__init__(timeseries_spec, df)
 
     @property
     def occurring_series_indices(self) -> pd.Index:
         return self._series_indices
 
     @property
     def time_series_count(self) -> int:
@@ -40,51 +40,51 @@
         self._series_indices = self._internal_index.index.get_level_values(1).unique()
 
     def _mk_indexed_timeseries_view(self, timeseries_type, objs, indices) -> TSI:
         df = self.df.loc[self._internal_index.loc[objs, indices]]
         return self._tsi_cls(timeseries_type, df, set(df[MDConcepts.Object]), df[MDExtensionConcepts.Index].unique())
 
     def get_for_obj_and_index(self, obj, index) -> TSI:
-        return self._mk_indexed_timeseries_view(self.timeseries_type, obj, index)
+        return self._mk_indexed_timeseries_view(self.timeseries_spec, obj, index)
 
     def view_indexed(self, objs: str | list[str] | slice, indices: str | list[str] | slice) -> TSI:
         if objs is None:
             objs = slice(None)
         if indices is None:
             indices = slice(None)
-        return self._mk_indexed_timeseries_view(self.timeseries_type, objs, indices)
+        return self._mk_indexed_timeseries_view(self.timeseries_spec, objs, indices)
 
-    def _mk_timeseries_view(self, timeseries_type, objs) -> TS:
+    def _mk_timeseries_view(self, timeseries_spec, objs) -> TS:
         df = self.df.loc[self._internal_index.loc[objs, :]]
-        return self._ts_cls(timeseries_type, df, set(df[MDConcepts.Object]))
+        return self._ts_cls(timeseries_spec, df, set(df[MDConcepts.Object]))
 
     def __str__(self):
-        return f'IndexedTimeseriesCollection(type={self.timeseries_type}, #time series={self.time_series_count}, #obs={self.observation_count}, #objects={len(self.occurring_objects)}, #series_indices={len(self.occurring_series_indices)})'
+        return f'IndexedTimeseriesCollection(type={self.timeseries_spec}, #time series={self.time_series_count}, #obs={self.observation_count}, #objects={len(self.occurring_objects)}, #series_indices={len(self.occurring_series_indices)})'
 
 
 class IndexedEventTimeseriesCollection(
-    EventTimeseriesCollection, TypedIndexedTimeseriesCollection[EventTimeseriesType, EventSeries, IndexedEventSeries]):
+    EventTimeseriesCollection, TypedIndexedTimeseriesCollection[EventTimeseriesSpec, EventSeries, IndexedEventSeries]):
     #_ts_type_cls = EventTimeseriesType
     #_ts_cls = EventSeries
     _tsi_cls = IndexedEventSeries
 
 
 class IndexedMeasurementTimeseriesCollection(
-    MeasurementTimeseriesCollection, TypedIndexedTimeseriesCollection[MeasurementTimeseriesType, MeasurementSeries, IndexedMeasurementSeries]):
+    MeasurementTimeseriesCollection, TypedIndexedTimeseriesCollection[MeasurementTimeseriesSpec, MeasurementSeries, IndexedMeasurementSeries]):
     #_ts_type_cls = MeasurementTimeseriesType
     #_ts_cls = MeasurementSeries
     _tsi_cls = IndexedMeasurementSeries
 
 
 ETSI = TypeVar('ETSI', bound=IndexedMachineDataTimeseries)
 MTSI = TypeVar('MTSI', bound=IndexedMachineDataTimeseries)
 
 
 class AbstractMultiplicityMachineData(Generic[ETSI, MTSI], AbstractMachineData[
-    EventTimeseriesType, MeasurementTimeseriesType, EventSeries, MeasurementSeries, IndexedEventTimeseriesCollection, IndexedMeasurementTimeseriesCollection]):
+    EventTimeseriesSpec, MeasurementTimeseriesSpec, EventSeries, MeasurementSeries, IndexedEventTimeseriesCollection, IndexedMeasurementTimeseriesCollection]):
     _etsc_cls = IndexedEventTimeseriesCollection
     _mtsc_cls = IndexedMeasurementTimeseriesCollection
     _etsi_cls: type[ETSI] = None
     _mtsi_cls: type[MTSI] = None
 
     def recalculate_index(self, **kwargs):
         super().recalculate_index(index_cols=MDExtensionConcepts.combined_columns, **kwargs)
@@ -93,35 +93,35 @@
     def occurring_series_indices(self) -> pd.Index:
         return self._occurring_series_indices
 
     def _repopulate_maps(self):
         super()._repopulate_maps()
         self._occurring_series_indices = pd.Index(self.index_frame[MDExtensionConcepts.Index].unique())
 
-    def view_event_series(self, label: EventTypeLabel, objs: str | list[str] | slice = None,
+    def view_event_series(self, label: EventSpecLabel, objs: str | list[str] | slice = None,
                           indices: str | list | slice = None,
                           **kwargs) -> MTSI:
         assert label is not None
         return self.event_series[label].view_indexed(objs, indices)
 
-    def view_measurement_series(self, label: MeasurementTypeLabel, objs: str | list[str] | slice = None,
+    def view_measurement_series(self, label: MeasurementSpecLabel, objs: str | list[str] | slice = None,
                                 indices: str | list | slice = None,
                                 **kwargs) -> MTSI:
         assert label is not None
         return self.measurement_series[label].view_indexed(objs, indices)
 
     def summary(self):
         first = min(self.index_frame[MDConcepts.Time])
         last = max(self.index_frame[MDConcepts.Time])
         num_obs = len(self.index_frame)
-        return f'#Observations: {num_obs} between {first} and {last}.' + '\n' + f'#Objects: {len(self.occurring_objects)}' + '\n' + f'#Series Indices: {len(self.occurring_series_indices)}' + '\n' + f'#Event types: {len(self.event_series_types)}' + '\n' + f'#Measurement types: {len(self.measurement_series_types)}'
+        return f'#Observations: {num_obs} between {first} and {last}.' + '\n' + f'#Objects: {len(self.occurring_objects)}' + '\n' + f'#Series Indices: {len(self.occurring_series_indices)}' + '\n' + f'#Event types: {len(self.event_specs)}' + '\n' + f'#Measurement types: {len(self.measurement_specs)}'
 
     def __str__(self) -> str:
-        ets = '\n'.join([f'\t{l}: {", ".join(tt.features)}' for l, tt in self.event_series_types.items()])
-        mts = '\n'.join([f'\t{l}: {", ".join(tt.features)}' for l, tt in self.measurement_series_types.items()])
+        ets = '\n'.join([f'\t{l}: {", ".join(tt.features)}' for l, tt in self.event_specs.items()])
+        mts = '\n'.join([f'\t{l}: {", ".join(tt.features)}' for l, tt in self.measurement_specs.items()])
         objs = ' ' + ', '.join(self.occurring_objects)
         sidx = ' ' + str(self.occurring_series_indices)
         return 'MachineData {' + '\n' + 'Event types:' + '\n' + ets + '\n' + 'Measurement types:' + '\n' + mts + '\n' + 'Objects:' + objs + '\n' + 'Series Indices:' + sidx + '\n' + '}'
 
 
 class MultiplicityMachineData(AbstractMultiplicityMachineData[IndexedEventSeries, IndexedMeasurementSeries]):
     _etsi_cls = IndexedEventSeries
```

### Comparing `mdata-0.1.1/src/mdata/core/factory.py` & `mdata-0.1.2/src/mdata/core/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 from __future__ import annotations
 
 import itertools
+from collections.abc import Iterable
 from typing import TypedDict
 
 import pandas as pd
 
-from mdata.core.machine_data_def import MDConcepts, TimeseriesTypeFactory, only_feature_columns, \
+from mdata.core.header import ObservationSpec, Meta
+from mdata.core.machine_data_def import MDConcepts, TimeseriesSpecFactory, only_feature_columns, \
     TimeseriesCollectionFactory, EventTimeseriesCollection, MachineData, MeasurementTimeseriesCollection, \
-    MachineDataTypes, build_shared_index
-from mdata.core.raw import create_machine_data_from_raw, RawHeaderType, RawDataType
+    ObservationTypes, build_shared_index, TypedTimeseriesCollection
+from mdata.core.raw import create_machine_data_from_raw, RawHeaderSpec, RawDataType, RawMetadataFeatureSpec
+from mdata.core.util import take_first
 
 
 def ets_from_df(df: pd.DataFrame, **kwargs):
-    return ts_from_df(df, type=MachineDataTypes.E, **kwargs)
+    return ts_from_df(df, type=ObservationTypes.E, **kwargs)
 
 
 def mts_from_df(df: pd.DataFrame, **kwargs):
-    return ts_from_df(df, type=MachineDataTypes.M, **kwargs)
+    return ts_from_df(df, type=ObservationTypes.M, **kwargs)
 
 
-def ts_from_df(df: pd.DataFrame, **kwargs):
+def ts_from_df(df: pd.DataFrame, specmeta: Iterable[RawMetadataFeatureSpec] = (), copy=False,
+               **kwargs) -> TypedTimeseriesCollection:
+    df = df.copy() if copy else df
+
     def match_spec_and_df(concept, col_idx):
         spec = kwargs.get(concept)
         if concept not in df.columns:
             assert spec is not None
             df.insert(col_idx, concept, spec)
         else:
             df_type = df.iloc[0][concept]
             assert spec is None or spec == df_type
             spec = df_type
         return spec
 
     if MDConcepts.Time in kwargs:
         spec_time = kwargs[MDConcepts.Time]
-        # if spec_time == 'artificial':
-        from mdata.core import df_utils
-        df.insert(0, MDConcepts.Time, df_utils.create_artificial_daterange(df))
+        if spec_time == 'artificial':
+            from mdata.core import df_utils
+            df.insert(0, MDConcepts.Time, df_utils.create_artificial_daterange(df))
     spec_object = match_spec_and_df(MDConcepts.Object, 1)
     spec_type = match_spec_and_df(MDConcepts.Type, 2)
     spec_label = match_spec_and_df(MDConcepts.Label, 3)
 
-    tt_cls = TimeseriesTypeFactory.for_name(spec_type)
+    tspec_cls = TimeseriesSpecFactory.for_type(spec_type)
     features = only_feature_columns(df.columns)
-    tt = tt_cls(spec_label, tuple(features))
+
+    specmeta = {take_first(fspec): fspec for fspec in specmeta}
+    tt = tspec_cls(spec_label, ObservationSpec.from_raw([specmeta[f] if f in specmeta else f for f in features]))
     return TimeseriesCollectionFactory.for_type(tt)(df)
 
 
-SeriesSpec = TypedDict('SeriesSpec',
-                       {'df': pd.DataFrame, MDConcepts.Object: str, MDConcepts.Time: str, MDConcepts.Label: str},
-                       total=False)
+ObservationSeriesDef = TypedDict('ObservationSeriesDef',
+                                 {'df': pd.DataFrame, MDConcepts.Object: str, MDConcepts.Time: str,
+                                  MDConcepts.Label: str, 'specmeta': list[RawMetadataFeatureSpec]},
+                                 total=False)
 
 
-def machine_data_from_spec(*series_defs: SeriesSpec, sort_by_time=True, **kwargs):
+def machine_data_from_series(*series_defs: ObservationSeriesDef, meta: Meta = Meta(), sort_by_time=True, copy_dfs=False,
+                             **kwargs) -> MachineData:
     ets, mts = [], []
     for sd in series_defs:
         assert 'df' in sd
-        tsc = ts_from_df(**sd)
+        tsc = ts_from_df(**sd, copy=copy_dfs)
         if isinstance(tsc, EventTimeseriesCollection):
             ets.append(tsc)
         elif isinstance(tsc, MeasurementTimeseriesCollection):
             mts.append(tsc)
 
     index_frame = build_shared_index(itertools.chain(ets, mts), sort_by_time=sort_by_time, **kwargs)
-    return MachineData(ets, mts, index_frame)
+    return MachineData(meta, ets, mts, index_frame)
 
 
-def machine_data_from_df(df: RawDataType, header: RawHeaderType):
+def machine_data_from_df(df: RawDataType, header: RawHeaderSpec) -> MachineData:
     return create_machine_data_from_raw(df, header)
```

### Comparing `mdata-0.1.1/src/mdata/core/machine_data_def.py` & `mdata-0.1.2/src/mdata/core/machine_data_def.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,202 +1,191 @@
 from __future__ import annotations
 
-import enum
 import itertools
 from abc import ABC
 from dataclasses import dataclass, field
 from functools import partial
-from typing import Iterable, Generic, TypeVar, Sized, TYPE_CHECKING, Any, Iterator, Collection, Literal, ClassVar
+from typing import Iterable, Generic, TypeVar, Sized, TYPE_CHECKING, Collection, Literal, ClassVar, Callable
 
 import numpy as np
 import pandas as pd
 
 from .df_utils import derive_categoricals
+from .header import Header, ObservationSpec, Meta, FeatureSpec
 from .util import mangle_arg_to_set, mangle_arg_with_bool_fallback, mangle_arg_to_list, mangle_arg_to_tuple, \
-    symmetric_difference, intersection, assert_in
+    symmetric_difference, intersection, assert_in, StringEnumeration
 
 if TYPE_CHECKING:
-    from .raw import RawHeaderType
-
-
-class MyStrEnum(enum.Enum):
-
-    @classmethod
-    def cast(cls, arg):
-        return arg if isinstance(arg, cls) else cls(arg)
-
-    def as_str(self):
-        return str(self.value)
-
+    pass
 
 MDConcept = str
 
 
-class MDConcepts(Iterable):
+class MDConcepts(StringEnumeration):
     Time = 'time'
     Object = 'object'
     Type = 'type'
     Label = 'label'
 
     base_columns = [Time, Object, Type, Label]
 
-    def __iter__(self):
-        return iter(MDConcepts.base_columns)
 
-
-class MDExtensionConcepts(Iterable):
+class MDExtensionConcepts(StringEnumeration):
     Index = 'series_index'
 
     extension_columns = [Index]
     combined_columns = MDConcepts.base_columns + extension_columns
 
-    def __iter__(self):
-        return iter(MDExtensionConcepts.extension_columns)
-
 
 def only_feature_columns(cols):
     return [c for c in cols if (c not in MDConcepts.base_columns) and (c not in MDExtensionConcepts.extension_columns)]
 
 
 def project_on_feature_columns(df: pd.DataFrame):
     return df[only_feature_columns(df.columns)]
 
 
-TimeseriesTypeKey = tuple[str, str]
 TimeseriesFeatureLabel = str
 TimeseriesFeatureLabels = tuple[TimeseriesFeatureLabel, ...]
 
-MachineDataType = str
-
+ObservationTypeType = str
 
-class MachineDataTypes(Iterable):
-    E: MachineDataType = 'E'
-    M: MachineDataType = 'M'
-    base_types = [E, M]
 
-    def __iter__(self) -> Iterator[MachineDataType]:
-        return iter(MachineDataTypes.base_types)
+class ObservationTypes(StringEnumeration):
+    E: ObservationTypeType = 'E'
+    M: ObservationTypeType = 'M'
 
 
 ObservationTypeLabel = str
-EventTypeLabel = str
-MeasurementTypeLabel = str
+ObservationSpecIdentifier = tuple[ObservationTypeType, ObservationTypeLabel]
+
+EventSpecLabel = str
+MeasurementSpecLabel = str
+
+TimeseriesSpecType = TypeVar('TimeseriesTypeType', bound='TimeseriesSpec')
+
+
+class TimeseriesTypeMergeException(Exception):
+    pass
 
 
-TimeseriesTypeType = TypeVar('TimeseriesTypeType', bound='TimeseriesType')
+class TimeseriesCollectionMergeException(Exception):
+    pass
+
+
+class MachineDataMergeException(Exception):
+    pass
 
 
 @dataclass(frozen=True, unsafe_hash=True, eq=True, repr=True, init=False)
-class TimeseriesType(Iterable, Sized):
-    type: ClassVar[MachineDataType]
+class TimeseriesSpec(Iterable, Sized):
+    type: ClassVar[ObservationTypeType]
     label: ObservationTypeLabel
-    features: TimeseriesFeatureLabels = field(default=())
+    base: ObservationSpec
+    features: TimeseriesFeatureLabels = field(init=False)
+    display_names: TimeseriesFeatureLabels = field(init=False)
 
-    def __init__(self, label: ObservationTypeLabel, features: TimeseriesFeatureLabels = ()) -> None:
+    def __init__(self, label: ObservationTypeLabel, spec: ObservationSpec) -> None:
         super().__init__()
         object.__setattr__(self, 'label', label)
-        object.__setattr__(self, 'features', features if isinstance(features, tuple) else tuple(features))
+        object.__setattr__(self, 'base', spec)
+        object.__setattr__(self, 'features', tuple((f.name for f in spec)))
+        object.__setattr__(self, 'display_names', tuple((f.print_name for f in spec)))
 
     def __iter__(self):
         return iter(self.features)
 
     def __len__(self):
         return len(self.features)
 
-    def askey(self) -> TimeseriesTypeKey:
+    @property
+    def identifier(self) -> ObservationSpecIdentifier:
         return self.type, self.label
 
-    def is_mergeable(self, other: TimeseriesType) -> bool:
+    def is_mergeable(self, other: TimeseriesSpec) -> bool:
         return (self.__class__ == other.__class__) and (self.type == other.type) and (self.label == other.label)
 
-    def feature_intersection(self, other: TimeseriesType) -> set[str]:
-        return set(self.features) & set(other.features)
+    def feature_intersection(self, other: TimeseriesSpec) -> list[str]:
+        return [f for f in self.features if f in set(other.features)]
 
-    def feature_symmetric_difference(self, other: TimeseriesType) -> tuple[set[str], set[str]]:
-        s1, s2 = set(self.features), set(other.features)
-        return s1 - s2, s2 - s1
+    def feature_symmetric_difference(self, other: TimeseriesSpec) -> tuple[list[str], list[str]]:
+        return [f for f in self.features if f not in set(other.features)], [f for f in other.features if
+                                                                            f not in set(self.features)]
 
-    def project(self: TimeseriesTypeType, feature_selection: bool | str | Collection[str]) -> TimeseriesTypeType:
+    def project(self: TimeseriesSpecType, feature_selection: bool | str | Collection[str]) -> TimeseriesSpecType:
         feature_selection = mangle_arg_with_bool_fallback(mangle_arg_to_tuple, feature_selection, if_true=self.features)
         assert all(f in self.features for f in feature_selection)
-        return self.__class__(self.label, feature_selection)
+        return self.__class__(self.label, ObservationSpec.of(*(self.base[f] for f in feature_selection)))
 
-    def merge(self: TimeseriesTypeType, other: TimeseriesTypeType) -> TimeseriesTypeType:
+    def merge(self: TimeseriesSpecType, other: TimeseriesSpecType) -> TimeseriesSpecType:
         assert self.is_mergeable(other)
-        return self.__class__(self.label,
-                              mangle_arg_to_tuple(itertools.chain(self.features, other.features), rm_duplicates=True))
+        specs = list(self.base.features)
+        for fspec in other.base:
+            if fspec not in self.base:
+                specs.append(fspec)
+            elif self.base[fspec.name] != fspec:
+                print('redefined', self.base, self.base[fspec.name], fspec.name)
+                raise TimeseriesTypeMergeException
+        return self.__class__(self.label, ObservationSpec.of(*specs))
 
 
 @dataclass(frozen=True, init=False)
-class EventTimeseriesType(TimeseriesType):
-    type = MachineDataTypes.E
+class EventTimeseriesSpec(TimeseriesSpec):
+    type = ObservationTypes.E
 
 
 @dataclass(frozen=True, init=False)
-class MeasurementTimeseriesType(TimeseriesType):
-    type = MachineDataTypes.M
+class MeasurementTimeseriesSpec(TimeseriesSpec):
+    type = ObservationTypes.M
 
 
-class TimeseriesTypeFactory:
-    types = {MachineDataTypes.E: EventTimeseriesType, MachineDataTypes.M: MeasurementTimeseriesType}
+class TimeseriesSpecFactory:
+    types = {ObservationTypes.E: EventTimeseriesSpec, ObservationTypes.M: MeasurementTimeseriesSpec}
 
     @classmethod
-    def for_name(cls, arg: str):
+    def for_type(cls, arg: str) -> Callable[[ObservationTypeLabel, ObservationSpec], TimeseriesSpec]:
         return cls.types[arg]
 
 
-@dataclass(frozen=True, eq=True, repr=True)
-class Header:
-    feature_definitions: dict[TimeseriesTypeKey, TimeseriesType]
-    extensions: set[MDExtensionConcepts] = field(init=False, default_factory=set)
-
-    @classmethod
-    def from_raw(cls, raw_feature_definitions: RawHeaderType):
-        return cls({k: TimeseriesTypeFactory.for_name(k[0])(k[1], v) for k, v in raw_feature_definitions.items()})
-
-    def __getitem__(self, item) -> TimeseriesFeatureLabels:
-        return self.feature_definitions[item].features
-
-
-TSType = TypeVar('TSType', bound=TimeseriesType)
+TSSpec = TypeVar('TSSpec', bound=TimeseriesSpec)
 
 
 @dataclass
-class AbstractMachineDataTimeseries(Generic[TSType], ABC):
-    timeseries_type: TSType
+class AbstractMachineDataTimeseries(Generic[TSSpec], ABC):
+    timeseries_spec: TSSpec
     df: pd.DataFrame
 
 
 @dataclass
-class MachineDataTimeseries(AbstractMachineDataTimeseries[TSType]):
+class MachineDataTimeseries(AbstractMachineDataTimeseries[TSSpec]):
     objects: Collection[str]
 
 
 @dataclass
-class EventSeries(MachineDataTimeseries[EventTimeseriesType]):
+class EventSeries(MachineDataTimeseries[EventTimeseriesSpec]):
     pass
 
 
 @dataclass
-class MeasurementSeries(MachineDataTimeseries[MeasurementTimeseriesType]):
+class MeasurementSeries(MachineDataTimeseries[MeasurementTimeseriesSpec]):
     pass
 
 
 TS = TypeVar('TS', bound=MachineDataTimeseries)
 
 TTC = TypeVar('TTC', bound='TypedTimeseriesCollection')
 
 
-class TypedTimeseriesCollection(Generic[TSType, TS], ABC):
-    _ts_type_cls: type[TSType] = None
+class TypedTimeseriesCollection(Generic[TSSpec, TS], ABC):
+    _ts_spec_cls: type[TSSpec] = None
     _ts_cls: type[TS] = None
 
-    def __init__(self, timeseries_type: TSType, df: pd.DataFrame) -> None:
+    def __init__(self, timeseries_spec: TSSpec, df: pd.DataFrame) -> None:
         super().__init__()
-        self.timeseries_type: TSType = timeseries_type
+        self.timeseries_spec: TSSpec = timeseries_spec
         self.df: pd.DataFrame = df
         self._object_map: dict[str, TS] = {}
         self._repopulate_internal_index()
 
     @property
     def observation_count(self) -> int:
         return len(self.df)
@@ -211,177 +200,205 @@
 
     @property
     def object_map(self) -> dict[str, TS]:
         return self._object_map
 
     @property
     def feature_column_view(self):
-        return self.df.loc[:, list(self.timeseries_type.features)]
+        return self.df.loc[:, list(self.timeseries_spec.features)]
+
+    @property
+    def prefixed_feature_column_view(self):
+        df = self.feature_column_view
+        return df.rename(
+            {c: self.timeseries_spec.type + '_' + self.timeseries_spec.label + '_' + c for c in df.columns},
+            inplace=False)
 
     def _repopulate_internal_index(self):
         self._internal_index = pd.Series(self.df.index, index=self.df[MDConcepts.Object])
         self._occurring_objects = set(self._internal_index.index)
         self._object_map = {obj: self.view(obj) for obj in self._occurring_objects}
 
     def _check_ts_features(self):
-        return set(self.timeseries_type.features) <= set(self.df.columns)
+        return set(self.timeseries_spec.features) <= set(self.df.columns)
 
-    def _mk_timeseries_view(self, timeseries_type, objs) -> TS:
+    def _mk_timeseries_view(self, timeseries_spec, objs) -> TS:
         df = self.df.loc[self._internal_index.loc[objs]]
-        return self._ts_cls(timeseries_type, df, set(df[MDConcepts.Object]))
+        return self._ts_cls(timeseries_spec, df, set(df[MDConcepts.Object]))
 
-    def _update_timeseries_type(self, timeseries_type: TSType = None) -> None:
-        self.timeseries_type = self._derive_timeseries_type()
+    def _update_timeseries_spec(self, timeseries_spec: TSSpec = None) -> None:
+        self.timeseries_spec = self._derive_timeseries_spec() if timeseries_spec is None else timeseries_spec
         assert self._check_ts_features()
 
-    def _derive_timeseries_type(self) -> TSType:
-        return self._ts_type_cls(self.timeseries_type.label,
-                                 only_feature_columns(self.df.columns))
+    def _derive_timeseries_spec(self) -> TSSpec:
+        current_features = only_feature_columns(self.df.columns)
+        from .extensions import metadata
+
+        specs: list[FeatureSpec] = []
+        for f in current_features:
+            fdt = metadata.get_type(self.df.loc[:, f])
+            long_name = f
+            if f in self.timeseries_spec.base:
+                fspec: FeatureSpec = self.timeseries_spec.base[f]
+                long_name = fspec.print_name
+            specs.append(FeatureSpec(f, long_name, fdt))
+
+        return self._ts_spec_cls(self.timeseries_spec.label, ObservationSpec(*specs))
 
     def update_index(self):
         self._repopulate_internal_index()
 
     def fit_to_data(self) -> None:
-        self._update_timeseries_type()
+        self._update_timeseries_spec()
         self.update_index()
 
     def view(self, objs: str | list[str] | slice) -> TS:
         objs = slice(None) if objs is None else objs
-        return self._mk_timeseries_view(self.timeseries_type, objs)
+        return self._mk_timeseries_view(self.timeseries_spec, objs)
 
     def __str__(self):
-        return f'TimeseriesCollection(type={self.timeseries_type}, #time series={self.time_series_count}, #obs={self.observation_count}, #objects={len(self.occurring_objects)})'
+        return f'TimeseriesCollection(spec={self.timeseries_spec}, #obs={self.observation_count}, #objects={len(self.occurring_objects)})'
 
     def __repr__(self) -> str:
         return str(self)
 
     def merge(self: TTC, other: TTC,
               axis: Literal['horizontal', 'vertical'] = 'vertical') -> TTC:
         assert axis in {'horizontal', 'vertical'}
         if axis == 'horizontal':
-            assert self.timeseries_type.is_mergeable(other.timeseries_type)
-            ov = self.timeseries_type.feature_intersection(other.timeseries_type)
+            assert self.timeseries_spec.is_mergeable(other.timeseries_spec)
+            ov = self.timeseries_spec.feature_intersection(other.timeseries_spec)
             if ov:
-                assert np.array_equal(self.df.loc[:, ov].values, other.df.loc[:, ov].values)
-            _, new_fs = self.timeseries_type.feature_symmetric_difference(other.timeseries_type)
+                assert self.df.loc[:, ov].equals(
+                    other.df.loc[:, ov])  # np.array_equal(self.df.loc[:, ov].values, other.df.loc[:, ov].values)
+            _, new_fs = self.timeseries_spec.feature_symmetric_difference(other.timeseries_spec)
             if new_fs:
-                assert self.df[MDConcepts.Time] == other.df[MDConcepts.Time]
-                df = pd.concat([self.df, other.df.loc[:, new_fs]], axis='columns', ignore_index=True, copy=True)
-                return self.__class__(self.timeseries_type.merge(other.timeseries_type), df)
+                assert self.df[MDConcepts.Time].equals(other.df[MDConcepts.Time])
+                df = pd.concat([self.df, other.df.loc[:, new_fs]], axis='columns', copy=True)
+                return self.__class__(self.timeseries_spec.merge(other.timeseries_spec), df)
             return self
         elif axis == 'vertical':
-            assert self.timeseries_type == other.timeseries_type
+            assert self.timeseries_spec == other.timeseries_spec
             df = pd.concat([self.df, other.df], axis='index', ignore_index=True, copy=True)
             df.sort_values(MDConcepts.Time, ignore_index=True, inplace=True)
-            return self.__class__(self.timeseries_type, df)
+            return self.__class__(self.timeseries_spec, df)
 
     @classmethod
     def lifted_merge(cls: type[TTC], tscs: dict[str, TTC], o_tscs: dict[str, TTC],
                      axis: Literal['horizontal', 'vertical'] = 'vertical') -> dict[str, TTC]:
         assert axis in {'horizontal', 'vertical'}
         ov = intersection(tscs.keys(), o_tscs.keys())
         s1, s2 = symmetric_difference(tscs.keys(), o_tscs.keys())
         res = {e: tscs[e] for e in s1} | {e: tscs[e].merge(o_tscs[e], axis=axis) for e in ov}
         if axis == 'horizontal':
             return res
         elif axis == 'vertical':
             return res | {e: o_tscs[e] for e in s2}
 
 
-class EventTimeseriesCollection(TypedTimeseriesCollection[EventTimeseriesType, EventSeries]):
-    _ts_type_cls = EventTimeseriesType
+class EventTimeseriesCollection(TypedTimeseriesCollection[EventTimeseriesSpec, EventSeries]):
+    _ts_spec_cls = EventTimeseriesSpec
     _ts_cls = EventSeries
 
 
-class MeasurementTimeseriesCollection(TypedTimeseriesCollection[MeasurementTimeseriesType, MeasurementSeries]):
-    _ts_type_cls = MeasurementTimeseriesType
+class MeasurementTimeseriesCollection(TypedTimeseriesCollection[MeasurementTimeseriesSpec, MeasurementSeries]):
+    _ts_spec_cls = MeasurementTimeseriesSpec
     _ts_cls = MeasurementSeries
 
 
-ETSType = TypeVar('ETSType', bound=TimeseriesType)
-MTSType = TypeVar('MTSType', bound=TimeseriesType)
+ETSType = TypeVar('ETSType', bound=TimeseriesSpec)
+MTSType = TypeVar('MTSType', bound=TimeseriesSpec)
 
 ETS = TypeVar('ETS', bound=MachineDataTimeseries)
 MTS = TypeVar('MTS', bound=MachineDataTimeseries)
 
 ETSC = TypeVar('ETSC', bound=TypedTimeseriesCollection)
 MTSC = TypeVar('MTSC', bound=TypedTimeseriesCollection)
 
 
 class TimeseriesCollectionFactory:
-    types = {MachineDataTypes.E: EventTimeseriesCollection, MachineDataTypes.M: MeasurementTimeseriesCollection}
+    types = {ObservationTypes.E: EventTimeseriesCollection, ObservationTypes.M: MeasurementTimeseriesCollection}
 
     @classmethod
-    def for_type(cls, timeseries_type: TimeseriesType):
-        if isinstance(timeseries_type, EventTimeseriesType):
-            return partial(cls.types[MachineDataTypes.E], timeseries_type)
-        elif isinstance(timeseries_type, MeasurementTimeseriesType):
-            return partial(cls.types[MachineDataTypes.M], timeseries_type)
+    def for_type(cls, timeseries_spec: TimeseriesSpec) -> Callable[[pd.DataFrame], TypedTimeseriesCollection]:
+        if isinstance(timeseries_spec, EventTimeseriesSpec):
+            return partial(cls.types[ObservationTypes.E], timeseries_spec)
+        elif isinstance(timeseries_spec, MeasurementTimeseriesSpec):
+            return partial(cls.types[ObservationTypes.M], timeseries_spec)
 
 
 AMD = TypeVar('AMD', bound='AbstractMachineData')
 
 
 class AbstractMachineData(Generic[ETSType, MTSType, ETS, MTS, ETSC, MTSC], ABC):
     _etsc_cls: type[ETSC] = None
     _mtsc_cls: type[MTSC] = None
 
-    def __init__(self, events: Iterable[ETSC],
+    def __init__(self, meta: Meta, events: Iterable[ETSC],
                  measurements: Iterable[MTSC],
                  index_frame: pd.DataFrame = None) -> None:
         self._index_frame: pd.DataFrame = index_frame
-        self.event_series_types: dict[EventTypeLabel, ETSType]
-        self.measurement_series_types: dict[MeasurementTypeLabel, MTSType]
-        self.event_series: dict[EventTypeLabel, ETSC] = {etc.timeseries_type.label: etc for etc in events}
-        self.measurement_series: dict[MeasurementTypeLabel, MTSC] = {mtc.timeseries_type.label: mtc for mtc in
+        self.meta: Meta = meta
+        self.event_specs: dict[EventSpecLabel, ETSType]
+        self.measurement_specs: dict[MeasurementSpecLabel, MTSType]
+        self.event_series: dict[EventSpecLabel, ETSC] = {etc.timeseries_spec.label: etc for etc in events}
+        self.measurement_series: dict[MeasurementSpecLabel, MTSC] = {mtc.timeseries_spec.label: mtc for mtc in
                                                                      measurements}
         self._repopulate_maps()
 
     @property
+    def header(self):
+        return Header(self.meta, {e: tspec.base for e, tspec in self.event_specs.items()},
+                      {m: tspec.base for m, tspec in self.measurement_specs.items()})
+
+    @property
     def index_frame(self) -> pd.DataFrame:
         if self._index_frame is None:
             self.recalculate_index()
         return self._index_frame
 
     @index_frame.setter
     def index_frame(self, value: pd.DataFrame):
         self._index_frame = value
 
     @property
     def occurring_objects(self) -> set[str]:
         return self._occurring_objects
 
     @property
+    def observation_count(self) -> int:
+        return len(self.index_frame)
+
+    @property
     def series_containers(self) -> list[ETSC | MTSC]:
         return list(self.event_series.values()) + list(self.measurement_series.values())
 
     @classmethod
     def from_series(cls: type[AMD], events: Iterable[ETSC],
-                    measurements: Iterable[MTSC], lazy_index_creation=True) -> AMD:
-        md = cls(events, measurements)
+                    measurements: Iterable[MTSC], lazy_index_creation=True, meta: Meta = Meta()) -> AMD:
+        md = cls(meta, events, measurements)
         if not lazy_index_creation:
             md.recalulate_index()
         return md
 
-    def recalculate_index(self, **kwargs):
+    def recalculate_index(self, override_categorical_types=True, sort_by_time=True, **kwargs):
         self._index_frame = build_shared_index(self.series_containers,
-                                               override_categorical_types=kwargs.pop('override_categorical_types',
-                                                                                     True),
-                                               sort_by_time=kwargs.pop('sort_by_time', True), **kwargs)
+                                               override_categorical_types=override_categorical_types,
+                                               sort_by_time=sort_by_time, **kwargs)
 
     def _repopulate_maps(self):
-        self.event_series_types = {es.timeseries_type.label: es.timeseries_type for es in self.event_series.values()}
-        self.measurement_series_types = {ms.timeseries_type.label: ms.timeseries_type for ms in
-                                         self.measurement_series.values()}
-        self.iter_all_timeseries()
+        self.event_specs = {es.timeseries_spec.label: es.timeseries_spec for es in
+                            self.event_series.values()}
+        self.measurement_specs = {ms.timeseries_spec.label: ms.timeseries_spec for ms in
+                                  self.measurement_series.values()}
         self._occurring_objects = set(self.index_frame[MDConcepts.Object])
 
     def fit_to_data(self, recreate_index=False):
         for tsc in self.iter_all_timeseries():
-            # retain only the rows that are referenced in the overall table
+            # retain only the rows that are referenced in the overall index
             if not recreate_index:
                 tsc.df = tsc.df.filter(items=self.index_frame.index, axis=0)
             tsc.fit_to_data()
 
         if recreate_index:
             self.recalculate_index()
         else:
@@ -391,31 +408,34 @@
             self.index_frame = self.index_frame.loc[mask]
 
         self._repopulate_maps()
 
     def iter_all_timeseries(self) -> Iterable[TypedTimeseriesCollection]:
         return itertools.chain(self.event_series.values(), self.measurement_series.values())
 
-    def create_joined_df(self, event_series_labels: Iterable[EventTypeLabel] | bool = None,
-                         measurement_series_labels: Iterable[MeasurementTypeLabel] | bool = None):
-        event_keys = self.event_series_types.keys()
+    def create_joined_df(self, event_series_labels: Iterable[EventSpecLabel] | bool = None,
+                         measurement_series_labels: Iterable[MeasurementSpecLabel] | bool = None,
+                         prefix_columns_to_avoid_collisions=True):
+        event_keys = self.event_specs.keys()
         esl = mangle_arg_with_bool_fallback(mangle_arg_to_tuple, event_series_labels,
                                             if_true=event_keys,
                                             rm_duplicates=True, preserve_order=True)
         assert_in(esl, event_keys)
-        measurement_keys = self.measurement_series_types.keys()
+        measurement_keys = self.measurement_specs.keys()
         msl = mangle_arg_with_bool_fallback(mangle_arg_to_tuple, measurement_series_labels,
                                             if_true=measurement_keys,
                                             rm_duplicates=True, preserve_order=True)
         assert_in(msl, measurement_keys)
-        return pd.concat([self.index_frame] + [self.event_series[est].feature_column_view for est in esl] + [
-            self.measurement_series[mst].feature_column_view for mst in msl], axis='columns', copy=False)
-
-    def create_index_view(self, typ: MachineDataType = None, types: Collection[MachineDataType] = None, obj: str = None,
-                          label: ObservationTypeLabel = None, objs: Iterable[str] = None,
+        return pd.concat([self.index_frame] + [
+            tsc.prefixed_feature_column_view if prefix_columns_to_avoid_collisions else tsc.feature_column_view for
+            tsc in self.series_containers], axis='columns', copy=False)
+
+    def create_index_view(self, typ: ObservationTypeType = None, types: Collection[ObservationTypeType] = None,
+                          obj: str = None, objs: Iterable[str] = None,
+                          label: ObservationTypeLabel = None,
                           labels: Iterable[ObservationTypeLabel] = None) -> pd.DataFrame:
         assert typ is None or types is None
         assert obj is None or objs is None
         assert label is None or labels is None
 
         mask = pd.Series(True, index=self.index_frame.index)
         if obj is not None:
@@ -430,129 +450,141 @@
             mask &= (self.index_frame[MDConcepts.Type] == typ)
         elif types is not None:
             mask &= (self.index_frame[MDConcepts.Type].isin(mangle_arg_to_set(typ)))
 
         return self.index_frame.loc[mask]
 
     def project(self: AMD,
-                measurement_feature_selection: dict[MeasurementTypeLabel, bool | Collection[TimeseriesFeatureLabel]] = None,
-                event_feature_selection: dict[EventTypeLabel, bool | Collection[TimeseriesFeatureLabel]] = None,
+                measurement_feature_selection: dict[
+                    MeasurementSpecLabel, bool | Collection[TimeseriesFeatureLabel]] = None,
+                event_feature_selection: dict[EventSpecLabel, bool | Collection[TimeseriesFeatureLabel]] = None,
                 project_underlying_dfs=False, copy_underlying_dfs=False) -> AMD:
         if measurement_feature_selection is None:
             measurement_feature_selection = {}
         if event_feature_selection is None:
             event_feature_selection = {}
         ms = []
         for m, fs in measurement_feature_selection.items():
             fs = mangle_arg_with_bool_fallback(mangle_arg_to_list, fs,
-                                               if_true=self.measurement_series_types[m].features, preserve_order=True)
+                                               if_true=self.measurement_specs[m].features,
+                                               preserve_order=True)
             mtc = self.measurement_series[m]
-            tt = mtc.timeseries_type.project(fs)
-            df = mtc.df.loc[:, MDConcepts.base_columns + list(tt.features)] if project_underlying_dfs else mtc.df
+            tspec = mtc.timeseries_spec.project(fs)
+            df = mtc.df.loc[:, MDConcepts.base_columns + list(tspec.features)] if project_underlying_dfs else mtc.df
             if copy_underlying_dfs:
                 df = df.copy()
-            ms.append(self._mtsc_cls(tt, df))
+            ms.append(self._mtsc_cls(tspec, df))
         es = []
         for m, fs in event_feature_selection.items():
             fs = mangle_arg_with_bool_fallback(mangle_arg_to_tuple, event_feature_selection,
-                                               if_true=self.event_series_types.keys(), preserve_order=True)
+                                               if_true=self.event_specs.keys(), preserve_order=True)
             etc = self.event_series[m]
-            tt = etc.timeseries_type.project(fs)
-            df = etc.df.loc[:, MDConcepts.base_columns + list(tt.features)] if project_underlying_dfs else etc.df
+            tspec = etc.timeseries_spec.project(fs)
+            df = etc.df.loc[:, MDConcepts.base_columns + list(tspec.features)] if project_underlying_dfs else etc.df
             if copy_underlying_dfs:
                 df = df.copy()
-            es.append(self._etsc_cls(tt, df))
+            es.append(self._etsc_cls(tspec, df))
 
         index_view = self.create_index_view(
             labels=itertools.chain(measurement_feature_selection.keys(), event_feature_selection.keys()))
         if copy_underlying_dfs:
             index_view = index_view.copy()
-        return self.__class__(es, ms, index_frame=index_view)
+        return self.__class__(self.meta, es, ms, index_frame=index_view)
 
     def is_mergeable(self, other: AbstractMachineData):
         if self.__class__ != other.__class__:
             return False
-        for e, et in self.event_series_types.items():
-            if o_et := other.event_series_types.get(e):
+        for e, et in self.event_specs.items():
+            if o_et := other.event_specs.get(e):
                 if not et.is_mergeable(o_et):
                     return False
-        for m, mt in self.measurement_series_types.items():
-            if o_mt := other.measurement_series_types.get(m):
+        for m, mt in self.measurement_specs.items():
+            if o_mt := other.measurement_specs.get(m):
                 if not mt.is_mergeable(o_mt):
                     return False
         return True
 
     def merge(self: AMD, other: AMD,
               axis: Literal['horizontal', 'vertical'] = 'horizontal') -> AMD:
-        return self.merge_series(other.event_series, other.measurement_series, axis=axis)
-
-    def merge_series(self, event_series: dict[EventTypeLabel, ETSC], measurement_series: dict[MeasurementTypeLabel, MTSC],
-                     axis: Literal['horizontal', 'vertical'] = 'horizontal'):
+        result = self.merge_series(other.event_series, other.measurement_series, axis=axis)
+        result.meta = self.meta.merge(other.meta)
+        return result
+
+    def merge_series(self, event_series: dict[EventSpecLabel, ETSC],
+                     measurement_series: dict[MeasurementSpecLabel, MTSC],
+                     axis: Literal['horizontal', 'vertical'] = 'horizontal') -> AMD:
         assert axis in {'horizontal', 'vertical'}
-        recalc_index = axis == 'vertical'
+        recalc_index = axis == 'vertical'  # TODO actually detect if index changed #or (tsc. for tsc in event_series.values())
         if event_series is None:
             event_series = {}
         if measurement_series is None:
             measurement_series = {}
         es: dict[str, ETSC] = self._etsc_cls.lifted_merge(self.event_series, event_series, axis=axis)
         ms: dict[str, MTSC] = self._mtsc_cls.lifted_merge(self.measurement_series, measurement_series, axis=axis)
         if recalc_index:
-            return self.from_series(es.values(), ms.values())
+            return self.__class__(self.meta, es.values(), ms.values())
         else:
-            return self.__class__(es.values(), ms.values(), self.index_frame)
+            return self.__class__(self.meta, es.values(), ms.values(), self.index_frame)
 
-    def get_event_series_collection(self, label: EventTypeLabel) -> ETSC:
+    def get_event_series_collection(self, label: EventSpecLabel) -> ETSC:
         return self.event_series[label]
 
-    def get_measurement_series_collection(self, label: MeasurementTypeLabel) -> MTSC:
+    def get_measurement_series_collection(self, label: MeasurementSpecLabel) -> MTSC:
         return self.measurement_series[label]
 
-    def view_measurement_series(self, label: MeasurementTypeLabel, objs: str | list[str] | slice = slice(None), **kwargs) -> MTS:
+    def view_measurement_series(self, label: MeasurementSpecLabel, objs: str | list[str] | slice = slice(None),
+                                **kwargs) -> MTS:
         return self.measurement_series[label].view(objs=objs)
 
-    def view_event_series(self, label: EventTypeLabel, objs: str | list[str] | slice = slice(None), **kwargs) -> ETS:
+    def view_event_series(self, label: EventSpecLabel, objs: str | list[str] | slice = slice(None),
+                          **kwargs) -> ETS:
         return self.event_series[label].view(objs=objs)
 
     def summary(self):
         first = min(self.index_frame[MDConcepts.Time])
         last = max(self.index_frame[MDConcepts.Time])
-        num_obs = len(self.index_frame)
-        return f'#Observations: {num_obs} between {first} and {last}.' + '\n' + f'#Objects: {len(self.occurring_objects)}' + '\n' + f'#Event types: {len(self.event_series_types)}' + '\n' + f'#Measurement types: {len(self.measurement_series_types)}'
+        return f'#Observations: {self.observation_count} between {first} and {last}.' + '\n' + f'#Objects: {len(self.occurring_objects)}' + '\n' + f'#Event Specs: {len(self.event_specs)}' + '\n' + f'#Measurement Specs: {len(self.measurement_specs)}'
 
     def __str__(self):
-        ets = '\n'.join([f'\t{l}: {", ".join(tt.features)}' for l, tt in self.event_series_types.items()])
-        mts = '\n'.join([f'\t{l}: {", ".join(tt.features)}' for l, tt in self.measurement_series_types.items()])
+        def spec_strings(specs_dict):
+            return '\n'.join([f'\t{l}: {", ".join(tspec.features)}' for l, tspec in specs_dict.items()])
+
+        especs = spec_strings(self.event_specs)
+        mspecs = spec_strings(self.measurement_specs)
         objs = ' ' + ', '.join(self.occurring_objects)
-        return 'MachineData {' + '\n' + 'Event types:' + '\n' + ets + '\n' + 'Measurement types:' + '\n' + mts + '\n' + 'Objects:' + objs + '\n' + '}'
+        return 'MachineData {' + '\n' + 'Event Specs:' + (
+            '\n' + especs if especs != "" else "[]") + '\n' + 'Measurement Specs:' + (
+            '\n' + mspecs if mspecs != "" else "[]") + '\n' + 'Objects:' + objs + '\n' + f'Observations: {self.observation_count}' + '\n' + '}'
 
     def __repr__(self):
         return str(self)
 
 
 class MachineData(AbstractMachineData[
-                      EventTimeseriesType, MeasurementTimeseriesType, EventSeries, MeasurementSeries, EventTimeseriesCollection, MeasurementTimeseriesCollection]):
+                      EventTimeseriesSpec, MeasurementTimeseriesSpec, EventSeries, MeasurementSeries, EventTimeseriesCollection, MeasurementTimeseriesCollection]):
     _etsc_cls = EventTimeseriesCollection
     _mtsc_cls = MeasurementTimeseriesCollection
 
 
-def build_shared_index(series: Iterable[TypedTimeseriesCollection], index_cols=None, override_categorical_types=True,
+def build_shared_index(series: Iterable[TypedTimeseriesCollection], index_cols=None,
+                       override_categorical_types=True,
                        sort_by_time=False):
     if index_cols is None:
         index_cols = MDConcepts.base_columns
     series = list(series)
     lengths = [len(tsc.df) for tsc in series]
     orig_idx_ranges = np.empty(len(lengths) + 1, dtype=int)
     np.cumsum(lengths, out=orig_idx_ranges[1:])
     orig_idx_ranges[0] = 0
 
     frame = pd.concat((tsc.df[index_cols] for tsc in series), ignore_index=True, join='inner',
                       copy=False)
 
     if sort_by_time:
-        sorted_idx = np.argsort(frame[MDConcepts.Time])
+        sorted_idx = np.argsort(frame[MDConcepts.Time].values)
         frame = frame.iloc[sorted_idx]
         frame.reset_index(drop=True, inplace=True)
         rev = np.empty_like(sorted_idx)
         rev[sorted_idx] = np.arange(len(sorted_idx))
         for tsc, start, end in zip(series, orig_idx_ranges[:-1], orig_idx_ranges[1:]):
             tsc.df.index = pd.Index(rev[start:end])
             tsc.update_index()
@@ -563,8 +595,7 @@
 
     cats = derive_categoricals(frame, [MDConcepts.Object, MDConcepts.Type, MDConcepts.Label])
     frame = frame.astype(cats, copy=False)
     if override_categorical_types:
         for tsc in series:
             tsc.df = tsc.df.astype(cats, copy=False)
     return frame
-
```

### Comparing `mdata-0.1.1/src/mdata/core/raw.py` & `mdata-0.1.2/src/mdata/core/raw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,131 @@
 from __future__ import annotations
 
+from typing import TypedDict, Any
+
 import numpy as np
 import pandas as pd
 
 from .df_utils import derive_categoricals
-from .machine_data_def import MDConcepts, TimeseriesTypeKey, TimeseriesFeatureLabels, Header, \
-    EventTimeseriesCollection, MeasurementTimeseriesCollection, MachineData, TimeseriesCollectionFactory, \
-    MachineDataTypes
-
-COLUMN_NAME_DICT = {
-    # internal to external label mapping
-    MDConcepts.Time: 'time',
-    MDConcepts.Object: 'object',
-    MDConcepts.Type: 'type',
-    MDConcepts.Label: 'label'
-}
-base_raw_machine_data_columns = list(map(COLUMN_NAME_DICT.get, MDConcepts.base_columns))
-
-MACHINE_DATA_TYPES_DICT = {
-    MachineDataTypes.E: 'E',
-    MachineDataTypes.M: 'M'
-}
-raw_machine_data_types = set(map(MACHINE_DATA_TYPES_DICT.get, MachineDataTypes.base_types))
+from .extensions import metadata
+from .header import create_header_from_raw, ObservationSpec, convert_header_to_raw
+from .machine_data_def import MDConcepts, EventTimeseriesCollection, MeasurementTimeseriesCollection, MachineData, \
+    TimeseriesCollectionFactory, TimeseriesSpecFactory
 
 
 def gen_feature_column_names(n):
     return [f'f_{i}' for i in range(1, n + 1)]
 
 
-RawHeaderType = dict[TimeseriesTypeKey, TimeseriesFeatureLabels]
+class FeatureMetadata(TypedDict, total=False):
+    data_type: str
+    print_name: str
+
+
+RawBaseFeatureSpec = str
+RawMetadataFeatureSpec = dict[str, FeatureMetadata]
+RawObservationSpecs = dict[str, list[RawBaseFeatureSpec | RawMetadataFeatureSpec]]
+
+
+class RawAnnotationSpecs(TypedDict, total=True):
+    input: RawObservationSpecs
+    output: RawObservationSpecs
+
+
+class RawHeaderSpec(TypedDict, total=False):
+    extensions: list[str]
+    event_specs: RawObservationSpecs
+    measurement_specs: RawObservationSpecs
+    annotation_specs: RawAnnotationSpecs
+    metadata: dict[str, Any]
+
+
 RawDataType = pd.DataFrame
 
 
-def convert_to_raw_header(md: MachineData) -> RawHeaderType:
-    header = {}
-    for typed_timeseries in md.iter_all_timeseries():
-        tt = typed_timeseries.timeseries_type
-        header[tt.askey()] = tuple(tt.features)
-    return header
+def convert_to_raw_header(md: MachineData) -> RawHeaderSpec:
+    return convert_header_to_raw(md.header)
 
 
 def convert_to_raw_data(md: MachineData) -> RawDataType:
-    max_features = max(map(lambda md_timeseries: len(md_timeseries.timeseries_type), md.iter_all_timeseries()))
-    #dfs = [pd.DataFrame(tsc.df[base_machine_data_columns + list(tsc.timeseries_type.features)], copy=False) for tsc in
+    max_features = max(map(lambda md_timeseries: len(md_timeseries.timeseries_spec), md.iter_all_timeseries()))
+    # dfs = [pd.DataFrame(tsc.df[base_machine_data_columns + list(tsc.timeseries_type.features)], copy=False) for tsc in
     #       md.iter_all_timeseries()]
-    #for df, tsc in zip(dfs, md.iter_all_timeseries()):
+    # for df, tsc in zip(dfs, md.iter_all_timeseries()):
     #    df.columns = base_machine_data_columns + gen_feature_column_names(len(tsc.timeseries_type.features))
-    #res = md.index_frame.join((df.drop(base_machine_data_columns, axis=1) for df in dfs), how='inner')
+    # res = md.index_frame.join((df.drop(base_machine_data_columns, axis=1) for df in dfs), how='inner')
     # TODO CHANGE BACK
 
-    res = pd.DataFrame(md.index_frame, copy=True)#.reindex(columns=))
+    res = pd.DataFrame(md.index_frame, copy=True)  # .reindex(columns=))
     res[gen_feature_column_names(max_features)] = np.NAN
 
-    #res.columns = base_raw_machine_data_columns + gen_feature_column_names(max_features)
+    # res.columns = base_raw_machine_data_columns + gen_feature_column_names(max_features)
     for tsc in md.iter_all_timeseries():
         df = tsc.df
-        cs = gen_feature_column_names(len(tsc.timeseries_type.features))
-        res.loc[df.index, cs] = df.loc[:, list(tsc.timeseries_type.features)].values
+        cs = gen_feature_column_names(len(tsc.timeseries_spec.features))
+        res.loc[df.index, cs] = df.loc[:, list(tsc.timeseries_spec.features)].values
 
     res.columns = MDConcepts.base_columns + gen_feature_column_names(max_features)
-    #res = pd.concat(dfs, ignore_index=True, copy=False, verify_integrity=False, join='inner') # TODO check copying
+    # res = pd.concat(dfs, ignore_index=True, copy=False, verify_integrity=False, join='inner') # TODO check copying
 
-    #res.sort_values(COLUMN_NAME_DICT[MDConcepts.Time], ascending=True, inplace=True)
+    # res.sort_values(COLUMN_NAME_DICT[MDConcepts.Time], ascending=True, inplace=True)
     return res
 
 
 def convert_to_raw_data_legacy(md: MachineData) -> RawDataType:
-    max_features = max(map(lambda md_timeseries: len(md_timeseries.timeseries_type), md.iter_all_timeseries()))
+    max_features = max(map(lambda md_timeseries: len(md_timeseries.timeseries_spec), md.iter_all_timeseries()))
     rows = []
     for typed_timeseries in md.iter_all_timeseries():
-        tt = typed_timeseries.timeseries_type
+        tt = typed_timeseries.timeseries_spec
         df = typed_timeseries.df
         for tup in df.itertuples(index=True):
             rows.append(
                 [getattr(tup, MDConcepts.Time), getattr(tup, MDConcepts.Object), tt.type,
                  tt.label] + [getattr(tup, f)
                               for f in
                               tt.features if
                               f in df.columns])
-    res = pd.DataFrame(rows, columns=(base_raw_machine_data_columns + gen_feature_column_names(max_features)))
-    res.sort_values(COLUMN_NAME_DICT[MDConcepts.Time], inplace=True)
+    res = pd.DataFrame(rows, columns=(MDConcepts.base_columns + gen_feature_column_names(max_features)))
+    res.sort_values(MDConcepts.Time, inplace=True)
     return res
 
 
-def create_header_from_raw(feature_definitions: RawHeaderType) -> Header:
-    return Header.from_raw(feature_definitions)
-
-
-def create_machine_data_from_raw(raw_data: RawDataType, raw_header: RawHeaderType):
+def create_machine_data_from_raw(raw_data: RawDataType, raw_header: RawHeaderSpec):
     header = create_header_from_raw(raw_header)
 
     mdes, mdms = [], []
 
-    categories = derive_categoricals(raw_data,
-                                     map(COLUMN_NAME_DICT.get, [MDConcepts.Object, MDConcepts.Label, MDConcepts.Type]))
-
-    base_colum_mapping = {old: new for new, old in COLUMN_NAME_DICT.items()}
+    categories = derive_categoricals(raw_data, [MDConcepts.Object, MDConcepts.Label, MDConcepts.Type])
 
-    overall = pd.DataFrame(raw_data, columns=base_raw_machine_data_columns, copy=True)
-    overall.rename(columns=base_colum_mapping, inplace=True)
+    overall = pd.DataFrame(raw_data, columns=MDConcepts.base_columns, copy=True)
     overall = overall.astype(categories, copy=False)
 
-    for group, idx in overall.groupby([COLUMN_NAME_DICT[MDConcepts.Type], COLUMN_NAME_DICT[MDConcepts.Label]]).groups.items():
+    for group, idx in overall.groupby([MDConcepts.Type, MDConcepts.Label]).groups.items():
         tpy, label = group
-        timeseries_type = header.feature_definitions[tpy, label]
+        spec: ObservationSpec = header.lookup_spec(tpy, label)
+
+        timeseries_type = TimeseriesSpecFactory.for_type(tpy)(label, spec)
+
         actual_feature_labels = timeseries_type.features
         feature_count = len(actual_feature_labels)
         placeholder_feature_labels = gen_feature_column_names(feature_count)
         df = pd.concat([overall.loc[idx, MDConcepts.base_columns], raw_data.loc[idx, placeholder_feature_labels]],
                        copy=True, axis=1).set_index(idx)
         # relevant_cols = list(base_machine_data_columns) + placeholder_feature_labels
         # df = pd.DataFrame(raw_data.loc[idx, relevant_cols], copy=True)
         # not a good idea in case of duplicates
         # df.set_index('time', inplace=True, verify_integrity=True, drop=False)
-        # df = df.astype(categories, copy=False)
         renaming_dict = {old: new for old, new in zip(placeholder_feature_labels, actual_feature_labels)}
-        # renaming_dict.update(base_colum_mapping)
         df.rename(columns=renaming_dict, inplace=True)
+
+        metadata.convert_df_inplace(df, {f.name: f.data_type for f in spec})
+
         ts_collection = TimeseriesCollectionFactory.for_type(timeseries_type)(df)
         if isinstance(ts_collection, EventTimeseriesCollection):
             mdes.append(ts_collection)
         elif isinstance(ts_collection, MeasurementTimeseriesCollection):
             mdms.append(ts_collection)
 
     placeholder_cols = list(set(overall.columns).difference(MDConcepts.base_columns))
     overall.drop(columns=placeholder_cols, inplace=True)
 
-    return MachineData(mdes, mdms, overall)
+    return MachineData(header.meta, mdes, mdms, index_frame=overall)
```

### Comparing `mdata-0.1.1/src/mdata/core/util.py` & `mdata-0.1.2/src/mdata/core/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,43 @@
 from __future__ import annotations
 
-from collections.abc import Iterable, Collection
+import enum
+from collections.abc import Iterable, Collection, Sized, Iterator
+from typing import Any, Optional
+
+
+class MyMeta(Iterable, Sized, type):
+    def __new__(cls, name, bases, dct):
+        cli = super().__new__(cls, name, bases, dct)
+        cli.value_map = {k: v for k, v in dct.items() if not str.startswith(k, '_') and type(v) is str}
+        cli.values = list(cli.value_map.values())
+        return cli
+
+    def __getitem__(self, key) -> str:
+        if key in self.value_map:
+            return self.value_map[key]
+        elif key in self.values:
+            return key
+
+    def __len__(self) -> int:
+        return len(self.value_map)
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self.values)
+
+    def derive_enum(cls, name=None):
+        return enum.Enum(cls.__class__.__name__[:-1] if name is None else name, cls.value_map)
+
+
+class StringEnumeration(metaclass=MyMeta):
+    pass
+
+
+def take_first(arg: Iterable[Any]) -> Optional[Any]:
+    return next(iter(arg), None)
 
 
 def intersection(a, b) -> set:
     if a is None or b is None:
         return set()
     else:
         return set(a) & set(b)
```

### Comparing `mdata-0.1.1/src/mdata/file_formats/__pycache__/io_utils.cpython-310.pyc` & `mdata-0.1.2/src/mdata/file_formats/__pycache__/io_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 13:07:38 2023 UTC, .py size: 2009 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,152 @@
-00000000: 6f0d 0d0a 0000 0000 9a5d 6f64 d907 0000  o........]od....
+00000000: 6f0d 0d0a 0000 0000 67c1 9264 fd08 0000  o.......g..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0173 5400 0000 6400  .....@...sT...d.
+00000020: 0004 0000 0040 0000 0173 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6404 6405 8400 5a06 6413  m.Z...d.d...Z.d.
-00000060: 6407 6408 8401 5a07 6414 6415 640e 640f  d.d...Z.d.d.d.d.
-00000070: 8405 5a08 6416 6411 6412 8404 5a09 6402  ..Z.d.d.d...Z.d.
-00000080: 5300 2917 e900 0000 0029 01da 0b61 6e6e  S.)......)...ann
-00000090: 6f74 6174 696f 6e73 4e29 01da 084f 7074  otationsN)...Opt
-000000a0: 696f 6e61 6c63 0100 0000 0000 0000 0000  ionalc..........
-000000b0: 0000 0200 0000 0400 0000 4300 0001 733a  ..........C...s:
-000000c0: 0000 0074 006a 01a0 027c 00a1 017d 017c  ...t.j...|...}.|
-000000d0: 0164 016b 0372 1974 006a 01a0 037c 01a1  .d.k.r.t.j...|..
-000000e0: 0173 1b74 006a 047c 0164 0264 038d 0201  .s.t.j.|.d.d....
-000000f0: 0064 0053 0064 0053 0064 0053 0029 044e  .d.S.d.S.d.S.).N
-00000100: da00 5429 01da 0865 7869 7374 5f6f 6b29  ..T)...exist_ok)
-00000110: 05da 026f 73da 0470 6174 68da 0764 6972  ...os..path..dir
-00000120: 6e61 6d65 da06 6578 6973 7473 da08 6d61  name..exists..ma
-00000130: 6b65 6469 7273 2902 7207 0000 0072 0800  kedirs).r....r..
-00000140: 0000 a900 720b 0000 00fa 4643 3a5c 5573  ....r.....FC:\Us
-00000150: 6572 735c 4c65 6168 5c50 7963 6861 726d  ers\Leah\Pycharm
-00000160: 5072 6f6a 6563 7473 5c6d 6461 7461 5c73  Projects\mdata\s
-00000170: 7263 5c6d 6461 7461 5c66 696c 655f 666f  rc\mdata\file_fo
-00000180: 726d 6174 735c 696f 5f75 7469 6c73 2e70  rmats\io_utils.p
-00000190: 79da 1765 6e73 7572 655f 6469 7265 6374  y..ensure_direct
-000001a0: 6f72 795f 6578 6973 7473 0800 0000 7308  ory_exists....s.
-000001b0: 0000 000c 0114 0112 0108 ff72 0d00 0000  ...........r....
-000001c0: 5463 0300 0000 0000 0000 0000 0000 0500  Tc..............
-000001d0: 0000 0300 0000 4300 0001 7338 0000 0074  ......C...s8...t
-000001e0: 006a 01a0 027c 00a1 015c 027d 037d 047c  .j...|...\.}.}.|
-000001f0: 0464 0075 0073 167c 0464 016b 0273 167c  .d.u.s.|.d.k.s.|
-00000200: 0272 1a7c 047c 016b 0372 1a7c 007c 0117  .r.|.|.k.r.|.|..
-00000210: 0053 007c 0053 0029 024e 7204 0000 0029  .S.|.S.).Nr....)
-00000220: 0372 0600 0000 7207 0000 00da 0873 706c  .r....r......spl
-00000230: 6974 6578 7429 0572 0700 0000 5a0b 6465  itext).r....Z.de
-00000240: 7369 7265 645f 6578 74da 0c6f 7665 7272  sired_ext..overr
-00000250: 6964 655f 6578 74da 0170 da01 6572 0b00  ide_ext..p..er..
-00000260: 0000 720b 0000 0072 0c00 0000 da0a 656e  ..r....r......en
-00000270: 7375 7265 5f65 7874 0e00 0000 7308 0000  sure_ext....s...
-00000280: 0010 011c 0108 0104 0272 1200 0000 fa05  .........r......
-00000290: 7574 662d 38da 0361 7267 fa31 7374 7220  utf-8..arg.1str 
-000002a0: 7c20 6f73 2e50 6174 684c 696b 655b 7374  | os.PathLike[st
-000002b0: 725d 207c 2069 6f2e 4279 7465 7349 4f20  r] | io.BytesIO 
-000002c0: 7c20 696f 2e53 7472 696e 6749 4fda 0672  | io.StringIO..r
-000002d0: 6574 7572 6efa 194f 7074 696f 6e61 6c5b  eturn..Optional[
-000002e0: 6c69 7374 5b6c 6973 745b 7374 725d 5d5d  list[list[str]]]
-000002f0: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00000300: 0008 0000 0043 0000 0173 b000 0000 6400  .....C...s....d.
-00000310: 7d02 6401 7d03 7400 7c00 7401 7402 6a03  }.d.}.t.|.t.t.j.
-00000320: 4200 8302 721e 7404 7c00 6402 6401 6403  B...r.t.|.d.d.d.
-00000330: 8d03 7d00 7405 7c00 6404 6405 7c01 6406  ..}.t.|.d.d.|.d.
-00000340: 8d04 7d02 6407 7d03 6e17 7400 7c00 7406  ..}.d.}.n.t.|.t.
-00000350: 6a07 8302 722d 7406 6a08 7c00 7c01 6405  j...r-t.j.|.|.d.
-00000360: 6408 8d03 7d02 6e08 7400 7c00 7406 6a09  d...}.n.t.|.t.j.
-00000370: 8302 7235 7c00 7d02 6409 6400 6c0a 7d04  ..r5|.}.d.d.l.}.
-00000380: 7a16 7c04 6a0b 7c02 640a 640b 8d02 7d05  z.|.j.|.d.d...}.
-00000390: 640c 640d 8400 7c05 4400 8301 5700 7c03  d.d...|.D...W.|.
-000003a0: 724f 7c02 a00c a100 0100 5300 5300 7c03  rO|.......S.S.|.
-000003b0: 7257 7c02 a00c a100 0100 7700 7700 290e  rW|.......w.w.).
-000003c0: 4e46 7a04 2e63 7376 a901 720f 0000 00da  NFz..csv..r.....
-000003d0: 0172 7204 0000 00a9 02da 076e 6577 6c69  .rr........newli
-000003e0: 6e65 da08 656e 636f 6469 6e67 54a9 0272  ne..encodingT..r
-000003f0: 1c00 0000 721b 0000 0072 0100 0000 da05  ....r....r......
-00000400: 6578 6365 6c29 01da 0764 6961 6c65 6374  excel)...dialect
-00000410: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000420: 0003 0000 0053 0000 0173 1000 0000 6700  .....S...s....g.
-00000430: 7c00 5d04 7d01 7c01 9102 7102 5300 720b  |.].}.|...q.S.r.
-00000440: 0000 0072 0b00 0000 2902 da02 2e30 7219  ...r....)....0r.
-00000450: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000460: 0000 da0a 3c6c 6973 7463 6f6d 703e 2400  ....<listcomp>$.
-00000470: 0000 7302 0000 0010 007a 2772 6561 645f  ..s......z'read_
-00000480: 6373 765f 6c69 6e65 735f 6672 6f6d 2e3c  csv_lines_from.<
-00000490: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000004a0: 703e 290d da0a 6973 696e 7374 616e 6365  p>)...isinstance
-000004b0: da03 7374 7272 0600 0000 da08 5061 7468  ..strr......Path
-000004c0: 4c69 6b65 7212 0000 00da 046f 7065 6eda  Liker......open.
-000004d0: 0269 6fda 0742 7974 6573 494f da0d 5465  .io..BytesIO..Te
-000004e0: 7874 494f 5772 6170 7065 72da 0853 7472  xtIOWrapper..Str
-000004f0: 696e 6749 4fda 0363 7376 da06 7265 6164  ingIO..csv..read
-00000500: 6572 da05 636c 6f73 6529 0672 1400 0000  er..close).r....
-00000510: 721c 0000 00da 0673 6f75 7263 65da 0e6c  r......source..l
-00000520: 6f63 616c 6c79 5f6f 7065 6e65 6472 2a00  ocally_openedr*.
-00000530: 0000 722b 0000 0072 0b00 0000 720b 0000  ..r+...r....r...
-00000540: 0072 0c00 0000 da13 7265 6164 5f63 7376  .r......read_csv
-00000550: 5f6c 696e 6573 5f66 726f 6d16 0000 0073  _lines_from....s
-00000560: 2600 0000 0401 0401 1001 0e01 1001 0601  &...............
-00000570: 0c01 1201 0c01 0401 0801 0201 0e01 0e01  ................
-00000580: 0402 0a01 06ff 0a01 02ff 722f 0000 00fa  ..........r/....
-00000590: 0e4f 7074 696f 6e61 6c5b 6469 6374 5d63  .Optional[dict]c
-000005a0: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-000005b0: 0800 0000 4300 0001 73d4 0000 0064 007d  ....C...s....d.}
-000005c0: 0164 017d 0264 0264 036c 006d 017d 0301  .d.}.d.d.l.m.}..
-000005d0: 007a 577a 4374 027c 0074 0374 046a 0542  .zWzCt.|.t.t.j.B
-000005e0: 0083 0272 2674 067c 0064 0464 0164 058d  ...r&t.|.d.d.d..
-000005f0: 037d 0074 077c 0064 0664 0764 0864 098d  .}.t.|.d.d.d.d..
-00000600: 047d 0164 0a7d 026e 1774 027c 0074 086a  .}.d.}.n.t.|.t.j
-00000610: 0983 0272 3574 086a 0a7c 0064 0864 0764  ...r5t.j.|.d.d.d
-00000620: 0b8d 037d 016e 0874 027c 0074 086a 0b83  ...}.n.t.|.t.j..
-00000630: 0272 3d7c 007d 0164 0264 006c 007d 047c  .r=|.}.d.d.l.}.|
-00000640: 04a0 0c7c 01a1 0157 0057 007c 0272 4e7c  ...|...W.W.|.rN|
-00000650: 01a0 0da1 0001 0053 0053 0004 007c 0379  .......S.S...|.y
-00000660: 6101 0001 0001 0059 0057 007c 0272 5f7c  a......Y.W.|.r_|
-00000670: 01a0 0da1 0001 0064 0053 0064 0053 0077  .......d.S.d.S.w
-00000680: 007c 0272 697c 01a0 0da1 0001 0077 0077  .|.ri|.......w.w
-00000690: 0029 0c4e 4672 0100 0000 2901 da0f 4a53  .).NFr....)...JS
-000006a0: 4f4e 4465 636f 6465 4572 726f 727a 052e  ONDecodeErrorz..
-000006b0: 6a73 6f6e 7218 0000 0072 1900 0000 7204  jsonr....r....r.
-000006c0: 0000 0072 1300 0000 721a 0000 0054 721d  ...r....r....Tr.
-000006d0: 0000 0029 0eda 046a 736f 6e72 3100 0000  ...)...jsonr1...
-000006e0: 7222 0000 0072 2300 0000 7206 0000 0072  r"...r#...r....r
-000006f0: 2400 0000 7212 0000 0072 2500 0000 7226  $...r....r%...r&
-00000700: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
-00000710: 0000 da04 6c6f 6164 722c 0000 0029 0572  ....loadr,...).r
-00000720: 1400 0000 722d 0000 0072 2e00 0000 7231  ....r-...r....r1
-00000730: 0000 0072 3200 0000 720b 0000 0072 0b00  ...r2...r....r..
-00000740: 0000 720c 0000 00da 1372 6561 645f 6a73  ..r......read_js
-00000750: 6f6e 5f64 6963 745f 6672 6f6d 2a00 0000  on_dict_from*...
-00000760: 7334 0000 0004 0104 010c 0104 0110 010e  s4..............
-00000770: 0110 0106 010c 0112 010c 0104 0108 010c  ................
-00000780: 0104 040a 0102 ff0c fd04 0104 020c 0104  ................
-00000790: ff02 fd04 030a 0102 ff72 3400 0000 2901  .........r4...).
-000007a0: 5429 0172 1300 0000 2904 7214 0000 0072  T).r....).r....r
-000007b0: 1500 0000 7216 0000 0072 1700 0000 2904  ....r....r....).
-000007c0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-000007d0: 3000 0000 290a da0a 5f5f 6675 7475 7265  0...)...__future
-000007e0: 5f5f 7202 0000 0072 2600 0000 7206 0000  __r....r&...r...
-000007f0: 00da 0674 7970 696e 6772 0300 0000 720d  ...typingr....r.
-00000800: 0000 0072 1200 0000 722f 0000 0072 3400  ...r....r/...r4.
-00000810: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00000820: 0072 0c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000830: 0100 0000 7310 0000 000c 0008 0208 010c  ....s...........
-00000840: 0108 030a 060c 080e 14                   .........
+00000050: 6d05 5a05 0100 6404 6405 8400 5a06 6417  m.Z...d.d...Z.d.
+00000060: 6407 6408 8401 5a07 6508 6503 6a09 6508  d.d...Z.e.e.j.e.
+00000070: 1900 4200 650a 4200 650b 4200 6502 6a0c  ..B.e.B.e.B.e.j.
+00000080: 4200 6502 6a0d 4200 5a0e 0909 090a 6418  B.e.j.B.Z.....d.
+00000090: 6419 640f 6410 8405 5a0f 641a 641b 6412  d.d.d...Z.d.d.d.
+000000a0: 6413 8405 5a10 641c 641d 6415 6416 8405  d...Z.d.d.d.d...
+000000b0: 5a11 6402 5300 291e e900 0000 0029 01da  Z.d.S.)......)..
+000000c0: 0b61 6e6e 6f74 6174 696f 6e73 4e29 01da  .annotationsN)..
+000000d0: 084f 7074 696f 6e61 6c63 0100 0000 0000  .Optionalc......
+000000e0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000000f0: 0001 733a 0000 0074 006a 01a0 027c 00a1  ..s:...t.j...|..
+00000100: 017d 017c 0164 016b 0372 1974 006a 01a0  .}.|.d.k.r.t.j..
+00000110: 037c 01a1 0173 1b74 006a 047c 0164 0264  .|...s.t.j.|.d.d
+00000120: 038d 0201 0064 0053 0064 0053 0064 0053  .....d.S.d.S.d.S
+00000130: 0029 044e da00 5429 01da 0865 7869 7374  .).N..T)...exist
+00000140: 5f6f 6b29 05da 026f 73da 0470 6174 68da  _ok)...os..path.
+00000150: 0764 6972 6e61 6d65 da06 6578 6973 7473  .dirname..exists
+00000160: da08 6d61 6b65 6469 7273 2902 7207 0000  ..makedirs).r...
+00000170: 0072 0800 0000 a900 720b 0000 00fa 4643  .r......r.....FC
+00000180: 3a5c 5573 6572 735c 4c65 6168 5c50 7963  :\Users\Leah\Pyc
+00000190: 6861 726d 5072 6f6a 6563 7473 5c6d 6461  harmProjects\mda
+000001a0: 7461 5c73 7263 5c6d 6461 7461 5c66 696c  ta\src\mdata\fil
+000001b0: 655f 666f 726d 6174 735c 696f 5f75 7469  e_formats\io_uti
+000001c0: 6c73 2e70 79da 1765 6e73 7572 655f 6469  ls.py..ensure_di
+000001d0: 7265 6374 6f72 795f 6578 6973 7473 0800  rectory_exists..
+000001e0: 0000 7308 0000 000c 0114 0112 0108 ff72  ..s............r
+000001f0: 0d00 0000 5463 0300 0000 0000 0000 0000  ....Tc..........
+00000200: 0000 0500 0000 0300 0000 4300 0001 7338  ..........C...s8
+00000210: 0000 0074 006a 01a0 027c 00a1 015c 027d  ...t.j...|...\.}
+00000220: 037d 047c 0464 0075 0073 167c 0464 016b  .}.|.d.u.s.|.d.k
+00000230: 0273 167c 0272 1a7c 047c 016b 0372 1a7c  .s.|.r.|.|.k.r.|
+00000240: 007c 0117 0053 007c 0053 0029 024e 7204  .|...S.|.S.).Nr.
+00000250: 0000 0029 0372 0600 0000 7207 0000 00da  ...).r....r.....
+00000260: 0873 706c 6974 6578 7429 0572 0700 0000  .splitext).r....
+00000270: da0b 6465 7369 7265 645f 6578 74da 0c6f  ..desired_ext..o
+00000280: 7665 7272 6964 655f 6578 74da 0170 da01  verride_ext..p..
+00000290: 6572 0b00 0000 720b 0000 0072 0c00 0000  er....r....r....
+000002a0: da0a 656e 7375 7265 5f65 7874 0e00 0000  ..ensure_ext....
+000002b0: 7308 0000 0010 011c 0108 0104 0272 1300  s............r..
+000002c0: 0000 fa05 2e6a 736f 6efa 0575 7466 2d38  .....json..utf-8
+000002d0: da03 6172 67da 0a44 6174 6153 6f75 7263  ..arg..DataSourc
+000002e0: 65da 0672 6574 7572 6efa 1874 7570 6c65  e..return..tuple
+000002f0: 5b69 6f2e 5374 7269 6e67 494f 2c20 626f  [io.StringIO, bo
+00000300: 6f6c 5d63 0300 0000 0000 0000 0000 0000  ol]c............
+00000310: 0500 0000 0600 0000 4300 0001 73bc 0000  ........C...s...
+00000320: 007c 007d 0364 017d 0474 007c 0074 0183  .|.}.d.}.t.|.t..
+00000330: 0272 0d7c 00a0 02a1 007d 0074 007c 0074  .r.|.....}.t.|.t
+00000340: 0383 0272 2374 046a 0574 04a0 067c 00a1  ...r#t.j.t...|..
+00000350: 017c 0264 0264 038d 037d 0364 047d 047c  .|.d.d...}.d.}.|
+00000360: 037c 0466 0253 0074 007c 0074 0774 086a  .|.f.S.t.|.t.t.j
+00000370: 0942 0083 0272 4074 0a7c 007c 0164 0164  .B...r@t.|.|.d.d
+00000380: 058d 037d 0074 0b7c 0064 0664 027c 0264  ...}.t.|.d.d.|.d
+00000390: 078d 047d 0364 047d 047c 037c 0466 0253  ...}.d.}.|.|.f.S
+000003a0: 0074 007c 0074 046a 0c83 0272 4c7c 007d  .t.|.t.j...rL|.}
+000003b0: 037c 037c 0466 0253 0074 007c 0074 046a  .|.|.f.S.t.|.t.j
+000003c0: 0683 0272 5a74 046a 057c 007c 0264 0264  ...rZt.j.|.|.d.d
+000003d0: 038d 037d 037c 037c 0466 0253 0029 084e  ...}.|.|.f.S.).N
+000003e0: 4672 0400 0000 2902 da08 656e 636f 6469  Fr....)...encodi
+000003f0: 6e67 da07 6e65 776c 696e 6554 2902 720f  ng..newlineT).r.
+00000400: 0000 0072 1000 0000 da01 7229 0272 1b00  ...r......r).r..
+00000410: 0000 721a 0000 0029 0dda 0a69 7369 6e73  ..r....)...isins
+00000420: 7461 6e63 65da 0a6d 656d 6f72 7976 6965  tance..memoryvie
+00000430: 77da 0774 6f62 7974 6573 da05 6279 7465  w..tobytes..byte
+00000440: 73da 0269 6fda 0d54 6578 7449 4f57 7261  s..io..TextIOWra
+00000450: 7070 6572 da07 4279 7465 7349 4fda 0373  pper..BytesIO..s
+00000460: 7472 7206 0000 00da 0850 6174 684c 696b  trr......PathLik
+00000470: 6572 1300 0000 da04 6f70 656e da08 5374  er......open..St
+00000480: 7269 6e67 494f 2905 7216 0000 00da 0d65  ringIO).r......e
+00000490: 7870 6563 7465 645f 6669 6c65 721a 0000  xpected_filer...
+000004a0: 00da 0673 6f75 7263 65da 0e6c 6f63 616c  ...source..local
+000004b0: 6c79 5f6f 7065 6e65 6472 0b00 0000 720b  ly_openedr....r.
+000004c0: 0000 0072 0c00 0000 da10 6372 6561 7465  ...r......create
+000004d0: 5f73 7472 696e 675f 696f 1900 0000 7326  _string_io....s&
+000004e0: 0000 0004 0304 010a 0108 010a 0216 0104  ................
+000004f0: 0108 0910 f80e 0110 0104 0108 050c fc04  ................
+00000500: 0108 030c fe10 0108 0172 2b00 0000 fa19  .........r+.....
+00000510: 4f70 7469 6f6e 616c 5b6c 6973 745b 6c69  Optional[list[li
+00000520: 7374 5b73 7472 5d5d 5d63 0200 0000 0000  st[str]]]c......
+00000530: 0000 0000 0000 0600 0000 0800 0000 4300  ..............C.
+00000540: 0001 7358 0000 0074 007c 0064 017c 0164  ..sX...t.|.d.|.d
+00000550: 028d 035c 027d 027d 0364 0364 006c 017d  ...\.}.}.d.d.l.}
+00000560: 047a 167c 046a 027c 0264 0464 058d 027d  .z.|.j.|.d.d...}
+00000570: 0564 0664 0784 007c 0544 0083 0157 007c  .d.d...|.D...W.|
+00000580: 0372 237c 02a0 03a1 0001 0053 0053 007c  .r#|.......S.S.|
+00000590: 0372 2b7c 02a0 03a1 0001 0077 0077 0029  .r+|.......w.w.)
+000005a0: 084e 7a04 2e63 7376 a902 7228 0000 0072  .Nz..csv..r(...r
+000005b0: 1a00 0000 7201 0000 00da 0565 7863 656c  ....r......excel
+000005c0: 2901 da07 6469 616c 6563 7463 0100 0000  )...dialectc....
+000005d0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000005e0: 5300 0001 7310 0000 0067 007c 005d 047d  S...s....g.|.].}
+000005f0: 017c 0191 0271 0253 0072 0b00 0000 720b  .|...q.S.r....r.
+00000600: 0000 0029 02da 022e 3072 1c00 0000 720b  ...)....0r....r.
+00000610: 0000 0072 0b00 0000 720c 0000 00da 0a3c  ...r....r......<
+00000620: 6c69 7374 636f 6d70 3e35 0000 0073 0200  listcomp>5...s..
+00000630: 0000 1000 7a27 7265 6164 5f63 7376 5f6c  ....z'read_csv_l
+00000640: 696e 6573 5f66 726f 6d2e 3c6c 6f63 616c  ines_from.<local
+00000650: 733e 2e3c 6c69 7374 636f 6d70 3e29 0472  s>.<listcomp>).r
+00000660: 2b00 0000 da03 6373 76da 0672 6561 6465  +.....csv..reade
+00000670: 72da 0563 6c6f 7365 2906 7216 0000 0072  r..close).r....r
+00000680: 1a00 0000 7229 0000 0072 2a00 0000 7232  ....r)...r*...r2
+00000690: 0000 0072 3300 0000 720b 0000 0072 0b00  ...r3...r....r..
+000006a0: 0000 720c 0000 00da 1372 6561 645f 6373  ..r......read_cs
+000006b0: 765f 6c69 6e65 735f 6672 6f6d 2f00 0000  v_lines_from/...
+000006c0: 7314 0000 0012 0208 0102 010e 010e 0104  s...............
+000006d0: 020a 0106 ff0a 0102 ff72 3500 0000 fa0e  .........r5.....
+000006e0: 4f70 7469 6f6e 616c 5b64 6963 745d 6303  Optional[dict]c.
+000006f0: 0000 0000 0000 0000 0000 0008 0000 000a  ................
+00000700: 0000 0043 0000 0173 9600 0000 7400 7c00  ...C...s....t.|.
+00000710: 6401 7c01 6402 8d03 5c02 7d03 7d04 6403  d.|.d...\.}.}.d.
+00000720: 6404 6c01 6d02 7d05 0100 7a33 7a12 6403  d.l.m.}...z3z.d.
+00000730: 6400 6c01 7d06 7c06 a003 7c03 a101 5700  d.l.}.|...|...W.
+00000740: 5700 7c04 7222 7c03 a004 a100 0100 5300  W.|.r"|.......S.
+00000750: 5300 0400 7c05 7942 0100 7d07 0100 7a14  S...|.yB..}...z.
+00000760: 7c02 723c 5700 5900 6400 7d07 7e07 5700  |.r<W.Y.d.}.~.W.
+00000770: 7c04 723a 7c03 a004 a100 0100 6400 5300  |.r:|.......d.S.
+00000780: 6400 5300 7c07 8201 6400 7d07 7e07 7701  d.S.|...d.}.~.w.
+00000790: 7700 7c04 724a 7c03 a004 a100 0100 7700  w.|.rJ|.......w.
+000007a0: 7700 2905 4e72 1400 0000 722d 0000 0072  w.).Nr....r-...r
+000007b0: 0100 0000 2901 da0f 4a53 4f4e 4465 636f  ....)...JSONDeco
+000007c0: 6465 4572 726f 7229 0572 2b00 0000 da04  deError).r+.....
+000007d0: 6a73 6f6e 7237 0000 00da 046c 6f61 6472  jsonr7.....loadr
+000007e0: 3400 0000 2908 7216 0000 0072 1a00 0000  4...).r....r....
+000007f0: da12 7377 616c 6c6f 775f 6578 6365 7074  ..swallow_except
+00000800: 696f 6e73 7229 0000 0072 2a00 0000 7237  ionsr)...r*...r7
+00000810: 0000 0072 3800 0000 7212 0000 0072 0b00  ...r8...r....r..
+00000820: 0000 720b 0000 0072 0c00 0000 da13 7265  ..r....r......re
+00000830: 6164 5f6a 736f 6e5f 6469 6374 5f66 726f  ad_json_dict_fro
+00000840: 6d3b 0000 0073 2800 0000 1202 0c01 0401  m;...s(.........
+00000850: 0801 0c01 0407 0a01 02ff 0efa 0401 0c01  ................
+00000860: 0404 0c01 04ff 04fe 0880 02fc 0406 0a01  ................
+00000870: 02ff 723b 0000 0029 0154 2902 7214 0000  ..r;...).T).r...
+00000880: 0072 1500 0000 2904 7216 0000 0072 1700  .r....).r....r..
+00000890: 0000 7218 0000 0072 1900 0000 2901 7215  ..r....r....).r.
+000008a0: 0000 0029 0472 1600 0000 7217 0000 0072  ...).r....r....r
+000008b0: 1800 0000 722c 0000 0029 0272 1500 0000  ....r,...).r....
+000008c0: 5429 0472 1600 0000 7217 0000 0072 1800  T).r....r....r..
+000008d0: 0000 7236 0000 0029 12da 0a5f 5f66 7574  ..r6...)...__fut
+000008e0: 7572 655f 5f72 0200 0000 7221 0000 0072  ure__r....r!...r
+000008f0: 0600 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00000900: 0072 0d00 0000 7213 0000 0072 2400 0000  .r....r....r$...
+00000910: 7225 0000 0072 2000 0000 721e 0000 0072  r%...r ...r....r
+00000920: 2300 0000 7227 0000 0072 1700 0000 722b  #...r'...r....r+
+00000930: 0000 0072 3500 0000 723b 0000 0072 0b00  ...r5...r;...r..
+00000940: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00000950: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000960: 1800 0000 0c00 0802 0801 0c01 0803 0a06  ................
+00000970: 2208 0203 0201 0cff 0c16 100c            "...........
```

### Comparing `mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-310.pyc` & `mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 10:14:14 2023 UTC, .py size: 1236 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,91 @@
-00000000: 6f0d 0d0a 0000 0000 76fb 8264 d404 0000  o.......v..d....
+00000000: 6f0d 0d0a 0000 0000 2f36 8c64 1a05 0000  o......./6.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c05 6d06 5a06 0100 6409  ..d.d.l.m.Z...d.
-00000050: 6404 6504 6a07 6405 6508 6406 6401 6606  d.e.j.d.e.d.d.f.
-00000060: 6407 6408 8405 5a09 6401 5300 290a e900  d.d...Z.d.S.)...
-00000070: 0000 004e 2901 da10 6d61 6368 696e 655f  ...N)...machine_
-00000080: 6461 7461 5f64 6566 2901 da08 696f 5f75  data_def)...io_u
-00000090: 7469 6c73 da02 6d64 da09 636f 6d70 6c65  tils..md..comple
-000000a0: 7665 6cda 0672 6574 7572 6e63 0300 0000  vel..returnc....
-000000b0: 0000 0000 0000 0000 0800 0000 0800 0000  ................
-000000c0: 0b00 0000 73f8 0000 0064 0188 0076 0172  ....s....d...v.r
-000000d0: 0864 0288 0064 013c 0074 00a0 017c 00a1  .d...d.<.t...|..
-000000e0: 0101 0074 00a0 027c 0064 03a1 027d 0074  ...t...|.d...}.t
-000000f0: 036a 047c 0064 0464 057c 0264 068d 048f  .j.|.d.d.|.d....
-00000100: 5689 0188 016a 0564 077c 016a 0666 0264  V....j.d.|.j.f.d
-00000110: 0874 076a 086a 0964 0964 0a9c 0388 00a4  .t.j.j.d.d......
-00000120: 018e 0101 0088 016a 0a64 0764 0b74 076a  .......j.d.d.t.j
-00000130: 086a 0b74 076a 086a 0c67 0364 0c64 0d8d  .j.t.j.j.g.d.d..
-00000140: 0301 0087 0087 0166 0264 0e64 0f84 087d  .......f.d.d...}
-00000150: 047c 016a 0da0 0ea1 0044 005d 0d5c 027d  .|.j.....D.].\.}
-00000160: 057d 067c 0464 107c 059b 009d 027c 066a  .}.|.d.|.....|.j
-00000170: 0f83 0201 0071 497c 016a 10a0 0ea1 0044  .....qI|.j.....D
-00000180: 005d 0d5c 027d 057d 077c 0464 117c 059b  .].\.}.}.|.d.|..
-00000190: 009d 027c 076a 0f83 0201 0071 5c57 0064  ...|.j.....q\W.d
-000001a0: 0004 0004 0083 0301 0064 0053 0031 0073  .........d.S.1.s
-000001b0: 7577 0101 0001 0001 0059 0001 0064 0053  uw.......Y...d.S
-000001c0: 0029 124e da06 666f 726d 6174 da01 747a  .).N..format..tz
-000001d0: 032e 6835 da01 77da 0562 6c6f 7363 2903  ..h5..w..blosc).
-000001e0: da04 6d6f 6465 da07 636f 6d70 6c69 6272  ..mode..complibr
-000001f0: 0500 0000 da06 6d61 7374 6572 5446 a903  ......masterTF..
-00000200: da05 696e 6465 78da 0c64 6174 615f 636f  ..index..data_co
-00000210: 6c75 6d6e 73da 0664 726f 706e 6172 0f00  lumns..dropnar..
-00000220: 0000 da04 6675 6c6c a902 da07 636f 6c75  ....full....colu
-00000230: 6d6e 73da 046b 696e 6463 0200 0000 0000  mns..kindc......
-00000240: 0000 0000 0000 0200 0000 0600 0000 1300  ................
-00000250: 0000 7342 0000 0088 016a 007c 007c 0166  ..sB.....j.|.|.f
-00000260: 0264 0174 016a 026a 0364 0264 039c 0388  .d.t.j.j.d.d....
-00000270: 00a4 018e 0101 0088 016a 047c 0064 0474  .........j.|.d.t
-00000280: 016a 026a 0574 016a 026a 0667 0364 0564  .j.j.t.j.j.g.d.d
-00000290: 068d 0301 0064 0053 0029 074e 5446 720e  .....d.S.).NTFr.
-000002a0: 0000 0072 0f00 0000 7212 0000 0072 1300  ...r....r....r..
-000002b0: 0000 2907 da03 7075 74da 036d 6464 da0a  ..)...put..mdd..
-000002c0: 4d44 436f 6e63 6570 7473 da0c 6261 7365  MDConcepts..base
-000002d0: 5f63 6f6c 756d 6e73 da12 6372 6561 7465  _columns..create
-000002e0: 5f74 6162 6c65 5f69 6e64 6578 da04 5469  _table_index..Ti
-000002f0: 6d65 da05 4c61 6265 6c29 02da 036b 6579  me..Label)...key
-00000300: da02 6466 a902 da06 6b77 6172 6773 da05  ..df....kwargs..
-00000310: 7374 6f72 65a9 00fa 4b43 3a5c 5573 6572  store...KC:\User
-00000320: 735c 4c65 6168 5c50 7963 6861 726d 5072  s\Leah\PycharmPr
-00000330: 6f6a 6563 7473 5c6d 6461 7461 5c73 7263  ojects\mdata\src
-00000340: 5c6d 6461 7461 5c66 696c 655f 666f 726d  \mdata\file_form
-00000350: 6174 735c 6864 665c 6578 706f 7274 696e  ats\hdf\exportin
-00000360: 672e 7079 da0a 7075 745f 7365 7269 6573  g.py..put_series
-00000370: 1100 0000 7308 0000 0018 0102 0106 ff22  ....s.........."
-00000380: 027a 2977 7269 7465 5f6d 6163 6869 6e65  .z)write_machine
-00000390: 5f64 6174 615f 6835 2e3c 6c6f 6361 6c73  _data_h5.<locals
-000003a0: 3e2e 7075 745f 7365 7269 6573 7a07 6576  >.put_seriesz.ev
-000003b0: 656e 7473 2f7a 0d6d 6561 7375 7265 6d65  ents/z.measureme
-000003c0: 6e74 732f 2911 7203 0000 00da 1765 6e73  nts/).r......ens
-000003d0: 7572 655f 6469 7265 6374 6f72 795f 6578  ure_directory_ex
-000003e0: 6973 7473 da0a 656e 7375 7265 5f65 7874  ists..ensure_ext
-000003f0: da02 7064 da08 4844 4653 746f 7265 7216  ..pd..HDFStorer.
-00000400: 0000 00da 0b69 6e64 6578 5f66 7261 6d65  .....index_frame
-00000410: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000420: 1a00 0000 721b 0000 0072 1c00 0000 da0c  ....r....r......
-00000430: 6576 656e 745f 7365 7269 6573 da05 6974  event_series..it
-00000440: 656d 7372 1e00 0000 da12 6d65 6173 7572  emsr......measur
-00000450: 656d 656e 745f 7365 7269 6573 2908 da08  ement_series)...
-00000460: 6669 6c65 6e61 6d65 7204 0000 0072 0500  filenamer....r..
-00000470: 0000 7220 0000 0072 2400 0000 da05 6c61  ..r ...r$.....la
-00000480: 6265 6cda 0365 7373 da03 6d73 7372 2200  bel..ess..mssr".
-00000490: 0000 721f 0000 0072 2300 0000 da15 7772  ..r....r#.....wr
-000004a0: 6974 655f 6d61 6368 696e 655f 6461 7461  ite_machine_data
-000004b0: 5f68 3507 0000 0073 2400 0000 0801 0801  _h5....s$.......
-000004c0: 0a01 0c01 1401 1401 0201 04ff 0201 06ff  ................
-000004d0: 1e02 0e02 1205 1401 1201 1401 02ff 22f4  ..............".
-000004e0: 7231 0000 0029 0172 0100 0000 290a da06  r1...).r....)...
-000004f0: 7061 6e64 6173 7227 0000 00da 0a6d 6461  pandasr'.....mda
-00000500: 7461 2e63 6f72 6572 0200 0000 7217 0000  ta.corer....r...
-00000510: 005a 126d 6461 7461 2e66 696c 655f 666f  .Z.mdata.file_fo
-00000520: 726d 6174 7372 0300 0000 da0b 4d61 6368  rmatsr......Mach
-00000530: 696e 6544 6174 61da 0369 6e74 7231 0000  ineData..intr1..
-00000540: 0072 2200 0000 7222 0000 0072 2200 0000  .r"...r"...r"...
-00000550: 7223 0000 00da 083c 6d6f 6475 6c65 3e01  r#.....<module>.
-00000560: 0000 0073 0800 0000 0800 0c02 0c01 1e03  ...s............
+00000020: 0007 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c03 6d04 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
+00000050: 6d07 5a07 0100 6409 6404 6505 6a08 6405  m.Z...d.d.e.j.d.
+00000060: 6509 6406 6401 6606 6407 6408 8405 5a0a  e.d.d.f.d.d...Z.
+00000070: 6401 5300 290a e900 0000 004e 2901 da10  d.S.)......N)...
+00000080: 6d61 6368 696e 655f 6461 7461 5f64 6566  machine_data_def
+00000090: 2901 da08 696f 5f75 7469 6c73 da02 6d64  )...io_utils..md
+000000a0: da09 636f 6d70 6c65 7665 6cda 0672 6574  ..complevel..ret
+000000b0: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
+000000c0: 0800 0000 0800 0000 0b00 0000 7308 0100  ............s...
+000000d0: 0064 0188 0076 0172 0864 0288 0064 013c  .d...v.r.d...d.<
+000000e0: 0074 007c 0074 0174 026a 0342 0083 0272  .t.|.t.t.j.B...r
+000000f0: 1b74 04a0 057c 00a1 0101 0074 04a0 067c  .t...|.....t...|
+00000100: 0064 03a1 027d 0074 076a 087c 0064 0464  .d...}.t.j.|.d.d
+00000110: 057c 0264 068d 048f 5689 0188 016a 0964  .|.d....V....j.d
+00000120: 077c 016a 0a66 0264 0874 0b6a 0c6a 0d64  .|.j.f.d.t.j.j.d
+00000130: 0964 0a9c 0388 00a4 018e 0101 0088 016a  .d.............j
+00000140: 0e64 0764 0b74 0b6a 0c6a 0f74 0b6a 0c6a  .d.d.t.j.j.t.j.j
+00000150: 1067 0364 0c64 0d8d 0301 0087 0087 0166  .g.d.d.........f
+00000160: 0264 0e64 0f84 087d 047c 016a 11a0 12a1  .d.d...}.|.j....
+00000170: 0044 005d 0d5c 027d 057d 067c 0464 107c  .D.].\.}.}.|.d.|
+00000180: 059b 009d 027c 066a 1383 0201 0071 517c  .....|.j.....qQ|
+00000190: 016a 14a0 12a1 0044 005d 0d5c 027d 057d  .j.....D.].\.}.}
+000001a0: 077c 0464 117c 059b 009d 027c 076a 1383  .|.d.|.....|.j..
+000001b0: 0201 0071 6457 0064 0004 0004 0083 0301  ...qdW.d........
+000001c0: 0064 0053 0031 0073 7d77 0101 0001 0001  .d.S.1.s}w......
+000001d0: 0059 0001 0064 0053 0029 124e da06 666f  .Y...d.S.).N..fo
+000001e0: 726d 6174 da01 747a 032e 6835 da01 77da  rmat..tz..h5..w.
+000001f0: 0562 6c6f 7363 2903 da04 6d6f 6465 da07  .blosc)...mode..
+00000200: 636f 6d70 6c69 6272 0500 0000 da06 6d61  complibr......ma
+00000210: 7374 6572 5446 a903 da05 696e 6465 78da  sterTF....index.
+00000220: 0c64 6174 615f 636f 6c75 6d6e 73da 0664  .data_columns..d
+00000230: 726f 706e 6172 0f00 0000 da04 6675 6c6c  ropnar......full
+00000240: a902 da07 636f 6c75 6d6e 73da 046b 696e  ....columns..kin
+00000250: 6463 0200 0000 0000 0000 0000 0000 0200  dc..............
+00000260: 0000 0600 0000 1300 0000 7342 0000 0088  ..........sB....
+00000270: 016a 007c 007c 0166 0264 0174 016a 026a  .j.|.|.f.d.t.j.j
+00000280: 0364 0264 039c 0388 00a4 018e 0101 0088  .d.d............
+00000290: 016a 047c 0064 0474 016a 026a 0574 016a  .j.|.d.t.j.j.t.j
+000002a0: 026a 0667 0364 0564 068d 0301 0064 0053  .j.g.d.d.....d.S
+000002b0: 0029 074e 5446 720e 0000 0072 0f00 0000  .).NTFr....r....
+000002c0: 7212 0000 0072 1300 0000 2907 da03 7075  r....r....)...pu
+000002d0: 74da 036d 6464 da0a 4d44 436f 6e63 6570  t..mdd..MDConcep
+000002e0: 7473 da0c 6261 7365 5f63 6f6c 756d 6e73  ts..base_columns
+000002f0: da12 6372 6561 7465 5f74 6162 6c65 5f69  ..create_table_i
+00000300: 6e64 6578 da04 5469 6d65 da05 4c61 6265  ndex..Time..Labe
+00000310: 6c29 02da 036b 6579 da02 6466 a902 da06  l)...key..df....
+00000320: 6b77 6172 6773 da05 7374 6f72 65a9 00fa  kwargs..store...
+00000330: 4b43 3a5c 5573 6572 735c 4c65 6168 5c50  KC:\Users\Leah\P
+00000340: 7963 6861 726d 5072 6f6a 6563 7473 5c6d  ycharmProjects\m
+00000350: 6461 7461 5c73 7263 5c6d 6461 7461 5c66  data\src\mdata\f
+00000360: 696c 655f 666f 726d 6174 735c 6864 665c  ile_formats\hdf\
+00000370: 6578 706f 7274 696e 672e 7079 da0a 7075  exporting.py..pu
+00000380: 745f 7365 7269 6573 1400 0000 7308 0000  t_series....s...
+00000390: 0018 0102 0106 ff22 027a 2977 7269 7465  .......".z)write
+000003a0: 5f6d 6163 6869 6e65 5f64 6174 615f 6835  _machine_data_h5
+000003b0: 2e3c 6c6f 6361 6c73 3e2e 7075 745f 7365  .<locals>.put_se
+000003c0: 7269 6573 7a07 6576 656e 7473 2f7a 0d6d  riesz.events/z.m
+000003d0: 6561 7375 7265 6d65 6e74 732f 2915 da0a  easurements/)...
+000003e0: 6973 696e 7374 616e 6365 da03 7374 72da  isinstance..str.
+000003f0: 026f 73da 0850 6174 684c 696b 6572 0300  .os..PathLiker..
+00000400: 0000 da17 656e 7375 7265 5f64 6972 6563  ....ensure_direc
+00000410: 746f 7279 5f65 7869 7374 73da 0a65 6e73  tory_exists..ens
+00000420: 7572 655f 6578 74da 0270 64da 0848 4446  ure_ext..pd..HDF
+00000430: 5374 6f72 6572 1600 0000 da0b 696e 6465  Storer......inde
+00000440: 785f 6672 616d 6572 1700 0000 7218 0000  x_framer....r...
+00000450: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000460: 721c 0000 00da 0c65 7665 6e74 5f73 6572  r......event_ser
+00000470: 6965 73da 0569 7465 6d73 721e 0000 00da  ies..itemsr.....
+00000480: 126d 6561 7375 7265 6d65 6e74 5f73 6572  .measurement_ser
+00000490: 6965 7329 08da 0866 696c 656e 616d 6572  ies)...filenamer
+000004a0: 0400 0000 7205 0000 0072 2000 0000 7224  ....r....r ...r$
+000004b0: 0000 00da 056c 6162 656c 5a03 6573 735a  .....labelZ.essZ
+000004c0: 036d 7373 7222 0000 0072 1f00 0000 7223  .mssr"...r....r#
+000004d0: 0000 00da 1577 7269 7465 5f6d 6163 6869  .....write_machi
+000004e0: 6e65 5f64 6174 615f 6835 0900 0000 7326  ne_data_h5....s&
+000004f0: 0000 0008 0108 0110 010a 010c 0114 0114  ................
+00000500: 0102 0104 ff02 0106 ff1e 020e 0212 0514  ................
+00000510: 0112 0114 0102 ff22 f472 3300 0000 2901  .......".r3...).
+00000520: 7201 0000 0029 0b72 2700 0000 da06 7061  r....).r'.....pa
+00000530: 6e64 6173 722b 0000 00da 0a6d 6461 7461  ndasr+.....mdata
+00000540: 2e63 6f72 6572 0200 0000 7217 0000 005a  .corer....r....Z
+00000550: 126d 6461 7461 2e66 696c 655f 666f 726d  .mdata.file_form
+00000560: 6174 7372 0300 0000 da0b 4d61 6368 696e  atsr......Machin
+00000570: 6544 6174 61da 0369 6e74 7233 0000 0072  eData..intr3...r
+00000580: 2200 0000 7222 0000 0072 2200 0000 7223  "...r"...r"...r#
+00000590: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000005a0: 0073 0a00 0000 0800 0802 0c02 0c01 1e03  .s..............
```

### Comparing `mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/importing.cpython-310.pyc` & `mdata-0.1.2/src/mdata/file_formats/hdf/__pycache__/importing.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 07:45:07 2023 UTC, .py size: 1303 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 83d8 8264 1705 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 2f36 8c64 1905 0000  o......./6.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6504 6a05 6602 6404 6405 8404  ..d.e.j.f.d.d...
 00000050: 5a06 6401 5300 2906 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da10 6d61 6368 696e 655f 6461 7461 5f64  ..machine_data_d
 00000070: 6566 da06 7265 7475 726e 6301 0000 0000  ef..returnc.....
@@ -52,15 +52,15 @@
 00000330: 6d74 73a9 0072 2300 0000 fa4b 433a 5c55  mts..r#....KC:\U
 00000340: 7365 7273 5c4c 6561 685c 5079 6368 6172  sers\Leah\Pychar
 00000350: 6d50 726f 6a65 6374 735c 6d64 6174 615c  mProjects\mdata\
 00000360: 7372 635c 6d64 6174 615c 6669 6c65 5f66  src\mdata\file_f
 00000370: 6f72 6d61 7473 5c68 6466 5c69 6d70 6f72  ormats\hdf\impor
 00000380: 7469 6e67 2e70 79da 1472 6561 645f 6d61  ting.py..read_ma
 00000390: 6368 696e 655f 6461 7461 5f68 3506 0000  chine_data_h5...
-000003a0: 0073 3000 0000 1002 0a01 1201 0801 1401  .s0.............
+000003a0: 0073 3000 0000 1003 0a01 1201 0801 1401  .s0.............
 000003b0: 0801 0e01 0a01 0401 1201 0201 04fe 0c03  ................
 000003c0: 0801 1401 0801 0e01 0a01 0401 1401 04ff  ................
 000003d0: 0c02 1201 24ec 7225 0000 0029 07da 0670  ....$.r%...)...p
 000003e0: 616e 6461 7372 0a00 0000 da0a 6d64 6174  andasr......mdat
 000003f0: 612e 636f 7265 7202 0000 0072 1000 0000  a.corer....r....
 00000400: 7218 0000 0072 2500 0000 7223 0000 0072  r....r%...r#...r
 00000410: 2300 0000 7223 0000 0072 2400 0000 da08  #...r#...r$.....
```

### Comparing `mdata-0.1.1/src/mdata/file_formats/hdf/exporting.py` & `mdata-0.1.2/src/mdata/file_formats/hdf/exporting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,48 @@
+import os
+
 import pandas as pd
 
 from mdata.core import machine_data_def as mdd
+from mdata.core.extensions import registry
 from mdata.file_formats import io_utils
 
 
 def write_machine_data_h5(filename, md: mdd.MachineData, complevel: int = 0, **kwargs) -> None:
     if 'format' not in kwargs:
         kwargs['format'] = 't'
-    io_utils.ensure_directory_exists(filename)
-    filename = io_utils.ensure_ext(filename, '.h5')
+    if isinstance(filename, str | os.PathLike):
+        io_utils.ensure_directory_exists(filename)
+        filename = io_utils.ensure_ext(filename, '.h5')
     with pd.HDFStore(filename, mode='w', complib='blosc', complevel=complevel) as store:
-        store.put('master', md.index_frame, index=True, data_columns=mdd.MDConcepts.base_columns,
+        store.put('index', md.index_frame, index=True, data_columns=mdd.MDConcepts.base_columns,
                   dropna=False, **kwargs)
-        store.create_table_index('master', columns=['index', mdd.MDConcepts.Time, mdd.MDConcepts.Label], kind='full')
+        store.create_table_index('index', columns=['index', mdd.MDConcepts.Time, mdd.MDConcepts.Label], kind='full')
 
         def put_series(key, df):
             store.put(key, df, index=True, data_columns=mdd.MDConcepts.base_columns, dropna=False,
                       **kwargs)
             store.create_table_index(key, columns=['index', mdd.MDConcepts.Time, mdd.MDConcepts.Label], kind='full')
 
         for label, ess in md.event_series.items():
             put_series(f'events/{label}', ess.df)
         for label, mss in md.measurement_series.items():
             put_series(f'measurements/{label}', mss.df)
+
+        if len(md.meta.extensions) > 0:
+            store.put('meta/extensions', list(md.meta.extensions), format='table', index=False)
+        if registry.Extension.Metadata in md.meta.extensions:
+            keys, values = map(list, zip(*((k, v) for k, v in md.meta.metadata.items())))
+            metadata_df = pd.DataFrame(data=values, index=pd.Index(keys, name='key'), columns=['value'])
+            store.put('meta/metadata', metadata_df)
+
+            specmeta = []
+            for tsc in md.series_containers:
+                tt = tsc.timeseries_spec
+                t, l = tt.identifier
+                for fspec in tt.base.features:
+                    row = [t, l, fspec.name, fspec.print_name if fspec.name != fspec.print_name else [],
+                           fspec.data_type if fspec.data_type is not None else []]
+                specmeta.append(row)
+            store.put('meta/specs', pd.DataFrame(specmeta,
+                                                 columns=[mdd.MDConcepts.Type, mdd.MDConcepts.Label, 'feature',
+                                                          'print_name', 'data_type']))
```

### Comparing `mdata-0.1.1/src/mdata/file_formats/io_utils.py` & `mdata-0.1.2/src/mdata/file_formats/io_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,50 +15,75 @@
     p, e = os.path.splitext(path)
     if e is None or e == '' or (override_ext and (e != desired_ext)):
         return path + desired_ext
     else:
         return path
 
 
-def create_string_io(arg: str | os.PathLike[str] | bytes | io.BytesIO | io.StringIO, expected_file='.json',
+DataSource = str | os.PathLike[str] | bytes | memoryview | io.BytesIO | io.StringIO
+
+
+def create_string_io(arg: DataSource, expected_file='.json',
                      encoding='utf-8') -> tuple[
     io.StringIO, bool]:
     source = arg
     locally_opened = False
+    if isinstance(arg, memoryview):
+        arg = arg.tobytes()
+
     if isinstance(arg, bytes):
         source = io.TextIOWrapper(io.BytesIO(arg), encoding=encoding, newline='')
         locally_opened = True
     elif isinstance(arg, str | os.PathLike):
         arg = ensure_ext(arg, desired_ext=expected_file, override_ext=False)
         source = open(arg, 'r', newline='', encoding=encoding)
         locally_opened = True
     elif isinstance(arg, io.StringIO):
         source = arg
     elif isinstance(arg, io.BytesIO):
         source = io.TextIOWrapper(arg, encoding=encoding, newline='')
     return source, locally_opened
 
 
-def read_csv_lines_from(arg: str | os.PathLike[str] | bytes | io.BytesIO | io.StringIO, encoding='utf-8') -> Optional[
+def read_csv_lines_from(arg: DataSource, encoding='utf-8') -> Optional[
     list[list[str]]]:
     source, locally_opened = create_string_io(arg, expected_file='.csv', encoding=encoding)
     import csv
     try:
         reader = csv.reader(source, dialect='excel')
         return [r for r in reader]
     finally:
         if locally_opened:
             source.close()
 
 
-def read_json_dict_from(arg: str | os.PathLike[str] | bytes | io.BytesIO | io.StringIO, encoding='utf-8') -> Optional[
-    dict]:
+def read_yaml_dict_from(arg: DataSource, encoding='utf-8', swallow_exceptions=True) -> Optional[dict]:
+    source, locally_opened = create_string_io(arg, expected_file='.yml', encoding=encoding)
+    from yaml import YAMLError
+    import yaml
+    try:
+        import json
+        return yaml.load(source, yaml.FullLoader)
+    except YAMLError as e:
+        if swallow_exceptions:
+            return None
+        else:
+            raise e
+    finally:
+        if locally_opened:
+            source.close()
+
+
+def read_json_dict_from(arg: DataSource, encoding='utf-8', swallow_exceptions=True) -> Optional[dict]:
     source, locally_opened = create_string_io(arg, expected_file='.json', encoding=encoding)
     from json import JSONDecodeError
     try:
         import json
         return json.load(source)
-    except JSONDecodeError:
-        return None
+    except JSONDecodeError as e:
+        if swallow_exceptions:
+            return None
+        else:
+            raise e
     finally:
         if locally_opened:
             source.close()
```

### Comparing `mdata-0.1.1/src/mdata/visualization/__pycache__/matplot.cpython-310.pyc` & `mdata-0.1.2/src/mdata/visualization/__pycache__/matplot.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 12:18:22 2023 UTC, .py size: 1102 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0e24 7f64 4e04 0000  o........$.dN...
+00000000: 6f0d 0d0a 0000 0000 11ee 8664 4e04 0000  o..........dN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6402 6c07 5a08 6400 6403 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
 00000060: 0100 640a 6404 650a 6a0b 6405 650c 6406  ..d.d.e.j.d.e.d.
 00000070: 650d 650c 1900 6407 650e 650c 1900 6608  e.e...d.e.e...f.
@@ -58,30 +58,30 @@
 00000390: 0179 da02 6178 2910 da12 6d65 6173 7572  .y..ax)...measur
 000003a0: 656d 656e 745f 7365 7269 6573 da04 6c69  ement_series..li
 000003b0: 7374 da0a 6f62 6a65 6374 5f6d 6170 da04  st..object_map..
 000003c0: 6b65 7973 da03 7365 7472 1000 0000 7209  keys..setr....r.
 000003d0: 0000 00da 0370 6c74 da08 7375 6270 6c6f  .....plt..subplo
 000003e0: 7473 da03 6c65 6eda 0965 6e75 6d65 7261  ts..len..enumera
 000003f0: 7465 da04 7669 6577 da03 736e 735a 086c  te..view..snsZ.l
-00000400: 696e 6570 6c6f 74da 0264 665a 0c74 6967  ineplot..dfZ.tig
+00000400: 696e 6570 6c6f 74da 0264 66da 0c74 6967  ineplot..df..tig
 00000410: 6874 5f6c 6179 6f75 7429 0c72 0600 0000  ht_layout).r....
 00000420: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00000430: 1500 0000 da02 6673 da03 6669 675a 0361  ......fs..figZ.a
+00000430: 1500 0000 da02 6673 da03 6669 67da 0361  ......fs..fig..a
 00000440: 7873 da01 6972 1100 0000 720c 0000 00da  xs..ir....r.....
 00000450: 0274 7372 0a00 0000 2902 720d 0000 0072  .tsr....).r....r
 00000460: 1200 0000 720e 0000 00da 1d63 7265 6174  ....r......creat
 00000470: 655f 6261 7369 635f 7374 6163 6b65 645f  e_basic_stacked_
 00000480: 7375 6270 6c6f 7473 0800 0000 7326 0000  subplots....s&..
 00000490: 000a 0104 0104 0108 0110 0116 0214 0108  ................
 000004a0: 010e 0118 0212 011a 0210 0208 010a 011a  ................
-000004b0: 0102 fe08 0504 0172 2b00 0000 2903 4e4e  .......r+...).NN
+000004b0: 0102 fe08 0504 0172 2d00 0000 2903 4e4e  .......r-...).NN
 000004c0: 4e29 10da 0674 7970 696e 6772 0200 0000  N)...typingr....
 000004d0: 7203 0000 0072 0400 0000 da11 6d61 7470  r....r......matp
 000004e0: 6c6f 746c 6962 2e70 7970 6c6f 74da 0670  lotlib.pyplot..p
-000004f0: 7970 6c6f 7472 2000 0000 5a07 7365 6162  yplotr ...Z.seab
+000004f0: 7970 6c6f 7472 2000 0000 da07 7365 6162  yplotr .....seab
 00000500: 6f72 6e72 2500 0000 da0a 6d64 6174 612e  ornr%.....mdata.
 00000510: 636f 7265 7205 0000 00da 0b4d 6163 6869  corer......Machi
 00000520: 6e65 4461 7461 da03 7374 7272 1f00 0000  neData..strr....
-00000530: 721c 0000 0072 2b00 0000 720a 0000 0072  r....r+...r....r
+00000530: 721c 0000 0072 2d00 0000 720a 0000 0072  r....r-...r....r
 00000540: 0a00 0000 720a 0000 0072 0e00 0000 da08  ....r....r......
 00000550: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
 00000560: 0014 000c 0208 010c 022a 02              .........*.
```

### Comparing `mdata-0.1.1/src/mdata/visualization/__pycache__/plotting.cpython-310.pyc` & `mdata-0.1.2/src/mdata/visualization/__pycache__/plotting.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 10:23:11 2023 UTC, .py size: 7737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8ffd 8264 391e 0000  o..........d9...
+00000000: 6f0d 0d0a 0000 0000 8aa8 9164 411e 0000  o..........dA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6400 6403 6c07 5a08 6400 6403 6c09  Z.d.d.l.Z.d.d.l.
 00000060: 5a09 6400 6403 6c0a 6d0b 5a0c 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6404 6c0d 6d0e 5a0e 0100 6400 6405 6c0f  d.l.m.Z...d.d.l.
@@ -136,40 +136,40 @@
 00000870: 6f77 da03 636f 6c72 2e00 0000 fa10 7267  ow..colr......rg
 00000880: 6261 2830 2c20 302c 2030 2c20 3029 da04  ba(0, 0, 0, 0)..
 00000890: 6e6f 6e65 a909 7232 0000 0072 3300 0000  none..r2...r3...
 000008a0: 7236 0000 0072 3400 0000 7230 0000 00da  r6...r4...r0....
 000008b0: 046c 696e 6572 3700 0000 7238 0000 00da  .liner7...r8....
 000008c0: 0968 6f76 6572 696e 666f 7a13 6361 7465  .hoverinfoz.cate
 000008d0: 676f 7279 2064 6573 6365 6e64 696e 67da  gory descending.
-000008e0: 046c 6566 7429 02da 0d63 6174 6567 6f72  .left)...categor
-000008f0: 796f 7264 6572 da04 7369 6465 da06 4576  yorder..side..Ev
+000008e0: 046c 6566 7429 025a 0d63 6174 6567 6f72  .left).Z.categor
+000008f0: 796f 7264 6572 da04 7369 6465 5a06 4576  yorder..sideZ.Ev
 00000900: 656e 7473 da08 6361 7465 676f 7279 2905  ents..category).
 00000910: da0a 7469 746c 655f 7465 7874 da07 7669  ..title_text..vi
 00000920: 7369 626c 65da 0474 7970 6572 3a00 0000  sible..typer:...
-00000930: 723b 0000 00da 0c4d 6561 7375 7265 6d65  r;.....Measureme
+00000930: 723b 0000 005a 0c4d 6561 7375 7265 6d65  r;...Z.Measureme
 00000940: 6e74 73da 084f 7665 7276 6965 77fa 153c  nts..Overview..<
 00000950: 6272 3e3c 7375 703e 2873 616d 706c 6564  br><sup>(sampled
 00000960: 2074 6f20 7a1e 2064 6174 6120 706f 696e   to z. data poin
 00000970: 7473 2070 6572 2073 6572 6965 7329 3c2f  ts per series)</
 00000980: 7375 703e da06 6365 6e74 6572 e918 0000  sup>..center....
 00000990: 0029 04da 0474 6578 74da 0778 616e 6368  .)...text..xanch
 000009a0: 6f72 7232 0000 00da 0966 6f6e 745f 7369  orr2.....font_si
 000009b0: 7a65 da07 4f62 6a65 6374 7367 3333 3333  ze..Objectsg3333
-000009c0: 3333 f33f da01 6829 0472 4600 0000 7232  33.?..h).rF...r2
+000009c0: 3333 f33f da01 6829 0472 4400 0000 7232  33.?..h).rD...r2
 000009d0: 0000 0072 3300 0000 da0b 6f72 6965 6e74  ...r3.....orient
 000009e0: 6174 696f 6e29 02da 0574 6974 6c65 da06  ation)...title..
 000009f0: 6c65 6765 6e64 2927 7205 0000 00da 0670  legend)'r......p
 00000a00: 6c6f 746c 79da 0663 6f6c 6f72 73da 0b71  lotly..colors..q
 00000a10: 7561 6c69 7461 7469 7665 da06 506c 6f74  ualitative..Plot
 00000a20: 6c79 da11 6f63 6375 7272 696e 675f 6f62  ly..occurring_ob
 00000a30: 6a65 6374 73da 037a 6970 7202 0000 00da  jects..zipr.....
 00000a40: 1369 7465 725f 616c 6c5f 7469 6d65 7365  .iter_all_timese
 00000a50: 7269 6573 da0f 7469 6d65 7365 7269 6573  ries..timeseries
-00000a60: 5f74 7970 6572 4800 0000 da03 6d64 64da  _typerH.....mdd.
-00000a70: 104d 6163 6869 6e65 4461 7461 5479 7065  .MachineDataType
+00000a60: 5f74 7970 6572 4600 0000 da03 6d64 64da  _typerF.....mdd.
+00000a70: 104f 6273 6572 7661 7469 6f6e 5479 7065  .ObservationType
 00000a80: 73da 0145 da08 6665 6174 7572 6573 da02  s..E..features..
 00000a90: 6466 da07 6772 6f75 7062 79da 0a4d 4443  df..groupby..MDC
 00000aa0: 6f6e 6365 7074 73da 064f 626a 6563 74da  oncepts..Object.
 00000ab0: 0667 726f 7570 73da 0569 7465 6d73 da03  .groups..items..
 00000ac0: 6c6f 6372 1f00 0000 da03 6d61 78da 0369  locr......max..i
 00000ad0: 6e74 7220 0000 00da 0661 7261 6e67 65da  ntr .....arange.
 00000ae0: 0469 6c6f 63da 0454 696d 65da 054c 6162  .iloc..Time..Lab
@@ -177,240 +177,241 @@
 00000b00: 6561 7475 7265 5f63 6f6c 756d 6e73 da02  eature_columns..
 00000b10: 676f da09 5363 6174 7465 7267 6cda 0753  go..Scattergl..S
 00000b20: 6361 7474 6572 da04 6469 6374 da05 6c61  catter..dict..la
 00000b30: 6265 6cda 0961 6464 5f74 7261 6365 da0c  bel..add_trace..
 00000b40: 7570 6461 7465 5f79 6178 6573 da0d 7570  update_yaxes..up
 00000b50: 6461 7465 5f6c 6179 6f75 7429 1f72 0b00  date_layout).r..
 00000b60: 0000 da0d 646f 776e 7361 6d70 6c65 5f74  ....downsample_t
-00000b70: 6fda 0675 7365 5f67 6cda 0366 6967 721c  o..use_gl..figr.
-00000b80: 0000 0072 2600 0000 da0e 6469 645f 646f  ...r&.....did_do
+00000b70: 6f5a 0675 7365 5f67 6cda 0366 6967 721c  oZ.use_gl..figr.
+00000b80: 0000 0072 2600 0000 5a0e 6469 645f 646f  ...r&...Z.did_do
 00000b90: 776e 7361 6d70 6c65 7223 0000 00da 046f  wnsampler#.....o
 00000ba0: 626a 73da 0a63 6f6c 6f72 5f64 6963 74da  bjs..color_dict.
-00000bb0: 0374 7363 725d 0000 00da 0374 7970 723a  .tscr].....typr:
-00000bc0: 0000 0072 1b00 0000 da01 67da 0467 6964  ...r......g..gid
-00000bd0: 78da 036f 626a 7262 0000 0072 2a00 0000  x..objrb...r*...
+00000bb0: 0374 7363 725a 0000 00da 0374 7970 723a  .tscrZ.....typr:
+00000bc0: 0000 0072 1b00 0000 da01 675a 0467 6964  ...r......gZ.gid
+00000bd0: 78da 036f 626a 725f 0000 0072 2a00 0000  x..objr_...r*...
 00000be0: da06 6c65 6e67 7468 da04 7374 6570 da03  ..length..step..
-00000bf0: 6964 7872 3200 0000 7233 0000 00da 0466  idxr2...r3.....f
+00000bf0: 6964 7872 3200 0000 7233 0000 005a 0466  idxr2...r3...Z.f
 00000c00: 5f64 66da 0363 6c73 7236 0000 00da 016e  _df..clsr6.....n
-00000c10: 7229 0000 0072 4600 0000 7213 0000 0072  r)...rF...r....r
+00000c10: 7229 0000 0072 4400 0000 7213 0000 0072  r)...rD...r....r
 00000c20: 1300 0000 7217 0000 00da 1463 7265 6174  ....r......creat
 00000c30: 655f 6f76 6572 7669 6577 5f70 6c6f 740e  e_overview_plot.
 00000c40: 0000 0073 6c00 0000 0801 0201 06ff 0803  ...sl...........
 00000c50: 1205 0405 0a01 0601 1801 0c02 0601 0601  ................
 00000c60: 1401 0601 1e01 0401 0c01 0801 0802 0c01  ................
 00000c70: 0c01 1601 0e01 0a01 0401 1a02 0a01 1001  ................
 00000c80: 0a01 1801 0c01 0a01 0201 06fe 1203 02eb  ................
 00000c90: 0817 0402 1c01 0c01 04ff 0201 0201 08fd  ................
 00000ca0: 0e05 1401 1401 0404 0601 1001 1201 0e01  ................
-00000cb0: 06ff 0404 7289 0000 0063 0000 0000 0000  ....r....c......
+00000cb0: 06ff 0404 7282 0000 0063 0000 0000 0000  ....r....c......
 00000cc0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
 00000cd0: 0000 733e 0000 0065 005a 0164 005a 0255  ..s>...e.Z.d.Z.U
 00000ce0: 0065 0365 0464 013c 0065 0365 0464 023c  .e.e.d.<.e.e.d.<
 00000cf0: 0065 0565 0319 0065 0642 0065 0464 033c  .e.e...e.B.e.d.<
 00000d00: 0065 0765 0319 0065 0642 0065 0464 043c  .e.e...e.B.e.d.<
 00000d10: 0064 0553 0029 06da 0953 656c 6563 7469  .d.S.)...Selecti
-00000d20: 6f6e da06 6f62 6a65 6374 da0b 6d65 6173  on..object..meas
-00000d30: 7572 656d 656e 7472 6100 0000 da06 6576  urementra.....ev
+00000d20: 6f6e da06 6f62 6a65 6374 5a0b 6d65 6173  on..objectZ.meas
+00000d30: 7572 656d 656e 7472 5e00 0000 da06 6576  urementr^.....ev
 00000d40: 656e 7473 4e29 08da 085f 5f6e 616d 655f  entsN)...__name_
 00000d50: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000d60: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 00000d70: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000d80: 5fda 046c 6973 74da 0462 6f6f 6cda 0373  _..list..bool..s
 00000d90: 6574 7213 0000 0072 1300 0000 7213 0000  etr....r....r...
-00000da0: 0072 1700 0000 728a 0000 0054 0000 0073  .r....r....T...s
-00000db0: 0a00 0000 0a00 0801 0801 1001 1401 728a  ..............r.
+00000da0: 0072 1700 0000 7283 0000 0054 0000 0073  .r....r....T...s
+00000db0: 0a00 0000 0a00 0801 0801 1001 1401 7283  ..............r.
 00000dc0: 0000 00e9 983a 0000 46da 106d 6561 7375  .....:..F..measu
-00000dd0: 7265 6d65 6e74 5f74 7970 6572 8b00 0000  rement_typer....
-00000de0: 7261 0000 0072 8d00 0000 6307 0000 0000  ra...r....c.....
+00000dd0: 7265 6d65 6e74 5f74 7970 6572 8400 0000  rement_typer....
+00000de0: 725e 0000 0072 8500 0000 6307 0000 0000  r^...r....c.....
 00000df0: 0000 0000 0000 001a 0000 000c 0000 0043  ...............C
-00000e00: 0000 0073 3a02 0000 7400 7401 7c04 7c00  ...s:...t.t.|.|.
+00000e00: 0000 0073 4002 0000 7400 7401 7c04 7c00  ...s@...t.t.|.|.
 00000e10: 6a02 a003 a100 6401 8d03 7d04 7c00 6a04  j.....d...}.|.j.
 00000e20: 7c01 1900 7d07 7400 7405 7c03 7c07 6a06  |...}.t.t.|.|.j.
 00000e30: 6a07 6401 8d03 7d03 7408 7c03 8301 7408  j.d...}.t.|...t.
 00000e40: 7c07 6a06 6a07 8301 6b01 7324 4a00 8201  |.j.j...k.s$J...
 00000e50: 7c07 6a09 7d08 6400 7d09 740a 7c08 8301  |.j.}.d.}.t.|...
 00000e60: 7d0a 7c0a 7c05 6b04 723a 6402 6403 6c0b  }.|.|.k.r:d.d.l.
 00000e70: 6d0c 7d0b 0100 7c0b 8300 7d09 7c08 6a0d  m.}...|...}.|.j.
 00000e80: 7c08 740e 6a0f 6a10 1900 7c02 6b02 740e  |.t.j.j...|.k.t.
 00000e90: 6a0f 6a11 6701 7c03 1700 6602 1900 7d08  j.j.g.|...f...}.
-00000ea0: 7c06 725d 740a 7c03 8301 7d0c 6404 7c0c  |.r]t.|...}.d.|.
-00000eb0: 1b00 6701 7c0c 1400 6405 6701 1700 7d0d  ..g.|...d.g...}.
-00000ec0: 6e04 6404 6405 6702 7d0d 7412 740a 7c0d  n.d.d.g.}.t.t.|.
-00000ed0: 8301 6406 7c0d 6407 6408 6409 8d05 7d0e  ..d.|.d.d.d...}.
-00000ee0: 7413 7c03 6406 640a 8d02 4400 5d4c 5c02  t.|.d.d...D.]L\.
-00000ef0: 7d0f 7d10 7c08 740e 6a0f 6a11 1900 7c08  }.}.|.t.j.j...|.
-00000f00: 7c10 1900 0202 7d11 7d12 7c12 a014 a100  |.....}.}.|.....
-00000f10: 0f00 7d13 7c11 7c13 1900 7c12 7c13 1900  ..}.|.|...|.|...
-00000f20: 0202 7d11 7d12 7c09 6400 7501 72a9 7c11  ..}.}.|.d.u.r.|.
-00000f30: 6a15 7d11 7c12 6a15 7d12 7c09 6a16 7c11  j.}.|.j.}.|.j.|.
-00000f40: 7c12 7c05 640b 8d03 7d14 7c11 7c14 1900  |.|.d...}.|.|...
-00000f50: 7d11 7c12 7c14 1900 7d12 7c06 72ad 7c0f  }.|.|...}.|.r.|.
-00000f60: 6e01 6406 7d15 7c0e 6a17 7418 6a19 7c10  n.d.}.|.j.t.j.|.
-00000f70: 7c11 7c12 640c 640d 8d04 7c15 6406 640e  |.|.d.d...|.d.d.
-00000f80: 8d03 0100 7172 740a 7c0d 8301 7d16 7c04  ....qrt.|...}.|.
-00000f90: 4400 5d2e 7d17 7c00 6a1a 7c17 1900 6a09  D.].}.|.j.|...j.
-00000fa0: 7d18 7c18 6a0d 7c18 6a1b 7c02 6b02 1900  }.|.j.|.j.|.k...
-00000fb0: 7d18 7c18 740e 6a0f 6a11 1900 7d11 7c0e  }.|.t.j.j...}.|.
-00000fc0: 6a17 7418 6a1c 7c17 7c11 741d a01e 7c11  j.t.j.|.|.t...|.
-00000fd0: a101 640f 741f 6410 6411 6412 6413 8d03  ..d.t.d.d.d.d...
-00000fe0: 6414 8d05 7c16 6406 640e 8d03 0100 71c5  d...|.d.d.....q.
-00000ff0: 7c0e 6a20 7c16 6406 6415 6416 8d03 0100  |.j |.d.d.d.....
-00001000: 6417 7d19 7c09 6400 7501 9001 720e 7c19  d.}.|.d.u...r.|.
-00001010: 6418 7c05 9b00 6419 7c0a 9b00 641a 9d05  d.|...d.|...d...
-00001020: 3700 7d19 7c0e 6a21 7c19 6407 741f 6402  7.}.|.j!|.d.t.d.
-00001030: 641b 641c 641d 8d03 641e 8d03 0100 7c0e  d.d.d...d.....|.
-00001040: 5300 291f 4e29 01da 0769 665f 7472 7565  S.).N)...if_true
-00001050: 7201 0000 0029 01da 154d 696e 4d61 784c  r....)...MinMaxL
-00001060: 5454 4244 6f77 6e73 616d 706c 6572 67cd  TTBDownsamplerg.
-00001070: cccc cccc ccec 3f72 0e00 0000 720d 0000  ......?r....r...
-00001080: 0054 679a 9999 9999 99a9 3f29 0572 0f00  .Tg.......?).r..
-00001090: 0000 7210 0000 00da 0b72 6f77 5f68 6569  ..r......row_hei
-000010a0: 6768 7473 7211 0000 0072 1200 0000 2901  ghtsr....r....).
-000010b0: da05 7374 6172 7429 01da 056e 5f6f 7574  ..start)...n_out
-000010c0: da05 6c69 6e65 7329 0472 3000 0000 7232  ..lines).r0...r2
-000010d0: 0000 0072 3300 0000 7234 0000 0072 3900  ...r3...r4...r9.
-000010e0: 0000 722f 0000 00e9 0a00 0000 e904 0000  ..r/............
-000010f0: 007a 0c6c 696e 652d 6e73 2d6f 7065 6e29  .z.line-ns-open)
-00001100: 03da 0473 697a 65da 0a6c 696e 655f 7769  ...size..line_wi
-00001110: 6474 68da 0673 796d 626f 6c29 0572 3000  dth..symbol).r0.
-00001120: 0000 7232 0000 0072 3300 0000 7234 0000  ..r2...r3...r4..
-00001130: 0072 3600 0000 4629 0372 3a00 0000 723b  .r6...F).r:...r;
-00001140: 0000 0072 4700 0000 da0a 5469 6d65 7365  ...rG.....Timese
-00001150: 7269 6573 724b 0000 007a 0820 6f75 7420  riesrK...z. out 
-00001160: 6f66 207a 1320 6461 7461 2070 6f69 6e74  of z. data point
-00001170: 7329 3c2f 7375 703e 679a 9999 9999 99c9  s)</sup>g.......
-00001180: bf72 5200 0000 2903 7232 0000 0072 3300  .rR...).r2...r3.
-00001190: 0000 7253 0000 0029 0372 4600 0000 7238  ..rS...).rF...r8
-000011a0: 0000 0072 5500 0000 2922 7208 0000 0072  ...rU...)"r....r
-000011b0: 0700 0000 da12 6576 656e 745f 7365 7269  ......event_seri
-000011c0: 6573 5f74 7970 6573 da04 6b65 7973 da12  es_types..keys..
-000011d0: 6d65 6173 7572 656d 656e 745f 7365 7269  measurement_seri
-000011e0: 6573 7209 0000 0072 5d00 0000 7261 0000  esr....r]...ra..
-000011f0: 0072 9500 0000 7262 0000 0072 1f00 0000  .r....rb...r....
-00001200: da0c 7473 646f 776e 7361 6d70 6c65 7299  ..tsdownsampler.
-00001210: 0000 0072 6800 0000 725e 0000 0072 6400  ...rh...r^...rd.
-00001220: 0000 7265 0000 0072 6d00 0000 7205 0000  ..re...rm...r...
-00001230: 0072 1a00 0000 da04 6973 6e61 da06 7661  .r......isna..va
-00001240: 6c75 6573 da0a 646f 776e 7361 6d70 6c65  lues..downsample
-00001250: 7275 0000 0072 7000 0000 7271 0000 00da  ru...rp...rq....
-00001260: 0c65 7665 6e74 5f73 6572 6965 7372 8b00  .event_seriesr..
-00001270: 0000 7272 0000 0072 2000 0000 da0a 7a65  ..rr...r .....ze
-00001280: 726f 735f 6c69 6b65 7273 0000 0072 7600  ros_likers...rv.
-00001290: 0000 7277 0000 0029 1a72 0b00 0000 7297  ..rw...).r....r.
-000012a0: 0000 0072 8b00 0000 7261 0000 0072 8d00  ...r....ra...r..
-000012b0: 0000 7278 0000 00da 1373 706c 6974 5f69  ..rx.....split_i
-000012c0: 6e74 6f5f 7375 6270 6c6f 7473 727e 0000  nto_subplotsr~..
-000012d0: 0072 6200 0000 da07 7361 6d70 6c65 72da  .rb.....sampler.
-000012e0: 0b66 756c 6c5f 6c65 6e67 7468 7299 0000  .full_lengthr...
-000012f0: 00da 0766 5f63 6f75 6e74 729a 0000 0072  ...f_countr....r
-00001300: 7a00 0000 7215 0000 0072 1600 0000 7232  z...r....r....r2
-00001310: 0000 0072 3300 0000 da05 6973 6e61 5fda  ...r3.....isna_.
-00001320: 0473 6964 7872 3a00 0000 da0c 6c61 7374  .sidxr:.....last
-00001330: 5f72 6f77 5f69 6478 da01 65da 0365 6466  _row_idx..e..edf
-00001340: 7246 0000 0072 1300 0000 7213 0000 0072  rF...r....r....r
-00001350: 1700 0000 da16 6372 6561 7465 5f74 696d  ......create_tim
-00001360: 6573 6572 6965 735f 706c 6f74 5b00 0000  eseries_plot[...
-00001370: 7362 0000 0014 030a 0112 0118 0206 0104  sb..............
-00001380: 0208 0108 010c 0106 0124 0204 0208 0116  .........$......
-00001390: 0108 020e 0102 0106 ff14 0316 020a 0112  ................
-000013a0: 0108 0106 0106 0110 0108 0108 010c 0220  ............... 
-000013b0: 0108 0208 010c 0110 010c 0104 0112 010c  ................
-000013c0: 0104 ff04 0108 fe10 0404 020a 0116 0108  ................
-000013d0: 010c 0106 ff04 0372 b600 0000 6302 0000  .......r....c...
-000013e0: 0000 0000 0000 0000 000e 0000 000e 0000  ................
-000013f0: 0043 0000 0073 7401 0000 7400 a001 a100  .C...st...t.....
-00001400: 7d02 7402 6a03 6a04 6a05 7d03 7c00 6a06  }.t.j.j.j.}.|.j.
-00001410: 7d04 6401 6402 8400 7407 7c04 7408 7c03  }.d.d...t.|.t.|.
-00001420: 8301 8302 4400 8301 7d05 7c00 6a09 a00a  ....D...}.|.j...
-00001430: a100 4400 5d6d 5c02 7d06 7d07 7c07 6a0b  ..D.]m\.}.}.|.j.
-00001440: a00a a100 4400 5d63 5c02 7d08 7d09 7c09  ....D.]c\.}.}.|.
-00001450: 6a0c 6403 1900 a00d a100 a00e a100 6404  j.d...........d.
-00001460: 6400 8502 1900 a00f 7410 6a11 6a12 a101  d.......t.j.j...
-00001470: 7d0a 7c01 7247 6404 7c0a 7c0a 6405 6b03  }.|.rGd.|.|.d.k.
-00001480: 1900 1b00 7d0b 6e04 7c0a 6406 1400 7d0b  ....}.n.|.d...}.
-00001490: 7413 7c0a 8301 6405 6b04 726c 7c0a 7c0a  t.|...d.k.rl|.|.
-000014a0: 6405 6b02 1900 a014 a100 7413 7c0a 8301  d.k.......t.|...
-000014b0: 1b00 7d0c 7c0c 6405 6b04 726c 7415 6407  ..}.|.d.k.rlt.d.
-000014c0: 6408 7c0c 1400 6409 9b04 640a 9d03 8301  d.|...d...d.....
-000014d0: 0100 7400 6a16 7c06 6701 7413 7c0b 8301  ..t.j.|.g.t.|...
-000014e0: 1400 7c0b 7c08 7417 7c05 7c08 1900 640b  ..|.|.t.|.|...d.
-000014f0: 8d01 640c 640d 7c08 640e 7c08 640f 8d09  ..d.d.|.d.|.d...
-00001500: 7d0d 7c02 a018 7c0d a101 0100 7126 711d  }.|...|.....q&q.
-00001510: 7c04 4400 5d1c 7d08 7c02 a018 7400 6a19  |.D.].}.|...t.j.
-00001520: 6400 6701 6400 6701 7417 7c05 7c08 1900  d.g.d.g.t.|.|...
-00001530: 640b 8d01 6410 7c08 6411 6412 6901 7c08  d...d.|.d.d.i.|.
-00001540: 640d 6413 6414 8d09 a101 0100 718d 7c02  d.d.d.......q.|.
-00001550: 6a1a 6415 7c01 72b1 6416 6e01 6417 6418  j.d.|.r.d.n.d.d.
-00001560: 6419 641a 641b 8d05 0100 7c02 5300 291c  d.d.d.....|.S.).
-00001570: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-00001580: 0000 0400 0000 5300 0000 7227 0000 0072  ......S...r'...r
-00001590: 1300 0000 7213 0000 0072 2800 0000 7213  ....r....r(...r.
-000015a0: 0000 0072 1300 0000 7217 0000 0072 2b00  ...r....r....r+.
-000015b0: 0000 9c00 0000 722c 0000 007a 3563 7265  ......r,...z5cre
-000015c0: 6174 655f 6d65 6173 7572 656d 656e 745f  ate_measurement_
-000015d0: 6672 6571 7565 6e63 795f 706c 6f74 2e3c  frequency_plot.<
-000015e0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
-000015f0: 703e da04 7469 6d65 720d 0000 0072 0100  p>..timer....r..
-00001600: 0000 69e8 0300 007a 184f 7665 726c 6170  ..i....z.Overlap
-00001610: 7069 6e67 2074 696d 6573 7461 6d70 733a  ping timestamps:
-00001620: 20e9 6400 0000 7a03 2e32 66fa 0125 722d   .d...z..2f..%r-
-00001630: 0000 00da 1173 7573 7065 6374 6564 6f75  .....suspectedou
-00001640: 746c 6965 7273 5446 2909 7232 0000 0072  tliersTF).r2...r
-00001650: 3300 0000 7230 0000 0072 3600 0000 da09  3...r0...r6.....
-00001660: 626f 7870 6f69 6e74 73da 0762 6f78 6d65  boxpoints..boxme
-00001670: 616e 7237 0000 0072 3800 0000 da0b 6f66  anr7...r8.....of
-00001680: 6673 6574 6772 6f75 7072 2f00 0000 722e  fsetgroupr/...r.
-00001690: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
-000016a0: 0000 7a33 456d 7069 7269 6361 6c20 4672  ..z3Empirical Fr
-000016b0: 6571 7565 6e63 7920 6f66 204d 6561 7375  equency of Measu
-000016c0: 7265 6d65 6e74 2054 7970 6573 2070 6572  rement Types per
-000016d0: 204f 626a 6563 747a 045b 487a 5d7a 045b   Objectz.[Hz]z.[
-000016e0: 6d73 5d7a 104d 6561 7375 7265 6d65 6e74  ms]z.Measurement
-000016f0: 2054 7970 6572 5100 0000 da05 6772 6f75   TyperQ.....grou
-00001700: 7029 0572 4600 0000 da0b 7961 7869 735f  p).rF.....yaxis_
-00001710: 7469 746c 65da 0b78 6178 6973 5f74 6974  title..xaxis_tit
-00001720: 6c65 da0c 6c65 6765 6e64 5f74 6974 6c65  le..legend_title
-00001730: da07 626f 786d 6f64 6529 1b72 7000 0000  ..boxmode).rp...
-00001740: da06 4669 6775 7265 7256 0000 0072 5700  ..FigurerV...rW.
-00001750: 0000 7258 0000 0072 5900 0000 725a 0000  ..rX...rY...rZ..
-00001760: 0072 5b00 0000 7202 0000 0072 a600 0000  .r[...r....r....
-00001770: 7267 0000 00da 0a6f 626a 6563 745f 6d61  rg.....object_ma
-00001780: 7072 6200 0000 da0b 736f 7274 5f76 616c  prb.....sort_val
-00001790: 7565 73da 0464 6966 66da 036d 6170 721d  ues..diff..mapr.
-000017a0: 0000 00da 0954 696d 6564 656c 7461 da0d  .....Timedelta..
-000017b0: 746f 7461 6c5f 7365 636f 6e64 7372 1f00  total_secondsr..
-000017c0: 0000 da05 636f 756e 74da 0570 7269 6e74  ....count..print
-000017d0: da03 426f 7872 7300 0000 7275 0000 0072  ..Boxrs...ru...r
-000017e0: 7200 0000 7277 0000 0029 0e72 0b00 0000  r...rw...).r....
-000017f0: da06 7573 655f 687a 727a 0000 0072 2300  ..use_hzrz...r#.
-00001800: 0000 727c 0000 0072 7d00 0000 da01 6dda  ..r|...r}.....m.
-00001810: 036d 7363 7229 0000 00da 0274 73da 0564  .mscr).....ts..d
-00001820: 6966 6673 7222 0000 00da 0d7a 6572 6f5f  iffsr".....zero_
-00001830: 6672 6163 7469 6f6e da01 6272 1300 0000  fraction..br....
-00001840: 7213 0000 0072 1700 0000 da21 6372 6561  r....r.....!crea
-00001850: 7465 5f6d 6561 7375 7265 6d65 6e74 5f66  te_measurement_f
-00001860: 7265 7175 656e 6379 5f70 6c6f 7498 0000  requency_plot...
-00001870: 0073 3e00 0000 0801 0a01 0601 1801 1201  .s>.............
-00001880: 1201 2401 0402 1201 0802 0c01 1801 0801  ..$.............
-00001890: 1601 2001 0201 0801 06fe 0c04 02f1 0811  .. .............
-000018a0: 0402 1c01 0c01 04ff 06ff 0603 0a01 0601  ................
-000018b0: 06fe 0403 72d4 0000 0029 0272 0a00 0000  ....r....).r....
-000018c0: 5429 0454 5472 9600 0000 4629 0154 291d  T).TTr....F).T).
-000018d0: da09 6974 6572 746f 6f6c 7372 0200 0000  ..itertoolsr....
-000018e0: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
-000018f0: 0000 da05 6e75 6d70 7972 2000 0000 da06  ....numpyr .....
-00001900: 7061 6e64 6173 721d 0000 0072 5600 0000  pandasr....rV...
-00001910: da14 706c 6f74 6c79 2e67 7261 7068 5f6f  ..plotly.graph_o
-00001920: 626a 6563 7473 da0d 6772 6170 685f 6f62  bjects..graph_ob
-00001930: 6a65 6374 7372 7000 0000 da0f 706c 6f74  jectsrp.....plot
-00001940: 6c79 2e73 7562 706c 6f74 7372 0500 0000  ly.subplotsr....
-00001950: da0a 6d64 6174 612e 636f 7265 7206 0000  ..mdata.corer...
-00001960: 0072 5e00 0000 da0f 6d64 6174 612e 636f  .r^.....mdata.co
-00001970: 7265 2e75 7469 6c72 0700 0000 7208 0000  re.utilr....r...
-00001980: 0072 0900 0000 da0b 4d61 6368 696e 6544  .r......MachineD
-00001990: 6174 6172 8900 0000 728a 0000 0072 9100  atar....r....r..
-000019a0: 0000 7294 0000 0072 b600 0000 72d4 0000  ..r....r....r...
-000019b0: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
-000019c0: 7217 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000019d0: 0000 0073 2600 0000 0c00 1001 0802 0801  ...s&...........
-000019e0: 0801 0c01 0c01 0c02 1401 1203 1046 0208  .............F..
-000019f0: 0201 12fe 0a01 02ff 0a02 0afe 163d       .............=
+00000ea0: 7c06 7260 7412 6404 740a 7c03 8301 8302  |.r`t.d.t.|.....
+00000eb0: 7d0c 6405 7c0c 1b00 6701 7c0c 1400 6406  }.d.|...g.|...d.
+00000ec0: 6701 1700 7d0d 6e04 6405 6406 6702 7d0d  g...}.n.d.d.g.}.
+00000ed0: 7413 740a 7c0d 8301 6404 7c0d 6407 6408  t.t.|...d.|.d.d.
+00000ee0: 6409 8d05 7d0e 7414 7c03 6404 640a 8d02  d...}.t.|.d.d...
+00000ef0: 4400 5d4c 5c02 7d0f 7d10 7c08 740e 6a0f  D.]L\.}.}.|.t.j.
+00000f00: 6a11 1900 7c08 7c10 1900 0202 7d11 7d12  j...|.|.....}.}.
+00000f10: 7c12 a015 a100 0f00 7d13 7c11 7c13 1900  |.......}.|.|...
+00000f20: 7c12 7c13 1900 0202 7d11 7d12 7c09 6400  |.|.....}.}.|.d.
+00000f30: 7501 72ac 7c11 6a16 7d11 7c12 6a16 7d12  u.r.|.j.}.|.j.}.
+00000f40: 7c09 6a17 7c11 7c12 7c05 640b 8d03 7d14  |.j.|.|.|.d...}.
+00000f50: 7c11 7c14 1900 7d11 7c12 7c14 1900 7d12  |.|...}.|.|...}.
+00000f60: 7c06 72b0 7c0f 6e01 6404 7d15 7c0e 6a18  |.r.|.n.d.}.|.j.
+00000f70: 7419 6a1a 7c10 7c11 7c12 640c 640d 8d04  t.j.|.|.|.d.d...
+00000f80: 7c15 6404 640e 8d03 0100 7175 740a 7c0d  |.d.d.....qut.|.
+00000f90: 8301 7d16 7c04 4400 5d2e 7d17 7c00 6a1b  ..}.|.D.].}.|.j.
+00000fa0: 7c17 1900 6a09 7d18 7c18 6a0d 7c18 6a1c  |...j.}.|.j.|.j.
+00000fb0: 7c02 6b02 1900 7d18 7c18 740e 6a0f 6a11  |.k...}.|.t.j.j.
+00000fc0: 1900 7d11 7c0e 6a18 7419 6a1d 7c17 7c11  ..}.|.j.t.j.|.|.
+00000fd0: 741e a01f 7c11 a101 640f 7420 6410 6411  t...|...d.t d.d.
+00000fe0: 6412 6413 8d03 6414 8d05 7c16 6404 640e  d.d...d...|.d.d.
+00000ff0: 8d03 0100 71c8 7c0e 6a21 7c16 6404 6415  ....q.|.j!|.d.d.
+00001000: 6416 8d03 0100 6417 7d19 7c09 6400 7501  d.....d.}.|.d.u.
+00001010: 9001 7211 7c19 6418 7c05 9b00 6419 7c0a  ..r.|.d.|...d.|.
+00001020: 9b00 641a 9d05 3700 7d19 7c0e 6a22 7c19  ..d...7.}.|.j"|.
+00001030: 6407 7420 6402 641b 641c 641d 8d03 641e  d.t d.d.d.d...d.
+00001040: 8d03 0100 7c0e 5300 291f 4e29 01da 0769  ....|.S.).N)...i
+00001050: 665f 7472 7565 7201 0000 0029 01da 154d  f_truer....)...M
+00001060: 696e 4d61 784c 5454 4244 6f77 6e73 616d  inMaxLTTBDownsam
+00001070: 706c 6572 720d 0000 0067 cdcc cccc cccc  plerr....g......
+00001080: ec3f 720e 0000 0054 679a 9999 9999 99a9  .?r....Tg.......
+00001090: 3f29 0572 0f00 0000 7210 0000 00da 0b72  ?).r....r......r
+000010a0: 6f77 5f68 6569 6768 7473 7211 0000 0072  ow_heightsr....r
+000010b0: 1200 0000 2901 da05 7374 6172 7429 015a  ....)...start).Z
+000010c0: 056e 5f6f 7574 da05 6c69 6e65 7329 0472  .n_out..lines).r
+000010d0: 3000 0000 7232 0000 0072 3300 0000 7234  0...r2...r3...r4
+000010e0: 0000 0072 3900 0000 722f 0000 00e9 0a00  ...r9...r/......
+000010f0: 0000 e904 0000 007a 0c6c 696e 652d 6e73  .......z.line-ns
+00001100: 2d6f 7065 6e29 03da 0473 697a 65da 0a6c  -open)...size..l
+00001110: 696e 655f 7769 6474 68da 0673 796d 626f  ine_width..symbo
+00001120: 6c29 0572 3000 0000 7232 0000 0072 3300  l).r0...r2...r3.
+00001130: 0000 7234 0000 0072 3600 0000 4629 0372  ..r4...r6...F).r
+00001140: 3a00 0000 723b 0000 0072 4500 0000 5a0a  :...r;...rE...Z.
+00001150: 5469 6d65 7365 7269 6573 7248 0000 007a  TimeseriesrH...z
+00001160: 0820 6f75 7420 6f66 207a 1320 6461 7461  . out of z. data
+00001170: 2070 6f69 6e74 7329 3c2f 7375 703e 679a   points)</sup>g.
+00001180: 9999 9999 99c9 bf72 4f00 0000 2903 7232  .......rO...).r2
+00001190: 0000 0072 3300 0000 7250 0000 0029 0372  ...r3...rP...).r
+000011a0: 4400 0000 7238 0000 0072 5200 0000 2923  D...r8...rR...)#
+000011b0: 7208 0000 0072 0700 0000 da12 6576 656e  r....r......even
+000011c0: 745f 7365 7269 6573 5f74 7970 6573 da04  t_series_types..
+000011d0: 6b65 7973 da12 6d65 6173 7572 656d 656e  keys..measuremen
+000011e0: 745f 7365 7269 6573 7209 0000 0072 5a00  t_seriesr....rZ.
+000011f0: 0000 725e 0000 0072 8d00 0000 725f 0000  ..r^...r....r_..
+00001200: 0072 1f00 0000 5a0c 7473 646f 776e 7361  .r....Z.tsdownsa
+00001210: 6d70 6c65 7291 0000 0072 6500 0000 725b  mpler....re...r[
+00001220: 0000 0072 6100 0000 7262 0000 0072 6a00  ...ra...rb...rj.
+00001230: 0000 7266 0000 0072 0500 0000 721a 0000  ..rf...r....r...
+00001240: 00da 0469 736e 61da 0676 616c 7565 735a  ...isna..valuesZ
+00001250: 0a64 6f77 6e73 616d 706c 6572 7200 0000  .downsamplerr...
+00001260: 726d 0000 0072 6e00 0000 da0c 6576 656e  rm...rn.....even
+00001270: 745f 7365 7269 6573 7284 0000 0072 6f00  t_seriesr....ro.
+00001280: 0000 7220 0000 00da 0a7a 6572 6f73 5f6c  ..r .....zeros_l
+00001290: 696b 6572 7000 0000 7273 0000 0072 7400  ikerp...rs...rt.
+000012a0: 0000 291a 720b 0000 0072 8f00 0000 7284  ..).r....r....r.
+000012b0: 0000 0072 5e00 0000 7285 0000 0072 7500  ...r^...r....ru.
+000012c0: 0000 da13 7370 6c69 745f 696e 746f 5f73  ....split_into_s
+000012d0: 7562 706c 6f74 7372 7900 0000 725f 0000  ubplotsry...r_..
+000012e0: 005a 0773 616d 706c 6572 5a0b 6675 6c6c  .Z.samplerZ.full
+000012f0: 5f6c 656e 6774 6872 9100 0000 5a07 665f  _lengthr....Z.f_
+00001300: 636f 756e 7472 9200 0000 7276 0000 0072  countr....rv...r
+00001310: 1500 0000 7216 0000 0072 3200 0000 7233  ....r....r2...r3
+00001320: 0000 005a 0569 736e 615f da04 7369 6478  ...Z.isna_..sidx
+00001330: 723a 0000 005a 0c6c 6173 745f 726f 775f  r:...Z.last_row_
+00001340: 6964 78da 0165 5a03 6564 6672 4400 0000  idx..eZ.edfrD...
+00001350: 7213 0000 0072 1300 0000 7217 0000 00da  r....r....r.....
+00001360: 1663 7265 6174 655f 7469 6d65 7365 7269  .create_timeseri
+00001370: 6573 5f70 6c6f 745b 0000 0073 6200 0000  es_plot[...sb...
+00001380: 1403 0a01 1201 1802 0601 0402 0801 0801  ................
+00001390: 0c01 0601 2402 0402 0e01 1601 0802 0e01  ....$...........
+000013a0: 0201 06ff 1403 1602 0a01 1201 0801 0601  ................
+000013b0: 0601 1001 0801 0801 0c02 2001 0802 0801  .......... .....
+000013c0: 0c01 1001 0c01 0401 1201 0c01 04ff 0401  ................
+000013d0: 08fe 1004 0402 0a01 1601 0801 0c01 06ff  ................
+000013e0: 0403 72a4 0000 0063 0200 0000 0000 0000  ..r....c........
+000013f0: 0000 0000 0e00 0000 0e00 0000 4300 0000  ............C...
+00001400: 7374 0100 0074 00a0 01a1 007d 0274 026a  st...t.....}.t.j
+00001410: 036a 046a 057d 037c 006a 067d 0464 0164  .j.j.}.|.j.}.d.d
+00001420: 0284 0074 077c 0474 087c 0383 0183 0244  ...t.|.t.|.....D
+00001430: 0083 017d 057c 006a 09a0 0aa1 0044 005d  ...}.|.j.....D.]
+00001440: 6d5c 027d 067d 077c 076a 0ba0 0aa1 0044  m\.}.}.|.j.....D
+00001450: 005d 635c 027d 087d 097c 096a 0c64 0319  .]c\.}.}.|.j.d..
+00001460: 00a0 0da1 00a0 0ea1 0064 0464 0085 0219  .........d.d....
+00001470: 00a0 0f74 106a 116a 12a1 017d 0a7c 0172  ...t.j.j...}.|.r
+00001480: 4764 047c 0a7c 0a64 056b 0319 001b 007d  Gd.|.|.d.k.....}
+00001490: 0b6e 047c 0a64 0614 007d 0b74 137c 0a83  .n.|.d...}.t.|..
+000014a0: 0164 056b 0472 6c7c 0a7c 0a64 056b 0219  .d.k.rl|.|.d.k..
+000014b0: 00a0 14a1 0074 137c 0a83 011b 007d 0c7c  .....t.|.....}.|
+000014c0: 0c64 056b 0472 6c74 1564 0764 087c 0c14  .d.k.rlt.d.d.|..
+000014d0: 0064 099b 0464 0a9d 0383 0101 0074 006a  .d...d.......t.j
+000014e0: 167c 0667 0174 137c 0b83 0114 007c 0b7c  .|.g.t.|.....|.|
+000014f0: 0874 177c 057c 0819 0064 0b8d 0164 0c64  .t.|.|...d...d.d
+00001500: 0d7c 0864 0e7c 0864 0f8d 097d 0d7c 02a0  .|.d.|.d...}.|..
+00001510: 187c 0da1 0101 0071 2671 1d7c 0444 005d  .|.....q&q.|.D.]
+00001520: 1c7d 087c 02a0 1874 006a 1964 0067 0164  .}.|...t.j.d.g.d
+00001530: 0067 0174 177c 057c 0819 0064 0b8d 0164  .g.t.|.|...d...d
+00001540: 107c 0864 1164 1269 017c 0864 0d64 1364  .|.d.d.i.|.d.d.d
+00001550: 148d 09a1 0101 0071 8d7c 026a 1a64 157c  .......q.|.j.d.|
+00001560: 0172 b164 166e 0164 1764 1864 1964 1a64  .r.d.n.d.d.d.d.d
+00001570: 1b8d 0501 007c 0253 0029 1c4e 6301 0000  .....|.S.).Nc...
+00001580: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00001590: 0053 0000 0072 2700 0000 7213 0000 0072  .S...r'...r....r
+000015a0: 1300 0000 7228 0000 0072 1300 0000 7213  ....r(...r....r.
+000015b0: 0000 0072 1700 0000 722b 0000 009c 0000  ...r....r+......
+000015c0: 0072 2c00 0000 7a35 6372 6561 7465 5f6d  .r,...z5create_m
+000015d0: 6561 7375 7265 6d65 6e74 5f66 7265 7175  easurement_frequ
+000015e0: 656e 6379 5f70 6c6f 742e 3c6c 6f63 616c  ency_plot.<local
+000015f0: 733e 2e3c 6469 6374 636f 6d70 3eda 0474  s>.<dictcomp>..t
+00001600: 696d 6572 0d00 0000 7201 0000 0069 e803  imer....r....i..
+00001610: 0000 7a18 4f76 6572 6c61 7070 696e 6720  ..z.Overlapping 
+00001620: 7469 6d65 7374 616d 7073 3a20 e964 0000  timestamps: .d..
+00001630: 007a 032e 3266 fa01 2572 2d00 0000 5a11  .z..2f..%r-...Z.
+00001640: 7375 7370 6563 7465 646f 7574 6c69 6572  suspectedoutlier
+00001650: 7354 4629 0972 3200 0000 7233 0000 0072  sTF).r2...r3...r
+00001660: 3000 0000 7236 0000 005a 0962 6f78 706f  0...r6...Z.boxpo
+00001670: 696e 7473 5a07 626f 786d 6561 6e72 3700  intsZ.boxmeanr7.
+00001680: 0000 7238 0000 00da 0b6f 6666 7365 7467  ..r8.....offsetg
+00001690: 726f 7570 722f 0000 0072 2e00 0000 723c  roupr/...r....r<
+000016a0: 0000 0072 3d00 0000 723e 0000 007a 3345  ...r=...r>...z3E
+000016b0: 6d70 6972 6963 616c 2046 7265 7175 656e  mpirical Frequen
+000016c0: 6379 206f 6620 4d65 6173 7572 656d 656e  cy of Measuremen
+000016d0: 7420 5479 7065 7320 7065 7220 4f62 6a65  t Types per Obje
+000016e0: 6374 7a04 5b48 7a5d 7a04 5b6d 735d 7a10  ctz.[Hz]z.[ms]z.
+000016f0: 4d65 6173 7572 656d 656e 7420 5479 7065  Measurement Type
+00001700: 724e 0000 00da 0567 726f 7570 2905 7244  rN.....group).rD
+00001710: 0000 005a 0b79 6178 6973 5f74 6974 6c65  ...Z.yaxis_title
+00001720: 5a0b 7861 7869 735f 7469 746c 655a 0c6c  Z.xaxis_titleZ.l
+00001730: 6567 656e 645f 7469 746c 65da 0762 6f78  egend_title..box
+00001740: 6d6f 6465 291b 726d 0000 00da 0646 6967  mode).rm.....Fig
+00001750: 7572 6572 5300 0000 7254 0000 0072 5500  urerS...rT...rU.
+00001760: 0000 7256 0000 0072 5700 0000 7258 0000  ..rV...rW...rX..
+00001770: 0072 0200 0000 729c 0000 0072 6400 0000  .r....r....rd...
+00001780: da0a 6f62 6a65 6374 5f6d 6170 725f 0000  ..object_mapr_..
+00001790: 00da 0b73 6f72 745f 7661 6c75 6573 da04  ...sort_values..
+000017a0: 6469 6666 da03 6d61 7072 1d00 0000 da09  diff..mapr......
+000017b0: 5469 6d65 6465 6c74 61da 0d74 6f74 616c  Timedelta..total
+000017c0: 5f73 6563 6f6e 6473 721f 0000 00da 0563  _secondsr......c
+000017d0: 6f75 6e74 da05 7072 696e 74da 0342 6f78  ount..print..Box
+000017e0: 7270 0000 0072 7200 0000 726f 0000 0072  rp...rr...ro...r
+000017f0: 7400 0000 290e 720b 0000 005a 0675 7365  t...).r....Z.use
+00001800: 5f68 7a72 7600 0000 7223 0000 0072 7700  _hzrv...r#...rw.
+00001810: 0000 7278 0000 00da 016d 5a03 6d73 6372  ..rx.....mZ.mscr
+00001820: 2900 0000 da02 7473 da05 6469 6666 7372  ).....ts..diffsr
+00001830: 2200 0000 5a0d 7a65 726f 5f66 7261 6374  "...Z.zero_fract
+00001840: 696f 6eda 0162 7213 0000 0072 1300 0000  ion..br....r....
+00001850: 7217 0000 00da 2163 7265 6174 655f 6d65  r.....!create_me
+00001860: 6173 7572 656d 656e 745f 6672 6571 7565  asurement_freque
+00001870: 6e63 795f 706c 6f74 9800 0000 733e 0000  ncy_plot....s>..
+00001880: 0008 010a 0106 0118 0112 0112 0124 0104  .............$..
+00001890: 0212 0108 020c 0118 0108 0116 0120 0102  ............. ..
+000018a0: 0108 0106 fe0c 0402 f108 1104 021c 010c  ................
+000018b0: 0104 ff06 ff06 030a 0106 0106 fe04 0372  ...............r
+000018c0: b900 0000 2902 720a 0000 0054 2904 5454  ....).r....T).TT
+000018d0: 728e 0000 0046 2901 5429 1dda 0969 7465  r....F).T)...ite
+000018e0: 7274 6f6f 6c73 7202 0000 00da 0674 7970  rtoolsr......typ
+000018f0: 696e 6772 0300 0000 7204 0000 00da 056e  ingr....r......n
+00001900: 756d 7079 7220 0000 00da 0670 616e 6461  umpyr .....panda
+00001910: 7372 1d00 0000 7253 0000 00da 1470 6c6f  sr....rS.....plo
+00001920: 746c 792e 6772 6170 685f 6f62 6a65 6374  tly.graph_object
+00001930: 73da 0d67 7261 7068 5f6f 626a 6563 7473  s..graph_objects
+00001940: 726d 0000 005a 0f70 6c6f 746c 792e 7375  rm...Z.plotly.su
+00001950: 6270 6c6f 7473 7205 0000 00da 0a6d 6461  bplotsr......mda
+00001960: 7461 2e63 6f72 6572 0600 0000 725b 0000  ta.corer....r[..
+00001970: 005a 0f6d 6461 7461 2e63 6f72 652e 7574  .Z.mdata.core.ut
+00001980: 696c 7207 0000 0072 0800 0000 7209 0000  ilr....r....r...
+00001990: 00da 0b4d 6163 6869 6e65 4461 7461 7282  ...MachineDatar.
+000019a0: 0000 0072 8300 0000 7289 0000 0072 8c00  ...r....r....r..
+000019b0: 0000 72a4 0000 0072 b900 0000 7213 0000  ..r....r....r...
+000019c0: 0072 1300 0000 7213 0000 0072 1700 0000  .r....r....r....
+000019d0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
+000019e0: 0000 000c 0010 0108 0208 0108 010c 010c  ................
+000019f0: 010c 0214 0112 0310 4602 0802 0112 fe0a  ........F.......
+00001a00: 0102 ff0a 020a fe16 3d                   ........=
```

### Comparing `mdata-0.1.1/src/mdata/visualization/matplot.py` & `mdata-0.1.2/src/mdata/visualization/matplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     fs = features
     if os is None:
         os = list(tsc.object_map.keys())
     else:
         assert os <= set(tsc.object_map.keys())
         os = [o for o in tsc.object_map if o in os]
     if fs is None:
-        fs = list(tsc.timeseries_type.features)
+        fs = list(tsc.timeseries_spec.features)
     else:
-        assert set(fs) <= set(tsc.timeseries_type.features)
-        fs = [f for f in fs if f in tsc.timeseries_type.features]
+        assert set(fs) <= set(tsc.timeseries_spec.features)
+        fs = [f for f in fs if f in tsc.timeseries_spec.features]
 
     fig, axs = plt.subplots(len(fs), 1, sharex=True, figsize=figsize)
 
     for i, f in enumerate(fs):
         for o in os:
             ts = tsc.view(o)
             sns.lineplot(data=ts.df, x='time', y=f, ax=axs[i])
```

### Comparing `mdata-0.1.1/src/mdata/visualization/plotting.py` & `mdata-0.1.2/src/mdata/visualization/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     did_downsample = False
     colorscale = plotly.colors.qualitative.Plotly
     objs = md.occurring_objects
     color_dict = {o: c for o, c in zip(objs, cycle(colorscale))}
 
     for tsc in md.iter_all_timeseries():
-        timeseries_type = tsc.timeseries_type
+        timeseries_type = tsc.timeseries_spec
         typ = timeseries_type.type
-        row = 1 if typ == mdd.MachineDataTypes.E else 2
+        row = 1 if typ == mdd.ObservationTypes.E else 2
         fs = timeseries_type.features
         for g, gidx in tsc.df.groupby(mdd.MDConcepts.Object).groups.items():
             obj = g
             df = tsc.df.loc[gidx]
             c = color_dict[g]
 
             length = len(df)
@@ -87,19 +87,19 @@
     features: list[str] | bool
     events: set[str] | bool
 
 
 def create_timeseries_plot(md: mdd.MachineData, measurement_type: str, object: str,
                            features: Collection[str] | bool = True,
                            events: Collection[str] | bool = True, downsample_to=15_000, split_into_subplots=False):
-    events = mangle_arg_with_bool_fallback(mangle_arg_to_set, events, if_true=md.event_series_types.keys())
+    events = mangle_arg_with_bool_fallback(mangle_arg_to_set, events, if_true=md.event_specs.keys())
     tsc = md.measurement_series[measurement_type]
-    features = mangle_arg_with_bool_fallback(mangle_arg_to_list, features, if_true=tsc.timeseries_type.features)
+    features = mangle_arg_with_bool_fallback(mangle_arg_to_list, features, if_true=tsc.timeseries_spec.features)
 
-    assert set(features) <= set(tsc.timeseries_type.features)
+    assert set(features) <= set(tsc.timeseries_spec.features)
     df = tsc.df
 
     sampler = None
     full_length = len(df)
     if full_length > downsample_to:
         from tsdownsample import MinMaxLTTBDownsampler
         sampler = MinMaxLTTBDownsampler()
```

### Comparing `mdata-0.1.1/PKG-INFO` & `mdata-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Keywords: data format,machine data
 Author: Leah Tacke genannt Unterberg
 Author-email: leah.tgu@pads.rwth-aachen.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bottleneck
-Requires-Dist: jupyter (>=1.0,<2.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numba
+Requires-Dist: immutabledict
+Requires-Dist: llvmlite (>=0.40,<0.41)
+Requires-Dist: matplotlib
+Requires-Dist: numba (>=0.57,<0.58)
 Requires-Dist: numexpr
 Requires-Dist: pandas (>=1.5,<2.0)
 Requires-Dist: plotly (>=5.15,<6.0)
 Requires-Dist: seaborn
-Requires-Dist: tables (>=3.8.0,<4.0.0)
+Requires-Dist: tables
 Requires-Dist: tsdownsample (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
 This is the official machine data format package.
 
 It supports csv importing, exporting and format compliance checking.
 Machine data is parsed into a python object that provides typed views on the contained measurement and event timeseries.
```

