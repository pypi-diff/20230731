# Comparing `tmp/daggerpy-0.0.4.tar.gz` & `tmp/daggerpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daggerpy-0.0.4.tar", last modified: Thu Jul 20 14:36:02 2023, max compression
+gzip compressed data, was "daggerpy-0.0.5.tar", last modified: Mon Jul 31 10:22:18 2023, max compression
```

## Comparing `daggerpy-0.0.4.tar` & `daggerpy-0.0.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:36:02.103742 daggerpy-0.0.4/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.4/AUTHORS.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.4/CONTRIBUTING.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      319 2023-07-20 14:35:29.000000 daggerpy-0.0.4/HISTORY.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.4/LICENSE
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.4/MANIFEST.in
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2642 2023-07-20 14:36:02.103742 daggerpy-0.0.4/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.4/README.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:36:02.103742 daggerpy-0.0.4/daggerpy.egg-info/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2642 2023-07-20 14:36:02.000000 daggerpy-0.0.4/daggerpy.egg-info/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1470 2023-07-20 14:36:02.000000 daggerpy-0.0.4/daggerpy.egg-info/SOURCES.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 14:36:02.000000 daggerpy-0.0.4/daggerpy.egg-info/dependency_links.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-20 14:36:02.000000 daggerpy-0.0.4/daggerpy.egg-info/entry_points.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.4/daggerpy.egg-info/not-zip-safe
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-20 14:36:02.000000 daggerpy-0.0.4/daggerpy.egg-info/requires.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-20 14:36:02.000000 daggerpy-0.0.4/daggerpy.egg-info/top_level.txt
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:36:02.103742 daggerpy-0.0.4/docs/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/Makefile
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/authors.rst
--rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.4/docs/conf.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/contributing.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/history.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/index.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/installation.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/make.bat
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/readme.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.4/docs/usage.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:36:02.103742 daggerpy-0.0.4/includes/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/D4connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121804 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/PerlinNoise.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26014 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/_cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/_graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/_old_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/_priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/boost_spread_sort.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/boundary_conditions.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3178 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/connector_checker.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26421 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14090 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/depression_hierarchy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126074 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/fastflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/fastflood_recorder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64105 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    87785 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/graphflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/hillshading.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/npy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18089 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/popscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/popscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15617 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27925 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/simple_depression_solver.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94622 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/trackscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/trackscape_enum.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/trackscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1110 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/veclike_holder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/veque.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/wrap_helper.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/wrap_helper_MATLAB.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/wrap_helper_cpp.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/wrap_helper_julia.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-20 14:35:46.000000 daggerpy-0.0.4/includes/wrap_helper_python.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82378 2023-07-20 14:35:46.000000 daggerpy-0.0.4/main.cpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-20 14:36:02.107742 daggerpy-0.0.4/setup.cfg
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-07-20 14:34:39.000000 daggerpy-0.0.4/setup.py
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-20 14:36:02.103742 daggerpy-0.0.4/tests/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.4/tests/__init__.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.4/tests/test_dagger.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.183649 daggerpy-0.0.5/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.5/AUTHORS.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.5/CONTRIBUTING.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      318 2023-07-26 19:47:04.000000 daggerpy-0.0.5/HISTORY.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.5/LICENSE
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.5/MANIFEST.in
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2641 2023-07-31 10:22:18.183649 daggerpy-0.0.5/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.5/README.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.179649 daggerpy-0.0.5/daggerpy.egg-info/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2641 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1502 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/entry_points.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.5/daggerpy.egg-info/not-zip-safe
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/requires.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/top_level.txt
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.179649 daggerpy-0.0.5/docs/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/Makefile
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/authors.rst
+-rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.5/docs/conf.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/contributing.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/history.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/index.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/installation.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/make.bat
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/readme.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/usage.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.183649 daggerpy-0.0.5/includes/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/D4connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121966 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/PerlinNoise.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26031 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_old_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/boost_spread_sort.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/boundary_conditions.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3199 2023-07-31 10:19:21.000000 daggerpy-0.0.5/includes/connector_checker.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26439 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14121 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/depression_hierarchy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126078 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/fastflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/fastflood_recorder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64124 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96313 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/graphflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/hillshading.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/npy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18092 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/popscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/popscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15619 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3764 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/river_tools_python.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27928 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/simple_depression_solver.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94626 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/trackscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/trackscape_enum.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/trackscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1061 2023-07-31 10:19:21.000000 daggerpy-0.0.5/includes/veclike_holder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/veque.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_MATLAB.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_cpp.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_julia.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_python.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82665 2023-07-31 10:19:21.000000 daggerpy-0.0.5/main.cpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-31 10:22:18.183649 daggerpy-0.0.5/setup.cfg
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-07-31 10:20:14.000000 daggerpy-0.0.5/setup.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.183649 daggerpy-0.0.5/tests/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.5/tests/__init__.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.5/tests/test_dagger.py
```

### Comparing `daggerpy-0.0.4/CONTRIBUTING.rst` & `daggerpy-0.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/LICENSE` & `daggerpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/PKG-INFO` & `daggerpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -87,8 +87,7 @@
 * Fixing compilation for conda-forge on MacOS and Windows
 * Adding a quick topo function as quick test
 
 0 (2023-07-20)
 ------------------
 
 * First release on PyPI.
-
```

### Comparing `daggerpy-0.0.4/README.rst` & `daggerpy-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/daggerpy.egg-info/PKG-INFO` & `daggerpy-0.0.5/daggerpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -87,8 +87,7 @@
 * Fixing compilation for conda-forge on MacOS and Windows
 * Adding a quick topo function as quick test
 
 0 (2023-07-20)
 ------------------
 
 * First release on PyPI.
-
```

### Comparing `daggerpy-0.0.4/daggerpy.egg-info/SOURCES.txt` & `daggerpy-0.0.5/daggerpy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 includes/graph.hpp
 includes/graphflood.hpp
 includes/hillshading.hpp
 includes/npy.hpp
 includes/popscape.hpp
 includes/popscape_utils.hpp
 includes/priority_flood.hpp
+includes/river_tools_python.hpp
 includes/simple_depression_solver.hpp
 includes/trackscape.hpp
 includes/trackscape_enum.hpp
 includes/trackscape_utils.hpp
 includes/utils.hpp
 includes/veclike_holder.hpp
 includes/veque.hpp
```

### Comparing `daggerpy-0.0.4/docs/Makefile` & `daggerpy-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/docs/conf.py` & `daggerpy-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/docs/installation.rst` & `daggerpy-0.0.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/docs/make.bat` & `daggerpy-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/D4connector.hpp` & `daggerpy-0.0.5/includes/D4connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/D8connector.hpp` & `daggerpy-0.0.5/includes/D8connector.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 public:
   // General informations about the graph
   // #-> number of nodes (integer and unsized int for loops or list innit).
   int nnodes = 0;
   int nlinks() { return this->nnodes * 4; };
   size_t nnodes_t = 0;
 
+  int nxy() const { return this->nnodes; }
+
   static const int nneighbours = 8;
   static const size_t nneighbours_t = 8;
 
   // #-> number of nodes in x direction.
   int nx = 0;
   // #-> number of nodes in x direction.
   int ny = 0;
@@ -128,15 +130,15 @@
 
   // Single graph receivers
   // -> Sreceivers: steepest recervers (nnodes size),
   // -> number of donors (nnodes size),
   // -> Steepest donors (nnodes * nneighbours size)
   // --> Sdonors of node i are located from index i*nneighbours to index
   // i*nneighbours + nSdonors[i] not included
-  std::vector<int> Sreceivers, nSdonors, Sdonors;
+  std::vector<int> _Sreceivers, nSdonors, Sdonors;
 
   // Single graph distance to receivers
   std::vector<T> Sdistance2receivers;
 
   // Steepest slope
   std::vector<T> SS;
 
@@ -161,14 +163,17 @@
     // like Julia are complicating non default constructor initialisation.
     this->init_dimensions(nx, ny, dx, dy, xmin, ymin);
 
     // this->_allocate_vectors();
     // this->precompute_links();
   }
 
