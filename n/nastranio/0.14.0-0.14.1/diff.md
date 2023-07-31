# Comparing `tmp/nastranio-0.14.0.tar.gz` & `tmp/nastranio-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nastranio-0.14.0.tar", last modified: Sat Jul 29 16:12:38 2023, max compression
+gzip compressed data, was "nastranio-0.14.1.tar", last modified: Mon Jul 31 06:05:52 2023, max compression
```

## Comparing `nastranio-0.14.0.tar` & `nastranio-0.14.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.111274 nastranio-0.14.0/
--rw-rw-r--   0 nic       (1001) nic       (1001)      172 2020-01-22 08:16:12.000000 nastranio-0.14.0/AUTHORS.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)      221 2020-01-22 08:16:12.000000 nastranio-0.14.0/CONTRIBUTING.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)       89 2020-01-22 08:16:12.000000 nastranio-0.14.0/HISTORY.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2020-01-22 08:16:12.000000 nastranio-0.14.0/LICENSE
--rw-rw-r--   0 nic       (1001) nic       (1001)      262 2020-01-22 08:16:12.000000 nastranio-0.14.0/MANIFEST.in
--rw-rw-r--   0 nic       (1001) nic       (1001)      668 2023-07-29 16:12:38.111274 nastranio-0.14.0/PKG-INFO
--rw-rw-r--   0 nic       (1001) nic       (1001)       89 2020-01-22 08:16:12.000000 nastranio-0.14.0/README.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.095274 nastranio-0.14.0/docs/
--rw-rw-r--   0 nic       (1001) nic       (1001)      610 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/Makefile
--rw-rw-r--   0 nic       (1001) nic       (1001)       28 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/authors.rst
--rwxrwxr-x   0 nic       (1001) nic       (1001)     4945 2023-04-28 07:42:45.000000 nastranio-0.14.0/docs/conf.py
--rw-rw-r--   0 nic       (1001) nic       (1001)       33 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/contributing.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)       28 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/history.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)      306 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/index.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)      102 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/installation.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)      771 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/make.bat
--rw-rw-r--   0 nic       (1001) nic       (1001)       27 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/readme.rst
--rw-rw-r--   0 nic       (1001) nic       (1001)       73 2020-01-22 08:16:12.000000 nastranio-0.14.0/docs/usage.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.099274 nastranio-0.14.0/nastranio/
--rw-rw-r--   0 nic       (1001) nic       (1001)     1479 2023-07-17 16:45:45.000000 nastranio-0.14.0/nastranio/__init__.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.099274 nastranio-0.14.0/nastranio/cards/
--rw-rw-r--   0 nic       (1001) nic       (1001)     3923 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cards/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     2030 2023-04-28 07:42:45.000000 nastranio-0.14.0/nastranio/cards/axis.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    18455 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cards/elements.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     8367 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cards/loading.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1617 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cards/materials.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    10494 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cards/properties.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     5807 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cards/types.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    46301 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cardslib.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1253 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/cli.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1435 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/constants.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    10731 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/decorators.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     7605 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/fields_writer.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.099274 nastranio-0.14.0/nastranio/mesh_api/
--rw-rw-r--   0 nic       (1001) nic       (1001)       27 2023-04-28 07:42:45.000000 nastranio-0.14.0/nastranio/mesh_api/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    89744 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/mesh_api/mesh_api.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    11809 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/mesh_api/mod.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     5885 2023-07-09 09:33:40.000000 nastranio-0.14.0/nastranio/mesh_api/rtree_indexes.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1453 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/pylib.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.103274 nastranio-0.14.0/nastranio/readers/
--rw-rw-r--   0 nic       (1001) nic       (1001)        0 2020-01-22 08:16:12.000000 nastranio-0.14.0/nastranio/readers/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    18462 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/bulk.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.103274 nastranio-0.14.0/nastranio/readers/gmsh/
--rw-rw-r--   0 nic       (1001) nic       (1001)       29 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    11627 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/gmsh.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     4359 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/mixins.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    17301 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/study.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.103274 nastranio-0.14.0/nastranio/readers/gmsh/ui_versions/
--rw-rw-r--   0 nic       (1001) nic       (1001)        0 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/ui_versions/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     4910 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/ui_versions/user_input_v1.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     9844 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/ui_versions/user_input_v2.py
--rw-rw-r--   0 nic       (1001) nic       (1001)      267 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/readers/gmsh/user_input.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     7210 2023-04-28 07:42:45.000000 nastranio-0.14.0/nastranio/readers/op2.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    12642 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/registry.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1702 2023-04-28 07:42:45.000000 nastranio-0.14.0/nastranio/serializer.py
--rw-rw-r--   0 nic       (1001) nic       (1001)      389 2021-03-23 07:27:54.000000 nastranio-0.14.0/nastranio/types.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    10920 2023-05-31 13:23:34.000000 nastranio-0.14.0/nastranio/utils.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.099274 nastranio-0.14.0/nastranio.egg-info/
--rw-rw-r--   0 nic       (1001) nic       (1001)      668 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/PKG-INFO
--rw-rw-r--   0 nic       (1001) nic       (1001)     2478 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/SOURCES.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/dependency_links.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)       50 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/entry_points.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/not-zip-safe
--rw-rw-r--   0 nic       (1001) nic       (1001)      129 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/requires.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)       10 2023-07-29 16:12:38.000000 nastranio-0.14.0/nastranio.egg-info/top_level.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)      486 2023-07-29 16:12:38.111274 nastranio-0.14.0/setup.cfg
--rw-rw-r--   0 nic       (1001) nic       (1001)     1376 2023-07-17 16:45:45.000000 nastranio-0.14.0/setup.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.103274 nastranio-0.14.0/tests/
--rw-rw-r--   0 nic       (1001) nic       (1001)       64 2020-01-22 08:16:12.000000 nastranio-0.14.0/tests/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3158 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_CBAR.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3802 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_CBUSH.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     5541 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_CQUAD4.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     5057 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_CTRIA3.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     2861 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_DUMMY.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3767 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_GRID.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    11027 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_PBEAM.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     4606 2021-03-23 07:27:55.000000 nastranio-0.14.0/tests/test_PCOMP.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     4011 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_PSHELL.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3392 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_RBE2.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     5270 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_RBE3.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    11195 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_mesh_modification.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.107274 nastranio-0.14.0/tests/test_mod/
--rw-rw-r--   0 nic       (1001) nic       (1001)       87 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_mod/README.md
--rw-rw-r--   0 nic       (1001) nic       (1001)      764 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_mod/frame_1d.geo
--rw-rw-r--   0 nic       (1001) nic       (1001)     1298 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_mod/frame_1d.msh
--rw-rw-r--   0 nic       (1001) nic       (1001)     2413 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_mod/frame_1d.nas
--rw-rw-r--   0 nic       (1001) nic       (1001)     2948 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_mod/frame_1d.params.json
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.107274 nastranio-0.14.0/tests/test_mod/run/
--rw-rw-r--   0 nic       (1001) nic       (1001)    27018 2023-03-10 07:39:33.000000 nastranio-0.14.0/tests/test_mod/run/frame_1d.ERR
--rw-rw-r--   0 nic       (1001) nic       (1001)     5698 2023-03-10 07:39:33.000000 nastranio-0.14.0/tests/test_mod/run/frame_1d.F06
--rw-rw-r--   0 nic       (1001) nic       (1001)     5996 2023-03-10 07:39:33.000000 nastranio-0.14.0/tests/test_mod/run/frame_1d.NEU
--rw-rw-r--   0 nic       (1001) nic       (1001)     1316 2023-03-10 07:39:33.000000 nastranio-0.14.0/tests/test_mod/run/frame_1d.OP2
--rw-rw-r--   0 nic       (1001) nic       (1001)     2413 2023-03-10 07:39:33.000000 nastranio-0.14.0/tests/test_mod/run/frame_1d.nas
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.111274 nastranio-0.14.0/tests/test_registry/
--rw-rw-r--   0 nic       (1001) nic       (1001)   162989 2022-10-15 07:27:34.000000 nastranio-0.14.0/tests/test_registry/bug310.nas
--rwxrwxr-x   0 nic       (1001) nic       (1001)  6185581 2020-01-22 08:30:40.000000 nastranio-0.14.0/tests/test_registry/fem20.dat
--rw-rw-r--   0 nic       (1001) nic       (1001)   563661 2022-10-26 07:27:35.000000 nastranio-0.14.0/tests/test_registry/nightstand.dat
--rw-rw-r--   0 nic       (1001) nic       (1001)    14594 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_registry/stiffpanel.nas
--rw-rw-r--   0 nic       (1001) nic       (1001)     9586 2020-01-22 08:16:12.000000 nastranio-0.14.0/tests/test_registry/test_panels.dat
--rw-rw-r--   0 nic       (1001) nic       (1001)     1326 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_registry__bug310.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     6224 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_registry__nightstand.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    11212 2023-03-28 16:15:44.000000 nastranio-0.14.0/tests/test_registry__panel.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     2652 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_registry__stiffpanel.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 16:12:38.111274 nastranio-0.14.0/tests/test_study/
--rw-rw-r--   0 nic       (1001) nic       (1001)    58861 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_study/tapered.msh
--rw-rw-r--   0 nic       (1001) nic       (1001)     3693 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_study/tapered.params.json
--rw-rw-r--   0 nic       (1001) nic       (1001)     2628 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_study/tapered.params_v1.json
--rw-rw-r--   0 nic       (1001) nic       (1001)     1414 2023-05-31 13:23:34.000000 nastranio-0.14.0/tests/test_study.py
--rw-rw-r--   0 nic       (1001) nic       (1001)      918 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_trans.py
--rw-rw-r--   0 nic       (1001) nic       (1001)      610 2023-04-28 07:42:45.000000 nastranio-0.14.0/tests/test_utils.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.492258 nastranio-0.14.1/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      172 2020-01-22 08:16:12.000000 nastranio-0.14.1/AUTHORS.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)      221 2020-01-22 08:16:12.000000 nastranio-0.14.1/CONTRIBUTING.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)       89 2020-01-22 08:16:12.000000 nastranio-0.14.1/HISTORY.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2020-01-22 08:16:12.000000 nastranio-0.14.1/LICENSE
+-rw-rw-r--   0 nic       (1001) nic       (1001)      262 2020-01-22 08:16:12.000000 nastranio-0.14.1/MANIFEST.in
+-rw-rw-r--   0 nic       (1001) nic       (1001)      668 2023-07-31 06:05:52.492258 nastranio-0.14.1/PKG-INFO
+-rw-rw-r--   0 nic       (1001) nic       (1001)       89 2020-01-22 08:16:12.000000 nastranio-0.14.1/README.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.476258 nastranio-0.14.1/docs/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      610 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/Makefile
+-rw-rw-r--   0 nic       (1001) nic       (1001)       28 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/authors.rst
+-rwxrwxr-x   0 nic       (1001) nic       (1001)     4945 2023-04-28 07:42:45.000000 nastranio-0.14.1/docs/conf.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)       33 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/contributing.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)       28 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/history.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)      306 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/index.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)      102 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/installation.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)      771 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/make.bat
+-rw-rw-r--   0 nic       (1001) nic       (1001)       27 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/readme.rst
+-rw-rw-r--   0 nic       (1001) nic       (1001)       73 2020-01-22 08:16:12.000000 nastranio-0.14.1/docs/usage.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.480258 nastranio-0.14.1/nastranio/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1479 2023-07-31 06:05:43.000000 nastranio-0.14.1/nastranio/__init__.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.480258 nastranio-0.14.1/nastranio/cards/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3923 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cards/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2030 2023-04-28 07:42:45.000000 nastranio-0.14.1/nastranio/cards/axis.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    18455 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cards/elements.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     8367 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cards/loading.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1617 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cards/materials.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    10494 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cards/properties.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5807 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cards/types.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    46301 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cardslib.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1253 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/cli.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1435 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/constants.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    10731 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/decorators.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     7605 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/fields_writer.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.480258 nastranio-0.14.1/nastranio/mesh_api/
+-rw-rw-r--   0 nic       (1001) nic       (1001)       27 2023-04-28 07:42:45.000000 nastranio-0.14.1/nastranio/mesh_api/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    89744 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/mesh_api/mesh_api.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    11809 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/mesh_api/mod.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5885 2023-07-09 09:33:40.000000 nastranio-0.14.1/nastranio/mesh_api/rtree_indexes.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1453 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/pylib.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.480258 nastranio-0.14.1/nastranio/readers/
+-rw-rw-r--   0 nic       (1001) nic       (1001)        0 2020-01-22 08:16:12.000000 nastranio-0.14.1/nastranio/readers/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    18462 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/bulk.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.484258 nastranio-0.14.1/nastranio/readers/gmsh/
+-rw-rw-r--   0 nic       (1001) nic       (1001)       29 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    11627 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/gmsh.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     4359 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/mixins.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    17301 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/study.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.484258 nastranio-0.14.1/nastranio/readers/gmsh/ui_versions/
+-rw-rw-r--   0 nic       (1001) nic       (1001)        0 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/ui_versions/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     4910 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/ui_versions/user_input_v1.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     9844 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/ui_versions/user_input_v2.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)      267 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/readers/gmsh/user_input.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     7210 2023-04-28 07:42:45.000000 nastranio-0.14.1/nastranio/readers/op2.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    12642 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/registry.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1702 2023-04-28 07:42:45.000000 nastranio-0.14.1/nastranio/serializer.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)      389 2021-03-23 07:27:54.000000 nastranio-0.14.1/nastranio/types.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    10920 2023-05-31 13:23:34.000000 nastranio-0.14.1/nastranio/utils.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.480258 nastranio-0.14.1/nastranio.egg-info/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      668 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/PKG-INFO
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2478 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/SOURCES.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/dependency_links.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)       50 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/entry_points.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/not-zip-safe
+-rw-rw-r--   0 nic       (1001) nic       (1001)      129 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/requires.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)       10 2023-07-31 06:05:52.000000 nastranio-0.14.1/nastranio.egg-info/top_level.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)      486 2023-07-31 06:05:52.496258 nastranio-0.14.1/setup.cfg
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1376 2023-07-31 06:05:43.000000 nastranio-0.14.1/setup.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.488258 nastranio-0.14.1/tests/
+-rw-rw-r--   0 nic       (1001) nic       (1001)       64 2020-01-22 08:16:12.000000 nastranio-0.14.1/tests/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3158 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_CBAR.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3802 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_CBUSH.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5541 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_CQUAD4.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5057 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_CTRIA3.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2861 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_DUMMY.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3767 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_GRID.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    11027 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_PBEAM.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     4606 2021-03-23 07:27:55.000000 nastranio-0.14.1/tests/test_PCOMP.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     4011 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_PSHELL.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3392 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_RBE2.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5270 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_RBE3.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    11195 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_mesh_modification.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.488258 nastranio-0.14.1/tests/test_mod/
+-rw-rw-r--   0 nic       (1001) nic       (1001)       87 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_mod/README.md
+-rw-rw-r--   0 nic       (1001) nic       (1001)      764 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_mod/frame_1d.geo
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1298 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_mod/frame_1d.msh
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2413 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_mod/frame_1d.nas
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2948 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_mod/frame_1d.params.json
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.488258 nastranio-0.14.1/tests/test_mod/run/
+-rw-rw-r--   0 nic       (1001) nic       (1001)    27018 2023-03-10 07:39:33.000000 nastranio-0.14.1/tests/test_mod/run/frame_1d.ERR
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5698 2023-03-10 07:39:33.000000 nastranio-0.14.1/tests/test_mod/run/frame_1d.F06
+-rw-rw-r--   0 nic       (1001) nic       (1001)     5996 2023-03-10 07:39:33.000000 nastranio-0.14.1/tests/test_mod/run/frame_1d.NEU
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1316 2023-03-10 07:39:33.000000 nastranio-0.14.1/tests/test_mod/run/frame_1d.OP2
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2413 2023-03-10 07:39:33.000000 nastranio-0.14.1/tests/test_mod/run/frame_1d.nas
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.492258 nastranio-0.14.1/tests/test_registry/
+-rw-rw-r--   0 nic       (1001) nic       (1001)   162989 2022-10-15 07:27:34.000000 nastranio-0.14.1/tests/test_registry/bug310.nas
+-rwxrwxr-x   0 nic       (1001) nic       (1001)  6185581 2020-01-22 08:30:40.000000 nastranio-0.14.1/tests/test_registry/fem20.dat
+-rw-rw-r--   0 nic       (1001) nic       (1001)   563661 2022-10-26 07:27:35.000000 nastranio-0.14.1/tests/test_registry/nightstand.dat
+-rw-rw-r--   0 nic       (1001) nic       (1001)    14594 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_registry/stiffpanel.nas
+-rw-rw-r--   0 nic       (1001) nic       (1001)     9586 2020-01-22 08:16:12.000000 nastranio-0.14.1/tests/test_registry/test_panels.dat
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1326 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_registry__bug310.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     6224 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_registry__nightstand.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    11212 2023-03-28 16:15:44.000000 nastranio-0.14.1/tests/test_registry__panel.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2652 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_registry__stiffpanel.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-31 06:05:52.492258 nastranio-0.14.1/tests/test_study/
+-rw-rw-r--   0 nic       (1001) nic       (1001)    58861 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_study/tapered.msh
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3693 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_study/tapered.params.json
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2628 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_study/tapered.params_v1.json
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1414 2023-05-31 13:23:34.000000 nastranio-0.14.1/tests/test_study.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)      918 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_trans.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)      610 2023-04-28 07:42:45.000000 nastranio-0.14.1/tests/test_utils.py
```

### Comparing `nastranio-0.14.0/PKG-INFO` & `nastranio-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nastranio
-Version: 0.14.0
+Version: 0.14.1
 Summary: Efficient Nastran Parser
 Home-page: UNKNOWN
 Author: Nicolas Cordier
 Author-email: nicolas.cordier@numeric-gmbh.ch
 License: UNKNOWN
 Keywords: nastranio
 Platform: UNKNOWN
