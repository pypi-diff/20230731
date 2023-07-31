# Comparing `tmp/evrm-78.tar.gz` & `tmp/evrm-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evrm-78.tar", last modified: Mon Sep  6 21:38:30 2021, max compression
+gzip compressed data, was "dist/evrm-9.tar", last modified: Mon Jan 16 15:20:02 2017, max compression
```

## Comparing `evrm-78.tar` & `evrm-9.tar`

### file list

```diff
@@ -1,122 +1,110 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.304817 evrm-78/
--rw-r--r--   0 bart      (1000) bart      (1000)      165 2021-09-06 19:50:10.000000 evrm-78/MANIFEST.in
--rw-r--r--   0 bart      (1000) bart      (1000)     8406 2021-09-06 21:38:30.304817 evrm-78/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     6992 2021-09-06 19:50:10.000000 evrm-78/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.292817 evrm-78/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2692 2021-09-06 21:37:03.000000 evrm-78/bin/evrm
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.292817 evrm-78/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)     1736 2021-09-06 19:50:10.000000 evrm-78/docs/README
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.292817 evrm-78/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1000)      102 2021-09-06 19:50:10.000000 evrm-78/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      527 2021-09-06 19:50:10.000000 evrm-78/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      260 2021-09-06 19:50:10.000000 evrm-78/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2260 2021-09-06 19:50:10.000000 evrm-78/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7353 2021-09-06 19:50:10.000000 evrm-78/docs/index.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.296817 evrm-78/docs/jpg/
--rw-r--r--   0 bart      (1000) bart      (1000)   549426 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/20140730_011.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   262781 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/20151028_009.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   226554 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/20151029_004.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   106616 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/69389.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   270024 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/absoluut2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   538506 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/aes.ico
--rw-r--r--   0 bart      (1000) bart      (1000)    60226 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/aesculaap.ico
--rw-r--r--   0 bart      (1000) bart      (1000)   629595 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/bart.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   449410 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/bart2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    19832 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/besloten.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   210710 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/bewijsgif3.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   167276 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/dodelijk.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    70170 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/fact.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     6707 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/geinformeerd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   162702 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/gelijk2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   180602 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/haarmaken.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   566905 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/igz.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   715150 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/minister.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   448476 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/nalatig.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    25974 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/nederland.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    23206 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/nederland2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    13101 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/neurotoxisch.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   180812 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/stoned2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    32684 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/tussenkomst.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    17550 2021-09-06 19:50:10.000000 evrm-78/docs/jpg/verbod.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    23206 2021-09-06 19:50:10.000000 evrm-78/docs/nederland2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      199 2021-09-06 19:50:10.000000 evrm-78/docs/requirements.txt
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.300817 evrm-78/docs/txt/
--rw-r--r--   0 bart      (1000) bart      (1000)      379 2021-09-06 19:50:10.000000 evrm-78/docs/txt/BIJWERKING
--rw-r--r--   0 bart      (1000) bart      (1000)      105 2021-09-06 19:50:10.000000 evrm-78/docs/txt/CONTACT
--rw-r--r--   0 bart      (1000) bart      (1000)      222 2021-09-06 19:50:10.000000 evrm-78/docs/txt/DOPAMINE
--rw-r--r--   0 bart      (1000) bart      (1000)        0 2021-09-06 19:50:10.000000 evrm-78/docs/txt/MADS
--rw-r--r--   0 bart      (1000) bart      (1000)      355 2021-09-06 19:50:10.000000 evrm-78/docs/txt/ONTWENNING
--rw-r--r--   0 bart      (1000) bart      (1000)     1427 2021-09-06 19:50:10.000000 evrm-78/docs/txt/README.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1803 2021-09-06 19:50:10.000000 evrm-78/docs/txt/VERGIFTIGING
--rw-r--r--   0 bart      (1000) bart      (1000)   568504 2021-09-06 19:50:10.000000 evrm-78/docs/txt/Wetboek-van-Strafrecht.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     5576 2021-09-06 19:50:10.000000 evrm-78/docs/txt/WvGGZ.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   142614 2021-09-06 19:50:10.000000 evrm-78/docs/txt/WvGGZ.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     2599 2021-09-06 19:50:10.000000 evrm-78/docs/txt/aangifte.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      366 2021-09-06 19:50:10.000000 evrm-78/docs/txt/aantallen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       66 2021-09-06 19:50:10.000000 evrm-78/docs/txt/absoluut.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      737 2021-09-06 19:50:10.000000 evrm-78/docs/txt/bedreiging.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       63 2021-09-06 19:50:10.000000 evrm-78/docs/txt/beuker.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1234 2021-09-06 19:50:10.000000 evrm-78/docs/txt/bijwerkingen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      905 2021-09-06 19:50:10.000000 evrm-78/docs/txt/clozapine.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      293 2021-09-06 19:50:10.000000 evrm-78/docs/txt/contact.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      863 2021-09-06 19:50:10.000000 evrm-78/docs/txt/dodelijk.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      522 2021-09-06 19:50:10.000000 evrm-78/docs/txt/echt.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      696 2021-09-06 19:50:10.000000 evrm-78/docs/txt/ernstig.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1458 2021-09-06 19:50:10.000000 evrm-78/docs/txt/evrm.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     4496 2021-09-06 19:50:10.000000 evrm-78/docs/txt/fact.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      793 2021-09-06 19:50:10.000000 evrm-78/docs/txt/gif.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     8293 2021-09-06 19:50:10.000000 evrm-78/docs/txt/greffe.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1179 2021-09-06 19:50:10.000000 evrm-78/docs/txt/hoogeraad.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       44 2021-09-06 19:50:10.000000 evrm-78/docs/txt/igz.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      104 2021-09-06 19:50:10.000000 evrm-78/docs/txt/index.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       59 2021-09-06 19:50:10.000000 evrm-78/docs/txt/kamerbrief.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     4079 2021-09-06 19:50:10.000000 evrm-78/docs/txt/kamerbrief.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     2299 2021-09-06 19:50:10.000000 evrm-78/docs/txt/kamerbrief2.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2433 2021-09-06 19:50:10.000000 evrm-78/docs/txt/kamerbrief3.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      784 2021-09-06 19:50:10.000000 evrm-78/docs/txt/ld50.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      819 2021-09-06 19:50:10.000000 evrm-78/docs/txt/leven.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      422 2021-09-06 19:50:10.000000 evrm-78/docs/txt/loggen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       66 2021-09-06 19:50:10.000000 evrm-78/docs/txt/minister.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     4192 2021-09-06 19:50:10.000000 evrm-78/docs/txt/misdrijf.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2742 2021-09-06 19:50:10.000000 evrm-78/docs/txt/mishandeling.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    23206 2021-09-06 19:50:10.000000 evrm-78/docs/txt/nederland2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      778 2021-09-06 19:50:10.000000 evrm-78/docs/txt/om.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      551 2021-09-06 19:50:10.000000 evrm-78/docs/txt/oorzaak.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      621 2021-09-06 19:50:10.000000 evrm-78/docs/txt/opzet2.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1209 2021-09-06 19:50:10.000000 evrm-78/docs/txt/pad.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1779 2021-09-06 19:50:10.000000 evrm-78/docs/txt/receptoren.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1176 2021-09-06 19:50:10.000000 evrm-78/docs/txt/recht.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      956 2021-09-06 19:50:10.000000 evrm-78/docs/txt/risico.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      746 2021-09-06 19:50:10.000000 evrm-78/docs/txt/schadelijk.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      741 2021-09-06 19:50:10.000000 evrm-78/docs/txt/sedatie.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      111 2021-09-06 19:50:10.000000 evrm-78/docs/txt/strafrecht.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      237 2021-09-06 19:50:10.000000 evrm-78/docs/txt/symptomen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      844 2021-09-06 19:50:10.000000 evrm-78/docs/txt/todo.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2521 2021-09-06 19:50:10.000000 evrm-78/docs/txt/toxic.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       78 2021-09-06 19:50:10.000000 evrm-78/docs/txt/tussenkomst.rst
--rw-r--r--   0 bart      (1000) bart      (1000)       72 2021-09-06 19:50:10.000000 evrm-78/docs/txt/uitspraak.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     6494 2021-09-06 19:50:10.000000 evrm-78/docs/txt/urls.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      476 2021-09-06 19:50:10.000000 evrm-78/docs/txt/vergiftiging.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1383 2021-09-06 19:50:10.000000 evrm-78/docs/txt/vervolgen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1965 2021-09-06 19:50:10.000000 evrm-78/docs/txt/verzoek.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      803 2021-09-06 19:50:10.000000 evrm-78/docs/txt/wet.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2248 2021-09-06 19:50:10.000000 evrm-78/docs/txt/wvggz.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     4365 2021-09-06 19:50:10.000000 evrm-78/docs/txt/zyprexa.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.304817 evrm-78/evrm/
--rw-r--r--   0 bart      (1000) bart      (1000)        0 2021-09-06 19:50:10.000000 evrm-78/evrm/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)    10859 2021-09-06 19:57:17.000000 evrm-78/evrm/obj.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3436 2021-09-06 19:50:10.000000 evrm-78/evrm/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20227 2021-09-06 21:33:49.000000 evrm-78/evrm/run.py
--rw-r--r--   0 bart      (1000) bart      (1000)      251 2021-09-06 19:50:10.000000 evrm-78/evrm/slg.py
--rw-r--r--   0 bart      (1000) bart      (1000)    22431 2021-09-06 21:37:32.000000 evrm-78/evrm/sui.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3463 2021-09-06 19:50:10.000000 evrm-78/evrm/trt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      118 2021-09-06 19:50:10.000000 evrm-78/evrm/ver.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5813 2021-09-06 19:50:10.000000 evrm-78/evrm/wsd.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2021-09-06 21:38:30.304817 evrm-78/evrm.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     8406 2021-09-06 21:38:30.000000 evrm-78/evrm.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     2287 2021-09-06 21:38:30.000000 evrm-78/evrm.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2021-09-06 21:38:30.000000 evrm-78/evrm.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2021-09-06 21:38:30.000000 evrm-78/evrm.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2021-09-06 21:38:30.000000 evrm-78/evrm.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2021-09-06 21:38:30.304817 evrm-78/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)     1306 2021-09-06 21:34:38.000000 evrm-78/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1057 2017-01-16 15:04:21.000000 evrm-9/LICENSE
+-rw-r--r--   0 bart      (1000) bart      (1000)     3369 2017-01-16 15:07:37.000000 evrm-9/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/evrm/
+-rw-r--r--   0 bart      (1000) bart      (1000)      120 2017-01-16 15:08:09.000000 evrm-9/evrm/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      140 2017-01-16 15:04:21.000000 evrm-9/evrm/version.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    26386 2017-01-16 15:04:21.000000 evrm-9/evrm/stats.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/evrm.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2017-01-16 15:20:02.000000 evrm-9/evrm.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2017-01-16 15:20:02.000000 evrm-9/evrm.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     2063 2017-01-16 15:20:02.000000 evrm-9/evrm.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2017-01-16 15:13:52.000000 evrm-9/evrm.egg-info/not-zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)     1919 2017-01-16 15:20:02.000000 evrm-9/evrm.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2017-01-16 15:20:02.000000 evrm-9/evrm.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     1736 2017-01-16 15:04:21.000000 evrm-9/README
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      417 2017-01-16 15:13:23.000000 evrm-9/bin/evrm
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2225 2017-01-16 15:04:21.000000 evrm-9/docs/conf.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/docs/jpg/
+-rw-r--r--   0 bart      (1000) bart      (1000)   270024 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/absoluut2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   566905 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/igz.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    19832 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/besloten.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   715150 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/minister.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   448476 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/nalatig.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   106616 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/69389.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    23206 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/nederland2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   449410 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/bart2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    17550 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/verbod.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    70170 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/fact.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    25974 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/nederland.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   262781 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/20151028_009.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   549426 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/20140730_011.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    32684 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/tussenkomst.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   538506 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/aes.ico
+-rw-r--r--   0 bart      (1000) bart      (1000)   629595 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/bart.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    60226 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/aesculaap.ico
+-rw-r--r--   0 bart      (1000) bart      (1000)     6707 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/geinformeerd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   226554 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/20151029_004.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   162702 2017-01-16 15:04:21.000000 evrm-9/docs/jpg/gelijk2.jpg
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/docs/txt/
+-rw-r--r--   0 bart      (1000) bart      (1000)       72 2017-01-16 15:04:21.000000 evrm-9/docs/txt/uitspraak.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)       59 2017-01-16 15:04:21.000000 evrm-9/docs/txt/kamerbrief.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     6257 2017-01-16 15:04:21.000000 evrm-9/docs/txt/urls.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      621 2017-01-16 15:04:21.000000 evrm-9/docs/txt/opzet2.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      355 2017-01-16 15:04:21.000000 evrm-9/docs/txt/ONTWENNING
+-rw-r--r--   0 bart      (1000) bart      (1000)     1965 2017-01-16 15:04:21.000000 evrm-9/docs/txt/verzoek.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      105 2017-01-16 15:04:21.000000 evrm-9/docs/txt/CONTACT
+-rw-r--r--   0 bart      (1000) bart      (1000)        0 2017-01-16 15:04:21.000000 evrm-9/docs/txt/MADS
+-rw-r--r--   0 bart      (1000) bart      (1000)      422 2017-01-16 15:04:21.000000 evrm-9/docs/txt/loggen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1209 2017-01-16 15:04:21.000000 evrm-9/docs/txt/pad.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   142614 2017-01-16 15:04:21.000000 evrm-9/docs/txt/WvGGZ.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      746 2017-01-16 15:04:21.000000 evrm-9/docs/txt/schadelijk.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      222 2017-01-16 15:04:21.000000 evrm-9/docs/txt/DOPAMINE
+-rw-r--r--   0 bart      (1000) bart      (1000)      778 2017-01-16 15:04:21.000000 evrm-9/docs/txt/om.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      522 2017-01-16 15:04:21.000000 evrm-9/docs/txt/echt.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      819 2017-01-16 15:04:21.000000 evrm-9/docs/txt/leven.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     4079 2017-01-16 15:04:21.000000 evrm-9/docs/txt/kamerbrief.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     8293 2017-01-16 15:04:21.000000 evrm-9/docs/txt/greffe.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      737 2017-01-16 15:04:21.000000 evrm-9/docs/txt/bedreiging.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1803 2017-01-16 15:04:21.000000 evrm-9/docs/txt/VERGIFTIGING
+-rw-r--r--   0 bart      (1000) bart      (1000)       66 2017-01-16 15:04:21.000000 evrm-9/docs/txt/absoluut.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      905 2017-01-16 15:04:21.000000 evrm-9/docs/txt/clozapine.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1383 2017-01-16 15:04:21.000000 evrm-9/docs/txt/vervolgen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      237 2017-01-16 15:04:21.000000 evrm-9/docs/txt/symptomen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      696 2017-01-16 15:04:21.000000 evrm-9/docs/txt/ernstig.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      803 2017-01-16 15:04:21.000000 evrm-9/docs/txt/wet.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     3747 2017-01-16 15:04:21.000000 evrm-9/docs/txt/fact.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      863 2017-01-16 15:04:21.000000 evrm-9/docs/txt/dodelijk.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1779 2017-01-16 15:04:21.000000 evrm-9/docs/txt/receptoren.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)       78 2017-01-16 15:04:21.000000 evrm-9/docs/txt/tussenkomst.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)       63 2017-01-16 15:04:21.000000 evrm-9/docs/txt/beuker.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   568504 2017-01-16 15:04:21.000000 evrm-9/docs/txt/Wetboek-van-Strafrecht.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      956 2017-01-16 15:04:21.000000 evrm-9/docs/txt/risico.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     4365 2017-01-16 15:04:21.000000 evrm-9/docs/txt/zyprexa.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      551 2017-01-16 15:04:21.000000 evrm-9/docs/txt/oorzaak.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)       66 2017-01-16 15:04:21.000000 evrm-9/docs/txt/minister.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      844 2017-01-16 15:04:21.000000 evrm-9/docs/txt/todo.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      476 2017-01-16 15:04:21.000000 evrm-9/docs/txt/vergiftiging.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      383 2017-01-16 15:04:21.000000 evrm-9/docs/txt/contact.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1176 2017-01-16 15:04:21.000000 evrm-9/docs/txt/recht.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      366 2017-01-16 15:04:21.000000 evrm-9/docs/txt/aantallen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)       44 2017-01-16 15:04:21.000000 evrm-9/docs/txt/igz.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      104 2017-01-16 15:04:21.000000 evrm-9/docs/txt/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      379 2017-01-16 15:04:21.000000 evrm-9/docs/txt/BIJWERKING
+-rw-r--r--   0 bart      (1000) bart      (1000)     2599 2017-01-16 15:04:21.000000 evrm-9/docs/txt/aangifte.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2299 2017-01-16 15:04:21.000000 evrm-9/docs/txt/kamerbrief2.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      741 2017-01-16 15:04:21.000000 evrm-9/docs/txt/sedatie.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      111 2017-01-16 15:04:21.000000 evrm-9/docs/txt/strafrecht.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2248 2017-01-16 15:04:21.000000 evrm-9/docs/txt/wvggz.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1179 2017-01-16 15:04:21.000000 evrm-9/docs/txt/hoogeraad.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1458 2017-01-16 15:04:21.000000 evrm-9/docs/txt/evrm.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1427 2017-01-16 15:04:21.000000 evrm-9/docs/txt/README.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2433 2017-01-16 15:04:21.000000 evrm-9/docs/txt/kamerbrief3.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      793 2017-01-16 15:04:21.000000 evrm-9/docs/txt/gif.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2521 2017-01-16 15:04:21.000000 evrm-9/docs/txt/toxic.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     4192 2017-01-16 15:04:21.000000 evrm-9/docs/txt/misdrijf.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2742 2017-01-16 15:04:21.000000 evrm-9/docs/txt/mishandeling.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     5576 2017-01-16 15:04:21.000000 evrm-9/docs/txt/WvGGZ.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     7973 2017-01-16 15:15:38.000000 evrm-9/docs/index.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1000)      527 2017-01-16 15:04:21.000000 evrm-9/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      260 2017-01-16 15:04:21.000000 evrm-9/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      102 2017-01-16 15:04:21.000000 evrm-9/docs/_templates/base.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2017-01-16 15:20:02.000000 evrm-9/doctests/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2579 2017-01-16 15:04:21.000000 evrm-9/doctests/mods.output.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      165 2017-01-16 15:04:21.000000 evrm-9/doctests/mads.obj.py
+-rw-r--r--   0 bart      (1000) bart      (1000)       59 2017-01-16 15:20:02.000000 evrm-9/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      206 2017-01-16 15:04:21.000000 evrm-9/MANIFEST.in
+-rw-r--r--   0 bart      (1000) bart      (1000)     1919 2017-01-16 15:20:02.000000 evrm-9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `evrm-78/docs/README` & `evrm-9/README`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/_templates/class.rst` & `evrm-9/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/conf.py` & `evrm-9/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 
 #curdir = os.path.abspath(".")
 curdir = os.getcwd()
 sys.path.insert(0, curdir + os.sep)
 sys.path.insert(0, curdir + os.sep + '..' + os.sep)
 
