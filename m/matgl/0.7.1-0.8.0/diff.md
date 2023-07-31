# Comparing `tmp/matgl-0.7.1.tar.gz` & `tmp/matgl-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.7.1.tar", last modified: Tue Jul 11 18:55:56 2023, max compression
+gzip compressed data, was "matgl-0.8.0.tar", last modified: Mon Jul 31 15:11:49 2023, max compression
```

## Comparing `matgl-0.7.1.tar` & `matgl-0.8.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.332251 matgl-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-11 18:55:44.000000 matgl-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-11 18:55:56.328251 matgl-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-11 18:55:44.000000 matgl-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/apps/pes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/data/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/data/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/ext/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/ext/pymatgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/graph/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/matgl/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_atom_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_bond.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_graph_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_three_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/matgl/models/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/_m3gnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/_megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/matgl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)   131200 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/sb_roots.npy
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-11 18:55:44.000000 matgl-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:55:56.332251 matgl-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-11 18:55:44.000000 matgl-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 18:55:44.000000 matgl-0.7.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.167516 matgl-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-31 15:08:34.000000 matgl-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-31 15:11:49.167516 matgl-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-31 15:08:34.000000 matgl-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.143516 matgl-0.8.0/matgl/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.147516 matgl-0.8.0/matgl/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/apps/pes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.147516 matgl-0.8.0/matgl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/data/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.151516 matgl-0.8.0/matgl/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/ext/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/ext/pymatgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.151516 matgl-0.8.0/matgl/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.159516 matgl-0.8.0/matgl/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_atom_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_three_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.163516 matgl-0.8.0/matgl/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/_m3gnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/_megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.167516 matgl-0.8.0/matgl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131200 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/sb_roots.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.147516 matgl-0.8.0/matgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-31 15:08:34.000000 matgl-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:11:49.167516 matgl-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-31 15:08:34.000000 matgl-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.167516 matgl-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 15:08:34.000000 matgl-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 15:08:34.000000 matgl-0.8.0/tests/test_integration.py
```

### Comparing `matgl-0.7.1/LICENSE` & `matgl-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/PKG-INFO` & `matgl-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.7.1
+Version: 0.8.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `matgl-0.7.1/README.md` & `matgl-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/apps/pes.py` & `matgl-0.8.0/matgl/apps/pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/cli.py` & `matgl-0.8.0/matgl/cli.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/config.py` & `matgl-0.8.0/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/data/transformer.py` & `matgl-0.8.0/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/ext/ase.py` & `matgl-0.8.0/matgl/ext/ase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Interfaces to the Atomic Simulation Environment package for dynamic simulations."""
 
 from __future__ import annotations
 
+import collections
 import contextlib
 import io
 import pickle
 import sys
 from typing import TYPE_CHECKING
 
 import numpy as np
+import pandas as pd
 import torch
 from ase import Atoms, units
 from ase.calculators.calculator import Calculator, all_changes
 from ase.constraints import ExpCellFilter
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen, NPTBerendsen
 from ase.md.nvtberendsen import NVTBerendsen
 from ase.optimize.bfgs import BFGS
@@ -252,15 +254,15 @@
 
         return {
             "final_structure": self.ase_adaptor.get_structure(atoms),
             "trajectory": obs,
         }
 
 
-class TrajectoryObserver:
+class TrajectoryObserver(collections.abc.Sequence):
     """Trajectory observer is a hook in the relaxation process that saves the
     intermediate structures.
     """
 
     def __init__(self, atoms: Atoms) -> None:
         """
         Init the Trajectory Observer from a Atoms.
@@ -273,24 +275,37 @@
         self.forces: list[np.ndarray] = []
         self.stresses: list[np.ndarray] = []
         self.atom_positions: list[np.ndarray] = []
         self.cells: list[np.ndarray] = []
 
     def __call__(self) -> None:
         """The logic for saving the properties of an Atoms during the relaxation."""
-        self.energies.append(self.compute_energy())
+        self.energies.append(float(self.atoms.get_potential_energy()))
         self.forces.append(self.atoms.get_forces())
         self.stresses.append(self.atoms.get_stress())
         self.atom_positions.append(self.atoms.get_positions())
         self.cells.append(self.atoms.get_cell()[:])
 
-    def compute_energy(self) -> float:
-        """Calculate the potential energy."""
-        energy = self.atoms.get_potential_energy()
-        return energy
+    def __getitem__(self, item):
+        return self.energies[item], self.forces[item], self.stresses[item], self.cells[item], self.atom_positions[item]
+
+    def __len__(self):
+        return len(self.energies)
+
+    def as_pandas(self) -> pd.DataFrame:
+        """Returns: DataFrame of energies, forces, streeses, cells and atom_positions."""
+        return pd.DataFrame(
+            {
+                "energies": self.energies,
+                "forces": self.forces,
+                "stresses": self.stresses,
+                "cells": self.cells,
+                "atom_positions": self.atom_positions,
+            }
+        )
 
     def save(self, filename: str) -> None:
         """Save the trajectory to file.
 
         Args:
             filename (str): filename to save the trajectory.
         """
```