```

### Comparing `nastranio-0.14.0/docs/Makefile` & `nastranio-0.14.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/docs/conf.py` & `nastranio-0.14.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/docs/make.bat` & `nastranio-0.14.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/__init__.py` & `nastranio-0.14.1/nastranio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.14.0"
+__version__ = "0.14.1"
 
 import logging
 import sys
 from typing import Dict, Optional
 
 from colorama import Back, Fore, Style
```

### Comparing `nastranio-0.14.0/nastranio/cards/__init__.py` & `nastranio-0.14.1/nastranio/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cards/axis.py` & `nastranio-0.14.1/nastranio/cards/axis.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cards/elements.py` & `nastranio-0.14.1/nastranio/cards/elements.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cards/loading.py` & `nastranio-0.14.1/nastranio/cards/loading.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cards/materials.py` & `nastranio-0.14.1/nastranio/cards/materials.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cards/properties.py` & `nastranio-0.14.1/nastranio/cards/properties.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cards/types.py` & `nastranio-0.14.1/nastranio/cards/types.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cardslib.py` & `nastranio-0.14.1/nastranio/cardslib.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/cli.py` & `nastranio-0.14.1/nastranio/cli.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/constants.py` & `nastranio-0.14.1/nastranio/constants.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/decorators.py` & `nastranio-0.14.1/nastranio/decorators.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/fields_writer.py` & `nastranio-0.14.1/nastranio/fields_writer.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/mesh_api/mesh_api.py` & `nastranio-0.14.1/nastranio/mesh_api/mesh_api.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/mesh_api/mod.py` & `nastranio-0.14.1/nastranio/mesh_api/mod.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/mesh_api/rtree_indexes.py` & `nastranio-0.14.1/nastranio/mesh_api/rtree_indexes.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/pylib.py` & `nastranio-0.14.1/nastranio/pylib.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/bulk.py` & `nastranio-0.14.1/nastranio/readers/bulk.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/gmsh/gmsh.py` & `nastranio-0.14.1/nastranio/readers/gmsh/gmsh.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/gmsh/mixins.py` & `nastranio-0.14.1/nastranio/readers/gmsh/mixins.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/gmsh/study.py` & `nastranio-0.14.1/nastranio/readers/gmsh/study.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/gmsh/ui_versions/user_input_v1.py` & `nastranio-0.14.1/nastranio/readers/gmsh/ui_versions/user_input_v1.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/gmsh/ui_versions/user_input_v2.py` & `nastranio-0.14.1/nastranio/readers/gmsh/ui_versions/user_input_v2.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/readers/op2.py` & `nastranio-0.14.1/nastranio/readers/op2.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/registry.py` & `nastranio-0.14.1/nastranio/registry.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/serializer.py` & `nastranio-0.14.1/nastranio/serializer.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio/utils.py` & `nastranio-0.14.1/nastranio/utils.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/nastranio.egg-info/PKG-INFO` & `nastranio-0.14.1/nastranio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nastranio
-Version: 0.14.0
+Version: 0.14.1
 Summary: Efficient Nastran Parser
 Home-page: UNKNOWN
 Author: Nicolas Cordier
 Author-email: nicolas.cordier@numeric-gmbh.ch
 License: UNKNOWN
 Keywords: nastranio
 Platform: UNKNOWN