+  // Complying to the standard
+  int Sreceivers(int i) const { return this->_Sreceivers[i]; };
+
   template <class topo_t> void update_links_from_topo(topo_t &ttopo) {
     auto topo = format_input(ttopo);
     this->update_links(topo);
   }
 
   // initialise with dimension
   void init_dimensions(int nx, int ny, T dx, T dy, T xmin, T ymin) {
@@ -1698,17 +1703,17 @@
     // initialising all the links to not_processed
     uI_t maxu = std::numeric_limits<uI_t>::max();
 
     this->links = std::vector<uI_t>(this->nnodes * 4, maxu);
 
     this->linkdir = std::vector<uI_t>(this->nnodes * 4, maxu);
     this->ridknil = std::vector<uI_t>(this->nnodes * 4, maxu);
-    this->Sreceivers = std::vector<int>(this->nnodes, -1);
+    this->_Sreceivers = std::vector<int>(this->nnodes, -1);
     for (int i = 0; i < this->nnodes; ++i)
-      this->Sreceivers[i] = i;
+      this->_Sreceivers[i] = i;
     this->Sdistance2receivers = std::vector<T>(this->nnodes, -1);
     this->SS = std::vector<T>(this->nnodes, 0.);
 
     // int tocheck = 9876;
     // auto lix = this->get_empty_neighbour<int>();
     for (int i = 0; i < this->nnodes * 4; ++i) {
 
@@ -1926,21 +1931,21 @@
 
       bool FORCED = this->is_link_forced(i);
 
       if (FORCED) {
         slope = this->randu->get();
         if (this->is_link_inverse(i)) {
           if (this->SS[to] < slope) {
-            this->Sreceivers[to] = from;
+            this->_Sreceivers[to] = from;
             this->Sdistance2receivers[to] = dx;
             this->SS[to] = slope;
           }
         } else if (this->SS[from] < slope) {
           // saving the Sreceivers info as temporary best choice
-          this->Sreceivers[from] = to;
+          this->_Sreceivers[from] = to;
           this->Sdistance2receivers[from] = dx;
           this->SS[from] = slope;
         }
 
         continue;
       }
 
@@ -1951,27 +1956,27 @@
       if (slope > 0 && this->boundaries.can_give(from) &&
           this->boundaries.can_receive(to)) {
         // Conventional direction
         this->links[i] = 1;
         // if Steepest Slope is higher than the current recorded one
         if (this->SS[from] < slope) {
           // saving the Sreceivers info as temporary best choice
-          this->Sreceivers[from] = to;
+          this->_Sreceivers[from] = to;
           this->Sdistance2receivers[from] = dx;
           this->SS[from] = slope;
         }
       } else if (this->boundaries.can_give(to) &&
                  this->boundaries.can_receive(from) && slope < 0) {
         // Otherwise the convention is inverted:
         // isrec is falese and to is giving to from
         this->links[i] = 0;
         // NOte that slope is absolute values
         slope = std::abs(slope);
         if (this->SS[to] < slope) {
-          this->Sreceivers[to] = from;
+          this->_Sreceivers[to] = from;
           this->Sdistance2receivers[to] = dx;
           this->SS[to] = slope;
         }
       } else
         this->links[i] = 4;
     }
 
@@ -1987,15 +1992,15 @@
     // All of thenm have the graph dimension
     this->Sdonors = std::vector<int>(this->nnodes * this->nneighbours, -1);
     this->nSdonors = std::vector<int>(this->nnodes, 0);
 
     // iterating through all the nodes
     for (int i = 0; i < this->nnodes; ++i) {
       // SF so rid == i cause there is only 1 rec
-      int trec = this->Sreceivers[i];
+      int trec = this->_Sreceivers[i];
       if (trec == i)
         continue;
 
       // feeding the Sdonors array at rec position with current node and...
       this->Sdonors[trec * this->nneighbours + this->nSdonors[trec]] = i;
       // ... incrementing the number of Sdonors
       this->nSdonors[trec] += 1;
@@ -2015,25 +2020,25 @@
       // for(int j=0; j < this->nneighbours; ++j)
       // 	this->Sdonors[i * this->nneighbours + j] = -1;
       this->nSdonors[i] = 0;
     }
 
     for (int i = 0; i < this->nnodes; ++i) {
       // SF so rid == i cause there is only 1 rec
-      int trec = this->Sreceivers[i];
+      int trec = this->_Sreceivers[i];
       if (trec == i)
         continue;
       this->Sdonors[trec * this->nneighbours + this->nSdonors[trec]] = i;
       this->nSdonors[trec] += 1;
     }
   }
 
   void _reallocate_vectors() {
     for (int i = 0; i < this->nnodes; ++i) {
-      this->Sreceivers[i] = i;
+      this->_Sreceivers[i] = i;
       this->Sdistance2receivers[i] = 0;
       this->SS[i] = 0;
     }
   }
 
   bool is_in_bound_and_can_create_link(int o) {
     bool linkvalid = (this->is_in_bound(o));
@@ -2080,18 +2085,18 @@
 
   // Debug function printing to the prompt the single receiver of a node
   // Will probably get deprecated
   std::vector<int> get_rowcol_Sreceivers(int row, int col) {
     int node = this->nodeid_from_row_col(row, col);
     std::vector<int> out_receivers;
     int trow, tcol;
-    this->rowcol_from_node_id(this->Sreceivers[node], trow, tcol);
+    this->rowcol_from_node_id(this->_Sreceivers[node], trow, tcol);
     out_receivers = std::vector<int>{trow, tcol};
 
-    std::cout << "Srec is " << this->Sreceivers[node] << " node was " << node
+    std::cout << "Srec is " << this->_Sreceivers[node] << " node was " << node
               << std::endl;
     return out_receivers;
   }
 
   template <class topo_t> void print_receivers(int i, topo_t &ttopography) {
     std::cout << std::setprecision(12);
     auto topography = format_input<topo_t>(ttopography);
@@ -2117,15 +2122,15 @@
       int r = neighbours[tr];
       int row, col;
       this->rowcol_from_node_id(r, row, col);
       std::cout << "Neighbour " << r << " row " << row << " col " << col
                 << " topo " << topography[r] << std::endl;
     }
 
-    std::cout << "And finally Srec is " << this->Sreceivers[i] << std::endl;
+    std::cout << "And finally Srec is " << this->_Sreceivers[i] << std::endl;
     ;
   }
 
   // Returns the number of links stored in the graph
   // Note that it comprises some unvalid linked!
   int get_rec_array_size() { return int(this->links.size()); }
 
@@ -2137,15 +2142,15 @@
   U sum_at_outlets(array_t &tarray, bool include_internal_pits = true) {
     std::cout << "DEPRECATION WARNING::sum_at_outlets::should be moved as a "
                  "standalone algorithm"
               << std::endl;
     auto array = format_input<array_t>(tarray);
     U out = 0;
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->Sreceivers[i] == i) {
+      if (this->_Sreceivers[i] == i) {
         if (include_internal_pits) {
           out += array[i];
         } else if (this->flow_out_model(i)) {
           out += array[i];
         }
       }
     }
@@ -2158,15 +2163,15 @@
   /// pits, wether they are on purpose or not
   template <class array_t, class out_t>
   out_t keep_only_at_outlets(array_t &tarray,
                              bool include_internal_pits = true) {
     auto array = format_input<array_t>(tarray);
     std::vector<T> out = std::vector<T>(this->nnodes, 0);
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->Sreceivers[i] == i) {
+      if (this->_Sreceivers[i] == i) {
         if (include_internal_pits)
           out[i] = array[i];
         else if (this->flow_out_model(i))
           out[i] = array[i];
       }
     }
     return format_output<decltype(out), out_t>(out);
@@ -2176,30 +2181,30 @@
   // reflects the connector version of the function, but adds extra graph
   // specific checks. For example a node with permissive outletting border will
   // be active in the connector sense, but can be inactive in the graph if it
   // has no downstream neighbours.
   template <class ti_t> bool flow_out_model(ti_t node) {
 
     bool con_val = this->boundaries.can_out(node);
-    if (con_val && this->Sreceivers[node] == int(node)) {
+    if (con_val && this->_Sreceivers[node] == int(node)) {
       return true;
     }
     return false;
   }
 
   template <class ti_t> bool is_pit(ti_t node) {
 
     bool con_val = this->boundaries.can_out(node);
-    if (!con_val && this->Sreceivers[node] == int(node))
+    if (!con_val && this->_Sreceivers[node] == int(node))
       return true;
     return false;
   }
 
   template <class ti_t> bool flow_out_or_pit(ti_t node) {
-    if (this->Sreceivers[node] == int(node))
+    if (this->_Sreceivers[node] == int(node))
       return true;
     return false;
   }
 
   std::vector<int> get_n_receivers() {
     std::vector<int> nrecs(this->nnodes, 0);
     for (size_t i = 0; i < this->links.size(); ++i) {
@@ -2209,15 +2214,15 @@
         ++nrecs[frto];
       }
     }
     return nrecs;
   }
 
   template <class out_t> out_t get_SFD_receivers() {
-    return format_output<std::vector<int>, out_t>(this->Sreceivers);
+    return format_output<std::vector<int>, out_t>(this->_Sreceivers);
   }
 
   template <class out_t> out_t get_SFD_dx() {
     return format_output<std::vector<T>, out_t>(this->Sdistance2receivers);
   }
 
   template <class out_t> out_t get_SFD_ndonors() {
@@ -2288,15 +2293,15 @@
     // 	out[i] = (this->links[i] >= 1)? std::vector<int>{this->linknodes[i*2],
     // this->linknodes[i*2+1]} :  std::vector<int>{this->linknodes[i*2 + 1],
     // this->linknodes[i*2]};
     // }
     return out;
   }
 
-  int get_SFD_receivers_at_node(int i) { return this->Sreceivers[i]; }
+  int get_SFD_receivers_at_node(int i) { return this->_Sreceivers[i]; }
 
   int get_SFD_dx_at_node(int i) { return this->Sdistance2receivers[i]; }
 
   int get_SFD_ndonors_at_node(int i) { return this->nSdonors[i]; }
 
   template <class out_t> out_t get_SFD_donors_at_node(int i) {
     std::vector<int> out(this->nneighbours);
@@ -2333,16 +2338,16 @@
     auto gradient = this->_get_SFD_gradient(topography);
     return format_output<decltype(gradient), out_t>(gradient);
   }
 
   template <class topo_t> std::vector<T> _get_SFD_gradient(topo_t &topography) {
     std::vector<T> gradient(this->nnodes, 0.);
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->Sreceivers[i] != i)
-        gradient[i] = (topography[i] - topography[this->Sreceivers[i]]) /
+      if (this->_Sreceivers[i] != i)
+        gradient[i] = (topography[i] - topography[this->_Sreceivers[i]]) /
                       this->Sdistance2receivers[i];
     }
     return gradient;
   }
 
   template <class out_t, class topo_t>
   out_t get_links_gradient(topo_t &ttopography, T min_slope) {
```

### Comparing `daggerpy-0.0.4/includes/PerlinNoise.hpp` & `daggerpy-0.0.5/includes/PerlinNoise.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/_D8connector.hpp` & `daggerpy-0.0.5/includes/_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/_cordonnier_versatile_2019.hpp` & `daggerpy-0.0.5/includes/_cordonnier_versatile_2019.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
       // getting the current nodes
       size_t node = Sstack[i];
 
       if (connector->boundaries.no_data(node))
         continue;
 
       // If it is its own receiver, then
-      if (connector->Sreceivers[node] == int(node)) {
+      if (connector->_Sreceivers[node] == int(node)) {
         // incrementing the basin label
         ++this->nbas;
         // is it a base level
         if (connector->boundaries.can_out(node)) {
           // then it is an open basin
           this->is_open_basin.emplace_back(true);
           // saving its pit node
@@ -470,38 +470,38 @@
             this->is_open_basin[bas] == false)
           continue;
 
         // std::cout << "A" << std::endl;
         int from = this->receivers_node[bas].first;
         int to = this->receivers_node[bas].second;
         // std::cout << "B" << std::endl;
-        // std::cout << connector->Sreceivers[this->pitnode[bas]] << "|";
+        // std::cout << connector->_Sreceivers[this->pitnode[bas]] << "|";
 
         int A = from;
-        int B = connector->Sreceivers[A];
+        int B = connector->_Sreceivers[A];
         int C = B;
         // std::cout << "C" << std::endl;
 
         while (A != this->pitnode[bas]) {
           // std::cout << B << std::endl;
-          C = connector->Sreceivers[B];
-          connector->Sreceivers[B] = A;
+          C = connector->_Sreceivers[B];
+          connector->_Sreceivers[B] = A;
           // connector->Sdistance2receivers[B] =
           // connector->Sdistance2receivers[A];
           connector->Sdistance2receivers[B] = connector->dx;
 
           A = B;
           B = C;
         }
         // std::cout << "D" << std::endl;
 
-        connector->Sreceivers[from] = to;
+        connector->_Sreceivers[from] = to;
         connector->Sdistance2receivers[from] = connector->dx;
 
-        // std::cout << connector->Sreceivers[this->pitnode[bas]] << std::endl;
+        // std::cout << connector->_Sreceivers[this->pitnode[bas]] << std::endl;
       }
 
     } else if (method == DEPRES::cordonnier_fill) {
 
       std::vector<std::uint8_t> inQ(connector->nnodes, 0);
       auto neighbours = connector->get_empty_neighbour();
       for (int i = 0; i < this->nbas; ++i)
@@ -515,15 +515,15 @@
             this->is_open_basin[bas] == false)
           continue;
 
         int from = this->receivers_node[bas].first;
         int to = this->receivers_node[bas].second;
 
         // float_t cost = topography[to];
-        connector->Sreceivers[from] = to;
+        connector->_Sreceivers[from] = to;
         connector->Sdistance2receivers[from] = connector->dx;
         topography[from] = std::max(topography[to], topography[from]) +
                            connector->randu->get() * 1e-6 + 1e-8;
         ;
 
         std::queue<int> Q;
         Q.emplace(from);
@@ -551,15 +551,15 @@
 
             if (topography[tn] > topography[n]) {
               continue;
             }
 
             topography[tn] =
                 topography[n] + connector->randu->get() * 1e-6 + 1e-8;
-            connector->Sreceivers[tn] = n;
+            connector->_Sreceivers[tn] = n;
             connector->Sdistance2receivers[tn] =
                 connector->Sdistance2receivers[n];
             Q.emplace(tn);
             inQ[tn] = 1;
           }
         }
       }
