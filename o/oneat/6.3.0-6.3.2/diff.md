# Comparing `tmp/oneat-6.3.0.tar.gz` & `tmp/oneat-6.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.3.0.tar", last modified: Mon Jul 31 09:44:57 2023, max compression
+gzip compressed data, was "oneat-6.3.2.tar", last modified: Mon Jul 31 09:54:31 2023, max compression
```

## Comparing `oneat-6.3.0.tar` & `oneat-6.3.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.739110 oneat-6.3.0/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.3.0/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.3.0/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.715107 oneat-6.3.0/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.718306 oneat-6.3.0/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.3.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.3.0/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.719427 oneat-6.3.0/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.719568 oneat-6.3.0/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.3.0/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.3.0/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.3.0/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.3.0/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.3.0/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 09:44:57.739202 oneat-6.3.0/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.3.0/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.723754 oneat-6.3.0/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.3.0/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.3.0/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.3.0/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.3.0/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.3.0/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.3.0/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.3.0/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.3.0/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.724932 oneat-6.3.0/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.3.0/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.3.0/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.3.0/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.3.0/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.3.0/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.3.0/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-31 09:43:42.000000 oneat-6.3.0/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-31 09:44:57.739555 oneat-6.3.0/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.715550 oneat-6.3.0/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.725792 oneat-6.3.0/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.729830 oneat-6.3.0/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.3.0/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38579 2023-07-31 08:35:36.000000 oneat-6.3.0/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.732262 oneat-6.3.0/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.3.0/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.3.0/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.3.0/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-31 09:43:48.000000 oneat-6.3.0/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.3.0/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.733758 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-29 13:48:14.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21320 2023-07-31 09:44:22.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.734671 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2883 2023-07-31 09:20:05.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70833 2023-07-31 08:33:33.000000 oneat-6.3.0/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.735033 oneat-6.3.0/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.738896 oneat-6.3.0/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.3.0/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:44:57.726583 oneat-6.3.0/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-31 09:44:57.000000 oneat-6.3.0/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.3.0/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.306327 oneat-6.3.2/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.3.2/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.3.2/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.281488 oneat-6.3.2/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.284598 oneat-6.3.2/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.3.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.3.2/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.285705 oneat-6.3.2/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.285851 oneat-6.3.2/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.3.2/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.3.2/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.3.2/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.3.2/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 09:54:31.306436 oneat-6.3.2/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.3.2/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.289368 oneat-6.3.2/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.3.2/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.3.2/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.3.2/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.3.2/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.3.2/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.3.2/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.3.2/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.3.2/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.290747 oneat-6.3.2/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.3.2/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.3.2/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.3.2/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.3.2/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.3.2/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.3.2/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-31 09:43:42.000000 oneat-6.3.2/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-31 09:54:31.306817 oneat-6.3.2/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.281938 oneat-6.3.2/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.291537 oneat-6.3.2/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.295788 oneat-6.3.2/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.3.2/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38579 2023-07-31 08:35:36.000000 oneat-6.3.2/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.298224 oneat-6.3.2/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.3.2/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.3.2/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.3.2/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-31 09:43:48.000000 oneat-6.3.2/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.3.2/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.299700 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-29 13:48:14.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21390 2023-07-31 09:53:44.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.300575 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2883 2023-07-31 09:20:05.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70833 2023-07-31 08:33:33.000000 oneat-6.3.2/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.300944 oneat-6.3.2/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.305325 oneat-6.3.2/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.3.2/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 09:54:31.292292 oneat-6.3.2/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-31 09:54:31.000000 oneat-6.3.2/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.3.2/tox.ini
```

### Comparing `oneat-6.3.0/.DS_Store` & `oneat-6.3.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/.github/workflows/test_and_deploy.yml` & `oneat-6.3.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/.gitignore` & `oneat-6.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/.pre-commit-config.yaml` & `oneat-6.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/LICENSE` & `oneat-6.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/PKG-INFO` & `oneat-6.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.3.0
+Version: 6.3.2
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.3.0/README.md` & `oneat-6.3.2/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/Xenopus_example.jpg` & `oneat-6.3.2/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/Xenopus_example.png` & `oneat-6.3.2/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/ch_0_crop.png` & `oneat-6.3.2/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/ch_1_crop.png` & `oneat-6.3.2/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/ch_2_crop.png` & `oneat-6.3.2/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/ch_3_crop.png` & `oneat-6.3.2/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/ch_4_crop.png` & `oneat-6.3.2/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/images/ch_5_crop.png` & `oneat-6.3.2/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/licenses/Apache-2` & `oneat-6.3.2/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/licenses/BSD-3` & `oneat-6.3.2/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/licenses/GPL-3` & `oneat-6.3.2/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/licenses/LGPL-3` & `oneat-6.3.2/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/licenses/MIT` & `oneat-6.3.2/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/licenses/MPL-2` & `oneat-6.3.2/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/setup.cfg` & `oneat-6.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.3.2/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.3.2/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.3.2/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.3.2/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/__init__.py` & `oneat-6.3.2/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/config.py` & `oneat-6.3.2/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.3.2/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/loss.py` & `oneat-6.3.2/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_focus.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.3.2/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATModels/nets.py` & `oneat-6.3.2/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.3.2/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.3.2/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/NMS.py` & `oneat-6.3.2/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.3.2/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.3.2/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.3.2/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,17 +409,18 @@
         self.score_locations = []
         self.event_locations = []
         self.confidence_locations = []
         csvnames = list(Path(self.csvdir).glob("*.csv"))
         for layer in list(self.viewer.layers):
             if "Detections" in layer.name or layer.name in "Detections":
                 self.viewer.layers.remove(layer)
-        
+        print(imagename, csv_event_name)
         for i in range(len(csvnames)): 
-            if imagename in csvnames and csv_event_name in csvnames:
+            print(csvnames[i])
+            if imagename in csvnames[i] and csv_event_name in csvnames[i]:
                     csvname = csvnames[i]
                     break   
         if csvname is None:
             print( "No csv file found for this image")                
         if csvname is not None:
 
             self.event_name = csv_event_name
```

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.3.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/plotters.py` & `oneat-6.3.2/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/NEATUtils/utils.py` & `oneat-6.3.2/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/__init__.py` & `oneat-6.3.2/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/_tests/test_nets.py` & `oneat-6.3.2/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/_tests/utils.py` & `oneat-6.3.2/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.3.2/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/_tests/variables/variables.index` & `oneat-6.3.2/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat/pretrained.py` & `oneat-6.3.2/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/src/oneat.egg-info/PKG-INFO` & `oneat-6.3.2/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.3.0
+Version: 6.3.2
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.3.0/src/oneat.egg-info/SOURCES.txt` & `oneat-6.3.2/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.3.0/tox.ini` & `oneat-6.3.2/tox.ini`

 * *Files identical despite different names*

