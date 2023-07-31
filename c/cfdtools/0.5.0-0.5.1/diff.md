# Comparing `tmp/cfdtools-0.5.0.tar.gz` & `tmp/cfdtools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdtools-0.5.0.tar", last modified: Wed Jul 26 11:45:56 2023, max compression
+gzip compressed data, was "cfdtools-0.5.1.tar", last modified: Mon Jul 31 18:01:30 2023, max compression
```

## Comparing `cfdtools-0.5.0.tar` & `cfdtools-0.5.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.940114 cfdtools-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-26 11:45:34.000000 cfdtools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-26 11:45:56.940114 cfdtools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-26 11:45:34.000000 cfdtools-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.928113 cfdtools-0.5.0/cfdtools/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/cgns/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/cgns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/cgns/cgns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/gmsh/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/gmsh/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9740 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/gmsh/_gmsh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15464 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/gmsh/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/hdf5/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1693 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/hdf5/_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/ic3/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/_ic3.py
--rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/reader_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/writerV2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/writerV3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/meshbase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/physics/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/physics/dicovar.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/probes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/probes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/probes/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/probes/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/polybase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/vtk/_vtk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-26 11:45:34.000000 cfdtools-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:45:56.940114 cfdtools-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_polybase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_cgns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_ic3.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.453290 cfdtools-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 18:01:11.000000 cfdtools-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-31 18:01:30.453290 cfdtools-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-31 18:01:11.000000 cfdtools-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.437290 cfdtools-0.5.1/cfdtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.437290 cfdtools-0.5.1/cfdtools/cgns/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/cgns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/cgns/cgns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.441290 cfdtools-0.5.1/cfdtools/gmsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/gmsh/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9488 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/gmsh/_gmsh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14661 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/gmsh/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.441290 cfdtools-0.5.1/cfdtools/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/hdf5/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/hdf5/_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.441290 cfdtools-0.5.1/cfdtools/ic3/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/ic3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/ic3/_ic3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26678 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/ic3/reader_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/ic3/writerV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/ic3/writerV3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.445290 cfdtools-0.5.1/cfdtools/meshbase/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/meshbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/meshbase/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/meshbase/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/meshbase/_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/meshbase/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/meshbase/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.445290 cfdtools-0.5.1/cfdtools/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/physics/dicovar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.445290 cfdtools-0.5.1/cfdtools/probes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/probes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/probes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/probes/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.445290 cfdtools-0.5.1/cfdtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/utils/_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/utils/polybase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.445290 cfdtools-0.5.1/cfdtools/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-31 18:01:11.000000 cfdtools-0.5.1/cfdtools/vtk/_vtk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.437290 cfdtools-0.5.1/cfdtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-31 18:01:30.000000 cfdtools-0.5.1/cfdtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-31 18:01:30.000000 cfdtools-0.5.1/cfdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:01:30.000000 cfdtools-0.5.1/cfdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-31 18:01:30.000000 cfdtools-0.5.1/cfdtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-31 18:01:30.000000 cfdtools-0.5.1/cfdtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 18:01:30.000000 cfdtools-0.5.1/cfdtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-31 18:01:11.000000 cfdtools-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 18:01:30.453290 cfdtools-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:01:30.453290 cfdtools-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_0_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_0_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_0_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_0_polybase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_1_cgns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_1_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_1_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_1_ic3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_1_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_1_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_2_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_2_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_2_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 18:01:11.000000 cfdtools-0.5.1/tests/test_probes.py
```

### Comparing `cfdtools-0.5.0/LICENSE` & `cfdtools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/PKG-INFO` & `cfdtools-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdtools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for mesh and solution management in CFD
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
         Copyright (c) 2022 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cfdtools-0.5.0/README.md` & `cfdtools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/cfdtools/_cli.py` & `cfdtools-0.5.1/cfdtools/_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,105 @@
 import argparse
 from pathlib import Path
 
+# Command-Line Interface
+
 import cfdtools.api as api
 
 # readers and writers - must be imported to update api format dict
 import cfdtools.ic3 as ic3  # .reader_legacy # needed to map readers
-import cfdtools.gmsh as gmsh
-import cfdtools.cgns as cgns
+import cfdtools.gmsh as gmsh  # .reader_legacy # needed to map readers
+import cfdtools.cgns as cgns  # .reader_legacy # needed to map readers
 import cfdtools.vtk as vtk
+
 #
 import cfdtools.meshbase.simple as simplemesh
 import cfdtools.probes.plot as probeplot
 import cfdtools.probes.data as probedata
 import numpy as np
 
 # To add a command line tool, just add the function pyproject.toml in section
 # [project.scripts]
 # cfdinfo = 'cfdtools._cli:info'
 
 # print(api._fileformat_map)
 
 
-def cli_header(name):
-    api.io.print('std', "CFDTOOLS - " + name)
+# W/o  argument: @cli_header()
+#                 --> <funcname>
+# With altfname: @cli_header(altfname="<altfn>")
+#                 --> <altfname>
+# With a prefix: @cli_header("<pfx>")
+#                 --> <pfx><funcname>
+# With altfname: @cli_header("<pfx>", altfname="<altfn>")
+#                 --> <pfx><altfname>
+def cli_header(prefix=None, altfname=None):
+    def name_decorator(func):
+        def decorator(*args, **kwargs):
+            fname = func.__name__ if altfname is None else altfname
+            if prefix is not None:
+                fname = prefix + fname
+            func.__globals__['__fname__'] = fname  # need noqa: F821 for flake8 if using __fname__
+            api.io.printstd(f"CFDTOOLS - {fname}")
+            return func(*args, **kwargs)
+
+        return decorator
+
+    return name_decorator
 
 
 class cli_argparser:
     def __init__(self, **kwargs):
         self._parser = argparse.ArgumentParser(**kwargs)
         self._available_readers = list(
-            filter(
-                lambda fname: 'reader' in api._fileformat_map[fname].keys(),
-                api._fileformat_map,
-            )
+            filter(lambda fname: 'reader' in api._fileformat_map[fname].keys(), api._fileformat_map)
         )
 
     def add_argument(self, option, **kwargs):
         return self._parser.add_argument(option, **kwargs)
 
     def addarg_filenameformat(self, format=None):
         self.add_argument('filename', help="file")
         self.add_argument('--fmt', help="input file format", choices=self._available_readers, default=format)
         self.add_argument('--outpath', help="output folder path")
-        self.add_argument("--check", action="store_true", dest="check", help="process some checks")
-        self.add_argument("--info", action="store_true", dest="info", help="print information")
+        self.add_argument('--check', action="store_true", dest="check", help="process some checks")
+        self.add_argument('--info', action="store_true", dest="info", help="print information")
 
     def addarg_prefix(self):
         self.add_argument('prefix', help="prefix of files")
 
-    def addarg_data(self):
+    def addarg_filelist(self):
+        self.add_argument('filelist', nargs="+", help="list of files")
+
+    def addarg_removedata(self):
         self.add_argument(
             '--remove-node-data',
             nargs='+',
-            help="list of data to remove",
+            help="list of node data to remove",
         )
         self.add_argument(
             '--remove-face-data',
             nargs='+',
-            help="list of data to remove",
+            help="list of face data to remove",
         )
         self.add_argument(
             '--remove-cell-data',
             nargs='+',
-            help="list of data to remove",
-        )
-
-    def addarg_transform(self):
-        self.add_argument(
-            '--extrude',
-            type=int,
-            help="total number of planes",
+            help="list of cell data to remove",
         )
         self.add_argument(
-            '--scale',
-            nargs=3,
-            type=float,
-            help="x, y, z scaling coefficients",
+            '--',
+            dest='',
+            help="may be used to separate data to remove from following filename\n\n",
         )
 
+    def addarg_transform(self):
+        self.add_argument('--extrude', type=int, help="total number of planes")
+        self.add_argument('--scale', nargs=3, type=float, help="x, y, z scaling coefficients")
+
     def parse_cli_args(self, argv):
         self._args = self._parser.parse_args(argv)
 
     def args(self, key=None):
         return self._args if key is None else vars(self._args)[key]
 
     def argsdict(self):
@@ -91,141 +109,159 @@
         """parse args to get filename, automatic or specified format"""
         if self.args().fmt is None:
             ext = Path(self._args.filename).suffix
             thisfmt = list(filter(lambda n: api._fileformat_map[n]['ext'] == ext, api._fileformat_map))
         else:
             thisfmt = [self.args().fmt]
         if len(thisfmt) == 0:
-            api.error_stop('no extension found')
+            api.error_stop("no extension found")
         elif len(thisfmt) > 1:
-            api.error_stop('too many extensions found, must specify format with --fmt')
+            api.error_stop("too many extensions found\n" "must specify format with --fmt")
         self._fileformat = thisfmt[0]
         self._reader = api._fileformat_map[self._fileformat].get('reader', None)
         self._writer = api._fileformat_map[self._fileformat].get('writer', None)
 
 
+@cli_header("cfd")
 def info(argv=None):
     """call specific printinfo function from reader
 
     Args:
         argv (_type_, optional): _description_. Defaults to None.
     """
-    cli_header("cfdinfo")
     # api.io.set_modes(api.io._available)
-    parser = cli_argparser()
+    parser = cli_argparser(prog=__fname__)  # noqa: F821
     parser.addarg_filenameformat()
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     #
     inputfile = Path(parser.args('filename'))
     r = parser._reader(str(inputfile), cIntegrity=parser.args('check'))
     r.read_data()
     mesh = r.export_mesh()
     mesh.printinfo()
     return True  # needed for pytest
 
 
+@cli_header()
 def ic3brief(argv=None):
-    cli_header("ic3brief")
-    parser = cli_argparser()
+    parser = cli_argparser(prog=__fname__)  # noqa: F821
     parser.addarg_filenameformat(format='IC3')
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     #
     r = ic3.binreader(parser.args().filename)
     r.read_headers()
     return True  # needed for pytest
 
 
+@cli_header()
 def vtkbrief(argv=None):
-    cli_header("vtkbrief")
     parser = cli_argparser()
     parser.addarg_filenameformat(format="VTK")
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     #
     r = vtk.vtkMesh()
     r.read(parser.args().filename)
     r.brief()
     return True  # needed for pytest
 
 
-def write_generic(argv, ext, writer):
+@cli_header()
+def vtkpack(argv=None):
     parser = cli_argparser()
+    parser.addarg_filelist()
+    parser.parse_cli_args(argv)
+    #
+    api.io.printstd(f"> number of files: {len(parser.args().filelist)}")
+    vtklist = vtk.vtkList(parser.args().filelist, verbose=True)
+    if vtklist.allexist():
+        api.io.printstd("  all files exist")
+    else:
+        api.error_stop("some files are missing")
+    vtklist.read()
+    outfilename = vtklist.dumphdf("dumped.h5")
+    api.io.printstd(f"> mesh and data dumped to {outfilename}")
+    return True  # needed for pytest
+
+
+def write_generic(argv, ext, writer, fname=None):
+    parser = cli_argparser(prog=fname)
     parser.addarg_filenameformat()
-    parser.addarg_data()
+    parser.addarg_removedata()
     parser.addarg_transform()
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     #
     file = api._files(parser.args().filename)
-    api.io.print(f'> read mesh file {file.filename}')
+    api.io.printstd(f"> read mesh file {file.filename}")
     timer = api.Timer()
     timer.start()
     r = parser._reader(file.filename)
     r.read_data()
     ncell = r.ncell
     timer.stop(nelem=ncell)
-    api.io.print('std', f"> export mesh ")
+    api.io.printstd("> export mesh ")
     cfdmesh = r.export_mesh()
     #
     if parser.args().remove_cell_data:
         for var in parser.args().remove_cell_data:
             if cfdmesh.pop_celldata(var) is None:
-                api.io.print('std', f'  cannot find cell data {var}')
+                api.io.printstd(f"  cannot find cell data {var}")
             else:
-                api.io.print('std', f'  pop cell data {var}')
+                api.io.printstd(f"  pop cell data {var}")
     #
     if parser.args().outpath is None:
         file.remove_dir()
     else:
         file.change_dir(parser.args().outpath)
     file.change_suffix(ext)
     if file.find_safe_newfile() > 0:
-        api.io.print("std", "change output to safe new name " + file.filename)
+        api.io.printstd("change output to safe new name " + file.filename)
     if parser.args().extrude:
         timer.start()
         nz = parser.args().extrude
-        api.io.print(f'> extrusion along nz={nz} cells, {nz*ncell} total cells')
+        api.io.printstd(f"> extrusion along nz={nz} cells, {nz*ncell} total cells")
         cfdmesh = cfdmesh.export_extruded(extrude=np.linspace(0.0, 1.0, nz + 1, endpoint=True))
         timer.stop(nelem=nz * ncell)
     if parser.args().scale:
         cfdmesh.scale(parser.args().scale)
     if parser.args().info:
         cfdmesh.printinfo()
     output = writer(cfdmesh)
     output.write_data(file.filename)
-    api.io.print('std', f"file {file.filename} written")
-    return file.filename  # True # needed for pytest (True not needed, filename for eventual rm)
+    api.io.printstd(f"file {file.filename} written")
+    return file.filename  # filename needed for pytest (for eventual rm)
 
 
+@cli_header("cfd")
 def write_ic3v2(argv=None):
-    cli_header("cfdwrite_ic3v2")
-    return write_generic(argv, '.ic3', ic3.writerV2.writer)
+    return write_generic(argv, '.ic3', ic3.writerV2.writer, fname=__fname__)  # noqa: F821
 
 
+@cli_header("cfd")
 def write_ic3v3(argv=None):
-    cli_header("cfdwrite_ic3v3")
-    return write_generic(argv, '.ic3', ic3.writerV3.writer)
+    return write_generic(argv, '.ic3', ic3.writerV3.writer, fname=__fname__)  # noqa: F821
 
 
+@cli_header("cfd")
 def write_vtk(argv=None):
-    cli_header("cfdwrite_vtk")
-    return write_generic(argv, '.vtu', vtk.vtkMesh)
+    return write_generic(argv, '.vtu', vtk.vtkMesh, fname=__fname__)  # noqa: F821
 
 
+@cli_header("cfd")
 def writecube(argv=None):
-    cli_header("cfdwritecube")
     """call specific printinfo function from reader
 
     Args:
         argv (_type_, optional): _description_. Defaults to None.
     """
     # api.io.set_modes(api.io._available)
-    parser = cli_argparser()
+    parser = cli_argparser(prog=__fname__)  # noqa: F821
     parser.addarg_filenameformat()
     parser.add_argument(
         "--nx",
         action="store",
         dest="nx",
         default=10,
         type=int,
@@ -247,65 +283,97 @@
         type=int,
         help="number of cells in z direction",
     )
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     nx, ny, nz = parser.args().nx, parser.args().ny, parser.args().nz
     #
-    api.io.print('std', f"> create Cube {nx}x{ny}x{nz}")
+    api.io.printstd(f"> create Cube {nx}x{ny}x{nz}")
     cube = simplemesh.Cube(nx, ny, nz)
     mesh = cube.export_mesh()
     #
     file = api._files(parser.args().filename)
     w = parser._writer(mesh)
     w.write_data(file.filename)
-    return file.filename  # True # needed for pytest (True not needed, filename for eventual rm)
+    return file.filename  # filename needed for pytest (for eventual rm)
 
 
+@cli_header()
 def ic3probe_plotline(argv=None):
-    cli_header("ic3probe_plotline")
     parser = cli_argparser(description="Process line probes from IC3")
     parser.addarg_prefix()
     # parser.add_argument("filenames", nargs="*", help="list of files")
-    parser.add_argument("-v", action="store_true", dest="verbose", help="verbose output")
-    parser.add_argument("--data", action="store", dest="datalist", default="P", help="quantity to plot")
-    parser.add_argument("--axis", action="store", dest="axis", default="X", help="axis to follow")
+    parser.add_argument(
+        "-v",
+        action="store_true",
+        dest="verbose",
+        help="verbose output",
+    )
+    parser.add_argument(
+        "--data",
+        action="store",
+        dest="datalist",
+        default="P",
+        help="quantity to plot",
+    )
+    parser.add_argument(
+        "--axis",
+        action="store",
+        dest="axis",
+        default="X",
+        help="axis to follow",
+    )
     parser.add_argument(
         "--map",
         action="store",
         dest="map",
         default="time",
         choices=["time", "freq"],
         help="type of map",
     )
-    parser.add_argument("--check", action="store_true", dest="check", help="process some checks")
-    parser.add_argument("--cmap", action="store", dest="cmap", default="turbo", help="colormap")
+    parser.add_argument(
+        "--check",
+        action="store_true",
+        dest="check",
+        help="process some checks",
+    )
+    parser.add_argument(
+        "--cmap",
+        action="store",
+        dest="cmap",
+        default="turbo",
+        help="colormap",
+    )
     parser.add_argument(
         "--cmaplevels",
         action="store",
         dest="nlevels",
         default=30,
         type=int,
         help="colormap number of levels",
     )
     parser.parse_cli_args(argv)
     # parser.parse_filenameformat()
     # basename, ext = os.path.splitext(parser.args().filenames[0])
     var = parser.args('datalist')[0]  # ext[1:]
     basename = parser.args('prefix')
+    # axis must be the last to get right time size
     expected_data = [
         var,
         parser.args().axis,
-    ]  # axis must be the last to get right time size
+    ]
     # check files and read data
     data = probedata.phydata(basename, verbose=parser.args().verbose)
 
     api.io.printstd(f"> read data in {basename}")
     for ivar in expected_data:
         data.check_data(ivar, prefix=basename)
 
     # --- read all expected data ---
-    api.io.print('std', "> processing " + parser.args().map + " map of " + var)
-    run_plot = {"time": probeplot.plot_timemap, "freq": probeplot.plot_freqmap}
+    api.io.printstd(f"> processing {parser.args().map} map of {var}")
+    run_plot = {
+        "time": probeplot.plot_timemap,
+        "freq": probeplot.plot_freqmap,
+    }
 
     # run
     run_plot[parser.args().map](data, **parser.argsdict())
```

### Comparing `cfdtools-0.5.0/cfdtools/api.py` & `cfdtools-0.5.1/cfdtools/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from functools import wraps
+from collections import namedtuple
 from pathlib import Path
 import numpy as np
 import time
 
 _fileformat_map = {}
 
 
 def fileformat_reader(name, extension):