-__version__ = 72
+from evrm import __version__, __txt__
 
 needs_sphinx='1.1'
 nitpick_ignore=[
                 ('py:class', 'builtins.BaseException'),
                ]
 
 extensions=[
@@ -37,15 +37,15 @@
 trim_doctest_flags=True
 doctest_flags=doctest.REPORT_UDIFF
 templates_path=['_templates',]
 source_suffix = '.rst'
 source_encoding = 'utf-8-sig'
 master_doc = 'index'
 project = "EVRM"
-copyright = 'Public Domain'
+copyright = '2016,2017 Bart Thate'
 version = '%s' % __version__
 release = '%s' % __version__
 language = ''
 today = ''
 today_fmt = '%B %d, %Y'
 exclude_patterns = ['_build', "_sources", "_templates"]
 default_role = ''
@@ -78,10 +78,7 @@
 html_file_suffix = '.html'
 htmlhelp_basename = 'pydoc'
 intersphinx_mapping = {
                        'python': ('https://docs.python.org/3', 'objects.inv'),
                        'sphinx': ('http://sphinx.pocoo.org/', None),
                       }
 intersphinx_cache_limit=1
-rst_prolog = """.. image:: nederland2.jpg
-    :width: 100%
-"""
```

### Comparing `evrm-78/docs/jpg/20140730_011.jpg` & `evrm-9/docs/jpg/20140730_011.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/20151028_009.jpg` & `evrm-9/docs/jpg/20151028_009.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/20151029_004.jpg` & `evrm-9/docs/jpg/20151029_004.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/69389.jpg` & `evrm-9/docs/jpg/69389.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/absoluut2.jpg` & `evrm-9/docs/jpg/absoluut2.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/aes.ico` & `evrm-9/docs/jpg/aes.ico`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/aesculaap.ico` & `evrm-9/docs/jpg/aesculaap.ico`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/bart.jpg` & `evrm-9/docs/jpg/bart.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/bart2.jpg` & `evrm-9/docs/jpg/bart2.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/besloten.jpg` & `evrm-9/docs/jpg/besloten.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/fact.jpg` & `evrm-9/docs/jpg/fact.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/geinformeerd.jpg` & `evrm-9/docs/jpg/geinformeerd.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/gelijk2.jpg` & `evrm-9/docs/jpg/gelijk2.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/igz.jpg` & `evrm-9/docs/jpg/igz.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/minister.jpg` & `evrm-9/docs/jpg/minister.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/nalatig.jpg` & `evrm-9/docs/jpg/nalatig.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/nederland.jpg` & `evrm-9/docs/jpg/nederland.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/nederland2.jpg` & `evrm-9/docs/jpg/nederland2.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/tussenkomst.jpg` & `evrm-9/docs/jpg/tussenkomst.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/jpg/verbod.jpg` & `evrm-9/docs/jpg/verbod.jpg`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/README.rst` & `evrm-9/docs/txt/README.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/VERGIFTIGING` & `evrm-9/docs/txt/VERGIFTIGING`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/Wetboek-van-Strafrecht.txt` & `evrm-9/docs/txt/Wetboek-van-Strafrecht.txt`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/WvGGZ.rst` & `evrm-9/docs/txt/WvGGZ.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/WvGGZ.txt` & `evrm-9/docs/txt/WvGGZ.txt`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/aangifte.rst` & `evrm-9/docs/txt/aangifte.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/bedreiging.rst` & `evrm-9/docs/txt/bedreiging.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/clozapine.rst` & `evrm-9/docs/txt/clozapine.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/dodelijk.rst` & `evrm-9/docs/txt/dodelijk.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/echt.rst` & `evrm-9/docs/txt/echt.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/ernstig.rst` & `evrm-9/docs/txt/ernstig.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/evrm.rst` & `evrm-9/docs/txt/evrm.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/fact.rst` & `evrm-9/docs/txt/fact.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-.. _fact:
-
 .. image:: ../jpg/fact.jpg
     :width: 100%
     :height: 4cm
 
+.. _fact:
+
 (F)ACT
 ######
 
-Brengt het toedienen van gif levensgevaar, het nalaten de noodzakelijke verpleging te leveren brengt de dood:
-
-1. Off-label toedienen.
-
-   Off-label toedienen houd in dat er of buiten de toegestaande bloedspiegels toegedient word of dat het medicijnen voor een andere ziekte word toegedient dan waarvoor hij getest is. Dient men hogere waardes toe dan toegestaan dan is men aan het vergiftigen. Dat een arts heden ten dage uberhaupt Off-label mag toedienen is al belachelijk (want per definitie vergiftiging).
-
-   Gif toedieningen dienen vervolgt te worden. 
-
-2. Onder de ondergrens toedienen.
-
-   Deze dodelijke stoffen hebben boven EN onder grenzen wat betreft bloedspiegels, depletie (het ontbreken van stoffen) is ook levensbedreigend.
-
-   De rechter mag alleen nog afbouwplannen goedkeuren.
-
-3. Ontkennen dat men dodelijke stoffen toedient.
-
-   Als een arts ontkent dat hij dodelijke stoffen toedient, dient hij MEER toe van die stof als de patient onstabiel word. I.p.v. de medicijnen af te bouwen, dient hij meer toe. De horror voor het slachtoffer dat in een toestand van vergiftiging meer gif krijgt toegedient.
-
-   Er moet een wet ter ontkenning van gif komen. 
-
-4. Bloedspiegel van een medicijn niet meten.
+(F)ACT bied niet de noodzakelijke verpleging om gif verantwoord toe te dienen:
 
-   Als een arts niet de bloedspiegels van een medicijn meet is hij niet op de hoogte van de toestand van de patient en kan dus ook geen goed oordeel vellen over het ziektebeeld van de patient. De arts probeert maar wat.
+1) Off-label toedienen.
 
