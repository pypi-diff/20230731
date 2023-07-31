# Comparing `tmp/opendrive2tessng-0.1.4.tar.gz` & `tmp/opendrive2tessng-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\opendrive2tessng-0.1.4.tar", last modified: Mon May 15 08:16:43 2023, max compression
+gzip compressed data, was "dist\opendrive2tessng-0.1.5.tar", last modified: Mon Jul 31 09:16:17 2023, max compression
```

## Comparing `opendrive2tessng-0.1.4.tar` & `opendrive2tessng-0.1.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/
--rw-rw-rw-   0        0        0     1091 2022-07-04 06:28:49.000000 opendrive2tessng-0.1.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/
--rw-rw-rw-   0        0        0      720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/
--rw-rw-rw-   0        0        0    12909 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py
--rw-rw-rw-   0        0        0    38355 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py
--rw-rw-rw-   0        0        0     9412 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/
--rw-rw-rw-   0        0        0     7920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/gui.py
--rw-rw-rw-   0        0        0     3585 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py
--rw-rw-rw-   0        0        0     4854 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/osm_convert.py
--rw-rw-rw-   0        0        0    13250 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/viewer.py
--rw-rw-rw-   0        0        0     1720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/__init__.py
--rw-rw-rw-   0        0        0    14324 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/network.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/
--rw-rw-rw-   0        0        0     2632 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py
--rw-rw-rw-   0        0        0     7137 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py
--rw-rw-rw-   0        0        0     3909 2023-05-06 02:10:21.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py
--rw-rw-rw-   0        0        0     2286 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py
--rw-rw-rw-   0        0        0     2616 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py
--rw-rw-rw-   0        0        0      920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py
--rw-rw-rw-   0        0        0     7954 2023-05-08 01:38:23.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py
--rw-rw-rw-   0        0        0     4099 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py
--rw-rw-rw-   0        0        0     5726 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py
--rw-rw-rw-   0        0        0     8934 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py
--rw-rw-rw-   0        0        0     2165 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py
--rw-rw-rw-   0        0        0     1495 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/__init__.py
--rw-rw-rw-   0        0        0    18529 2023-05-08 01:48:35.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/
--rw-rw-rw-   0        0        0    12247 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py
--rw-rw-rw-   0        0        0     4085 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/osm.py
--rw-rw-rw-   0        0        0    23038 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py
--rw-rw-rw-   0        0        0     1872 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/parser.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/
--rw-rw-rw-   0        0        0     4222 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/border.py
--rw-rw-rw-   0        0        0    14407 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py
--rw-rw-rw-   0        0        0    17452 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/utils.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/
--rw-rw-rw-   0        0        0     1833 2023-05-06 03:35:43.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/config.py
--rw-rw-rw-   0        0        0    11765 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/convert_utils.py
--rw-rw-rw-   0        0        0     8363 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/external_utils.py
--rw-rw-rw-   0        0        0     7638 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/functions.py
--rw-rw-rw-   0        0        0    33740 2023-03-27 07:35:27.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/network_utils.py
--rw-rw-rw-   0        0        0    10707 2023-03-14 07:15:21.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/unity_utils.py
--rw-rw-rw-   0        0        0      228 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/utils/__init__.py
--rw-rw-rw-   0        0        0      688 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.4/opendrive2tessng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      583 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2756 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/opendrive2tessng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      583 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      118 2022-07-04 07:03:18.000000 opendrive2tessng-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 08:16:43.000000 opendrive2tessng-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-05-15 08:14:54.000000 opendrive2tessng-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2022-07-04 06:28:49.000000 opendrive2tessng-0.1.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/
+-rw-rw-rw-   0        0        0      720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/
+-rw-rw-rw-   0        0        0    12909 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py
+-rw-rw-rw-   0        0        0    38355 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py
+-rw-rw-rw-   0        0        0     9412 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/
+-rw-rw-rw-   0        0        0     7920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/gui.py
+-rw-rw-rw-   0        0        0     3585 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py
+-rw-rw-rw-   0        0        0     4854 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/osm_convert.py
+-rw-rw-rw-   0        0        0    13250 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/viewer.py
+-rw-rw-rw-   0        0        0     1720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/__init__.py
+-rw-rw-rw-   0        0        0    14324 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/network.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/
+-rw-rw-rw-   0        0        0     2632 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py
+-rw-rw-rw-   0        0        0     7137 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py
+-rw-rw-rw-   0        0        0     3909 2023-05-06 02:10:21.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py
+-rw-rw-rw-   0        0        0     2286 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py
+-rw-rw-rw-   0        0        0     2616 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py
+-rw-rw-rw-   0        0        0      920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py
+-rw-rw-rw-   0        0        0     7954 2023-05-08 01:38:23.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py
+-rw-rw-rw-   0        0        0     4099 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py
+-rw-rw-rw-   0        0        0     5726 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py
+-rw-rw-rw-   0        0        0     8934 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py
+-rw-rw-rw-   0        0        0     2165 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py
+-rw-rw-rw-   0        0        0     1495 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/__init__.py
+-rw-rw-rw-   0        0        0    18715 2023-07-01 14:13:19.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/
+-rw-rw-rw-   0        0        0    12247 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py
+-rw-rw-rw-   0        0        0     4085 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm.py
+-rw-rw-rw-   0        0        0    23038 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py
+-rw-rw-rw-   0        0        0     1872 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/
+-rw-rw-rw-   0        0        0     4222 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/border.py
+-rw-rw-rw-   0        0        0    14407 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py
+-rw-rw-rw-   0        0        0    17452 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/utils.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/
+-rw-rw-rw-   0        0        0     1982 2023-07-31 09:11:10.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/config.py
+-rw-rw-rw-   0        0        0    11765 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/convert_utils.py
+-rw-rw-rw-   0        0        0     8363 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/external_utils.py
+-rw-rw-rw-   0        0        0    11529 2023-07-31 03:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/functions.py
+-rw-rw-rw-   0        0        0    42188 2023-07-31 09:07:26.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/network_utils.py
+-rw-rw-rw-   0        0        0    10707 2023-03-14 07:15:21.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/unity_utils.py
+-rw-rw-rw-   0        0        0      228 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      583 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2756 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      583 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      118 2022-07-04 07:03:18.000000 opendrive2tessng-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-07-31 09:14:39.000000 opendrive2tessng-0.1.5/setup.py
```

### Comparing `opendrive2tessng-0.1.4/LICENSE` & `opendrive2tessng-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/main.py` & `opendrive2tessng-0.1.5/opendrive2tessng/main.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/converter.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/converter.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/gui.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/gui.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/osm_convert.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/osm_convert.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/viewer.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/viewer.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/network.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/network.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,23 +342,29 @@
             new_lane.level = (
                 "true" if lane.get("level") in [1, "1", "true"] else "false"
             )
 
             # Lane Links
             if lane.find("link") is not None:
 