@@ -587,27 +587,27 @@
       // 	int bas = this->stack[i];
       // 	if(connector->boundaries.can_out(this->pitnode[bas]))
       // 		continue;
 
       // 	int from = this->receivers_node[bas].first;
       // 	int to = this->receivers_node[bas].second;
       // 	float_t zref = std::max(topography[from], topography[to]);
-      // 	connector->Sreceivers[from] = to;
+      // 	connector->_Sreceivers[from] = to;
       // 	connector->Sdistance2receivers[from] = connector->dx;
       // 	isinQ[from] = true;
       // 	std::queue<int> Q;Q.emplace(from);
       // 	while(Q.empty() == false)
       // 	{
       // 		int next = Q.front();Q.pop();
       // 		isfilled[next] = true;
       // 		int nn = connector->get_neighbour_idx(next, neighbours);
 
       // 		float_t lowest_z =
-      // std::max(topography[connector->Sreceivers[next]],topography[next]);
-      // int nznodeext = connector->Sreceivers[next];
+      // std::max(topography[connector->_Sreceivers[next]],topography[next]);
+      // int nznodeext = connector->_Sreceivers[next];
 
       // 		for(int tnn = 0 ; tnn<nn; ++tnn )
       // 		{
 
       // 			int n = neighbours[tnn];
 
       // 			if (n<0 || n >= connector->nnodes)
@@ -632,24 +632,24 @@
       // 			// if(basfam[basn] != basfam[bas])
       // 			if(basn != bas)
       // 				continue;
       // 			if(basinDone[basn])
       // 				continue;
       // 			if(topography[n] <= zref)
       // 			{
-      // 				connector->Sreceivers[n] = next;
+      // 				connector->_Sreceivers[n] = next;
       // 				isinQ[n] = true;
       // 				Q.emplace(n);
       // 			}
       // 		}
 
       // 		topography[next] = std::max(lowest_z + minimum_slope +
       // connector->randu->get() * slope_randomness, topography[next]);
       // zref = std::max(topography[next],zref);
-      // connector->Sreceivers[next] = nznodeext;
+      // connector->_Sreceivers[next] = nznodeext;
       // connector->Sdistance2receivers[next] = connector->dx;
       // 	}
 
       // 	basinDone[bas] = true;
       // }
 
     }
@@ -660,15 +660,15 @@
         int bas = this->stack[i];
         if (connector->boundaries.can_out(this->pitnode[bas]))
           continue;
 
         int to = this->receivers_node[bas].second;
         // std::cout << "rerouting " << this->pitnode[bas] << " to " << to <<
         // std::endl;
-        connector->Sreceivers[this->pitnode[bas]] = to;
+        connector->_Sreceivers[this->pitnode[bas]] = to;
         connector->Sdistance2receivers[this->pitnode[bas]] = connector->dx;
       }
     }
 
     // std::cout << "DEBUGLM_II::11" <<std::endl;
 
     return true;
@@ -768,15 +768,15 @@
 // 		std::priority_queue< PQ_helper<std::pair<int,int>,float_t>,
 // std::vector<PQ_helper<std::pair<int,int>,float_t> >,
 // std::greater<PQ_helper<std::pair<int,int>,float_t> > > maPQ;
 
 // 		std::vector<int> next_nodes;
 // 		next_nodes.reserve(this->con->nx * 4);
 // 		for(int i=0; i<this->graph->nnodes; ++i) if(i ==
-// this->graph->connector->Sreceivers[i]) next_nodes.emplace_back(i);
+// this->graph->connector->_Sreceivers[i]) next_nodes.emplace_back(i);
 // bool keepon = true; 		do
 // 		{
 // 			this->toposort_section(next_nodes);
 // 			while(this->idx_stack_checker <
 // int(this->Sstack.size()))
 // 			{
 
@@ -828,15 +828,15 @@
 // 	int get_Sdonors_manual(int i)
 // 	{
 // 		// this->rinit_is_Sdonor();
 // 		int nn = this->con->get_neighbour_idx(i,this->neighbours);
 // 		int jn = 0;
 // 		for(int j=0; j< nn; ++j)
 // 		{
-// 			if(this->graph->connector->Sreceivers[this->neighbours[j]]
+// 			if(this->graph->connector->_Sreceivers[this->neighbours[j]]
 // == i)
 // 			{
 // 				// this->is_Sdonor[j] = true;
 // 				this->neighbours[jn] = this->neighbours[j];
 // 				++jn;
 // 			}
 // 		}
```

### Comparing `daggerpy-0.0.4/includes/_graph.hpp` & `daggerpy-0.0.5/includes/_graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/_old_D8connector.hpp` & `daggerpy-0.0.5/includes/_old_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/_priority_flood.hpp` & `daggerpy-0.0.5/includes/_priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/boost_spread_sort.hpp` & `daggerpy-0.0.5/includes/boost_spread_sort.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/boundary_conditions.hpp` & `daggerpy-0.0.5/includes/boundary_conditions.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/connector_checker.hpp` & `daggerpy-0.0.5/includes/connector_checker.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,75 @@
 /*
-Defines the standardised loose connection of the connectors. 
+Defines the standardised loose connection of the connectors.
 
 There are 2 different level of standards:
 
-	- the generic standard, defining the functions that will be called in the different modules. 
-They are the only one allowed in module accepting different types of connectors.
-	
-	- the specifyers standards, defining function specific to build, set and customise given subsets of connectors. 
-For example a regular grid will need nx and ny, not needed by a voronoi one. 
-THESE CAN ONLY BE CALLED OUTSIDE OF THE MODULES. The modules should not need to know how the connector is structured (loosely connected). 
-
-It uses phantom functions, called during the building of a new connector, 
-checking the said connector has all the required functions to fit the template. 
-
-
-A typical script would construct the connector first, calling generic and specific functions, 
-then throw the connector inside the module (e.g. graph, graphflood, trackscape)
-where it would only use the generic functions.
-
-That way, I can for example build a connector from a regular grid, setting the nx, ny, dx, dy and boundary condition efficiently
-and then build graphflood with that connector.
+        - the generic standard, defining the functions that will be called in
+the different modules. They are the only one allowed in module accepting
+different types of connectors.
+
+        - the specifyers standards, defining function specific to build, set and
+customise given subsets of connectors. For example a regular grid will need nx
+and ny, not needed by a voronoi one. THESE CAN ONLY BE CALLED OUTSIDE OF THE
+MODULES. The modules should not need to know how the connector is structured
+(loosely connected).
+
+It uses phantom functions, called during the building of a new connector,
+checking the said connector has all the required functions to fit the template.
+
+
+A typical script would construct the connector first, calling generic and
+specific functions, then throw the connector inside the module (e.g. graph,
+graphflood, trackscape) where it would only use the generic functions.
+
+That way, I can for example build a connector from a regular grid, setting the
+nx, ny, dx, dy and boundary condition efficiently and then build graphflood with
+that connector.
 
 */
 
-
 #ifndef CONNECTOR_CHECKER_HPP
 #define CONNECTOR_CHECKER_HPP
 