-   Bloedmetingen voordat er een diagnose gepleegd word zouden verplicht moeten worden. 
+   Off-label toedienen houd in dat er of buiten de toegestaande
+   bloedspiegels toegedient word of dat het medicijnen voor een andere ziekte
+   word toegedient dan waarvoor hij getest is. Dient men hogere waardes toe dan 
+   toegestaan dan is men aan het vergiftigen. Dat een arts heden ten dage
+   uberhaupt Off-label mag toedienen is al belachelijk (want per definitie
+   vergiftiging).
 
-5. Symptomen van een vergiftiging niet (willen) zien.
+2) Onder de ondergrens toedienen.
 
-   Als een arts al dodelijk stoffen toedient en dat zelf niet wil erkennen is het voor hem ook onmogelijk om symptomen die ontstaan door het toedienen van dodelijke stoffen aan de dodelijke stoffen toe te kennen. Als een arts niet symptomen van vergiftiging erkent, komt de patient in een neerwaartse spiraal terecht waarbij zijn toestand met de dag verslechterd.
+   Deze dodelijke stoffen hebben boven EN beneden grenzen wat betreft bloedspiegels,
+   depletie (het ontbreken van stoffen) is ook levensbedreigend. 
 
-   Zou een wet tegen ontkenning van gif ook moeten voorkomen.   
+3) Ontkennen dat men dodelijke stoffen toedient.
 
-6. Eerst een afspraak maken voordat je een crisis kan melden,in het weekend en avonduren niet beschikbaar.
+   Als een arts ontkent dat hij dodelijke stoffen toedient, dient hij MEER toe
+   van die stof als de patient onstabiel word. I.p.v. de medicijnen af te
+   bouwen, dient hij meer toe. De horror voor het slachtoffer dat in een
+   toestand van vergiftiging meer gif krijgt toegedient.
 
-   De (F)ACT teams die de toediening van dodelijke stoffen verantwoord zouden moeten doen, zijn er in het weekend niet, in de avonduren niet, laten je een afspraak maken dat je een crisis mag melden, doen alles om maar niet te hoefen reageren om hulproepen van hun slachtoffers. Het niet aanwezig zijn van de noodzakelijke verpleging als met met dodelijke stoffen behandelt brengt wanhoop en paniek bij de slachtoffers die voor hun leven moeten vrezen.
+4) Bloedspiegel van een medicijn niet meten.
 
-   Verplichte herinvoering van 24/7 door huisartsen en niet HAP is weer de behandelaar verantwoordelijk maken voor de behandeling.
+   Als een arts niet de bloedspiegels van een medicijn meet is hij niet op de
+   hoogte van de toestand van de patient en kan dus ook geen goed oordeel
+   vellen over het ziektebeeld van de patient. De arts probeert maar wat.
 
-7. Pas zorgverlenen als de ellende al gebeurd is.
+5) Symptomen van een vergiftiging niet (willen) zien.
 
-   Men werkt met het principe van “stepped-care”, geschakelde zorg, waarbij men meer zorg levert naar gelang de toestand van het slachtoffer daar omvraagt. Dit maakt dat men altijd eerst de ellende laat gebeuren, waarna men pas extra zorg inschakelt. Wat men hier bezigt is “budget overschot is winst”, de zorg die men niet levert kan men als winst inboeken.
+   Als een arts al dodelijk stoffen overtreed en dat zelf niet wil erkennen is
+   het voor hem ook onmogelijk om symptomen die ontstaan door het toedienen van
+   dodelijke stoffen aan de dodelijke stoffen toe te kennen. Als een arts niet
+   symptomen van vergiftiging erkent, komt de patient in een neerwaartse
+   spiraal terecht waarbij zijn toestand met de dag verslechterd.
 
-   De SPV-er/casemanager in de basisverzekering is nodig.
+6) Eerst een afspraak maken voordat je een crisis kan melden.
+7) In het weekend en avonduren niet beschikbaar.
 
-8. Symptomen zelf bijhouden.
+   De FACT teams die de toediening van dodelijke stoffen verantwoord zouden
+   moeten doen, zijn er in het weekend niet, in de avonduren niet, laten je een
+   afspraak maken dat je een crisis mag melden, doen alles om maar niet te
+   hoefen reageren om hulproepen van hun slachtoffers. Het niet aanwezig zijn
+   van de noodzakelijke verpleging als met met dodelijke stoffen behandelt
+   brengt wanhoop en paniek bij de slachtoffers die voor hun leven moeten
+   vrezen.
 
