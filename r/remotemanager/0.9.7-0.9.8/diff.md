# Comparing `tmp/remotemanager-0.9.7.tar.gz` & `tmp/remotemanager-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.7.tar", last modified: Fri Jul 28 13:16:39 2023, max compression
+gzip compressed data, was "remotemanager-0.9.8.tar", last modified: Mon Jul 31 11:04:29 2023, max compression
```

## Comparing `remotemanager-0.9.7.tar` & `remotemanager-0.9.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-28 13:16:39.780554 remotemanager-0.9.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-28 12:51:04.000000 remotemanager-0.9.7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.772554 remotemanager-0.9.7/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-28 12:51:04.000000 remotemanager-0.9.7/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.7/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:10.000000 remotemanager-0.9.7/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:04.000000 remotemanager-0.9.7/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:04.000000 remotemanager-0.9.7/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.7/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.7/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:57.000000 remotemanager-0.9.7/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    55665 2023-07-28 12:51:04.000000 remotemanager-0.9.7/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    10839 2023-07-28 11:41:58.000000 remotemanager-0.9.7/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.7/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    23111 2023-07-28 11:41:58.000000 remotemanager-0.9.7/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.7/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:27.000000 remotemanager-0.9.7/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.7/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.7/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.7/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.7/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.7/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:30.000000 remotemanager-0.9.7/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.7/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.7/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:31.000000 remotemanager-0.9.7/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:27.000000 remotemanager-0.9.7/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.7/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.7/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.772554 remotemanager-0.9.7/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 13:16:39.780554 remotemanager-0.9.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-31 11:04:29.803992 remotemanager-0.9.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-31 10:33:38.000000 remotemanager-0.9.8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.795992 remotemanager-0.9.8/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.795992 remotemanager-0.9.8/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.8/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12848 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-07-31 09:51:39.000000 remotemanager-0.9.8/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.8/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.8/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6671 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26005 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    55681 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10837 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.8/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    23111 2023-07-28 11:41:58.000000 remotemanager-0.9.8/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.8/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-31 09:51:39.000000 remotemanager-0.9.8/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.8/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.8/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.8/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5243 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:30.000000 remotemanager-0.9.8/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10025 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.8/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4504 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.8/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.795992 remotemanager-0.9.8/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 11:04:29.803992 remotemanager-0.9.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.8/setup.py
```

### Comparing `remotemanager-0.9.7/LICENSE` & `remotemanager-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/PKG-INFO` & `remotemanager-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.7
+Version: 0.9.8
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.7/README.md` & `remotemanager-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/pyproject.toml` & `remotemanager-0.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.7"
+current_version = "0.9.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.7/remotemanager/connection/cmd.py` & `remotemanager-0.9.8/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/connection/computers/base.py` & `remotemanager-0.9.8/remotemanager/connection/computers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,14 @@
         Returns:
             None
         """
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def resources_block(self, **kwargs):
-
         self.update_resources(**kwargs)
 
         if not self.valid:
             raise RuntimeError(f"missing required arguments: {self.missing}")
 
         if self._parser is None:
             return []
```

### Comparing `remotemanager-0.9.7/remotemanager/connection/computers/example.py` & `remotemanager-0.9.8/remotemanager/connection/computers/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 class Example_Torque(BaseComputer):
     """
     example class for connecting to a remote computer using a torque scheduler
     """
 
     def __init__(self, **kwargs):
-
         if "host" not in kwargs:
             kwargs["host"] = "remote.address.for.connection"
 
         super().__init__(**kwargs)
 
         self.submitter = "qsub"
         self.shebang = "#!/bin/bash"
@@ -32,15 +31,14 @@
 
 class Example_Slurm(BaseComputer):
     """
     example class for connecting to a remote computer using a slurm scheduler
     """
 
     def __init__(self, **kwargs):
-
         if "host" not in kwargs:
             kwargs["host"] = "remote.address.for.connection"
 
         super().__init__(**kwargs)
 
         self.submitter = "sbatch"
         self.shebang = "#!/bin/bash"
```

### Comparing `remotemanager-0.9.7/remotemanager/connection/computers/options.py` & `remotemanager-0.9.8/remotemanager/connection/computers/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from remotemanager import SendableMixin, LoggingMixin
+from remotemanager.logging import LoggingMixin
+from remotemanager.storage import SendableMixin
 
 
 class placeholder_option(SendableMixin, LoggingMixin):
     """
     .. warning::
         This class is intended to be subclassed by the optional and required
         placeholders.
