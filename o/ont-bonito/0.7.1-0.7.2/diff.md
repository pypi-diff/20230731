# Comparing `tmp/ont-bonito-0.7.1.tar.gz` & `tmp/ont-bonito-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-bonito-0.7.1.tar", last modified: Thu Jun  1 13:10:26 2023, max compression
+gzip compressed data, was "ont-bonito-0.7.2.tar", last modified: Mon Jul 31 15:01:21 2023, max compression
```

## Comparing `ont-bonito-0.7.1.tar` & `ont-bonito-0.7.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.335109 ont-bonito-0.7.1/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    14470 2023-04-05 10:36:21.000000 ont-bonito-0.7.1/LICENCE.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      179 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/MANIFEST.in
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5127 2023-06-01 13:10:26.331505 ont-bonito-0.7.1/PKG-INFO
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4821 2023-04-03 12:37:54.000000 ont-bonito-0.7.1/README.md
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.083858 ont-bonito-0.7.1/bonito/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      937 2023-06-01 12:51:57.000000 ont-bonito-0.7.1/bonito/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1550 2022-01-09 17:00:34.000000 ont-bonito-0.7.1/bonito/aligner.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.156103 ont-bonito-0.7.1/bonito/cli/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/cli/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7975 2023-05-31 13:55:48.000000 ont-bonito-0.7.1/bonito/cli/basecaller.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5096 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/cli/convert.py
--rwxr-xr-x   0 cseymour  (5744) domain users  (1113)     4773 2023-05-31 13:55:48.000000 ont-bonito-0.7.1/bonito/cli/download.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    12570 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/cli/duplex.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3647 2022-02-13 12:34:47.000000 ont-bonito-0.7.1/bonito/cli/evaluate.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     6815 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/cli/export.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4704 2023-05-05 09:40:35.000000 ont-bonito-0.7.1/bonito/cli/train.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      567 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/cli/view.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.185212 ont-bonito-0.7.1/bonito/crf/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/crf/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2627 2023-04-04 08:37:25.000000 ont-bonito-0.7.1/bonito/crf/basecall.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     8951 2023-04-13 14:08:39.000000 ont-bonito-0.7.1/bonito/crf/model.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.210045 ont-bonito-0.7.1/bonito/ctc/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/ctc/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2018 2022-02-13 12:34:47.000000 ont-bonito-0.7.1/bonito/ctc/basecall.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7110 2022-11-17 14:06:33.000000 ont-bonito-0.7.1/bonito/ctc/model.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.221146 ont-bonito-0.7.1/bonito/data/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       95 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/data/README.md
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2868 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/data.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     6672 2023-05-31 13:47:00.000000 ont-bonito-0.7.1/bonito/fast5.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    19373 2023-04-03 09:38:52.000000 ont-bonito-0.7.1/bonito/io.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3067 2022-06-11 12:11:56.000000 ont-bonito-0.7.1/bonito/mod_util.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.232862 ont-bonito-0.7.1/bonito/models/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      115 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/models/README.md
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.264946 ont-bonito-0.7.1/bonito/models/configs/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1206 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v1.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1289 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v2.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      290 2021-10-27 17:31:48.000000 ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v3.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7948 2021-12-03 16:22:18.000000 ont-bonito-0.7.1/bonito/multiprocessing.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    11194 2023-01-27 13:44:25.000000 ont-bonito-0.7.1/bonito/nn.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4718 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/pod5.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4550 2023-04-13 14:08:39.000000 ont-bonito-0.7.1/bonito/reader.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3330 2021-11-22 13:56:15.000000 ont-bonito-0.7.1/bonito/schedule.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    10481 2023-04-13 14:08:39.000000 ont-bonito-0.7.1/bonito/training.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    13024 2023-01-05 13:16:22.000000 ont-bonito-0.7.1/bonito/util.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.319405 ont-bonito-0.7.1/ont_bonito.egg-info/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5127 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/PKG-INFO
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      987 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/SOURCES.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/dependency_links.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       40 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/entry_points.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      261 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/requires.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)        7 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/top_level.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      304 2023-04-13 14:09:16.000000 ont-bonito-0.7.1/requirements.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       38 2023-06-01 13:10:26.338927 ont-bonito-0.7.1/setup.cfg
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1270 2022-09-05 12:28:38.000000 ont-bonito-0.7.1/setup.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.250695 ont-bonito-0.7.2/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    14470 2023-04-05 10:36:21.000000 ont-bonito-0.7.2/LICENCE.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      179 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/MANIFEST.in
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5078 2023-07-31 15:01:21.249514 ont-bonito-0.7.2/PKG-INFO
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4772 2023-07-31 13:06:29.000000 ont-bonito-0.7.2/README.md
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.141961 ont-bonito-0.7.2/bonito/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      937 2023-07-31 13:05:49.000000 ont-bonito-0.7.2/bonito/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       31 2023-06-30 15:20:06.000000 ont-bonito-0.7.2/bonito/__main__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1550 2022-01-09 17:00:34.000000 ont-bonito-0.7.2/bonito/aligner.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.181617 ont-bonito-0.7.2/bonito/cli/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/cli/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7975 2023-05-31 13:55:48.000000 ont-bonito-0.7.2/bonito/cli/basecaller.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5152 2023-07-31 13:56:55.000000 ont-bonito-0.7.2/bonito/cli/convert.py
+-rwxr-xr-x   0 cseymour  (5744) domain users  (1113)     4773 2023-05-31 13:55:48.000000 ont-bonito-0.7.2/bonito/cli/download.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    12570 2023-04-01 22:07:04.000000 ont-bonito-0.7.2/bonito/cli/duplex.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3647 2022-02-13 12:34:47.000000 ont-bonito-0.7.2/bonito/cli/evaluate.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6898 2023-06-30 15:20:06.000000 ont-bonito-0.7.2/bonito/cli/export.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4704 2023-05-05 09:40:35.000000 ont-bonito-0.7.2/bonito/cli/train.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      567 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/cli/view.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.196938 ont-bonito-0.7.2/bonito/crf/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/crf/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2632 2023-06-30 15:20:06.000000 ont-bonito-0.7.2/bonito/crf/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     8951 2023-04-13 14:08:39.000000 ont-bonito-0.7.2/bonito/crf/model.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.206949 ont-bonito-0.7.2/bonito/ctc/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/ctc/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2018 2022-02-13 12:34:47.000000 ont-bonito-0.7.2/bonito/ctc/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7110 2022-11-17 14:06:33.000000 ont-bonito-0.7.2/bonito/ctc/model.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.210483 ont-bonito-0.7.2/bonito/data/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       95 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/data/README.md
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2868 2023-04-01 22:07:04.000000 ont-bonito-0.7.2/bonito/data.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6672 2023-05-31 13:47:00.000000 ont-bonito-0.7.2/bonito/fast5.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    19373 2023-04-03 09:38:52.000000 ont-bonito-0.7.2/bonito/io.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3110 2023-06-06 12:50:58.000000 ont-bonito-0.7.2/bonito/mod_util.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.213206 ont-bonito-0.7.2/bonito/models/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      115 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/models/README.md
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.226975 ont-bonito-0.7.2/bonito/models/configs/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1206 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/models/configs/dna_r9.4.1@v1.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1289 2021-10-27 17:31:47.000000 ont-bonito-0.7.2/bonito/models/configs/dna_r9.4.1@v2.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      290 2021-10-27 17:31:48.000000 ont-bonito-0.7.2/bonito/models/configs/dna_r9.4.1@v3.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7948 2021-12-03 16:22:18.000000 ont-bonito-0.7.2/bonito/multiprocessing.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    11194 2023-01-27 13:44:25.000000 ont-bonito-0.7.2/bonito/nn.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4718 2023-04-01 22:07:04.000000 ont-bonito-0.7.2/bonito/pod5.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4550 2023-04-13 14:08:39.000000 ont-bonito-0.7.2/bonito/reader.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3330 2021-11-22 13:56:15.000000 ont-bonito-0.7.2/bonito/schedule.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    10481 2023-04-13 14:08:39.000000 ont-bonito-0.7.2/bonito/training.py
+-rwxr-xr-x   0 cseymour  (5744) domain users  (1113)    13291 2023-06-30 15:20:06.000000 ont-bonito-0.7.2/bonito/util.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-07-31 15:01:21.245270 ont-bonito-0.7.2/ont_bonito.egg-info/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5078 2023-07-31 15:01:20.000000 ont-bonito-0.7.2/ont_bonito.egg-info/PKG-INFO
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1006 2023-07-31 15:01:20.000000 ont-bonito-0.7.2/ont_bonito.egg-info/SOURCES.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2023-07-31 15:01:20.000000 ont-bonito-0.7.2/ont_bonito.egg-info/dependency_links.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       40 2023-07-31 15:01:20.000000 ont-bonito-0.7.2/ont_bonito.egg-info/entry_points.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      260 2023-07-31 15:01:20.000000 ont-bonito-0.7.2/ont_bonito.egg-info/requires.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        7 2023-07-31 15:01:20.000000 ont-bonito-0.7.2/ont_bonito.egg-info/top_level.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      303 2023-07-25 11:27:34.000000 ont-bonito-0.7.2/requirements.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       38 2023-07-31 15:01:21.251384 ont-bonito-0.7.2/setup.cfg
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1270 2022-09-05 12:28:38.000000 ont-bonito-0.7.2/setup.py
```

### Comparing `ont-bonito-0.7.1/LICENCE.txt` & `ont-bonito-0.7.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/PKG-INFO` & `ont-bonito-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-bonito
-Version: 0.7.1
+Version: 0.7.2
 Summary: UNKNOWN
 Home-page: https://github.com/nanoporetech/bonito
 Author: Oxford Nanopore Technologies, Ltd
 Author-email: support@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -80,16 +80,15 @@
 
 ```bash
 $ git clone https://github.com/nanoporetech/bonito.git  # or fork first and clone that
 $ cd bonito
 $ python3 -m venv venv3
 $ source venv3/bin/activate
 (venv3) $ pip install --upgrade pip
-(venv3) $ pip install -r requirements.txt
-(venv3) $ python setup.py develop
+(venv3) $ pip install -e .
 ```
 
 ## Interface
 
  - `bonito view` - view a model architecture for a given `.toml` file and the number of parameters in the network.
  - `bonito train` - train a bonito model.
  - `bonito evaluate` - evaluate a model performance.
