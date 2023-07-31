# Comparing `tmp/president-101.tar.gz` & `tmp/president-110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "president-101.tar", last modified: Sun Jan  8 03:25:02 2023, max compression
+gzip compressed data, was "president-110.tar", last modified: Mon Jul 31 11:30:17 2023, max compression
```

## Comparing `president-101.tar` & `president-110.tar`

### file list

```diff
@@ -1,118 +1,144 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.113036 president-101/
--rw-r--r--   0 bart      (1000) bart      (1000)     3644 2023-01-08 03:25:02.113036 president-101/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     2865 2023-01-08 03:19:33.000000 president-101/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.097036 president-101/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2768 2023-01-08 03:19:33.000000 president-101/bin/president
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.109036 president-101/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)   549426 2023-01-08 03:19:33.000000 president-101/docs/20140730_011.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   262781 2023-01-08 03:19:33.000000 president-101/docs/20151028_009.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   226554 2023-01-08 03:19:33.000000 president-101/docs/20151029_004.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   106616 2023-01-08 03:19:33.000000 president-101/docs/69389.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   142614 2023-01-08 03:19:33.000000 president-101/docs/WvGGZ.txt
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.109036 president-101/docs/_static/
--rw-r--r--   0 bart      (1000) bart      (1000)      785 2023-01-08 03:19:33.000000 president-101/docs/_static/president.css
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.109036 president-101/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1000)      309 2023-01-08 03:19:33.000000 president-101/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      543 2023-01-08 03:19:33.000000 president-101/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      833 2023-01-08 03:19:33.000000 president-101/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2679 2023-01-08 03:19:33.000000 president-101/docs/aangifte.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      450 2023-01-08 03:19:33.000000 president-101/docs/aantallen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      142 2023-01-08 03:19:33.000000 president-101/docs/absoluut.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   270024 2023-01-08 03:19:33.000000 president-101/docs/absoluut2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   538506 2023-01-08 03:19:33.000000 president-101/docs/aes.ico
--rw-r--r--   0 bart      (1000) bart      (1000)    60226 2023-01-08 03:19:33.000000 president-101/docs/aesculaap.ico
--rw-r--r--   0 bart      (1000) bart      (1000)   629595 2023-01-08 03:19:33.000000 president-101/docs/bart.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   449410 2023-01-08 03:19:33.000000 president-101/docs/bart2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      819 2023-01-08 03:19:33.000000 president-101/docs/bedreiging.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    19832 2023-01-08 03:19:33.000000 president-101/docs/besloten.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      137 2023-01-08 03:19:33.000000 president-101/docs/beuker.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   210710 2023-01-08 03:19:33.000000 president-101/docs/bewijsgif3.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      500 2023-01-08 03:19:33.000000 president-101/docs/bijwerking.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1318 2023-01-08 03:19:33.000000 president-101/docs/bijwerkingen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      985 2023-01-08 03:19:33.000000 president-101/docs/clozapine.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     3252 2023-01-08 03:19:33.000000 president-101/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1000)      105 2023-01-08 03:19:33.000000 president-101/docs/contact
--rw-r--r--   0 bart      (1000) bart      (1000)      309 2023-01-08 03:19:33.000000 president-101/docs/contact.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   167276 2023-01-08 03:19:33.000000 president-101/docs/dodelijk.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      942 2023-01-08 03:19:33.000000 president-101/docs/dodelijk.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      222 2023-01-08 03:19:33.000000 president-101/docs/dopamine
--rw-r--r--   0 bart      (1000) bart      (1000)      621 2023-01-08 03:19:33.000000 president-101/docs/echt.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      761 2023-01-08 03:19:33.000000 president-101/docs/ernstig.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1465 2023-01-08 03:19:33.000000 president-101/docs/evrm.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    70170 2023-01-08 03:19:33.000000 president-101/docs/fact.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     4510 2023-01-08 03:19:33.000000 president-101/docs/fact.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    27045 2023-01-08 03:19:33.000000 president-101/docs/fluoxetine.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     6707 2023-01-08 03:19:33.000000 president-101/docs/geinformeerd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   162702 2023-01-08 03:19:33.000000 president-101/docs/gelijk2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      868 2023-01-08 03:19:33.000000 president-101/docs/gif.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     8312 2023-01-08 03:19:33.000000 president-101/docs/greffe.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   180602 2023-01-08 03:19:33.000000 president-101/docs/haarmaken.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     1260 2023-01-08 03:19:33.000000 president-101/docs/hoogeraad.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   566905 2023-01-08 03:19:33.000000 president-101/docs/igz.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      115 2023-01-08 03:19:33.000000 president-101/docs/igz.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     3074 2023-01-08 03:19:33.000000 president-101/docs/index.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      156 2023-01-08 03:19:33.000000 president-101/docs/kamerbrief.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     4052 2023-01-08 03:19:33.000000 president-101/docs/kamerbrief.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     2400 2023-01-08 03:19:33.000000 president-101/docs/kamerbrief2.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2534 2023-01-08 03:19:33.000000 president-101/docs/kamerbrief3.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      871 2023-01-08 03:19:33.000000 president-101/docs/ld50.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      885 2023-01-08 03:19:33.000000 president-101/docs/leven.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      499 2023-01-08 03:19:33.000000 president-101/docs/loggen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-01-08 03:19:33.000000 president-101/docs/mads
--rw-r--r--   0 bart      (1000) bart      (1000)   715150 2023-01-08 03:19:33.000000 president-101/docs/minister.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      142 2023-01-08 03:19:33.000000 president-101/docs/minister.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     4274 2023-01-08 03:19:33.000000 president-101/docs/misdrijf.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2855 2023-01-08 03:19:33.000000 president-101/docs/mishandeling.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   448476 2023-01-08 03:19:33.000000 president-101/docs/nalatig.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    25974 2023-01-08 03:19:33.000000 president-101/docs/nederland.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    23206 2023-01-08 03:19:33.000000 president-101/docs/nederland2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    13101 2023-01-08 03:19:33.000000 president-101/docs/neurotoxisch.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      871 2023-01-08 03:19:33.000000 president-101/docs/om.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      477 2023-01-08 03:19:33.000000 president-101/docs/ontwenning.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      629 2023-01-08 03:19:33.000000 president-101/docs/oorzaak.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      697 2023-01-08 03:19:33.000000 president-101/docs/opzet2.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1281 2023-01-08 03:19:33.000000 president-101/docs/pad.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1860 2023-01-08 03:19:33.000000 president-101/docs/receptoren.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1268 2023-01-08 03:19:33.000000 president-101/docs/recht.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1009 2023-01-08 03:19:33.000000 president-101/docs/risico.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      851 2023-01-08 03:19:33.000000 president-101/docs/schadelijk.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      819 2023-01-08 03:19:33.000000 president-101/docs/sedatie.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      372 2023-01-08 03:19:33.000000 president-101/docs/source.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   180812 2023-01-08 03:19:33.000000 president-101/docs/stoned2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      224 2023-01-08 03:19:33.000000 president-101/docs/symptomen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      802 2023-01-08 03:19:33.000000 president-101/docs/teksten.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      919 2023-01-08 03:19:33.000000 president-101/docs/todo.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2597 2023-01-08 03:19:33.000000 president-101/docs/toxic.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    32684 2023-01-08 03:19:33.000000 president-101/docs/tussenkomst.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)      157 2023-01-08 03:19:33.000000 president-101/docs/tussenkomst.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      149 2023-01-08 03:19:33.000000 president-101/docs/uitspraak.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     6957 2023-01-08 03:19:33.000000 president-101/docs/urls.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    17550 2023-01-08 03:19:33.000000 president-101/docs/verbod.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     1881 2023-01-08 03:19:33.000000 president-101/docs/vergiftiging
--rw-r--r--   0 bart      (1000) bart      (1000)      559 2023-01-08 03:19:33.000000 president-101/docs/vergiftiging.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1407 2023-01-08 03:19:33.000000 president-101/docs/vervolgen.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2043 2023-01-08 03:19:33.000000 president-101/docs/verzoek.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      877 2023-01-08 03:19:33.000000 president-101/docs/wet.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2324 2023-01-08 03:19:33.000000 president-101/docs/wvggz.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   126215 2023-01-08 03:19:33.000000 president-101/docs/zyprexa.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     4443 2023-01-08 03:19:33.000000 president-101/docs/zyprexa.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   236738 2023-01-08 03:19:33.000000 president-101/docs/zyprexa2.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    27393 2023-01-08 03:19:33.000000 president-101/docs/zyprexa3.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   241483 2023-01-08 03:19:33.000000 president-101/docs/zyprexa5.jpg
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.109036 president-101/president/
--rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-01-08 03:19:33.000000 president-101/president/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)    10797 2023-01-08 03:19:33.000000 president-101/president/obj.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3347 2023-01-08 03:19:33.000000 president-101/president/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20169 2023-01-08 03:19:33.000000 president-101/president/run.py
--rw-r--r--   0 bart      (1000) bart      (1000)      251 2023-01-08 03:19:33.000000 president-101/president/slg.py
--rw-r--r--   0 bart      (1000) bart      (1000)    22431 2023-01-08 03:19:33.000000 president-101/president/sui.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3463 2023-01-08 03:19:33.000000 president-101/president/trt.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5813 2023-01-08 03:19:33.000000 president-101/president/wsd.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-01-08 03:25:02.109036 president-101/president.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3644 2023-01-08 03:25:01.000000 president-101/president.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1980 2023-01-08 03:25:02.000000 president-101/president.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-01-08 03:25:01.000000 president-101/president.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-01-08 03:25:01.000000 president-101/president.egg-info/not-zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       10 2023-01-08 03:25:01.000000 president-101/president.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-01-08 03:25:02.113036 president-101/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)     4914 2023-01-08 03:24:07.000000 president-101/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.255043 president-110/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3438 2023-07-31 11:30:17.255043 president-110/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     2865 2023-07-29 12:33:00.000000 president-110/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.247043 president-110/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)   549426 2023-07-29 12:33:00.000000 president-110/docs/20140730_011.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   262781 2023-07-29 12:33:00.000000 president-110/docs/20151028_009.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   226554 2023-07-29 12:33:00.000000 president-110/docs/20151029_004.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   106616 2023-07-29 12:33:00.000000 president-110/docs/69389.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      379 2023-07-30 20:22:11.000000 president-110/docs/BIJWERKING
+-rw-r--r--   0 bart      (1000) bart      (1000)      105 2023-07-30 20:22:29.000000 president-110/docs/CONTACT
+-rw-r--r--   0 bart      (1000) bart      (1000)      222 2023-07-30 20:22:42.000000 president-110/docs/DOPAMINE
+-rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-07-30 20:22:54.000000 president-110/docs/MADS
+-rw-r--r--   0 bart      (1000) bart      (1000)      355 2023-07-30 20:23:19.000000 president-110/docs/ONTWENNING
+-rw-r--r--   0 bart      (1000) bart      (1000)     1803 2023-07-30 20:24:08.000000 president-110/docs/VERGIFTIGING
+-rw-r--r--   0 bart      (1000) bart      (1000)   568504 2023-07-30 20:20:40.000000 president-110/docs/Wetboek-van-Strafrecht.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     5627 2023-07-30 20:24:23.000000 president-110/docs/WvGGZ.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   142614 2023-07-30 20:24:23.000000 president-110/docs/WvGGZ.txt
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.247043 president-110/docs/_static/
+-rw-r--r--   0 bart      (1000) bart      (1000)      785 2023-07-29 12:33:00.000000 president-110/docs/_static/president.css
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.247043 president-110/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1000)      284 2023-07-30 21:00:27.000000 president-110/docs/_templates/base.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      543 2023-07-29 12:33:00.000000 president-110/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      833 2023-07-29 12:33:00.000000 president-110/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2714 2023-07-30 21:03:30.000000 president-110/docs/aangifte.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      481 2023-07-30 21:04:14.000000 president-110/docs/aantallen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1484 2023-07-30 20:15:25.000000 president-110/docs/about.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      175 2023-07-30 21:32:53.000000 president-110/docs/absoluut.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   270024 2023-07-29 12:33:00.000000 president-110/docs/absoluut2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   538506 2023-07-29 12:33:00.000000 president-110/docs/aes.ico
+-rw-r--r--   0 bart      (1000) bart      (1000)    60226 2023-07-29 12:33:00.000000 president-110/docs/aesculaap.ico
+-rw-r--r--   0 bart      (1000) bart      (1000)   629595 2023-07-29 12:33:00.000000 president-110/docs/bart.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   449410 2023-07-29 12:33:00.000000 president-110/docs/bart2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      856 2023-07-30 21:05:30.000000 president-110/docs/bedreiging.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    19832 2023-07-29 12:33:00.000000 president-110/docs/besloten.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      169 2023-07-30 21:06:04.000000 president-110/docs/beuker.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1353 2023-07-30 21:06:37.000000 president-110/docs/bijwerkingen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1021 2023-07-30 21:07:38.000000 president-110/docs/clozapine.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     3333 2023-07-31 05:52:40.000000 president-110/docs/conf.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      345 2023-07-30 21:08:09.000000 president-110/docs/contact.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      977 2023-07-30 21:08:35.000000 president-110/docs/dodelijk.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      657 2023-07-30 21:09:14.000000 president-110/docs/echt.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      798 2023-07-30 21:09:39.000000 president-110/docs/ernstig.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1500 2023-07-30 21:10:02.000000 president-110/docs/evrm.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    70170 2023-07-29 12:33:00.000000 president-110/docs/fact.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)     4545 2023-07-30 21:10:29.000000 president-110/docs/fact.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     6707 2023-07-29 12:33:00.000000 president-110/docs/geinformeerd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   162702 2023-07-29 12:33:00.000000 president-110/docs/gelijk2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      868 2023-07-29 12:33:00.000000 president-110/docs/gif.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     8347 2023-07-30 21:11:02.000000 president-110/docs/greffe.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   180602 2023-07-29 12:33:00.000000 president-110/docs/haarmaken.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)     1295 2023-07-30 21:11:34.000000 president-110/docs/hoogeraad.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   566905 2023-07-29 12:33:00.000000 president-110/docs/igz.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      151 2023-07-30 21:11:59.000000 president-110/docs/igz.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     3096 2023-07-30 20:59:08.000000 president-110/docs/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      193 2023-07-30 21:13:29.000000 president-110/docs/kamerbrief.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2436 2023-07-30 21:12:39.000000 president-110/docs/kamerbrief2.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2571 2023-07-30 21:13:05.000000 president-110/docs/kamerbrief3.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      910 2023-07-30 21:13:58.000000 president-110/docs/ld50.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      922 2023-07-30 21:14:30.000000 president-110/docs/leven.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      537 2023-07-30 21:14:59.000000 president-110/docs/loggen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2555 2023-07-30 21:34:23.000000 president-110/docs/manual.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   715150 2023-07-29 12:33:00.000000 president-110/docs/minister.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      177 2023-07-30 21:15:45.000000 president-110/docs/minister.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     4313 2023-07-30 21:16:17.000000 president-110/docs/misdrijf.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2893 2023-07-30 21:16:46.000000 president-110/docs/mishandeling.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   448476 2023-07-29 12:33:00.000000 president-110/docs/nalatig.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    23206 2023-07-29 12:33:00.000000 president-110/docs/nederland2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    13101 2023-07-29 12:33:00.000000 president-110/docs/neurotoxisch.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)     4787 2023-07-30 21:17:25.000000 president-110/docs/notworking.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      907 2023-07-30 21:17:52.000000 president-110/docs/om.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      629 2023-07-29 12:33:00.000000 president-110/docs/oorzaak.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      734 2023-07-30 21:19:05.000000 president-110/docs/opzet2.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1317 2023-07-30 21:19:30.000000 president-110/docs/pad.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2812 2023-07-30 20:23:33.000000 president-110/docs/realtweedekamer.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1900 2023-07-30 21:20:22.000000 president-110/docs/receptoren.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1307 2023-07-30 21:20:56.000000 president-110/docs/recht.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1047 2023-07-30 21:21:24.000000 president-110/docs/risico.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)       23 2023-07-30 20:14:26.000000 president-110/docs/robots.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      890 2023-07-30 21:22:05.000000 president-110/docs/schadelijk.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      857 2023-07-30 21:22:43.000000 president-110/docs/sedatie.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   287102 2023-07-30 20:19:52.000000 president-110/docs/skull.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     1294 2023-07-30 20:19:07.000000 president-110/docs/source.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   180812 2023-07-29 12:33:00.000000 president-110/docs/stoned2.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      164 2023-07-30 20:23:46.000000 president-110/docs/strafrecht.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      216 2023-07-30 21:02:45.000000 president-110/docs/symptomen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      956 2023-07-30 21:23:36.000000 president-110/docs/todo.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2632 2023-07-30 21:24:01.000000 president-110/docs/toxic.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    32684 2023-07-29 12:33:00.000000 president-110/docs/tussenkomst.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      189 2023-07-30 21:24:36.000000 president-110/docs/tussenkomst.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      181 2023-07-30 21:25:16.000000 president-110/docs/uitspraak.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     6993 2023-07-30 21:25:45.000000 president-110/docs/urls.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    17550 2023-07-29 12:33:00.000000 president-110/docs/verbod.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)      594 2023-07-30 21:26:12.000000 president-110/docs/vergiftiging.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1407 2023-07-29 12:33:00.000000 president-110/docs/vervolgen.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2043 2023-07-29 12:33:00.000000 president-110/docs/verzoek.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      912 2023-07-30 21:26:37.000000 president-110/docs/wet.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2360 2023-07-30 21:26:59.000000 president-110/docs/wvggz.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     4479 2023-07-30 21:27:25.000000 president-110/docs/zyprexa.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.251043 president-110/president/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3122 2023-07-30 11:41:29.000000 president-110/president/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      932 2023-07-30 11:41:29.000000 president-110/president/bus.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1904 2023-07-30 11:41:29.000000 president-110/president/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1559 2023-07-30 11:41:29.000000 president-110/president/define.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1160 2023-07-30 11:41:29.000000 president-110/president/error.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      847 2023-07-30 11:41:29.000000 president-110/president/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2170 2023-07-30 11:41:29.000000 president-110/president/json.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      191 2023-07-30 11:41:29.000000 president-110/president/locks.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.255043 president-110/president/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      431 2023-07-30 11:41:35.000000 president-110/president/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      265 2023-07-30 11:41:35.000000 president-110/president/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-30 11:41:35.000000 president-110/president/modules/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      787 2023-07-30 11:41:35.000000 president-110/president/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      539 2023-07-30 11:41:35.000000 president-110/president/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    19721 2023-07-30 11:41:35.000000 president-110/president/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      933 2023-07-30 11:41:35.000000 president-110/president/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17007 2023-07-30 11:41:35.000000 president-110/president/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      492 2023-07-30 11:41:35.000000 president-110/president/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2359 2023-07-30 11:41:35.000000 president-110/president/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7411 2023-07-30 11:41:35.000000 president-110/president/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      983 2023-07-30 11:41:35.000000 president-110/president/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      394 2023-07-30 11:41:35.000000 president-110/president/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      956 2023-07-30 11:41:35.000000 president-110/president/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1005 2023-07-30 11:41:35.000000 president-110/president/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2989 2023-07-30 11:41:35.000000 president-110/president/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5716 2023-07-30 11:41:35.000000 president-110/president/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5581 2023-07-30 11:41:29.000000 president-110/president/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1299 2023-07-30 11:41:29.000000 president-110/president/parser.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3683 2023-07-30 11:41:29.000000 president-110/president/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2042 2023-07-30 11:41:29.000000 president-110/president/reactor.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1161 2023-07-30 11:41:29.000000 president-110/president/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      104 2023-07-30 11:41:29.000000 president-110/president/run.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1705 2023-07-30 11:41:29.000000 president-110/president/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2506 2023-07-30 11:41:29.000000 president-110/president/utils.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-31 11:30:17.251043 president-110/president.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3438 2023-07-31 11:30:17.000000 president-110/president.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     2630 2023-07-31 11:30:17.000000 president-110/president.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-31 11:30:17.000000 president-110/president.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       57 2023-07-31 11:30:17.000000 president-110/president.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-31 11:30:17.000000 president-110/president.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       10 2023-07-31 11:30:17.000000 president-110/president.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-31 11:30:17.000000 president-110/president.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)     5754 2023-07-31 11:30:06.000000 president-110/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-31 11:30:17.255043 president-110/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-30 19:58:59.000000 president-110/setup.py
```

### Comparing `president-101/PKG-INFO` & `president-110/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,69 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: president
-Version: 101
-Summary: @KarimKhanQC reconsider OTP-CR-117/19
-Home-page: https://bitbucket.org/bthate/president
-Author: Bart Thate
-Author-email: bthate@dds.nl
+Version: 110
+Summary: Reconsidder OTP-CR-117/19
+Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
-Description: 
-        Geachte Minister-President,
-        
-        Ik ben Bart Thate, een 50 jaar oude schizofrenie patient.
-        
-        Op 20 Oktober 2012 heb ik na correspondentie met de Koningin een klacht tegen de Nederland ingedient (Thate tegen Nederland 69389/12). De klacht betrof het falen van de
-        (F)ACT methodiek, de methode die GGZ Nederland gebruikt om vorm te geven aan de wetten die gedwongen behandeling in Nederland mogelijk maken. De uitspraak is niet-ontvankelijk.
-        
-        Omdat de Koningin gemeld heeft dat ze vanwege ministeriele verantwoordelijkheden geen tussenkomst kan bieden, wend ik mij tot u.
-        
-        Er is bewijs dat antipsychotica schadelijk voor de hersenen zijn, bijv. Haldol brengt 4% aantasting van de hippocampus:
-        
-        1) http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3476840/ 
-        2) https://jamanetwork.com/journals/jamapsychiatry/article-abstract/2672208
-        
-        De geneesmiddelenwet zegt dat u stoffen van de geneesmiddelenmarkt dient te halen als deze schadelijk blijken te zijn.
-        Daarom eis ik van u dat u direct medicijnen die gifstoffen blijken te zijn van de geneesmiddelmarkt haalt.
-        
-        Er is bewijs dat antipsychotica gif zijn:
-        
-        1) clozapine (leponex) - https://echa.europa.eu/substance-information/-/substanceinfo/100.024.831
-        2) olanzapine (zyprexa) - https://echa.europa.eu/substance-information/-/substanceinfo/100.125.320
-        3) aripriprazole (abilify) https://echa.europa.eu/substance-information/-/substanceinfo/100.112.532
-        4) haloperiodol (haldol) - https://echa.europa.eu/substance-information/-/substanceinfo/100.000.142
-        
-        Dat het hier gif betreft en niet een onschadelijk medicijn maakt dat men een strafbaar feit pleegt. 
-        Daarom eis ik van u dat u gif toedieningen laat vervolgen door het Openbaar Ministerie.
-        
-        Het is voor mij niet mogelijk gebleken om aangifte te doen van mishandeling als de psychiater zijn patient met gif mishandelt:
-        
-        1) De IGZ treft geen structurele onzorgvuldigheid in de afhandeling van klachten bij GGZ-NHN aan.
-        2) De Hoge Raad concludeert dat het geen verantwoordelijkheid heeft en verwijst naar het Openbaar Ministerie, dat niet reageert.
-        3) Daarna heb ik het Europeese Hof voor de Rechten van de Mens aangeschreven om een klacht tegen Nederland in te dienen.
-        4) Pas na een gang langs het EVRM reageert Het Openbaar Ministerie wel en verwijst naar de IGZ, die de klacht melding al heeft afgesloten.
-        
-        Het ontbreekt de GGZ patient aan een daadwerkelijke remedie om een einde te kunnen maken aan de mishandeling die een arts pleegt als hij gif toedient.
-        Daarom eis ik ook dat u voor de GGZ patient gif toedienende artsen laat vervolgen.
-        
-        Mijn eisen zijn dus:
-        
-        1) medicijnen die gif blijken te zijn van de markt af.
-        2) gif toedieningen door het Openbaar Ministerie laten vervolgen.
-        3) voor de GGZ patient deze vervolging te doen..
-        
-        Er van uitgaande dat u mijn eisen inwilligt,
-        
-        
-        Bart Thate 
-            
-        
-        
-Platform: UNKNOWN
+Project-URL: home, https://pypi.org/project/president
+Project-URL: bugs, https://github.com/bthate/president/issues
+Project-URL: source, https://github.com/bthate/president
 Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+
