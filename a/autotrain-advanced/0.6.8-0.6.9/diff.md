# Comparing `tmp/autotrain-advanced-0.6.8.tar.gz` & `tmp/autotrain-advanced-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.8.tar", last modified: Wed Jul 26 15:06:32 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.9.tar", last modified: Wed Jul 26 19:06:38 2023, max compression
```

## Comparing `autotrain-advanced-0.6.8.tar` & `autotrain-advanced-0.6.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.374771 autotrain-advanced-0.6.8/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.8/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 15:06:32.374771 autotrain-advanced-0.6.8/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.8/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 15:06:32.374771 autotrain-advanced-0.6.8/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.8/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.370771 autotrain-advanced-0.6.8/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.370771 autotrain-advanced-0.6.8/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 15:06:21.000000 autotrain-advanced-0.6.8/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37656 2023-07-26 15:05:24.000000 autotrain-advanced-0.6.8/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.370771 autotrain-advanced-0.6.8/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.8/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.8/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.8/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.8/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2618 2023-07-26 14:01:59.000000 autotrain-advanced-0.6.8/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.8/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.8/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.370771 autotrain-advanced-0.6.8/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.8/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17232 2023-07-26 14:08:33.000000 autotrain-advanced-0.6.8/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.370771 autotrain-advanced-0.6.8/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.8/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.8/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.8/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.8/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.8/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8237 2023-07-26 14:21:44.000000 autotrain-advanced-0.6.8/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.8/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.8/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.370771 autotrain-advanced-0.6.8/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/clm.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.374771 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13667 2023-07-26 14:28:19.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/main.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21311 2023-07-26 12:28:59.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13240 2023-07-26 12:29:40.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.8/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 15:06:32.374771 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 15:06:32.000000 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 15:06:32.000000 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 15:06:32.000000 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 15:06:32.000000 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 15:06:32.000000 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 15:06:32.000000 autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.9/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.9/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.9/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.415821 autotrain-advanced-0.6.9/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.415821 autotrain-advanced-0.6.9/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 19:06:29.000000 autotrain-advanced-0.6.9/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37885 2023-07-26 16:39:39.000000 autotrain-advanced-0.6.9/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.415821 autotrain-advanced-0.6.9/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.9/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.9/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.9/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.9/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2618 2023-07-26 14:01:59.000000 autotrain-advanced-0.6.9/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.9/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.9/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.9/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17232 2023-07-26 14:08:33.000000 autotrain-advanced-0.6.9/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.9/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.9/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.9/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.9/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.9/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8237 2023-07-26 14:21:44.000000 autotrain-advanced-0.6.9/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.9/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.9/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/clm.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13704 2023-07-26 19:04:47.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/main.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21393 2023-07-26 19:05:58.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13240 2023-07-26 12:29:40.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.9/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 19:06:38.419821 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 19:06:38.000000 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 19:06:38.000000 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 19:06:38.000000 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 19:06:38.000000 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 19:06:38.000000 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 19:06:38.000000 autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.8/LICENSE` & `autotrain-advanced-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/PKG-INFO` & `autotrain-advanced-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.8
+Version: 0.6.9
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.8/setup.py` & `autotrain-advanced-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/__init__.py` & `autotrain-advanced-0.6.9/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 # os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
```

### Comparing `autotrain-advanced-0.6.8/src/autotrain/app.py` & `autotrain-advanced-0.6.9/src/autotrain/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,20 +338,30 @@
         hub_models = list(hub_models1) + list(hub_models2)
     elif task == "lm_training":
         hub_models = list(list_models(filter="text-generation", sort="downloads", direction=-1, limit=100))
     elif task == "image_multi_class_classification":
         hub_models = list(list_models(filter="image-classification", sort="downloads", direction=-1, limit=100))
     elif task == "dreambooth":
         hub_models = list(list_models(filter="text-to-image", sort="downloads", direction=-1, limit=100))
-        hub_models = ["stabilityai/stable-diffusion-xl-base-1.0"] + hub_models
     else:
         raise NotImplementedError
     # sort by number of downloads in descending order
     hub_models = [{"id": m.modelId, "downloads": m.downloads} for m in hub_models if m.private is False]
     hub_models = sorted(hub_models, key=lambda x: x["downloads"], reverse=True)
+
+    if task == "dreambooth":
+        choices = ["stabilityai/stable-diffusion-xl-base-1.0"] + [m["id"] for m in hub_models]
+        value = choices[0]
+        return gr.Dropdown.update(
+            choices=choices,
+            value=value,
+            visible=True,
+            interactive=True,
+        )
+
     return gr.Dropdown.update(
         choices=[m["id"] for m in hub_models],
         value=hub_models[0]["id"],
         visible=True,
         interactive=True,
     )
```

### Comparing `autotrain-advanced-0.6.8/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.9/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.9/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.6.9/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.9/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.9/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/dataset.py` & `autotrain-advanced-0.6.9/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/help.py` & `autotrain-advanced-0.6.9/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.9/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/params.py` & `autotrain-advanced-0.6.9/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.9/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.9/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.9/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.9/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/project.py` & `autotrain-advanced-0.6.9/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/tasks.py` & `autotrain-advanced-0.6.9/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/main.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,11 +348,12 @@
         warmup_steps=0,
         num_steps=job_config.num_steps,
         revision=None,
         push_to_hub=True,
         hub_model_id=f"{repo_user}/{repo_name}",
         xl=xl,
         prompt=concept_prompts,
+        hub_token=huggingface_token,
     )
     train(args)
 
     _ = co2_tracker.stop()
```

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,22 +437,24 @@
         self.accelerator.end_training()
 
     def push_to_hub(self):
         repo_id = create_repo(
             repo_id=self.config.hub_model_id,
             exist_ok=True,
             private=True,
+            token=self.config.hub_token,
         ).repo_id
 
         utils.create_model_card(
             repo_id,
             base_model=self.config.model,
             train_text_encoder=self.config.train_text_encoder,
             prompt=self.config.prompt,
             repo_folder=self.config.output,
         )
         upload_folder(
             repo_id=repo_id,
             folder_path=self.config.output,
             commit_message="End of training",
             ignore_patterns=["step_*", "epoch_*"],
+            token=self.config.hub_token,
         )
```

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.9/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain/utils.py` & `autotrain-advanced-0.6.9/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.8
+Version: 0.6.9
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.8/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.9/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