```

### Comparing `remotemanager-0.9.7/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.8/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/connection/testing_object.py` & `remotemanager-0.9.8/remotemanager/connection/testing_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
                 with open(tmp, "w+") as o:
                     o.write(f"test_{i}")
                     written_files.append(tmp)
 
         passed = False
         transport_tests = {}
         for tmp_transport in transport_instances:
-
             name = tmp_transport.__module__
             print(f"Testing {name}:\n\tsend... ", end="")
 
             t0 = time.time()
             self.parent.cmd("mkdir -p connection_test")
 
             tmp_transport.queue_for_push(written_files, ".", "connection_test")
```

### Comparing `remotemanager-0.9.7/remotemanager/connection/url.py` & `remotemanager-0.9.8/remotemanager/connection/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         raise_errors: bool = True,
         keyfile: str = None,
         passfile: str = None,
         envpass: str = None,
         cmd_history_depth: int = 10,
         **kwargs,
     ):
-
         self._verbose = Verbosity(verbose)
 
         if host is None:
             host = URL._localhost
         self._conn = {"user": user, "host": host, "port": port}
 
         self.timeout = timeout
@@ -581,15 +580,14 @@
 
     Arguments:
         parent (URL):
             parent class to provide utils to
     """
 
     def __init__(self, parent: URL):
-
         self._logger = logging.getLogger(__name__ + ".URLUtils")
         self._logger.info(f"creating a utils extension to parent: {parent}")
 
         self._parent = parent
 
     def file_mtime(
         self,
@@ -631,15 +629,14 @@
 
         self._logger.info("received:")
         self._logger.info(times)
         self._logger.info(error)
         output = {}
         for file in files:
             if file in times:
-
                 mtime = times[file][0]
                 fsize = times[file][1]
                 if ignore_empty and fsize == 0:
                     output[file] = None
                 else:
                     output[file] = mtime
             else:
```

### Comparing `remotemanager-0.9.7/remotemanager/dataset/dataset.py` & `remotemanager-0.9.8/remotemanager/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,16 +247,15 @@
             **kwargs:
                 keyword args as passed to Dataset
         Returns:
             Dataset
         """
 
         for obj in gc.get_objects():
-            if type(obj) == cls:
-
+            if isinstance(obj, cls):
                 tmp = cls(*args, **kwargs)
                 if obj == tmp:
                     print("returning stored obj")
                     return obj
 
         if raise_if_not_found:
             raise ValueError("Dataset with args not found!")
@@ -392,15 +391,14 @@
     @property
     def is_parent(self) -> bool:
         if self.dependency is None:
             return False
         return self.short_uuid in self.dependency._parents
 
     def _mirror_dependency(self, dataset) -> None:
-
         self._logger.info(f"connecting with dataset {dataset}")
         if dataset.dependency is not None:
             self._logger.info("target has dependency, joining")
             self._dependency = dataset.dependency
         elif self.dependency is not None:
             self._logger.info("self has dependency, joining")
             dataset._dependency = self._dependency
@@ -1088,15 +1086,15 @@
             )
             self._url = URL(verbose=self.verbose)
         else:
             if not isinstance(url, URL):
                 raise ValueError("URL is not a valid URL instance")
             self._url = url
 
-        if not type(url) == URL and issubclass(type(url), URL):
+        if not type(url) == URL and issubclass(type(url), URL):  # noqa: E721
             self._computer = True
 
         timeout = self._global_run_args.get("timeout", None)
         max_timeouts = self._global_run_args.get("max_timeouts", None)
 
         self._url.timeout = timeout
         self._url.max_timeouts = max_timeouts
```

### Comparing `remotemanager-0.9.7/remotemanager/dataset/dependency.py` & `remotemanager-0.9.8/remotemanager/dataset/dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from remotemanager.storage.remotefunction import cached_functions
 from remotemanager.logging import LoggingMixin
 from remotemanager.storage.sendablemixin import SendableMixin
 
 
 class Dependency(SendableMixin, LoggingMixin):
-
     _do_not_package = ["_network"]
 
     def __init__(self):
         self._logger.info("new Dependency created")
 
         self._network = []
         self._parents = []
@@ -49,15 +48,14 @@
             if self._children[i] == uuid:
                 tmp.append(self.network[i][0])
 
         return tmp
 
     @property
     def ds_list(self):
-
         datasets = []
         for pair in self.network:
             for ds in pair:
                 if ds not in datasets:
                     datasets.append(ds)
 
         return datasets
```

### Comparing `remotemanager-0.9.7/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.8/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/dataset/runner.py` & `remotemanager-0.9.8/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.8/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/jupyter/magic.py` & `remotemanager-0.9.8/remotemanager/jupyter/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
 