+/// Generic checker: checks if the connector has the minimal set of functions to
+/// be accepted by the other modules
+template <class Connector_t, class fT, class CONTAINER_NEIGHBOURS_INT,
+          class CONTAINER_NEIGHBOURS_fT, class VECLIKE>
+void check_connector_template_generic(Connector_t &con) {
+
+  // Generic init function
+  // Return nothing, initialise the data structure.
+  // Argument: the number of nodes in the connector (includes no data)
+  void (Connector_t::*init)(int) = &Connector_t::init;
+
+  // Generic function precomputing elements in the graph.
+  // Its interpretation is free and really depends on the type of
+  // grid/connection is needed. This is where, for example, a connector
+  // optimised for cpu can compute all the receivers/donors information from
+  // topography; an irregular grid could regrid there, or simply, if the
+  // neighbouring never caches anything for a memory-saving connector, do
+  // nothing.
+  void (Connector_t::*compute)() = &Connector_t::compute;
+
+  // Connect a (new) topography, to be used for computing receivers/donors.
+  void (Connector_t::*connect_topo)(VECLIKE &) = &Connector_t::connect_topo;
+
+  // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with
+  // nn neighbours
+  int (Connector_t::*Neighbours)(int, CONTAINER_NEIGHBOURS_INT &) =
+      &Connector_t::Neighbours;
+
+  // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT and
+  // with nn neighbours
+  int (Connector_t::*Neighbours)(int, CONTAINER_NEIGHBOURS_INT &,
+                                 CONTAINER_NEIGHBOURS_fT &) =
+      &Connector_t::neighbouring_nodes_and_distance;
+
+  // // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT
+  // with nn links int (Connector_t::*Neighbours) (int,
+  // CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_links;
 
-/// Generic checker: checks if the connector has the minimal set of functions to be accepted by the other modules
-template<class Connector_t, class fT, class CONTAINER_NEIGHBOURS_INT, class CONTAINER_NEIGHBOURS_fT, class VECLIKE>
-void check_connector_template_generic(Connector_t& con)
-{
-
-	// Generic init function
-	// Return nothing, initialise the data structure.
-	// Argument: the number of nodes in the connector (includes no data)
-	void (Connector_t::*initialisation)(int) = &Connector_t::init;
-
-	// Generic function precomputing elements in the graph.
-	// Its interpretation is free and really depends on the type of grid/connection is needed.
-	// This is where, for example, a connector optimised for cpu can compute all the receivers/donors information from topography;
-	// an irregular grid could regrid there, or simply, if the neighbouring never caches anything for a memory-saving connector, do nothing.
-	void (Connector_t::*preco)() = &Connector_t::compute;
-
-	// Connect a (new) topography, to be used for computing receivers/donors.
-	void (Connector_t::*connect_topo)(VECLIKE&) = &Connector_t::connect_topography;
-
-	// return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with nn neighbours
-	int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_nodes;
-
-	// return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT and  with nn neighbours
-	int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&, CONTAINER_NEIGHBOURS_fT&) = &Connector_t::neighbouring_nodes_and_distance;
-
-	// // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with nn links
-	// int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_links;
-
-	// Returns the area at a diven node index
-	fT (Connector_t::*Area)(int) = &Connector_t::Area;
-
+  // Returns the area at a diven node index
+  fT (Connector_t::*Area)(int) = &Connector_t::Area;
 }
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-#endif
+#endif
```

### Comparing `daggerpy-0.0.4/includes/cordonnier_versatile_2019.hpp` & `daggerpy-0.0.5/includes/cordonnier_versatile_2019.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     for (int i = 0; i < connector->nnodes; ++i) {
       // getting the current nodes
       size_t node = Sstack[i];
       if (connector->boundaries.no_data(node))
         continue;
 
       // If it is its own receiver, then
-      if (connector->Sreceivers[node] == int(node)) {
+      if (connector->_Sreceivers[node] == int(node)) {
         // incrementing the basin label
         ++this->nbas;
         // is it a base level
         if (connector->boundaries.can_out(node)) {
           // then it is an open basin
           this->is_open_basin.emplace_back(true);
           // saving its pit node
@@ -465,42 +465,42 @@
                 this->pitnode[bas])) // || this->is_open_basin[bas] == false)
           continue;
 
         // std::cout << "A" << std::endl;
         int from = this->receivers_node[bas].first;
         int to = this->receivers_node[bas].second;
         // std::cout << "B" << std::endl;
-        // std::cout << connector->Sreceivers[this->pitnode[bas]] << "|";
+        // std::cout << connector->_Sreceivers[this->pitnode[bas]] << "|";
 
         int A = from;
-        int B = connector->Sreceivers[A];
+        int B = connector->_Sreceivers[A];
         int C = B;
         // std::cout << "C" << std::endl;
 
         while (A != this->pitnode[bas]) {
           // std::cout << B << std::endl;
-          C = connector->Sreceivers[B];
-          connector->Sreceivers[B] = A;
+          C = connector->_Sreceivers[B];
+          connector->_Sreceivers[B] = A;
           // connector->Sdistance2receivers[B] =
           // connector->Sdistance2receivers[A];
           connector->Sdistance2receivers[B] = connector->dx;
 
           A = B;
           B = C;
         }
         // std::cout << "D" << std::endl;
 
-        connector->Sreceivers[from] = to;
+        connector->_Sreceivers[from] = to;
         connector->Sdistance2receivers[from] = connector->dx;
 
-        // std::cout << connector->Sreceivers[this->pitnode[bas]] << std::endl;
+        // std::cout << connector->_Sreceivers[this->pitnode[bas]] << std::endl;
       }
 
       for (int i = 0; i < connector->nnodes; ++i) {
-        if (i == connector->Sreceivers[i]) {
+        if (i == connector->_Sreceivers[i]) {
           if (connector->boundaries.force_giving(i))
             throw std::runtime_error("HAPPENS::force_giving_is_outlet");
         }
       }
 
     } else if (method == DEPRES::cordonnier_fill &&
                false) // artificially disconnected, see bellow
@@ -522,15 +522,15 @@
             this->is_open_basin[bas] == false)
           continue;
 
         int from = this->receivers_node[bas].first;
         int to = this->receivers_node[bas].second;
 
         // float_t cost = topography[to];
-        connector->Sreceivers[from] = to;
+        connector->_Sreceivers[from] = to;
         connector->Sdistance2receivers[from] = connector->dx;
         topography[from] = std::max(topography[to], topography[from]) +
                            connector->randu->get() * 1e-6 + 1e-8;
         ;
 
         std::queue<int> Q;
         Q.emplace(from);
@@ -564,15 +564,15 @@
               continue;
 
             // if( tn == 0 )
             // 	std::cout << "before::" << topography[tn];
             // topography[tn] = topography[n] + connector->randu->get() * 1e-6 +
             // 1e-8; if( tn == 0 ) 	std::cout << "after::" << topography[tn]
             // << std::endl;;
-            connector->Sreceivers[tn] = n;
+            connector->_Sreceivers[tn] = n;
             connector->Sdistance2receivers[tn] =
                 connector->Sdistance2receivers[n];
             Q.emplace(tn);
             inQ[tn] = 1;
           }
         }
       }
@@ -600,27 +600,27 @@
       // 	int bas = this->stack[i];
       // 	if(connector->boundaries.can_out(this->pitnode[bas]))
       // 		continue;
 
       // 	int from = this->receivers_node[bas].first;
       // 	int to = this->receivers_node[bas].second;
       // 	float_t zref = std::max(topography[from], topography[to]);
-      // 	connector->Sreceivers[from] = to;
+      // 	connector->_Sreceivers[from] = to;
       // 	connector->Sdistance2receivers[from] = connector->dx;
       // 	isinQ[from] = true;
       // 	std::queue<int> Q;Q.emplace(from);
       // 	while(Q.empty() == false)
       // 	{
       // 		int next = Q.front();Q.pop();
       // 		isfilled[next] = true;
       // 		int nn = connector->get_neighbour_idx(next, neighbours);
 
       // 		float_t lowest_z =
-      // std::max(topography[connector->Sreceivers[next]],topography[next]);
-      // int nznodeext = connector->Sreceivers[next];
+      // std::max(topography[connector->_Sreceivers[next]],topography[next]);
+      // int nznodeext = connector->_Sreceivers[next];
 
       // 		for(int tnn = 0 ; tnn<nn; ++tnn )
       // 		{
 
       // 			int n = neighbours[tnn];
 
       // 			if (n<0 || n >= connector->nnodes)
@@ -645,24 +645,24 @@
       // 			// if(basfam[basn] != basfam[bas])
       // 			if(basn != bas)
       // 				continue;
       // 			if(basinDone[basn])
       // 				continue;
       // 			if(topography[n] <= zref)
       // 			{
-      // 				connector->Sreceivers[n] = next;
+      // 				connector->_Sreceivers[n] = next;
       // 				isinQ[n] = true;
       // 				Q.emplace(n);
       // 			}
       // 		}
 
       // 		topography[next] = std::max(lowest_z + minimum_slope +
       // connector->randu->get() * slope_randomness, topography[next]);
       // zref = std::max(topography[next],zref);
-      // connector->Sreceivers[next] = nznodeext;
+      // connector->_Sreceivers[next] = nznodeext;
       // connector->Sdistance2receivers[next] = connector->dx;
       // 	}
 
       // 	basinDone[bas] = true;
       // }
 
     }
@@ -673,15 +673,15 @@
         int bas = this->stack[i];
         if (connector->boundaries.can_out(this->pitnode[bas]))
           continue;
 
         int to = this->receivers_node[bas].second;
         // std::cout << "rerouting " << this->pitnode[bas] << " to " << to <<
         // std::endl;
-        connector->Sreceivers[this->pitnode[bas]] = to;
+        connector->_Sreceivers[this->pitnode[bas]] = to;
         connector->Sdistance2receivers[this->pitnode[bas]] = connector->dx;
       }
     }
 
     // std::cout << "DEBUGLM_II::11" <<std::endl;
 
     return true;
@@ -781,15 +781,15 @@
 // 		std::priority_queue< PQ_helper<std::pair<int,int>,float_t>,
 // std::vector<PQ_helper<std::pair<int,int>,float_t> >,
 // std::greater<PQ_helper<std::pair<int,int>,float_t> > > maPQ;
 
 // 		std::vector<int> next_nodes;
 // 		next_nodes.reserve(this->con->nx * 4);
 // 		for(int i=0; i<this->graph->nnodes; ++i) if(i ==
-// this->graph->connector->Sreceivers[i]) next_nodes.emplace_back(i);
+// this->graph->connector->_Sreceivers[i]) next_nodes.emplace_back(i);
 // bool keepon = true; 		do
 // 		{
 // 			this->toposort_section(next_nodes);
 // 			while(this->idx_stack_checker <
 // int(this->Sstack.size()))
 // 			{
 
@@ -841,15 +841,15 @@
 // 	int get_Sdonors_manual(int i)
 // 	{
 // 		// this->rinit_is_Sdonor();
 // 		int nn = this->con->get_neighbour_idx(i,this->neighbours);
 // 		int jn = 0;
 // 		for(int j=0; j< nn; ++j)
 // 		{
-// 			if(this->graph->connector->Sreceivers[this->neighbours[j]]
+// 			if(this->graph->connector->_Sreceivers[this->neighbours[j]]
 // == i)
 // 			{
 // 				// this->is_Sdonor[j] = true;
 // 				this->neighbours[jn] = this->neighbours[j];
 // 				++jn;
 // 			}
 // 		}
```

### Comparing `daggerpy-0.0.4/includes/depression_hierarchy.hpp` & `daggerpy-0.0.5/includes/depression_hierarchy.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 // 	std::vector<int> depression_labels(connector->nnodes, -2);
 
 // 	//Step 1: label ocean-connected cells in steepest descent
 // 	for(int i=0; i<connector.nodes; ++i)
 // 	{
 // 		int node = connector.Sstack[i];
 // 		if(connector.boundaries.no_data(node)) continue;
-// 		int rec = connector.Sreceivers[node];
+// 		int rec = connector._Sreceivers[node];
 // 		if(node == rec)
 // 		{
 // 			if(connector.flow_out_model(node))
 // 			{
 // 				depression_labels[node] = -1;
 // 			}
 // 			else
