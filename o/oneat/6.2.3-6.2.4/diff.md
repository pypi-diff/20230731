# Comparing `tmp/oneat-6.2.3.tar.gz` & `tmp/oneat-6.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.2.3.tar", last modified: Sat Jul 29 13:48:34 2023, max compression
+gzip compressed data, was "oneat-6.2.4.tar", last modified: Mon Jul 31 08:39:52 2023, max compression
```

## Comparing `oneat-6.2.3.tar` & `oneat-6.2.4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.572481 oneat-6.2.3/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.2.3/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.2.3/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.537303 oneat-6.2.3/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.541658 oneat-6.2.3/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.2.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.2.3/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.543034 oneat-6.2.3/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.543233 oneat-6.2.3/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.2.3/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.2.3/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.2.3/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.2.3/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.2.3/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:48:34.572638 oneat-6.2.3/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.2.3/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.550296 oneat-6.2.3/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.2.3/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.2.3/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.2.3/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.2.3/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.2.3/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.2.3/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.2.3/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.2.3/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.552026 oneat-6.2.3/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.2.3/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.2.3/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.2.3/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.2.3/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.2.3/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.2.3/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.2.3/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-29 13:48:34.573289 oneat-6.2.3/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.538014 oneat-6.2.3/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.553895 oneat-6.2.3/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.559711 oneat-6.2.3/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.2.3/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38493 2023-07-29 13:36:58.000000 oneat-6.2.3/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.562692 oneat-6.2.3/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.2.3/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.2.3/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.2.3/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.2.3/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.564422 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-29 13:48:14.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.565711 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70774 2023-07-29 13:46:47.000000 oneat-6.2.3/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.566276 oneat-6.2.3/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.572171 oneat-6.2.3/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.2.3/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:48:34.555098 oneat-6.2.3/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-29 13:48:34.000000 oneat-6.2.3/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.2.3/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.393343 oneat-6.2.4/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.2.4/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.2.4/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.369599 oneat-6.2.4/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.372506 oneat-6.2.4/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.2.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.2.4/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.373793 oneat-6.2.4/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.373951 oneat-6.2.4/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.2.4/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.2.4/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.2.4/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.2.4/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 08:39:52.393431 oneat-6.2.4/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.2.4/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.377984 oneat-6.2.4/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.2.4/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.2.4/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.2.4/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.2.4/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.2.4/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.2.4/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.2.4/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.2.4/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.379727 oneat-6.2.4/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.2.4/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.2.4/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.2.4/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.2.4/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.2.4/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.2.4/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.2.4/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-31 08:39:52.393794 oneat-6.2.4/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.370051 oneat-6.2.4/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.380509 oneat-6.2.4/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.384090 oneat-6.2.4/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.2.4/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38579 2023-07-31 08:35:36.000000 oneat-6.2.4/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.386420 oneat-6.2.4/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.2.4/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.2.4/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.2.4/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.2.4/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.387355 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-29 13:48:14.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.388179 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70833 2023-07-31 08:33:33.000000 oneat-6.2.4/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.388555 oneat-6.2.4/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.392356 oneat-6.2.4/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.2.4/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 08:39:52.381310 oneat-6.2.4/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-31 08:39:52.000000 oneat-6.2.4/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.2.4/tox.ini
```

### Comparing `oneat-6.2.3/.DS_Store` & `oneat-6.2.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/.github/workflows/test_and_deploy.yml` & `oneat-6.2.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/.gitignore` & `oneat-6.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/.pre-commit-config.yaml` & `oneat-6.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/LICENSE` & `oneat-6.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/PKG-INFO` & `oneat-6.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.2.3
+Version: 6.2.4
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.2.3/README.md` & `oneat-6.2.4/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/Xenopus_example.jpg` & `oneat-6.2.4/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/Xenopus_example.png` & `oneat-6.2.4/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/ch_0_crop.png` & `oneat-6.2.4/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/ch_1_crop.png` & `oneat-6.2.4/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/ch_2_crop.png` & `oneat-6.2.4/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/ch_3_crop.png` & `oneat-6.2.4/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/ch_4_crop.png` & `oneat-6.2.4/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/images/ch_5_crop.png` & `oneat-6.2.4/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/licenses/Apache-2` & `oneat-6.2.4/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/licenses/BSD-3` & `oneat-6.2.4/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/licenses/GPL-3` & `oneat-6.2.4/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/licenses/LGPL-3` & `oneat-6.2.4/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/licenses/MIT` & `oneat-6.2.4/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/licenses/MPL-2` & `oneat-6.2.4/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/setup.cfg` & `oneat-6.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.2.4/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.2.4/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.2.4/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.2.4/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/__init__.py` & `oneat-6.2.4/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/config.py` & `oneat-6.2.4/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.2.4/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/loss.py` & `oneat-6.2.4/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,15 @@
         self.segimage = None         
 
         return self.marker_tree
     
     def predict(self, 
                 image : np.ndarray,  
                 savedir : str = None, 
+                savename: str = '',
                 n_tiles : tuple = (1, 1, 1), 
                 overlap_percent : float =0.8,
                 event_threshold : float = 0.5, 
                 event_confidence : float = 0.5, 
                 iou_threshold : float = 0.1,  
                 dtype : np.dtype = np.uint8,
                 marker_tree : dict = None, 
@@ -277,14 +278,15 @@
         
         self.dtype = dtype
         self.nms_function = nms_function 
         self.originalimage = image.astype(self.dtype)
         self.ndim = len(self.originalimage.shape)
         self.activations = activations
         self.savedir = savedir
+        self.savename = savename
         if self.savedir is not None:
            Path(self.savedir).mkdir(exist_ok=True)
         if len(n_tiles) == 3:   
            n_tiles = (n_tiles[-3], n_tiles[-2], n_tiles[-1])
         else:
             n_tiles = (1,1,1)   
         self.n_tiles = n_tiles
@@ -593,15 +595,15 @@
 
                best_iou_classedboxes[event_name] = [best_sorted_event_box]
                
         self.iou_classedboxes = best_iou_classedboxes
 
 
     def to_csv(self):
-             save_volume_csv( self.key_categories, self.iou_classedboxes, self.savedir)          
+             save_volume_csv( self.key_categories, self.iou_classedboxes, self.savedir, self.savename)          
  
     def to_activations(self):
              self.all_iou_classedboxes =  save_volume( self.key_categories, self.iou_classedboxes, self.all_iou_classedboxes)
 
     def overlaptiles(self, sliceregion):
 
         if self.n_tiles == (1, 1, 1):
```

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_focus.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.2.4/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATModels/nets.py` & `oneat-6.2.4/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.2.4/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.2.4/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/NMS.py` & `oneat-6.2.4/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.2.4/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.2.4/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.2.4/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.2.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/plotters.py` & `oneat-6.2.4/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/NEATUtils/utils.py` & `oneat-6.2.4/src/oneat/NEATUtils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1549,15 +1549,15 @@
                         boxes = boxes + oldboxes[0]
 
             all_iou_classed_boxes[event_name] = [boxes]
     return all_iou_classed_boxes
 
 
 def save_volume_csv(
-    key_categories: dict, iou_classedboxes: dict, savedir: str
+    key_categories: dict, iou_classedboxes: dict, savedir: str, savename: str
 ):
 
     for (event_name, event_label) in key_categories.items():
 
         if event_label > 0:
             xlocations = []
             ylocations = []
@@ -1612,17 +1612,17 @@
                 ]
             )
             event_count = sorted(
                 event_count, key=lambda x: x[0], reverse=False
             )
             event_data = []
             csvname = Path(savedir) /  f"pred_{event_name}_locations"
-
-            writer = csv.writer(open(str(csvname) + ".csv", "a", newline=""))
-            filesize = os.stat(str(csvname) + ".csv").st_size
+            
+            writer = csv.writer(open(str(csvname) + str(savename) + ".csv", "a", newline=""))
+            filesize = os.stat(str(csvname) + str(savename) + ".csv").st_size
 
             if filesize < 1:
                 writer.writerow(
                     ["T", "Z", "Y", "X", "Score", "Size", "Confidence"]
                 )
             for line in event_count:
                 if line not in event_data:
```

### Comparing `oneat-6.2.3/src/oneat/__init__.py` & `oneat-6.2.4/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/_tests/test_nets.py` & `oneat-6.2.4/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/_tests/utils.py` & `oneat-6.2.4/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.2.4/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/_tests/variables/variables.index` & `oneat-6.2.4/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat/pretrained.py` & `oneat-6.2.4/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/src/oneat.egg-info/PKG-INFO` & `oneat-6.2.4/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.2.3
+Version: 6.2.4
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.2.3/src/oneat.egg-info/SOURCES.txt` & `oneat-6.2.4/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.2.3/tox.ini` & `oneat-6.2.4/tox.ini`

 * *Files identical despite different names*