-from remotemanager.logging import LoggingMixin
-from remotemanager import Dataset, Quiet
+from remotemanager.logging import LoggingMixin, Quiet
+from remotemanager import Dataset
 
 from IPython.core.magic import Magics, magics_class, cell_magic, needs_local_scope
 
 
 @magics_class
 class RCell(Magics, LoggingMixin):
     """
```

### Comparing `remotemanager-0.9.7/remotemanager/logging/__init__.py` & `remotemanager-0.9.8/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/logging/log.py` & `remotemanager-0.9.8/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/logging/utils.py` & `remotemanager-0.9.8/remotemanager/logging/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         return "\n" + "\n".join(ret)
 
     def treat_iterable(inp):
         exclude.append("")
 
         ret = []
         for v in inp:
-
             if v not in exclude:
                 if type(v) in dispatch.keys():
                     v = format_iterable(iterable=v, exclude=exclude, indent=indent + 1)
                 ret.append(INDENT_CHAR * (indent - 1) + f"- {v}")
 
         return f"\n" + f"\n".join(ret)
```

### Comparing `remotemanager-0.9.7/remotemanager/logging/verbosity.py` & `remotemanager-0.9.8/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.8/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/serialisation/serial.py` & `remotemanager-0.9.8/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.8/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.8/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/storage/database.py` & `remotemanager-0.9.8/remotemanager/storage/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         file (str):
             filename to write to
     """
 
     _versionkey = "~database-version~"
 
     def __init__(self, file):
-
         file = ensure_filetype(file, "yaml")
 
         self._logger = logging.getLogger(__name__ + ".Database")
 
         self._path = file
         self._storage = self._read()
         self._tree = None
@@ -164,41 +163,68 @@
             if isinstance(data[key], dict):
                 tmp.append(key)
                 ret += self.climb(data[key], branch + tmp)
             else:
                 ret.append(joinchar.join(branch + [key]))
         return ret
 
-    def find(self, key: str):
+    def find(self, key: str, greedy: bool = False):
         """
         Find the first instance of key within the database tree
 
         Args:
-            key (str):
+            key:
                 key (uuid) to look for
+            greedy:
+                returns the first value found if True. Faster, but does not respect
+                the tree "layers"
 
         Returns:
             database tree below key
         """
 
-        def get_minimum_path(p, k):
+        def get_minimum_path(p: str, k: str) -> list:
+            """
+            Returns the path segments of path p up to target k
+
+            >>> get_minimum_path('a/b/c/d/', 'b')
+            >>> ['a', 'b']
+
+            Args:
+                p:
+                    /path/containing/target/k/value
+                k:
+                    target within path p
+
+            Returns:
+                list of steps within path, leading to k
+            """
             fullpath = p.split("/")
             return fullpath[: fullpath.index(k) + 1]
 
-        target = []
+        target = None
         for path in self.tree:
             if key in path:
-                target = get_minimum_path(path, key)
-                break
+                tmp = get_minimum_path(path, key)
+                if greedy:
+                    target = tmp
+                    break
+                # we should prefer targets lower down the tree
+                if target is None or len(tmp) < len(target):
+                    target = tmp
+
+        if target is None:
+            return None
+
         data = chain_get(self._storage, target)
 
         return data
 
 
-def chain_get(d: dict, keys: str):
+def chain_get(d: dict, keys: list):
     """
     Get item from a nested dict using a list of keys
 
     Args:
         d (dict):
             nested dict to query
         keys (list):
```

### Comparing `remotemanager-0.9.7/remotemanager/storage/function.py` & `remotemanager-0.9.8/remotemanager/storage/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     Args:
         func:
             python function for serialisation
     """
 
     def __init__(self, func: [typing.Callable, str]):
-
         self._logger.debug(f"creating new serialisable function for {func}")
 
         self._uuid = ""
         try:
             source = inspect.getsource(func)
             source = source.replace("@RemoteFunction", "").strip()