@@ -282,55 +282,55 @@
 // 	}
 
 // }
 
 template <class Connector_t>
 int reroute(Connector_t *connector,
             // std::vector<int>& baslab,
-            std::vector<int> &Sreceivers, int from, int pass) {
+            std::vector<int> &_Sreceivers, int from, int pass) {
   // std::cout << "rerouting" << std::endl;
   int A = from;
-  int B = Sreceivers[A];
+  int B = _Sreceivers[A];
   bool goon = true;
   while (goon) {
-    int C = Sreceivers[B];
+    int C = _Sreceivers[B];
     if (C == B)
       goon = false;
-    Sreceivers[B] = A;
+    _Sreceivers[B] = A;
     A = B;
     B = C;
   }
 
   // int i=0;
   // do
   // {
   // 	// ++i;
-  // 	int C = Sreceivers[B];
-  // 	Sreceivers[B] = A;
+  // 	int C = _Sreceivers[B];
+  // 	_Sreceivers[B] = A;
   // 	connector->debug_print_row_col(B);
   // 	// std::cout << " now gives to "; connector->debug_print_row_col(A);
   // std::cout << "||"; 	A = B; 	B = C;
   // 	// if(i >1000)
   // 		// std::cout << A  << "|" << B << std::endl;
-  // }while(Sreceivers[B] != B);
+  // }while(_Sreceivers[B] != B);
 
   if (pass != -1)
-    Sreceivers[from] = pass;
+    _Sreceivers[from] = pass;
   else
-    Sreceivers[pass] = pass;
+    _Sreceivers[pass] = pass;
 
   return B;
 
-  // if(passout) Sreceivers[pass] = pass;
+  // if(passout) _Sreceivers[pass] = pass;
 }
 
 template <class float_t, class topo_t, class Connector_t>
 bool simple_depression_hierarchy(topo_t &topography, Connector_t *connector,
                                  std::vector<size_t> &Sstack,
-                                 std::vector<int> &Sreceivers) {
+                                 std::vector<int> &_Sreceivers) {
 
   // PROBLEM IDENTIFIED:: WHEN REROUTING THE SF, THE SFD DOES NOT NECESSARILY
   // DRAINS TO THE BASIN, ITSELF CALCULATED IN MFD LIKE
 
   // std::cout << "running?" << std::endl;
 
   // record the basin labels
@@ -346,15 +346,15 @@
   int lab = 1;
   for (int i = 0; i < connector->nnodes; ++i) {
     int node = int(Sstack[i]);
 
     if (connector->boundaries.no_data(node))
       continue;
 
-    int rec = Sreceivers[node];
+    int rec = _Sreceivers[node];
 
     if (node == rec) {
 
       if (connector->flow_out_model(node)) {
         // std::cout << "OUT!!! :: ";
         // connector->debug_print_row_col(node);
         baslab[node] = 0;
@@ -403,15 +403,15 @@
       // std::cout << " pass!";
       continue;
     }
 
     if (connector->boundaries.can_out(next.node)) {
       // std::cout << "A" << std::endl;
       // std::cout << " reroute from edges";
-      reroute(connector, Sreceivers, next.node, -1);
+      reroute(connector, _Sreceivers, next.node, -1);
       // std::cout << " done";
       // std::cout << "B" << std::endl;
       basopen[tbas] = true;
       continue;
     }
 
     int nn = connector->get_neighbour_idx(next.node, neighbours);
@@ -433,48 +433,49 @@
       // bnei != tbas))
       if (bnei >= 0) {
         if (bnei != tbas) {
 
           does_it_outlets = true;
           node_outlet.node = nei;
           node_outlet.score = topography[nei];
-          restor_Srec = Sreceivers[nei];
+          restor_Srec = _Sreceivers[nei];
         }
       }
 
       if (bnei == -1) {
         PQ.emplace(PQH(nei, topography[nei]));
         baslab[nei] = tbas;
         bnei = tbas;
-        Sreceivers[nei] = next.node;
+        _Sreceivers[nei] = next.node;
       }
     }
 
     // if(does_it_outlets && tbas ==2)
     // {
     // 	std::cout << "Processed " << next.node << " | outlet: " <<
     // node_outlet.node << std::endl;
     // }
 
     // found an outlet, rereouting
     if (does_it_outlets) {
       // std::cout << " potential outlet. ";
 
       int bnei = baslab[node_outlet.node];
-      Sreceivers[node_outlet.node] = restor_Srec;
+      _Sreceivers[node_outlet.node] = restor_Srec;
       // if(bnei == 0)
       // 	throw
 
       if (basopen[bnei] == true) {
         // std::cout << "C::" << "|" <<  node_outlet.node << "|" << next.node <<
         // "|" << basopen[bnei] << "|" << std::to_string(bnei == tbas)<<
         // std::endl; std::cout << " rerouting: link is " ;
         // connector->debug_print_row_col(node_outlet.node); std::cout << " to
         // "; connector->debug_print_row_col(next.node);
-        int lnode = reroute(connector, Sreceivers, next.node, node_outlet.node);
+        int lnode =
+            reroute(connector, _Sreceivers, next.node, node_outlet.node);
         // std::cout << "D" << std::endl;
         // basopen[tbas] = true;
         std::queue<int> basb;
 
         basb.emplace(tbas);
 
         while (basb.empty() == false) {
@@ -488,15 +489,15 @@
             // baslab[link[1]]  << std::endl;
 
             if (basopen[baslab[link[1]]] == true)
               continue;
 
             // std::cout << "C1::" << "|" <<  baslab[link[0]] << "|" <<
             // next.node << std::endl;
-            lnode = reroute(connector, Sreceivers, link[1], link[0]);
+            lnode = reroute(connector, _Sreceivers, link[1], link[0]);
             // std::cout << "D" << std::endl;
             basb.emplace(baslab[lnode]);
           }
         }
 
       } else {
         // if(tbas == bnei)
```

### Comparing `daggerpy-0.0.4/includes/fastflood.hpp` & `daggerpy-0.0.5/includes/fastflood.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     // std::cout << "DEBUGDEBUGA5" << std::endl;
     int nneg = 0;
     double exp1 = 1. / 2.;
     double exp2 = 5. / 3.;
     std::vector<bool> done(this->connector->nnodes, false);
     for (int ti = this->connector->nnodes - 1; ti >= 0; --ti) {
       int i = int(this->graph->Sstack[ti]);
-      int rec = this->connector->Sreceivers[i];
+      int rec = this->connector->_Sreceivers[i];
 
       if (gradients[i] < 0) {
         ++nneg;
         gradients[i] = 0;
       }
       // sumgrad_sqrt += std::sqrt(gradients[i]);
 
@@ -827,15 +827,15 @@
         surf[i] = this->topography[i] + this->hw[i];
       std::vector<float_t> surfpp(surf);
       (*this->graph)._compute_graph(surfpp, false, true);
     }
 
     for (int i = 0; i < this->graph->nnodes; ++i) {
       if (!this->connector->flow_out_model(i)) {
-        int rec = this->connector->Sreceivers[i];
+        int rec = this->connector->_Sreceivers[i];
         float_t dx = this->connector->Sdistance2receivers[i];
         S_h[i] = std::max((this->topography[i] + this->hw[i] -
                            this->topography[rec] - this->hw[rec]) /
                               dx,
                           0.);
       }
     }
@@ -1061,15 +1061,15 @@
 
       // if node is inactive or there is no water -> skip
       if (!this->connector->flow_out_model(node) == false ||
           this->hw[node] <= 0)
         continue;
 
       // Receiver node
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
 
       // distance to the next node and to othogonal nodes
       float_t tdx = this->connector->Sdistance2receivers[node];
       float_t tdw = this->connector->get_travers_dy_from_dx(tdx);
 
       // Getting the height of flow
       float_t thf = this->get_hflow_from_nodes(node, rec);
@@ -3452,15 +3452,15 @@
           if (tS > steepest_slope) {
             steepest_slope = tS;
             steepest_i = ri;
           } else if (tS == steepest_slope)
             throw std::runtime_error("EQUALITYYYYYY");
         }
 
-        if (this->connector->Sreceivers[i] != steepest_i)
+        if (this->connector->_Sreceivers[i] != steepest_i)
           throw std::runtime_error("QQQQWAGYNIARD");
       }
     }
     std::cout << "All good with SFD checks." << std::endl;
   }
 
 #ifdef OPENMP_YOLO
```

### Comparing `daggerpy-0.0.4/includes/fastflood_recorder.hpp` & `daggerpy-0.0.5/includes/fastflood_recorder.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/graph.hpp` & `daggerpy-0.0.5/includes/graph.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
         need_recompute = depsolver.run(this->depression_resolver, faketopo,
                                        this->connector, this->Sstack);
       }
       // else
       // {
       // 	// need_recompute = simple_depression_hierarchy<fT,
       // std::vector<fT>, Connector_t >(faketopo, this->connector, this->Sstack,