+MINISTER-PRESIDENT
+##################
+
+Geachte Minister-President,
+
+Ik ben Bart Thate, een 50 jaar oude schizofrenie patient.
+
+Op 20 Oktober 2012 heb ik na correspondentie met de Koningin een klacht tegen de Nederland ingedient (Thate tegen Nederland 69389/12). De klacht betrof het falen van de
+(F)ACT methodiek, de methode die GGZ Nederland gebruikt om vorm te geven aan de wetten die gedwongen behandeling in Nederland mogelijk maken. De uitspraak is niet-ontvankelijk.
+
+Omdat de Koningin gemeld heeft dat ze vanwege ministeriele verantwoordelijkheden geen tussenkomst kan bieden, wend ik mij tot u.
+
+Er is bewijs dat antipsychotica schadelijk voor de hersenen zijn, bijv. Haldol brengt 4% aantasting van de hippocampus:
+
+1) http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3476840/ 
+2) https://jamanetwork.com/journals/jamapsychiatry/article-abstract/2672208
+
+De geneesmiddelenwet zegt dat u stoffen van de geneesmiddelenmarkt dient te halen als deze schadelijk blijken te zijn.
+Daarom eis ik van u dat u direct medicijnen die gifstoffen blijken te zijn van de geneesmiddelmarkt haalt.
+
+Er is bewijs dat antipsychotica gif zijn:
+
+1) haloperiodol (haldol) - https://echa.europa.eu/substance-information/-/substanceinfo/100.000.142
+2) clozapine (leponex) - https://echa.europa.eu/substance-information/-/substanceinfo/100.024.831
+3) olanzapine (zyprexa) - https://echa.europa.eu/substance-information/-/substanceinfo/100.125.320
+4) aripriprazole (abilify) https://echa.europa.eu/substance-information/-/substanceinfo/100.112.532
+
+Dat het hier gif betreft en niet een onschadelijk medicijn maakt dat men een strafbaar feit pleegt. 
+Daarom eis ik van u dat u gif toedieningen laat vervolgen door het Openbaar Ministerie.
+
+Het is voor mij niet mogelijk gebleken om aangifte te doen van mishandeling als de psychiater zijn patient met gif mishandelt:
+
+1) De IGZ treft geen structurele onzorgvuldigheid in de afhandeling van klachten bij GGZ-NHN aan.
+2) De Hoge Raad concludeert dat het geen verantwoordelijkheid heeft en verwijst naar het Openbaar Ministerie, dat niet reageert.
+3) Daarna heb ik het Europeese Hof voor de Rechten van de Mens aangeschreven om een klacht tegen Nederland in te dienen.
+4) Pas na een gang langs het EVRM reageert Het Openbaar Ministerie wel en verwijst naar de IGZ, die de klacht melding al heeft afgesloten.
+
+Het ontbreekt de GGZ patient aan een daadwerkelijke remedie om een einde te kunnen maken aan de mishandeling die een arts pleegt als hij gif toedient.
+Daarom eis ik ook dat u voor de GGZ patient gif toedienende artsen laat vervolgen.
+
+Mijn eisen zijn dus:
+
+1) medicijnen die gif blijken te zijn van de markt af.
+2) gif toedieningen door het Openbaar Ministerie laten vervolgen.
+3) voor de GGZ patient deze vervolging te doen..
+4) de casemanager in de Zorgverzekeringswet.
+
+Er van uitgaande dat u mijn eisen inwilligt,
+
+
+
+Bart Thate
```

### Comparing `president-101/README.rst` & `president-110/README.rst`

 * *Files identical despite different names*

### Comparing `president-101/bin/president` & `president-110/president/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,156 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,W0212,W0611
+# flake8: noqa
+
+
+"runtime"
 