-    """decorator to register fileformat properties for given name in api._fileformat_map
+    """decorator to register fileformat properties for given name
+       in api._fileformat_map
 
     a reader is a class which is initialized with a filename
     and has the following functions
     - read_data()
     - export_mesh() which returns a meshbase._mesh.mesh class
     """
 
@@ -23,15 +25,17 @@
             _fileformat_map[name] = properties
         return thisclass
 
     return decorator
 
 
 def fileformat_writer(name, extension):
-    """decorator to register fileformat properties for given name  in api._fileformat_map"""
+    """decorator to register fileformat properties for given name
+       in api._fileformat_map
+    """
 
     def decorator(thisclass):
         properties = {'writer': thisclass, 'ext': extension}
         if name in _fileformat_map:
             _fileformat_map[name].update(properties)
         else:
             _fileformat_map[name] = properties
@@ -51,14 +55,15 @@
     else:
         print(string + ': ' + str(type(value)))
 
 
 class api_output:
     """class to handle library outputs"""
 
+    _contd = False
     _prefix = {
         'internal': 'int:',
         'error': 'ERROR:',
         'warning': 'WARNING:',
         'std': '',
         'debug': 'debug:',
     }
@@ -84,16 +89,32 @@
     def get_modes(self):
         return self._api_output
 
     def set_default(self):
         self.set_modes(self._default)
 
     def print(self, mode, *args, **kwargs):
+        if self._contd:
+            # if timed, pass the line to be continued...
+            print()
+            # ...and tell the timer stop printer
+            self._contd = False
         if mode in self._api_output:
-            print(self._prefix[mode], *args, **kwargs)
+            prefix = self._prefix[mode]
+            if len(prefix) == 0:
+                # avoid leading space if prefix is empty
+                print(*args, **kwargs)
+            else:
+                spcpfx = (len(prefix) + 1) * ' '
+                # add space-replaced prefix for additional lines
+                print(
+                    prefix,
+                    *([s.replace('\n', '\n' + spcpfx) for s in args]),
+                    **kwargs
+                )
 
     def printstd(self, *args, **kwargs):
         self.print('std', *args, **kwargs)
 
     def printdebug(self, *args, **kwargs):
         self.print('debug', *args, **kwargs)
 
@@ -145,89 +166,119 @@
         folder = safepath.parent
         stem = safepath.stem
         suff = safepath.suffix
         i = 0
         while safepath.exists():
             i += 1
             # safepath = safepath.with_stem(stem+f'({i})') # only python >= 3.9
-            # print(dir,stem,f'({i})',suff)
+            # print(folder, stem, f"({i})", suff)
             safepath = Path(folder / (stem + f'({i})' + suff))
         self._path = safepath
         return i > 0
 
     def printinfo(self):
         print(self)
 
 
 class TimerError(Exception):
     """A custom exception used to report errors in use of Timer class"""
 
 
 class Timer:  # from https://realpython.com/python-timer/
-    default_tab = 60
+    default_ltab = 60
     default_msg = ""
 
-    def __init__(self, task="", msg=default_msg, nelem=None, tab=default_tab):
+    def __init__(self, task="", msg=default_msg, nelem=None, ltab=default_ltab):
         self.reset()
         self._nelem = nelem
-        self._tab = tab
+        self._ltab = ltab
         self._task = task
         self._msg = msg
 
     def reset(self):
         self._start_time = None
         self._task = ""
-        self._col = 0
+        self._ncol = 0
         self._elapsed = 0.
 
     @property
     def elapsed(self):
         return self._elapsed
-        
+
     def start(self):
         """Start a new timer"""
         if self._start_time is not None:
-            raise TimerError(f"Timer is running. Use .stop() to stop it")
+            raise TimerError("Timer is running. Use .stop() to stop it")
         self._start_time = time.perf_counter()
 
     def pause(self):
         """Stop the timer, add elapsed and do NOT report"""
         if self._start_time is None:
-            raise TimerError(f"Timer is not running. Use .start() to start it")
+            raise TimerError("Timer is not running. Use .start() to start it")
         self._elapsed += time.perf_counter() - self._start_time
         self._start_time = None
 
     def stop(self, nelem=None):
         """Stop the timer, and report the elapsed time"""
         if nelem is not None:
             self._nelem = nelem
         self.pause()
         normalized_time_ms = (
             0.0 if self._nelem is None else 1e6 * self._elapsed / self._nelem
         )
+        if io._contd:
+            # There was no print, line can be continued
+            io._contd = False
+        else:
+            # There was a print, line is restarted
+            self._ncol = 0
+        nspc = (self._ltab - self._ncol) * ' '
+        io.printstd(nspc + f"wtime: {self._elapsed:0.4f}s", end='')
         if self._nelem is None:
-            io.printstd(f"{' '*(self._tab-self._col)}wtime: {self._elapsed:0.4f}s")
+            io.printstd("")
         else:
-            io.printstd(f"{' '*(self._tab-self._col)}wtime: {self._elapsed:0.4f}s | {normalized_time_ms:0.4f}µs/elem",)
+            io.printstd(f" | {normalized_time_ms:0.4f}µs/elem",)
         # reset
         self.reset()
 
     def __enter__(self):
-        io.print('std', self._task, end='')
-        self._col = len(self._task) + 1
+        # Print line to be continued
+        io.printstd(self._task, end='')
+        self._ncol = len(self._task)
+        # If line is too long...
+        if self._ncol >= self._ltab:
+            self._ncol = 0
+            # ...then line is restarted...
+            io.printstd('')
+        # ...else line is continued
+        else:
+            io._contd = True
         self.start()
 
     def __exit__(self, *exitoptions):
         self.stop()
 
 
 def memoize(f):
     cache = {}
+    hits = 0
+    misses = 0
+    maxsize = None
+
+    _CacheInfo = namedtuple("CacheInfo", ["hits", "misses", "maxsize", "currsize"])
+
+    def cache_info():
+        return _CacheInfo(hits, misses, maxsize, len(cache))
 
     @wraps(f)
     def wrapper(*args):
-        if not args in cache:
+        nonlocal hits, misses
+        if args in cache:
+            hits += 1
+        else:
+            misses += 1
             cache[args] = f(*args)
         # Warning: You may wish to do a deepcopy here if returning objects
         return cache[args]
 
+    wrapper.cache_info = cache_info
     return wrapper
```

### Comparing `cfdtools-0.5.0/cfdtools/cgns/cgns.py` & `cfdtools-0.5.1/cfdtools/cgns/cgns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # cgns.py
 from pathlib import Path
-from cfdtools.api import io, error_stop, fileformat_reader, memoize
+try:
+    from functools import cache  # python >= 3.9
+except ImportError:
+    from functools import lru_cache  #  3.6 <= python <= 3.8
+    cache = lru_cache(maxsize=None)
+    del lru_cache
+from cfdtools.api import io, error_stop, fileformat_reader  # , memoize
 from cfdtools.hdf5 import h5File, h5_str
 from cfdtools.meshbase._mesh import Mesh, submeshmark
-import cfdtools.meshbase._connectivity as conn
-import cfdtools.meshbase._elements as ele
-import numpy as np
+import cfdtools.meshbase._connectivity as _conn
+import cfdtools.meshbase._elements as _elem
 
 cgtype = {}
 ele_cgns2local = {2: 'node1', 3: 'bar2', 5: 'tri3', 7: 'quad4', 17: 'hexa8'}
 
 
 def cgnstype(obj):
     cgnsdatatype = obj.attrs.get('label')
@@ -24,14 +29,15 @@
     assert cgnstype(bc) in [b"BC_t", b"GridConnectivity_t"]
     if "GridLocation" in bc.keys():
         bcloc = h5_str(bc["GridLocation/ data"])
     else:
         bcloc = "Vertex"
     return bcloc
 
+
 class cgnszone:
     def __init__(self, zone, geodim=None) -> None:
         self._zone = zone
         self._zonetype = h5_str(zone["ZoneType/ data"])
         self._geodim = geodim
         assert self._zonetype == "Unstructured", "Only Unstructured zone expected"
         # look for Elements
@@ -55,68 +61,69 @@
     def coords(self):
         x = self._zone['GridCoordinates']['CoordinateX/ data'][:]
         y = self._zone['GridCoordinates']['CoordinateY/ data'][:]
         z = self._zone['GridCoordinates']['CoordinateZ/ data'][:]
         return x, y, z
 
     def elemcon(self, geodim):
-        cellconn = conn.elem_connectivity()
+        cellconn = _conn.elem_connectivity()
         for _, elements in self._elems.items():
             cgnstype = elements[" data"][0]
             etype = ele_cgns2local[cgnstype]
-            nnode = ele.nnode_elem[etype]
+            nnode = _elem.nnode_elem[etype]
             # extract cell connectivity only
-            if ele.elem_dim[etype] == geodim:
-                index = conn.indexlist(irange=elements["ElementRange/ data"][:] - 1)
+            if _elem.elem_dim[etype] == geodim:
+                index = _conn.indexlist(irange=elements["ElementRange/ data"][:] - 1)
                 econ = elements["ElementConnectivity/ data"][:].reshape((-1, nnode))
-                econ -= 1 # shift node index (starts 0)
+                econ -= 1  # shift node index (starts 0)
                 cellconn.add_elems(etype, econ, index)
         return cellconn
 
-    def export_cellcon(self): 
+    def export_cellcon(self):
         return self.elemcon(self._geodim)
 
-    @memoize
+    # @memoize
+    @cache
     def export_facecon(self):
         return self.elemcon(self._geodim-1)
 
     def export_BC(self, BC):
         if "FamilyName" in BC.keys():
             name = h5_str(BC["FamilyName/ data"])
         else:
-            name = Path(BC.name).name # extract final name of 
+            name = Path(BC.name).name  # extract final name of
         boco = submeshmark(name)
         boco.geodim = 'node'  # don't know if node, intnode or bdnode
         boco.type = 'boundary'
         boco.properties['BCtype'] = h5_str(BC[" data"])
         boco.properties['periodic_transform'] = None
         if "PointList" in BC.keys():
-            indexlist = (BC["PointList/ data"][:] - 1).ravel().tolist() 
+            indexlist = (BC["PointList/ data"][:] - 1).ravel().tolist()
             gridloc = cg_gridlocation(BC)
-        elif "ElementList" in BC.keys(): # not in CGNS norm
-            indexlist = (BC["ElementList/ data"][:] - 1).ravel().tolist() 
+        elif "ElementList" in BC.keys():  # not in CGNS norm
+            indexlist = (BC["ElementList/ data"][:] - 1).ravel().tolist()
             gridloc = "FaceCenter"
             if len(indexlist) == self.ncell:
                 gridloc = "CellCenter"
                 boco.type = 'internal'
         else:
             error_stop(f"Unknown indexing of BC mark: {name}")
         # convert to node marks
         if gridloc == "FaceCenter":
             nodelist = self.export_facecon().nodes_of_indexlist(indexlist)
         elif gridloc == "Vertex":
             nodelist = indexlist
             if len(nodelist) == self.nnode:
                 boco.type = 'internal'
         elif gridloc == "CellCenter":
-            nodelist = indexlist # cells indeed
+            nodelist = indexlist  # cells indeed
             boco.geodim = 'cell'
         else:
             error_stop(f'unknown gridlocation {gridloc}')
-        boco.index = conn.indexlist(ilist=nodelist)  # must start at 0
+        boco.index = _conn.indexlist(ilist=nodelist)  # must start at 0
         return boco
 
 
 class cgnsfile(h5File):
     def __init__(self, filename: str):
         super().__init__(filename)
         self.open()
@@ -138,19 +145,23 @@
 
 @fileformat_reader('CGNS', '.cgns')
 class cgnsMesh:
     def __init__(self, filename) -> None:
         self._filename = filename
         self._ncell = None
 
-    @property 
+    @property
     def ncell(self):
         return self._ncell
-    
+
     def read_data(self, zone=None):
+        io.printstd(f"> CGNS reader: starts reading {self._filename}")
+        # Check file exists
+        if not Path(self._filename).exists():
+            error_stop(f"File not found: {self._filename!r}")
         self._file = cgnsfile(self._filename)
         # get BASE list
         self._bases = self._file.list_bases()
         for base in self._bases:
             # print('base', self._file._h5file[base].name, self._file._h5file[base][" data"][:])
             self._zones = dict_cgnstype(self._file._h5file[base], b'Zone_t')
         # geo dimension from base
@@ -162,42 +173,41 @@
             name = list(self._zones.keys())[0]
         else:
             name = zone
         self._zonename = name
         self._zone = cgnszone(self._zones[name], self._geodim)
         self._ncell = self._zone.ncell
 
-
     def printinfo(self):
         # super().printinfo()
         self._file.printinfo()
-        io.print('std', 'CGNS version:', self._file._cgnsver)
-        io.print('std', 'bases:', self._bases)
-        io.print('std', 'zones:', list(self._zones.keys()))
+        io.printstd('CGNS version:', self._file._cgnsver)
+        io.printstd('bases:', self._bases)
+        io.printstd('zones:', list(self._zones.keys()))
         for zn, _ in self._zones.items():
-            io.print('std', f"  Zone {zn}")
+            io.printstd(f"  Zone {zn}")
             # for bcn, bc in
 
     def export_mesh(self):
-        # io.print('std', f"> export mesh ") # printed by parent
+        # io.printstd(f"> export mesh ") # printed by parent
         cgzone = self._zone
         io.printstd(f"Parse zone {self._zonename} ({self._geodim}D) ncell: {cgzone.ncell}, nnode: {cgzone.nnode}",)
         meshdata = Mesh(ncell=cgzone.ncell, nnode=cgzone.nnode)
         # get coordinates
         meshdata.set_nodescoord_xyz(*cgzone.coords())
         # # cell connectivity
         meshdata.set_cell2node(cgzone.export_cellcon())
         # boundary conditions
         for _, bc in cgzone._BCs.items():
             boco = cgzone.export_BC(bc)
             # filter full domain
             if boco.type in ['internal']:
-                io.print('std', f"  filter internal mark {boco.name}")
+                io.printstd(f"  filter internal mark {boco.name}")
             else:
-                io.print('std', f"  add boco {boco}")
+                io.printstd(f"  add boco {boco}")
                 meshdata.add_boco(boco)
         # meshdata.check()
         # meshdata.printinfo()
         return meshdata
 
 
 # if __name__ == "__main__":
```

### Comparing `cfdtools-0.5.0/cfdtools/data.py` & `cfdtools-0.5.1/cfdtools/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import numpy as np
 import numpy.fft as fftm
 import matplotlib.pyplot as plt
 import cfdtools.api as api
 import cfdtools.hdf5 as hdf5
 
-# import numpy as np
-
 
 class DataSetBase:
 
     _available_Xrep = ('nodal', 'cellaverage')
     _available_Trep = 'instant'
 
     def __init__(self, Xrep='cellaverage', ndof=1, Trep='instant'):
         self.Trep = Trep
         self.Xrep = Xrep
-        self.ndof = ndof # must be placed after Xrep set up
+        self.ndof = ndof  # must be placed after Xrep set up
         self.xsize = 0
         self._properties = dict()
         self._geoprop = dict()
 
     @property
     def ndof(self):
         return self._ndof
@@ -102,52 +100,56 @@
     def plot(self, x, y, axes=plt, **kwargs):
         axes.plot(self._data[x], self._data[y], **kwargs)
 
     def contourf(self, x, y, v, axes=plt, **kwargs):
         axes.contourf(self._data[x], self._data[y], self._data[v].T, **kwargs)
 
     def dataSet_spectrum(self, datafilter=None, imin=None, imax=None):
-        dtavg, dtdev, n = self.dtstats(imin, imax) # check 'timeevol'
+        dtavg, dtdev, n = self.dtstats(imin, imax)  # check 'timeevol'
         if dtdev / dtavg > 1.e-6:
-            api.io.warning(f"dt standard deviation is significant: {dtdev / dtavg}")
+            api.io.warning(
+                f"dt standard deviation is significant: {dtdev / dtavg}"
+            )
         f = fftm.fftfreq(n, dtavg)
         newdataset = DataSet(self.Xrep, self.ndof, Trep='spectrum')
         newdataset.add_data('freq', f)
         datalist = datafilter if datafilter else list(self.keys())
         datalist.remove('time')
         for name in datalist:
             newdataset.add_data(name, np.abs(fftm.fft(self[name]-dtavg)))
         return newdataset
 
     def dataSet_spectrogram(self, datafilter=None, window=None):
         lowcrop = 2
         datalist = datafilter if datafilter else list(self.keys())
         datalist.remove('time')
-        dtavg, dtdev, ntot = self.dtstats() # check 'timeevol'
-        #print(dtavg, dtdev)
+        dtavg, dtdev, ntot = self.dtstats()  # check 'timeevol'
+        # print(dtavg, dtdev)
         if dtdev / dtavg > 1.e-6:
-            api.io.warning(f"dt standard deviation is significant: {100*dtdev / dtavg:.4f}%")
+            api.io.warning(
+                f"dt standard deviation is significant: {100*dtdev / dtavg:.4f}%"
+            )
         newdataset = DataSet(self.Xrep, self.ndof, Trep='spectrogram')
         nwind = window if window else int(ntot/100)
         hwin = int(nwind/2)
         f = fftm.fftfreq(nwind, dtavg)
         newdataset.add_data('freq', f[lowcrop:hwin+1])
         nit = int(2*ntot/nwind)-1
         newdataset.add_data('time', (self['time'][hwin::hwin])[:-1])
         for name in datalist:
             v = np.zeros((nit, hwin+1-lowcrop))
-            #print(ntot, nit, nwind, hwin, newdataset['freq'].shape, f.shape)
+            # print(ntot, nit, nwind, hwin, newdataset['freq'].shape, f.shape)
             for i in range(nit):
                 v[i,:] = np.log(np.abs(fftm.rfft(self[name][hwin*i:hwin*(i+2)+1]*np.hanning(2*hwin+1))))[lowcrop:]  
-            #print(v.shape, newdataset['freq'].shape, newdataset['time'].shape)
+            # print(v.shape, newdataset['freq'].shape, newdataset['time'].shape)
             newdataset.add_data(name, v)
         return newdataset
 
 # class manufactured_DataSet(DataSet):
-
+#
 #     def __init__(self, datafunctions, Xrep='cellaverage', ndof=1, Trep='instant'):
 #         super().__init__(Xrep, ndof, Trep)
 
 
 class DataSetList(DataSetBase):
 
     _available_Xrep = ('nodal', 'cellaverage', 'spectralcell')
@@ -162,25 +164,25 @@
         if time:
             datalist['time'] = time
         self._datalist.append(datalist)
 
     def dataSet(self, datafilter=None):
         datalist = datafilter if datafilter else list(self.keys())
         datalist.remove('time')
-        dtavg, dtdev, ntot = self.dtstats() # check 'timeevol'
-        #print(dtavg, dtdev)
+        dtavg, dtdev, ntot = self.dtstats()  # check 'timeevol'
+        # print(dtavg, dtdev)
         if dtdev / dtavg > 1.e-6:
             api.io.warning(f"dt standard deviation is significant: {100*dtdev / dtavg:.4f}%")
         newdataset = DataSet(self.Xrep, self.ndof, Trep='spectrogram')
         return newdataset
 
     def _dumphdfgroup(self, hgroup: hdf5.Group, **options):
         """dump all data to an hdf group, should be used as an internal function of cfdtools, not the user
 
         Args:
             hgroup (hdf5.Group): _description_
         """
-        n = len(self._datalist)
+        # ? n = len(self._datalist)
         for i, datadict in enumerate(self._datalist):
             datagroup = hgroup.create_group(f"i{i:06}")
             for vname, var in datadict.items():
                 datagroup.create_dataset(vname, data=var, **options)
```

### Comparing `cfdtools-0.5.0/cfdtools/gmsh/_gmsh.py` & `cfdtools-0.5.1/cfdtools/gmsh/_gmsh.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Import modules
 # import collections
 # import cfdtools.meshbase._mesh as _mesh
 # import cfdtools.meshbase._connectivity as _conn
 
 # import os
 
-import cfdtools.api as api
-import numpy as np
+# import cfdtools.api as api
+# import numpy as np
 
 # from operator import itemgetter
 
 # Gmsh element types to canonical types see description below after ReaderGmsh class object
 gmshtype_elem = {
     1: "bar2",
     2: "tri3",
@@ -47,79 +47,84 @@
 #     "hex" : "hexa8"
 # }
 
 # #================================================================================================
 # #================================================================================================
 
 # From GMSH doc -
-# 1  : 2-node line.
-# 2  : 3-node triangle.
-# 3  : 4-node quadrangle.
-# 4  : 4-node tetrahedron.
-# 5  : 8-node hexahedron.
-# 6  : 6-node prism.
-# 7  : 5-node pyramid.
-# 8  : 3-node second order line (2 nodes associated with the vertices and 1 with the edge).
-# 9  : 6-node second order triangle (3 nodes associated with the vertices and 3 with the edges).
-# 10 : 9-node second order quadrangle (4 nodes associated with the vertices, 4 with the edges and 1 with the face).
-# 11 : 10-node second order tetrahedron (4 nodes associated with the vertices and 6 with the edges).
-# 12 : 27-node second order hexahedron (8 nodes associated with the vertices, 12 with the edges, 6 with the faces and 1 with the volume).
-# 13 : 18-node second order prism (6 nodes associated with the vertices, 9 with the edges and 3 with the quadrangular faces).
-# 14 : 14-node second order pyramid (5 nodes associated with the vertices, 8 with the edges and 1 with the quadrangular face).
-# 15 : 1-node point.
-# 16 : 8-node second order quadrangle (4 nodes associated with the vertices and 4 with the edges).
-# 17 : 20-node second order hexahedron (8 nodes associated with the vertices and 12 with the edges).
-# 18 : 15-node second order prism (6 nodes associated with the vertices and 9 with the edges).
-# 19 : 13-node second order pyramid (5 nodes associated with the vertices and 8 with the edges).
-# 20 : 9-node third order incomplete triangle (3 nodes associated with the vertices, 6 with the edges)
-# 21 : 10-node third order triangle (3 nodes associated with the vertices, 6 with the edges, 1 with the face)
-# 22 : 12-node fourth order incomplete triangle (3 nodes associated with the vertices, 9 with the edges)
-# 23 : 15-node fourth order triangle (3 nodes associated with the vertices, 9 with the edges, 3 with the face)
-# 24 : 15-node fifth order incomplete triangle (3 nodes associated with the vertices, 12 with the edges)
-# 25 : 21-node fifth order complete triangle (3 nodes associated with the vertices, 12 with the edges, 6 with the face)
-# 26 : 4-node third order edge (2 nodes associated with the vertices, 2 internal to the edge)
-# 27 : 5-node fourth order edge (2 nodes associated with the vertices, 3 internal to the edge)
-# 28 : 6-node fifth order edge (2 nodes associated with the vertices, 4 internal to the edge)
-# 29 : 20-node third order tetrahedron (4 nodes associated with the vertices, 12 with the edges, 4 with the faces)
-# 30 : 35-node fourth order tetrahedron (4 nodes associated with the vertices, 18 with the edges, 12 with the faces, 1 in the volume)
-# 31 : 56-node fifth order tetrahedron (4 nodes associated with the vertices, 24 with the edges, 24 with the faces, 4 in the volume)
-# 92 : 64-node third order hexahedron (8 nodes associated with the vertices, 24 with the edges, 24 with the faces, 8 in the volume)
-# 93 : 125-node fourth order hexahedron (8 nodes associated with the vertices, 36 with the edges, 54 with the faces, 27 in the volume)
+#                                                     (node associations)
+# *  1 :   2-node 1-D            line.
+# *  2 :   3-node 2-D            triangle.
+# *  3 :   4-node 2-D            quadrangle.
+# *  4 :   4-node 3-D            tetrahedron.
+# *  5 :   8-node 3-D            hexahedron.
+# *  6 :   6-node 3-D            prism.
+# *  7 :   5-node 3-D            pyramid.
+# *  8 :   3-node 1-D 2-nd order line                 (2 w/vertices,  1 w/edge).
+# *  9 :   6-node 2-D 2-nd order triangle             (3 w/vertices,  3 w/edges).
+# * 10 :   9-node 2-D 2-nd order quadrangle           (4 w/vertices,  4 w/edges,  1 w/face).
+# * 11 :  10-node 3-D 2-nd order tetrahedron          (4 w/vertices,  6 w/edges).
+# * 12 :  27-node 3-D 2-nd order hexahedron           (8 w/vertices, 12 w/edges,  6 w/faces,  1 w/volume).
+# * 13 :  18-node 3-D 2-nd order prism                (6 w/vertices,  9 w/edges,  3 w/quad faces).
+# * 14 :  14-node 3-D 2-nd order pyramid              (5 w/vertices,  8 w/edges,  1 w/quad face).
+#   15 :   1-node 0-D            point.
+# * 16 :   8-node 2-D 2-nd order quadrangle           (4 w/vertices,  4 w/edges).
+# * 17 :  20-node 3-D 2-nd order hexahedron           (8 w/vertices, 12 w/edges).
+# * 18 :  15-node 3-D 2-nd order prism                (6 w/vertices,  9 w/edges).
+# * 19 :  13-node 3-D 2-nd order pyramid              (5 w/vertices,  8 w/edges).
+# * 20 :   9-node 2-D 3-rd order incomplete triangle  (3 w/vertices,  6 w/edges)
+# * 21 :  10-node 2-D 3-rd order triangle             (3 w/vertices,  6 w/edges,  1 w/face)
+# * 22 :  12-node 2-D 4-th order incomplete triangle  (3 w/vertices,  9 w/edges)
+# * 23 :  15-node 2-D 4-th order triangle             (3 w/vertices,  9 w/edges,  3 w/face)
+#   24 :  15-node 2-D 5-th order incomplete triangle  (3 w/vertices, 12 w/edges)
+#   25 :  21-node 2-D 5-th order complete triangle    (3 w/vertices, 12 w/edges,  6 w/face)
+# * 26 :   4-node 1-D 3-rd order edge                 (2 w/vertices,  2 w/edge)
+#   27 :   5-node 1-D 4-th order edge                 (2 w/vertices,  3 w/edge)
+#   28 :   6-node 1-D 5-th order edge                 (2 w/vertices,  4 w/edge)
+#   29 :  20-node 3-D 3-rd order tetrahedron          (4 w/vertices, 12 w/edges,  4 w/faces)
+#   30 :  35-node 3-D 4-th order tetrahedron          (4 w/vertices, 18 w/edges, 12 w/faces,  1 w/volume)
+#   31 :  56-node 3-D 5-th order tetrahedron          (4 w/vertices, 24 w/edges, 24 w/faces,  4 w/volume)
+#   92 :  64-node 3-D 3-rd order hexahedron           (8 w/vertices, 24 w/edges, 24 w/faces,  8 w/volume)
+#   93 : 125-node 3-D 4-th order hexahedron           (8 w/vertices, 36 w/edges, 54 w/faces, 27 w/volume)
 
-# Line:                   Line3:           Line4:
+
+# *  1:Line:              *  8:Line3:      * 26:Line4:
 
 # 0----------1 --> u      0-----2----1     0----2----3----1
 
-# Triangle:               Triangle6:          Triangle9/10:          Triangle12/15:
+
+# *  2:Triangle:          *  9:Triangle6:      * 20/21:Triangle9/10:  * 22/23:Triangle12/15:
 
 # v
 # ^                                                                   2
 # |                                                                   | \
 # 2                       2                    2                      9   8
 # |`\                     |`\                  | \                    |     \
 # |  `\                   |  `\                7   6                 10 (14)  7
 # |    `\                 5    `4              |     \                |         \
 # |      `\               |      `\            8  (9)  5             11 (12) (13) 6
 # |        `\             |        `\          |         \            |             \
 # 0----------1 --> u      0-----3----1         0---3---4---1          0---3---4---5---1
 
-# Quadrangle:            Quadrangle8:            Quadrangle9:
+
+# *  3:Quadrangle:       * 16:Quadrangle8:       * 10:Quadrangle9:
 
 #       v
 #       ^
 #       |
 # 3-----------2          3-----6-----2           3-----6-----2
 # |     |     |          |           |           |           |
 # |     |     |          |           |           |           |
 # |     +---- | --> u    7           5           7     8     5
 # |           |          |           |           |           |
 # |           |          |           |           |           |
 # 0-----------1          0-----4-----1           0-----4-----1
 
-# Tetrahedron:                          Tetrahedron10:
+
+# *  4:Tetrahedron:                     * 11:Tetrahedron10:
 
 #                    v
 #                  .
 #                ,/
 #               /
 #            2                                     2
 #          ,/|`\                                 ,/|`\
@@ -131,30 +136,33 @@
 #  `\.         |      ,/                 `\.         |      ,/
 #     `\.      |    ,/                      `\.      |    ,9
 #        `\.   '. ,/                           `7.   '. ,/
 #           `\. |/                                `\. |/
 #              `3                                    `3
 #                 `\.
 #                    ` w
-# Hexahedron:             Hexahedron20:          Hexahedron27:
+
+
+# *  5:Hexahedron:        * 17:Hexahedron20:     * 12:Hexahedron27:
 
 #        v
 # 3----------2            3----13----2           3----13----2
 # |\     ^   |\           |\         |\          |\         |\
 # | \    |   | \          | 15       | 14        |15    24  | 14
 # |  \   |   |  \         9  \       11 \        9  \ 20    11 \
 # |   7------+---6        |   7----19+---6       |   7----19+---6
 # |   |  +-- |-- | -> u   |   |      |   |       |22 |  26  | 23|
 # 0---+---\--1   |        0---+-8----1   |       0---+-8----1   |
 #  \  |    \  \  |         \  17      \  18       \ 17    25 \  18
 #   \ |     \  \ |         10 |        12|        10 |  21    12|
 #    \|      w  \|           \|         \|          \|         \|
 #     4----------5            4----16----5           4----16----5
 
-# Prism:                      Prism15:               Prism18:
+
+# *  6:Prism:                 * 18:Prism15:          * 13:Prism18:
 
 #            w
 #            ^
 #            |
 #            3                       3                      3
 #          ,/|`\                   ,/|`\                  ,/|`\
 #        ,/  |  `\               12  |  13              12  |  13
@@ -167,15 +175,16 @@
 #    ,|      |      |\        10     |      11       10-----17-----11
 #  ,/ |      0      | `\      |      0      |        |      0      |
 # u   |    ,/ `\    |    v    |    ,/ `\    |        |    ,/ `\    |
 #     |  ,/     `\  |         |  ,6     `7  |        |  ,6     `7  |
 #     |,/         `\|         |,/         `\|        |,/         `\|
 #     1-------------2         1------9------2        1------9------2
 
-# Pyramid:                     Pyramid13:                   Pyramid14:
+
+# *  7:Pyramid:                * 19:Pyramid13:              * 14:Pyramid14:
 
 #                4                            4                            4
 #              ,/|\                         ,/|\                         ,/|\
 #            ,/ .'|\                      ,/ .'|\                      ,/ .'|\
 #          ,/   | | \                   ,/   | | \                   ,/   | | \
 #        ,/    .' | `.                ,/    .' | `.                ,/    .' | `.
 #      ,/      |  '.  \             ,7      |  12  \             ,7      |  12  \
```

### Comparing `cfdtools-0.5.0/cfdtools/gmsh/reader.py` & `cfdtools-0.5.1/cfdtools/gmsh/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 # coding: utf8
 
 # Import modules
 import collections
 import cfdtools.meshbase._mesh as _mesh
 import cfdtools.meshbase._connectivity as _conn
-import cfdtools.meshbase._elements as _ele
+import cfdtools.meshbase._elements as _elem
 from cfdtools.gmsh._gmsh import gmshtype_elem  # , nodes_per_cell
 
 # import os
 
 import cfdtools.api as api
 import numpy as np
 
 # from operator import itemgetter
 
 
 @api.fileformat_reader('GMSH', '.msh')
 class reader(api._files):
     """Implementation of the reader to read Gmsh meshes."""
 
-    @property 
+    @property
     def ncell(self):
         return self._ncell
-    
+
     def read_data(self):
-        api.io.print('std', f'> GMSH reader: starts reading {self.filename}')
+        api.io.printstd(f"> GMSH reader: starts reading {self.filename}")
         # Check file exists
         if not self.exists():
-            api.error_stop("File %s cannot be found." % (self.filename))
+            api.error_stop(f"File not found: {self.filename!r}")
 
         # Read file.
         filename = self.filename
         fam, bctype, x, y, z, elts = self.__read_sections(filename)
         # fam: dict with index: family name
         # bctype: dict with name: type
         # elts: list of list[index, element type, x, x, x, nodes index ]
-        api.io.print("std", "Analyze...", end='')
+        api.io.printstd("Analyze...", end='')
 
         # Check for 3D
-        self._maxdim = np.amax([_ele.elem_dim[gmshtype_elem[e[1]]] for e in elts])
+        self._maxdim = np.amax([_elem.elem_dim[gmshtype_elem[e[1]]] for e in elts])
 
         # Define list of element
         if self._maxdim == 3:
-            api.io.print("std", "3D mesh")
+            api.io.printstd("3D mesh")
             mesh_elt = ["tet", "hexa8", "pri", "pyr", "tet2", "hex2", "pri2", "pyr2"]
             bc_elt = ["tri3", "quad4"]
         elif self._maxdim == 2:
-            api.io.print("std", "2D mesh")
+            api.io.printstd("2D mesh")
             mesh_elt = ["tri3", "quad4"]
             bc_elt = ["bar2", "bar3"]
         else:
             api.error_stop(f"unexpected max element dimension: {self._maxdim}")
 
         # Initialize returned variables
         boundaries = {}
         connectivity = collections.OrderedDict({})
         self._nboco = 0
         bnd, bnd2fam = collections.defaultdict(list), {}
 
         # Volume Connectivity
         self._ncell = 0
-        api.io.print("std", "  extract volume connectivity")
+        api.io.printstd("  extract volume connectivity")
         bnd_connect = 1
         for elt in elts:
             if elt[1] in gmshtype_elem.keys():
                 elt_type = gmshtype_elem[elt[1]]
                 if elt_type in mesh_elt:
                     self._ncell += 1
                     if elt_type not in connectivity.keys():
                         connectivity[elt_type] = []
                     ntag = elt[2]  # expected to be 2
                     connectivity[elt_type].append(elt[3 + ntag :])
                     bnd_connect += 1
+
         # Boundary Connectivity
-        api.io.print("std", "  extract boundaries connectivity")
+        api.io.printstd("  extract boundaries connectivity")
         connect_bc = {}
         for elt in elts:
             if elt[1] in gmshtype_elem.keys():
                 elt_type = gmshtype_elem[elt[1]]
                 if elt_type in bc_elt:
                     ntag = elt[2]  # expected to be 2
                     # bnd_tag = elt[2 + tag]
@@ -93,15 +94,15 @@
                     connect_bc[bnd_tag][elt_type].append(elt[3 + ntag :])
                     # if bnd_tag not in bnd.keys():
                     #     bnd[bnd_tag] = []
                     bnd[bnd_tag].append(bnd_connect)
                     # if bnd_fam not in bnd2fam:
                     bnd2fam[bnd_tag] = bnd_fam
                     bnd_connect += 1
-        api.io.print("std", f"    tags are {bnd2fam}")
+        api.io.printstd(f"    tags are {bnd2fam}")
         # Reindex connectivities
         # Element-to-vertex
         for elt_type in connectivity.keys():
             connectivity[elt_type] = np.array(connectivity[elt_type]) - 1
         # Boundary patches element-to-vertex
         for bnd_tag in connect_bc.keys():
             for elt_type in connect_bc[bnd_tag].keys():
@@ -153,22 +154,22 @@
 
         self._elems = elts
         self._coords = (x, y, z)
         self._cellconnectivity = connectivity
         self._boundaries = boundaries
 
     def export_mesh(self):
-        api.io.print('std', f'> export gmsh mesh to cfdtools mesh data')
+        api.io.printstd("> export gmsh mesh to cfdtools mesh data")
         meshdata = _mesh.Mesh(nnode=len(self._coords[0]))
         meshdata.set_nodescoord_xyz(*self._coords)
         # meshdata.set_face2node(self.mesh['connectivity']['noofa'])
         cellconn = _conn.elem_connectivity()
         # extract cell connectivity only
         for etype, econn in self._cellconnectivity.items():
-            if _ele.elem_dim[etype] == self._maxdim:
+            if _elem.elem_dim[etype] == self._maxdim:
                 cellconn.add_elems(etype, econn)
         meshdata.set_cell2node(cellconn)
         for name, bc_dict in self._boundaries.items():
             if bc_dict['type'] == 'boundary':
                 boco = _mesh.submeshmark(name)
                 boco.geodim = 'bdnode'
                 boco.properties['type'] = bc_dict['type']
@@ -196,15 +197,15 @@
             bc = boundaries[family]
             bc["type"] = "None"
             bc["periodic_transform"] = "None"
             bc["slicing"] = bc["slicing"].tolist()
             for elt_type in connectivity.keys():
                 raveled = np.unique(connectivity[elt_type].ravel())
                 bc2["slicing"] += raveled.tolist()
-            # api.io.print('std',bc["slicing"])
+            # api.io.printstd(bc["slicing"])
             bc["slicing"] += bc2["slicing"]
             bc["slicing"] = np.unique(bc["slicing"])
             bc["type"] = "boundary"
             bc["periodic_transform"] = np.zeros((16,), dtype=np.float64)
 
         else:
             boundaries[family] = {
@@ -219,163 +220,159 @@
                 raveled = np.unique(connectivity[elt_type].ravel())
                 bc["slicing"] += raveled.tolist()
             bc["slicing"] = np.array(bc["slicing"])
             bc["type"] = "boundary"
             bc["periodic_transform"] = np.zeros((16,), dtype=np.float64)
             self._famm.append(fff)
 
+    def __get_section_from_name(self, msh, sectionName):
+
+        assert sectionName.startswith('$')
+        ibeg = msh.index(["$" + sectionName[1:]])
+        iend = msh.index(["$End" + sectionName[1:]])
+        return msh[ibeg+1:iend]
+
+    def __read_sections_V2(self, msh):
+
+        # ------------------------------------------
+        # Reading msh file for version 2.0 and below
+        # ------------------------------------------
+
+        api.io.printstd("Running version 2.0 reader")
+
+        # Find the families.
+        api.io.printstd("  parse Physical Names")
+        if ["$PhysicalNames"] in msh:
+            families = self.__get_section_from_name(msh, "$PhysicalNames")
+            fam = {}
+            bctype = {}
+            for i in range(1, int(families[0][0]) + 1):
+                fam[families[i][1]] = families[i][2][1:-1]
+                bctype[families[i][2][1:-1]] = families[i][0]
+            api.io.printstd(f"    found Physical names {fam}")
+            api.io.printstd(f"    found Entities {bctype}")
+        else:
+            fam = None
+            bctype = None
+
+        # Find the coordinates.
+        api.io.printstd("  parse Nodes")
+        coords = self.__get_section_from_name(msh, "$Nodes")
+        nnodes = int(coords[0][0])
+        x = [float(coords[i][1]) for i in range(1, nnodes + 1)]
+        y = [float(coords[i][2]) for i in range(1, nnodes + 1)]
+        z = [float(coords[i][3]) for i in range(1, nnodes + 1)]
+
+        # Find the elements.
+        api.io.printstd("  parse Elements")
+        elements = self.__get_section_from_name(msh, "$Elements")
+        elts = []
+        nelems = int(elements[0][0])
+        for i in range(1, nelems + 1):
+            elts.append([int(j) for j in elements[i]])
+
+        return fam, bctype, x, y, z, elts
+
+    def __read_sections_V4(self, msh):
+
+        # ------------------------------------------
+        # Reading msh file for version 4.0 and above
+        # ------------------------------------------
+
+        api.io.printstd("Running version 4.x reader")
+
+        # Find the families.
+        api.io.printstd("  parse Physical Names")
+        if ["$PhysicalNames"] in msh:
+            families = self.__get_section_from_name(msh, "$PhysicalNames")
+            fam = {}
+            bctype = {}
+            for i in range(1, int(families[0][0]) + 1):
+                fam[families[i][1]] = families[i][2][1:-1]
+                bctype[families[i][2][1:-1]] = families[i][0]
+            api.io.printstd(f"    found Physical names {fam}")
+            api.io.printstd(f"    found Entities {bctype}")
+        else:
+            fam = None
+            bctype = None
+
+        # To find the entity number used for concatenation of the mesh.
+        # The returned values corresponds to the physical group
+        def find_ent(j):
+            entities = self.__get_section_from_name(msh, "$Entities")
+            addd = 0  # temporary variable to seek the line and return
+            bot = int(entities[0][0]) + int(entities[0][1])
+            top = int(entities[0][2]) + bot
+            for i in range(bot, top + 1):
+                if j == int(entities[i][0]) and len(entities[i]) >= 8:
+                    addd = int(entities[i][8])
+                    break
+            return addd
+
+        # Find the coordinates.
+        api.io.printstd("  parse Nodes")
+        coords = self.__get_section_from_name(msh, "$Nodes")
+        nnodes = int(coords[0][3])
+        nodes = 1
+        count = 1
+        counter = 1
+        x = [None] * (nnodes)
+        y = [None] * (nnodes)
+        z = [None] * (nnodes)
+        while nodes < nnodes:
+            cnt = int(coords[counter][3])
+            for i in range(counter + 1, counter + cnt + 1):
+                pos = int(coords[i][0]) - 1
+                x[pos] = float(coords[i + cnt][0])
+                y[pos] = float(coords[i + cnt][1])
+                z[pos] = float(coords[i + cnt][2])
+            nodes += cnt
+            counter = counter + 2 * cnt + 1
+
+        # Find the elements.
+        api.io.printstd("  parse Elements")
+        elements = self.__get_section_from_name(msh, "$Elements")
+        # header is: numEntityBlocks, numElements, minIndex, maxIndex
+        elts = []
+        counter = 1
+        count = 1
+        neltypes = int(elements[0][0])
+        # entityblock: dimEntity EntityIndex ElemType numElements
+        # elements: ElementIndex NodesIndex
+        for i in range(0, neltypes):
+            a = int(elements[count][2])  # dimension
+            b = int(2)  # No. of tags
+            d = int(elements[count][1])  # Entity group
+            c = find_ent(d)  # Physical group
+            nxtrange = int(elements[count][3])
+            for j in range(count + 1, count + nxtrange + 1):
+                elt1 = [int(k) for k in elements[j]]
+                elt1.insert(1, a)
+                elt1.insert(2, b)
+                elt1.insert(3, c)
+                elt1.insert(4, d)
+                elts.append(elt1)
+            count += nxtrange + 1
+
+        return fam, bctype, x, y, z, elts
+
     def __read_sections(self, filename):
         # Read the entire mesh.
         msh = []
-        api.io.print('std', f"Reading file {filename!r}...", end='')
+        api.io.printstd(f"Reading file {filename!r}...", end='')
         with open(filename) as fid:
             for l in fid:
                 msh.append(l.split())
-        api.io.print('std', " done")
+        api.io.printstd(" done")
 
         # Find version of the GMSH used
-        ibeg = msh.index(["$MeshFormat"])  # To be safe, use these indicators
-        iend = msh.index(["$EndMeshFormat"])
-        version = msh[ibeg + 1 : iend]
+        version = self.__get_section_from_name(msh, "$MeshFormat")
         self.version = int(float(version[0][0]))
         assert int(version[0][1]) == 0, "only ASCII version is supported"
         assert int(version[0][2]) == 8, "size of float must be 8 (64bits)"
 
-        # -------------------------------------
-        # Reading the msh file for version 2.0
-        # -------------------------------------
-
         if self.version <= 2:
-            api.io.print('std', "Running version 2.0 reader")
-            # Find the families.
-            if ["$PhysicalNames"] in msh:
-                ibeg = msh.index(["$PhysicalNames"])
-                iend = msh.index(["$EndPhysicalNames"])
-                families = msh[ibeg + 1 : iend]
-                fam = {}
-                bctype = {}
-                for i in range(1, int(families[0][0]) + 1):
-                    fam[families[i][1]] = families[i][2][1:-1]
-                    bctype[families[i][2][1:-1]] = families[i][0]
-
-            else:
-                fam = None
-                bctype = None
-            # Find the coordinates.
-            ibeg = msh.index(["$Nodes"])
-            iend = msh.index(["$EndNodes"])
-            coordinates = msh[ibeg + 1 : iend]
-            x, y, z = [], [], []
-            for i in range(1, int(coordinates[0][0]) + 1):
-                x.append(float(coordinates[i][1]))
-                y.append(float(coordinates[i][2]))
-                z.append(float(coordinates[i][3]))
-            # api.io.print('std',x)
-            # Find the elements.
-            ibeg = msh.index(["$Elements"])
-            iend = msh.index(["$EndElements"])
-            elements = msh[ibeg + 1 : iend]
-            elts = []
-            for i in range(1, int(elements[0][0]) + 1):
-                elts.append([int(j) for j in elements[i]])
-
-            return fam, bctype, x, y, z, elts
-
-        # ---------------------------------------
-        # msh reading for version 4.0 and above
-        # ---------------------------------------
-
+            return self.__read_sections_V2(msh)
         elif self.version >= 4:
-            api.io.print('std', "Running 4.x reader")
-            # Find the families.
-            api.io.print('std', "  parse Physical Names")
-            if ["$PhysicalNames"] in msh:
-                ibeg = msh.index(["$PhysicalNames"])
-                iend = msh.index(["$EndPhysicalNames"])
-                families = msh[ibeg + 1 : iend]
-                fam = {}
-                bctype = {}
-                for i in range(1, int(families[0][0]) + 1):
-                    # fam[]
-                    fam[families[i][1]] = families[i][2][1:-1]
-                    bctype[families[i][2][1:-1]] = families[i][0]
-                api.io.print('std', f"    found Physical names {fam}")
-                api.io.print('std', f"    found Entities {bctype}")
-            else:
-                fam = None
-                bctype = None
-            # api.io.print('std',(fam, bctype))
-            # To find the entitie number used for concantination of the
-            # mesh. The returned values corresponds to the physical group
-            def find_ent(j):
-                ibeg = msh.index(["$Entities"])
-                iend = msh.index(["$EndEntities"])
-                entities = msh[ibeg + 1 : iend]
-                addd = 0  # temporary variable to seek the line and return
-                low = int(entities[0][0]) + int(entities[0][1])
-                up = int(entities[0][2]) + low
-                for i in range(low, up + 1):
-                    if j == int(entities[i][0]) and len(entities[i]) >= 8:
-                        addd = int(entities[i][8])
-                        break
-                return addd
-
-                # Find the coordinates.
-
-            api.io.print('std', "  parse Nodes")
-            ibeg = msh.index(["$Nodes"])
-            iend = msh.index(["$EndNodes"])
-            coordinates = msh[ibeg + 1 : iend]
-            counter = 1
-            maxnodes = int(coordinates[0][3])
-            nodes = 1
-            count = 1
-            x = [None] * (maxnodes)
-            y = [None] * (maxnodes)
-            z = [None] * (maxnodes)
-            while nodes < maxnodes:
-                cnt = int(coordinates[counter][3])
-                for i in range(counter + 1, counter + cnt + 1):
-                    pos = int(coordinates[i][0]) - 1
-                    x[pos] = float(coordinates[i + cnt][0])
-                    y[pos] = float(coordinates[i + cnt][1])
-                    z[pos] = float(coordinates[i + cnt][2])
-                nodes += cnt
-                counter = counter + 2 * cnt + 1
-            # Find the elements.
-            api.io.print('std', "  parse Elements")
-            ibeg = msh.index(["$Elements"])
-            iend = msh.index(["$EndElements"])
-            # header is: numEntityBlocks, numElements, minIndex, maxIndex
-            elements = msh[ibeg + 1 : iend]
-            elts = []
-            counter = 1
-            count = 1
-            # self._eltts = []
-            totcomp = int(elements[0][0])
-            # entityblock: dimEntity EntityIndex ElemType numElements
-            # elements: ElementIndex NodesIndex
-            totelm = int(elements[0][1])
-            for i in range(0, totcomp):
-                a = int(elements[count][2])  # dimension
-                b = int(2)  # No. of tags
-                d = int(elements[count][1])  # Entity group
-                c = find_ent(d)  # Physical group
-                nxtrange = int(elements[count][3])
-                for j in range(count + 1, count + nxtrange + 1):
-                    elt1 = [int(k) for k in elements[j]]
-                    # elt2=[a, b, c, d]
-                    # eltadd = elt2+elt1
-                    # elt1.insert(0,y)
-                    elt1.insert(1, a)
-                    elt1.insert(2, b)
-                    elt1.insert(3, c)
-                    elt1.insert(4, d)
-                    elts.append(elt1)
-
-                count = count + nxtrange + 1
-            # max_j = np.max([len(l) for l in elts])
-            # np_elts = np.zeros((len(elts), max_j), dtype=np.int8)
-            # elts = np.array(elts) # numpy depreciation
-            # print(elts)
-            # api.io.print('std',elts)
-            return fam, bctype, x, y, z, elts
+            return self.__read_sections_V4(msh)
+        else:
+            api.error_stop(f"unexpected mesh version: {self.version} (expected <= 2 or >= 4)")
```

### Comparing `cfdtools-0.5.0/cfdtools/hdf5/_hdf5.py` & `cfdtools-0.5.1/cfdtools/hdf5/_hdf5.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 from cfdtools import __version__
 from cfdtools.api import io, _files, error_stop
 
 try:
     import h5py
+
     import_h5py = True
 except ImportError:
     import_h5py = False
 
 
-from h5py import Group # to be available in _hdf5
+from h5py import Group  # to be available in _hdf5
 
 _available_types = ('external', 'dataset', 'datalist', 'probes', 'cfdmesh')
 
 
 def h5_str(obj):
     str = ""
     for c in map(chr, obj[:]):
         str += c
     return str
 
 
 class h5File(_files):
     def __init__(self, filename: str):
         super().__init__(filename)
+        self._openedmode = None
 
     def open(self, mode='r', datatype=None):
         try:
             self._h5file = h5py.File(self._path, mode=mode)
-        except:
+        except NameError:
             io.print('error', "h5py could not be imported")
             raise
         if mode == 'w':
             assert datatype in _available_types
             self._h5file.attrs.update({'cfdtools_version': __version__, 'cfd_datatype': datatype})
         elif mode == 'r':
             if self.exists():
                 # only for cgns file (I guess)
                 self._h5ver = self._h5file.get(' hdf5version', None)
                 self._datatype = self._h5file.attrs.get('cfd_datatype', None)
             else:
                 error_stop(f"unable to find {self.filename} (mode r)")
         else:
             error_stop("unknown mode for opening h5 file")
+        self._openedmode = mode
 
     def close(self):
         return self._h5file.close()
-    
+
     @property
     def datatype(self):
         return self._datatype
 
     def __getitem__(self, item):
         return self._h5file[item]
 
     def printinfo(self):
         super().printinfo()
-        io.printstd(h5_str(self._h5ver))
+        if self._openedmode:
+            if self._h5ver:
+                io.printstd(f"   hdf5 version: {h5_str(self._h5ver)}")
+            if self._datatype:
+                io.printstd(f"  cfdtools type: {self._datatype}")
 
 
 # if __name__ == "__main__":
 #     box = Cube(2, 1, 1)
 #     mesh = box.export_mesh()
 #     mesh.printinfo()
```

### Comparing `cfdtools-0.5.0/cfdtools/ic3/_ic3.py` & `cfdtools-0.5.1/cfdtools/ic3/_ic3.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,67 +29,31 @@
     "UGP_IO_CV_D3": 43,
     "UGP_IO_CV_D33": 44,
     "UGP_IO_CV_II1": 45,
     "UGP_IO_DATA": 50,
     "UGP_IO_EOF": 51,
 }
 
+scode, sz, ntype = 'structcode', 'size', 'numpytype'
+
 properties_ugpcode = {
-    ic3_restart_codes["UGP_IO_FA_D1"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_FA_D3"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_NO_D1"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_NO_D3"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_CV_D1"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_CV_D3"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_CV_D33"]: {
-        'structcode': "d",
-        'size': 8,
-        'numpytype': np.float64,
-    },
-    ic3_restart_codes["UGP_IO_FA_II1"]: {
-        'structcode': "q",
-        'size': 8,
-        'numpytype': np.int64,
-    },
-    ic3_restart_codes["UGP_IO_NO_II1"]: {
-        'structcode': "q",
-        'size': 8,
-        'numpytype': np.int64,
-    },
-    ic3_restart_codes["UGP_IO_CV_II1"]: {
-        'structcode': "q",
-        'size': 8,
-        'numpytype': np.int64,
-    },
+    ic3_restart_codes["UGP_IO_FA_D1"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_FA_D3"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_NO_D1"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_NO_D3"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_CV_D1"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_CV_D3"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_CV_D33"]: {scode: "d", sz: 8, ntype: np.float64},
+    ic3_restart_codes["UGP_IO_FA_II1"]: {scode: "q", sz: 8, ntype: np.int64},
+    ic3_restart_codes["UGP_IO_NO_II1"]: {scode: "q", sz: 8, ntype: np.int64},
+    ic3_restart_codes["UGP_IO_CV_II1"]: {scode: "q", sz: 8, ntype: np.int64},
 }
 
+del scode, sz, ntype
+
 # Dictionary to convert type of data [string] to a number of bytes for clean binary parsing
 type2nbytes = {
     "char": 1,
     "int32": 4,
     "int64": 8,
     "float32": 4,
     "float64": 8,
@@ -199,19 +163,18 @@
                     "mismatched record ({}) and expected ({}) sizes".format(
                         len(record), size,
                     ),
                 )
                 break
             return s.unpack(record)
     except IOError:
-        api.io.print(
-            'error',
-            "Fatal error. Could not read %d bytes from %s. Exiting." % (size, bfile.name),
+        api.error_stop(
+            f"Fatal error. Could not read {size} bytes from {bfile.name!r}."
+            " Exiting."
         )
-        exit()
 
 
 ###################################################################################################
 def BinaryWrite(bfile, endian, form, varargs):
     '''
     Method to encapsulate the few lines necessary for the translation
     of formatted components to a piece of formatted binary.
@@ -228,15 +191,17 @@
     # Actually pack the string now
     packed_ba = s.pack(*varargs)
 
     # Try to write the bytes to the file otherwise crash
     try:
         bfile.write(packed_ba)
     except IOError:
-        api.error_stop("Fatal error. Could not write to %s. Exiting." % (bfile.name))
+        api.error_stop(
+            "Fatal error. Could not write to {bfile.name!r}. Exiting."
+        )
 
 
 class restartSectionHeader:
     '''
     This class is designed to handle the header that is present
     before every variable/section/category saved into the restart file.
     '''
@@ -272,25 +237,23 @@
             + self.idata.size * type2nbytes["int64"]
             + self.rdata.size * type2nbytes["float64"]
         )
 
     def skip(self):
         return self._skip[0]  # numpy array size 1 to handle int type
 
-    def readVar(self, bfile, byte_swap, nametypes, reset_offset=True):
+    def readVar(self, bfile, byte_swap, nametypes, reset_offset=True, required=False):
         """
         Once initialization is done, this method actually reads
         the header data from the packed binary formatted string.
         """
-        id_list = []
-        for nametype in nametypes:
-            id_list.append(ic3_restart_codes[nametype])
+        id_list = [ic3_restart_codes[nametype] for nametype in nametypes]
         if reset_offset:
             bfile.seek(8, os.SEEK_SET)
-        while (self.id[0] not in id_list) and (self.id[0] != ic3_restart_codes["UGP_IO_EOF"]):
+        while True:
             self.name = ""
             self.id = np.zeros((1,), dtype=np.int32)
             self.idata = np.zeros((8,), dtype=np.int64)
             self.rdata = np.zeros((16,), dtype=np.float64)
 
             api.io.print('debug', "skipping data %d" % self.skip())
             if self.skip() > 0:
@@ -316,16 +279,31 @@
             self._skip[0] = s[nlen + self.id.size]  # store size in skip for next read
             ibeg = nlen + self.id.size + self._skip.size
             iend = ibeg + self.idata.size
             self.idata = s[ibeg:iend]
             ibeg = iend
             iend = ibeg + self.rdata.size
             self.rdata = s[ibeg:iend]
+            if self.id[0] in id_list:
+                return True
+            if self.id[0] == ic3_restart_codes["UGP_IO_EOF"]:
+                break
+        if required:
+            api.error_stop(
+                f"Fatal error."
+                f" Section(s) {nametypes} not found in dataset {self.name}."
+                f" Exiting."
+            )
+        return False
 
-        return self.id[0] in id_list
+    def readReqVar(self, *args, **kwargs):
+        """
+        error_stop if required data is not found.
+        """
+        return self.readVar(*args, **kwargs, required=True)
 
     def write(self, bfile, endian):
         """
         Once initialization is done, this method actually writes
         the header data from the packed binary formatted string.
         """
 
@@ -342,24 +320,36 @@
             varargs.append(self.idata[kk])
         for kk in range(16):
             varargs.append(self.rdata[kk])
         # Now write everything at once
         BinaryWrite(bfile, endian, self.binstr, varargs)
 
     def __str__(self):
-        mystring = "> Header: \n"
-        mystring += "Name : %s\n" % self.name
-
-        mystring += "Id   : %i %s\n" % (
+        mystring = "> Header:"
+        mystring += "\n"
+        mystring += "Name : %s" % self.name
+        mystring += "\n"
+        mystring += "Id   : %i %s" % (
             self.id,
-            list(dict(filter(lambda items: items[1] == self.id[0], ic3_restart_codes.items())).keys()),
+            list(
+                dict(
+                    filter(
+                        lambda items: items[1] == self.id[0],
+                        ic3_restart_codes.items()
+                    )
+                ).keys()
+            ),
         )
-        mystring += "hsize: %i\n" % self.hsize
-        mystring += "skip : %i\n" % self.skip()
-        mystring += "idata: (" + ", ".join(str(i) for i in self.idata) + ")\n"
+        mystring += "\n"
+        mystring += "hsize: %i" % self.hsize
+        mystring += "\n"
+        mystring += "skip : %i" % self.skip()
+        mystring += "\n"
+        mystring += "idata: (" + ", ".join(str(i) for i in self.idata) + ")"
+        mystring += "\n"
         mystring += "rdata: (" + ", ".join(str(r) for r in self.rdata) + ")"
         return mystring
 
 
 class binreader(api._files):
     '''Implementation of the reader to read IC3 restart files.'''
 
@@ -371,18 +361,18 @@
     #               whether to check the integrity of the file beforehand [type boolean]
     #     '''
     #     super().__init__(filename)
     #     self.check_integrity = cIntegrity
     #     self.ic3_version = -1
 
     def read_headers(self):
-        '''
+        """
         Main method of the IC3 restart reader.
         Parses in order the file using sub-methods described below.