-      // this->connector->Sreceivers); 	need_recompute =
+      // this->connector->_Sreceivers); 	need_recompute =
       // simple_depression_solver
       // }
 
       // Right, if reomputed needs to be
       if (need_recompute) {
 
         // Re-inverting the Sreceivers into Sdonors
@@ -378,15 +378,15 @@
 
   void compute_npits() {
     if (this->debug_mask)
       this->_debug_mask = std::vector<std::uint8_t>(this->nnodes, 0);
 
     for (int i = 0; i < this->nnodes; ++i) {
       if (this->connector->boundaries.can_out(i) == false &&
-          i == this->connector->Sreceivers[i]) {
+          i == this->connector->_Sreceivers[i]) {
         if (this->debug_mask)
           this->_debug_mask[i] = 1;
         ++this->n_pits;
       }
     }
   }
 
@@ -539,15 +539,15 @@
     // The stack container helper
     std::stack<size_t, std::vector<size_t>> stackhelper;
     // std::vector<bool> isdone(this->nnodes,false);
     // going through all the nodes
     int istack = 0;
     for (int i = 0; i < this->nnodes; ++i) {
       // if they are base level I include them in the stack
-      if (this->connector->Sreceivers[i] == i) {
+      if (this->connector->_Sreceivers[i] == i) {
         stackhelper.emplace(i);
         // ++istack;
       }
 
       // While I still have stuff in the stack helper
       while (stackhelper.empty() == false) {
         // I get the next node and pop it from the stack helper
@@ -692,15 +692,15 @@
     for (int i = this->nnodes - 1; i >= 0; --i) {
       // Getting the node
       int node = this->Sstack[i];
       // Checking its validiyt AND if it is not a base level
       if (this->connector->flow_out_model(node))
         continue;
       // Getting the single receiver info
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       // Checking the difference in elevation
       fT dz = topography[node] - topography[rec];
       // if the difference in elevation is bellow 0 I need to carve
       if (dz <= 0) {
         // And I do ! Note that I add some very low-grade randomness to avoid
         // flat links
         topography[rec] =
@@ -715,15 +715,15 @@
   /// when a node is bellow its receiver, we correct the slope
   template <class topo_t> void fill_topo_v2(fT slope, topo_t &topography) {
     for (int i = 0; i < this->nnodes; ++i) {
       int node = this->Sstack[i];
       if (this->connector->flow_out_model(node))
         continue;
 
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       fT dz = topography[node] - topography[rec];
 
       if (dz <= 0) {
         topography[node] = std::nextafter(
             topography[rec], std::numeric_limits<fT>::max()); // * d2rec;
       }
     }
@@ -783,30 +783,30 @@
     }
 
     // IS the stack in the right order in accordance with the SStack array
     std::vector<bool> isdone(this->nnodes, false);
     for (int i = this->nnodes - 1; i >= 0; --i) {
       auto v = this->Sstack[i];
       isdone[v] = true;
-      if (int(v) != this->connector->Sreceivers[v]) {
-        if (isdone[this->connector->Sreceivers[v]]) {
+      if (int(v) != this->connector->_Sreceivers[v]) {
+        if (isdone[this->connector->_Sreceivers[v]]) {
           std::cout << "Receiver processed before node stack is fucked"
                     << std::endl;
           return false;
         }
       }
     }
 
     return true;
   }
 
   std::vector<bool> has_Srecs() {
     std::vector<bool> haSrecs(this->nnodes, true);
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->connector->Sreceivers[i] == i)
+      if (this->connector->_Sreceivers[i] == i)
         haSrecs[i] = false;
     }
     return haSrecs;
   }
 
   bool is_method_cordonnier() {
     if (this->depression_resolver == DEPRES::cordonnier_carve ||
@@ -866,15 +866,15 @@
     // marking the initial node as true
     vis[node] = true;
 
     for (auto tnode : this->Sstack) {
       // ignoring the not ode and outlets
       if (this->connector->flow_out_or_pit(tnode) == false) {
         // Getting the receiver
-        int rec = this->connector->Sreceivers[tnode];
+        int rec = this->connector->_Sreceivers[tnode];
         // checkng if receiver is visited but not node
         if (vis[rec]) {
           // current noer is visited
           vis[tnode] = true;
           // and is draining to this node
           out.emplace_back(tnode);
         }
@@ -952,15 +952,15 @@
     vis[node] = true;
 
     for (int i = this->nnodes - 1; i >= 0; --i) {
       int tnode = this->Sstack[i];
       // ignoring the not ode and outlets
       if (this->connector->flow_out_or_pit(tnode) == false) {
         // Getting the receiver
-        int rec = this->connector->Sreceivers[tnode];
+        int rec = this->connector->_Sreceivers[tnode];
         // checkng if receiver is visited but not node
         if (vis[node] && rec != node && tnode != node) {
           // current noer is visited
           vis[rec] = true;
           // and is draining to this node
           out.emplace_back(tnode);
         }
@@ -1021,15 +1021,15 @@
   std::vector<int> _get_flow_acc() {
     std::vector<int> flowacc(this->nnodes, 0);
     for (int i = this->nnodes - 1; i >= 0; --i) {
       int node = this->Sstack[i];
       if (this->connector->boundaries.no_data(node) == false)
         continue;
 
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       if (this->connector->flow_out_or_pit(node) == false) {
         flowacc[rec] += flowacc[node] + 1;
       }
     }
 
     return flowacc;
   }
@@ -1117,25 +1117,25 @@
       tot += var;
 
       if (this->connector->flow_out_or_pit(node)) {
         // if(this->connector->is_on_dem_edge(node) == false)
         // {
         // 	std::cout << "WARNING_DEBUG_45b::FLOW OUTS - NOT ON DEM EDGE "
         // << std::endl;; 	std::cout << node << "||" <<
-        // this->connector->Sreceivers[node] << std::endl;
+        // this->connector->_Sreceivers[node] << std::endl;
         // 	this->connector->debug_print_neighbours(node);
 
         // }
         if (this->connector->flow_out_model(node))
           bal -= out[node];
 
         continue;
       }
 
-      out[this->connector->Sreceivers[node]] += out[node];
+      out[this->connector->_Sreceivers[node]] += out[node];
     }
 
     // if(abs(bal) > 1e-3)
     // 	std::cout << "DEBUG BALANCE = " << bal << std::endl;
     // std::cout << "DEBUG TOTOUT " << tot << std::endl;
     return out;
   }
@@ -1159,15 +1159,15 @@
         continue;
 
       out[node] += var[node];
 
       if (this->connector->flow_out_or_pit(node))
         continue;
 
-      out[this->connector->Sreceivers[node]] += out[node];
+      out[this->connector->_Sreceivers[node]] += out[node];
     }
 
     return out;
   }
 
   template <class topo_t, class out_t>
   out_t accumulate_constant_downstream_MFD(topo_t &tweights, fT var) {
@@ -1251,15 +1251,15 @@
     for (int i = this->nnodes - 1; i >= 0; --i) {
       int node = this->Sstack[i];
 
       if (this->connector->boundaries.no_data(node))
         continue;
 
       out[node] += this->connector->get_area_at_node(node);
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       if (node != rec)
         out[rec] += out[node];
     }
     return out;
   }
 
   template <class out_t, class topo_t>
@@ -1359,15 +1359,15 @@
     for (int i = 0; i < this->nnodes; ++i) {
       // next node in the stack
       int node = this->Sstack[i];
       // checking if active
       if (this->connector->flow_out_or_pit(node))
         continue;
       // Getting the receiver
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       // And integrating the distance from outlets
       distfromoutlet[node] =
           distfromoutlet[rec] + this->connector->Sdistance2receivers[node];
     }
   }
 
   /// this function computes the flow distance from model outlets using the
@@ -1383,15 +1383,15 @@
     // the receiver
     for (int i = this->nnodes - 1; i >= 0; --i) {
       // next node in the stack
       int node = this->Sstack[i];
       // checking if active
       if (this->connector->flow_out_or_pit(node))
         continue;
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       if (distfromsources[rec] == 0 ||
           distfromsources[rec] > distfromsources[node] +
                                      this->connector->Sdistance2receivers[node])
         distfromsources[rec] =
             distfromsources[node] + this->connector->Sdistance2receivers[node];
     }
   }
@@ -1409,15 +1409,15 @@
     // the receiver
     for (int i = this->nnodes - 1; i >= 0; --i) {
       // next node in the stack
       int node = this->Sstack[i];
       // checking if active
       if (this->connector->flow_out_or_pit(node))
         continue;
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       if (distfromsources[rec] == 0 ||
           distfromsources[rec] < distfromsources[node] +
                                      this->connector->Sdistance2receivers[node])
         distfromsources[rec] =
             distfromsources[node] + this->connector->Sdistance2receivers[node];
     }
   }
@@ -1700,15 +1700,15 @@
   // depsolver.run(this->depression_resolver, faketopo, this->connector,
   // this->Sstack);
   // 		}
   // 		else
   // 		{
   // 			need_recompute = simple_depression_hierarchy<fT,
   // std::vector<fT>, Connector_t >(faketopo, this->connector, this->Sstack,
-  // this->connector->Sreceivers);
+  // this->connector->_Sreceivers);
   // 		}
 
   // 		// Right, if reomputed needs to be
   // 		if(need_recompute)
   // 		{
 
   // 			// Re-inverting the Sreceivers into Sdonors
```

### Comparing `daggerpy-0.0.4/includes/graphflood.hpp` & `daggerpy-0.0.5/includes/graphflood.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -701,15 +701,15 @@
     this->gen = std::mt19937(this->rd());
   }
 
   // # Setting initial topo (or updating topo from external sources)
   template <class topo_t> void set_topo(topo_t &topo) {
     // formatting input from higher level languages to c++ veclike stuff
     auto tin = DAGGER::format_input(topo);
-    std::vector<double> temp = DAGGER::to_vec(tin);
+    std::vector<fT> temp = DAGGER::to_vec(tin);
 
     // Initialising flow depth if not done yet
     bool inithw = false;
     if (this->_hw.size() == 0) {
       inithw = true;
       this->_hw = std::vector<fT>(this->graph->nnodes, 0);
     }
@@ -725,15 +725,15 @@
     // Done
   }
 
   // # Setting the flow depth to an external value
   template <class topo_t> void set_hw(topo_t &thw) {
     // formatting input from higher level languages to c++ veclike stuff
     auto tin = DAGGER::format_input(thw);
-    std::vector<double> temp = DAGGER::to_vec(tin);
+    std::vector<fT> temp = DAGGER::to_vec(tin);
 
     // case one: no preexisting flow depth, adding hw to hydraulic surface
     if (this->_hw.size() == 0) {
       this->_hw = std::move(temp);
       for (int i = 0; i < this->graph->nnodes; ++i)
         this->_surface[i] += this->_hw[i];
     }
@@ -1260,19 +1260,19 @@
         this->DEBUGNTOPO[node] = topological_number_v2;
       }
 
     } else {
 
       // ROUTINES FOR Single FLow Directions
       // -> Slope
-      Smax = this->get_Sw(node, this->connector->Sreceivers[node],
+      Smax = this->get_Sw(node, this->connector->_Sreceivers[node],
                           this->connector->Sdistance2receivers[node],
                           this->minslope);
       // -> rec
-      recmax = this->connector->Sreceivers[node];
+      recmax = this->connector->_Sreceivers[node];
       // -> dy (integrated width)
       dw0max = this->connector->get_travers_dy_from_dx(
           this->connector->Sdistance2receivers[node]);
       // -> dx (flow distance)
       dx = this->connector->Sdistance2receivers[node];
 
       // boundary case
@@ -1655,15 +1655,15 @@
     int ti = std::distance(FD.begin(), maxElement);
 
     std::vector<int> flow_line;
     flow_line.reserve(this->connector->nnodes);
 
     while (this->connector->flow_out_or_pit(ti) == false) {
       flow_line.emplace_back(ti);
-      ti = this->connector->Sreceivers[ti];
+      ti = this->connector->_Sreceivers[ti];
     }
     // std::cout << "Last node is " << ti << std::endl;
 
     if (this->connector->flow_out_model(ti) == false)
       std::cout << "WARNING::convergence checker flow line ends in a pit, this "
                    "can impact its liability"
                 << std::endl;
@@ -2306,15 +2306,15 @@
       int node = this->graph->Sstack[i];
 
       if (this->connector->boundaries.no_data(node))
         continue;
 
       // if(vis[node]) continue;
 
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       if (Ath < DA[node]) {
         vis[node] = true;
       } else {
         tprecs[rec] += tprecs[node];
       }
 
       vis[rec] = vis[node];
@@ -2359,15 +2359,15 @@
     std::vector<std::uint8_t> vis(this->connector->nnodes, false);
     std::vector<int> starters;
     starters.reserve(1000);
     for (int i = this->connector->nnodes - 1; i >= 0; --i) {
       int node = this->graph->Sstack[i];
       if (vis[node])
         continue;
-      int rec = this->connector->Sreceivers[node];
+      int rec = this->connector->_Sreceivers[node];
       vis[node] = true;
       if (Ath < DA[node]) {
         vis[rec] = true;
         starters.emplace_back(node);
       }
     }
 
@@ -2719,11 +2719,263 @@
       // 	{
       // 		std::cout << weights[j] << std::endl;;
       // 		throw std::runtime_error("QSREC NAN AFTER");
       // 	}
       // }
     }
   }
+
+  // EXPERIMENTAL STUFF
+  // # MAin running function
+  void run_hydro_only() {
+    // Saving the topological number if needed
+    if (this->debugntopo)
+      this->DEBUGNTOPO = std::vector<fT>(this->connector->nnodes, 0);
+
+    this->debug_CFL = 0.;
+
+    this->tau_max = 0.;
+
+    if (this->courant_dt_hydro <= 0)
+      this->courant_dt_hydro = 1e-3;
+
+    // Graph Processing
+    this->graph_automator();
+
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
+
+    // Am I in SFD or MFD
+    bool SF = (this->hydromode == HYDRO::GRAPH_SFD);
+
+    // To be used if courant dt hydro is selected
+    fT tcourant_dt_hydro = std::numeric_limits<fT>::max();
+
+    // Caching neighbours, slopes and weights
+    auto receivers = this->connector->get_empty_neighbour();
+    std::array<fT, 8> weights, slopes;
+
+    // main loop
+    for (int i = this->graph->nnodes - 1; i >= 0; --i) {
+
+      // Getting next node in line
+      int node = this->get_istack_node(i);
+
+      // Processing case where the node is a model edge, or no data
+      // this function  returns true if the node was boundary and does not need
+      // to be processed THis is where all the boundary treatment happens, if
+      // you need to add something happening at the boundaries
+      if (this->_initial_check_boundary_pit(node, receivers))
+        continue;
+
+      // Getting the receivers
+      int nrecs;
+      if (SF)
+        nrecs = 1;
+      else
+        nrecs = this->connector->get_receivers_idx_links(node, receivers);
+
+      // Caching Slope max
+      fT Smax;
+      fT dw0max;
+      fT dx;
+      int recmax = node;
+
+      // NOTE:
+      //  No need to calculate the topological number anymore, but keeping it
+      //  for recording its value
+      fT topological_number_v2 = 0.;
+
+      this->_compute_slopes_weights_et_al(node, SF, Smax, slopes, weights,
+                                          nrecs, receivers, recmax, dx, dw0max,
+                                          topological_number_v2);
+
+      // Initialising the total Qout
+      fT Qwin = this->_Qw[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+      // std:: cout << "pohw:" << pohw << "|" << this->_hw[node] << std::endl;
+
+      // Squarerooting Smax
+      // fT debug_S = Smax;
+      auto sqrtSmax = std::sqrt(Smax);
+
+      // Flow Velocity
+      fT u_flow = pohw * sqrtSmax / this->mannings(node);
+      // Volumetric discahrge
+      fT Qwout = dw0max * this->_hw[node] * u_flow;
+      // std::cout << Qwout << "|";
+
+      // Eventually recording Smax
+      if (this->record_Sw)
+        this->_rec_Sw[node] = Smax;
+
+      // transfer fluxes
+      // Computing the transfer of water and sed
+      this->_compute_transfers(nrecs, recmax, node, SF, receivers, weights,
+                               Qwin, Qwout);
+
+      // Computing courant based dt
+      if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT && u_flow > 0) {
+        fT provisional_dt = (this->courant_number * dx) / u_flow;
+        provisional_dt = std::min(provisional_dt, this->max_courant_dt_hydro);
+        provisional_dt = std::max(provisional_dt, this->min_courant_dt_hydro);
+        tcourant_dt_hydro = std::min(provisional_dt, tcourant_dt_hydro);
+      }
+
+      // computing hydro vertical motion changes for next time step
+      fT dH = this->dt_hydro(node) * (this->_Qw[node] - Qwout) /
+              this->connector->get_area_at_node(node);
+
+      this->_hw[node] += dH;
+      if (this->_hw[node] < 0) {
+        dH -= this->_hw[node];
+        this->_hw[node] = 0;
+      }
+      this->_surface[node] += dH;
+
+      if (this->record_Qw_out)
+        this->_rec_Qwout[node] += Qwout;
+    }
+
+    // if(this->tau_max > 500)
+    //  std::cout << "WARNING::tau_max is " << this->tau_max << std::endl;
+
+    // END OF MAIN LOOP
+
+    // Computing final courant based dt
+
+    if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT) {
+      if (this->courant_dt_hydro == -1)
+        this->courant_dt_hydro = 1e-3;
+      else if (tcourant_dt_hydro > 0 &&
+               tcourant_dt_hydro != std::numeric_limits<fT>::max())
+        this->courant_dt_hydro = tcourant_dt_hydro;
+    }
+
+    // if (this->convergence_mode == CONVERGENCE::ALL ||
+    //     this->convergence_mode == CONVERGENCE::DHW) {
+    //   for (int i = 0; i < this->n_nodes_convergence(); ++i)
+    //     this->conv_dhw[i].emplace_back(
+    //         vmot_hw[this->conv_nodes
+    //                     [i]]); // /this->dt_hydro(this->conv_nodes[i]));
+    // }
+
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::QWR) {
+      for (int i = 0; i < this->n_nodes_convergence(); ++i)
+        this->conv_Qr[i].emplace_back(this->_rec_Qwout[this->conv_nodes[i]] /
+                                      this->_Qw[this->conv_nodes[i]]);
+    }
+  }
+
+  // EXPERIMENTAL STUFF
+  // # MAin running function
+  void run_experimental() {
+    this->hydromode = HYDRO::GRAPH_SFD;
+    // Saving the topological number if needed
+    if (this->debugntopo)
+      this->DEBUGNTOPO = std::vector<fT>(this->connector->nnodes, 0);
+
+    this->debug_CFL = 0.;
+
+    this->tau_max = 0.;
+
+    if (this->courant_dt_hydro <= 0)
+      this->courant_dt_hydro = 1e-3;
+
+    // Graph Processing
+    this->graph_automator();
+
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
+
+    std::vector<fT> tQwin = this->graph->_accumulate_constant_downstream_SFD(
+        this->precipitations(0));
+    std::vector<fT> tQwout(this->connector->nnodes, 0.);
+    ;
+
+// main loop
+#ifdef _OPENMP
+#pragma omp parallel for num_threads(4)
+#endif
+    for (int node = 0; node < this->connector->nnodes; ++node) {
+      // Caching Slope max
+      fT Smax = this->connector->SS[node];
+      fT dx = this->connector->Sdistance2receivers[node];
+      fT dw0max = this->connector->get_travers_dy_from_dx(dx);
+      int recmax = this->connector->_Sreceivers[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+      auto sqrtSmax = std::sqrt(Smax);
+
+      // Flow Velocity
+      fT u_flow = pohw * sqrtSmax / this->mannings(node);
+      // Volumetric discahrge
+      tQwout[node] = dw0max * this->_hw[node] * u_flow;
+
+      // // Computing courant based dt
+      // if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT && u_flow > 0) {
+      //   fT provisional_dt = (this->courant_number * dx) / u_flow;
+      //   provisional_dt = std::min(provisional_dt,
+      //   this->max_courant_dt_hydro); provisional_dt =
+      //   std::max(provisional_dt, this->min_courant_dt_hydro);
+      //   tcourant_dt_hydro = std::min(provisional_dt, tcourant_dt_hydro);
+      // }
+    }
+
+#ifdef _OPENMP
+#pragma omp parallel for num_threads(4)
+#endif
+    for (int node = 0; node < this->connector->nnodes; ++node) {
+      // computing hydro vertical motion changes for next time step
+      fT dH = this->dt_hydro(node) * (this->_Qw[node] - tQwout[node]) /
+              this->connector->get_area_at_node(node);
+      this->_hw[node] += dH;
+      if (this->_hw[node] < 0) {
+        dH -= this->_hw[node];
+        this->_hw[node] = 0;
+      }
+      this->_surface[node] += dH;
+    }
+
+    if (this->record_Qw_out)
+      this->_rec_Qwout = tQwout;
+
+    // if(this->tau_max > 500)
+    //  std::cout << "WARNING::tau_max is " << this->tau_max << std::endl;
+
+    // END OF MAIN LOOP
+
+    // Computing final courant based dt
+
+    // if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT) {
+    //   if (this->courant_dt_hydro == -1)
+    //     this->courant_dt_hydro = 1e-3;
+    //   else if (tcourant_dt_hydro > 0 &&
+    //            tcourant_dt_hydro != std::numeric_limits<fT>::max())
+    //     this->courant_dt_hydro = tcourant_dt_hydro;
+    // }
+
+    // if (this->convergence_mode == CONVERGENCE::ALL ||
+    //     this->convergence_mode == CONVERGENCE::DHW) {
+    //   for (int i = 0; i < this->n_nodes_convergence(); ++i)
+    //     this->conv_dhw[i].emplace_back(
+    //         vmot_hw[this->conv_nodes
+    //                     [i]]); // /this->dt_hydro(this->conv_nodes[i]));
+    // }
+
+    // if (this->convergence_mode == CONVERGENCE::ALL ||
+    //     this->convergence_mode == CONVERGENCE::QWR) {
+    //   for (int i = 0; i < this->n_nodes_convergence(); ++i)
+    //     this->conv_Qr[i].emplace_back(this->_rec_Qwout[this->conv_nodes[i]] /
+    //                                   this->_Qw[this->conv_nodes[i]]);
+    // }
+  }
 };
 // end of graphflood class
 
 } // namespace DAGGER