-   De controle op de geleverde verpleging is zo slecht dat het aan een slachtoffer is om bij te houden hoe het met toename/afname van symptomen gaat. Het slachtoffer is echter helemaal niet in staat om symptomen bij te houden, het is aan de mantelzorger om te constateren dat een slachtoffer in een toestand van vergiftiging verkeerd.
+8) Pas zorgverlenen als de ellende al gebeurd is.
 
-   Ik probeer dit programma zo te maken dat men symptomen ook kan loggen.
+   Men werkt met het principe van "stepped-care", geschakelde zorg, waarbij men meer zorg levert
+   naar gelang de toestand van het slachtoffer daar omvraagt. Dit maakt dat men
+   altijd eerst de ellende laat gebeuren, waarna men pas extra zorg inschakeld.
+   Wat men hier bezigt is budget overschot is winst, de zorg die men niet
+   leverd kan men als winst inboeken.
 
-9. Oordeel “geen crisis”
+9) Symptomen zelf bijhouden.
 
-   Het toedienen van gif onder onverantwoorde omstandigheden maakt dat het slachtoffer in levensbedreigende situaties terecht komt. Deze door de “zorg” gegenereerde levensbedreiging is waar het slachtoffer mee te maken krijgt. Wel symptomen van dodelijke aandoeningen dan oordelen dat er geen opname nodig is, maakt dat noodzakelijke medische hulp hierbij word ontzegt.
+   De controle op de geleverde verpleging is zo slecht dat het aan een slachtoffer is om bij te houden hoe het met toename/afname van symptomen gaat. Echter
+   het slachtoffer is helemaal niet in staat om symptomen bij te houden, het is aan de mantelzorger om te constateren dat een slachtoffer in een toestand 
+   van vergiftiging verkeerd.
 
-   Iemand de noodzakelijke hulp bij vergiftiging ontzeggen vind ik inhumaan.
+10) Aanzetten tot zelfdoding.
 
-10. Behandelplan niet ingevuld.
+    Het toedienen van gif onder onverantwoorde omstandigheden maakt dat het
+    slachtoffer in levensbedreigende situaties terecht komt. Deze door de "zorg"
+    gegenereerde levensbedreiging is waar het slachtoffer mee te maken krijgt.
+    Niet alleen de schade door de medicijnen, de levensbedreiging van de
+    behandeling, is wat de mentale problemen oplevert.
 
-    Bij de behandeling door de GGZ word er zo min mogelijk aan verplichtingen opgeschreven in het behandelplan zodat er ook geen claims tot prestatie gemaakt kunnen worden. 
+11) Oordeel "geen crisis"
 
-    Volledig ingevulde behandelplannen zouden een vereiste moeten zijn voor behandeling.
+    Wel symptomen van dodelijke aandoeningen dan oordeel dat er geen opname nodig is, nooodzakelijke medische hulp word hierbij ontzegt.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `evrm-78/docs/txt/gif.rst` & `evrm-9/docs/txt/gif.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/greffe.rst` & `evrm-9/docs/txt/greffe.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/hoogeraad.rst` & `evrm-9/docs/txt/hoogeraad.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/kamerbrief.txt` & `evrm-9/docs/txt/kamerbrief.txt`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/kamerbrief2.rst` & `evrm-9/docs/txt/kamerbrief2.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/kamerbrief3.rst` & `evrm-9/docs/txt/kamerbrief3.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/leven.rst` & `evrm-9/docs/txt/leven.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/misdrijf.rst` & `evrm-9/docs/txt/misdrijf.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/mishandeling.rst` & `evrm-9/docs/txt/mishandeling.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/om.rst` & `evrm-9/docs/txt/om.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/oorzaak.rst` & `evrm-9/docs/txt/oorzaak.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/opzet2.rst` & `evrm-9/docs/txt/opzet2.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/pad.rst` & `evrm-9/docs/txt/pad.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/receptoren.rst` & `evrm-9/docs/txt/receptoren.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/recht.rst` & `evrm-9/docs/txt/recht.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/risico.rst` & `evrm-9/docs/txt/risico.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/schadelijk.rst` & `evrm-9/docs/txt/schadelijk.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/sedatie.rst` & `evrm-9/docs/txt/sedatie.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/todo.rst` & `evrm-9/docs/txt/todo.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/toxic.rst` & `evrm-9/docs/txt/toxic.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/urls.rst` & `evrm-9/docs/txt/urls.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 .. _urls:
 
 urls
 ####
 
-.. _sds:
-
-Clozapine Safety Data Sheet
-
-* https://drive.google.com/open?id=0BwaFXkZBje4OLTZ2ZEhmVWhZZmc
-
-.. _highlights:
-
-Clozapine Highlights of Prescribing Information
-
-*  https://drive.google.com/open?id=0BwaFXkZBje4OdnBmS05sQ2dkUEE
-
-
 GENEESMIDDELENBANK
 
 * http://www.geneesmiddeleninformatiebank.nl/ords/f?p=111
 
 GEBRUIK
 
 * https://www.nza.nl/publicaties/1048188/Marktscan_en_beleidsbrief_GGZ_2012
```

### Comparing `evrm-78/docs/txt/vervolgen.rst` & `evrm-9/docs/txt/vervolgen.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/verzoek.rst` & `evrm-9/docs/txt/verzoek.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/wet.rst` & `evrm-9/docs/txt/wet.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/wvggz.rst` & `evrm-9/docs/txt/wvggz.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/docs/txt/zyprexa.rst` & `evrm-9/docs/txt/zyprexa.rst`

 * *Files identical despite different names*

### Comparing `evrm-78/evrm/sui.py` & `evrm-9/evrm/stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,169 @@
-# This file is placed in the Public Domain.
+# suicide.py
 #
-# EM_T04_OTP-CR-117_19 otp.informationdesk@icc-cpi.int https://genocide.rtfd.io
+#
+
+""" show statistics on suicide. """
+
+from mads.time import elapsed, to_time, today, now
+from mads.clock import Repeater
+from mads.event import Event
+from mads.obj import Object
 
-"suicide stats"
+from mids import main, storage, launcher, storage, fleet
+
+cfgs = Object()
 
 import random
 import time
 
-from .run import Bus, Event, Repeater, elapsed
-from .obj import Object, get, items, keys
-
-source = "https://github.com/bthate/genocide"
-startdate = "2018-10-05 00:00:00"
-starttime = time.mktime(time.strptime(startdate, "%Y-%m-%d %H:%M:%S"))
-
-def init(k):
-    for _name, obj in items(wanted):
-        for key in keys(obj):
-            val = get(obj, key, None)
-            if val:
-                e = Event()
-                e.txt = ""
-                e.rest = key
+startdate = "2012-10-12 00:00:00"
+#startdate = "2016-01-01 00:00:00"
+starttime = to_time(startdate)
+source = "https://bitbucket.org/thatebart/mads"
+
+def init(event):
+    args = event._parsed.args
+    for name, obj in wanted.items():
+        if name in main.cfg.init.split(",") or args and name in args:
+            for key, val in obj.items():
                 sec = seconds(val)
-                repeater = Repeater(sec, stat, e, name=key)
-                repeater.start()
+                repeater = Repeater(sec, stat, event, name="Stats.%s" % key)
+                launcher.launch(repeater.start)
 
-class ENOSTATS(Exception):
+def shutdown(event):
+    launcher.kill("Stats")
 
-    pass
-
-def seconds(nrs, period="jaar"):
-    if not nrs:
-        return nrs
-    return get(nrsec, period) / float(nrs)
+def seconds(nr, period="jaar"):
+    if not nr: return nr
+    return nrsec.get(period) / float(nr)
 
 def nr(name):
-    for key in keys(wanted):
-        obj = get(wanted, key, None)
-        for n in keys(obj):
-            if n == name:
-                return get(obj, n)
-    raise ENOSTATS(name)
-
-def stat(e):
-    name = e.rest or "suicide"
-    if "." in name:
-        name = name.split(".")[-1]
+    delta = time.time() - starttime
+    awake = time.time() - today()
+    for key, obj in wanted.items():
+        for n, val in obj.items():
+            if n == name: return val
+    return 0
+
+def stats(event, **kwargs):
+    args = event._parsed.args
+    txt = "Sinds %s\n\n" % time.ctime(starttime)
+    delta = time.time() - starttime
+    for name, obj in wanted.items():
+        for key, val in obj.items():
+            needed = seconds(nr(key))
+            if not needed: continue
+            nrtimes = int(delta/needed)
+            txt += "%s #%s %s " % (key.upper(), nrtimes, tags.get(key, ""))
+    event.reply(txt.strip())
+
+def stat(event, **kwargs):
+    e = Event(kwargs)
+    cfg = cfgs.get("stats", None)
+    if not cfg:
+       cfgs.stats = cfg = storage.last("cfg", "stats")
+    name = event._parsed.rest or e.name 
+    if "." in name: name = name.split(".")[-1]
     name = name.lower()
     delta = time.time() - starttime
-    try:
-        needed = seconds(nr(name))
-    except ENOSTATS:
-        return
+    awake = time.time() - today()
     needed = seconds(nr(name))
     if needed:
         nrtimes = int(delta/needed)
         txt = "%s #%s" % (name.upper(), nrtimes)
         if name in omschrijving:
-            txt += " (%s)" % get(omschrijving, name)
+            txt += " (%s)" % omschrijving.get(name)
         txt += " elke %s" % elapsed(seconds(nr(name)))
-        if name in tags:
-            txt += " %s" % get(tags,name)
+        if name in soort:
+            txt += " door een %s" % soort.get(name)
         else:
-            txt += " %s" % random.choice(list(tags.values()))
-        Bus.announce(txt)
+            txt += " door een %s" % random.choice(list(soort.values()))
+        txt += " bijv. in %s" % random.choice(gemeenten)
+        if name in tags:
+            txt += " %s" % tags.get(name)
+        else: txt += " %s" % random.choice(list(tags.values()))
+        if cfg and cfg.showurl and name in urls:
+            txt += " - %s" % urls.get(name)
+        for bot in fleet.bots:
+            bot.announce(txt)
+
+antidepressiva = Object()
+antidepressiva["2010"] = 935567
+antidepressiva["2011"] = 956091
+antidepressiva["2012"] = 968662
+antidepressiva["2013"] = 981179
+antidepressiva["2014"] = 1010005
+
+antipsychotica = Object()
+antipsychotica["2010"] = 272772
+antipsychotica["2011"] = 277832
+antipsychotica["2012"] = 286158
+antipsychotica["2013"] = 292950
+antipsychotica["2014"] = 304815
+
+adhdmiddel = Object()
+adhdmiddel["2010"] = 146747
+adhdmiddel["2011"] = 164282
+adhdmiddel["2012"] = 178059
+adhdmiddel["2013"] = 189845
+adhdmiddel["2014"] = 206381 
 
-def sts(event):
-    txt = "Sinds %s\n" % time.ctime(starttime)
-    delta = time.time() - starttime
-    for _name, obj in items(wanted):
-        for key, _val in items(obj):
-            needed = seconds(nr(key))
-            if not needed:
-                continue
-            nrtimes = int(delta/needed)
-            txt += "\n%s #%s %s %s" % (key.upper(), nrtimes, get(tags, key, ""), get(zorg, random.choice(list(keys(zorg))), ""))
-    event.reply(txt.strip())
+#:
+nrsec = Object()
+nrsec.dag = 24 * 60 * 60.0
+nrsec.jaar = 365 * nrsec.dag
+nrsec.weekend = 2 / 7 * (24 * 60 * 60.0 * 365) / 52
+nrsec.avond = 16 / 24 * (24 * 60 * 60.0)
+
+
+#:
+times = Object()
+times.weekend = 2 / 7 * (24 * 60 * 60.0 * 365) / 52
+times.avond = 16 / 24 * (24 * 60 * 60.0)
+times.dag = 24 * 60 * 60.0
+times.jaar = 365 * 24 * 60 * 60.0
 
+#:
+rechter = Object()
+rechter.ibs = 8171
+rechter.rm = 16171
+rechter.vwm = 6516
+rechter.mvv = 4034
+rechter.vm = 5566
+rechter.mev = 45
+#rechter.om = 0
+rechter.zm= 6
+
+#:
+drugs = Object()
+drugs.speed = 20000
+drugs.cocaine = 50000
+drugs.alcohol = 400000
+drugs.wiet = 500000
+
+#:
+recepten = Object()
+recepten.antipsychotica = 150000
+recepten.antidepresiva = 600000
+recepten.slaapmiddel = 1000000
+
+#:
+demografie = Object()
+demografie.ambulant = 792000
+demografie.verslaving = 13000
+demografie.schizofrenie = 9800
+demografie.depressie = 9600
+demografie.verslaafden = 2074278
+demografie.arbeidshandicap = 103000
+demografie.huisartsen = 11345
+demografie.zorgmijder = 24000
+
+#:
 cijfers = Object()
-cijfers.melding = 61000
 cijfers.opnames = 24338
 cijfers.crisis = 150000
 cijfers.oordeel = 150000
 cijfers.pogingen = 94000
 cijfers.incidenten = 66000
 cijfers.poh = 1300000
 cijfers.vergiftigingen = 25262
@@ -97,22 +177,41 @@
 cijfers.tumor = 12000
 cijfers.detox = 65654
 cijfers.acuut = 8000
 cijfers.spoedeisendpoging = 14000
 cijfers.weguitkliniek = 2539
 cijfers.bewindvoering = 295000
 cijfers.suicidegedachtes = 410000
-cijfers.psychosestoornis = 13076
-cijfers.oorzaak = cijfers.psychosestoornis + cijfers.suicide
 
+#:
+medicijnen = Object()
+medicijnen.amitriptyline = 189137
+medicijnen.paroxetine = 186028
+medicijnen.citalopram = 154620
+medicijnen.oxazepam = 133608
+medicijnen.venlafaxine = 112000
+medicijnen.mirtazapine = 110742
+medicijnen.quetiapine = 84414
+medicijnen.diazepam = 72000
+medicijnen.sertraline = 68000
+medicijnen.haloperidol = 59825
+
+#:
+oordeel = Object()
+oordeel.verwijs = cijfers.crisis * 0.85 
+oordeel.uitstroom = cijfers.crisis * 0.05
+oordeel.opname = cijfers.crisis * 0.10
+
+#:
 alarm = Object()
-alarm.politie = 0.30 * cijfers.crisis
+alarm.politie = 0.15 * cijfers.crisis
 alarm.hap = 0.40 * cijfers.crisis
-alarm.keten = 0.30 * cijfers.crisis
+alarm.keten = 0.45 * cijfers.crisis
 
+#:
 dbc = Object()
 dbc.middelgebondenstoornissen = 33060
 dbc.somatoformestoornissen = 21841
 dbc.cognitievestoornissen = 25717
 dbc.angststoornissen = 54458
 dbc.aanpassingsstoornissen = 43079
 dbc.depressievestoornissen = 102361
@@ -125,58 +224,148 @@
 dbc.posttraumatischestressstoornis = 24716
 dbc.persoonlijkheidsstoornissen = 36574
 dbc.adhd = 25951
 dbc.gedrag = 1176
 dbc.kindertijdoverig = 1035
 dbc.autismespectrum = 9436
 
-
-demografie = Object()
-demografie.ambulant = 792000
-demografie.verslaving = 13000
-demografie.schizofrenie = 9800
-demografie.depressie = 9600
-demografie.verslaafden = 2074278
-demografie.arbeidshandicap = 103000
-demografie.huisartsen = 11345
-demografie.zorgmijder = 24000
-
-drugs = Object()
-drugs.speed = 20000
-drugs.cocaine = 50000
-drugs.alcohol = 400000
-drugs.wiet = 500000
-
-e33 = Object()
-e33.melding = 61000
-
+#:
 halfwaarde = Object()
 halfwaarde.zyprexa = 30
 halfwaarde.abilify = 75
 halfwaarde.haldol = 30
 halfwaarde.alprazolam = 11
 halfwaarde.orap = 55
 halfwaarde.paracetamol = 2.5
 halfwaarde.lorazepam = 12
-halfwaarde.paroxetine = 21
+halfwaarde.paroxetine = 21 
 halfwaarde.citalopram = 35
 halfwaarde.oxazepam = 8.2
 halfwaarde.quetiapine = 6
 halfwaarde.diazepam = 100
 halfwaarde.wiet = 7
 
+#: 
+perdag = Object()
+perdag.medicijnen = medicijnen
+perdag.drugs = drugs
+
+#:
+suicidejaar = Object()
+suicidejaar["2008"] = 1435
+suicidejaar["2009"] = 1525
+suicidejaar["2010"] = 1600
+suicidejaar["2011"] = 1647
+suicidejaar["2012"] = 1753
+suicidejaar["2013"] = 1857
+suicidejaar["2014"] = 1839
+suicidejaar["2015"] = 1871 
+
+
+#:
+ziekenhuis = Object()
+ziekenhuis["2010"] = 7800
+ziekenhuis["2011"] = 9600
+ziekenhuis["2012"] = 9200
+ziekenhuis["2013"] = 8300
+ziekenhuis["2014"] = 8500
+
+#:
+seh = Object()
+seh["2010"] = 13700
+seh["2011"] = 16000
+seh["2012"] = 15800
+seh["2013"] = 13300
+seh["2014"] = 14000
+
+#:
+suicide = Object()
+suicide.suicide = cijfers.suicide
+
+pogingen = Object()
+pogingen.pogingen = cijfers.pogingen
+
+
+#:
+poging = Object()
+poging.ziekenhuis = ziekenhuis["2014"]
+poging.seh = seh["2014"]
+
+#:
+meds = Object()
+meds.antidepressiva = antidepressiva["2014"]
+meds.antipsychotica = antipsychotica["2014"]
+meds.adhdmiddel = adhdmiddel["2014"]
+
+#:
+wanted = Object()
+wanted.rechter = rechter
+wanted.oordeel = oordeel
+wanted.alarm = alarm
+wanted.suicide = suicide
+wanted.pogingen = pogingen
+wanted.meds = meds
+
+#:
 omdat = Object()
 omdat.blokkeren = "met antipsychotica de werking van receptoren BLOKKEREN en dat dat benadeling van de gezondheid is."
 omdat.wetboek = "het Wetboek van Strafrecht zegt dat mishandeling wordt gelijkgesteld aan opzettelijke benadeling van de gezondheid."
 omdat.benadeling = "men op de hoogte is van de benadeling is er van opzet altijd sprake."
 omdat.vergiftigt = "men vergiftigt kan worden door deze medicijnen."
 omdat.zolang = ", zolang een arts de bloedspiegel van een medicijn niet meet, de toestand van vergiftiging niet opgeheven word."
 omdat.toestand = "men met deze toestand de kans op overlijden geeft."
 omdat.dood = "men eraan dood gaat."
 