-        '''
+        """
         api.io.print('std', "READER RESTART IC3 - only headers")
 
         if not self.exists():
             print("Fatal error. File %s cannot be found." % (self.filename))
             exit()
 
         # Open the file for binary reading
@@ -437,9 +427,10 @@
             aux_struct = struct.Struct("<i")
             s[1] = aux_struct.unpack(packed_version)[0]
 
         # Some info for the user
         self.ic3_version = s[1]
         api.io.print(
             'std',
-            f"  version: {self.ic3_version} " + ("little-endian" if self.byte_swap else "big-endian"),
+            f"  version: {self.ic3_version} "
+            + ("little-endian" if self.byte_swap else "big-endian"),
         )
```

### Comparing `cfdtools-0.5.0/cfdtools/ic3/reader_legacy.py` & `cfdtools-0.5.1/cfdtools/ic3/reader_legacy.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # Import modules
 # import struct
 import numpy as np
 import sys
 import cfdtools.api as api
 import cfdtools.meshbase._mesh as _mesh
 import cfdtools.data as _data
-import cfdtools.meshbase._connectivity as conn
+import cfdtools.meshbase._connectivity as _conn
 
-# import cfdtools.ic3._ic3 as ic3b
 from cfdtools.ic3._ic3 import (
     binreader,
     type2nbytes,
     restartSectionHeader,
     ic3_restart_codes,
     BinaryRead,
     zonekind2type,
@@ -102,50 +101,56 @@
         '''
         Main method of the IC3 restart reader.
         Parses in order the file using sub-methods described below.
         output: the mesh itself
                 a lot of variables stored in the restart file
                 information on the state of the simulation
         '''
-        api.io.print('std', "READER RESTART IC3")
+        api.io.printstd("READER RESTART IC3")
 
         if not self.exists():  # pragma: no cover
             api.error_stop("Fatal error. File %s cannot be found." % (self.filename))
 
         # Open the file for binary reading
         api.io.print('debug', f"Opening file {self.filename!r}")
         with open(self.filename, "rb") as self.fid:
             #
-            api.io.print('std', "Reading binary file header")
+            api.io.printstd("Reading binary file header")
             self._ReadRestartHeader()
             #
-            api.io.print('std', "Reading connectivity...")
+            api.io.printstd("Reading connectivity...")
             self._ReadRestartConnectivity()
             #
-            api.io.print('std', "Reading informative values...")
+            api.io.printstd("Reading informative values...")
             self._ReadInformativeValues()
             #
-            api.io.print('std', "Reading variables...")
+            api.io.printstd("Reading variables...")
             self.celldata = _data.DataSet('cellaverage')
             self.nodedata = _data.DataSet('nodal')
             self.facedata = _data.DataSet('nodal')
             self._ReadRestartVar()
             #
             self._ncell = self.mesh['params']['cv_count']  # for generic writer and timer
 
         # file identifier as shortcut only
         del self.fid
 
     def export_mesh(self):
-        # return self.mesh["coordinates"], self.mesh["connectivity"]["e2v"], self.mesh["bocos"], self.variables["nodes"], self.variables["cells"], (self.simulation_state, self.mesh["params"])
-        meshdata = _mesh.Mesh(self.mesh['params']['cv_count'], self.mesh['params']['no_count'])
+        # return (
+        #     self.mesh["coordinates"],
+        #     self.mesh["connectivity"]["e2v"],
+        #     self.mesh["bocos"],
+        #     self.variables["nodes"],
+        #     self.variables["cells"],
+        #     (self.simulation_state, self.mesh["params"]),
+        # )
         meshdata = _mesh.Mesh(self.mesh['params']['cv_count'], self.mesh['params']['no_count'])
         meshdata.set_nodescoord_nd(self.mesh['coordinates'])
-        face2cell = conn.indexindirection(self.mesh['connectivity']['cvofa']['cvofa'])
-        face2node = conn.elem_connectivity()
+        face2cell = _conn.indexindirection(self.mesh['connectivity']['cvofa']['cvofa'])
+        face2node = _conn.elem_connectivity()
         face2node.importfrom_compressedindex(self.mesh['connectivity']['noofa'])
         meshdata.add_faces('mixed', face2node, face2cell)
         for boco in self.mesh['bocos']:
             meshdata.add_boco(boco)
         meshdata.set_celldata(self.celldata)
         meshdata.set_nodedata(self.nodedata)
         meshdata.set_facedata(self.facedata)
@@ -159,136 +164,155 @@
         '''
         Method reading the first blocks passed the header, containing informations
         on the nodes, the faces, the cells and the connectivity in between those
         input:  handle on an open restart file [type file identifier]
                 endianness flag [boolean]
         output: mesh structure containing all the necessary information to build the grid
         '''
+
         # Initialize the mesh
         self.mesh = {
-            "params": {"no_count": 0, "fa_count": 0, "cv_count": 0, "noofa_count": 0, "nboco": 0},
+            "params": {
+                "no_count": 0,
+                "fa_count": 0,
+                "cv_count": 0,
+                "noofa_count": 0,
+                "nboco": 0,
+            },
             "connectivity": {"noofa": {}, "cvofa": {}, "nkeys": 0},
             "coordinates": None,
             "bocos": {"nfa_b": 0, "nfa_bp": 0},
             "partition": None,
         }
 
         # Get the header
         h = restartSectionHeader()
-        if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_NO_FA_CV_NOOFA_COUNTS"]):
-            exit()
+        h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_NO_FA_CV_NOOFA_COUNTS"])
         # Store the size informations at the right place
         # and set the local shortcut names
         # number of nodes/vertices
         no_count = self.mesh["params"]["no_count"] = h.idata[0]
         # number of faces
         fa_count = self.mesh["params"]["fa_count"] = h.idata[1]
         # number of cells/volume elements
         cv_count = self.mesh["params"]["cv_count"] = h.idata[2]
         # number of nodes from faces
         noofa_count = self.mesh["params"]["noofa_count"] = h.idata[3]
-        api.io.printstd("mesh with {} cells, {} faces and {} nodes".format(h.idata[2], h.idata[1], h.idata[0]))
-        #
+        api.io.printstd(
+            f"mesh with {cv_count} cells, {fa_count} faces and {no_count} nodes",
+        )
         # Integrity check
         if self.check_integrity:
             # Check the restart is whole by counting the global ids of no, fa and cv
             # For nodes
             api.io.printstd("  Checking nodes integrity ..")
             sys.stdout.flush()
             h = restartSectionHeader()
             if h.readVar(self.fid, self.byte_swap, ["UGP_IO_NO_CHECK"]):
                 assert h.idata[0] == no_count
                 assert h.id[0] == ic3_restart_codes["UGP_IO_NO_CHECK"]
-                s = BinaryRead(self.fid, "%di" % no_count, self.byte_swap, type2nbytes["int32"] * no_count)
+                s = BinaryRead(
+                        self.fid, "%di" % no_count, self.byte_swap,
+                        type2nbytes["int32"] * no_count
+                    )
                 nodes_id = np.asarray(s)
                 assert np.allclose(nodes_id, np.arange(no_count))
-                api.io.print('std', "end of node integrity")
+                api.io.printstd("end of node integrity")
                 sys.stdout.flush()
                 del nodes_id
                 # For faces
-                api.io.print('std', "  Checking faces integrity ..")
+                api.io.printstd("  Checking faces integrity ..")
                 sys.stdout.flush()
                 h = restartSectionHeader()
-                if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_FA_CHECK"]):
-                    exit()
-                s = BinaryRead(self.fid, "%di" % fa_count, self.byte_swap, type2nbytes["int32"] * fa_count)
+                h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_FA_CHECK"])
+                s = BinaryRead(
+                        self.fid, "%di" % fa_count, self.byte_swap,
+                        type2nbytes["int32"] * fa_count
+                    )
                 faces_id = np.asarray(s)
                 assert np.allclose(faces_id, np.arange(fa_count))
-                api.io.print('std', "end of face integrity")
+                api.io.printstd("end of face integrity")
                 sys.stdout.flush()
                 del faces_id
                 # For cells
-                api.io.print('std', "  Checking cells integrity ..")
+                api.io.printstd("  Checking cells integrity ..")
                 sys.stdout.flush()
                 h = restartSectionHeader()
-                if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_CV_CHECK"]):
-                    exit()
+                h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_CV_CHECK"])
                 assert h.idata[0] == cv_count
                 assert h.id[0] == ic3_restart_codes["UGP_IO_CV_CHECK"]
-                cells_id = np.empty((cv_count,), dtype=np.int32)
-                s = BinaryRead(self.fid, "%di" % cv_count, self.byte_swap, type2nbytes["int32"] * cv_count)
+                s = BinaryRead(
+                        self.fid, "%di" % cv_count, self.byte_swap,
+                        type2nbytes["int32"] * cv_count
+                    )
                 cells_id = np.asarray(s)
                 assert np.allclose(cells_id, np.arange(cv_count))
-                api.io.print('std', "end of cell integrity")
+                api.io.printstd("end of cell integrity")
                 sys.stdout.flush()
                 del cells_id
             else:
                 api.io.warning("check integrity: no check, UGP_IO_NO_CHECK missing")
 
         # The two connectivities now
         #
         # - First, NOOFA
         #
-        api.io.print('std', "  Parsing face to node connectivity...")
+        api.io.printstd("  Parsing face to node connectivity...")
         sys.stdout.flush()
         h = restartSectionHeader()
-        if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_NOOFA_I_AND_V"]):
-            exit()
+        h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_NOOFA_I_AND_V"])
         assert h.idata[0] == fa_count
         assert h.idata[1] == noofa_count
 
         # Get the node count per face
-        s = BinaryRead(self.fid, "%di" % fa_count, self.byte_swap, type2nbytes["int32"] * fa_count)
+        s = BinaryRead(
+                self.fid, "%di" % fa_count, self.byte_swap,
+                type2nbytes["int32"] * fa_count
+            )
         nno_per_face = np.asarray(s)
         uniq, counts = np.unique(nno_per_face, return_counts=True)
         for facesize, nfacesize in zip(uniq, counts):
-            api.io.print('std', f"  {nfacesize} faces of {facesize} nodes")
+            api.io.printstd(f"  {nfacesize} faces of {facesize} nodes")
         # Initialize the proper connectivity arrays in self.mesh
         face2node_index = np.concatenate(([0], np.cumsum(nno_per_face)))
         # np.sum(nno_per_face) == noofa_count
         assert face2node_index[0] == 0
         assert face2node_index[-2] == noofa_count - nno_per_face[-1]
         # Now loop on the restart file to fill the connectivities
-        s = BinaryRead(self.fid, "%di" % noofa_count, self.byte_swap, type2nbytes["int32"] * noofa_count)
+        s = BinaryRead(
+                self.fid, "%di" % noofa_count, self.byte_swap,
+                type2nbytes["int32"] * noofa_count
+            )
         # store in 8 bytes
         face2node_value = np.asarray(s).astype(np.int64)
-        zface2node = conn.compressed_listofindex(face2node_index, face2node_value)
+        zface2node = _conn.compressed_listofindex(face2node_index, face2node_value)
         zface2node.check()
         self.mesh["connectivity"]["noofa"] = zface2node
-        api.io.print('std', "end of face/vertex connectivity")
+        api.io.printstd("end of face/vertex connectivity")
         sys.stdout.flush()
         del nno_per_face, uniq, counts
         #
         # - Second, CVOFA
         #
-        api.io.print('std', "  Parsing face to cell connectivity...")
+        api.io.printstd("  Parsing face to cell connectivity...")
         sys.stdout.flush()
         h = restartSectionHeader()
-        if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_CVOFA"]):
-            exit()
+        h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_CVOFA"])
 
         assert h.idata[0] == fa_count
         assert h.idata[1] == 2
-        # Initialize the proper connectivity arrays in self.mesh
-        # Now loop on the restart file to fill the connectivities
-        s = BinaryRead(self.fid, "%di" % (fa_count * 2), self.byte_swap, type2nbytes["int32"] * fa_count * 2)
+        # Fill the connectivities
+        s = BinaryRead(
+                self.fid, "%di" % (fa_count * 2), self.byte_swap,
+                type2nbytes["int32"] * fa_count * 2
+            )
         # store in 8 bytes
         self.mesh["connectivity"]["cvofa"]["cvofa"] = np.asarray(s).astype(np.int64).reshape((fa_count, 2))
 
-        api.io.print('std', "end of face/cell connectivity")
+        api.io.printstd("end of face/cell connectivity")
         sys.stdout.flush()
 
         # Checks and a few associations
         assert self.mesh["connectivity"]["cvofa"]["cvofa"].max() < cv_count
         assert self.mesh["connectivity"]["cvofa"]["cvofa"].max() == cv_count - 1
         uniq, counts = np.unique(self.mesh["connectivity"]["cvofa"]["cvofa"][:, 1], return_counts=True)
         # Number of assigned boundary faces
@@ -305,84 +329,87 @@
         )
         # All periodic boundary faces to -1
         # mask = self.mesh["connectivity"]["cvofa"]["cvofa"][:,1] < -1
         # self.mesh["connectivity"]["cvofa"]["cvofa"][:,1][mask] = -1
         # print("RC",self.mesh["connectivity"]["cvofa"]["cvofa"])
         #
         # The boundary conditions now
-        api.io.print('std', "  Parsing boundary conditions...")
+        api.io.printstd("  Parsing boundary conditions...")
         sys.stdout.flush()
         self.mesh['bocos'] = []  # init list of bocos
         while True:
             h = restartSectionHeader()
             if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_FA_ZONE"], reset_offset=False):
                 break
             # UGP_IO_FA_ZONE header
             # 3 ints: kind, face range (begin, start)
             self.mesh["params"]["nboco"] += 1
             boco = _mesh.submeshmark(h.name)
             boco.type = zonekind2type[h.idata[0]]
             boco.geodim = 'intface' if boco.type == 'internal' else 'bdface'
-            boco.index = conn.indexlist(irange=[h.idata[1], h.idata[2]])
+            boco.index = _conn.indexlist(irange=[h.idata[1], h.idata[2]])
             boco.properties["periodic_transform"] = h.rdata
             #
             famin, famax = boco.index.range()
             sta = face2node_index[famin]
             try:
                 sto = face2node_index[famax + 1]
             except IndexError:
                 sto = face2node_value.size
             #
             boco.properties["slicing"] = np.unique(face2node_value[sta:sto])
             self.mesh['bocos'].append(boco)
             if h.idata[0] == 6:
                 break
-        api.io.print('std', "end of boundary conditions")
+        api.io.printstd("end of boundary conditions")
         sys.stdout.flush()
 
         # Parse the header of the partition information
-        api.io.print('std', "  Parsing partitioning information...")
+        api.io.printstd("  Parsing partitioning information...")
         sys.stdout.flush()
         h = restartSectionHeader()
-        if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_CV_PART"]):
-            exit()
+        h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_CV_PART"])
 
         self.mesh["partition"] = {}
         self.mesh["partition"]['npart'] = h.idata[1]
         self.mesh["partition"]['icvpart'] = np.zeros((cv_count,), dtype=np.int32)
-        s = BinaryRead(self.fid, "%di" % cv_count, self.byte_swap, type2nbytes["int32"] * cv_count)
+        s = BinaryRead(
+                self.fid, "%di" % cv_count, self.byte_swap,
+                type2nbytes["int32"] * cv_count
+            )
         self.mesh["partition"]['icvpart'] = np.asarray(s)
-        api.io.print('std', "end of partition")
+        api.io.printstd("end of partition")
         sys.stdout.flush()
 
         # The coordinates of the vertices finally
-        api.io.print('std', "  Parsing vertices coordinates...")
+        api.io.printstd("  Parsing vertices coordinates...")
         sys.stdout.flush()
         h = restartSectionHeader()
-        if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_X_NO"]):
-            exit()
+        h.readReqVar(self.fid, self.byte_swap, ["UGP_IO_X_NO"])
 
         assert h.idata[0] == no_count
         assert h.idata[1] == 3
         s = BinaryRead(
-            self.fid, "%dd" % (no_count * 3), self.byte_swap, type2nbytes["float64"] * no_count * 3
-        )
+                self.fid, "%dd" % (no_count * 3), self.byte_swap,
+                type2nbytes["float64"] * no_count * 3
+            )
         self.mesh["coordinates"] = np.ascontiguousarray(np.asarray(s).reshape(no_count, 3))
-        api.io.print('std', "end of node coordinates")
+        api.io.printstd("end of node coordinates")
         sys.stdout.flush()
 
     def _ReadInformativeValues(self):
         '''
         Method reading all the values also stored in a restart file,
         i.e. the step number, the time, the timestep.
         input:  handle on an open restart file, [type file identifier]
                 endianness flag [boolean]
         output: simulation state structure containing informations about the current state
                 of the simulation
         '''
+
         # Initialize the state dictionary
         self.simulation_state = {"step": 0, "dt": 0, "time": 0, "wgt": {}}
 
         # First, a header saying data to introduce to this block we are parsing now
 
         # removed as not used at the moment
         # h = restartSectionHeader()
@@ -410,18 +437,20 @@
         ndof = 1
         if self.ic3_version < 0:
             raise ValueError("unknown IC3 version number")
         elif self.ic3_version < 3:
             pass
             # ignore ints
             # if intndof != 0: # 0 is expected value for version 1 and 2
-            #     api.io.print("warning", "unexpected non zero value for ndof in IC3 version 1 and 2")
+            #     api.io.print('warning', "unexpected non zero value for ndof in IC3 version 1 and 2")
         else:  # version >= 3
             if intndof == 0:  # 0 is NOT expected
-                api.io.warning("unexpected zero value for ndof in IC3 version 3; set to 1 !")
+                api.io.warning(
+                    "unexpected zero value for ndof in IC3 version 3; set to 1 !",
+                )
                 ndof = 1
             else:
                 ndof = intndof
         # if self.get_datacell_properties().get("ndof", ndof) != ndof:
         #     raise ValueError("Inconsistent cell data size (ndof)")
         # self.get_datacell_properties()["ndof"] = ndof
         return ndof
@@ -442,21 +471,20 @@
         self.variables = {"nodes": {}, "cells": {}, "faces": {}}
         # set the local shortcut names
         no_count = self.mesh["params"]["no_count"]
         fa_count = self.mesh["params"]["fa_count"]
         cv_count = self.mesh["params"]["cv_count"]
 
         # First come the scalars
-        api.io.print('std', "  First the scalars...")
+        api.io.printstd("  First the scalars...")
         reset_offset = True
         while True:
             h = restartSectionHeader()
             if not h.readVar(
-                self.fid,
-                self.byte_swap,
+                self.fid, self.byte_swap,
                 [
                     "UGP_IO_NO_D1",
                     "UGP_IO_NO_II1",
                     "UGP_IO_FA_D1",
                     "UGP_IO_CV_D1",
                     "UGP_IO_CV_II1",
                 ],
@@ -466,140 +494,136 @@
             reset_offset = False
             #
             typechar = properties_ugpcode[h.id[0]]['structcode']
             typesize = properties_ugpcode[h.id[0]]['size']
             nptype = properties_ugpcode[h.id[0]]['numpytype']
             #
             if h.idata[0] == no_count:
-                s = BinaryRead(self.fid, "%d" % no_count + typechar, self.byte_swap, typesize * no_count)
-                var = self.variables["nodes"][h.name] = np.asarray(s).astype(nptype)
-
+                s = BinaryRead(
+                        self.fid, "%d" % no_count + typechar, self.byte_swap,
+                        typesize * no_count
+                    )
+                scalar = self.variables["nodes"][h.name] = np.asarray(s).astype(nptype)
             elif h.idata[0] == fa_count:
-                s = BinaryRead(self.fid, "%d" % fa_count + typechar, self.byte_swap, typesize * fa_count)
-                var = self.variables["faces"][h.name] = np.asarray(s).astype(nptype)
-
+                s = BinaryRead(
+                        self.fid, "%d" % fa_count + typechar, self.byte_swap,
+                        typesize * fa_count
+                    )
+                scalar = self.variables["faces"][h.name] = np.asarray(s).astype(nptype)
             elif h.idata[0] == cv_count:
-                api.io.print(
-                    "internal",
-                    "cell variable section of size number of cells * ndofs {}x{}".format(
-                        h.idata[0], h.idata[1]
-                    ),
-                )
                 ndof = self._set_ndof_properties(h.idata[1])
                 if ndof > 1:
                     self.celldata.Xrep = 'spectralcell'
                     self.celldata.ndof = ndof
-                s = BinaryRead(
-                    self.fid, "%d" % (ndof * cv_count) + typechar, self.byte_swap, typesize * ndof * cv_count
+                api.io.print(
+                    'internal',
+                    "cell variable section of size ncells * ndofs"
+                    " {}x{}".format(cv_count, ndof),
                 )
-                var = np.asarray(s).astype(nptype)
-
-                # If multiple connectivities, gotta order the tables correctly
+                s = BinaryRead(
+                        self.fid, "%d" % (ndof * cv_count) + typechar, self.byte_swap,
+                        typesize * ndof * cv_count
+                    )
+                scalar = np.asarray(s).astype(nptype)
+                # If multiple connectivities, order the tables correctly
                 if self.mesh["connectivity"]["nkeys"] > 1:
-                    aux = copy.deepcopy(var)
-                    var = np.empty((0,), dtype=aux.dtype)
+                    aux = copy.deepcopy(scalar)
+                    scalar = np.empty((0,), dtype=aux.dtype)
                     for uns_type, indices in self.mesh["connectivity"]["cell_indices"].items():
-                        var = np.concatenate((var, aux[indices]))
-                self.celldata.add_data(h.name, var)
+                        scalar = np.concatenate((scalar, aux[indices]))
+                self.celldata.add_data(h.name, scalar)
             else:
                 api.error_stop(f"Fatal error. Incoherence in dataset {h.name}. Exiting.")
-
-            print_stats_scalar(h.name, var)
-
-        api.io.print('std', "  end of scalars")
+            print_stats_scalar(h.name, scalar)
+        api.io.printstd("  end of scalars")
 
         # Then the vectors
-        api.io.print('std', "  Then the vectors...")
+        api.io.printstd("  Then the vectors...")
         reset_offset = True
         while True:
             h = restartSectionHeader()
             if not h.readVar(
-                self.fid,
-                self.byte_swap,
-                ["UGP_IO_NO_D3", "UGP_IO_FA_D3", "UGP_IO_CV_D3"],
+                self.fid, self.byte_swap,
+                [
+                    "UGP_IO_NO_D3",
+                    "UGP_IO_FA_D3",
+                    "UGP_IO_CV_D3",
+                ],
                 reset_offset=reset_offset,
             ):
                 break
             reset_offset = False
-
+            #
             if h.idata[0] == no_count:
                 s = BinaryRead(
-                    self.fid, "%dd" % (no_count * 3), self.byte_swap, type2nbytes["float64"] * no_count * 3
-                )
+                        self.fid, "%dd" % (no_count * 3), self.byte_swap,
+                        type2nbytes["float64"] * no_count * 3
+                    )
                 vector = self.variables["nodes"][h.name] = np.asarray(s).reshape((no_count, 3))
-
-            elif h.idata[0] == self.mesh["params"]["fa_count"]:
+            elif h.idata[0] == fa_count:
                 self.variables["faces"][h.name] = np.zeros(
-                    (self.mesh["params"]["fa_count"], 3), dtype=np.float64
+                    (fa_count, 3), dtype=np.float64
                 )
                 s = BinaryRead(
-                    self.fid, "%dd" % (fa_count * 3), self.byte_swap, type2nbytes["float64"] * fa_count * 3
-                )
+                        self.fid, "%dd" % (fa_count * 3), self.byte_swap,
+                        type2nbytes["float64"] * fa_count * 3
+                    )
                 vector = self.variables["faces"][h.name] = np.asarray(s).reshape((fa_count, 3))
-
             elif h.idata[0] == cv_count:
                 ndof = self._set_ndof_properties(h.idata[1])
                 if ndof > 1:
                     self.celldata.Xrep = 'spectralcell'
                     self.celldata.ndof = ndof
                 s = BinaryRead(
-                    self.fid,
-                    "%dd" % (ndof * cv_count * 3),
-                    self.byte_swap,
-                    type2nbytes["float64"] * ndof * cv_count * 3,
-                )
+                        self.fid, "%dd" % (ndof * cv_count * 3), self.byte_swap,
+                        type2nbytes["float64"] * ndof * cv_count * 3,
+                    )
                 vector = np.asarray(s).reshape((ndof * cv_count, 3))
                 # If multiple connectivities, gotta order the tables correctly
                 if self.mesh["connectivity"]["nkeys"] > 1:
                     aux = copy.deepcopy(vector)
                     vector = np.empty((0, 3), dtype=aux.dtype)
                     for indices in self.mesh["connectivity"]["cell_indices"].values():
                         vector = np.concatenate((vector, aux[indices, :]), axis=0)
                 self.celldata.add_data(h.name, vector)
             else:
-                api.io.print('std', "Fatal error. Incoherence in dataset %s. Exiting." % (h.name))
-                exit()
-
+                api.error_stop(f"Fatal error. Incoherence in dataset {h.name}. Exiting.")
             print_stats_vector(h.name, vector)
-
-        api.io.print('std', "  end of vectors")
+        api.io.printstd("  end of vectors")
 
         # Then the tensors
-        api.io.print('std', "  Then the tensors...")
+        api.io.printstd("  Then the tensors...")
         reset_offset = True
         while True:
             h = restartSectionHeader()
             if not h.readVar(self.fid, self.byte_swap, ["UGP_IO_CV_D33"], reset_offset=reset_offset):
                 break
             reset_offset = False
 
             if h.idata[0] == cv_count:
                 ndof = self._set_ndof_properties(h.idata[1])
                 if ndof > 1:
                     self.celldata.Xrep = 'spectralcell'
                     self.celldata.ndof = ndof
                 s = BinaryRead(
-                    self.fid,
-                    "%dd" % (ndof * cv_count * 3 * 3),
-                    self.byte_swap,
-                    type2nbytes["float64"] * ndof * cv_count * 3 * 3,
-                )
-                pdata = np.asarray(s).reshape((ndof * cv_count, 3, 3))
+                        self.fid, "%dd" % (ndof * cv_count * 3 * 3), self.byte_swap,
+                        type2nbytes["float64"] * ndof * cv_count * 3 * 3,
+                    )
+                tensor = np.asarray(s).reshape((ndof * cv_count, 3, 3))
                 # If multiple connectivities, gotta order the tables correctly
                 if self.mesh["connectivity"]["nkeys"] > 1:
-                    aux = copy.deepcopy(pdata)
-                    pdata = np.empty((0, 3, 3), dtype=aux.dtype)
-                    for uns_type, indices in self.mesh["connectivity"]["cell_indices"].items():
-                        pdata = np.concatenate((pdata, aux[indices, :, :]), axis=0)
-                self.celldata.add_data(h.name, pdata)
-                print_stats_scalar(h.name, pdata)
+                    aux = copy.deepcopy(tensor)
+                    tensor = np.empty((0, 3, 3), dtype=aux.dtype)
+                    for indices in self.mesh["connectivity"]["cell_indices"].values():
+                        tensor = np.concatenate((tensor, aux[indices, :, :]), axis=0)
+                self.celldata.add_data(h.name, tensor)
+                print_stats_scalar(h.name, tensor)
             else:
-                api.io.print('std', "Fatal error. Incoherence in dataset %s. Exiting." % (h.name))
-                exit()
-        api.io.print('std', "  end of tensors")
+                api.error_stop(f"Fatal error. Incoherence in dataset {h.name}. Exiting.")
+        api.io.printstd("  end of tensors")
 
     # def __reachedEOF(self):
     #     '''
     #     Method to check whether the reader reached EOF.
     #     It should happen right after reading all the variable blocks.
     #     input   : handle on an open restart file, [type file identifier]
     #               endianness flag [boolean]