```

### Comparing `daggerpy-0.0.4/includes/hillshading.hpp` & `daggerpy-0.0.5/includes/hillshading.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/npy.hpp` & `daggerpy-0.0.5/includes/npy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/popscape.hpp` & `daggerpy-0.0.5/includes/popscape.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
           this->connector.get_area_at_node(0));
       for (int i = 0; i < this->graph.nnodes; ++i) {
         int node = this->graph.Sstack[i];
 
         if (this->connector.flow_out_or_pit(node))
           continue;
 
-        int rec = this->connector.Sreceivers[node];
+        int rec = this->connector._Sreceivers[node];
         this->topography[node] =
             this->topography[rec] +
             this->connector.Sdistance2receivers[node] *
                 std::pow(this->UE(node) /
                              (this->Kbase(node) * this->Kmod(node)),
                          1. / this->n(node)) *
                 std::pow(this->QA[node], -this->m(node) / this->n(node));
@@ -266,15 +266,15 @@
   std::vector<fT> _chi_star() {
     std::vector<fT> A = this->graph._accumulate_constant_downstream_SFD(
         this->connector.get_area_at_node(0));
     std::vector<fT> chistar(this->graph.nnodes, 0.);
     fT chimax = 0;
     for (int i = 0; i < this->graph.nnodes; ++i) {
       int node = this->graph.Sstack[i];
-      int rec = this->connector.Sreceivers[node];
+      int rec = this->connector._Sreceivers[node];
       if (node == rec)
         continue;
 
       // chistar[node] = chistar[rec] +
       // this->connector.Sdistance2receivers[node] * (std::pow(1/A[node],
       // this->m(node)/this->n(node)));
       chistar[node] = chistar[rec] + this->connector.Sdistance2receivers[node] *
@@ -436,15 +436,15 @@
 
       // std::cout << nit << "|C" << std::endl;
 
       for (int i = 0; i < this->graph.nnodes; ++i) {
         int node = this->graph.Sstack[i];
         if (this->connector.flow_out_or_pit(node))
           continue;
-        int rec = this->connector.Sreceivers[node];
+        int rec = this->connector._Sreceivers[node];
         this->topography[node] =
             this->topography[rec] + this->connector.Sdistance2receivers[node] *
                                         std::pow(1e2, 1. / n) /
                                         std::pow(this->QA[node], m / n);
         // this->topography[node] = this->topography[rec] + 1;
       }
       // std::cout << nit << "|D" << std::endl;
@@ -498,15 +498,15 @@
   }
 
   void solve_SFD_SPL_imp(fT m, fT n, fT K, fT dt) {
 
     for (int i = 0; i < this->graph.nnodes; ++i) {
 
       int node = this->graph.Sstack[i];
-      int rec = this->connector.Sreceivers[node];
+      int rec = this->connector._Sreceivers[node];
 
       if (!this->connector.flow_out_or_pit(node) == false)
         continue;
 
       fT factor = K * dt * std::pow(this->QA[node], m) /
                   std::pow(this->connector.Sdistance2receivers[node], n);
 
@@ -596,19 +596,16 @@
     if (i < ncycles)
       psc.restriction(5);
   }
 
   return psc.topography;
 }
 
-
-
-template<class fT, class out_t>
-out_t quick_fluvial_topo(int ncycles, std::string boundaries)
-{
+template <class fT, class out_t>
+out_t quick_fluvial_topo(int ncycles, std::string boundaries) {
   std::vector<fT> out = _quick_fluvial_topo<fT>(ncycles, boundaries);
   return DAGGER::format_output<std::vector<fT>, out_t>(out);
 }
 
 // End of namespace fastflood
 }; // namespace DAGGER
```

### Comparing `daggerpy-0.0.4/includes/popscape_utils.hpp` & `daggerpy-0.0.5/includes/popscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/priority_flood.hpp` & `daggerpy-0.0.5/includes/priority_flood.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
         open.emplace(n, topography[n]);
         connector->update_local_link(lix, topography);
         fT dx = connector->get_dx_from_links_idx(lix);
         fT ts = (topography[n] - topography[c.node]) / dx;
         if (ts >= connector->SS[n]) {
           connector->SS[n] = ts;
-          connector->Sreceivers[n] = c.node;
+          connector->_Sreceivers[n] = c.node;
           connector->Sdistance2receivers[n] = dx;
         }
       }
     }
   }
   connector->compute_SF_donors_from_receivers();
 }