```

### Comparing `ont-bonito-0.7.1/README.md` & `ont-bonito-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 
 ```bash
 $ git clone https://github.com/nanoporetech/bonito.git  # or fork first and clone that
 $ cd bonito
 $ python3 -m venv venv3
 $ source venv3/bin/activate
 (venv3) $ pip install --upgrade pip
-(venv3) $ pip install -r requirements.txt
-(venv3) $ python setup.py develop
+(venv3) $ pip install -e .
 ```
 
 ## Interface
 
  - `bonito view` - view a model architecture for a given `.toml` file and the number of parameters in the network.
  - `bonito train` - train a bonito model.
  - `bonito evaluate` - evaluate a model performance.
```

### Comparing `ont-bonito-0.7.1/bonito/aligner.py` & `ont-bonito-0.7.2/bonito/aligner.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/cli/basecaller.py` & `ont-bonito-0.7.2/bonito/cli/basecaller.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/cli/convert.py` & `ont-bonito-0.7.2/bonito/cli/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     )
     chunks, targets = zip(*tqdm(take(all_chunks, num_chunks), total=num_chunks))
     targets, target_lens = pad_lengths(targets) # convert refs from ragged arrray
     return ChunkDataSet(chunks, targets, target_lens)
 
 
 def validation_split(reads, num_valid=1000):