```

### Comparing `cfdtools-0.5.0/cfdtools/ic3/writerV2.py` & `cfdtools-0.5.1/cfdtools/ic3/writerV2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # Import modules
 import numpy as np
 import cfdtools.api as api
 
-# import cfdtools.meshbase._mesh as _mesh
-from cfdtools.ic3._ic3 import ic3_restart_codes, struct_endian, BinaryWrite, restartSectionHeader, type2nbytes, type2zonekind
+from cfdtools.ic3._ic3 import (
+    ic3_restart_codes,
+    type2nbytes,
+    type2zonekind,
+    struct_endian,
+    BinaryWrite,
+    restartSectionHeader,
+)
 
 ###################################################################################################
 
 
 @api.fileformat_writer('IC3', '.ic3')
 class writer:
     '''Implementation of the writer to write ic3 restart files'''
 
     __version__ = "2"
 
     def __init__(self, mesh, endian='native'):
         """
         Initialization of a ic3 restart file writer.
         """
-        api.io.print('std', "> Initialization of IC3 writer V" + self.__version__)
+        api.io.printstd("> Initialization of IC3 writer V" + self.__version__)
         if not endian in struct_endian.keys():
             raise ValueError("unknown endian key")
         else:
             self.endian = endian
-        #self.vars = {"nodes": {}, "cells": {}}
+        # self.vars = {"nodes": {}, "cells": {}}
         self._mesh = mesh
         self.params = {}
         # Initialize the simulation state
         self.set_simstate()
         self.set_mesh()
         self.set_bocos()
         self.set_vars()