-__version__ = 100
 
-import importlib
 import os
-import pkgutil
-import readline
+
+
+NAME  = __file__.split(os.sep)[-2]
+VERSION = 30
+WORKDIR = os.path.expanduser(f"~/.{NAME}")
+
+
 import sys
-import termios
-import time
 
 
 sys.path.insert(0, os.getcwd())
 
 
-from president.obj import RunCfg, Object, fmt, keys, save
-from president.run import Client, Runtime, Table, elapsed, find, fntime, get_exception
-from president.run import listfiles, spl
+import readline
+import termios
+import threading
+import time
+import _thread
 
 
-RunCfg.wd = os.path.expanduser("~/.president")
+from .bus     import Bus
+from .command import Command, scan
+from .error   import Error, waiter
+from .event   import Event
+from .object  import printable
+from .parser  import parse
+from .persist import Persist
+from .reactor import Reactor
+from .run     import Cfg
+from .thread  import launch
+from .utils   import wait
+from .        import modules
 
 
-class Console(Client):
+Cfg.mod = "cmd,err,log,sts,tdo,thr"
+Persist.workdir = WORKDIR
 
-    def handle(self, clt, e):
-        k.put(e)
-        e.wait()
 
-    def poll(self):
-        return input("> ")
+class CLI(Reactor):
+
+    def __init__(self):
+        Reactor.__init__(self)
+        Bus.add(self)
+        self.register("event", Command.handle)
+
+    def announce(self, txt):
+        pass
 
     def raw(self, txt):
         print(txt)
         sys.stdout.flush()
 
 
