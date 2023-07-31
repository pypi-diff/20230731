# Comparing `tmp/SciFiReaders-0.0.9.tar.gz` & `tmp/SciFiReaders-0.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciFiReaders-0.0.9.tar", last modified: Fri Apr 28 20:58:44 2023, max compression
+gzip compressed data, was "SciFiReaders-0.10.0.tar", last modified: Mon Jul 31 20:55:27 2023, max compression
```

## Comparing `SciFiReaders-0.0.9.tar` & `SciFiReaders-0.10.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.637819 SciFiReaders-0.0.9/SciFiReaders/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/SID/
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/SID/Nsid_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/SID/Usid_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/SID/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/converters/hyperspy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/generic/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/dm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/emd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/nion_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/stem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/stem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/ion/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/ion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20352 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/mdt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/pifm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/SpeReader.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 20:58:44.645819 SciFiReaders-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.403321 SciFiReaders-0.10.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-31 20:55:27.403321 SciFiReaders-0.10.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/SID/
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/SID/Nsid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/SID/Usid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/SID/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/converters/hyperspy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/generic/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/dm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/emd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/nion_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/stem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/stem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/ion/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/ion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.403321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/mdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/pifm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.403321 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25193 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.403321 SciFiReaders-0.10.0/SciFiReaders/readers/spectroscopy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/spectroscopy/SpeReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 20:53:01.000000 SciFiReaders-0.10.0/SciFiReaders/readers/spectroscopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:55:27.399321 SciFiReaders-0.10.0/SciFiReaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-31 20:55:27.000000 SciFiReaders-0.10.0/SciFiReaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-31 20:55:27.000000 SciFiReaders-0.10.0/SciFiReaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:55:27.000000 SciFiReaders-0.10.0/SciFiReaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 20:55:27.000000 SciFiReaders-0.10.0/SciFiReaders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 20:55:27.000000 SciFiReaders-0.10.0/SciFiReaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 20:55:27.403321 SciFiReaders-0.10.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-31 20:53:02.000000 SciFiReaders-0.10.0/setup.py
```

### Comparing `SciFiReaders-0.0.9/LICENSE` & `SciFiReaders-0.10.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/PKG-INFO` & `SciFiReaders-0.10.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciFiReaders
-Version: 0.0.9
+Version: 0.10.0
 Summary: Tools for extracting data and metadata from scientific data files
 Home-page: https://pycroscopy.github.io/SciFiReaders/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific
 Platform: Linux
@@ -13,24 +13,22 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides-Extra: hyperspy
-Provides-Extra: igor
+Provides-Extra: igor2
 Provides-Extra: gwyddion
-Provides-Extra: nanonispy
 Provides-Extra: sid
 Provides-Extra: image
 License-File: LICENSE
 
 SciFiReaders
 ============
```

### Comparing `SciFiReaders-0.0.9/README.rst` & `SciFiReaders-0.10.0/README.rst`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/ingestor.py` & `SciFiReaders-0.10.0/SciFiReaders/ingestor.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/SID/Nsid_reader.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/SID/Nsid_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/SID/Usid_reader.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/SID/Usid_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/converters/hyperspy.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/converters/hyperspy.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/generic/image.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/generic/image.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/dm_reader.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/dm_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
                                                                 dimension_type=sidpy.DimensionType.SPECTRAL))
             elif '1/' in units or units in ['mrad', 'rad']:
                 dataset.set_dimension(int(dim), sidpy.Dimension(values, name=reciprocal_name, units=units,
                                                                 quantity='reciprocal distance',
                                                                 dimension_type=sidpy.DimensionType.RECIPROCAL))
                 reciprocal_name = chr(ord(reciprocal_name) + 1)
             elif 'm' in units:
-                units = 'counts'
+                # units = 'counts'
                 dataset.set_dimension(int(dim), sidpy.Dimension(values, name=spatial_name, units=units,
                                                                 quantity='distance',
                                                                 dimension_type=sidpy.DimensionType.SPATIAL))
                 spatial_name = chr(ord(spatial_name) + 1)
             else:
                 units = 'frame'
                 dataset.set_dimension(int(dim), sidpy.Dimension(values, name=spatial_name, units=units,
```

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/emd_reader.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/emd_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/nion_reader.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/em/tem/nion_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/base_utils.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/base_utils.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 import numpy as np  # For array operations
 import sidpy as sid
 from sidpy.sid import Reader
 import re
 from warnings import warn
 
 try:
-    from igor import binarywave as bw
+    from igor2 import binarywave as bw
 except ModuleNotFoundError:
-    print("You don't have igor installed. \
+    print("You don't have igor2 installed. \
     If you wish to open igor files, you will need to install it \
-    (pip install igor) before attempting.")
+    (pip install igor2) before attempting.")
     bw = None
 
 class IgorMatrixReader(Reader):
     """
     Extracts data and metadata from Igor Binary Wave (.ibw) files exported from MatrixFiles
     This is a very specific reader that cannot be reconciled with the generic ibw reader due to severe inconsistencies.
     Unless you exported Matrix files as ibw files using IGOR5 Exporter v120401, this reader will not work.
     """
     def __init__(self, file_path, *args, **kwargs):
         if bw == None:
-            raise ModuleNotFoundError('You attempted to load an Igor file, but this requires igor.\n \
-            Please Load it with pip install igor , restart and retry')
+            raise ModuleNotFoundError('You attempted to load an Igor file, but this requires igor2.\n \
+            Please Load it with pip install igor2 , restart and retry')
 
         super().__init__(file_path, *args, **kwargs)
 
     def read(self, verbose=False, parm_encoding='utf-8'):
         """
         Reads the file given in file_path into a sidpy dataset
 
@@ -257,16 +257,16 @@
 class IgorIBWReader(Reader):
     """
     Extracts data and metadata from Igor Binary Wave (.ibw) files containing
     images or force curves
     """
     def __init__(self, file_path, *args, **kwargs):
         if bw == None:
-            raise ModuleNotFoundError('You attempted to load an Igor file, but this requires igor.\n \
-            Please Load it with pip install igor , restart and retry')
+            raise ModuleNotFoundError('You attempted to load an Igor file, but this requires igor2.\n \
+            Please Load it with pip install igor2 , restart and retry')
 
         super().__init__(file_path, *args, **kwargs)
 
     def read(self, verbose=False, parm_encoding='utf-8'):
         """
         Reads the file given in file_path into a sidpy dataset
```

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/mdt.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/mdt.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/pifm.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/afm/pifm.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,19 @@
 
 @author: Rama Vasudevan
 """
 
 import numpy as np  # For array operations
 import sidpy as sid
 from sidpy.sid import Reader, Dimension, DimensionType
-
-try:
-    import nanonispy as nap
-except ModuleNotFoundError:
-    nap = None
-
-
+from .nanonis_base import Grid
 class Nanonis3dsReader(Reader):
 
     def __init__(self, file_path, *args, **kwargs):
-        if nap == None:
-            raise ModuleNotFoundError('You attempted to load a Nanonis file, but this requires Nanonispy.\n \
-            Please Load it with pip install nanonispy , restart and retry')
+
         super().__init__(file_path, *args, **kwargs)
 
     @staticmethod
     def _parse_3ds_parms(header_dict, signal_dict):
         """
         Parse 3ds files.
         Parameters
@@ -120,15 +112,15 @@
     def read(self):
         """
         Returns
         -------
         list of sidpy.Dataset objects containing the spectroscopy data
         """
         
-        reader = nap.read.Grid
+        reader = Grid
         override_header = {
             'Delay before measuring (s)': 0.0,
             'Start time': 0.0,
             'End time': 1000.0,
             'Comment': 'Default values for delay before measuring (s), Start time and End time fields were used! Beware!'
         }
         nanonis_data = reader(self._input_file_path, header_override=override_header)
@@ -190,11 +182,9 @@
 
     def can_read(self):
         """
         Tests whether or not the provided file has a .3ds extension
         Returns
         -------
         """
-    
-        if nap is None:
-            return False
-        return super(Nanonis3dsReader, self).can_read(extension='3ds')
+
+        return
```

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,18 @@
 Created on Fri Nov 5 16:43:00 2021
 
 @author: Rama Vasudevan
 """
 import numpy as np  # For array operations
 import sidpy as sid
 from sidpy.sid import Reader, Dimension, DimensionType
-
-try:
-    import nanonispy as nap
-except ModuleNotFoundError:
-    nap = None
-
+from .nanonis_base import Scan
 class NanonisSXMReader(Reader):
 
     def __init__(self, file_path, *args, **kwargs):
-        if nap == None:
-            raise ModuleNotFoundError('You attempted to load a Nanonis file, but this requires Nanonispy.\n \
-            Please Load it with pip install nanonispy , restart and retry')
         super().__init__(file_path, *args, **kwargs)
 
     @staticmethod
     def _parse_sxm_parms(header_dict, signal_dict):
         """
         Parse sxm files.
         Parameters
@@ -94,15 +86,15 @@
         Thus returning a list of length N where N is the number of channels.
 
         Returns
         -------
         dataset_list: (list) of sidpy.Dataset objects
         """
        
-        reader = nap.read.Scan
+        reader = Scan
        
         nanonis_data = reader(self._input_file_path)
 
         header_dict = nanonis_data.header
         signal_dict = nanonis_data.signals
 
         parm_dict, data_dict = self._parse_sxm_parms(header_dict,
@@ -153,11 +145,9 @@
 
     def can_read(self):
         """
         Tests whether or not the provided file has a .dm3 extension
         Returns
         -------
         """
-        # TODO: Add dat eventually
-        if nap is None:
-            return False
-        return super(NanonisSXMReader, self).can_read(extension='sxm')
+       
+        return
```

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/SpeReader.py` & `SciFiReaders-0.10.0/SciFiReaders/readers/spectroscopy/SpeReader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.9/SciFiReaders.egg-info/PKG-INFO` & `SciFiReaders-0.10.0/SciFiReaders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciFiReaders
-Version: 0.0.9
+Version: 0.10.0
 Summary: Tools for extracting data and metadata from scientific data files
 Home-page: https://pycroscopy.github.io/SciFiReaders/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific
 Platform: Linux
@@ -13,24 +13,22 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides-Extra: hyperspy
-Provides-Extra: igor
+Provides-Extra: igor2
 Provides-Extra: gwyddion
-Provides-Extra: nanonispy
 Provides-Extra: sid
 Provides-Extra: image
 License-File: LICENSE
 
 SciFiReaders
 ============
```

### Comparing `SciFiReaders-0.0.9/SciFiReaders.egg-info/SOURCES.txt` & `SciFiReaders-0.10.0/SciFiReaders.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,12 +34,13 @@
 SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py
 SciFiReaders/readers/microscopy/spm/afm/gwyddion.py
 SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py
 SciFiReaders/readers/microscopy/spm/afm/mdt.py
 SciFiReaders/readers/microscopy/spm/afm/pifm.py
 SciFiReaders/readers/microscopy/spm/stm/__init__.py
 SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py
+SciFiReaders/readers/microscopy/spm/stm/nanonis_base.py
 SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py
 SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py
 SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py
 SciFiReaders/readers/spectroscopy/SpeReader.py
 SciFiReaders/readers/spectroscopy/__init__.py
```

### Comparing `SciFiReaders-0.0.9/setup.py` & `SciFiReaders-0.10.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     long_description = f.read()
 
 with open(os.path.join(here, 'SciFiReaders/__version__.py')) as f:
     __version__ = f.read().split("'")[1]
 
 # TODO: Move requirements to requirements.txt
 requirements = [  # basic
-                'numpy>=1.10',
+                'numpy==1.24.4',
                 'toolz',  # dask installation failing without this
                 'cytoolz',  # dask installation failing without this
                 'dask>=2.20.0',
                 'sidpy>=0.11.2',
-                'numba',
-                'ipython==7.1.0'
+                'numba==0.57.1',
+                'ipython>=7.1.0'
                 # generic:
                 # Reader specific ones go to extras
                ]
 
 setup(
     name='SciFiReaders',
     version=__version__,
@@ -32,15 +32,14 @@
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering :: Information Analysis'],
     keywords=['imaging', 'spectra', 'multidimensional', 'scientific'],
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*",
@@ -57,17 +56,16 @@
     test_suite='pytest',
     # dependency='',
     # dependency_links=[''],
     include_package_data=True,
     # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-dependencies
     extras_require={
         'hyperspy':  ["hyperspy"],
-        'igor': ["igor"],
+        'igor2': ["igor2"],
         "gwyddion": ["gwyfile"],
-        'nanonispy': ['nanonispy'],
         'sid': ['pyUSID', 'pyNSID'],
         'image': ['pillow', 'tifffile']
     },
     # If there are data files included in your packages that need to be
     # installed, specify them here.  If using Python 2.6 or less, then these
     # have to be included in MANIFEST.in as well.
     # package_data={
```