@@ -36,15 +42,15 @@
         """
         Store the coordinates of the nodes and the
         element-to-vertex connectivity. Also triggers the creation
         of a face-to-element and face-to-vertex connectivity
         as per CharlesX implementation.
         """
         timer = api.Timer()
-        api.io.print('std', "> Check connectivity and compute mandatory")
+        api.io.printstd("> Check connectivity and compute mandatory")
         if not self._mesh._faces:  # empty dict of faces
             with api.Timer(task="  generate all faces"):
                 self._mesh.make_face_connectivity()
         if any([boco.nodebased() for _, boco in self._mesh._bocos.items()]):
             with api.Timer(task="  change boco marks (node to face)"):
                 self._mesh.bocomarks_set_node_to_face()
         if 'boundary' in self._mesh._faces.keys():
@@ -53,15 +59,15 @@
         # self._mesh.printinfo()
         if any([boco.index.type == 'list' for _, boco in self._mesh._bocos.items()]):
             with api.Timer(
                 task="  reindex boundary faces with boco marks and compress"
             ):
                 self._mesh.reindex_boundaryfaces()
 
-        api.io.print('std', "Setting coordinates and connectivity arrays..")
+        api.io.printstd("Setting coordinates and connectivity arrays..")
 
         # Nodes
         self.coordinates = np.stack(
             [self._mesh._nodes[c] for c in 'xyz'], axis=1
         )
 
         # Compute the number of nodes and elements
@@ -106,15 +112,15 @@
     def set_bocos(self, nboco=None):
         """
         Set the boundary conditions dictionary for the restart.
         It will be later written to the file using the
         __WriteRestartConnectivity method.
         The bocos slicing is expressed in terms of faces.
         """
-        api.io.print('std', "Setting boundary conditions...")
+        api.io.printstd("Setting boundary conditions...")
         self.bocos = {
             key: boco
             for key, boco in self._mesh._bocos.items()
             if not boco.type == 'internal'
         }
         # self.bocos.pop("nfa_b")
         # self.bocos.pop("nfa_bp")