-class Kernel(Runtime):
+class Console(CLI):
 
-    def error(self, txt):
-        print(txt)
-        sys.stdout.flush()
 
-    def log(self, txt):
-        if "PONG" in txt or "PING" in txt:
-            return
-        if RunCfg.verbose:
-            print(txt.rstrip())
-            sys.stdout.flush()
-
-
-class Table(Table):
-
-    def addmod(self, mn):
-        spc = importlib.util.find_spec(mn)
-        if not spc:
-            return
-        mod = importlib.import_module(mn)
-        self.introspect(mod)
-
-    def scan(self, pn):
-        spc = importlib.util.find_spec(pn)
-        if not spc:
-            return
-        pkg = importlib.import_module(pn)
-        for mn in pkgutil.walk_packages(pkg.__path__, pn + "."):
-            mod = importlib.import_module(mn.name)
-            if mod:
-                self.introspect(mod)
+    prompting = threading.Event()
+
+    def __init__(self):
+        CLI.__init__(self)
+
+    def handle(self, evt):
+        Command.handle(evt)
+        evt.wait()
 
+    def prompt(self):
+        self.prompting.set()
+        x = input("> ")
+        self.prompting.clear()
+        return x
+        
+    def poll(self):
+        try:
+            return self.event(self.prompt())
+        except EOFError:
+            _thread.interrupt_main()
+      
+
+def banner(cfg):
+    cfgg = printable(cfg, skip="otxt,password")
+    return f"{NAME.upper()} {VERSION} {cfgg}"
+
+
+def cprint(txt):
+    if Console.prompting.is_set():
+        txt = "\n" + txt
+    print(txt)
+    Console.prompting.clear()
+    sys.stdout.flush()
 
 def daemon():
     pid = os.fork()
     if pid != 0:
-        termreset()
         os._exit(0)
     os.setsid()
     os.umask(0)
-    si = open("/dev/null", 'r')
-    so = open("/dev/null", 'a+')
-    se = open("/dev/null", 'a+')
-    os.dup2(si.fileno(), sys.stdin.fileno())
-    os.dup2(so.fileno(), sys.stdout.fileno())
-    os.dup2(se.fileno(), sys.stderr.fileno())
+    sis = open('/dev/null', 'r', encoding="utf-8")
+    os.dup2(sis.fileno(), sys.stdin.fileno())
+    sos = open('/dev/null', 'a+', encoding="utf-8")
+    ses = open('/dev/null', 'a+', encoding="utf-8")
+    os.dup2(sos.fileno(), sys.stdout.fileno())
+    os.dup2(ses.fileno(), sys.stderr.fileno())
 
 
-def wrap(func):
-    fd = sys.stdin.fileno()
-    old = termios.tcgetattr(fd)
+def wrap(func) -> None:
+    old = termios.tcgetattr(sys.stdin.fileno())
     try:
         func()
-    except KeyboardInterrupt:
+    except (EOFError, KeyboardInterrupt):
         print("")
+        sys.stdout.flush()
     finally:
-        termios.tcsetattr(fd, termios.TCSADRAIN, old)
-
+        termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old)
+    waiter()
 
-clt = Console()
-k = Kernel()
-tbl = Table()
 
+def wrapped():
+    wrap(main)
 
-def cmd(event):
-    event.reply(",".join(tbl.modnames))
-
-
-def ver(event):
-    event.reply("KAMER %s" % __version__)
-    
 
 def main():
-    k.boot()
-    tbl.add(cmd)
-    tbl.add(ver)
-    if RunCfg.verbose:
-        k.log("PRESIDENT %s" % __version__)
-        k.log(fmt(RunCfg, ["bork","console","daemon","debug","verbose","wd"]))
-    tbl.scan("president")
-    if RunCfg.verbose:
-        k.log(",".join(tbl.modnames))
-    if k.cfg.txt:
-        return k.cmd(k.cfg.otxt)
-    if RunCfg.daemon:
+    parse(Cfg, " ".join(sys.argv[1:]))
+    if "v" in Cfg.opts:
+        Error.raw = cprint
+        Error.verbose = True
+    if "d" in Cfg.opts:
         daemon()
-    if RunCfg.console or k.cfg.mod:
-        k.start()
-        for mn in spl(k.cfg.mod):
-            k.init("president.%s" % mn)
-        clt.start()
-        k.wait()
-
+        scan(modules, Cfg.mod, True, "a" in Cfg.opts)
+        wait()
+    elif "c" in Cfg.opts:
+        print(banner(Cfg))
+        scan(modules, Cfg.mod, True, "a" in Cfg.opts, True)
+        csl = Console()
+        csl.start()
+        wait()
+    else:
+        cli = CLI()
+        scan(modules, Cfg.mod, False, True)
+        evt = Event()
+        evt.orig = repr(cli)
+        evt.txt = Cfg.otxt
+        evt._thr = launch(Command.handle, evt)
+        evt.wait()
 
-wrap(main)
+if __name__ == "__main__":
+    wrapped()
```

### Comparing `president-101/docs/20140730_011.jpg` & `president-110/docs/20140730_011.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/20151028_009.jpg` & `president-110/docs/20151028_009.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/20151029_004.jpg` & `president-110/docs/20151029_004.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/69389.jpg` & `president-110/docs/69389.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/WvGGZ.txt` & `president-110/docs/WvGGZ.txt`

 * *Files identical despite different names*

### Comparing `president-101/docs/_static/president.css` & `president-110/docs/_static/president.css`

 * *Files identical despite different names*

### Comparing `president-101/docs/_templates/class.rst` & `president-110/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `president-101/docs/_templates/module.rst` & `president-110/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `president-101/docs/aangifte.rst` & `president-110/docs/aangifte.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. title:: aangifte
 
 .. _aangifte:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
+.. raw:: html
+
+    <center>
 
 aangifte
 ========
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 Van: Bart Thate [mailto:bthate@gmail.com<mailto:bthate@gmail.com>]
 Verzonden: dinsdag 16 oktober 2012 21:49
 Aan: AP-Alkmaar (Parket Alkmaar); Info Hoge Raad
 Onderwerp: Re: verzoek aan de officier van justitie om tot strafrechtelijke
```

### Comparing `president-101/docs/absoluut2.jpg` & `president-110/docs/absoluut2.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/aes.ico` & `president-110/docs/aes.ico`

 * *Files identical despite different names*

### Comparing `president-101/docs/aesculaap.ico` & `president-110/docs/aesculaap.ico`

 * *Files identical despite different names*

### Comparing `president-101/docs/bart.jpg` & `president-110/docs/bart.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/bart2.jpg` & `president-110/docs/bart2.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/bedreiging.rst` & `president-110/docs/bedreiging.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 .. _bedreiging:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: bedreiging
 