@@ -305,15 +305,15 @@
     if (connector.boundaries.no_data(node)) {
       closed[node] = true;
       ++checker;
       continue;
     }
 
     if (connector.boundaries.can_out(node) == false) {
-      closed[node] = closed[connector.Sreceivers[node]];
+      closed[node] = closed[connector._Sreceivers[node]];
 
       if (closed[node])
         ++checker;
 
       continue;
     }
```

### Comparing `daggerpy-0.0.4/includes/simple_depression_solver.hpp` & `daggerpy-0.0.5/includes/simple_depression_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
   // checking each and every nodes
   for (int i = 0; i < connector->nnodes; ++i) {
     // Ignore the ones who escape the model and/or aren't valid
     if (connector->boundaries.no_data(i) || connector->flow_out_model(i))
       continue;
 
     // then emplace if pit
-    if (connector->Sreceivers[i] == i) {
+    if (connector->_Sreceivers[i] == i) {
       sirius.emplace(PQH(i, topography[i]));
       int tlab = tree.add();
       baslab[i] = tlab;
       inQ[i] = 1;
     }
   }
 
@@ -734,15 +734,15 @@
 
 // std::vector<fT> minscore(connector->nnodes, std::numeric_limits<fT>::max());
 // std::vector<int> minnode(connector->nnodes, -1);
 // std::vector<std::uint8_t> processed(connector->nnodes, false);
 // for(auto node:Sstack)
 // {
 // 	if(connector->flow_out_model(node)) processed[node] = true;
-// 	else processed[node] = processed[connector->Sreceivers[node]];
+// 	else processed[node] = processed[connector->_Sreceivers[node]];
 // }
 
 // PQ_i_d nexus;
 
 // for(int i=0; i<connector->nlinks(); ++i)
 // {
 // 	if(connector->is_link_valid(i) == false) continue;
@@ -910,15 +910,15 @@
 // {
 
 // 	// STEP 1 LABEL ALL BASINS and fetch the one giving out
 // 	std::vector<int> basin_key(this->connector->nnodes, -1);
 // 	int lab = 0;
 // 	for(auto node : Sstack)
 // 	{
-// 		int rec = connector->Sreceivers[node];
+// 		int rec = connector->_Sreceivers[node];
 // 		if(connector->flow_out_model(node))
 // 		{
 // 			basin_key[node] = 0;
 // 		}
 // 		else if (node == rec)
 // 		{
 // 			++lab;
```

### Comparing `daggerpy-0.0.4/includes/trackscape.hpp` & `daggerpy-0.0.5/includes/trackscape.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -842,15 +842,15 @@
 
         // Check if base level
         if (this->connector.flow_out_or_pit(this->tnode)) {
           // manage the base level evolution here
           continue;
         }
 
-        this->tSrec = this->connector.Sreceivers[this->tnode];
+        this->tSrec = this->connector._Sreceivers[this->tnode];
 
         // feeding the local private variables
         this->tdx = this->connector.Sdistance2receivers[this->tnode];
         this->tdy = this->connector.get_travers_dy_from_dx(this->tdx);
         this->tZ = this->z_surf[this->tnode];
         // this->tSS = this->connector.SS[this->tnode];
         this->tSS =
@@ -1949,15 +1949,15 @@
 
   void remove_shear_height_at_once(int i, fT dZ) {
     this->h_sed[i] = std::max(0., this->h_sed[i] - dZ);
     this->z_surf[i] -= dZ;
   }
 
   void _ready_node_state() {
-    this->tSrec = this->connector.Sreceivers[this->tnode];
+    this->tSrec = this->connector._Sreceivers[this->tnode];
 
     // feeding the local private variables
     this->tdx = this->connector.Sdistance2receivers[this->tnode];
     this->tdy = this->connector.get_travers_dy_from_dx(this->tdx);
     this->tZ = this->z_surf[this->tnode];
     // this->tSS = this->connector.SS[this->tnode];
     if (this->marine == TSC_MARINE::NONE)
@@ -2136,15 +2136,15 @@
       // Getting geometrical info
       // # location
       int node = this->graph.Sstack[i];
       // # Aborting if outnode
       if (!this->connector.flow_out_or_pit(node) == false)
         continue;
       // # receiver
-      int rec = this->connector.Sreceivers[node];
+      int rec = this->connector._Sreceivers[node];
       // # distance to receiver
       fT dx = this->connector.Sdistance2receivers[node];
       // # cell area
       fT cellarea = this->connector.get_area_at_node(node);
       // # local gradient
       fT S = std::max((this->z_surf[node] - this->z_surf[rec]) / dx, 1e-9);
 
@@ -2301,15 +2301,15 @@
     } else
       this->Qw = this->graph._accumulate_constant_downstream_SFD(
           this->connector.get_area_at_node(0));
 
     for (int i = 0; i < this->graph.nnodes; ++i) {
 
       int node = this->graph.Sstack[i];
-      int rec = this->connector.Sreceivers[node];
+      int rec = this->connector._Sreceivers[node];
 
       if (this->connector.flow_out_or_pit(node))
         continue;
 
       fT tK = this->Kr(node);
 
       fT factor =
```

### Comparing `daggerpy-0.0.4/includes/trackscape_utils.hpp` & `daggerpy-0.0.5/includes/trackscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/utils.hpp` & `daggerpy-0.0.5/includes/utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/veque.hpp` & `daggerpy-0.0.5/includes/veque.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/wrap_helper.hpp` & `daggerpy-0.0.5/includes/wrap_helper.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/wrap_helper_MATLAB.hpp` & `daggerpy-0.0.5/includes/wrap_helper_MATLAB.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/wrap_helper_julia.hpp` & `daggerpy-0.0.5/includes/wrap_helper_julia.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/includes/wrap_helper_python.hpp` & `daggerpy-0.0.5/includes/wrap_helper_python.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.4/main.cpp` & `daggerpy-0.0.5/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #include "popscape_utils.hpp"
 // #include "fastflood.hpp"
 #include "graphflood.hpp"
 #include "simple_depression_solver.hpp"
 #include "trackscape.hpp"
 #include "utils.hpp"
 
+#include "river_tools_python.hpp"
+
 using namespace DAGGER;
 
 template <typename CONNECTOR_T>
 void declare_graph(py::module &m, std::string typestr) {
 
   py::class_<graph<double, CONNECTOR_T>>(m, typestr.c_str(), R"pdoc(
 Full Graph module, to plug on a connector to unlock non-local topological operations.
@@ -1329,14 +1331,16 @@
       .def("run_precipitions",
            &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_precipitions)
       .def("run_precipitions_exp",
            &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_precipitions_exp)
       .def("run_graphipiton",
            &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_graphipiton)
       .def("run_exp", &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_exp)
+      .def("run_hydro_only",
+           &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_hydro_only)
 
       .def("define_precipitations_Ath",
            &graphflood<fT, GRAPH_T, CONNECTOR_T>::define_precipitations_Ath)
 
       ;
 }
 
@@ -2271,14 +2275,18 @@
   m.def("standalone_priority_flood_opti",
         &standalone_priority_flood_opti<
             D8connector<double>,
             DAGGER::graph<double, DAGGER::D8connector<double>>,
             py::array_t<double, 1>, py::array_t<double, 1>, double>,
         py::arg("topography"), py::arg("connector"), py::arg("graph"));
 
+  m.def("RiverNetwork",
+        RiverNetwork<double, DAGGER::D8connector<double>,
+                     DAGGER::graph<double, DAGGER::D8connector<double>>>);
+
   // m.def(
   //   "check_connector_template",
   //   &check_connector_template< D8connector<double>, double >
   // );
 
   declare_popscape_old<DAGGER::D8connector<double>>(m, "popscape_old");
   declare_popscape<DAGGER::D8connector<double>>(m, "popscape");
@@ -2295,12 +2303,12 @@
                      DAGGER::D8connector<double>>(m, "graphflood");
 
   m.def("generate_perlin_noise_2D",
         &generate_perlin_noise_2D<py::array_t<double, 1>, double,
                                   D8connector<double>>);
 
   m.def("quick_fluvial_topo",
-        &quick_fluvial_topo<float, py::array_t<float, 1> >);
+        &quick_fluvial_topo<float, py::array_t<float, 1>>);
 };
 ;
 
 // end of file
```

### Comparing `daggerpy-0.0.4/setup.py` & `daggerpy-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # pybind11 is used for c++ integration
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup, find_packages
 import os
 import platform
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 
 #############################################
 # Admin inputs
 #############################################
```

### Comparing `daggerpy-0.0.4/tests/test_dagger.py` & `daggerpy-0.0.5/tests/test_dagger.py`

 * *Files identical despite different names*

