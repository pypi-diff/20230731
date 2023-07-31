# Comparing `tmp/tomoscan-1.3.0a2.tar.gz` & `tmp/tomoscan-1.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomoscan-1.3.0a2.tar", last modified: Wed Jun 21 13:51:30 2023, max compression
+gzip compressed data, was "tomoscan-1.3.0a4.tar", last modified: Mon Jul 31 13:43:32 2023, max compression
```

## Comparing `tomoscan-1.3.0a2.tar` & `tomoscan-1.3.0a4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/
--rw-r--r--   0 payno     (1001) payno     (1001)     1253 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/LICENSE
--rw-r--r--   0 payno     (1001) payno     (1001)      953 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)      609 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/README.md
--rw-r--r--   0 payno     (1001) payno     (1001)     1213 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/setup.cfg
--rw-r--r--   0 payno     (1001) payno     (1001)     1486 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/setup.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan/
--rw-r--r--   0 payno     (1001) payno     (1001)       67 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan/esrf/
--rw-r--r--   0 payno     (1001) payno     (1001)     1992 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)      263 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/edfscan.py
--rw-r--r--   0 payno     (1001) payno     (1001)      266 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/hdf5scan.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan/esrf/identifier/
--rw-r--r--   0 payno     (1001) payno     (1001)     1765 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2926 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/edfidentifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5467 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/folderidentifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/hdf5Identifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2302 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/jp2kidentifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2732 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/rawidentifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3621 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/tiffidentifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2431 2023-06-21 13:50:57.000000 tomoscan-1.3.0a2/tomoscan/esrf/identifier/url_utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)      254 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/mock.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/esrf/scan/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    44250 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/edfscan.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/
--rw-r--r--   0 payno     (1001) payno     (1001)      118 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    25256 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/edfframereducer.py
--rw-r--r--   0 payno     (1001) payno     (1001)     8542 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
--rw-r--r--   0 payno     (1001) payno     (1001)    57936 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/hdf5scan.py
--rw-r--r--   0 payno     (1001) payno     (1001)    37157 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/mock.py
--rw-r--r--   0 payno     (1001) payno     (1001)    22716 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/scan/utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)      257 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/utils.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/esrf/volume/
--rw-r--r--   0 payno     (1001) payno     (1001)     1637 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5369 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/edfvolume.py
--rw-r--r--   0 payno     (1001) payno     (1001)    19300 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/hdf5volume.py
--rw-r--r--   0 payno     (1001) payno     (1001)     8962 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/jp2kvolume.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3035 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/mock.py
--rw-r--r--   0 payno     (1001) payno     (1001)    17047 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/rawvolume.py
--rw-r--r--   0 payno     (1001) payno     (1001)    15152 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/singleframebase.py
--rw-r--r--   0 payno     (1001) payno     (1001)    17517 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/tiffvolume.py
--rw-r--r--   0 payno     (1001) payno     (1001)     9222 2023-06-21 13:43:50.000000 tomoscan-1.3.0a2/tomoscan/esrf/volume/utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)    10032 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/factory.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3757 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/framereducerbase.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2434 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/identifier.py
--rw-r--r--   0 payno     (1001) payno     (1001)     6006 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/io.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/nexus/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.670940 tomoscan-1.3.0a2/tomoscan/nexus/paths/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)      831 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxdetector.py
--rw-r--r--   0 payno     (1001) payno     (1001)      406 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxinstrument.py
--rw-r--r--   0 payno     (1001) payno     (1001)      250 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxmonitor.py
--rw-r--r--   0 payno     (1001) payno     (1001)      540 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxsample.py
--rw-r--r--   0 payno     (1001) payno     (1001)      276 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxsource.py
--rw-r--r--   0 payno     (1001) payno     (1001)    11151 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/nexus/paths/nxtomo.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5438 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/normalization.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3214 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/progress.py
--rw-r--r--   0 payno     (1001) payno     (1001)    67019 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/scanbase.py
--rw-r--r--   0 payno     (1001) payno     (1001)      303 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/scanfactory.py
--rw-r--r--   0 payno     (1001) payno     (1001)     8224 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/serie.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.674940 tomoscan-1.3.0a2/tomoscan/test/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)      266 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/conftest.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1732 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_framereducerbase.py
--rw-r--r--   0 payno     (1001) payno     (1001)      451 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_hdf5_utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2850 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_io.py
--rw-r--r--   0 payno     (1001) payno     (1001)     7466 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_normalization.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2013 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_progress.py
--rw-r--r--   0 payno     (1001) payno     (1001)     8996 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_scanbase.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4569 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_scanfactory.py
--rw-r--r--   0 payno     (1001) payno     (1001)     6223 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_serie.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1611 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_tomoobject.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3704 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)    11616 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_validator.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1502 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_version.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2933 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/test_volume_base.py
--rw-r--r--   0 payno     (1001) payno     (1001)     6186 2023-06-21 13:43:50.000000 tomoscan-1.3.0a2/tomoscan/test/test_volume_utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)     8574 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/test/utils.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2341 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/tomoobject.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/tomoscan/unitsystem/
--rw-r--r--   0 payno     (1001) payno     (1001)     1657 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2447 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/electriccurrentsystem.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3270 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/energysystem.py
--rw-r--r--   0 payno     (1001) payno     (1001)     6542 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/metricsystem.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3165 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/timesystem.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1846 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/unit.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1975 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/unitsystem/voltagesystem.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.678940 tomoscan-1.3.0a2/tomoscan/utils/
--rw-r--r--   0 payno     (1001) payno     (1001)      175 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1120 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/decorator.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2976 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/geometry.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2666 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/hdf5.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1512 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/io.py
--rw-r--r--   0 payno     (1001) payno     (1001)     8884 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/utils/volume.py
--rw-r--r--   0 payno     (1001) payno     (1001)    17014 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/validator.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4346 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/version.py
--rw-r--r--   0 payno     (1001) payno     (1001)    21351 2023-06-21 13:33:06.000000 tomoscan-1.3.0a2/tomoscan/volumebase.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-21 13:51:30.666940 tomoscan-1.3.0a2/tomoscan.egg-info/
--rw-r--r--   0 payno     (1001) payno     (1001)      953 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)     2741 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1001) payno     (1001)      300 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/requires.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        9 2023-06-21 13:51:30.000000 tomoscan-1.3.0a2/tomoscan.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1253 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)      953 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      609 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     1213 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1486 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan/
+-rw-r--r--   0 payno     (1000) payno     (1000)       67 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan/esrf/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1992 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      263 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/edfscan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      266 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/hdf5scan.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan/esrf/identifier/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1765 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2926 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/edfidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5467 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/folderidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5781 2023-07-20 08:59:28.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/hdf5Identifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2302 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/jp2kidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2732 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/rawidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3621 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/tiffidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2431 2023-07-20 08:59:28.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/url_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      254 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/mock.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.174681 tomoscan-1.3.0a4/tomoscan/esrf/scan/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    44382 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/edfscan.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.174681 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/
+-rw-r--r--   0 payno     (1000) payno     (1000)      118 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25256 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/edfframereducer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8542 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    58068 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/hdf5scan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    37157 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/mock.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22858 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      257 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.174681 tomoscan-1.3.0a4/tomoscan/esrf/volume/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1637 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5369 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/edfvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19300 2023-07-20 08:59:28.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/hdf5volume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8962 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/jp2kvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3035 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/mock.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17047 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/rawvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15152 2023-07-20 08:50:33.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/singleframebase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17517 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/tiffvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9222 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10102 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/factory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3757 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/framereducerbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2434 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/identifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6006 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.178681 tomoscan-1.3.0a4/tomoscan/nexus/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.178681 tomoscan-1.3.0a4/tomoscan/nexus/paths/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      831 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      406 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      250 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      540 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      276 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11151 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5438 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3214 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/progress.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    67365 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/scanbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      303 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/scanfactory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8224 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/serie.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/tomoscan/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      266 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/conftest.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1732 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_framereducerbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      451 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_hdf5_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2850 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_io.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7466 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2013 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_progress.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8996 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_scanbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4569 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_scanfactory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6223 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_serie.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1611 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_tomoobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3704 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11616 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_validator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1502 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_version.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2933 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_volume_base.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6186 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_volume_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8574 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2341 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/tomoobject.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/tomoscan/unitsystem/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1657 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2447 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/electriccurrentsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3270 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/energysystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6542 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/metricsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3165 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/timesystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1846 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/unit.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1975 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/voltagesystem.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/tomoscan/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)      175 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1120 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/decorator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2976 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/geometry.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2666 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/hdf5.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1512 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/io.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8884 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/volume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17014 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/validator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4346 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/version.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21318 2023-07-27 11:43:47.000000 tomoscan-1.3.0a4/tomoscan/volumebase.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)      953 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     2741 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      300 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        9 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/top_level.txt
```

### Comparing `tomoscan-1.3.0a2/LICENSE` & `tomoscan-1.3.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/PKG-INFO` & `tomoscan-1.3.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a2
+Version: 1.3.0a4
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a2/README.md` & `tomoscan-1.3.0a4/README.md`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/setup.cfg` & `tomoscan-1.3.0a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/setup.py` & `tomoscan-1.3.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/__init__.py` & `tomoscan-1.3.0a4/tomoscan/esrf/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/__init__.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/edfidentifier.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/edfidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/folderidentifier.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/folderidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/hdf5Identifier.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/hdf5Identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/jp2kidentifier.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/jp2kidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/rawidentifier.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/rawidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/tiffidentifier.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/tiffidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/identifier/url_utils.py` & `tomoscan-1.3.0a4/tomoscan/esrf/identifier/url_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/scan/edfscan.py` & `tomoscan-1.3.0a4/tomoscan/esrf/scan/edfscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1211,24 +1211,26 @@
     @docstring(TomoScanBase)
     def save_reduced_darks(
         self,
         darks: dict,
         output_urls: tuple = REDUCED_DARKS_DATAURLS,
         darks_infos=None,
         metadata_output_urls=REDUCED_DARKS_METADATAURLS,
+        overwrite: bool = False,
     ):
         if len(darks) > 1:
             _logger.warning(
                 "EDFTomoScan expect at most one dark. Only one will be save"
             )
         super().save_reduced_darks(
             darks=darks,
             output_urls=output_urls,
             darks_infos=darks_infos,
             metadata_output_urls=metadata_output_urls,
+            overwrite=overwrite,
         )
 
     @docstring(TomoScanBase)
     def load_reduced_darks(
         self,
         inputs_urls: tuple = REDUCED_DARKS_DATAURLS,
         metadata_input_urls: tuple = REDUCED_DARKS_METADATAURLS,
@@ -1254,20 +1256,22 @@
     @docstring(TomoScanBase)
     def save_reduced_flats(
         self,
         flats: dict,
         output_urls: tuple = REDUCED_FLATS_DATAURLS,
         flats_infos=None,
         metadata_output_urls=REDUCED_FLATS_METADATAURLS,
+        overwrite: bool = False,
     ) -> dict:
         super().save_reduced_flats(
             flats=flats,
             output_urls=output_urls,
             flats_infos=flats_infos,
             metadata_output_urls=metadata_output_urls,
+            overwrite=overwrite,
         )
 
     @docstring(TomoScanBase)
     def load_reduced_flats(
         self,
         inputs_urls: tuple = REDUCED_FLATS_DATAURLS,
         metadata_input_urls: tuple = REDUCED_FLATS_METADATAURLS,
```

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/edfframereducer.py` & `tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/edfframereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/scan/framereducer/hdf5framereducer.py` & `tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/hdf5framereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/scan/hdf5scan.py` & `tomoscan-1.3.0a4/tomoscan/esrf/scan/hdf5scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1259,23 +1259,25 @@
     @docstring(TomoScanBase)
     def save_reduced_darks(
         self,
         darks: dict,
         output_urls: tuple = REDUCED_DARKS_DATAURLS,
         darks_infos=None,
         metadata_output_urls=REDUCED_DARKS_METADATAURLS,
+        overwrite: bool = False,
     ):
         """
         Dump computed dark (median / mean...) into files
         """
         super().save_reduced_darks(
             darks=darks,
             output_urls=output_urls,
             darks_infos=darks_infos,
             metadata_output_urls=metadata_output_urls,
+            overwrite=overwrite,
         )
 
     @docstring(TomoScanBase)
     def load_reduced_darks(
         self,
         inputs_urls: tuple = REDUCED_DARKS_DATAURLS,
         metadata_input_urls=REDUCED_DARKS_METADATAURLS,
@@ -1295,23 +1297,25 @@
     @docstring(TomoScanBase)
     def save_reduced_flats(
         self,
         flats: dict,
         output_urls: tuple = REDUCED_FLATS_DATAURLS,
         flats_infos=None,
         metadata_output_urls: tuple = REDUCED_FLATS_METADATAURLS,
+        overwrite: bool = False,
     ) -> dict:
         """
         Dump computed flats (median / mean...) into files
         """
         super().save_reduced_flats(
             flats=flats,
             metadata_output_urls=metadata_output_urls,
             output_urls=output_urls,
             flats_infos=flats_infos,
+            overwrite=overwrite,
         )
 
     @docstring(TomoScanBase)
     def load_reduced_flats(
         self,
         inputs_urls: tuple = REDUCED_FLATS_DATAURLS,
         metadata_input_urls=REDUCED_FLATS_METADATAURLS,
```

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/scan/mock.py` & `tomoscan-1.3.0a4/tomoscan/esrf/scan/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/scan/utils.py` & `tomoscan-1.3.0a4/tomoscan/esrf/scan/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,15 +497,19 @@
                         )
     else:
         # for other file format don't need to do the same
         return silx_get_data(url)
 
 
 def copy_h5_dict_darks_to(
-    scan, darks_url: DataUrl, save=False, raise_error_if_url_empty=True
+    scan,
+    darks_url: DataUrl,
+    save: bool = False,
+    raise_error_if_url_empty: bool = True,
+    overwrite: bool = False,
 ):
     """
     :param TomwerScanBase scan: target to copy darks
     :param DataUrl darks_url: DataUrl to find darks to be copied
     :param bool save: should we save the darks to disk. If not will only be set on scan cache
     :param bool raise_error_if_url_empty: if the provided DataUrl lead to now data shoudl we raise an error (like file or dataset missing...)
     """
@@ -533,19 +537,23 @@
         else:
             return
     data, metadata = ReducedFramesInfos.split_data_and_metadata(my_dict)
     # handle relative frame position if any
     data = from_relative_reduced_frames_to_absolute(reduced_frames=data, scan=scan)
     scan.set_reduced_darks(darks=data, darks_infos=metadata)
     if save:
-        scan.save_reduced_darks(darks=data, darks_infos=metadata)
+        scan.save_reduced_darks(darks=data, darks_infos=metadata, overwrite=overwrite)
 
 
 def copy_h5_dict_flats_to(
-    scan, flats_url: DataUrl, save=False, raise_error_if_url_empty=True
+    scan,
+    flats_url: DataUrl,
+    save=False,
+    raise_error_if_url_empty=True,
+    overwrite: bool = False,
 ):
     """
     :param TomwerScanBase scan: target to copy darks
     :param DataUrl darks_url: DataUrl to find darks to be copied
     :param bool save: should we save the darks to disk. If not will only be set on scan cache
     :param bool raise_error_if_url_empty: if the provided DataUrl lead to now data shoudl we raise an error (like file or dataset missing...)
     """
@@ -573,15 +581,15 @@
         else:
             return
     data, metadata = ReducedFramesInfos.split_data_and_metadata(my_dict)
     # handle relative frame position if any
     data = from_relative_reduced_frames_to_absolute(reduced_frames=data, scan=scan)
     scan.set_reduced_flats(flats=data, flats_infos=metadata)
     if save:
-        scan.save_reduced_flats(flats=data, flats_infos=metadata)
+        scan.save_reduced_flats(flats=data, flats_infos=metadata, overwrite=overwrite)
 
 
 def from_relative_reduced_frames_to_absolute(reduced_frames: dict, scan: TomoScanBase):
     if not isinstance(reduced_frames, dict):
         raise TypeError(
             f"reduced_frames is expected to be a dict, {type(reduced_frames)} provided"
         )
```

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/__init__.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/edfvolume.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/edfvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/hdf5volume.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/hdf5volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/jp2kvolume.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/jp2kvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/mock.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/rawvolume.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/rawvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/singleframebase.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/singleframebase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/tiffvolume.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/tiffvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/esrf/volume/utils.py` & `tomoscan-1.3.0a4/tomoscan/esrf/volume/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/factory.py` & `tomoscan-1.3.0a4/tomoscan/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "27/02/2019"
 
 
 import os
-from typing import Union
+from typing import Union, Optional
 from urllib.parse import urlparse
 
 from tomoscan.esrf.identifier.jp2kidentifier import JP2KVolumeIdentifier
 from tomoscan.esrf.identifier.rawidentifier import RawVolumeIdentifier
 from tomoscan.esrf.identifier.tiffidentifier import (
     MultiTiffVolumeIdentifier,
     TIFFVolumeIdentifier,
@@ -155,27 +155,27 @@
         elif scheme == "raw":
             if tomo_type == VolumeIdentifier.TOMO_TYPE:
                 return RawVolume.from_identifier(identifier=identifier)
         else:
             raise ValueError(f"Scheme {scheme} not recognized")
 
     @staticmethod
-    def create_scan_object(scan_path: str) -> TomoScanBase:
+    def create_scan_object(scan_path: str, entry: Optional[str] = None) -> TomoScanBase:
         """
 
         :param str scan_path: path to the scan directory or file
         :return: ScanBase instance fitting the scan folder or scan path
         :rtype: TomoScanBase
         """
         # remove any final separator (otherwise basename might fail)
         scan_path = scan_path.rstrip(os.path.sep)
-        if EDFTomoScan.is_tomoscan_dir(scan_path):
+        if entry is None and EDFTomoScan.is_tomoscan_dir(scan_path):
             return EDFTomoScan(scan=scan_path)
         elif HDF5TomoScan.is_tomoscan_dir(scan_path):
-            return HDF5TomoScan(scan=scan_path)
+            return HDF5TomoScan(scan=scan_path, entry=entry)
         else:
             raise ValueError(f"{scan_path} is not a valid scan path")
 
     @staticmethod
     def create_scan_objects(scan_path: str) -> tuple:
         """
```

### Comparing `tomoscan-1.3.0a2/tomoscan/framereducerbase.py` & `tomoscan-1.3.0a4/tomoscan/framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/identifier.py` & `tomoscan-1.3.0a4/tomoscan/identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/io.py` & `tomoscan-1.3.0a4/tomoscan/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/nexus/paths/nxdetector.py` & `tomoscan-1.3.0a4/tomoscan/nexus/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/nexus/paths/nxsample.py` & `tomoscan-1.3.0a4/tomoscan/nexus/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/nexus/paths/nxtomo.py` & `tomoscan-1.3.0a4/tomoscan/nexus/paths/nxtomo.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/normalization.py` & `tomoscan-1.3.0a4/tomoscan/normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/progress.py` & `tomoscan-1.3.0a4/tomoscan/progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/scanbase.py` & `tomoscan-1.3.0a4/tomoscan/scanbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1210,14 +1210,15 @@
 
     def _dump_frame_dict(
         self,
         frames: dict,
         output_urls,
         frames_metadata: Optional[ReducedFramesInfos],
         metadata_output_urls: Optional[tuple],
+        overwrite: bool = False,
     ):
         """
         utils function to save some frames in set of output_urls
 
         Behavior with HDF5: it expects to have a dedicated group where it can save the different frame with indices.
         It will do a first iteration at this group level to remove unused dataset and will overwrite the one he can in order to reduced memory print
         """
@@ -1274,14 +1275,16 @@
                 used_datasets.append(
                     format_data_path(
                         url, entry=entry, idx=idx, idx_zfill4=idx_zfill4
                     ).split("/")[-1]
                 )
             with HDF5File(file_path, mode="a") as h5s:
                 if group_path in h5s:
+                    if not overwrite:
+                        raise KeyError("group_path already exists")
                     for key in h5s[group_path].keys():
                         if key not in used_datasets:
                             del h5s[group_path][key]
 
         # save data
         for url in output_urls:
             clean_frame_group(url=url)
@@ -1342,14 +1345,15 @@
 
                         edf_writer = fabio.edfimage.EdfImage(
                             data=frame,
                             header=header,
                         )
                         edf_writer.write(file_path)
                 elif scheme in ("hdf5", "silx"):
+                    os.makedirs(os.path.dirname(file_path), exist_ok=True)
                     with HDF5File(file_path, mode="a") as h5s:
                         if data_path in h5s:
                             h5s[data_path][()] = frame
                         else:
                             h5s[data_path] = frame
                         h5s[data_path].attrs["interpretation"] = "image"
                 else:
@@ -1643,23 +1647,25 @@
 
     def save_reduced_darks(
         self,
         darks: dict,
         output_urls: tuple,
         darks_infos: Optional[ReducedFramesInfos] = None,
         metadata_output_urls: Optional[tuple] = None,
+        overwrite: bool = False,
     ) -> None:
         """
         Dump computed dark (median / mean...) into files
         """
         self._dump_frame_dict(
             frames=darks,
             output_urls=output_urls,
             frames_metadata=darks_infos,
             metadata_output_urls=metadata_output_urls,
+            overwrite=overwrite,
         )
 
     def load_reduced_darks(
         self,
         inputs_urls: tuple,
         metadata_input_urls=None,
         return_as_url: bool = False,
@@ -1680,23 +1686,25 @@
 
     def save_reduced_flats(
         self,
         flats: dict,
         output_urls: tuple,
         flats_infos: Optional[ReducedFramesInfos] = None,
         metadata_output_urls: Optional[tuple] = None,
+        overwrite: bool = False,
     ) -> None:
         """
         Dump reduced flats (median / mean...) into files
         """
         self._dump_frame_dict(
             frames=flats,
             output_urls=output_urls,
             frames_metadata=flats_infos,
             metadata_output_urls=metadata_output_urls,
+            overwrite=overwrite,
         )
 
     def load_reduced_flats(
         self,
         inputs_urls: tuple,
         metadata_input_urls=None,
         return_as_url: bool = False,
```

### Comparing `tomoscan-1.3.0a2/tomoscan/serie.py` & `tomoscan-1.3.0a4/tomoscan/serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_framereducerbase.py` & `tomoscan-1.3.0a4/tomoscan/test/test_framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_io.py` & `tomoscan-1.3.0a4/tomoscan/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_normalization.py` & `tomoscan-1.3.0a4/tomoscan/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_progress.py` & `tomoscan-1.3.0a4/tomoscan/test/test_progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_scanbase.py` & `tomoscan-1.3.0a4/tomoscan/test/test_scanbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_scanfactory.py` & `tomoscan-1.3.0a4/tomoscan/test/test_scanfactory.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_serie.py` & `tomoscan-1.3.0a4/tomoscan/test/test_serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_tomoobject.py` & `tomoscan-1.3.0a4/tomoscan/test/test_tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_utils.py` & `tomoscan-1.3.0a4/tomoscan/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_validator.py` & `tomoscan-1.3.0a4/tomoscan/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_version.py` & `tomoscan-1.3.0a4/tomoscan/test/test_version.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_volume_base.py` & `tomoscan-1.3.0a4/tomoscan/test/test_volume_base.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/test_volume_utils.py` & `tomoscan-1.3.0a4/tomoscan/test/test_volume_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/test/utils.py` & `tomoscan-1.3.0a4/tomoscan/test/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/tomoobject.py` & `tomoscan-1.3.0a4/tomoscan/tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/__init__.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/electriccurrentsystem.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/electriccurrentsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/energysystem.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/energysystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/metricsystem.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/metricsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/timesystem.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/timesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/unit.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/unit.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/unitsystem/voltagesystem.py` & `tomoscan-1.3.0a4/tomoscan/unitsystem/voltagesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/utils/decorator.py` & `tomoscan-1.3.0a4/tomoscan/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/utils/geometry.py` & `tomoscan-1.3.0a4/tomoscan/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/utils/hdf5.py` & `tomoscan-1.3.0a4/tomoscan/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/utils/io.py` & `tomoscan-1.3.0a4/tomoscan/utils/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/utils/volume.py` & `tomoscan-1.3.0a4/tomoscan/utils/volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/validator.py` & `tomoscan-1.3.0a4/tomoscan/validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a2/tomoscan/version.py` & `tomoscan-1.3.0a4/tomoscan/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 3
 MICRO = 0
 RELEV = "alpha"  # <16
-SERIAL = 2  # <16
+SERIAL = 4  # <16
 
 date = __date__
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
 )
```

### Comparing `tomoscan-1.3.0a2/tomoscan/volumebase.py` & `tomoscan-1.3.0a4/tomoscan/volumebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
             if index == "middle":
                 index = self.get_volume_shape()[axis] // 2
             elif index == "first":
                 index = 0
             elif index == "last":
                 index = -1
 
-        print("index is", index)
         if self.data is not None:
             return self.select(
                 volume=self.data, xy=xy, xz=xz, yz=yz, axis=axis, index=index
             )
         else:
             return None
```

### Comparing `tomoscan-1.3.0a2/tomoscan.egg-info/PKG-INFO` & `tomoscan-1.3.0a4/tomoscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a2
+Version: 1.3.0a4
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a2/tomoscan.egg-info/SOURCES.txt` & `tomoscan-1.3.0a4/tomoscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