+
+.. raw:: html
+
+    <center>
+
 bedreiging op het leven
 =======================
 
+
 .. raw:: html
 
+    </center>
     <br>
 
 
 | 285.1 Bedreiging met enig misdrijf tegen het leven gericht wordt gestraft met gevangenisstraf van ten hoogste twee jaren of geldboete van de vierde categorie.
 
 2.3. Voor een veroordeling ter zake van bedreiging met enig misdrijf tegen het leven gericht is in een geval als het onderhavige vereist dat
      de bedreiging  van dien aard is en onder zodanige omstandigheden is geschied dat bij de bedreigde in redelijkheid de vrees kon ontstaan
```

### Comparing `president-101/docs/besloten.jpg` & `president-110/docs/besloten.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/bijwerkingen.rst` & `president-110/docs/bijwerkingen.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 .. _bijwerkingen:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: bijwerkingen
 
 
+.. raw:: html
+
+    <center>
+
 bijwerkingen clozapine
 ======================
 
 .. raw:: html
 
+    </center>
     <br>
 
 Table 10. Adverse Reactions (≥2%) Reported in CLOZARIL-treated Patients (N=842) Across all CLOZARIL Studies (excluding the 2-year InterSePTTM Study)
 
 Body System Adverse Reaction*
 
 CLOZARIL
```

### Comparing `president-101/docs/clozapine.rst` & `president-110/docs/clozapine.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _clozapine:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: clozapine
 
+
+.. raw:: html
+
+    <center>
+
 clozapine
 =========
 
 .. raw:: html
 
+    </center>
     <br>
 
 Clozapine is een dodelijke stof, zie de bijsluiter van de FDA:
 
 https://drive.google.com/open?id=0BwaFXkZBje4OdnBmS05sQ2dkUEE
 
 deze potentieel dodelijk aandoeningen kan men door toediening van clozapine oplopen:
```

### Comparing `president-101/docs/conf.py` & `president-110/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # -- Options for GENERIC output ---------------------------------------------
 
 
 project = __name__
 master_doc = 'index'
 version = '%s' % __version__
 release = '%s' % __version__
-language = ''
+language = 'utf-8'
 today = ''
 today_fmt = '%B %d, %Y'
 needs_sphinx='1.7'
 exclude_patterns = ['_build', '_templates', '_source', 'Thumbs.db', '.DS_Store']
 source_suffix = '.rst'
 source_encoding = 'utf-8-sig'
 modindex_common_prefix = [""]
@@ -85,15 +85,15 @@
     'link_hover': '#000',
     'nosidebar': True,
     'show_powered_by': False,
     'show_relbar_top': False,
     'sidebar_width': 0,
 }
 html_favicon = "aes.ico"
-html_extra_path = []
+html_extra_path = ["robots.txt"]
 html_last_updated_fmt = '%Y-%b-%d'
 html_additional_pages = {}
 html_domain_indices = False
 html_use_index = False
 html_split_index = False
 html_show_sourcelink = False
 html_show_sphinx = False
@@ -106,33 +106,42 @@
 intersphinx_mapping = {
                        'python': ('https://docs.python.org/3', 'objects.inv'),
                        'sphinx': ('http://sphinx.pocoo.org/', None),
                       }
 intersphinx_cache_limit=1
 
 
-rst_prolog = '''.. image:: nederland2.jpg
+rst_prolog = '''.. image:: bewijsgif4.jpg
     :width: 100%
-    :height: 3cm
+    :height: 2.6cm
     :target: index.html
-'''
 
-rst_epilog = """.. raw:: html
+
+.. raw:: html
 
     <br>
-    <center><b>
+
+'''
 
 
-:ref:`home <home>` - :ref:`teksten <teksten>` - :ref:`source <source>`
+rst_epilog = '''.. raw:: html
 
+     <br>
+     <center>
+     <b>
+
+:ref:`home <home>` - :ref:`manual <manual>` - :ref:`source <source>` - :ref:`about <about>`
 
 .. raw:: html
 
-    </b></center>
-"""
+    </b>
+    </center>
+'''
+
+
 autosummary_generate=True
 autodoc_default_flags=['members', 'undoc-members', 'private-members', "imported-members"]
 autodoc_member_order='groupwise'
 autodoc_docstring_signature=True
 autoclass_content="class"
 doctest_global_setup=""
 doctest_global_cleanup=""
```

### Comparing `president-101/docs/dodelijk.rst` & `president-110/docs/dodelijk.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. _dodelijk:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: dodelijk
 
+.. raw:: html
+
+    <center>
+
 dodelijk
 ========
 
 .. raw:: html
 
+    </center>
     <br>
 
 Antipsychotica zijn levenbedreigend, toedienen brengt de kans op sterven:
 
 | Antipsychotica zijn neurotoxisch, zie https://nl.wikipedia.org/wiki/Neurotoxine.
 | Antipsychotica zijn dodelijk, zie :ref:`toxic <toxic>`.
 | Antipsychotica zijn dodelijk, zie bijsluiter van bijv. :ref:`clozapine <clozapine>`.
```

### Comparing `president-101/docs/ernstig.rst` & `president-110/docs/ernstig.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 .. _ernstig:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: ernstig
 
+
+.. raw:: html
+
+
+    <center>
+
 ernstig
 =======
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 Voor de toepassing van deze wet en de daarop berustende bepalingen wordt onder “ernstig nadeel” verstaan, het bestaan van of het aanzienlijk risico op:
 
 levensgevaar, ernstig lichamelijk letsel, ernstige psychische, materiële, immateriële of financiële schade, ernstige verwaarlozing of maatschappelijke teloorgang, ernstig verstoorde ontwikkeling voor of vanbetrokkene of een ander; bedreiging van de veiligheid van betrokkene al dan niet doordat hij onder invloed van een ander raakt;
 de situatie dat betrokkene met hinderlijk gedrag agressie van anderen oproept;
```

### Comparing `president-101/docs/evrm.rst` & `president-110/docs/evrm.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. title:: evrm
 
 .. _evrm:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
+.. raw:: html
+
+    <center>
 
 evrm
 ====
 
 .. raw:: html
 
+    </center>
     <br>
 
 | In 2012 heb ik het Europeese Hof voor de Rechten van de Mens :ref:`aangeschreven <verzoek>` om een klacht tegen Nederland in te dienen.
 | De :ref:`klacht <greffe>` betrof het afwezig zijn van verpleging in het nieuwe ambulante behandeltijdperk van de GGZ.
 | :ref:`Uitspraak <uitspraak>` is niet-ontvankelijk. 
 
 | Het EVRM is voor de GGZ patient een doodlopende weg.
```

### Comparing `president-101/docs/fact.jpg` & `president-110/docs/fact.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/fact.rst` & `president-110/docs/fact.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 .. _fact:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: fact
 
 
+.. raw:: html
+
+    <center>
+
 (f)act
 ======
 
 .. raw:: html
 
+    </center>
     <br>
 
 Brengt het toedienen van gif levensgevaar, het nalaten de noodzakelijke verpleging te leveren brengt de dood:
 
 1. Off-label toedienen.
 
    Off-label toedienen houd in dat er of buiten de toegestaande bloedspiegels toegedient word of dat het medicijnen voor een andere ziekte word toegedient dan waarvoor hij getest is. Dient men hogere waardes toe dan toegestaan dan is men aan het vergiftigen. Dat een arts heden ten dage uberhaupt Off-label mag toedienen is al belachelijk (want per definitie vergiftiging).
```

### Comparing `president-101/docs/geinformeerd.jpg` & `president-110/docs/geinformeerd.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/gelijk2.jpg` & `president-110/docs/gelijk2.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/gif.rst` & `president-110/docs/gif.rst`

 * *Files identical despite different names*

### Comparing `president-101/docs/greffe.rst` & `president-110/docs/greffe.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. _greffe:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: greffe
 
+.. raw:: html
+
+    <center>
+
 greffe
 ======
 
 .. raw:: html
 
+    </center>
     <br>
 
 | 2012/11/8 Bart Thate <bthate@gmail.com<mailto:bthate@gmail.com>
 |
 |                            Le Greffe
 |                            Cour Europeenne des Droits de l'Homme
 |                            Conseil de l'Europe
```

### Comparing `president-101/docs/haarmaken.jpg` & `president-110/docs/haarmaken.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/hoogeraad.rst` & `president-110/docs/hoogeraad.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. _hogeraad:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: hogeraad
 
+.. raw:: html
+
+    <center>
+
 hogeraad
 =========
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 2012/10/22 Info Hoge Raad <info@hogeraad.nl<mailto:info@hogeraad.nl>>
 Geachte heer Thate,
 
 Op 20 september 2012 ontvingen wij per mail uw bericht. Helaas kan de Hoge