+zorg = Object()
+zorg.interventie = "een interventie, bestaande uit een vorm van verzorging, bejegening, behandeling, begeleiding of bescherming"
+zorg.toediening = "toediening van medicatie, vocht en voeding, regelmatige medische controle of andere medische handelingen"
+zorg.maatregel = "pedagogische of therapeutische maatregelen"
+zorg.opname = "opname in een accommodatie"
+zorg.beperking = "beperking van de bewegingsvrijheid"
+zorg.seperatie = "afzondering of separatie in een daartoe geschikte verblijfsruimte"
+zorg.beperking = "beperking van het recht op het ontvangen van bezoek of het gebruik van communicatiemiddelen"
+zorg.toezicht = "toezicht op betrokkene"
+zorg.onderzoek = "onderzoek aan kleding of lichaam"
+zorg.controle = "controle op de aanwezigheid van gedrag beïnvloedende middelen"
+zorg.beperkingen = "beperkingen in de vrijheid het eigen leven in te richten, die tot gevolg hebben dat betrokkene iets moet doen of nalaten."
+
+#:
+tags = Object()
+tags.keten = "#burgemeester"
+tags.politie = "#broodjepindakaas"
+tags.hap = "#triagetrien"
+tags.verwijs = "#maandagweer"
+tags.uitstroom = "#zorgwekkend"
+tags.opname = "#meermedicijn"  
+tags.crisis = "#triade"
+tags.suicide = "#wetverplichteggz"
+tags.pogingen = "#prettigweekend" 
+tags.incidenten = "#jammerdan"    
+tags.acuut = "#geenbedvoorjou"    
+tags.zorgmijder = "#helaas"       
+tags.inwoners = "#gebodenvrucht"  
+tags.crisis = "#medicijnen"
+tags.alarm = "#telaat"
+tags.oordeel = "#geencrisis"
+tags.vergiftigingen = "#overduur"
+tags.neurotoxisch = "#overdosis" 
+tags.schizofrenie = "#gifmedicijn"
+tags.angst = "#gifmedicijn"
+tags.depressie = "#gifmedicijn"
+tags.meds = "#gifmedicijn"
+tags.ibs = "#overlast"
+tags.rm = "#benadeling"
+tags.vwm = "#maatregel"
+tags.vm = "#nogeven"
+tags.mvv = "#direct!!"
+tags.mev = "#kieserzelfvoor"
+tags.om = "#ffkijken#"
+tags.zm = "????"
+
+#:
 omschrijving = Object()
 omschrijving.ibs = "inbewaringstelling"
 omschrijving.rm = "rechterlijke machtiging"
 omschrijving.vm = "voorlopige rechterlijke machtiging"
 omschrijving.mvv = "machtiging voortgezet verblijf"
 omschrijving.vwm = "voorwaardelijke rechterlijke machtiging"
 omschrijving.mev = "machtiging eigen verzoek"
@@ -243,53 +432,16 @@
 omschrijving.posttraumatischestressstoornis = "stress na trauma"
 omschrijving.persoonlijkheidsstoornissen = "aanpassings problemen"
 omschrijving.adhd = "te druk, te veel energie"
 omschrijving.gedrag = "moelijk opvoedbaar"
 omschrijving.kindertijdoverig = "vroegtijdig trauma"
 omschrijving.autismespectrum = "valt in een autisme categorie"
 omschrijving.seh = "spoedeisende hulp"
-omschrijving.psychosestoornis = "een door de psychose zelf overleden persoon"
-omschrijving.oorzaak = "oorzaak van overlijden"
-
-medicijnen = Object()
-medicijnen.amitriptyline = 189137
-medicijnen.paroxetine = 186028
-medicijnen.citalopram = 154620
-medicijnen.oxazepam = 133608
-medicijnen.venlafaxine = 112000
-medicijnen.mirtazapine = 110742
-medicijnen.quetiapine = 84414
-medicijnen.diazepam = 72000
-medicijnen.sertraline = 68000
-medicijnen.haloperidol = 59825
-
-demo = Object()
-demo.dbc = dbc
-demo.medicijnen = medicijnen
-demo.drugs = drugs
-
-oordeel = Object()
-oordeel.verwijs = cijfers.crisis * 0.85
-oordeel.uitstroom = cijfers.crisis * 0.05
-oordeel.opname = cijfers.crisis * 0.10
-
-oorzaak = Object()
-oorzaak.suicide = 1800
-oorzaak.psychosestoornis = 12000
-
-nrsec = Object()
-nrsec.dag = 24 * 60 * 60.0
-nrsec.jaar = 365 * nrsec.dag
-nrsec.weekend = 2 / 7 * (24 * 60 * 60.0 * 365) / 52
-nrsec.avond = 16 / 24 * (24 * 60 * 60.0)
-
-perdag = Object()
-perdag.medicijnen = medicijnen
-perdag.drugs = drugs
 
+#:
 periode = Object()
 periode.ibs = "voor 6 weken"
 periode.rm = "voor 6 maanden"
 periode.vlm = "max 18 uur"
 periode.mvv = "voor 6 maanden"
 periode.vwm = "voor jaren"
 periode.mev = "voor jaren"
@@ -311,89 +463,84 @@
 periode.inwoners = ""
 periode.crisis = "elke dag"
 periode.alarm = "elke dag"
 periode.oordeel = "buiten kantoor uren en in het weekend"
 periode.vergiftigingen = "elke dag"
 periode.neurotoxisch = "elke dag"
 
-pogingen = Object()
-pogingen.pogingen = cijfers.pogingen
-
-recepten = Object()
-recepten.antipsychotica = 150000
-recepten.antidepresiva = 600000
-recepten.slaapmiddel = 1000000
-
-rechter = Object()
-rechter.ibs = 8861
-rechter.rm = 17746
-rechter.vwm = 6657
-rechter.mvv = 4431
-rechter.vm = 6690
-rechter.mev = 65
-rechter.zm = 3
-
-seh = Object()
-seh.y2010 = 13700
-seh.y2011 = 16000
-seh.y2012 = 15800
-seh.y2013 = 13300
-seh.y2014 = 14000
-
-suicidejaar = Object()
-suicidejaar.y2008 = 1435
-suicidejaar.y2009 = 1525
-suicidejaar.y2010 = 1600
-suicidejaar.y2011 = 1647
-suicidejaar.y2012 = 1753
-suicidejaar.y2013 = 1857
-suicidejaar.y2014 = 1839
-suicidejaar.y2015 = 1871
-suicidejaar.y2016 = 1894
-suicidejaar.y2017 = 1917
-
-show = Object()
-show.opnames = 24338
-show.crisis = 150000
-show.oordeel = 150000
-show.pogingen = 94000
-show.incidenten = 66000
-show.vergiftigingen = 25262
-show.overlast = 18000
-show.insluiting = 24000
-show.aangiftes = 134000
-show.suicide = 1871
-show.burenoverlast = 12000
-show.uitzetting = 5900
-show.volwassendoop = 500
-show.detox = 65654
-show.acuut = 8000
-show.spoedeisendpoging = 14000
-show.weguitkliniek = 2539
-show.bewindvoering = 295000
-show.pogingen = cijfers.pogingen
+#:
+urls = Object()
+urls.IBS = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.RM = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.VM = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.MVV = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.VW = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.MEV = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.ZB = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.OB = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
+urls.opname = "http://www.tijdschriftvoorpsychiatrie.nl/issues/434/articles/8318"
+urls.crisis = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
+urls.tuchtrecht = "http://tuchtrecht.overheid.nl/zoeken/resultaat/uitspraak/2014/ECLI_NL_TGZRAMS_2014_94?zaaknummer=2013%2F221&Pagina=1&ItemIndex=1"
+urls.suicide = "http://www.cbs.nl/nl-NL/menu/themas/bevolking/publicaties/artikelen/archief/2014/2014-4204-wm.htm"
+urls.incident = "https://www.wodc.nl/onderzoeksdatabase/2337-de-effectiviteit-van-de-politiele-taakuitvoering-en-de-taken-en-verantwoordelijkheden-van-andere-partijen.aspx"
+urls.zorgmijder = "http://www.gezondheidsraad.nl/sites/default/files/samenvatting_noodgedwongen_0.pdf"
+urls.acuut = "http://www.gezondheidsraad.nl/sites/default/files/samenvatting_noodgedwongen_0.pdf"
+urls.wvggz = "https://www.dwangindezorg.nl/de-toekomst/wetsvoorstellen/wet-verplichte-geestelijke-gezondheidszorg"
+urls.politie = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
+urls.hap = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
+urls.keten = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
+urls.verwijs = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
+urls.uitstroom = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html" 
+urls.opnames = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
+urls.vergifitigingen = "http://www.umcutrecht.nl/getmedia/f9f152e2-8638-4ffc-a05f-fce72f5f416a/NVIC-Jaaroverzicht-2014.pdf.aspx?ext=.pdf"
+urls.neurotoxisch = "http://www.umcutrecht.nl/getmedia/f9f152e2-8638-4ffc-a05f-fce72f5f416a/NVIC-Jaaroverzicht-2014.pdf.aspx?ext=.pdf"
+urls.incidenten = "http://www.dsp-groep.nl/userfiles/file/Politie%20en%20verwarde%20personen%20_DSP-groep.pdf"
+urls.ambulant = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.verslaving = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.poh = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.meds = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.depressie = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.angst = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.schizofrenie = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
+urls.detox = "https://www.jellinek.nl/vraag-antwoord/hoeveel-mensen-zijn-verslaafd-en-hoeveel-zijn-er-in-behandeling/"
+urls.verslaafden = "https://www.jellinek.nl/vraag-antwoord/hoeveel-mensen-zijn-verslaafd-en-hoeveel-zijn-er-in-behandeling/"
+urls.volwassendoop = ""
+urls.arbeidshandicap = "http://www.nationalezorggids.nl/gehandicaptenzorg/nieuws/27841-ruim-100-000-mensen-op-sociale-werkplaats.html"
+urls.overlast = "http://nos.nl/artikel/2075227-verwarde-huurders-veroorzaken-steeds-meer-overlast.html"
+urls.insluiting = "http://www.tweedekamer.nl/downloads/document?id=78ee0f32-7487-4bcc-ba01-e01ace2bc4b4&title=Arrestantenzorg%20Nederland%20Landelijke%20rapportage.pdf"
+urls.zyprexa = "http://www.ema.europa.eu/docs/nl_NL/document_library/EPAR_-_Product_Information/human/000287/WC500055611.pdf"
+urls.factor = "http://nos.nl/artikel/2090676-aantal-incidenten-met-verwarde-mensen-flink-onderschat.html"
+urls.dbc = "https://www.nza.nl/1048076/1048181/Marktscan_ggz_2014_deel_B_en_beleidsbrief.pdf"
+urls.dbs2015 = "https://www.rijksoverheid.nl/documenten/rapporten/2016/05/25/marktscan-ggz"
+urls.medicijnen="https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/geestelijke-gezondheidszorg/row-5/welke-geneesmiddelen-worden-het-meest-voorgeschreven-in-de-ggz/"
+urls.pogingen="http://www.nfzp.nl/wp/wp-content/uploads/2010/09/Einddocument-AF0943-Kwaliteitsdcoument-Ketenzorg-bij-Suicidaliteit.pdf"
+urls.suicidegedachte="http://www.nfzp.nl/wp/wp-content/uploads/2010/09/Einddocument-AF0943-Kwaliteitsdcoument-Ketenzorg-bij-Suicidaliteit.pdf"
+urls.ziekenhuisopnames = "https://www.tweedekamer.nl/kamerstukken/detail?id=2016D13371&did=2016D13371"
+urls.seh = "https://www.tweedekamer.nl/kamerstukken/detail?id=2016D13371&did=2016D13371"
+urls.epa = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/ernstige-psychiatrische-aandoeningen/"
 