```

### Comparing `nastranio-0.14.0/nastranio.egg-info/SOURCES.txt` & `nastranio-0.14.1/nastranio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/setup.py` & `nastranio-0.14.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     include_package_data=True,
     keywords="nastranio",
     name="nastranio",
     packages=find_packages(include=["nastranio", "nastranio.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
-    version="0.14.0",
+    version="0.14.1",
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "nastranio=nastranio.cli:main",
         ],
     },
 )
```

### Comparing `nastranio-0.14.0/tests/test_CBAR.py` & `nastranio-0.14.1/tests/test_CBAR.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_CBUSH.py` & `nastranio-0.14.1/tests/test_CBUSH.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_CQUAD4.py` & `nastranio-0.14.1/tests/test_CQUAD4.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_CTRIA3.py` & `nastranio-0.14.1/tests/test_CTRIA3.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_DUMMY.py` & `nastranio-0.14.1/tests/test_DUMMY.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_GRID.py` & `nastranio-0.14.1/tests/test_GRID.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_PBEAM.py` & `nastranio-0.14.1/tests/test_PBEAM.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_PCOMP.py` & `nastranio-0.14.1/tests/test_PCOMP.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_PSHELL.py` & `nastranio-0.14.1/tests/test_PSHELL.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_RBE2.py` & `nastranio-0.14.1/tests/test_RBE2.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_RBE3.py` & `nastranio-0.14.1/tests/test_RBE3.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mesh_modification.py` & `nastranio-0.14.1/tests/test_mesh_modification.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/frame_1d.geo` & `nastranio-0.14.1/tests/test_mod/frame_1d.geo`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/frame_1d.msh` & `nastranio-0.14.1/tests/test_mod/frame_1d.msh`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/frame_1d.nas` & `nastranio-0.14.1/tests/test_mod/frame_1d.nas`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/frame_1d.params.json` & `nastranio-0.14.1/tests/test_mod/frame_1d.params.json`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/run/frame_1d.ERR` & `nastranio-0.14.1/tests/test_mod/run/frame_1d.ERR`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/run/frame_1d.F06` & `nastranio-0.14.1/tests/test_mod/run/frame_1d.F06`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/run/frame_1d.NEU` & `nastranio-0.14.1/tests/test_mod/run/frame_1d.NEU`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/run/frame_1d.OP2` & `nastranio-0.14.1/tests/test_mod/run/frame_1d.OP2`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_mod/run/frame_1d.nas` & `nastranio-0.14.1/tests/test_mod/run/frame_1d.nas`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry/bug310.nas` & `nastranio-0.14.1/tests/test_registry/bug310.nas`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry/fem20.dat` & `nastranio-0.14.1/tests/test_registry/fem20.dat`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry/nightstand.dat` & `nastranio-0.14.1/tests/test_registry/nightstand.dat`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry/stiffpanel.nas` & `nastranio-0.14.1/tests/test_registry/stiffpanel.nas`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry/test_panels.dat` & `nastranio-0.14.1/tests/test_registry/test_panels.dat`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry__bug310.py` & `nastranio-0.14.1/tests/test_registry__bug310.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry__nightstand.py` & `nastranio-0.14.1/tests/test_registry__nightstand.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry__panel.py` & `nastranio-0.14.1/tests/test_registry__panel.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_registry__stiffpanel.py` & `nastranio-0.14.1/tests/test_registry__stiffpanel.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_study/tapered.msh` & `nastranio-0.14.1/tests/test_study/tapered.msh`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_study/tapered.params.json` & `nastranio-0.14.1/tests/test_study/tapered.params.json`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_study/tapered.params_v1.json` & `nastranio-0.14.1/tests/test_study/tapered.params_v1.json`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_study.py` & `nastranio-0.14.1/tests/test_study.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_trans.py` & `nastranio-0.14.1/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.14.0/tests/test_utils.py` & `nastranio-0.14.1/tests/test_utils.py`

 * *Files identical despite different names*