-                if lane.find("link").find("predecessor") is not None:
-                    new_lane.link.predecessorId = (
-                        lane.find("link").find("predecessor").get("id")
-                    )
+                try:
+                    if lane.find("link").find("predecessor") is not None:
+                        new_lane.link.predecessorId = (
+                            lane.find("link").find("predecessor").get("id")
+                        )
+                except:
+                    continue
 
-                if lane.find("link").find("successor") is not None:
-                    new_lane.link.successorId = (
-                        lane.find("link").find("successor").get("id")
-                    )
+                try:
+                    if lane.find("link").find("successor") is not None:
+                        new_lane.link.successorId = (
+                            lane.find("link").find("successor").get("id")
+                        )
+                except:
+                    continue
 
             # Width
             for widthIdx, width in enumerate(lane.findall("width")):
                 newWidth = RoadLaneSectionLaneWidth(
                     float(width.get("a")),
                     float(width.get("b")),
                     float(width.get("c")),
```

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/osm.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/osm/parser.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/parser.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/border.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/border.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/opendrive2lanelet/utils.py` & `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/utils/config.py` & `opendrive2tessng-0.1.5/opendrive2tessng/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # opendrive —> tess 车道, 不在此映射表中的车道不予显示
 # tess 中车道类型定义 机动车道/机非共享/非机动车道/公交专用道
 LANE_TYPE_MAPPING = {
     'driving': '机动车道',
     'biking': '非机动车道',
-    'sidewalk': '非机动车道',  # 行人道实际无意义
+    'sidewalk': '人行道',  # 行人道实际无意义
     'stop': '应急车道',
 
     # 'onRamp': '机动车道',
     # 'offRamp': '机动车道',
     # 'entry': '机动车道',
     # 'exit': '机动车道',
     # 'connectingRamp': '机动车道',
@@ -16,14 +16,18 @@
     # 'none': '',
     # 'redtricted': '',
     # 'parking': '停车带',
     # 'median': '',
     # 'curb': '',
 }
 
+# 当前后几个点的向量夹角小于 default_angle 且点距小于 max_length(除非夹角为0 ) 时，抹除过渡点
+default_angle = 1
+max_length = 50
+
 # 连续次数后可视为正常车道，或者连续次数后可视为连接段,最小值为2
 point_require = 2
 POINT_REQUIRE = max(2, point_require)
 
 # 当 opendrive 连接段的首尾连接长度低于此值时，抛弃原有的点序列，使用自动连接
 MIN_CONNECTOR_LENGTH = None
 
@@ -32,18 +36,18 @@
 
 # 需要被处理的车道类型及处理参数
 WIDTH_LIMIT = {
     '机动车道': {
         'split': 2,  # 作为正常的最窄距离
         'join': 1.5,  # 被忽略时的最宽距离
     },
-    # '非机动车道': {
-    #     'split': 2,
-    #     'join': 0.5,
-    # },
+    '非机动车道': {
+        'split': 2,
+        'join': 0.5,
+    },
 }
 
 # unity 信息提取的类型映射
 UNITY_LANE_MAPPING = {
     "Driving": ["driving", "stop", "parking", "entry", "exit", "offRamp", "onRamp", "connectingRamp", ],
     "None": ["none"],
     "GreenBelt": ["shoulder", "border", "median", "curb"],
```

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/utils/convert_utils.py` & `opendrive2tessng-0.1.5/opendrive2tessng/utils/convert_utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/utils/external_utils.py` & `opendrive2tessng-0.1.5/opendrive2tessng/utils/external_utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/utils/unity_utils.py` & `opendrive2tessng-0.1.5/opendrive2tessng/utils/unity_utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng/__init__.py` & `opendrive2tessng-0.1.5/opendrive2tessng/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng.egg-info/PKG-INFO` & `opendrive2tessng-0.1.5/opendrive2tessng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendrive2tessng
-Version: 0.1.4
+Version: 0.1.5
 Summary: convert opendrive to road_network
 Home-page: UNKNOWN
 Author: Author
 Author-email: 17315487709@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opendrive2tessng-0.1.4/opendrive2tessng.egg-info/SOURCES.txt` & `opendrive2tessng-0.1.5/opendrive2tessng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.4/PKG-INFO` & `opendrive2tessng-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendrive2tessng
-Version: 0.1.4
+Version: 0.1.5
 Summary: convert opendrive to road_network
 Home-page: UNKNOWN
 Author: Author
 Author-email: 17315487709@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opendrive2tessng-0.1.4/setup.py` & `opendrive2tessng-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="opendrive2tessng",
-    version="0.1.4",
+    version="0.1.5",
     author="Author",
     author_email="17315487709@163.com",
     description="convert opendrive to road_network",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     install_requires=[
```