+#:
 soort = Object()
 soort.alarm = "patient"
 soort.oordeel = "arts"
 soort.neurotoxisch = "patient"
 soort.angst = "patient"
 soort.depressie = "patient"
 soort.schizofrenie = "patient"
 soort.ibs = "burgemeester"
 soort.rm = "civiele rechter"
 soort.vm = "civiele rechter"
 soort.mvv = "civiele rechter"
 soort.vwm = "civiele rechter"
 soort.ev = "civiele rechter"
-soort.om = "civiele rechter"
+soort.om ="civiele rechter"
 soort.zm = "civiele rechter"
 soort.politie = "agent"
 soort.hap = "huisarts"
-soort.keten = "spv/psychiater"
+soort.keten  = "spv/psychiater"
 soort.verwijs = "crisisdienst"
 soort.uitstroom = "eigen behandelaar"
 soort.suicide = "slachtoffer"
 soort.crisis = "burger"
 soort.pogingen = "wanhopige patient"
 soort.incidenten = "hulproepende patient"
 soort.acuut = "vergiftigde patient"
@@ -409,141 +556,402 @@
 soort.sertrali = "patient"
 soort.haloperidol = "patient"
 soort.insluiting = "politie"
 soort.ambulant = "casemanager"
 soort.verslaafden = "gebruiker"
 soort.slaapmiddel = "insomnia patient"
 