```

### Comparing `remotemanager-0.9.7/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.8/remotemanager/storage/remotefunction.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     >>> ds = Dataset(main)
     >>> ...
 
     .. versionadded:: 0.3.6
     """
 
     def __init__(self, function):
-
         self._storedfunction = function
 
         storedfunction = Function(function)
         self._logger.info(f"caching function {storedfunction.raw_source}")
         cached_functions[function.__name__] = storedfunction
 
     def __call__(self, *args, **kwargs):
```

### Comparing `remotemanager-0.9.7/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.8/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.8/remotemanager/storage/trackedfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 
 import os
 
 from remotemanager.utils import dir_delta
 
 
 class TrackedFile(LoggingMixin, SendableMixin):
-
     __slots__ = ("_remote_path", "_local_path", "_file")
 
     def __init__(self, local_path, remote_path, file):
-
         self._remote_path = remote_path
         self._local_path = local_path
         self._file = file
 
         self._last_seen = {"remote": -1, "local": -1}
 
     def __repr__(self):
```

### Comparing `remotemanager-0.9.7/remotemanager/transport/cp.py` & `remotemanager-0.9.8/remotemanager/transport/cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 from remotemanager.transport.transport import Transport
 
 
 class cp(Transport):
     def __init__(self, *args, **kwargs):
-
         super().__init__(*args, **kwargs)
 
         self._logger.info("created new cp transport")
 
         self._cmd = "mkdir -p {secondary} ; " "cp -r --preserve {primary} {secondary}"
 
     def cmd(self, primary, secondary):
```

### Comparing `remotemanager-0.9.7/remotemanager/transport/rsync.py` & `remotemanager-0.9.8/remotemanager/transport/rsync.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Args:
         checksum (bool):
             Adds checksum arg, which if True will add --checksum flag to
             parameters
     """
 
     def __init__(self, *args, **kwargs):
-
         super().__init__(*args, **kwargs)
 
         # flags can be exposed, to utilise their flexibility
         flags = kwargs.pop("flags", "auv")
         self.flags = flags
 
         if kwargs.get("checksum", False):
@@ -29,15 +28,14 @@
             self.flags += "--checksum"
 
         self._logger.info("created new rsync transport")
 
         self._cmd = "rsync {flags} {password}{inner_dir}{primary} {secondary}"
 
     def cmd(self, primary, secondary):
-
         if self.url.passfile and self.url.keyfile:
             raise RuntimeError(
                 "rsync appears to have an issue when "
                 "specifying sshpass AND ssh-key. Either set up "
                 "your ssh config and remove the keyfile or use "
                 "transport.scp"
             )
```

### Comparing `remotemanager-0.9.7/remotemanager/transport/scp.py` & `remotemanager-0.9.8/remotemanager/transport/scp.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
     Args:
         url (URL):
             url to extract remote address from
     """
 
     def __init__(self, *args, **kwargs):
-
         super().__init__(*args, **kwargs)
 
         # flags can be exposed, to utilise their flexibility
         flags = kwargs.pop("flags", "r")
         self.flags = flags
 
         self._transfers = {}
@@ -55,15 +54,14 @@
 
         if ":" not in folder:
             return scp_join(inp)
         remote, folder = folder.split(":")
         return f'{remote}:"{scp_join(inp)}"'
 
     def cmd(self, primary, secondary):
-
         password = ""
         if self.url.passfile is not None:
             password = f"sshpass -f {self.url.passfile} "
 
         sshkey = ""
         if self.url.keyfile is not None:
             sshkey = f"-i {self.url.keyfile} "
```

### Comparing `remotemanager-0.9.7/remotemanager/transport/transport.py` & `remotemanager-0.9.8/remotemanager/transport/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     Args:
         url (URL):
             url to extract remote address from
     """
 
     def __init__(self, url=None, *args, **kwargs):
-
         self._remote_address = None
         self._url = url if url is not None else URL()
         self.set_remote(url)
 
         self._flags = Flags()
         self._transfers = {}
 
@@ -305,15 +304,14 @@
             the dry run string, or None
         """
 
         self._logger.info(f"executing a transfer")
 
         commands = []
         for pair, files in self.transfers.items():
-
             primary, secondary = Transport.split_pair(pair)
 
             primary = self._format_for_cmd(primary, files)
 
             base_cmd = self.cmd(primary=primary, secondary=secondary)
 
             commands.append(base_cmd)
```

### Comparing `remotemanager-0.9.7/remotemanager/utils/__init__.py` & `remotemanager-0.9.8/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager/utils/flags.py` & `remotemanager-0.9.8/remotemanager/utils/flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         initial_flags (str):
             initial base flags to be used and modified if needed
     """
 
     _logger = logging.getLogger(__name__ + ".Flags")
 
     def __init__(self, *initial_flags):
-
         if not isinstance(initial_flags, str):
             initial_flags = " ".join(initial_flags)
 
         self._logger.debug(f"creating Flags with initial flags " f"{initial_flags}")
 
         self._flags = {}
         self.flags = initial_flags
```

### Comparing `remotemanager-0.9.7/remotemanager/utils/version.py` & `remotemanager-0.9.8/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.7/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.8/remotemanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.7
+Version: 0.9.8
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.7/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.8/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