```

### Comparing `president-101/docs/igz.jpg` & `president-110/docs/igz.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/index.rst` & `president-110/president.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-.. _home:
+Metadata-Version: 2.1
+Name: president
+Version: 110
+Summary: Reconsidder OTP-CR-117/19
+Author-email: Bart Thate <bthate@dds.nl>
+License: Public Domain
+Project-URL: home, https://pypi.org/project/president
+Project-URL: bugs, https://github.com/bthate/president/issues
+Project-URL: source, https://github.com/bthate/president
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: Public Domain
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 
-.. raw:: html
-
-    <br><br><br>
-
-.. title:: Prosecutor. Court. Reconsider OTP-CR-117/19.
-
-
-minister-president
+MINISTER-PRESIDENT
 ##################
 
-.. raw:: html
-
-    <br>
-
-
 Geachte Minister-President,
 
 Ik ben Bart Thate, een 50 jaar oude schizofrenie patient.
 
 Op 20 Oktober 2012 heb ik na correspondentie met de Koningin een klacht tegen de Nederland ingedient (Thate tegen Nederland 69389/12). De klacht betrof het falen van de
-:ref:`(F)ACT <fact>` methodiek, de methode die GGZ Nederland gebruikt om vorm te geven aan de wetten die gedwongen behandeling in Nederland mogelijk maken. De uitspraak is niet-ontvankelijk.
+(F)ACT methodiek, de methode die GGZ Nederland gebruikt om vorm te geven aan de wetten die gedwongen behandeling in Nederland mogelijk maken. De uitspraak is niet-ontvankelijk.
 
 Omdat de Koningin gemeld heeft dat ze vanwege ministeriele verantwoordelijkheden geen tussenkomst kan bieden, wend ik mij tot u.
 
 Er is bewijs dat antipsychotica schadelijk voor de hersenen zijn, bijv. Haldol brengt 4% aantasting van de hippocampus:
 
 1) http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3476840/ 
 2) https://jamanetwork.com/journals/jamapsychiatry/article-abstract/2672208
@@ -57,18 +60,10 @@
 1) medicijnen die gif blijken te zijn van de markt af.
 2) gif toedieningen door het Openbaar Ministerie laten vervolgen.
 3) voor de GGZ patient deze vervolging te doen..
 4) de casemanager in de Zorgverzekeringswet.
 
 Er van uitgaande dat u mijn eisen inwilligt,
 
-.. raw:: html
 
-    <br><br>
 
 Bart Thate
-
-
-.. toctree::
-    :hidden:
-
-    teksten
```

### Comparing `president-101/docs/kamerbrief2.rst` & `president-110/docs/kamerbrief2.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _kamerbrief2:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: kamerbrief2
 
+
+.. raw:: html
+
+    <center>
+
 kamerbrief2
 ===========
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 
 								   Heerhugowaard, 26 oktober 2015
```

### Comparing `president-101/docs/kamerbrief3.rst` & `president-110/docs/kamerbrief3.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 .. _kamerbrief3:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: kamerbrief3
 
+
+.. raw:: html
+
+    <center>
+
+
 kamerbrief3
 ===========
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 Geachte mevrouw Ricagnoli,
 
 bedankt voor uw reactie op mijn brief van 26 oktober 2015. Ik wil hieronder nog een keer duidelijk maken waarom verplichte behandeling met antipsychotica mishandeling is en dat uw kamer het zich niet kan veroorloven een wet aan te nemen die tot deze mishandeling verplicht EN deze mishandeling daarmee niet strafbaar maakt.
```

### Comparing `president-101/docs/ld50.rst` & `president-110/docs/ld50.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 .. _ld50:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: ld50
 
+
+.. raw:: html
+
+
+    <center>
+
 ld50 oral intake
 ================
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 Cannabidiol:
 
 http://www.chemblink.com/MSDS/MSDSFiles/13956-29-1_Clear%20Synth.pdf
```

### Comparing `president-101/docs/leven.rst` & `president-110/docs/wet.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-.. _leven:
+.. _wet:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
+.. title:: wet
+
+.. raw:: html
 
-.. title:: leven
+    <center>
 
-leven
-=====
+wet
+===
 
 .. raw:: html
 
+    </center>
     <br>
 
 285.1 Bedreiging met enig misdrijf tegen het leven gericht wordt gestraft met gevangenisstraf van ten hoogste twee jaren of geldboete van de vierde categorie.
 
 287   Hij die opzettelijk een ander van het leven berooft, wordt, als schuldig aan doodslag, gestraft met gevangenisstraf van ten hoogste vijftien jaren of geldboete van de vijfde categorie.
 
 289   Hij die opzettelijk en met voorbedachten rade een ander van het leven berooft, wordt, als schuldig aan moord, gestraft met levenslange gevangenisstraf of tijdelijke van ten hoogste dertig jaren of geldboete van de vijfde categorie.
```

### Comparing `president-101/docs/minister.jpg` & `president-110/docs/minister.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/misdrijf.rst` & `president-110/docs/misdrijf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 .. _misdrijven:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: misdrijven
 
+
+.. raw:: html
+
+    <center>
+
+
 misdrijven
 ==========
 
 .. raw:: html
 
+    </center>
     <br>
 
 
 Titel XIX. Misdrijven tegen het leven gericht
 
   Artikel 287
```

### Comparing `president-101/docs/mishandeling.rst` & `president-110/docs/mishandeling.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 .. _mishandeling:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: mishandeling
 
+
+.. raw:: html
+
+    <center>
+
 mishandeling
 ============
 
 .. raw:: html
 
+    </center>
     <br>
 
 “After 17 to 27 months of treatment, both haloperidol- and olanzapine-treated monkeys had an equivalent and highly significant 8% to 11% decrease in fresh brain weight and volume when compared with the sham group.”
 
 .. _bewijs:
 
 "Gerichte schade toebrenging."
```

### Comparing `president-101/docs/nalatig.jpg` & `president-110/docs/nalatig.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/nederland2.jpg` & `president-110/docs/nederland2.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/neurotoxisch.jpg` & `president-110/docs/neurotoxisch.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/om.rst` & `president-110/docs/om.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _om:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: om
 
+
+.. raw:: html
+
+    <center>
+
 om
 ==
 
 .. raw:: html
 
+    </center>
     <br>
 
 | 1 Mon, 14 Jan 2013 11:48:20 +0000 "Keijzer, N.D. (OM Haarlem-Alkmaar)" <n.d.keijzer@om.nl> RE: verzoek aan de officier van justitie om tot strafrechtelijke vervolging over te gaan
 |
 
 | Geachte heer Thate,
```

### Comparing `president-101/docs/oorzaak.rst` & `president-110/docs/oorzaak.rst`

 * *Files identical despite different names*

### Comparing `president-101/docs/opzet2.rst` & `president-110/docs/opzet2.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 .. _opzet:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: opzet
 
+
+.. raw:: html
+
+    <center>
+
 opzet
 =====
 
+
 .. raw:: html
 
+    </center>
     <br>
 
 Aan de (F)ACT methodiek kan men zien dat men een opzet tot vergiftigen heeft, men zegt het toedienen van gif “verantwoord” te kunnen doen:
 
 | men huurt een arts in om te zorgen dat de vergiftiging zorgvuldig gebeurd.
 | men zegt dat de dosis geen schade kan.
 | men geeft een bijsluiter voor de schade die men wel op kan doen.
```

### Comparing `president-101/docs/pad.rst` & `president-110/docs/pad.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _pad:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: pad
 
+
+.. raw:: html
+
+    <center>
+
 pad
 ===
 
 .. raw:: html
 
+    </center>
     <br>
 
 | In 2012 heb ik het Europeese Hof voor de Rechten van de Mens :ref:`aangeschreven <verzoek>` om een klacht tegen Nederland in te dienen.
 | De :ref:`klacht <greffe>` betrof het afwezig zijn van verpleging in het nieuwe ambulante behandeltijdperk van de GGZ.
 | :ref:`Uitspraak <uitspraak>` is niet-ontvankelijk. 
 | Het EVRM is voor de GGZ patient een doodlopende weg.
```

### Comparing `president-101/docs/receptoren.rst` & `president-110/docs/receptoren.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 .. _receptoren:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: receptoren
 
+
+... raw:: html
+
+
+    <center>
+
 receptoren
 ==========
 
 .. raw:: html
 
+    </center>
     <br>
 
 De volgende informatie geldt voor antipsychotica in het algemeen:
 
 Blokkade van dopamine D 2-receptoren in het voorste deel van de hypofyse stimuleert prolactinesecretie en kan leiden tot o.a. gynecomastie, menstruele veranderingen en seksuele dysfunctie [bre, had].
 
 Blokkade van dopamine D 2-receptoren in het voorste deel van de hypothalamus verstoort de temperatuurregulatie, resulterend in hypo- of hyperthermie, afhankelijk van de omgevingstemperatuur [bre, had].
```

### Comparing `president-101/docs/recht.rst` & `president-110/docs/recht.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 .. _recht:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: recht
 
+
+.. raw:: html
+
+     <center>
+
 recht
 =====
 
 .. raw:: html
 