@@ -141,52 +147,52 @@
         Set the variables for the restart.
         They will be later written to the file using the
         __WriteRestartVar method.
         """
         api.io.printstd("Setting variables..")
         self.vars = {
             "nodes": self._mesh._nodedata,
-            "cells": self._mesh._celldata
-            }
+            "cells": self._mesh._celldata,
+        }
         # Start with the variables stored at the vertices
         # for key, item in self._mesh._nodedata.items():
-        #     api.io.print('std', "  node data: " + key)
+        #     api.io.printstd("  node data: " + key)
         #     self.vars["nodes"][key] = item
 
         # # Then the variables stored at the cells:
         # for key, item in self._mesh._celldata.items():
-        #     api.io.print('std', "  cell data: " + key)
+        #     api.io.printstd("  cell data: " + key)
         #     self.vars["cells"][key] = item
 
     def write_data(self, filename):
         """
         Main method of the ic3 restart file writer
         """
-        api.io.print('std', f"> WRITING FILE {filename!r}")
+        api.io.printstd(f"> WRITING FILE {filename!r}")
         self.filename = filename
         # Open the file for binary reading
         with open(self.filename, "wb") as self.fid:
             #
-            api.io.print('std', "> check consistency before writing")
+            api.io.printstd("> check consistency before writing")
             if not self.check():
                 raise RuntimeError("Inconsistent data to write")
             #
-            api.io.print('std', "> Writing header")
+            api.io.printstd("> Writing header")
             self.__WriteRestartHeader()
             #
-            api.io.print('std', "> Writing connectivity")
+            api.io.printstd("> Writing connectivity")
             self.__WriteRestartConnectivity()
             #
-            api.io.print('std', "> Writing informative values")
+            api.io.printstd("> Writing informative values")
             self.__WriteInformativeValues()
             #
-            api.io.print('std', "> Writing variables")
+            api.io.printstd("> Writing variables")
             self.__WriteRestartVar()
             #
-            api.io.print('std', "> End of file")
+            api.io.printstd("> End of file")
             header = restartSectionHeader()
             header.name = "EOF"
             header.id = ic3_restart_codes["UGP_IO_EOF"]
             header.skip = header.hsize
             header.write(self.fid, self.endian)
             #
             # self.fid is closed
@@ -290,15 +296,15 @@
         #
         # don't really know how useful it was; suppressed in V3
         self.__WriteRestartConnectivity_check()
         #
         # Connectivities
         # Faces-to-nodes connectivities
         # Header
-        api.io.print('std', f"  face to node connectivity")
+        api.io.printstd(f"  face to node connectivity")
         header = restartSectionHeader()
         header.name = "NOOFA_I_AND_V"
         header.id = ic3_restart_codes["UGP_IO_NOOFA_I_AND_V"]
         header.skip = (
             header.hsize
             + type2nbytes["int32"] * nface
             + type2nbytes["int32"] * self.params["noofa_count"]
@@ -313,48 +319,48 @@
         # Flattened face-to-node connectivity
         BinaryWrite(
             self.fid,
             self.endian,
             "i" * self.params["noofa_count"],
             self.f2v["noofa_v"].tolist(),
         )
-        # print('noofa',self.f2v["noofa"] )
-        # print('noofa_v',self.f2v["noofa_v"] )
+        # print('noofa', self.f2v["noofa"] )
+        # print('noofa_v', self.f2v["noofa_v"] )
         # Faces-to-cells connectivities
         # Header
-        api.io.print('std', f"  face to cell connectivity")
+        api.io.printstd(f"  face to cell connectivity")
         header = restartSectionHeader()
         header.name = "CVOFA"
         header.id = ic3_restart_codes["UGP_IO_CVOFA"]
         header.skip = header.hsize + type2nbytes["int32"] * nface * 2
         header.idata[0] = nface
         header.idata[1] = 2
         header.write(self.fid, self.endian)
         # Flattened face-to-cell connectivity
-        # print("W",self.f2e)
+        # print("W", self.f2e)
         # print(self.f2e.ravel())
         BinaryWrite(self.fid, self.endian, "i" * nface * 2, self.f2e.ravel().tolist())
-        # print('cellofface',self.f2e.ravel().tolist() )
+        # print('cellofface', self.f2e.ravel().tolist() )
         # Face zones, a.k.a boundary condition patches
-        api.io.print('std', f"  marks (face based)")
+        api.io.printstd(f"  marks (face based)")
         last_boco = 0
         for key, boco in self.bocos.items():
             assert key == boco.name
             assert boco.geodim in ('face', 'bdface'), "boco marks must be faces index"
             # Header
             header = restartSectionHeader()
             header.name = key
             header.id = ic3_restart_codes["UGP_IO_FA_ZONE"]
             header.skip = header.hsize
             # diff# print(self.bocos[key]["type"], type2zonekind)
             assert (
                 boco.type in type2zonekind.keys()
             ), f"unsupported type of boco for IC3 output: {boco.type}"
             ifmin, ifmax = boco.index.range()
-            api.io.print('std', f"  . ({boco.type}) {boco.name}: {ifmin}-{ifmax}")
+            api.io.printstd(f"  . ({boco.type}) {boco.name}: {ifmin}-{ifmax}")
             header.idata[0] = type2zonekind[boco.type]
             assert (
                 boco.index.type == 'range'
             ), "indexing must be a range and may need reordering"
             header.idata[1] = ifmin
             header.idata[2] = ifmax
             last_boco = max(last_boco, ifmax)
@@ -374,15 +380,15 @@
         )
         header.idata[0] = type2zonekind['internal']
         header.idata[1] = ifmin
         header.idata[2] = ifmax
         header.rdata[:] = 0.0
         header.write(self.fid, self.endian)  # Partition information
         # Header
-        api.io.print('std', f"  cell based partition info")
+        api.io.printstd(f"  cell based partition info")
         header = restartSectionHeader()
         header.name = "CV_PART"
         header.id = ic3_restart_codes["UGP_IO_CV_PART"]
         header.skip = header.hsize + type2nbytes["int32"] * ncell
         header.idata[0] = ncell
         header.idata[1] = self.params['partition'].get('npart', 1)
         header.write(self.fid, self.endian)
@@ -391,15 +397,15 @@
             self.fid,
             self.endian,
             "i" * ncell,
             self.params['partition'].get('icvpart', np.zeros((ncell,), dtype=np.int32)),
         )
         # Coordinates
         # Header
-        api.io.print('std', f"  nodes coordinates")
+        api.io.printstd(f"  nodes coordinates")
         header = restartSectionHeader()
         header.name = "X_NO"
         header.id = ic3_restart_codes["UGP_IO_X_NO"]
         header.skip = header.hsize + type2nbytes["float64"] * nnode * 3
         header.idata[0] = nnode
         header.idata[1] = 3
         header.write(self.fid, self.endian)
@@ -422,26 +428,24 @@
         header.write(self.fid, self.endian)
         # Write current number of iteration
         # Header
         key = "STEP"
         header = restartSectionHeader()
         header.name = key
         value = self.simstate[key.lower()]
-        api.io.print("std", "  write section for {} parameter: {}".format(key, value))
+        api.io.printstd(f"  write section for {key} parameter: {value}")
         header.id = ic3_restart_codes["UGP_IO_I0"]
         header.skip = header.hsize
         header.idata[0] = value
         header.write(self.fid, self.endian)
         # Write the rest, all double values
         # The monomials first
         for key in ["DT", "TIME"]:
             value = self.simstate[key.lower()]
-            api.io.print(
-                "std", "  write section for {} parameter: {}".format(key, value)
-            )
+            api.io.printstd(f"  write section for {key} parameter: {value}")
             header = restartSectionHeader()
             header.name = key
             header.id = ic3_restart_codes["UGP_IO_D0"]
             header.skip = header.hsize
             header.rdata[0] = value
             header.write(self.fid, self.endian)
         # The second level now
@@ -455,102 +459,116 @@
 
     def __WriteRestartVar(self):
         """
         Method to write all the variables into a restart file.
         Scalars, vectors and tensors all together.
         """
         # Start with the node based variables
-        for key, item in self.vars["nodes"].items():
+        #
+        nno = self.params["no_count"]
+        #
+        for ndname, nddata in self.vars["nodes"].items():
             # Scalar
-            if item.size == item.shape[0]:
+            if nddata.size == nddata.shape[0]:
                 # Header
+                api.io.printstd(f"  write node scalar data {ndname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = ndname
                 header.id = ic3_restart_codes["UGP_IO_NO_D1"]
                 header.skip = (
-                    header.hsize + type2nbytes["float64"] * self.params["no_count"]
+                    header.hsize + type2nbytes["float64"] * nno
                 )
-                header.idata[0] = self.params["no_count"]
+                header.idata[0] = nno
                 header.write(self.fid, self.endian)
                 # Field
-                BinaryWrite(self.fid, self.endian, "d" * self.params["no_count"], item)
-        for key, item in self.vars["nodes"].items():
+                BinaryWrite(
+                    self.fid, self.endian, "d" * nno, nddata,
+                )
+        #
+        for ndname, nddata in self.vars["nodes"].items():
             # Vector
-            if len(item.shape) == 2:
+            if len(nddata.shape) == 2:
+                api.io.printstd(f"  write node vector data {ndname}")
                 # Header
                 header = restartSectionHeader()
-                header.name = key
+                header.name = ndname
                 header.id = ic3_restart_codes["UGP_IO_NO_D3"]
                 header.skip = (
-                    header.hsize + type2nbytes["float64"] * self.params["no_count"] * 3
+                    header.hsize + type2nbytes["float64"] * nno * 3
                 )
-                header.idata[0] = self.params["no_count"]
+                header.idata[0] = nno
                 header.idata[1] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
-                    self.fid,
-                    self.endian,
-                    "d" * self.params["no_count"] * 3,
-                    item.ravel(order='C'),
+                    self.fid, self.endian, "d" * nno * 3,
+                    nddata.ravel(order='C'),
                 )
-        for key, item in self.vars["nodes"].items():
+        #
+        for ndname, nddata in self.vars["nodes"].items():
             # Tensor
-            if len(item.shape) == 3:
+            if len(nddata.shape) == 3:
                 pass
 
         # Then the cell based variables
-        for key, item in self.vars["cells"].items():
+        #
+        if self.vars["cells"]:  # if defined
+            ncv = self.params["cv_count"]
+        #
+        for cvname, cvdata in self.vars["cells"].items():
             # Scalar
-            if item.size == item.shape[0]:
+            if cvdata.size == cvdata.shape[0]:
                 # Header
+                api.io.printstd(f"  write cell scalar data {cvname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = cvname
                 header.id = ic3_restart_codes["UGP_IO_CV_D1"]
                 header.skip = (
-                    header.hsize + type2nbytes["float64"] * self.params["cv_count"]
+                    header.hsize + type2nbytes["float64"] * ncv
                 )
-                header.idata[0] = self.params["cv_count"]
+                header.idata[0] = ncv
                 header.write(self.fid, self.endian)
                 # Field
-                BinaryWrite(self.fid, self.endian, "d" * self.params["cv_count"], item)
-        for key, item in self.vars["cells"].items():
+                BinaryWrite(
+                    self.fid, self.endian, "d" * ncv, cvdata,
+                )
+        #
+        for cvname, cvdata in self.vars["cells"].items():
             # Vector
-            if len(item.shape) == 2:
+            if len(cvdata.shape) == 2:
                 # Header
+                api.io.printstd(f"  write cell vector data {cvname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = cvname
                 header.id = ic3_restart_codes["UGP_IO_CV_D3"]
                 header.skip = (
-                    header.hsize + type2nbytes["float64"] * self.params["cv_count"] * 3
+                    header.hsize + type2nbytes["float64"] * ncv * 3
                 )
-                header.idata[0] = self.params["cv_count"]
+                header.idata[0] = ncv
                 header.idata[1] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
-                    self.fid,
-                    self.endian,
-                    "d" * self.params["cv_count"] * 3,
-                    item.ravel(order='C'),
+                    self.fid, self.endian, "d" * ncv * 3,
+                    cvdata.ravel(order='C'),
                 )
-        for key, item in self.vars["cells"].items():
+        #
+        for cvname, cvdata in self.vars["cells"].items():
             # Tensor
-            if len(item.shape) == 3:
+            if len(cvdata.shape) == 3:
                 # Header
+                api.io.printstd(f"  write cell tensor data {cvname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = cvname
                 header.id = ic3_restart_codes["UGP_IO_CV_D33"]
                 header.skip = (
-                    header.hsize + type2nbytes["float64"] * self.params["cv_count"] * 9
+                    header.hsize + type2nbytes["float64"] * ncv * 9
                 )
-                header.idata[0] = self.params["cv_count"]
+                header.idata[0] = ncv
                 header.idata[1] = 3
                 header.idata[2] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
-                    self.fid,
-                    self.endian,
-                    "d" * self.params["cv_count"] * 9,
-                    item.ravel(order='C'),
+                    self.fid, self.endian, "d" * ncv * 9,
+                    cvdata.ravel(order='C'),
                 )
```

### Comparing `cfdtools-0.5.0/cfdtools/ic3/writerV3.py` & `cfdtools-0.5.1/cfdtools/ic3/writerV3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Import modules
-import numpy as np
+# import numpy as np
 import cfdtools.api as api
-import cfdtools.meshbase._mesh as _mesh
-from cfdtools.ic3._ic3 import *
-from cfdtools.ic3.writerV2 import writer as writer_v2
+
+from cfdtools.ic3._ic3 import (
+    ic3_restart_codes,
+    properties_ugpcode,
+    type2nbytes,
+    BinaryWrite,
+    restartSectionHeader,
+)
+from cfdtools.ic3 import writerV2
 
 ###################################################################################################
 
 
 @api.fileformat_writer('IC3', '.ic3')
-class writer(writer_v2):
+class writer(writerV2.writer):
     '''Implementation of the writer to write ic3 restart files'''
 
     __version__ = "3"
 
     def __init__(self, mesh, endian='native'):
         """
         Initialization of a ic3 restart file writer.
@@ -28,125 +34,141 @@
         Method writing the header of a restart file.
         It is composed of two integers, the "magic number" used as a flag for endianness
         and the CharlesX version number.
         input   : handle on an open restart file, [type file identifier]
         """
         # Write the two integers
         BinaryWrite(
-            self.fid, self.endian, "ii", [ic3_restart_codes["UGP_IO_MAGIC_NUMBER"], 3]
+            self.fid, self.endian, "ii",
+            [ic3_restart_codes["UGP_IO_MAGIC_NUMBER"], 3],
         )
 
     def __WriteRestartConnectivity_check(self):
         # nothing to do in V3
         return
 
     def __WriteRestartVar(self):
         """
         Method to write all the variables into a restart file.
         Scalars, vectors and tensors all together.
         """
         # Start with the node based variables
-        for key, item in self.vars["nodes"].items():
+        #
+        nno = self.params["no_count"]
+        #
+        for ndname, nddata in self.vars["nodes"].items():
             # Scalar
-            if item.size == item.shape[0]:
+            if nddata.size == nddata.shape[0]:
                 # Header
-                api.io.print('std', '  write node scalar data ' + key)
+                api.io.printstd(f"  write node scalar data {ndname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = ndname
                 header.id = {
                     "float64": ic3_restart_codes["UGP_IO_NO_D1"],
                     "int64": ic3_restart_codes["UGP_IO_NO_II1"],
-                }[item.dtype.name]
-                header.skip = header.hsize + item.itemsize * self.params["no_count"]
-                header.idata[0] = self.params["no_count"]
+                }[nddata.dtype.name]
+                header.skip = header.hsize + nddata.itemsize * nno
+                header.idata[0] = nno
                 header.write(self.fid, self.endian)
                 # Field
                 chartype = properties_ugpcode[header.id]['structcode']
                 BinaryWrite(
-                    self.fid, self.endian, chartype * self.params["no_count"], item
+                    self.fid, self.endian, chartype * nno, nddata,
                 )
-        for key, item in self.vars["nodes"].items():
+        #
+        for ndname, nddata in self.vars["nodes"].items():
             # Vector
-            if len(item.shape) == 2:
-                api.io.print('std', '  write node vector data ' + key)
+            if len(nddata.shape) == 2:
+                api.io.printstd(f"  write node vector data {ndname}")
                 # Header
                 header = restartSectionHeader()
-                header.name = key
+                header.name = ndname
                 header.id = ic3_restart_codes["UGP_IO_NO_D3"]
                 header.skip = (
-                    header.hsize + type2nbytes["float64"] * self.params["no_count"] * 3
+                    header.hsize + type2nbytes["float64"] * nno * 3
                 )
-                header.idata[0] = self.params["no_count"]
+                header.idata[0] = nno
                 header.idata[1] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
-                    self.fid,
-                    self.endian,
-                    "d" * self.params["no_count"] * 3,
-                    item.ravel(order='C'),
+                    self.fid, self.endian, "d" * nno * 3,
+                    nddata.ravel(order='C'),
                 )
-        for key, item in self.vars["nodes"].items():
+        #
+        for ndname, nddata in self.vars["nodes"].items():
             # Tensor
-            if len(item.shape) == 3:
+            if len(nddata.shape) == 3:
                 pass
 
         # Then the cell based variables
-        if self.vars["cells"]: # if defined
+        #
+        if self.vars["cells"]:  # if defined
             ndof = self.vars["cells"].ndof
-        for key, npdata in self.vars["cells"].items():
             ncv = self.params["cv_count"]
             totsize = ndof * ncv
+        #
+        for cvname, cvdata in self.vars["cells"].items():
             # Scalar
-            if npdata.size == npdata.shape[0]:
+            if cvdata.size == cvdata.shape[0]:
                 # Header
-                api.io.print('std', '  write cell scalar data ' + key)
+                api.io.printstd(f"  write cell scalar data {cvname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = cvname
                 header.id = {
                     "float64": ic3_restart_codes["UGP_IO_CV_D1"],
                     "int64": ic3_restart_codes["UGP_IO_CV_II1"],
-                }[npdata.dtype.name]
-                header.skip = header.hsize + type2nbytes[npdata.dtype.name] * totsize
+                }[cvdata.dtype.name]
+                header.skip = (
+                    header.hsize + type2nbytes[cvdata.dtype.name] * totsize
+                )
                 header.idata[0] = ncv
                 header.idata[1] = ndof
                 header.write(self.fid, self.endian)
                 # Field
                 chartype = properties_ugpcode[header.id]['structcode']
-                BinaryWrite(self.fid, self.endian, chartype * totsize, npdata)
-        for key, npdata in self.vars["cells"].items():
-            totsize = ndof * self.params["cv_count"]
+                BinaryWrite(
+                    self.fid, self.endian, chartype * totsize, cvdata,
+                )
+        #
+        for cvname, cvdata in self.vars["cells"].items():
             # Vector
-            if len(npdata.shape) == 2:
+            if len(cvdata.shape) == 2:
                 # Header
-                api.io.print('std', '  write cell vector data ' + key)
+                api.io.printstd(f"  write cell vector data {cvname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = cvname
                 header.id = ic3_restart_codes["UGP_IO_CV_D3"]
-                header.skip = header.hsize + type2nbytes["float64"] * totsize * 3
+                header.skip = (
+                    header.hsize + type2nbytes["float64"] * totsize * 3
+                )
                 header.idata[0] = ncv
                 header.idata[1] = ndof
                 # header.idata[1] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
-                    self.fid, self.endian, "d" * totsize * 3, npdata.ravel(order='C')
+                    self.fid, self.endian, "d" * totsize * 3,
+                    cvdata.ravel(order='C'),
                 )
-        for key, npdata in self.vars["cells"].items():
-            totsize = ndof * self.params["cv_count"]
+        #
+        for cvname, cvdata in self.vars["cells"].items():
             # Tensor
-            if len(npdata.shape) == 3:
+            if len(cvdata.shape) == 3:
                 # Header
-                api.io.print('std', '  write cell tensor data ' + key)
+                api.io.printstd(f"  write cell tensor data {cvname}")
                 header = restartSectionHeader()
-                header.name = key
+                header.name = cvname
                 header.id = ic3_restart_codes["UGP_IO_CV_D33"]
-                header.skip = header.hsize + type2nbytes["float64"] * totsize * 9
+                header.skip = (
+                    header.hsize + type2nbytes["float64"] * totsize * 9
+                )
                 header.idata[0] = ncv
                 header.idata[1] = ndof
                 # header.idata[1] = 3
                 header.idata[2] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
-                    self.fid, self.endian, "d" * totsize * 9, npdata.ravel(order='C')
+                    self.fid, self.endian, "d" * totsize * 9,
+                    cvdata.ravel(order='C'),
                 )
```

### Comparing `cfdtools-0.5.0/cfdtools/meshbase/_connectivity.py` & `cfdtools-0.5.1/cfdtools/meshbase/_connectivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cfdtools.api as api
-import cfdtools.meshbase._elements as ele
+import cfdtools.meshbase._elements as _elem
 from collections import defaultdict, OrderedDict
 from itertools import chain
 import numpy as np
 
 
 class indexlist:
     """class of different implementation of list of index
@@ -210,21 +210,20 @@
     # def reindexed_elems(self, etype):
     #     ind = self._elem2node[etype]['index']
     #     e2n[ind,:] = self._elem2node[etype]['elem2node'] # dangerous, index may be too large
     #     return e2n
 
     def print(self, prefix="", detailed=False):
         for elemtype, elemco in self._elem2node.items():
-            api.io.print(
-                "std",
+            api.io.printstd(
                 prefix + f"{elemtype}: {elemco['elem2node'].shape} with index {elemco['index']}",
             )
             if detailed:
-                api.io.print("std", prefix + f"  index: {elemco['index'].list()}")
-                api.io.print("std", prefix + f"  faces: {elemco['elem2node']}")
+                api.io.printstd(prefix + f"  index: {elemco['index'].list()}")
+                api.io.printstd(prefix + f"  faces: {elemco['elem2node']}")
 
     def all_index(self):
         return list(sum([econ['index'].list() for _, econ in self.items()], []))
 
     # def index_elem_tuples(self):
     #     # optim: here, .list() is not mandatory but avoid massively calling .list().getitem()
     #     return list( (i, face.ravel().tolist())
@@ -255,15 +254,15 @@
         return list(set(joinlist))  # make unique
 
     def importfrom_compressedindex(self, zconn: compressed_listofindex):
         # there is no test but must only applied to faces
         nodeperface = zconn._index[1:] - zconn._index[:-1]
         uniq, counts = np.unique(nodeperface, return_counts=True)
         for facesize, nface in zip(uniq, counts):
-            typef = ele.face_from_nnode[facesize]
+            typef = _elem.face_from_nnode[facesize]
             index = np.argwhere(nodeperface == facesize)
             zind = zconn._index[index]
             nodes = np.hstack(tuple(zconn._value[zind + i] for i in range(facesize)))
             self.add_elems(typef, nodes, indexlist(ilist=index))
 
     # @profile
     def exportto_compressedindex(self) -> compressed_listofindex:
@@ -312,27 +311,27 @@
                 elemtype,
                 elemsdict,
             ) in self._elem2node.items():  # elemtype: 'hexa8', elemsarray: ndarray[nelem,8]
                 index = elemsdict['index'].list()  # call export to list now
                 elemsarray = elemsdict['elem2node']
                 # V0
                 # for ielem in range(elemsarray.shape[0]):
-                #     for ftype, listfaces in ele.elem2faces[elemtype].items():
+                #     for ftype, listfaces in _elem.elem2faces[elemtype].items():
                 #         # for face in listfaces:
                 #         #     faces_neighbour[ftype].append( (tuple(elemsarray[ielem, face]), index[ielem]) )
                 #         faces_neighbour[ftype].extend(
                 #             [ (tuple(elemsarray[ielem, face]), index[ielem]) for face in listfaces ] )
                 # V1 (-3%)