### Comparing `matgl-0.7.1/matgl/ext/pymatgen.py` & `matgl-0.8.0/matgl/ext/pymatgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,28 +52,27 @@
 
         :param mol: pymatgen molecule object
         :return: (dgl graph, state features)
         """
         natoms = len(mol)
         R = mol.cart_coords
         element_types = self.element_types
-        np.array([site.specie.Z for site in mol])
         weight = mol.composition.weight / len(mol)
         dist = np.linalg.norm(R[:, None, :] - R[None, :, :], axis=-1)
         dists = mol.distance_matrix.flatten()
         nbonds = (np.count_nonzero(dists <= self.cutoff) - natoms) / 2
         nbonds /= natoms
         adj = sp.csr_matrix(dist <= self.cutoff) - sp.eye(natoms, dtype=np.bool_)
         adj = adj.tocoo()
         g, _ = super().get_graph_from_processed_structure(
             structure=mol,
             src_id=adj.row,
             dst_id=adj.col,
-            images=torch.zeros(len(adj.row), 3),
-            lattice_matrix=torch.zeros(1, 3, 3),
+            images=np.zeros((len(adj.row), 3)),
+            lattice_matrix=np.zeros((1, 3, 3)),
             element_types=element_types,
             cart_coords=R,
         )
         state_attr = [weight, nbonds]
         return g, state_attr
```

### Comparing `matgl-0.7.1/matgl/graph/compute.py` & `matgl-0.8.0/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/graph/converters.py` & `matgl-0.8.0/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/graph/data.py` & `matgl-0.8.0/matgl/graph/data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/__init__.py` & `matgl-0.8.0/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_activations.py` & `matgl-0.8.0/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_atom_ref.py` & `matgl-0.8.0/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_basis.py` & `matgl-0.8.0/matgl/layers/_basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         r_c = r.clone()
         r_c[r_c > self.cutoff] = self.cutoff
         roots = SPHERICAL_BESSEL_ROOTS[: self.max_l, : self.max_n]
 
         results = []
         factor = torch.tensor(sqrt(2.0 / self.cutoff**3))
         for i in range(self.max_l):
-            root = torch.tensor(roots[i])
+            root = roots[i].clone().detach()
             func = self.funcs[i]
             func_add1 = self.funcs[i + 1]
             results.append(
                 func(r_c[:, None] * root[None, :] / self.cutoff) * factor / torch.abs(func_add1(root[None, :]))
             )
         return torch.cat(results, axis=1)
```

### Comparing `matgl-0.7.1/matgl/layers/_bond.py` & `matgl-0.8.0/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_core.py` & `matgl-0.8.0/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_embedding.py` & `matgl-0.8.0/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_graph_convolution.py` & `matgl-0.8.0/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/layers/_three_body.py` & `matgl-0.8.0/matgl/layers/_three_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,15 @@
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
         three_cutoff = torch.unsqueeze(three_cutoff, dim=1)  # type: ignore
-        weights = torch.reshape(
-            three_cutoff[torch.stack(list(line_graph.edges()), dim=1).to(torch.int64)], (-1, 2)  # type: ignore
-        )
+        weights = torch.reshape(three_cutoff[torch.stack(list(line_graph.edges()), dim=1)], (-1, 2))  # type: ignore
         weights = torch.prod(weights, axis=-1)  # type: ignore
         basis = basis * weights[:, None]
         new_bonds = scatter_sum(
             basis.to(torch.float32),
             segment_ids=get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
             num_segments=graph.num_edges(),
             dim=0,
```

### Comparing `matgl-0.7.1/matgl/models/_m3gnet.py` & `matgl-0.8.0/matgl/models/_m3gnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
     Computational Science, 2023, 2, 718-728. DOI: 10.1038/s43588-022-00349-3.
 
 """
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 import dgl
 import torch
 from torch import nn
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import (
@@ -45,15 +45,15 @@
 
 logger = logging.getLogger(__file__)
 
 
 class M3GNet(nn.Module, IOMixIn):
     """The main M3GNet model."""
 
-    __version__ = 1
+    __version__ = 2
 
     def __init__(
         self,
         element_types: tuple[str],
         dim_node_embedding: int = 64,
         dim_edge_embedding: int = 64,
         dim_state_embedding: int | None = None,
@@ -70,15 +70,15 @@
         threebody_cutoff: float = 4.0,
         units: int = 64,
         ntargets: int = 1,
         use_smooth: bool = False,
         use_phi: bool = False,
         niters_set2set: int = 3,
         nlayers_set2set: int = 3,
-        field: str = "node_feat",
+        field: Literal["node_feat", "edge_feat"] = "node_feat",
         include_state: bool = False,
         activation_type: str = "swish",
         **kwargs,
     ):
         """
         Args:
             element_types (tuple): list of elements appearing in the dataset
@@ -186,15 +186,17 @@
                 )
                 for _ in range(nblocks)
             }
         )
         if is_intensive:
             input_feats = dim_node_embedding if field == "node_feat" else dim_edge_embedding
             if readout_type == "set2set":
-                self.readout = Set2SetReadOut(num_steps=niters_set2set, num_layers=nlayers_set2set, field=field)
+                self.readout = Set2SetReadOut(
+                    in_feats=input_feats, n_iters=niters_set2set, n_layers=nlayers_set2set, field=field
+                )
                 readout_feats = 2 * input_feats + dim_state_feats if include_state else 2 * input_feats  # type: ignore
             else:
                 self.readout = ReduceReadOut("mean", field=field)  # type: ignore
                 readout_feats = input_feats + dim_state_feats if include_state else input_feats  # type: ignore
 
             dims_final_layer = [readout_feats, units, units, ntargets]
             self.final_layer = MLP(dims_final_layer, activation, activate_last=False)
```

### Comparing `matgl-0.7.1/matgl/models/_megnet.py` & `matgl-0.8.0/matgl/models/_megnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/models/_wrappers.py` & `matgl-0.8.0/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/utils/cutoff.py` & `matgl-0.8.0/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/utils/io.py` & `matgl-0.8.0/matgl/utils/io.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/utils/maths.py` & `matgl-0.8.0/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/utils/sb_roots.npy` & `matgl-0.8.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl/utils/training.py` & `matgl-0.8.0/matgl/utils/training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.1/matgl.egg-info/PKG-INFO` & `matgl-0.8.0/matgl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.7.1
+Version: 0.8.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `matgl-0.7.1/matgl.egg-info/SOURCES.txt` & `matgl-0.8.0/matgl.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 matgl/models/_wrappers.py
 matgl/utils/__init__.py
 matgl/utils/cutoff.py
 matgl/utils/io.py
 matgl/utils/maths.py
 matgl/utils/sb_roots.npy
 matgl/utils/training.py
-tests/test_config.py
+tests/test_config.py
+tests/test_integration.py
```

### Comparing `matgl-0.7.1/pyproject.toml` & `matgl-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -69,22 +69,20 @@
   "PLW0603", # Using the global statement to update variables is discouraged
   "PLW2901", # redefined-loop-name
   "RET504",  # unnecessary-assign
   "SIM105",  # Use contextlib.suppress(OSError) instead of try-except-pass
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
-extend-exclude = ["tests"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
-"maths.py" = ["PERF"]
 "setup.py" = ["D"]
 "tasks.py" = ["D"]
-"tests/**/*" = ["D"]
+"tests/**/*" = ["D", "PERF"]
 "docs/**/*" = ["D"]
 "examples/**/*" = ["D"]
 
 [tool.pytest.ini_options]
 addopts = "--durations=30 --quiet -rXs --color=yes -p no:warnings"
 
 [tool.mypy]
@@ -96,7 +94,24 @@
 [[tool.mypy.overrides]]
 module = ["requests.*", "tabulate.*"]
 ignore_missing_imports = true
 
 [tool.codespell]
 ignore-words-list = "mater,te,nd"
 check-filenames = true
+
+[tool.coverage.run]
+relative_files = true
+
+[tool.coverage.report]
+exclude_lines = [
+  "@deprecated",
+  "def __repr__",
+  "if 0:",
+  "if __name__ == .__main__.:",
+  "if self.debug:",
+  "if settings.DEBUG",
+  "pragma: no cover",
+  "raise AssertionError",
+  "raise NotImplementedError",
+  "input"
+]
```

### Comparing `matgl-0.7.1/setup.py` & `matgl-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.7.1",
+    version="0.8.0",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