+    </center>
     <br>
 
 | 285.1 Bedreiging met enig misdrijf tegen het leven gericht wordt gestraft met gevangenisstraf van ten hoogste twee jaren of geldboete van de vierde categorie.
 
 | 287   Hij die opzettelijk een ander van het leven berooft, wordt, als schuldig aan doodslag, gestraft met gevangenisstraf van ten hoogste vijftien jaren of geldboete van de vijfde categorie.
 
 | 289   Hij die opzettelijk en met voorbedachten rade een ander van het leven berooft, wordt, als schuldig aan moord, gestraft met levenslange gevangenisstraf of tijdelijke van ten hoogste dertig jaren of geldboete van de vijfde categorie.
```

### Comparing `president-101/docs/risico.rst` & `president-110/docs/risico.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 .. _risico:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: risico
 
+
+.. raw:: html
+
+    <center>
+
 risico
 ======
 
 .. raw:: html
 
+    </center>
     <br>
 
 "Zonder schuldig bevinding !"
 
 Voor de toepassing van deze wet en de daarop berustende bepalingen wordt onder “ernstig nadeel” verstaan, het bestaan van of het aanzienlijk risico op:
 
 | levensgevaar
```

### Comparing `president-101/docs/schadelijk.rst` & `president-110/docs/schadelijk.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 .. _schadelijk:
 
+
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: schadelijk
 
+
+.. raw:: html
+
+    <center>
+
+
 schadelijk
 ==========
 
 .. raw:: html
 
+    </center>
     <br>
 
 “After 17 to 27 months of treatment, both haloperidol- and olanzapine-treated monkeys had an equivalent and highly significant 8% to 11% decrease in fresh brain weight and volume when compared with the sham group.”
 
 Schade zijn de volgende ziektes veroorzaakt door antipsychotica:
 
 | Akathisia
```

### Comparing `president-101/docs/sedatie.rst` & `president-110/docs/sedatie.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 .. _sedatie:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
 
 .. title:: sedatie
 
+
+.. raw:: html
+
+    <center>
+
 sedatie
 =======
 
 .. raw:: html
 
+    </center>
     <br>
 
+
 "Intoxicaties met antipsychotica geven vaak aanleiding tot depressie van het centraal zenuwstelsel (CZS), zich in eerste instantie uitend in sedatie."
 
 Quote van https://vergiftigingen.info, zoek bijv. Zyprexa
 
 Sederen om gevaar te weren, is vergiftiging van de hersenen om tot een depressie van het CZS zodat men in een toestand van sedatie terecht komt.
 Een depressie van het centrale zenuwstelsel kan men een benadeling van de gezondheid noemen, men kan het ook een bedreiging op het leven benoemen.
```

### Comparing `president-101/docs/stoned2.jpg` & `president-110/docs/stoned2.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/todo.rst` & `president-110/docs/todo.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 .. _todo:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: todo
 
+
+.. raw:: html
+
+
+    <center>
+
 todo
 ====
 
 .. raw:: html
 
+    </center>
     <br>
 
 Er moet aangifte tegen de staat gedaan worden voor het op grote schaal overtreden van de eigen wet, namelijk het misdrijf tegen het leven gericht.
 
 Tweede kamer voor de stemming over de Wet verplichte GGZ nog een van het plegen van misdrijven in het kader van die wet benadrukken.
 
 Advocaten email lijst opvragen bij voorzitter van advocatenverenigingen, om zodoende advies te kunnen vragen of er een "class action" achtige aangifte gedaan kan worden ofzo, is stap 1.
```

### Comparing `president-101/docs/toxic.rst` & `president-110/docs/toxic.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. _toxic:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: toxic
 
+.. raw:: html
+
+    <center>
+
 tocix
 =====
 
 .. raw:: html
 
+    </center>
     <br>
 
 Haldol:
 
 | 128 mg/kg [Rat]
 | 71 mg/kg [Mouse]
 | 90 mg/kg [Dog].
```

### Comparing `president-101/docs/tussenkomst.jpg` & `president-110/docs/tussenkomst.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/urls.rst` & `president-110/docs/urls.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _urls:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: urls
 
+
+.. raw:: html
+
+    <center>
+
 urls
 ====
 
 .. raw:: html
 
+    </center>
     <br>
 
 .. _18procent:
 
 18% van de opnames zijn vanwege de medicijnen.
 
 https://www.pw.nl/archief/wp/2013wp02/a1308/at_download/file
```

### Comparing `president-101/docs/verbod.jpg` & `president-110/docs/verbod.jpg`

 * *Files identical despite different names*

### Comparing `president-101/docs/vergiftiging` & `president-110/docs/VERGIFTIGING`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 De medicijnen zijn hoog giftig, gebruik brengt levensgevaar met zich mee en zolang een arts de bloedspiegel van een medicijn niet meet word de toestand van vergiftiging niet opgeheven. Dodelijk als de noodzakelijke verpleging niet aanwezig is om medicijnen snel af te bouwen.
-
  
 mild
-~~~~
-
-.. raw:: html
-
-    <br>
+====
 
 1) gedragsveranderingen (bijv., rusteloosheid, crankiness)
 2) diarree
 3) duizeligheid
 4) slaperigheid
 5) vermoeidheid
 6) hoofdpijn
 7) verlies van eetlust
 8) kleine huid- of oogirritaties
 9) misselijkheid of maagklachten
 10) passen hoest (hoest die komt en gaat)
 11) pijn of stijfheid in de gewrichten
 12) dorst
 
-
 matig
-~~~~~
-
-.. raw:: html
-
-    <br>
+=====
 
 1) wazig zicht
 2) Verwarring en desoriëntatie
 3) ademhalingsproblemen
 4) kwijlen
 5) overmatig tranen
 6) koorts
@@ -45,21 +35,16 @@
 14) ernstige misselijkheid
 15) maagkrampen
 16) zweten
 17) dorst
 18) bevend
 19) zwakte
 
-
 ernstig
-~~~~~~~
-
-.. raw:: html
-
-    <br>
+=======
 
 1) hartstilstand
 2) krampen
 3) diffuse intravasale stolling (mits ongecontroleerde bloeden of bloedstolling veroorzaakt)
 4) oesofageale vernauwing (vernauwing van het orgaan dat voedsel uit de mond draagt naar de maag)
 5) koorts (vaak hoog)
 6) onvermogen om te ademen
```

### Comparing `president-101/docs/vergiftiging.rst` & `president-110/docs/vergiftiging.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .. _vergiftiging:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: vergiftiging
 
+.. raw:: html
+
+    <center>
+
 vergiftiging
 ============
 
 .. raw:: html
 
+    </center>
     <br>
 
 “Test toont dat men aan het vergiftigen is. De bijwerkingen zijn vergiftigingssymptomen.”
 
 Table 9. Common Adverse Reactions (≥5%) in the 6-Week, Randomized, Chlorpromazine-controlled Trial in Treatment-Resistant Schizophrenia:
 
 | Sedation 21
```

### Comparing `president-101/docs/vervolgen.rst` & `president-110/docs/vervolgen.rst`

 * *Files identical despite different names*

### Comparing `president-101/docs/verzoek.rst` & `president-110/docs/verzoek.rst`

 * *Files identical despite different names*

### Comparing `president-101/docs/wet.rst` & `president-110/docs/leven.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-.. _wet:
+.. _leven:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
+
+.. title:: leven
+
+
+.. raw:: html
+
+    <center>
 
-.. title:: wet
 
-wet
-===
+leven
+=====
 
 .. raw:: html
 
+    </center>
     <br>
 
 285.1 Bedreiging met enig misdrijf tegen het leven gericht wordt gestraft met gevangenisstraf van ten hoogste twee jaren of geldboete van de vierde categorie.
 
 287   Hij die opzettelijk een ander van het leven berooft, wordt, als schuldig aan doodslag, gestraft met gevangenisstraf van ten hoogste vijftien jaren of geldboete van de vijfde categorie.
 
 289   Hij die opzettelijk en met voorbedachten rade een ander van het leven berooft, wordt, als schuldig aan moord, gestraft met levenslange gevangenisstraf of tijdelijke van ten hoogste dertig jaren of geldboete van de vijfde categorie.
```

### Comparing `president-101/docs/wvggz.rst` & `president-110/docs/wvggz.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _wvggz:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: wvggz
 
+
+.. raw:: html
+
+    <center>
+
 wvggz
 =====
 
 .. raw:: html
 
+    </center>
     <br>
 
 Peter C. Gotzsche heeft de Tweede Kamer op 29 maart 2016 geinformeerd over de dodelijkheid van psychiatrische medicijnen. 
 De Tweede Kamer is dus op de hoogte dat het om gif gaat en niet om medicijnen. Ook de minister weet dat het hier om gif gaat, 
 maar maakt de max. dosis bekend waarmee de stof geacht word niet giftig te zijn en geen schade aan de patient te brengen. 
 Natuurlijk is het onzin dat een gif onder een bepaalde dosis niet meer giftig zou zijn. De bijsluiters tonen waar men risico 
 op loopt door deze stoffen wel toe te dienen. Een behandelplan met elke dag risico voor de patient ook dat dat risico ook plaats
```

### Comparing `president-101/docs/zyprexa.rst` & `president-110/docs/zyprexa.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .. _zyprexa:
 
 .. raw:: html
 