-                # for ftype, listfaces in ele.elem2faces[elemtype].items():
+                # for ftype, listfaces in _elem.elem2faces[elemtype].items():
                 #     for face in listfaces:
                 #         faces_neighbour[ftype].extend(
                 #             [ (tuple(elemsarray[ielem, face]), index[ielem]) for ielem in range(elemsarray.shape[0]) ] )
                 # V2 (-30%)
                 # NODE ORDER of face IS REVERSED
-                for ftype, face_of_elem in ele.elem2faces[elemtype].items():
+                for ftype, face_of_elem in _elem.elem2faces[elemtype].items():
                     for eface in face_of_elem:
                         reindex_f = elemsarray[:, list(reversed(eface))].tolist()
                         faces_neighbour[ftype].extend(
                             [(tuple(fnodes), ind) for fnodes, ind in zip(reindex_f, index)]
                         )
             return faces_neighbour
 
@@ -413,17 +412,17 @@
         """
         assert nplanes > 1
         ncell = nplanes - 1
         newcon = elem_connectivity()
         for etype, econ in self.items():
             nelem = econ['elem2node'].shape[0]
             elemcon = np.tile(econ['elem2node'], (ncell, 2))
-            fnnode = ele.nnode_elem[etype]
+            fnnode = _elem.nnode_elem[etype]
             elemcon[:, fnnode : 2 * fnnode] += inodeshift
             for i in range(ncell):
                 elemcon[i * nelem : (i + 1) * nelem, :] += i * inodeshift
             # print(etype, econ['elem2node'], elemcon)
             index = np.tile(econ['index'].list(), (ncell))
             for i in range(ncell):
                 index[i * nelem : (i + 1) * nelem] += i * inodeshift
-            newcon.add_elems(ele.extruded_face[etype], elemcon, indexlist(ilist=index.tolist()))
+            newcon.add_elems(_elem.extruded_face[etype], elemcon, indexlist(ilist=index.tolist()))
         return newcon
```

### Comparing `cfdtools-0.5.0/cfdtools/meshbase/_elements.py` & `cfdtools-0.5.1/cfdtools/meshbase/_elements.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,56 @@
 # import cfdtools.api as api
 
 geodim = {'point': 0, 'line': 1, 'surface': 2, 'volume': 3}
 
 elem_properties = [  # itype, name, nnode, geodim, extruded
-    (0, 'node1', 1, 0, 'bar2'),
-    (0, 'bar2', 2, 1, 'quad4'),
-    (0, 'tri3', 3, 2, 'penta6'),
-    (0, 'quad4', 4, 2, 'hexa8'),
-    (0, 'tetra4', 4, 3, 'none'),
-    (0, 'hexa8', 8, 3, 'none'),
+    (0, '   node1', 1, 0, '    bar2'),
+    (0, '    bar2', 2, 1, '   quad4'),
+    (0, '    tri3', 3, 2, '  penta6'),
+    (0, '   quad4', 4, 2, '   hexa8'),
+    (0, '  tetra4', 4, 3, '    none'),
+    (0, '   hexa8', 8, 3, '    none'),
 ]
 
-elem_dim = {e: d for _, e, _, d, _ in elem_properties}
-nnode_elem = {e: n for _, e, n, _, _ in elem_properties}
-face_from_nnode = {n: e for _, e, n, d, _ in elem_properties if d <= 2}
-extruded_face = {e: ex for _, e, n, d, ex in elem_properties if d <= 2}
+elem_properties = [
+    tuple(  i.lstrip() if type(i) is str else i for i in u )
+    for u in elem_properties
+]
+
+elem_dim = {
+    e: d for _, e, _, d, _ in elem_properties
+}
+nnode_elem = {
+    e: n for _, e, n, _, _ in elem_properties
+}
+face_from_nnode = {
+    n: e for _, e, n, d, _ in elem_properties if d <= 2
+}
+extruded_face = {
+    e: x for _, e, _, d, x in elem_properties if d <= 2
+}
+
+del elem_properties
 
 # define list of faces from an element type
 #   faces are defined with inward normal
 # see https://cgns.github.io/CGNS_docs_current/sids/conv.html#unst_hexa
 elem2faces = {
-    'quad4': {'bar2': [[0, 1], [1, 2], [2, 3], [3, 0]]},
+    'quad4': {
+        'bar2': [
+            [0, 1],
+            [1, 2],
+            [2, 3],
+            [3, 0]
+        ]
+    },
     'hexa8': {
         'quad4': [
             [0, 1, 2, 3],
             [4, 7, 6, 5],
             [0, 4, 5, 1],
             [2, 6, 7, 3],
             [0, 3, 7, 4],
-            [1, 5, 6, 2],
+            [1, 5, 6, 2]
         ]
     },
 }
```

### Comparing `cfdtools-0.5.0/cfdtools/meshbase/_mesh.py` & `cfdtools-0.5.1/cfdtools/meshbase/_mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cfdtools.api as api
-import cfdtools.meshbase._connectivity as conn
-# import cfdtools.meshbase._elements as ele
+import cfdtools.meshbase._connectivity as _conn
+# import cfdtools.meshbase._elements as _elem
 from cfdtools.utils.maths import minavgmax
 import itertools
 import numpy as np
 
 
 class submeshmark:
     # authorized geomdim type and actual dimension
@@ -46,15 +46,15 @@
         self._geodim = geodim
 
     @property
     def index(self):
         return self._index
 
     @index.setter
-    def index(self, index: conn.indexlist):
+    def index(self, index: _conn.indexlist):
         assert self.geodim in self._available_geodim
         self._index = index
 
     @property
     def type(self):
         return self._properties['type']
 
@@ -132,64 +132,69 @@
         self._nodes['y'] = y
         self._nodes['z'] = z
 
     def nodescoord(self, ndarray=False):
         coords = tuple(self._nodes[c] for c in ['x', 'y', 'z'])
         return np.column_stack(coords) if ndarray else coords
 
-    def set_cell2node(self, cell2node: conn.elem_connectivity):
+    def set_cell2node(self, cell2node: _conn.elem_connectivity):
         """set cell to node connectivity
 
         Args:
             cell2node (elem_connectivity): connectivity of cells
         """
         self._cell2node = cell2node
         self._ncell = self._cell2node.nelem
         self._check_cell2node()
 
     def add_faces(
         self,
         facetype: str,
-        face2node: conn.elem_connectivity,
-        face2cell: conn.indexindirection = None,
+        face2node: _conn.elem_connectivity,
+        face2cell: _conn.indexindirection = None,
     ):
         """set faces connectivity with face type et optional face/cell connectivity
 
         Args:
             facetype (str): _description_