-suicidejaar = Object()
-suicidejaar.y2008 = 1435
-suicidejaar.y2009 = 1525
-suicidejaar.y2010 = 1600
-suicidejaar.y2011 = 1647
-suicidejaar.y2012 = 1753
-suicidejaar.y2013 = 1857
-suicidejaar.y2014 = 1839
-suicidejaar.y2015 = 1871
-suicidejaar.y2016 = 1894
-suicidejaar.y2017 = 1917
-
-suicide = Object()
-suicide.suicide = suicidejaar.y2017
-
-tags = Object()
-tags.keten = "#burgemeester"
-tags.politie = "#broodjepindakaas"
-tags.hap = "#triagetrien"
-tags.verwijs = "#maandagweer"
-tags.uitstroom = "#zorgwekkend"
-tags.opname = "#meermedicijn"
-tags.crisis = "#triade"
-tags.suicide = "#wetverplichteggz"
-tags.pogingen = "#prettigweekend"
-tags.incidenten = "#jammerdan"
-tags.acuut = "#geenbedvoorjou"
-tags.zorgmijder = "#helaas"
-tags.inwoners = "#gebodenvrucht"
-tags.crisis = "#medicijnen"
-tags.alarm = "#telaat"
-tags.oordeel = "#geencrisis"
-tags.vergiftigingen = "#overduur"
-tags.neurotoxisch = "#overdosis"
-tags.schizofrenie = "#gifmedicijn"
-tags.angst = "#gifmedicijn"
-tags.depressie = "#gifmedicijn"
-tags.meds = "#gifmedicijn"
-tags.ibs = "#overlast"
-tags.rm = "#benadeling"
-tags.vwm = "#maatregel"
-tags.vm = "#nogeven"
-tags.mvv = "#direct!!"
-tags.mev = "#kieserzelfvoor"
-tags.om = "#ffkijken#"
-tags.zm = "#zelfwat?"
-
-times = Object()
-times.weekend = 2 / 7 * (24 * 60 * 60.0 * 365) / 52
-times.avond = 16 / 24 * (24 * 60 * 60.0)
-times.dag = 24 * 60 * 60.0
-times.jaar = 365 * 24 * 60 * 60.0
-
-urls = Object()
-urls.ibs = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.rm = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.vm = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.mvv = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.vw = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.mev = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.zb = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.ob = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.zm = "http://www.tijdschriftvoorpsychiatrie.nl/assets/articles/57-2015-4-artikel-broer.pdf"
-urls.iatrogeen = "https://www.nrc.nl/nieuws/2011/04/22/eenvijfde-van-de-opnames-te-wijten-aan-medicijnen-12012115-a426225"
-urls.opname = "http://www.tijdschriftvoorpsychiatrie.nl/issues/434/articles/8318"
-urls.crisis = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.tuchtrecht = "http://tuchtrecht.overheid.nl/zoeken/resultaat/uitspraak/2014/ECLI_NL_TGZRAMS_2014_94?zaaknummer=2013%2F221&Pagina=1&ItemIndex=1"
-urls.suicide = "http://www.cbs.nl/nl-NL/menu/themas/bevolking/publicaties/artikelen/archief/2014/2014-4204-wm.htm"
-urls.incident = "https://www.wodc.nl/onderzoeksdatabase/2337-de-effectiviteit-van-de-politiele-taakuitvoering-en-de-taken-en-verantwoordelijkheden-van-andere-partijen.aspx"
-urls.zorgmijder = "http://www.gezondheidsraad.nl/sites/default/files/samenvatting_noodgedwongen_0.pdf"
-urls.acuut = "http://www.gezondheidsraad.nl/sites/default/files/samenvatting_noodgedwongen_0.pdf"
-urls.wvggz = "https://www.dwangindezorg.nl/de-toekomst/wetsvoorstellen/wet-verplichte-geestelijke-gezondheidszorg"
-urls.politie = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.hap = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.keten = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.verwijs = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.uitstroom = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.opnames = "http://www.rijksoverheid.nl/documenten-en-publicaties/rapporten/2015/02/11/acute-geestelijke-gezondheidszorg-knelpunten-en-verbetervoorstellen-in-de-keten.html"
-urls.vergifitigingen = "http://www.umcutrecht.nl/getmedia/f9f152e2-8638-4ffc-a05f-fce72f5f416a/NVIC-Jaaroverzicht-2014.pdf.aspx?ext=.pdf"
-urls.neurotoxisch = "http://www.umcutrecht.nl/getmedia/f9f152e2-8638-4ffc-a05f-fce72f5f416a/NVIC-Jaaroverzicht-2014.pdf.aspx?ext=.pdf"
-urls.incidenten = "http://www.dsp-groep.nl/userfiles/file/Politie%20en%20verwarde%20personen%20_DSP-groep.pdf"
-urls.ambulant = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.verslaving = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.poh = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.meds = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.depressie = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.angst = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.schizofrenie = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/"
-urls.detox = "https://www.jellinek.nl/vraag-antwoord/hoeveel-mensen-zijn-verslaafd-en-hoeveel-zijn-er-in-behandeling/"
-urls.verslaafden = "https://www.jellinek.nl/vraag-antwoord/hoeveel-mensen-zijn-verslaafd-en-hoeveel-zijn-er-in-behandeling/"
-urls.volwassendoop = ""
-urls.arbeidshandicap = "http://www.nationalezorggids.nl/gehandicaptenzorg/nieuws/27841-ruim-100-000-mensen-op-sociale-werkplaats.html"
-urls.overlast = "http://nos.nl/artikel/2075227-verwarde-huurders-veroorzaken-steeds-meer-overlast.html"
-urls.insluiting = "http://www.tweedekamer.nl/downloads/document?id=78ee0f32-7487-4bcc-ba01-e01ace2bc4b4&title=Arrestantenzorg%20Nederland%20Landelijke%20rapportage.pdf"
-urls.zyprexa = "http://www.ema.europa.eu/docs/nl_NL/document_library/EPAR_-_Product_Information/human/000287/WC500055611.pdf"
-urls.factor = "http://nos.nl/artikel/2090676-aantal-incidenten-met-verwarde-mensen-flink-onderschat.html"
-urls.dbc = "https://www.nza.nl/1048076/1048181/Marktscan_ggz_2014_deel_B_en_beleidsbrief.pdf"
-urls.dbs2015 = "https://www.rijksoverheid.nl/documenten/rapporten/2016/05/25/marktscan-ggz"
-urls.medicijnen = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/geestelijke-gezondheidszorg/row-5/welke-geneesmiddelen-worden-het-meest-voorgeschreven-in-de-ggz/"
-urls.pogingen = "http://www.nfzp.nl/wp/wp-content/uploads/2010/09/Einddocument-AF0943-Kwaliteitsdcoument-Ketenzorg-bij-Suicidaliteit.pdf"
-urls.suicidegedachte = "http://www.nfzp.nl/wp/wp-content/uploads/2010/09/Einddocument-AF0943-Kwaliteitsdcoument-Ketenzorg-bij-Suicidaliteit.pdf"
-urls.ziekenhuisopnames = "https://www.tweedekamer.nl/kamerstukken/detail?id=2016D13371&did=2016D13371"
-urls.seh = "https://www.tweedekamer.nl/kamerstukken/detail?id=2016D13371&did=2016D13371"
-urls.epa = "https://www.zorgprismapubliek.nl/informatie-over/geestelijke-gezondheidszorg/ernstige-psychiatrische-aandoeningen/"
-urls.rechter = "https://www.ggdghorkennisnet.nl/?file=43865&m=1541606110&action=file.download"
-urls.psychosestoornis = "https://www.volksgezondheidenzorg.info/echi-indicators/mortality#node-disease-specific-mortality"
-
-zorg = Object()
-zorg.interventie = "een interventie, bestaande uit een vorm van verzorging, bejegening, behandeling, begeleiding of bescherming"
-zorg.toediening = "toediening van medicatie, vocht en voeding, regelmatige medische controle of andere medische handelingen"
-zorg.maatregel = "pedagogische of therapeutische maatregelen"
-zorg.opname = "opname in een accommodatie"
-zorg.beperking = "beperking van de bewegingsvrijheid"
-zorg.seperatie = "afzondering of separatie in een daartoe geschikte verblijfsruimte"
-zorg.beperking = "beperking van het recht op het ontvangen van bezoek of het gebruik van communicatiemiddelen"
-zorg.toezicht = "toezicht op betrokkene"
-zorg.onderzoek = "onderzoek aan kleding of lichaam"
-zorg.controle = "controle op de aanwezigheid van gedrag beïnvloedende middelen"
-zorg.beperkingen = "beperkingen in de vrijheid het eigen leven in te richten, die tot gevolg hebben dat betrokkene iets moet doen of nalaten."
-
-wanted = Object()
-wanted.oorzaak = oorzaak
-wanted.pogingen = pogingen
-
-ziekenhuis = Object()
-ziekenhuis.y2010 = 7800
-ziekenhuis.y2011 = 9600
-ziekenhuis.y2012 = 9200
-ziekenhuis.y2013 = 8300
-ziekenhuis.y2014 = 8500
-
-poging = Object()
-poging.ziekenhuis = ziekenhuis.y2014
-poging.seh = seh.y2014
+#:
+gemeenten = """Amsterdam
+Aa en Hunze
+Aalburg
+Aalsmeer
+Aalten
+Achtkarspelen
+Alblasserdam
+Albrandswaard
+Alkmaar
+Almelo
+Almere
+Alphen aan den Rijn
+Alphen-Chaam
+Ameland
+Amersfoort
+Amstelveen
+Amsterdam
+Apeldoorn
+Appingedam
+Arnhem
+Assen
+Asten
+Baarle-Nassau
+Baarn
+Barendrecht
+Barneveld
+Bedum
+Beek
+Beemster
+Beesel
+Bellingwedde
+Bergeijk
+Bergen (Limburg)
+Bergen (Noord-Holland)
+Bergen op Zoom
+Berkelland
+Bernheze
+Best
+Beuningen
+Beverwijk
+Binnenmaas
+Bladel
+Blaricum
+Bloemendaal
+Bodegraven-Reeuwijk
+Boekel
+Bonaire
+Borger-Odoorn
+Borne
+Borsele
+Boxmeer
+Boxtel
+Breda
+Brielle
+Bronckhorst
+Brummen
+Brunssum
+Bunnik
+Bunschoten
+Buren
+Bussum
+Capelle aan den IJssel
+Castricum
+Coevorden
+Cranendonck
+Cromstrijen
+Cuijk
+Culemborg
+Dalfsen
+Dantumadeel
+De Bilt
+De Friese Meren
+De Marne
+De Ronde Venen
+De Wolden
+Delft
+Delfzijl
+Den Haag s-Gravenhage
+Den Helder
+Deurne
+Deventer
+Diemen
+Dinkelland
+Doesburg
+Doetinchem
+Dongen
+Dongeradeel
+Dordrecht
+Drechterland
+Drimmelen
+Dronten
+Druten
+Duiven
+Echt-Susteren
+Edam-Volendam
+Ede
+Eemnes
+Eemsmond
+Eersel
+Eijsden-Margraten
+Eindhoven
+Elburg
+Emmen
+Enkhuizen
+Enschede
+Epe
+Ermelo
+Etten-Leur
+Ferwerderadeel
+Geertruidenberg
+Geldermalsen
+Geldrop-Mierlo
+Gemert-Bakel
+Gennep
+Giessenlanden
+Gilze en Rijen
+Goeree-Overflakkee
+Goes
+Goirle
+Gorinchem (Gorcum of Gorkum)
+Gouda
+Grave
+Groesbeek
+Groningen
+Grootegast
+Gulpen-Wittem
+Haaksbergen
+Haaren
+Haarlem
+Haarlemmermeer
+Halderberge
+Hardenberg
+Harderwijk
+Hardinxveld-Giessendam
+Haren
+Harlingen
+Hattem
+Heemskerk
+Heemstede
+Heerde
+Heerenveen
+Heerhugowaard
+Heerlen
+Heeze-Leende
+Heiloo
+Hellendoorn
+Hellevoetsluis
+Helmond
+Hendrik-Ido-Ambacht
+Hengelo (Overijssel)
+s-Hertogenbosch (Den Bosch)
+Het Bildt
+Heumen
+Heusden
+Hillegom
+Hilvarenbeek
+Hilversum
+Hof van Twente
+Hollands Kroon
+Hoogeveen
+Hoogezand-Sappemeer
+Hoorn
+Horst aan de Maas
+Houten
+Huizen
+Hulst
+IJsselstein
+Kaag en Braassem
+Kampen
+Kapelle
+Katwijk
+Kerkrade
+Koggenland
+Kollumerland en Nieuwkruisland
+Korendijk
+Krimpen aan den IJssel
+Krimpenerwaard
+Laarbeek
+Landerd
+Landgraaf
+Landsmeer
+Langedijk
+Lansingerland
+Laren
+Leek
+Leerdam
+Leeuwarden
+Leeuwarderadeel
+Leiden
+Leiderdorp
+Leidschendam-Voorburg
+Lelystad
+Leudal
+Leusden
+Lingewaal
+Lingewaard
+Lisse
+Littenseradeel
+Lochem
+Loon op Zand
+Lopik
+Loppersum
+Losser
+Maasdriel
+Maasgouw
+Maassluis
+Maastricht
+Marum
+Medemblik
+Meerssen
+Menaldumadeel
+Menterwolde
+Meppel
+Middelburg
+Midden-Delfland
+Midden-Drenthe
+Mill en Sint Hubert
+Moerdijk
+Molenwaard
+Montferland
+Montfoort
+Mook en Middelaar
+Muiden
+Naarden
+Neder-Betuwe
+Nederweert
+Neerijnen
+Nieuwegein
+Nieuwkoop
+Nijkerk
+Nijmegen
+Nissewaard
+Noord-Beveland
+Noordenveld
+Noordoostpolder
+Noordwijk
+Noordwijkerhout
+Nuenen, Gerwen en Nedercoreten
+Nunspeet
+Nuth
+Oegstgeest
+Oirschot
+Oisterwijk
+Oldambt
+Oldebroek
+Oldenzaal
+Olst-Wijhe
+Ommen
+Onderbanken
+Oost Gelre
+Oosterhout
+Ooststellingwerf
+Oostzaan
+Opmeer
+Opsterland
+Oss
+Oud-Beijerland
+Oude IJsselstreek
+Ouder-Amstel
+Oudewater
+Overbetuwe
+Papendrecht
+Peel en Maas
+Pekela
+Pijnacker-Nootdorp
+Purmerend
+Putten
+Raalte
+Reimerswaal
+Renkum
+Renswoude
+Reusel-De Mierden
+Rheden
+Rhenen
+Ridderkerk
+Rijnwaarden
+Rijssen-Holten
+Rijswijk
+Roerdalen
+Roermond
+Roosendaal
+Rotterdam
+Rozendaal
+Rucphen
+Saba
+Schagen
+Scherpenzeel
+Schiedam
+Schiermonnikoog
+Schijndel
+Schinnen
+Schouwen-Duiveland
+Simpelveld
+Sint Anthonis
+Sint Eustatius
+Sint-Michielsgestel
+Sint-Oedenrode
+Sittard-Geleen
+Sliedrecht
+Slochteren
+Sluis
+Smallingerland
+Soest
+Someren
+Son en Breugel
+Stadskanaal
+Staphorst
+Stede Broec
+Steenbergen
+Steenwijkerland
+Stein
+Stichtse Vecht
+Strijen
+Ten Boer
+Terneuzen
+Terschelling
+Texel
+Teylingen
+Tholen
+Tiel
+Tietjerksteradeel
+Tilburg
+Tubbergen
+Twenterand
+Tynaarlo
+Uden
+Uitgeest
+Uithoorn
+Urk
+Utrecht
+Utrechtse Heuvelrug
+Vaals
+Valkenburg aan de Geul
+Valkenswaard
+Veendam
+Veenendaal
+Veere
+Veghel
+Veldhoven
+Velsen
+Venlo
+Venray
+Vianen
+Vlaardingen
+Vlagtwedde
+Vlieland
+Vlissingen
+Voerendaal
+Voorschoten
+Voorst
+Vught
+Waalre
+Waalwijk
+Waddinxveen
+Wageningen
+Wassenaar
+Waterland
+Weert
+Weesp
+Werkendam
+West Maas en Waal
+Westerveld
+Westervoort
+Westland
+Weststellingwerf
+Westvoorne
+Wierden
+Wijchen
+Wijdemeren
+Wijk bij Duurstede
+Winsum
+Winterswijk
+Woensdrecht
+Woerden
+Wormerland
+Woudenberg
+Woudrichem
+Zaanstad
+Zaltbommel
+Zandvoort
+Zederik
+Zeevang
+Zeewolde
+Zeist
+Zevenaar
+Zoetermeer
+Zoeterwoude
+Zuidhorn
+Zuidplas
+Zundert
+Zutphen
+Zwartewaterland
+Zwijndrecht
+Zwolle""".split("\n")
```