-    <br><br><br>
+    <br>
 
 .. title:: zyprexa
 
+
+.. raw:: html
+
+    <center>
+
 zyprexa
 =======
 
 .. raw:: html
 
+    </center>
     <br>
 
 4. MOGELIJKE BIJWERKINGEN
 
 Zoals elk geneesmiddel kan dit geneesmiddel bijwerkingen hebben, al krijgt niet iedereen daarmee te
 maken.
```

### Comparing `president-101/president/wsd.py` & `president-110/president/modules/wsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is placed in the Public Domain.
 #
-# EM_T04_OTP-CR-117_19 otp.informationdesk@icc-cpi.int https://genocide.rtfd.io
+# pylint: disable=C,I,R
+# flake8: noqa=E501
 
-"the trip in between"
 
-#:
-txt = """| wijsheid, wijs !
+"""| wijsheid, wijs !
 
 | OVERDRACHT
 | ==========
 
 | No Voice, No Description:
 
 | enkelt eenlingen
@@ -183,14 +182,13 @@
 | brievenbus en graf
 | twee eieren (gemeente huis en buiging naar west)
 | vreedevernoeming
 | duiding
 | coding
 """
 
+
 import random
 
-def register(k):
-    k.addcmd(wsd)
 
 def wsd(event):
-    event.reply(random.choice(txt.split("\n")).strip()[2:])
+    event.reply(random.choice(__doc__.split("\n")).strip()[2:])
```

### Comparing `president-101/president.egg-info/PKG-INFO` & `president-110/docs/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,80 @@
-Metadata-Version: 1.1
-Name: president
-Version: 101
-Summary: @KarimKhanQC reconsider OTP-CR-117/19
-Home-page: https://bitbucket.org/bthate/president
-Author: Bart Thate
-Author-email: bthate@dds.nl
-License: Public Domain
-Description: 
-        Geachte Minister-President,
-        
-        Ik ben Bart Thate, een 50 jaar oude schizofrenie patient.
-        
-        Op 20 Oktober 2012 heb ik na correspondentie met de Koningin een klacht tegen de Nederland ingedient (Thate tegen Nederland 69389/12). De klacht betrof het falen van de
-        (F)ACT methodiek, de methode die GGZ Nederland gebruikt om vorm te geven aan de wetten die gedwongen behandeling in Nederland mogelijk maken. De uitspraak is niet-ontvankelijk.
-        
-        Omdat de Koningin gemeld heeft dat ze vanwege ministeriele verantwoordelijkheden geen tussenkomst kan bieden, wend ik mij tot u.
-        
-        Er is bewijs dat antipsychotica schadelijk voor de hersenen zijn, bijv. Haldol brengt 4% aantasting van de hippocampus:
-        
-        1) http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3476840/ 
-        2) https://jamanetwork.com/journals/jamapsychiatry/article-abstract/2672208
-        
-        De geneesmiddelenwet zegt dat u stoffen van de geneesmiddelenmarkt dient te halen als deze schadelijk blijken te zijn.
-        Daarom eis ik van u dat u direct medicijnen die gifstoffen blijken te zijn van de geneesmiddelmarkt haalt.
-        
-        Er is bewijs dat antipsychotica gif zijn:
-        
-        1) clozapine (leponex) - https://echa.europa.eu/substance-information/-/substanceinfo/100.024.831
-        2) olanzapine (zyprexa) - https://echa.europa.eu/substance-information/-/substanceinfo/100.125.320
-        3) aripriprazole (abilify) https://echa.europa.eu/substance-information/-/substanceinfo/100.112.532
-        4) haloperiodol (haldol) - https://echa.europa.eu/substance-information/-/substanceinfo/100.000.142
-        
-        Dat het hier gif betreft en niet een onschadelijk medicijn maakt dat men een strafbaar feit pleegt. 
-        Daarom eis ik van u dat u gif toedieningen laat vervolgen door het Openbaar Ministerie.
-        
-        Het is voor mij niet mogelijk gebleken om aangifte te doen van mishandeling als de psychiater zijn patient met gif mishandelt:
-        
-        1) De IGZ treft geen structurele onzorgvuldigheid in de afhandeling van klachten bij GGZ-NHN aan.
-        2) De Hoge Raad concludeert dat het geen verantwoordelijkheid heeft en verwijst naar het Openbaar Ministerie, dat niet reageert.
-        3) Daarna heb ik het Europeese Hof voor de Rechten van de Mens aangeschreven om een klacht tegen Nederland in te dienen.
-        4) Pas na een gang langs het EVRM reageert Het Openbaar Ministerie wel en verwijst naar de IGZ, die de klacht melding al heeft afgesloten.
-        
-        Het ontbreekt de GGZ patient aan een daadwerkelijke remedie om een einde te kunnen maken aan de mishandeling die een arts pleegt als hij gif toedient.
-        Daarom eis ik ook dat u voor de GGZ patient gif toedienende artsen laat vervolgen.
-        
-        Mijn eisen zijn dus:
-        
-        1) medicijnen die gif blijken te zijn van de markt af.
-        2) gif toedieningen door het Openbaar Ministerie laten vervolgen.
-        3) voor de GGZ patient deze vervolging te doen..
-        
-        Er van uitgaande dat u mijn eisen inwilligt,
-        
-        
-        Bart Thate 
-            
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Topic :: Utilities
+.. _home:
+
+.. raw:: html
+
+    <br>
+
+.. title:: Prosecutor. Court. Reconsider OTP-CR-117/19.
+
+
+.. raw:: html
+
+    <center>
+
+president
+#########
+
+.. raw:: html
+
+    </center>
+    <br>
+
+
+Geachte Minister-President,
+
+Ik ben Bart Thate, een 50 jaar oude schizofrenie patient.
+
+Op 20 Oktober 2012 heb ik na correspondentie met de Koningin een klacht tegen de Nederland ingedient (Thate tegen Nederland 69389/12). De klacht betrof het falen van de
+:ref:`(F)ACT <fact>` methodiek, de methode die GGZ Nederland gebruikt om vorm te geven aan de wetten die gedwongen behandeling in Nederland mogelijk maken. De uitspraak is niet-ontvankelijk.
+
+Omdat de Koningin gemeld heeft dat ze vanwege ministeriele verantwoordelijkheden geen tussenkomst kan bieden, wend ik mij tot u.
+
+Er is bewijs dat antipsychotica schadelijk voor de hersenen zijn, bijv. Haldol brengt 4% aantasting van de hippocampus:
+
+1) http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3476840/ 
+2) https://jamanetwork.com/journals/jamapsychiatry/article-abstract/2672208
+
+De geneesmiddelenwet zegt dat u stoffen van de geneesmiddelenmarkt dient te halen als deze schadelijk blijken te zijn.
+Daarom eis ik van u dat u direct medicijnen die gifstoffen blijken te zijn van de geneesmiddelmarkt haalt.
+
+Er is bewijs dat antipsychotica gif zijn:
+
+1) haloperiodol (haldol) - https://echa.europa.eu/substance-information/-/substanceinfo/100.000.142
+2) clozapine (leponex) - https://echa.europa.eu/substance-information/-/substanceinfo/100.024.831
+3) olanzapine (zyprexa) - https://echa.europa.eu/substance-information/-/substanceinfo/100.125.320
+4) aripriprazole (abilify) https://echa.europa.eu/substance-information/-/substanceinfo/100.112.532
+
+Dat het hier gif betreft en niet een onschadelijk medicijn maakt dat men een strafbaar feit pleegt. 
+Daarom eis ik van u dat u gif toedieningen laat vervolgen door het Openbaar Ministerie.
+
+Het is voor mij niet mogelijk gebleken om aangifte te doen van mishandeling als de psychiater zijn patient met gif mishandelt:
+
+1) De IGZ treft geen structurele onzorgvuldigheid in de afhandeling van klachten bij GGZ-NHN aan.
+2) De Hoge Raad concludeert dat het geen verantwoordelijkheid heeft en verwijst naar het Openbaar Ministerie, dat niet reageert.
+3) Daarna heb ik het Europeese Hof voor de Rechten van de Mens aangeschreven om een klacht tegen Nederland in te dienen.
+4) Pas na een gang langs het EVRM reageert Het Openbaar Ministerie wel en verwijst naar de IGZ, die de klacht melding al heeft afgesloten.
+
+Het ontbreekt de GGZ patient aan een daadwerkelijke remedie om een einde te kunnen maken aan de mishandeling die een arts pleegt als hij gif toedient.
+Daarom eis ik ook dat u voor de GGZ patient gif toedienende artsen laat vervolgen.
+
+Mijn eisen zijn dus:
+
+1) medicijnen die gif blijken te zijn van de markt af.
+2) gif toedieningen door het Openbaar Ministerie laten vervolgen.
+3) voor de GGZ patient deze vervolging te doen..
+4) de casemanager in de Zorgverzekeringswet.
+
+Er van uitgaande dat u mijn eisen inwilligt,
+
+.. raw:: html
+
+    <br><br>
+
+Bart Thate
+
+
+.. toctree::
+    :glob:
+    :hidden:
+
+    *
```