-            face2node (conn.elem_connectivity): _description_
-            face2cell (conn.indexindirection, optional): _description_. Defaults to None.
+            face2node (_conn.elem_connectivity): _description_
+            face2cell (_conn.indexindirection, optional): _description_. Defaults to None.
         """
         if facetype in self.__available_facetypes:
             self._faces[facetype] = {'face2node': face2node, 'face2cell': face2cell}
         else:
-            api.io.error_stop(f"bad face type: {facetype} since {self.__available_facetypes} expected")
-        self.nface = np.sum([fcon['face2node'].nelem for _, fcon in self._faces.items()])
+            api.io.error_stop(
+                f"bad face type: {facetype}"
+                f" since {self.__available_facetypes} expected"
+            )
+        self.nface = np.sum(
+            [fcon['face2node'].nelem for _, fcon in self._faces.items()]
+        )
 
     def pop_faces(self, facetype: str):
         if facetype in self.__available_facetypes:
             if facetype in self._faces.keys():
                 for key, item in self._faces[facetype].items():
                     del item
                 self._faces.pop(facetype)
 
     def export_mixedfaces(self):
-        mixedfaces_con = conn.elem_connectivity()
+        mixedfaces_con = _conn.elem_connectivity()
         mixedfaces_con.importfrom_merge(
             (self._faces['boundary']['face2node'], self._faces['internal']['face2node'])
         )
-        face2cell = conn.indexindirection()
+        face2cell = _conn.indexindirection()
         face2cell.conn = np.concatenate(
             (
                 self._faces['boundary']['face2cell'].conn,
                 self._faces['internal']['face2cell'].conn,
             ),
             axis=0,
         )
-        # print('merge',face2cell.conn)
+        # print('merge', face2cell.conn)
         return mixedfaces_con, face2cell
 
     def add_boco(self, boco: submeshmark):
         self._bocos[boco.name] = boco
 
     def remove_boco(self, name):
         self._bocos.pop(name)
@@ -206,57 +211,71 @@
         assert 'boundary' in self._faces.keys()
         index_face_tuples = self._faces['boundary']['face2node'].index_elem_tuples()
         for _, boco in self._bocos.items():
             if boco.nodebased():
                 nodeset = set(boco.index.list())
                 # get all face index whose nodes are all in nodeset
                 listface_index = [
-                    i for i, _ in filter(lambda t: face_in_nodelist(t[1], nodeset), index_face_tuples)
+                    i
+                    for i, _ in filter(
+                        lambda t: face_in_nodelist(t[1], nodeset), index_face_tuples
+                    )
                 ]
                 boco.geodim = 'bdface'
-                boco.index = conn.indexlist(ilist=listface_index)
+                boco.index = _conn.indexlist(ilist=listface_index)
                 # print(boco.name, len(nodeset), len(boco.index.list()))
 
     def list_boco_index(self):
-        return list(itertools.chain(*[boco.index.list() for _, boco in self._bocos.items()]))
+        return list(
+            itertools.chain(
+                *[boco.index.list() for _, boco in self._bocos.items()]
+            )
+        )
 
     def make_unmarked_BC(self, name="unmarked_faces"):
         """check all boundaring faces are marked and create a specific boco if not"""
         if 'boundary' in self._faces.keys():
             # number of (boundary) faces in face connectivity
             # nbdface = self._faces['boundary']['face2node'].nelem
             for _, boco in self._bocos.items():
                 assert boco.geodim in ('face', 'bdface'), "boco marks must be faces index"
             list_marked = self.list_boco_index()
-            list_missing = list(set(self._faces['boundary']['face2node'].all_index()) - set(list_marked))
+            list_missing = list(
+                    set(self._faces['boundary']['face2node'].all_index())
+                  - set(list_marked)
+            )
             if list_missing:
                 boco = submeshmark(name)
                 boco.geodim = 'bdface'
                 boco.type = 'boundary'
                 boco.properties['periodic_transform'] = None
-                boco.index = conn.indexlist(ilist=list_missing)
+                boco.index = _conn.indexlist(ilist=list_missing)
                 self.add_boco(boco)
         else:
             list_missing = []
             api.io.print(
                 'warning', "can only reindex faces according to boco if separated in 'boundary' list"
             )
         return list_missing
 
-    def seekmark(self, name: str) -> submeshmark:
+    def seekmark(self, name: str) -> submeshmark:  # What is this method ??
         """look for diffent marks set to find mark name"""
         # only _bocos for now
         return self._bocos[name]
 
-    def exportmark_asmesh(self, name):
-        meshmark = self.seekmark(name)
+    def exportmark_asmesh(self, name):  # What is this method ??
+        # meshmark = self.seekmark(name)  # Never used. Uncomment if useful...
         newmesh = Mesh()
         return newmesh
 
-    def export_extruded(self, direction=np.array([0.0, 0.0, 1.0]), extrude=[0.0, 1.0], domain="fluid"):
+    def export_extruded(self, direction=None, extrude=None, domain="fluid"):
+        if direction is None:
+            direction = np.array([0.0, 0.0, 1.0])
+        if extrude is None:
+            extrude = [0.0, 1.0]
         extrude_range = np.array(extrude)
         nrange = extrude_range.size
         assert nrange > 1, "extrusion only possible for at least 2 planes"
         newmesh = Mesh(ncell=self.ncell * nrange, nnode=self.nnode * nrange)
         # SHOULD CHECK DIRECTION AND MESH ORIENTATION
         # extrude nodes
         ntotnode = self.nnode
@@ -273,29 +292,29 @@
             newboco = submeshmark(boco.name)
             newboco.geodim = boco.geodim
             newboco.type = boco.type
             index = np.tile(boco.index.list(), (nrange))
             nbcnode = boco.index.size
             for i in range(nrange):
                 index[i * nbcnode : (i + 1) * nbcnode] += i * ntotnode
-            newboco.index = conn.indexlist(ilist=index.tolist())
+            newboco.index = _conn.indexlist(ilist=index.tolist())
             newmesh.add_boco(newboco)
         # create initial 2D domain as boco
         newboco = submeshmark(name=domain + '0')
         newboco.geodim = 'bdnode'
         newboco.type = 'boundary'
         index = self._cell2node.nodelist()
-        newboco.index = conn.indexlist(ilist=index)
+        newboco.index = _conn.indexlist(ilist=index)
         newmesh.add_boco(newboco)
         # create extruded 2D domain as boco
         newboco = submeshmark(name=domain + '1')
         newboco.geodim = 'bdnode'
         newboco.type = 'boundary'
         index = (np.array(index) + (nrange - 1) * ntotnode).tolist()
-        newboco.index = conn.indexlist(ilist=index)
+        newboco.index = _conn.indexlist(ilist=index)
         newmesh.add_boco(newboco)
         return newmesh
 
     def set_params(self, params):
         self._params = params
 
     def update_params(self, params):
@@ -327,83 +346,88 @@
         nbdface = self._faces['boundary']['face2node'].nelem
         for _, boco in self._bocos.items():
             assert boco.geodim in ('face', 'bdface'), "boco marks must be faces index"
         oldindex = self.list_boco_index()
         # checks
         c_unique = np.all(np.unique(oldindex) == sorted(oldindex))
         if not c_unique:
-            api.io.print('error', "  some faces are marked by several boundary marks")
+            api.io.print('error',
+                "  some faces are marked by several boundary marks")
         c_min0 = min(oldindex) == 0
         if not c_min0:
-            api.io.print(
-                'error',
+            api.io.print('error',
                 "  first face index (0) is not marked as a boundary\n"
-                + "  some boundary faces may be missing",
+                "  some boundary faces may be missing",
             )
         c_max = max(oldindex) <= len(oldindex) - 1
         if not c_max:
-            api.io.print(
-                'error',
+            api.io.print('error',
                 "  max face reference is greater than the number of found faces\n"
-                + "  boundary faces must be indexed first before reindexing",
+                "  boundary faces must be indexed first before reindexing",
             )
         c_lengths = len(oldindex) == nbdface
         if not c_lengths:
-            api.io.print('error', f"  some boundary faces are not marked: {nbdface-len(oldindex)}")
+            api.io.print('error',
+                f"  some boundary faces are not marked: {nbdface-len(oldindex)}")
         if not (c_unique and c_min0 and c_max):
             api.error_stop("inconsistent face marks when reordering")
         newindex = np.full_like(oldindex, -1)
         newindex[oldindex] = np.arange(len(oldindex))
         assert min(newindex) >= 0, "inconsistency: there must not be -1 index"
         # reindex boco
         for _, boco in self._bocos.items():
-            boco.index = conn.indexlist(ilist=newindex[boco.index.list()].tolist())
+            boco.index = _conn.indexlist(ilist=newindex[boco.index.list()].tolist())
             boco.index.compress()  # try to (and must) make it a range
         # reindex boundary faces
         for _, fdict in self._faces['boundary']['face2node'].items():
-            fdict['index'] = conn.indexlist(ilist=newindex[fdict['index'].list()].tolist())
+            fdict['index'] = _conn.indexlist(ilist=newindex[fdict['index'].list()].tolist())
             # fdict['index'].compress() # not expected
         if 'face2cell' in self._faces['boundary']:
-            self._faces['boundary']['face2cell'].conn = self._faces['boundary']['face2cell'].conn[oldindex, :]
+            self._faces['boundary']['face2cell'].conn = (
+                self._faces['boundary']['face2cell'].conn[oldindex, :]
+            )
 
     def printinfo(self, detailed=False):
-        api.io.print("std", f"nnode: {self.nnode}")
+        api.io.printstd(f"nnode: {self.nnode}")
         for c in ('x', 'y', 'z'):
             api.io.printstd(
-                "  {} min:avg:max = {:.3f}:{:.3f}:{:.3f}".format(c, *minavgmax(self._nodes[c])),
+                f"  {c} min:avg:max ="
+                " {:.3f}:{:.3f}:{:.3f}".format(*minavgmax(self._nodes[c])),
             )
 
-        api.io.print("std", f"ncell: {self.ncell}")
+        api.io.printstd(f"ncell: {self.ncell}")
         if self._cell2node:
             self._cell2node.print()
         else:
-            api.io.print("std", "  no cell/node connectivity")
-        api.io.print('std', "nnode:", self.nnode)
-        api.io.print('std', "nface:", self.nface)
+            api.io.printstd("  no cell/node connectivity")
+        api.io.printstd("nnode:", self.nnode)
+        api.io.printstd("nface:", self.nface)
         if self._faces:
             for t, facedict in self._faces.items():
-                api.io.print("std", f"  type {t}: {' '.join(facedict['face2node'].elems())}")
+                api.io.printstd(
+                    f"  type {t}: {' '.join(facedict['face2node'].elems())}"
+                )
                 facedict['face2node'].print(prefix='  . ', detailed=detailed)
         else:
-            api.io.print("std", "  no face/node connectivity")
-        api.io.print('std', f"bocos: {' '.join(self._bocos.keys())}")
+            api.io.printstd("  no face/node connectivity")
+        api.io.printstd(f"bocos: {' '.join(self._bocos.keys())}")
         for name, boco in self._bocos.items():
-            api.io.print("std", f"  BC {boco}")
-        api.io.print("std", "params:", self._params)
+            api.io.printstd(f"  BC {boco}")
+        api.io.printstd("params:", self._params)
 
     def _check_cell2node(self):
         if self._cell2node is not None:
             assert isinstance(
-                self._cell2node, conn.elem_connectivity
+                self._cell2node, _conn.elem_connectivity
             ), "cell2node connecitivity is not the expected class"
             assert (
                 self.ncell == self._cell2node.nelem
             ), f"inconsistent size of cells {self.ncell} and {self._cell2node.nelem}"
-        # for etype, conn in self._cell2node.items():
-        #    assert etype in ele.elem2faces.keys()
+        # for etype, econn in self._cell2node.items():
+        #    assert etype in _elem.elem2faces.keys()
         return True
 
     def make_face_connectivity(self):
         (
             intfaces,
             intf2c,
             boundfaces,
@@ -415,15 +439,15 @@
 
     def check(self):
         """check a consistent mesh with adequate boundary conditions"""
         # check cell2node and cell numbers
         assert self.ncell > 0
         assert self.nnode > 0
         self._check_cell2node()
-        # api.io.print('std','ckeck: at least cell/node or face/node face/cell connectivity')
+        # api.io.printstd('ckeck: at least cell/node or face/node face/cell connectivity')
         # assert(not self._cell2node or (not self._face2node and not self._face2cell))
         # assert self._check_cell2node() # not compulsory
         assert not self.make_unmarked_BC()
         return True
 
     def morph(self, fmorph):
         '''
```

### Comparing `cfdtools-0.5.0/cfdtools/meshbase/simple.py` & `cfdtools-0.5.1/cfdtools/meshbase/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # simple subpackage
 import cfdtools.api as api
 import cfdtools.meshbase._mesh as _mesh
-import cfdtools.meshbase._connectivity as conn
+import cfdtools.meshbase._connectivity as _conn
 from itertools import product
 import numpy as np
 
 
 class Cube:
     def __init__(self, nx, ny, nz=1) -> None:
         self._nx = nx
@@ -56,17 +56,17 @@
         )
         index = self.elemglobindex_ijk(ei, ej, ek)
         return hexa2node, index.tolist()
 
     def export_mesh(self):
         meshdata = _mesh.Mesh(ncell=self.ncell, nnode=self.nnode)
         # set cell connectivity
-        cell2node = conn.elem_connectivity()
+        cell2node = _conn.elem_connectivity()
         hexanode, ielem = self._elems()
-        cell2node.add_elems('hexa8', np.array(hexanode), conn.indexlist(ilist=ielem))
+        cell2node.add_elems('hexa8', np.array(hexanode), _conn.indexlist(ilist=ielem))
         meshdata.set_cell2node(cell2node)
         # set node coordinates
         ni, nj, nk = np.array(self.nodes_ijk()).T
         x, y, z = self.nodes_xyz(ni, nj, nk)
         meshdata.set_nodescoord_xyz(x, y, z)
         # boco
         tasks = {
@@ -97,15 +97,15 @@
         }
         for name, task in tasks.items():
             bcmark = _mesh.submeshmark(name)
             bcmark.geodim = 'bdnode'
             bcmark.type = 'boundary'
             ni, nj, nk = np.array(list(task['ijknodes'])).T
             nodes = self.nodeglobindex_ijk(ni, nj, nk)
-            bcmark.index = conn.indexlist(ilist=nodes.tolist())
+            bcmark.index = _conn.indexlist(ilist=nodes.tolist())
             meshdata.add_boco(bcmark)
         return meshdata
 
 
 if __name__ == "__main__":
     box = Cube(2, 1, 1)
     mesh = box.export_mesh()
```

### Comparing `cfdtools-0.5.0/cfdtools/physics/dicovar.py` & `cfdtools-0.5.1/cfdtools/physics/dicovar.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/cfdtools/probes/data.py` & `cfdtools-0.5.1/cfdtools/probes/data.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/cfdtools/probes/plot.py` & `cfdtools-0.5.1/cfdtools/probes/plot.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/cfdtools/utils/polybase.py` & `cfdtools-0.5.1/cfdtools/utils/polybase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from ..utils._dev import lazyprop
+try:
+    from ..utils._dev import lazyprop
+except ImportError:
+    from _dev import lazyprop
 import numpy as np
 import numpy.linalg as lin
 import numpy.polynomial.legendre as polyL
 import numpy.polynomial.polynomial as poly
-from scipy.special import roots_legendre, eval_legendre
+from scipy.special import roots_legendre  # , eval_legendre
 
 polybasis_dict = {
-    'legendre' : polyL.Legendre,
-    'polynomial' : poly.Polynomial
+    'legendre': polyL.Legendre,
+    'polynomial': poly.Polynomial
 }
 
+
 class poly1d():
     def __init__(self, order: int, series='legendre') -> None:
         self._name = series
         self._order = order
-        self._roots, self._weights = roots_legendre(order)
+        self._roots, self._wghts = roots_legendre(order)
         self._basis = [ (0,)*i+(1,) for i in range(order) ]
         self._polyeval = polybasis_dict[series]
         self._gradbasis = [
             self._polyeval(ibas).deriv().coef
                 for ibas in self._basis
         ]
 
     @lazyprop
     def vdm(self):
-        """vandermonde matrix for base to Lagrange
-        
-        """
+        """vandermonde matrix for base to Lagrange"""
         return np.array([
             self._polyeval(ibas)(self._roots)
                 for ibas in self._basis
         ])
 
     @lazyprop
     def invvdm(self):
@@ -38,20 +40,31 @@
 
     def interp_weights(self, x):
         return self.invvdm @ np.array([
             self._polyeval(ibas)(x)
                 for ibas in self._basis
         ])
 
+    value_weights = interp_weights
+
     def diff_weights(self, x):
         return self.invvdm @ np.array([
             self._polyeval(ibas)(x)
                 for ibas in self._gradbasis
         ])
 
+    gradv_weights = diff_weights
+
 
 if __name__ == "__main__":
-    b = poly1d(3, series='legendre')
-    print(b._roots)
-    #print(b._basis)
-    print("interp", b.interp_weights(-1))
-    print("diff", b.diff_weights(-1))
+    with np.printoptions(precision=12, floatmode='fixed', sign=' '):
+        # b = poly1d(3, series='legendre')
+        # b = poly1d(3, series='polynomial')
+        for p in polybasis_dict:
+            b = poly1d(4, series=p)
+            print(f"    basis:  {b._basis}")
+            print(f"    roots:  {b._roots}")
+            print(f"    wghts:  {b._wghts}")
+            print(f"(-1)value:  {b.value_weights(-1)}")
+            print(f"(+1)value:  {b.value_weights(+1)}")
+            print(f"(-1)gradv:  {b.gradv_weights(-1)}")
+            print(f"(+1)gradv:  {b.gradv_weights(+1)}")
```

### Comparing `cfdtools-0.5.0/cfdtools/vtk/_vtk.py` & `cfdtools-0.5.1/cfdtools/vtk/_vtk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 try:
     import pyvista as pv
     from pyvista import CellType
+
     importpyvista = True
 except ImportError:
     importpyvista = False
 import cfdtools.api as api
 import cfdtools.utils.maths as maths
 import cfdtools.meshbase._elements as ele
 import cfdtools.meshbase._mesh as cfdmesh
 from cfdtools.data import DataSetList
 import cfdtools.hdf5 as hdf5
 from pathlib import Path
 import numpy as np
 import scipy.spatial as spspa
 
 
-vtktype_ele = {'bar2': CellType.LINE, 'quad4': CellType.QUAD, 'hexa8': CellType.HEXAHEDRON}
-ele_vtktype = { i: etype for etype, i in vtktype_ele.items() }
+try:
+    vtktype_ele = {
+        'bar2': CellType.LINE,
+        'quad4': CellType.QUAD,
+        'hexa8': CellType.HEXAHEDRON,
+    }
+    ele_vtktype = {i: etype for etype, i in vtktype_ele.items()}
+except NameError:
+    api.io.print('error', "pyvista (with CellType) could not be imported")
+    raise
+
 
 @api.fileformat_writer("VTK", '.vtu')
 class vtkMesh:
     '''Implementation of the writer to write binary Vtk files using pyvista'''
 
     def __init__(self, mesh=None, pvmesh=None):
-        self._mesh = mesh
         if mesh and pvmesh:
             api.error_stop("vtkMesh cannot be initialized by both structures")
         if mesh:
             self.set_mesh(mesh)
         if pvmesh:
             self.set_pvmesh(pvmesh)
 
+    def _reset(self):
+        self._volume = None
+
     def set_mesh(self, mesh: cfdmesh.Mesh):
+        self._reset()
         self._mesh = mesh
         coords = self._mesh.nodescoord(ndarray=True)
         try:
             self._celldict = {
                 vtktype_ele[etype]: elem2node['elem2node']
                 for etype, elem2node in self._mesh._cell2node.items()
             }
             self._grid = pv.UnstructuredGrid(self._celldict, coords)
-        except:
+        except NameError:
             api.error_stop("pyvista (with CellType) could not be imported")
 
     def set_pvmesh(self, pvmesh: cfdmesh.Mesh):
+        self._reset()
         self._grid = pvmesh
 
     def write_data(self, filename):
         self._grid.save(filename)
 
     def read(self, filename):
         self.__init__()
@@ -65,46 +79,57 @@
             api.io.printstd(f"  bounds : {m.bounds}")
             api.io.printstd(f"  ncells : {m.n_cells}")
             api.io.printstd(f"  npoints: {m.n_points}")
             api.io.printstd("> data")
             api.io.printstd(f"  cell  data names: {m.cell_data.keys()}")
             api.io.printstd(f"  point data names: {m.point_data.keys()}")
             api.io.printstd(f"  field data names: {m.field_data.keys()}")
-            #api.io.printstd("> properties")
+            # api.io.printstd("> properties")
         else:
             api.io.warning("  no pyvista mesh available")
 
     def plot(self, background='white', show_edges=True, *args, **kwargs):
         self.pyvista_grid().plot(background=background, show_edges=show_edges, *args, **kwargs)
 
+    def importhdfgroup(self, hgroup: hdf5.Group, verbose=False):
+        assert hgroup.attrs['meshtype'] == 'unsvtk'
+        points = np.array(hgroup["nodes"])
+        celldict = {vtktype_ele[etype]: np.array(elem2node) for etype, elem2node in hgroup["cells"].items()}
+        self.set_pvmesh(pv.UnstructuredGrid(celldict, points))
+
     def dumhdfgroup(self, hgroup: hdf5.Group, **options):
         hgroup.attrs['meshtype'] = 'unsvtk'
         hgroup.create_dataset("nodes", data=self._grid.points, **options)
         hcells = hgroup.create_group("cells")
         for itype, cellco in self._grid.cells_dict.items():
             hcells.create_dataset(ele_vtktype[itype], data=cellco, **options)
 
+    def volumes(self):
+        if not self._volume:
+            self._volume = self._grid.compute_cell_sizes().cell_data["Volume"]
+        return self._volume
 
 
-class vtkList():
-
+class vtkList:
     def __init__(self, filelist, verbose=False) -> None:
         self._list = filelist
         self._verbose = verbose
 
     @property
     def nfile(self):
         return len(self._list)
-    
+
     def allexist(self):
         return all(Path(file).exists() for file in self._list)
 
     def check_order(self, pos='cellcenter', tol=1e-10):
-        mappos = { 'cellcenter' : lambda m: m.cell_centers().points,
-                   'node' : lambda m: m.points }        
+        mappos = {
+            'cellcenter': lambda m: m.cell_centers().points,
+            'node': lambda m: m.points,
+        }
         count = 0
         assert self.nfile > 0
         ref = mappos[pos](pv.read(self._list[0]))
         for name in self._list:
             mesh = pv.read(name)
             d = np.max(maths.distance(ref, mappos[pos](mesh)))
             if d > tol:
@@ -122,43 +147,49 @@
         Tcomp = api.Timer()
         Tsort = api.Timer()
         Tread.start()
         self._mesh = pv.read(self._list[0])
         self._ncell = self._mesh.n_cells
         ctrRef = self._mesh.cell_centers().points
         Tread.pause()
+        if self._verbose:
+            api.io.printstd("> build kd-tree")
         Tsort.start()
         tree = spspa.KDTree(ctrRef)
         Tsort.pause()
         #
         self._data = DataSetList(self.nfile, Xrep='cellaverage', Trep='instant')
         # may add alive-progress or other
+        if self._verbose:
+            api.io.printstd("> read all files, get only CELL data")
+        if filterdata:
+            api.io.printstd(f"  select only {', '.join(filterdata)}")
         for name in self._list:
+            if self._verbose:
+                api.io.printstd(f"  - {name}")
             Tread.start()
             vtk = pv.read(name)
             Tread.pause()
             namelist = filterdata if filterdata else vtk.cell_data.keys()
             Tcomp.start()
             ctr = vtk.cell_centers().points
             d = np.max(maths.distance(ctrRef, ctr))
             Tcomp.pause()
             if d > tol:
                 count += 1
-                #if self._verbose:
-                #    api.io.printstd(f"  . {name}: {d}")
+                # if self._verbose:
+                #     api.io.printstd(f"  . {name}: {d}")
                 Tsort.start()
                 dfinal, index = tree.query(ctr, p=2)
                 # reverse indexing to sort new arrays
                 rindex = index.copy()
-                rindex[index] = np.arange(index.size) 
+                rindex[index] = np.arange(index.size)
                 assert np.max(dfinal) <= tol
                 # automatically deals with differnt shapes
-                datalist = {
-                    name: vtk.cell_data[name][rindex] for name in namelist
-                }
+                datalist = {name: vtk.cell_data[name][rindex] for name in namelist}
                 Tsort.pause()
                 self._data.add_datalist(datalist)
         if self._verbose:
             api.io.printstd(f"  {count}/{self.nfile} grids were not coincident")
             api.io.printstd(f"       file reading: {Tread.elapsed:.2f}s")
             api.io.printstd(f"    grid comparison: {Tcomp.elapsed:.2f}s")
             api.io.printstd(f"    data reordering: {Tsort.elapsed:.2f}s")
@@ -170,8 +201,8 @@
         hmesh = file._h5file.create_group("mesh")
         vtkmesh = vtkMesh(pvmesh=self._mesh)
         vtkmesh.dumhdfgroup(hmesh, **options)
         #
         hdata = file._h5file.create_group("datalist")
         self._data._dumphdfgroup(hdata, **options)
         file.close()
-        
+        return file.filename
```

### Comparing `cfdtools-0.5.0/cfdtools.egg-info/PKG-INFO` & `cfdtools-0.5.1/cfdtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdtools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for mesh and solution management in CFD
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
         Copyright (c) 2022 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cfdtools-0.5.0/cfdtools.egg-info/SOURCES.txt` & `cfdtools-0.5.1/cfdtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/pyproject.toml` & `cfdtools-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cfdtools"
-version = "0.5.0"
+version = "0.5.1"
 description = "Tools for mesh and solution management in CFD"
 authors = [{name="J. Gressier", email="jeremie.gressier@isae-supaero.fr"}]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
@@ -37,14 +37,15 @@
 ic3brief = 'cfdtools._cli:ic3brief'
 ic3probe_plotline = 'cfdtools._cli:ic3probe_plotline'
 cfdwrite_ic3v2 = 'cfdtools._cli:write_ic3v2'
 cfdwrite_ic3v3 = 'cfdtools._cli:write_ic3v3'
 cfdwrite_ic3 = 'cfdtools._cli:write_ic3v3'
 cfdwrite_vtk = 'cfdtools._cli:write_vtk'
 vtkbrief = 'cfdtools._cli:vtkbrief'
+vtkpack = 'cfdtools._cli:vtkpack'
 
 [project.optional-dependencies]
 dev = [ 
     "pytest >= 6.0", 
     "pytest-cov >= 2.11.1",
     "pylint >= 2.6.0" ]
 doc = [ 
@@ -63,15 +64,15 @@
 minversion = "6.0"
 addopts = "--cov -v"
 testpaths = [
     "tests"
 ]
 
 [tool.bumpver]
-current_version = "v0.5.0"
+current_version = "v0.5.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `cfdtools-0.5.0/tests/test_0_connectivity.py` & `cfdtools-0.5.1/tests/test_0_connectivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import cfdtools.meshbase._connectivity as conn
+import cfdtools.meshbase._connectivity as _conn
 import numpy as np
 import pytest
 
 
 def test_indexlist_initlist0():
     ilist = [10, 12, 15, 20]
-    iconn = conn.indexlist()
+    iconn = _conn.indexlist()
     iconn.set_list(ilist)
     assert iconn.list() == ilist
 
 
 def test_indexlist_initlist1():
     ilist = [10, 12, 15, 20]
-    iconn = conn.indexlist(ilist=ilist)
+    iconn = _conn.indexlist(ilist=ilist)
     assert iconn.list() == ilist  # test property
 
 
 def test_indexlist_initrange0():
     imin, imax = 10, 20
-    iconn = conn.indexlist()
+    iconn = _conn.indexlist()
     iconn.set_range([imin, imax])
     assert iconn.range() == [imin, imax]
     assert iconn.list() == list(range(imin, imax + 1))
 
 
 def test_indexindirection_void():
-    dconn = conn.indexindirection()
+    dconn = _conn.indexindirection()
     assert dconn.nelem == 0
 
 
 def test_indexindirection_init():
     i = np.arange(10)
     j = np.arange(10) * 2
-    dconn = conn.indexindirection(array=np.array([i, j]).T)
+    dconn = _conn.indexindirection(array=np.array([i, j]).T)
     assert np.all(dconn.conn[:, 1] == j)
     assert np.all(dconn[:, 1] == j)
 
 
 def test_indexindirection_append():
     i = np.arange(10)
     j = np.arange(10) * 2
-    dconn = conn.indexindirection(array=np.array([i, j]).T)
+    dconn = _conn.indexindirection(array=np.array([i, j]).T)
     i = np.arange(10) + 10
     j = np.arange(10) * 3
     dconn.append(np.array([i, j]).T)
     assert dconn.nelem == 20
 
 
 def test_compressed_listofindex():
     i = np.arange(11) * 3  # 10 elements of 3 values, add last index 30
     v = 100 + np.arange(30)
-    zcon = conn.compressed_listofindex(i, v)
+    zcon = _conn.compressed_listofindex(i, v)
     assert zcon.check()
 
 
 class TestElem:
     dict_basiccon = {
         '2quads': ('quad4', np.array([[0, 1, 2, 3], [2, 1, 4, 5]])),
         '3quadsintri': ('quad4', np.array([[0, 5, 6, 4], [5, 1, 3, 6], [2, 4, 6, 3]])),
         '2hexas': (
             'hexa8',
             np.array([[0, 1, 2, 3, 4, 5, 6, 7], [4, 5, 6, 7, 8, 9, 10, 11]]),
         ),
     }
 
     def set_elemcon(self, econ):
-        elemc = conn.elem_connectivity()
+        elemc = _conn.elem_connectivity()
         elemc.add_elems(*self.dict_basiccon[econ])  # type and connectivy
         return elemc
 
     @pytest.mark.parametrize('econ', ['2quads', '2hexas'])
     def test_elem_init(self, econ):
         elemc = self.set_elemcon(econ)
         assert elemc.check()
@@ -86,18 +86,18 @@
         assert iface2cell.nelem == intfaces.nelem
         assert bface2cell.nelem == boundaryfaces.nelem
 
     @pytest.mark.parametrize('econ', ['3quadsintri', '2hexas'])
     def test_elem_merge(self, econ):
         elemc = self.set_elemcon(econ)
         intfaces, _, boundaryfaces, _ = elemc.create_faces_from_elems()
-        mergedfaces = conn.elem_connectivity()
+        mergedfaces = _conn.elem_connectivity()
         mergedfaces.importfrom_merge((boundaryfaces, intfaces))
         for ec in [boundaryfaces, intfaces, mergedfaces]:
             ec.print()
         mergedfaces.check()
 
     def test_elemtocompress(self):
-        elemc = conn.elem_connectivity()
+        elemc = _conn.elem_connectivity()
         elemc.add_elems(*self.dict_basiccon['2quads'])  # type and connectivy
         zconn = elemc.exportto_compressedindex()
         assert np.all(zconn._index == [0, 4, 8])
```

### Comparing `cfdtools-0.5.0/tests/test_0_polybase.py` & `cfdtools-0.5.1/tests/test_0_polybase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import cfdtools.utils.polybase as poly
 import numpy as np
 import pytest
 
-def test_initlegendre():
-    order = 3
-    b = poly.poly1d(order, series='legendre')
-    assert b._name == 'legendre'
-    assert len(b._basis) == order
-
-def test_initpolynomial():
+@pytest.mark.parametrize('series', ['legendre', 'polynomial'])
+def test_init(series):
     order = 3
-    b = poly.poly1d(3, series='polynomial')
-    assert b._name == 'polynomial'
+    b = poly.poly1d(order, series=series)
+    assert b._name == series
     assert len(b._basis) == order
 
 @pytest.mark.parametrize('series', ['legendre', 'polynomial'])
 def test_consistency(series):
     for order in range(2, 10):
-        b = poly.poly1d(3, series=series)
-        for pos in [-1, 0., .5, 1.]:
-            assert sum(b.interp_weights(pos)) == pytest.approx(1.)
-            assert sum(b.diff_weights(pos)) == pytest.approx(0.)
+        b = poly.poly1d(order, series=series)
+        for pos in [-1.0, 0.0, 0.5, 1.0]:
+            assert sum(b.value_weights(pos)) == pytest.approx(1.0, rel=1e-6)
+            assert sum(b.gradv_weights(pos)) == pytest.approx(0.0, abs=1e-12)
 
-def test_compare_interp():
+def test_compare_value():
     order = 5
-    b1 = poly.poly1d(3, series='legendre')
-    b2 = poly.poly1d(3, series='polynomial')
-    assert np.allclose(b1.interp_weights(-1), b2.interp_weights(-1))
+    b1 = poly.poly1d(order, series='legendre')
+    b2 = poly.poly1d(order, series='polynomial')
+    # interpolation coefficients must be the same, non dependant of poly basis
+    assert np.allclose(b1.value_weights(-1), b2.value_weights(-1))
+    assert b1.value_weights(-1) == pytest.approx(b2.value_weights(-1))
 
-def test_compare_diff():
+def test_compare_gradv():
     order = 5
-    b1 = poly.poly1d(3, series='legendre')
-    b2 = poly.poly1d(3, series='polynomial')
-    # interpolation coefficients must be the same, non dependant of poly basis
-    assert np.allclose(b1.diff_weights(-1), b2.diff_weights(-1))
+    b1 = poly.poly1d(order, series='legendre')
+    b2 = poly.poly1d(order, series='polynomial')
+    # differentiation coefficients must be the same, non dependant of poly basis
+    assert np.allclose(b1.gradv_weights(-1), b2.gradv_weights(-1))
+    assert b1.gradv_weights(-1) == pytest.approx(b2.gradv_weights(-1))
```

### Comparing `cfdtools-0.5.0/tests/test_1_data.py` & `cfdtools-0.5.1/tests/test_1_data.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/tests/test_1_gmsh.py` & `cfdtools-0.5.1/tests/test_1_gmsh.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,42 +15,32 @@
         "box3d-v41.msh",
         "test_2d.msh",
         "test_2d_small.msh",
         "test_3d.msh",
     ],
 )
 def test_reader(filename):
-    gmesh = gmsh.reader(_datadir.joinpath(filename))
+    gmesh = gmsh.reader(_datadir / filename)
     gmesh.read_data()
     rmesh = gmesh.export_mesh()
     assert rmesh.check()
 
 
 @pytest.mark.parametrize(
     "filename",
     [
         "box3d-v22.msh",
         "box3d-v41.msh",
         "test_3d.msh",
     ],
 )
 def test_convert_ic3(filename):
-    gmesh = gmsh.reader(_datadir.joinpath(filename))
+    gmesh = gmsh.reader(_datadir / filename)
     gmesh.read_data()
     rmesh = gmesh.export_mesh()
+    assert rmesh.check()
     ic3write = ic3writer.writer(rmesh)
     _builddir.mkdir(exist_ok=True)
-    outfile = api._files(_builddir / Path(filename))
+    outfile = api._files(_builddir / filename)
     outfile.change_suffix('.ic3')
     ic3write.write_data(outfile.filename)
     Path(outfile.filename).unlink()
-
-
-# def test_reader3dv22():
-#     rmesh = gmsh.reader(_datadir+'box3d-v22.msh')
-#     rmesh = gmshmesh.read_data()
-#     assert rmesh.check()
-
-# def test_reader3dv41():
-#     gmshmesh = gmsh.reader(_datadir+'box3d-v41.msh')
-#     rmesh = gmshmesh.read_data()
-#     assert rmesh.check()
```

### Comparing `cfdtools-0.5.0/tests/test_1_vtk.py` & `cfdtools-0.5.1/tests/test_1_vtk.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
     namelist = list(datadir.glob("cubemixed00*.vtu"))
     vtklist = vtkList(namelist, verbose=True)
     vtklist.read()
     h5filename = builddir / "vtklist.hdf"
     vtklist.dumphdf(h5filename)
     h5file = h5File(h5filename)
     h5file.open()
-    assert h5file.datatype == 'datalist'
+    assert h5file.datatype == 'datalist'
```

### Comparing `cfdtools-0.5.0/tests/test_2_cli.py` & `cfdtools-0.5.1/tests/test_2_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 
 
 def test_vtkbrief(datadir: Path):
     file = "cubemixed0000.vtu"
     assert cli.vtkbrief([str(datadir / file)])
 
 
+def test_vtkpack(datadir: Path):
+    filelist = map(str, sorted(list(datadir.glob("cubemixed*.vtu"))))
+    print(filelist)
+    assert cli.vtkpack(filelist)
+
+
 @pytest.mark.parametrize("args", [["--fmt", "CGNS", "./tests/data/cavity-degen.hdf"]])
 def test_vtkwrite(builddir, args):
     builddir.mkdir(exist_ok=True)
     file1 = cli.write_vtk(outdirlist(args))
     assert file1
     Path(file1).unlink()
```

### Comparing `cfdtools-0.5.0/tests/test_2_convert.py` & `cfdtools-0.5.1/tests/test_2_convert.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.5.0/tests/test_2_data.py` & `cfdtools-0.5.1/tests/test_2_data.py`

 * *Files identical despite different names*