-    reads = np.random.permutation(sorted(reads.items()))
+    reads = np.random.permutation(np.array(sorted(reads.items()), dtype=object))
     return OrderedDict(reads[:-num_valid]), OrderedDict(reads[-num_valid:])
 
 
 def typical_indices(x, n=2.5):
     mu, sd = np.mean(x), np.std(x)
     idx, = np.where((mu - n*sd < x) & (x < mu + n*sd))
     return idx
@@ -106,21 +106,21 @@
     random.seed(args.seed)
     np.random.seed(args.seed)
 
     reads = h5py.File(args.chunkify_file, 'r')['Reads']
     training, validation = validation_split(reads, args.validation_reads)
 
     print("> preparing training chunks\n")
-    training_chunks = chunk_dataset(training, args.chunksize)
+    training_chunks = chunk_dataset(training, args.chunksize, len(training))
     training_indices = typical_indices(training_chunks.lengths)
     training_chunks = filter_chunks(training_chunks, np.random.permutation(training_indices))
     save_chunks(training_chunks, args.output_directory)
 
     print("\n> preparing validation chunks\n")
-    validation_chunks = chunk_dataset(validation, args.chunksize)
+    validation_chunks = chunk_dataset(validation, args.chunksize, len(validation))
     validation_indices = typical_indices(validation_chunks.lengths)
     validation_chunks = filter_chunks(validation_chunks, validation_indices)
     save_chunks(validation_chunks, os.path.join(args.output_directory, "validation"))
 
 
 def argparser():
     parser = ArgumentParser(
```

### Comparing `ont-bonito-0.7.1/bonito/cli/download.py` & `ont-bonito-0.7.2/bonito/cli/download.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/cli/duplex.py` & `ont-bonito-0.7.2/bonito/cli/duplex.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/cli/evaluate.py` & `ont-bonito-0.7.2/bonito/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/cli/export.py` & `ont-bonito-0.7.2/bonito/cli/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,22 +114,22 @@
     layer['size'] = layer['out_features']
     layer['activation'] = 'identity'
     del layer['in_features']
     del layer['out_features']
     return layer
 
 
-def to_guppy_dict(model, include_weights=True, binary_weights=True):
+def to_guppy_dict(model, include_weights=True, binary_weights=True, v4=True):
     guppy_dict = bonito.nn.to_dict(model.encoder, include_weights=include_weights)
     guppy_dict['sublayers'] = [x for x in guppy_dict['sublayers'] if x['type'] != 'permute']
     guppy_dict['sublayers'] = [dict(x, type='LSTM', activation='tanh', gate='sigmoid') if x['type'] == 'lstm' else x for x in guppy_dict['sublayers']]
     guppy_dict['sublayers'] = [dict(x, padding=(x['padding'], x['padding'])) if x['type'] == 'convolution' else x for x in guppy_dict['sublayers']]
     guppy_dict['sublayers'] = [to_guppy_feed_forward(x) if x['type'] == 'linear' else x for x in guppy_dict['sublayers']]
     idx = -1 if guppy_dict['sublayers'][-1]['type'] == 'linearcrfencoder' else -2
-    guppy_dict['sublayers'][idx] = reformat_output_layer(guppy_dict['sublayers'][idx])
+    guppy_dict['sublayers'][idx] = reformat_output_layer(guppy_dict['sublayers'][idx], v4=v4)
 
     if binary_weights:
         for layer_dict in guppy_dict['sublayers']:
             if 'params' in layer_dict:
                 layer_dict['params'] = {
                     f'{k}_binary': base64.b64encode(v.data.detach().numpy().astype(np.float32).tobytes()) for (k, v) in layer_dict['params'].items()
                 }
@@ -151,15 +151,16 @@
 
     if args.fuse_bn:
         # model weights might be saved in half when training and PyTorch's bn fusion
         # code uses an op (rsqrt) that currently (1.11) only has a float implementation
         model = model.to(torch.float32).apply(fuse_bn_)
 
     if args.format == 'guppy':
-        jsn = to_guppy_dict(model)
+        v4 = True if 'type' in config['encoder'] else False
+        jsn = to_guppy_dict(model, v4=v4)
         jsn["md5sum"] = file_md5(model_file)
         json.dump(jsn, sys.stdout, cls=JsonEncoder)
     elif args.format == 'dorado':
         for name, tensor in model.encoder.state_dict().items():
             save_tensor(args.model, name, tensor)
     elif args.format == 'torchscript':
         tmp_tensor = torch.rand(10, 1, 1000)
```

### Comparing `ont-bonito-0.7.1/bonito/cli/train.py` & `ont-bonito-0.7.2/bonito/cli/train.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/cli/view.py` & `ont-bonito-0.7.2/bonito/cli/view.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/crf/basecall.py` & `ont-bonito-0.7.2/bonito/crf/basecall.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 def basecall(model, reads, chunksize=4000, overlap=100, batchsize=32,
              reverse=False, rna=False):
     """
     Basecalls a set of reads.
     """
     chunks = thread_iter(
-        ((read, 0, len(read.signal)), chunk(torch.from_numpy(read.signal), chunksize, overlap))
+        ((read, 0, read.signal.shape[-1]), chunk(torch.from_numpy(read.signal), chunksize, overlap))
         for read in reads
     )
 
     batches = thread_iter(batchify(chunks, batchsize=batchsize))
 
     scores = thread_iter(
         (read, compute_scores(model, batch, reverse=reverse)) for read, batch in batches
```

### Comparing `ont-bonito-0.7.1/bonito/crf/model.py` & `ont-bonito-0.7.2/bonito/crf/model.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/ctc/basecall.py` & `ont-bonito-0.7.2/bonito/ctc/basecall.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/ctc/model.py` & `ont-bonito-0.7.2/bonito/ctc/model.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/data.py` & `ont-bonito-0.7.2/bonito/data.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/fast5.py` & `ont-bonito-0.7.2/bonito/fast5.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/io.py` & `ont-bonito-0.7.2/bonito/io.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/mod_util.py` & `ont-bonito-0.7.2/bonito/mod_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         return load_model(
             pore=pore,
             basecall_model_type=bc_model_subtype,
             basecall_model_version=model_version,
             modified_bases=mod_bases,
             quiet=True,
             device=device,
+            eval_only=True
         )
-    return load_model(model_path, quiet=True, device=device)
+    return load_model(model_path, quiet=True, device=device, eval_only=True)
 
 
 def mods_tags_to_str(mods_tags):
     return [
         f"MM:Z:{mods_tags[0]}",
         f"ML:B:C,{','.join(map(str, mods_tags[1]))}"
     ]
```

### Comparing `ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v1.toml` & `ont-bonito-0.7.2/bonito/models/configs/dna_r9.4.1@v1.toml`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v2.toml` & `ont-bonito-0.7.2/bonito/models/configs/dna_r9.4.1@v2.toml`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/multiprocessing.py` & `ont-bonito-0.7.2/bonito/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/nn.py` & `ont-bonito-0.7.2/bonito/nn.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/pod5.py` & `ont-bonito-0.7.2/bonito/pod5.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/reader.py` & `ont-bonito-0.7.2/bonito/reader.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/schedule.py` & `ont-bonito-0.7.2/bonito/schedule.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/training.py` & `ont-bonito-0.7.2/bonito/training.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.1/bonito/util.py` & `ont-bonito-0.7.2/bonito/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,26 +149,30 @@
             return {line.strip().split()[idx] for line in tsv.readlines()}
 
 
 def chunk(signal, chunksize, overlap):
     """
     Convert a read into overlapping chunks before calling
     """
-    T = signal.shape[0]
+    if signal.ndim == 1:
+        signal = signal.unsqueeze(0)
+    T = signal.shape[-1]
     if chunksize == 0:
         chunks = signal[None, :]
     elif T < chunksize:
         n, overhang = divmod(chunksize, T)
-        chunks = torch.cat((signal.repeat(n), signal[:overhang]))[None, :]
+        # np.tile operates only on dimension -1 by default, 
+        # whereas torch.repeat requires explicit listing of all input dimensions eg (1,n) or (1,1,n)
+        chunks = torch.cat((torch.from_numpy(np.tile(signal,n)), signal[...,:overhang]), dim=-1)[None, :]
     else:
         stub = (T - overlap) % (chunksize - overlap)
-        chunks = signal[stub:].unfold(0, chunksize, chunksize - overlap)
+        chunks = signal[...,stub:].unfold(-1, chunksize, chunksize - overlap).movedim(-2,0)
         if stub > 0:
-            chunks = torch.cat([signal[None, :chunksize], chunks], dim=0)
-    return chunks.unsqueeze(1)
+            chunks = torch.cat([signal[None, ..., :chunksize], chunks], dim=0)
+    return chunks
 
 
 def stitch(chunks, chunksize, overlap, length, stride, reverse=False):
     """
     Stitch chunks together with a given overlap
     """
     if chunks.shape[0] == 1: return chunks.squeeze(0)
```

### Comparing `ont-bonito-0.7.1/ont_bonito.egg-info/PKG-INFO` & `ont-bonito-0.7.2/ont_bonito.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-bonito
-Version: 0.7.1
+Version: 0.7.2
 Summary: UNKNOWN
 Home-page: https://github.com/nanoporetech/bonito
 Author: Oxford Nanopore Technologies, Ltd
 Author-email: support@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -80,16 +80,15 @@
 
 ```bash
 $ git clone https://github.com/nanoporetech/bonito.git  # or fork first and clone that
 $ cd bonito
 $ python3 -m venv venv3
 $ source venv3/bin/activate
 (venv3) $ pip install --upgrade pip
-(venv3) $ pip install -r requirements.txt
-(venv3) $ python setup.py develop
+(venv3) $ pip install -e .
 ```
 
 ## Interface
 
  - `bonito view` - view a model architecture for a given `.toml` file and the number of parameters in the network.
  - `bonito train` - train a bonito model.
  - `bonito evaluate` - evaluate a model performance.
```

### Comparing `ont-bonito-0.7.1/ont_bonito.egg-info/SOURCES.txt` & `ont-bonito-0.7.2/ont_bonito.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE.txt
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 bonito/__init__.py
+bonito/__main__.py
 bonito/aligner.py
 bonito/data.py
 bonito/fast5.py
 bonito/io.py
 bonito/mod_util.py
 bonito/multiprocessing.py
 bonito/nn.py
```

### Comparing `ont-bonito-0.7.1/setup.py` & `ont-bonito-0.7.2/setup.py`

 * *Files identical despite different names*

