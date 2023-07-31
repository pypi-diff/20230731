# Comparing `tmp/CircuitCalculator-0.0.9.tar.gz` & `tmp/CircuitCalculator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircuitCalculator-0.0.9.tar", last modified: Wed Apr  5 14:53:27 2023, max compression
+gzip compressed data, was "CircuitCalculator-0.1.0.tar", last modified: Mon Jul 31 12:34:50 2023, max compression
```

## Comparing `CircuitCalculator-0.0.9.tar` & `CircuitCalculator-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.190033 CircuitCalculator-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:53:27.190033 CircuitCalculator-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.182033 CircuitCalculator-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/EquivalentSources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/labelmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/supernodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/NodalAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/PlottingTemplates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Display.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:49.996682 CircuitCalculator-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:49.996682 CircuitCalculator-0.1.0/src/CircuitCalculator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.000682 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/impedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Circuit/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.000682 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/NodalAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/equivalent_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/labelmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/supernodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Network/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/PlottingTemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.000682 CircuitCalculator-0.1.0/src/CircuitCalculator/SignalProcessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SignalProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SignalProcessing/periodic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SignalProcessing/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.000682 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/plot_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/Display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/Elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/DIN/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/DIN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/DIN/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/styles/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/src/CircuitCalculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:49.996682 CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-31 12:34:49.000000 CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-31 12:34:49.000000 CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:34:49.000000 CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 12:34:49.000000 CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 12:34:49.000000 CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:34:50.004682 CircuitCalculator-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-31 12:34:40.000000 CircuitCalculator-0.1.0/tests/test_integration.py
```

### Comparing `CircuitCalculator-0.0.9/LICENSE` & `CircuitCalculator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.9/PKG-INFO` & `CircuitCalculator-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.0.9
+Version: 0.1.0
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CircuitCalculator
```

### Comparing `CircuitCalculator-0.0.9/README.md` & `CircuitCalculator-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/elements.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Network/elements.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Protocol, TypedDict
+from typing import Protocol
 from dataclasses import dataclass
 import numpy as np
 
 class NortenTheveninElement(Protocol):
     @property
     def name(self) -> str:
         """Name of element"""
@@ -12,40 +12,40 @@
         """Impedance value of element"""
         ...
     @property
     def Y(self) -> complex:
         """Admittance value of element"""
         ...
     @property
-    def U(self) -> complex:
+    def V(self) -> complex:
         """Voltage value of element"""
         ...
     @property
     def I(self) -> complex:
         """Current value of element"""
         ...
 
 @dataclass(frozen=True)
 class NortenElement:
     name : str
     type : str
     Z : complex
-    U : complex
+    V : complex
 
     @property
     def Y(self) -> complex:
         try:
             return 1/self.Z
         except ZeroDivisionError:
             return np.inf
 
     @property
     def I(self) -> complex:
         try:
-            return self.U/self.Z
+            return complex(self.V)/self.Z
         except ZeroDivisionError:
             return np.nan
 
 @dataclass(frozen=True)
 class TheveninElement:
     name : str
     type : str
@@ -56,49 +56,49 @@
     def Z(self) -> complex:
         try:
             return 1/self.Y
         except ZeroDivisionError:
             return np.inf
 
     @property
-    def U(self) -> complex:
+    def V(self) -> complex:
         try:
-            return self.I/self.Y
+            return complex(self.I)/self.Y
         except ZeroDivisionError:
             return np.nan
 
 def impedance(name : str, Z : complex) -> NortenTheveninElement:
-    return NortenElement(Z=Z, U=0, name=name, type='impedance')
+    return NortenElement(Z=Z, V=0, name=name, type='impedance')
 
 def admittance(name : str, Y : complex) -> NortenTheveninElement:
     return TheveninElement( Y=Y, I=0, name=name, type='admittance')
 
 def resistor(name : str, R : float) -> NortenTheveninElement:
-    return NortenElement(Z=R, U=0, name=name, type='resistor')
+    return NortenElement(Z=R, V=0, name=name, type='resistor')
 
 def conductor(name : str, G : float) -> NortenTheveninElement:
     return TheveninElement(Y=G, I=0, name=name, type='conductor')
 
 def linear_current_source(name : str, I : complex, Y : complex) -> NortenTheveninElement:
     return TheveninElement(I=I, Y=Y, name=name, type='linear_current_source')
 
 def current_source(name : str, I : complex) -> NortenTheveninElement:
     return TheveninElement(I=I, Y=0, name=name, type='current_source')
 
-def linear_voltage_source(name : str, U : complex, Z : complex) -> NortenTheveninElement:
-    return NortenElement(U=U, Z=Z, name=name, type='linear_voltage_source')
+def linear_voltage_source(name : str, V : complex, Z : complex) -> NortenTheveninElement:
+    return NortenElement(V=V, Z=Z, name=name, type='linear_voltage_source')
 
-def voltage_source(name : str, U : complex) -> NortenTheveninElement:
-    return NortenElement(U=U, Z=0, name=name, type='voltage_source')
+def voltage_source(name : str, V : complex) -> NortenTheveninElement:
+    return NortenElement(V=V, Z=0, name=name, type='voltage_source')
 
 def open_circuit(name : str) -> NortenTheveninElement:
     return TheveninElement(I=0, Y=0, name=name, type='open_circuit')
 
 def short_cicruit(name : str) -> NortenTheveninElement:
-    return NortenElement(U=0, Z=0, name=name, type='short_circuit')
+    return NortenElement(V=0, Z=0, name=name, type='short_circuit')
 
 def impedance_value(R : float = 0.0, X : float = 0.0, absZ : float = -1.0, phi : float = 0.0, degree : bool = False) -> complex:
     if degree:
         phi *= np.pi/180
     if absZ > 0:
         return complex(absZ*np.cos(phi), absZ*np.sin(phi))
     return complex(R, X)
@@ -116,15 +116,15 @@
     if deg:
         phi = np.radians(phi)
     if not np.isfinite(X):
         return complex(np.inf, 0)
     return X*complex(np.cos(phi), np.sin(phi))
 
 def is_voltage_source(element: NortenTheveninElement) -> bool:
-    return np.abs(element.U) > 0
+    return np.abs(element.V) > 0
 
 def is_current_source(element: NortenTheveninElement) -> bool:
     return np.abs(element.I) > 0
 
 def is_ideal_voltage_source(element: NortenTheveninElement) -> bool:
     return is_voltage_source(element) and element.Z==0
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/loaders.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Network/loaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from typing import Any, Callable
 from .network import Network, Branch
-from .elements import NortenTheveninElement
 from . import elements as elm
 import numpy as np
 
 class FileFormatError(Exception):
     ...
 
 def to_complex(z: dict[str, float], degree: bool = False) -> complex:
     try:
         return complex(z['real'], z['imag'])
-    except KeyError:
+    except (KeyError, TypeError):
         ...
     try:
         if degree:
             z['phase'] *= np.pi/180
         return z['abs']*complex(np.cos(z['phase']), np.sin(z['phase']))
-    except KeyError:
+    except (KeyError, TypeError):
         raise FileFormatError
 
 def translate_to_complex(keys : list[str], **kwargs):
     for value in keys:
         kwargs.update({value : to_complex(kwargs[value])})
     return kwargs
 
-network_branch_translators : dict[str, Callable[..., NortenTheveninElement]] = {
+network_branch_translators : dict[str, Callable[..., elm.NortenTheveninElement]] = {
     "resistor" : elm.resistor,
     "conductor" : elm.conductor,
-    "impedance" : lambda **kwargs: elm.impedance(Z=to_complex(kwargs['Z']), **kwargs),
+    "impedance" : lambda **kwargs: elm.impedance(Z=to_complex(kwargs.pop('Z')), **kwargs),
     "admittance" : lambda **kwargs: elm.admittance(Y=to_complex(kwargs['Y']), **kwargs),
     "linear_current_source" : lambda **kwargs: elm.linear_current_source(**translate_to_complex(keys=['I', 'Y'], **kwargs)),
-    "current_source" : lambda **kwargs: elm.current_source(I=to_complex(kwargs['I']), **kwargs),
+    "current_source" : lambda **kwargs: elm.current_source(I=to_complex(kwargs.pop('I')), **kwargs),
     "real_current_source" : elm.current_source,
-    "linear_voltage_source" : lambda **kwargs: elm.linear_voltage_source(U=to_complex(kwargs['U']), Z=to_complex(kwargs['Z']), **kwargs),
-    "voltage_source" : lambda **kwargs: elm.voltage_source(U=to_complex(kwargs['U']), **kwargs),
+    "linear_voltage_source" : lambda **kwargs: elm.linear_voltage_source(V=to_complex(kwargs.pop('V')), Z=to_complex(kwargs.pop('Z')), **kwargs),
+    "voltage_source" : lambda **kwargs: elm.voltage_source(V=to_complex(kwargs.pop('V')), **kwargs),
     "real_voltage_source" : elm.voltage_source,
 }
 
 def load_network(network_dict: list[dict[str, Any]]) -> Network:
     def entry_to_branch(entry: dict[str, Any]) -> Branch:
         n1 = entry.pop('N1')
         n2 = entry.pop('N2')
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/network.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Network/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,38 +14,40 @@
     @property
     def id(self) -> str:
         return self.element.name
 
 @dataclass(frozen=True)
 class Network:
     branches: list[Branch]
-    zero_node_label: str = '0'
+    node_zero_label: str = '0'
 
     def __post_init__(self):
-        if self.zero_node_label not in self.node_labels:
+        if self.node_zero_label not in self.node_labels and self.number_of_nodes != 0:
             raise FloatingGroundNode
         if len(set(self.branch_ids)) != len(self.branches):
             raise AmbiguousBranchIDs
         
     @property
     def branch_ids(self) -> list[str]:
         return [b.id for b in self.branches]
 
     @property
     def node_labels(self) -> list[str]:
+        if len(self.branches) == 0:
+            return [self.node_zero_label]
         node1_set = {branch.node1 for branch in self.branches}
         node2_set = {branch.node2 for branch in self.branches}
         return sorted(list(node1_set.union(node2_set)))
 
     @property
     def number_of_nodes(self) -> int:
         return len(self.node_labels)
 
     def is_zero_node(self, node: str) -> bool:
-        return node == self.zero_node_label
+        return node == self.node_zero_label
 
     def branches_connected_to(self, node: str) -> list[Branch]:
         connected_branches = [branch for branch in self.branches if branch.node1 == node or branch.node2 == node]
         connected_branches.sort(key=lambda x: x.node1 if x.node1!=node else x.node2)
         return connected_branches
 
     def nodes_connected_to(self, node: str) -> set[str]:
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/supernodes.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Network/supernodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             if network.is_zero_node(node) or node in self.active_nodes:
                 raise AmbiguousElectricalPotential
             self.voltage_sources.append(voltage_source.element)
             self._super_nodes.append(
                 SuperNode(
                     reference_node=other_node,
                     active_node=node,
-                    voltage=voltage_source.element.U if node == voltage_source.node1 else -voltage_source.element.U,
+                    voltage=voltage_source.element.V if node == voltage_source.node1 else -voltage_source.element.V,
                     voltage_source=voltage_source.element
                 )
             )
 
     @property
     def active_nodes(self) -> list[str]:
         return [sn.active_node for sn in self._super_nodes]
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/transformers.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Network/transformers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from .network import Network, Branch
 from .elements import NortenTheveninElement, is_ideal_current_source, is_ideal_voltage_source
 from .supernodes import SuperNodes
 
 def switch_ground_node(network: Network, new_ground: str) -> Network:
     return Network(network.branches, new_ground)
 
+def remove_element(network: Network, element: str) -> Network:
+    branches = list(network.branches)
+    branches.remove(network[element])
+    return Network(branches)
+
 def remove_ideal_current_sources(network: Network, keep: list[NortenTheveninElement] = []) -> Network:
-    return Network([b for b in network.branches if not is_ideal_current_source(b.element) or b.element in keep], zero_node_label=network.zero_node_label)
+    return Network([b for b in network.branches if not is_ideal_current_source(b.element) or b.element in keep], node_zero_label=network.node_zero_label)
 
 def remove_ideal_voltage_sources(network: Network, keep: list[NortenTheveninElement] = []) -> Network:
     branches = network.branches
     super_nodes = SuperNodes(network)
     voltage_sources = [b for b in network.branches if is_ideal_voltage_source(b.element)]
     voltage_sources = [vs for vs in voltage_sources if vs.element not in keep]
     short_circuit_nodes = [(vs.node1, vs.node2) if super_nodes.is_active(vs.node1) else (vs.node2, vs.node1) for vs in voltage_sources]
     for an, rn in short_circuit_nodes:
         branches = [Branch(rn, b.node2, b.element) if b.node1 == an else b for b in branches]
         branches = [Branch(b.node1, rn, b.element) if b.node2 == an else b for b in branches]
         branches = [b for b in branches if b.node1 != b.node2]
-    return Network(branches, zero_node_label=network.zero_node_label)
+    return Network(branches, node_zero_label=network.node_zero_label)
 
 def passive_network(network: Network, keep: list[NortenTheveninElement] = []) -> Network:
     return remove_ideal_voltage_sources(remove_ideal_current_sources(network, keep=keep), keep=keep)
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/NodalAnalysis.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Network/NodalAnalysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,99 @@
 import numpy as np
-from .Network.network import Network
-from .Network.elements import is_ideal_current_source, is_ideal_voltage_source, is_current_source
-from .Network.transformers import passive_network
-from .Network.supernodes import SuperNodes
-from .Network import labelmapper as map
-from .Network.solution import NetworkSolution
+from .network import Network
+from .elements import is_ideal_current_source, is_ideal_voltage_source, is_current_source, is_voltage_source
+from .supernodes import SuperNodes
+from . import labelmapper as map
+from . import transformers as trf
+from .solution import NetworkSolution
 import itertools
 
-class DimensionError(Exception): pass
+class DimensionError(Exception):
+    ...
 
 def admittance_connected_to(network: Network, node: str) -> complex:
     return sum(b.element.Y for b in network.branches_connected_to(node) if np.isfinite(b.element.Y))
 
 def admittance_between(network: Network, node1: str, node2: str) -> complex:
     return sum([b.element.Y for b in network.branches_between(node1, node2) if np.isfinite(b.element.Y)])
 
+def connected_nodes(network: Network, node: str) -> list[str]:
+    return [b.node1 if b.node1 != node else b.node2 for b in network.branches_connected_to(node)]
+
 def create_node_matrix_from_network(network: Network, node_index_mapper: map.NodeIndexMapper = map.default) -> np.ndarray:
-    super_nodes = SuperNodes(network)
-    passive_net = passive_network(network)
-    node_mapping = node_index_mapper(network)
-    A = np.zeros((network.number_of_nodes-1, network.number_of_nodes-1), dtype=complex)
-    def passive_node_pair(node1: str, node2: str) -> bool:
-        return not super_nodes.is_active(node1) and not super_nodes.is_active(node2)
-    def both_active(node1: str, node2: str) -> bool:
-        return super_nodes.is_active(node1) and super_nodes.is_active(node2)
-    def passive_matrix_element(node1: str, node2: str) -> complex:
-        if node1 == node2:
-            return admittance_connected_to(passive_net, node1)
-        else:
-            return -admittance_between(passive_net, node1, node2)
-    def non_active_j_label() -> complex:
-        Aij = -admittance_between(network, i_label, j_label)
-        if super_nodes.is_reference(j_label):
-            Aij -= admittance_between(network, i_label, super_nodes.get_active_node(j_label))
-        if super_nodes.belong_to_same(i_label, j_label):
-            Aij += admittance_connected_to(network, i_label)
-        return Aij
-    def matrix_element(i_label: str, j_label: str) -> complex:
-        if passive_node_pair(i_label, j_label):
-            return passive_matrix_element(i_label, j_label)
+    def node_matrix_element(i_label:str, j_label:str) -> complex:
         if i_label == j_label:
-            return -super_nodes.sign(i_label)
-        if both_active(i_label, j_label) and super_nodes.belong_to_same(j_label, i_label):
-            return super_nodes.sign(j_label)
-        if not super_nodes.is_active(j_label):
-            return non_active_j_label()
-        return 0+0j
+            return admittance_connected_to(passive_net, i_label)
+        return -admittance_between(passive_net, i_label, j_label)
+    passive_net = trf.passive_network(network)
+    node_mapping = node_index_mapper(network)
+    A = np.zeros((len(node_mapping), len(node_mapping)), dtype=complex)
     for (i_label, i), (j_label, j) in itertools.product(node_mapping.items(), repeat=2):
-        A[i, j] = matrix_element(i_label, j_label)
+        A[i, j] = node_matrix_element(i_label, j_label)
     return A
 
 def create_current_vector_from_network(network: Network, node_index_mapper: map.NodeIndexMapper = map.default) -> np.ndarray:
     super_nodes = SuperNodes(network)
-    b = np.zeros(network.number_of_nodes-1, dtype=complex)
     node_mapping = node_index_mapper(network)
-    active_node_labels = [l for l in node_mapping.keys() if super_nodes.is_active(l)]
+    reference_node_mapping = {n: i for n, i in node_mapping.items() if super_nodes.is_reference(n)}
+    b = np.zeros(len(node_mapping), dtype=complex)
     def current_sources(node: str) -> complex:
         current_sources = [b for b in network.branches_connected_to(node) if is_current_source(b.element)]
         return sum([-cs.element.I if cs.node1 == node else cs.element.I for cs in current_sources])
-    def connected_active_nodes(active_node: str) -> list[str]:
-        return [n for n in network.nodes_connected_to(active_node) if super_nodes.is_active(n)]
-    def active_node_current(active_node: str) -> complex:
-        I_connected_admittances = super_nodes.voltage_to_next_reference(active_node)*admittance_connected_to(network, active_node)
-        reference_node = super_nodes.get_reference_node(active_node)
-        if super_nodes.is_active(reference_node):
-            I_parallel_admittance = super_nodes.voltage_to_next_reference(reference_node)*admittance_between(network, active_node, reference_node)
-            return I_parallel_admittance-I_connected_admittances
-        return sum([super_nodes.voltage_to_next_reference(cn)*admittance_between(network, active_node, cn) for cn in connected_active_nodes(active_node)])-I_connected_admittances
-    def passive_node_current(passive_node: str) -> complex:
-        I_parallel_admittances = sum([super_nodes.voltage_to_next_reference(an)*admittance_between(network, an, passive_node) for an in active_node_labels if super_nodes.get_reference_node(an) != passive_node])
-        if super_nodes.is_reference(passive_node):
-            active_node = super_nodes.get_active_node(passive_node)
-            I_connected_admittances = super_nodes.voltage_to_next_reference(active_node)*admittance_connected_to(network, active_node)
-            I_parallel_to_active_nodes = sum([super_nodes.voltage_to_next_reference(cn)*admittance_between(network, active_node, cn) for cn in connected_active_nodes(active_node)])
-            I_parallel_to_passive_nodes = super_nodes.voltage_to_next_reference(active_node)*admittance_between(network, active_node, passive_node)
-            return I_parallel_admittances+I_parallel_to_active_nodes+I_parallel_to_passive_nodes-I_connected_admittances
-        return I_parallel_admittances
-    def current_of_voltage_sources(node: str) -> complex:
-        if super_nodes.is_active(node):
-            return active_node_current(node)
-        return passive_node_current(node)
+    def currents_of_connected_active_nodes(node: str) -> complex:
+        connected_active_nodes = {n for n in connected_nodes(network, node) if super_nodes.is_active(n)}
+        connected_active_nodes = {n for n in connected_active_nodes if not super_nodes.belong_to_same(n, node)}
+        return sum([super_nodes.voltage_to_next_reference(cn)*admittance_between(network, cn, node) for cn in connected_active_nodes])
+    def currents_of_belonging_voltage_sources(reference_node: str) -> complex:
+        an = super_nodes.get_active_node(reference_node)
+        connected_admittances_without_parallel_one = admittance_connected_to(network, an)-admittance_between(network, an, reference_node)
+        return -super_nodes.voltage_to_next_reference(an)*connected_admittances_without_parallel_one
     for i_label, i in node_mapping.items():
-        b[i] = current_sources(i_label) + current_of_voltage_sources(i_label)
+        b[i] = current_sources(i_label)
+        b[i] += currents_of_connected_active_nodes(i_label)
+    for ref_label, i in reference_node_mapping.items():
+        b[i] += current_sources(super_nodes.get_active_node(ref_label))
+        b[i] += currents_of_connected_active_nodes(super_nodes.get_active_node(ref_label))
+        b[i] += currents_of_belonging_voltage_sources(ref_label)
     return b
+        
+def open_circuit_impedance(network: Network, node1: str, node2: str, node_index_mapper: map.NodeIndexMapper = map.default) -> complex:
+    if node1 == node2:
+        return 0
+    if any([is_ideal_voltage_source(b.element) for b in network.branches_between(node1, node2)]):
+        return 0
+    if network.is_zero_node(node1):
+        node1, node2 = node2, node1
+    network = trf.switch_ground_node(network=network, new_ground=node2)
+    network = trf.passive_network(network)
+    Y = create_node_matrix_from_network(network, node_index_mapper=node_index_mapper)
+    Z = np.linalg.inv(Y)
+    i1 = node_index_mapper(network)[node1]
+    return Z[i1][i1]
+
+def element_impedance(network: Network, element: str, node_index_mapper: map.NodeIndexMapper = map.default) -> complex:
+    return open_circuit_impedance(
+        network=trf.remove_element(network, element),
+        node1=network[element].node1,
+        node2=network[element].node2,
+        node_index_mapper=node_index_mapper
+    )
+
+def open_circuit_voltage(network: Network, node1: str, node2: str) -> complex:
+    if node1 == node2:
+        return 0
+    solution = NodalAnalysisSolution(network)
+    phi1 = solution.get_potential(node=node1)
+    phi2 = solution.get_potential(node=node2)
+    return phi1-phi2
+
+def short_circuit_current(network: Network, node1: str, node2: str) -> complex:
+    Z = open_circuit_impedance(network, node1, node2)
+    V = open_circuit_voltage(network, node1, node2)
+    return V/Z
 
 def calculate_node_voltages(Y : np.ndarray, I : np.ndarray) -> np.ndarray:
     if np.any(np.logical_not(np.isfinite(Y))):
         raise ValueError
     if np.any(np.logical_not(np.isfinite(I))):
         raise ValueError
     if Y.ndim != 2:
@@ -99,41 +106,57 @@
     return np.linalg.solve(Y, I)
 
 class NodalAnalysisSolution:
     def __init__(self, network : Network, node_mapper: map.NodeIndexMapper = map.default) -> None:
         Y = create_node_matrix_from_network(network, node_index_mapper=node_mapper)
         I = create_current_vector_from_network(network, node_index_mapper=node_mapper)
         self._network = network
-        self._solution_vector = calculate_node_voltages(Y, I)
         self._super_nodes = SuperNodes(network)
         self._node_mapping = node_mapper(network)
+        try:
+            self._solution_vector = calculate_node_voltages(Y, I)
+        except np.linalg.LinAlgError:
+            self._solution_vector = np.zeros(np.size(I))
+        if np.any(np.isnan(self._solution_vector)):
+            self._solution_vector = np.zeros(np.size(I))
+
+    def _select_active_node(self, branch_id: str) -> str:
+        branch = self._network[branch_id]
+        if self._super_nodes.is_active(branch.node1):
+            return branch.node1
+        return branch.node2
 
-    def _calculate_potential_of_node(self, node: str) -> complex:
+    def get_potential(self, node: str) -> complex:
         V_active = 0+0j
         if self._super_nodes.is_active(node):
             V_active = self._super_nodes.voltage_to_next_reference(node)
             node = self._super_nodes.next_reference(node)
         if self._network.is_zero_node(node):
             return V_active
         return self._solution_vector[self._node_mapping[node]] + V_active
-
-    def _select_active_node(self, branch_id: str) -> str:
-        branch = self._network[branch_id]
-        if self._super_nodes.is_active(branch.node1):
-            return branch.node1
-        return branch.node2
     
     def get_voltage(self, branch_id: str) -> complex:
-        phi1 = self._calculate_potential_of_node(self._network[branch_id].node1)
-        phi2 = self._calculate_potential_of_node(self._network[branch_id].node2)
+        phi1 = self.get_potential(self._network[branch_id].node1)
+        phi2 = self.get_potential(self._network[branch_id].node2)
         return phi1-phi2
 
     def get_current(self, branch_id: str) -> complex:
-        branch_element = self._network[branch_id].element
-        if is_ideal_current_source(branch_element):
-            return branch_element.I
-        if is_ideal_voltage_source(branch_element):
-            return self._solution_vector[self._node_mapping[self._select_active_node(branch_id)]]
-        return self.get_voltage(branch_id)/branch_element.Z
+        branch = self._network[branch_id]
+        if is_ideal_current_source(branch.element):
+            return branch.element.I
+        if is_ideal_voltage_source(branch.element):
+            Z = element_impedance(self._network, branch_id)
+            I_branch_element = -branch.element.V/Z
+            I_other_elements = short_circuit_current(
+                trf.remove_element(self._network, branch_id),
+                branch.node1,
+                branch.node2)
+            return  I_branch_element+I_other_elements
+        if is_voltage_source(branch.element):
+            return -(self.get_voltage(branch_id)+branch.element.V)/branch.element.Z
+        return self.get_voltage(branch_id)/branch.element.Z
+
+    def get_power(self, branch_id: str) -> complex:
+        return self.get_voltage(branch_id)*self.get_current(branch_id).conjugate()
 
-def nodal_analysis_solver(network) -> NetworkSolution:
+def nodal_analysis_solver(network: Network) -> NetworkSolution:
     return NodalAnalysisSolution(network)
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/PlottingTemplates.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/PlottingTemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
 import numpy as np
 from functools import partial
 from CircuitCalculator.Utils import scientific_float
-from CircuitCalculator.EquivalentSources import NortenEquivalentSource, TheveninEquivalentSource
+from CircuitCalculator.Network.EquivalentSources import NortenEquivalentSource, TheveninEquivalentSource
 
 def plot_equivalent_source_diagram(x0: float, y0: float, xlabel: str, ylabel: str, m2: float = 0, title: str = '', x0label: str = '', y0label: str = '') -> tuple[Figure, Axes]:
     fig, ax = plt.subplots()
     ax.plot([0, x0], [y0, 0], linewidth=2)
     ax.grid(visible=True)
     ax.set_xlim(left=0, right=ax.get_xticks()[-1])
     ax.set_ylim(bottom=0, top=ax.get_yticks()[-1])
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Elements.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleAnalysis/plot_elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,9 +57,15 @@
     if tail:
         xy0[0]+=height*np.cos(alpha)/aspect
         xy0[1]+=height*np.sin(alpha)/aspect
     xy1[0]-=height*np.cos(alpha)/aspect
     xy1[1]-=height*np.sin(alpha)/aspect
     ax.plot([xy0[0], xy1[0]], [xy0[1], xy1[1]], color=color, **kwargs)
 
-def complex_pointer(ax: Axes, z0, z1, **kwargs) -> None:
-    arrow(ax, [np.real(z0), np.imag(z0)], [np.real(z1), np.imag(z1)], **kwargs)
+def complex_pointer(ax: Axes, z0, z1, width=0.05, height=0.05, **kwargs) -> None:
+    xlim, ylim = ax.get_xlim(), ax.get_ylim()
+    delta_x, delta_y = xlim[1]-xlim[0], ylim[1]-ylim[0]
+    max_stretch = max(delta_x, delta_y)
+    width *= max_stretch
+    height *= max_stretch
+    if z0 != z1:
+        arrow(ax, [np.real(z0), np.imag(z0)], [np.real(z1), np.imag(z1)], width, height, **kwargs)
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,40 @@
+from ..Network import network as ntw
+from ..Network import elements as ntw_elm
+
 from . import Elements as elm
-from ..Circuit import components
 from .SchemdrawTranslatorTypes import ElementTranslatorMap
-import numpy as np
 
 
-def resistor_translator(element: elm.Resistor, nodes: tuple[str, str]) -> components.Resistor:
-    return components.Resistor(nodes=nodes, id=element.name, R=element.R)
+def linear_current_source_translator(element: elm.RealCurrentSource, nodes: tuple[str, str]) -> ntw.Branch:
+    return ntw.Branch(nodes[0], nodes[1], ntw_elm.linear_current_source(I=element.I, Y=1/element.R, name=element.name))
 
-def current_source_translator(element: elm.CurrentSource, nodes: tuple[str, str]) -> components.CurrentSource:
-    return components.CurrentSource(nodes=nodes, id=element.name, I=element.I)
+def resistor_translator(element: elm.Resistor, nodes: tuple[str, str]) -> ntw.Branch:
+    return ntw.Branch(nodes[0], nodes[1], ntw_elm.resistor(R=element.R, name=element.name))
 
-def voltage_source_translator(element: elm.VoltageSource, nodes: tuple[str, str]) -> components.VoltageSource:
-    return components.VoltageSource(nodes=nodes, id=element.name, V=element.V)
+def impedance_translator(element: elm.Resistor, nodes: tuple[str, str]) -> ntw.Branch:
+    return ntw.Branch(nodes[0], nodes[1], ntw_elm.impedance(Z=element.Z, name=element.name))
 
-def capacitor_translator(element: elm.Capacitor, nodes: tuple[str, str]) -> components.Capacitor:
-    return components.Capacitor(nodes=nodes, id=element.name, C=element.C)
+def current_source_translator(element: elm.CurrentSource, nodes: tuple[str, str]) -> ntw.Branch:
+    return ntw.Branch(nodes[0], nodes[1], ntw_elm.current_source(I=element.I, name=element.name))
 
-def inductance_translator(element: elm.Inductance, nodes: tuple[str, str]) -> components.Inductance:
-    return components.Inductance(nodes=nodes, id=element.name, L=element.L)
+def linear_voltage_source_translator(element: elm.RealVoltageSource, nodes: tuple[str, str]) -> ntw.Branch:
+    return ntw.Branch(nodes[0], nodes[1], ntw_elm.linear_voltage_source(V=-element.V, Z=element.R, name=element.name))
 
-def ground_translator(element: elm.Ground, nodes: tuple[str]) -> components.Ground:
-    return components.Ground(nodes=nodes, id=element.name)
+def voltage_source_translator(element: elm.VoltageSource, nodes: tuple[str, str]) -> ntw.Branch:
+    return ntw.Branch(nodes[0], nodes[1], ntw_elm.voltage_source(V=-element.V, name=element.name))
 
-def ac_voltage_source_translator(element: elm.ACVoltageSource, nodes: tuple[str, str]) -> components.VoltageSource:
-    return components.VoltageSource(
-        nodes=nodes,
-        id=element.name,
-        V=element.V,
-        w=element.w,
-        phi=element.phi*np.pi/180 if element.deg else element.phi
-    )
+def none_translator(*_) -> None:
+    return None
 
-circuit_translator_map : ElementTranslatorMap = {
+network_translator_map : ElementTranslatorMap = {
     elm.Resistor : resistor_translator,
-    elm.CurrentSource : current_source_translator,
-    elm.VoltageSource : voltage_source_translator,
-    elm.Capacitor : capacitor_translator,
-    elm.Inductance : inductance_translator,
-    elm.Ground : ground_translator,
-    elm.ACVoltageSource : ac_voltage_source_translator,
+    elm.Impedance : impedance_translator,
+    elm.CurrentSource: current_source_translator,
+    elm.VoltageSource: voltage_source_translator,
+    elm.RealCurrentSource: linear_current_source_translator,
+    elm.RealVoltageSource: linear_voltage_source_translator,
+    elm.Line: none_translator,
+    elm.Node: none_translator,
+    elm.LabelNode: none_translator,
+    elm.Ground: none_translator,
 }
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Elements.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/SimpleCircuit/Elements.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,212 @@
-import schemdraw
-import schemdraw.elements
-from .Display import red, blue, print_voltage, print_current
+import schemdraw, schemdraw.elements, schemdraw.util
+from . import schemdraw_element_extension as extension
+
+from . import Display as dsp
+
+import numpy as np
+
 from typing import Any
-from ..Utils import ScientificFloat, ScientificComplex
+from enum import Enum
+from abc import ABC
+
+def round_node(node: schemdraw.util.Point) -> schemdraw.util.Point:
+    def local_round(x):
+        return round(x, ndigits=2)
+    return schemdraw.util.Point((local_round(node.x), local_round(node.y)))
+
+def get_nodes(element: schemdraw.elements.Element, n_labels: tuple[str, ...]=('start', 'end')) -> list[schemdraw.util.Point]:
+    try:
+        return [round_node(element.absanchors[n_label]) for n_label in n_labels]
+    except KeyError:
+        return []
+
+def get_node_direction(node1: schemdraw.util.Point, node2: schemdraw.util.Point) -> tuple[int, int]:
+    delta = node2 - node1
+    delta_x = +1 if delta.x >= 0 else -1
+    delta_y = +1 if delta.y >= 0 else -1
+    return delta_x, delta_y
+
+def is_reverse(element: schemdraw.elements.Element) -> bool:
+    n1, n2 = get_nodes(element)
+    dx, dy = get_node_direction(n1, n2)
+    if dx < 0 or dy < 0:
+        return True
+    return False
 
 def segments_of(element: schemdraw.elements.Element) -> list[schemdraw.segments.SegmentType]:
     return element.segments
 
+class SwitchState(Enum):
+    OPEN = False
+    CLOSED = True
+
 class Schematic(schemdraw.Drawing):
     def __init__(self, unit=7, **kwargs):
         super().__init__(unit=unit, **kwargs)
 
+    def __getitem__(self, id: str) -> schemdraw.elements.Element:
+        names = [e.name for e in self.elements if hasattr(e, 'name')]
+        try:
+            index = names.index(id)
+        except ValueError:
+            raise KeyError
+        return self.elements[index]
+
+    def clear_labels(self) -> None:
+        self.elements = [e for e in self.elements if not isinstance(e, VoltageLabel) and not isinstance(e, CurrentLabel)]
+
+    def draw(self, *args, **kwargs):
+        if self.fig is not None:
+            self.fig.clear()
+        return super().draw(*args, **kwargs)
+
     def save_copy(self, fname: str, **kwargs) -> None:
         import copy
         cpy = copy.deepcopy(self)
         cpy.save(fname, **kwargs)
 
-class VoltageSource(schemdraw.elements.sources.Source):
-    def __init__(self, V: complex, name: str, *args, reverse=False, precision=3, **kwargs):
-        super().__init__(*args, reverse=reverse, **kwargs)
-        if reverse:
-            self._V = -V
-        else:
-            self._V = V
+class SimpleAnalysisElement(ABC):
+    def __init__(self, *, name: str, reverse: bool = False):
         self._name = name
-        self.anchors['V_label'] = (0.5, 1.1)
-        self.label(f'{self._name}={print_voltage(V, precision=precision)}', rotate=True, color=blue, loc='V_label', halign='center', valign='center')
-        self.segments.append(schemdraw.segments.Segment([(0, 0), (1, 0)]))
-
-        a, b = (1.5, 0.7), (-0.5, 0.7)
-        self.segments.append(schemdraw.Segment((a, b), arrow='->', arrowwidth=.3, arrowlength=.4, color=blue))
+        self._reverse = reverse
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
+    def is_reverse(self) -> bool:
+        return self._reverse
+
+    def values(self) -> dict[str, complex]:
+        ...
+
+def simple_analysis_element(element):
+    class decorated_element(element, SimpleAnalysisElement):
+        def __init__(self, *args, **kwargs):
+            element.__init__(self, *args, **kwargs)
+            SimpleAnalysisElement.__init__(self, name=kwargs['name'], reverse=kwargs.get('reverse', False))
+    return decorated_element
+
+@extension.source
+@simple_analysis_element
+class VoltageSource(schemdraw.elements.SourceV):
+    def __init__(self, *args, name: str, V: complex, reverse: bool = False, precision: int = 3, **kwargs):
+        super().__init__(*args, reverse=not reverse, **kwargs)
+        self._V = V if not reverse else -V
+        label = dsp.print_complex(V, unit='V', precision=precision)
+        self.label(f'{name}={label}', rotate=True, color=dsp.blue, loc='value_label', halign='center', valign='center')
+        self.segments.append(extension.voltage_arrow())
+
+    @property
     def V(self) -> complex:
         return self._V
 
     def values(self) -> dict[str, complex]:
-        return {'U' : self.V}
+        return {'V' : self.V}
+
+@extension.source
+@simple_analysis_element
+class CurrentSource(schemdraw.elements.SourceI):
+    def __init__(self, *args, I: complex, name: str, reverse=False, precision=3, **kwargs):
+        super().__init__(*args, reverse=reverse, **kwargs)
+        self._I = I if not reverse else -I
+        label = dsp.print_complex(I, unit='A', precision=precision)
+        self.label(f'{name}={label}', loc='i_label', ofst=(0, 0.4), rotate=True, color=dsp.red)
+        self.segments.append(extension.current_arrow())
+
+    @property
+    def I(self) -> complex:
+        return self._I
 
-class ACVoltageSource(VoltageSource):
+    def values(self) -> dict[str, complex]:
+        return {'I' : self.I}
+
+@extension.resistor
+@simple_analysis_element
+class Resistor(schemdraw.elements.Resistor):
+    def __init__(self, *args, R: float, name: str, show_name: bool = True, show_value: bool = True, reverse: bool = False, **kwargs):
+        super().__init__(*args, reverse=reverse, **kwargs)
+        self._R = R
+        label = ''
+        label += f'{name}' if show_name else ''
+        label += '=' if  show_name and show_value else ''
+        label += dsp.print_resistance(self.R) if show_value else ''
+        self.label(label, rotate=True, loc='value_label', halign='center')
+
+    @property
+    def R(self) -> float:
+        return self._R
+
+    @property
+    def G(self) -> float:
+        return 1/self._R
+
+    def values(self) -> dict[str, float]:
+        return {'R' : self._R}
+
+@extension.resistor
+@simple_analysis_element
+class Conductance(schemdraw.elements.Resistor):
+    def __init__(self, *args, G: float, name: str, show_name: bool = True, show_value: bool = True, reverse: bool = False, **kwargs):
+        super().__init__(*args, reverse=reverse, **kwargs)
+        self._G = G
+        label = ''
+        label += f'{name}' if show_name else ''
+        label += '=' if  show_name and show_value else ''
+        label += dsp.print_conductance(self.G) if show_value else ''
+        self.label(label, rotate=True, loc='value_label', halign='center')
+
+    @property
+    def R(self) -> float:
+        return 1/self._G
+
+    @property
+    def G(self) -> float:
+        return self._G
+
+    def values(self) -> dict[str, float]:
+        return {'G' : self._R}
+
+@extension.resistor
+@simple_analysis_element
+class Impedance(schemdraw.elements.Resistor):
+    def __init__(self, *args, Z: complex, name: str, show_name: bool = True, show_value: bool = True, precision: int = 3, reverse: bool = False, **kwargs):
+        super().__init__(*args, reverse=reverse, **kwargs)
+        self._Z = Z
+        label = ''
+        label += f'{name}' if show_name else ''
+        label += '=' if  show_name and show_value else ''
+        label += dsp.print_impedance(self.Z, precision=precision) if show_value else ''
+        self.label(label, rotate=True, loc='value_label', halign='center')
+
+    @property
+    def Z(self) -> complex:
+        return self._Z
+
+    @property
+    def Y(self) -> complex:
+        return 1/self._Z
+
+    def values(self) -> dict[str, complex]:
+        return {'Z' : self._Z}
+
+@extension.source
+@simple_analysis_element
+class ACVoltageSource(schemdraw.elements.SourceSin):
     def __init__(self, V: float, w: float, phi: float, name: str, *args, sin=False, deg=False, reverse=False, precision=3, label_offset: float = 0.2, **kwargs):
-        super().__init__(V, name, *args, reverse=reverse, precision=precision, **kwargs)
+        super().__init__(*args, reverse=not reverse, **kwargs)
+        self._V = V if not reverse else -V
         self._w = w
         self._phi = phi
         self._deg = deg
         self._sin = sin
-        label = '$' + f'{self._V:4.2f}' + '\\mathrm{V}\\cdot\\cos(' + f'{self._w:4.2g}' + '\\cdot t + ' + f'{self._phi:4.2f}' + ')$'
-        self.label(label, rotate=True, ofst=label_offset)
+        label = dsp.print_sinosoidal(V*np.exp(1j*phi), unit='V', precision=precision, w=w, deg=deg)
+        self.label(f'{name}={label}', rotate=True, color=dsp.blue, loc='value_label', halign='center', valign='center')
 
     @property
     def w(self) -> float:
         return self._w
 
     @property
     def phi(self) -> float:
@@ -64,267 +216,233 @@
     def sin(self) -> bool:
         return self._sin
 
     @property
     def deg(self) -> bool:
         return self._deg
 
-class CurrentSource(schemdraw.elements.sources.SourceI):
-    def __init__(self, I: complex, name: str, *args, reverse=False, precision=3, **kwargs):
+    @property
+    def V(self) -> float:
+        return self._V
+
+    def values(self) -> dict[str, complex]:
+        return {'U' : self.V}
+
+@extension.source
+@simple_analysis_element
+class ACCurrentSource(schemdraw.elements.SourceSin):
+    def __init__(self, *args, I: float, w: float, phi: float, name: str, sin=False, deg=False, reverse=False, precision=3, **kwargs):
         super().__init__(*args, reverse=reverse, **kwargs)
-        if reverse:
-            self._I = -I
-        else:
-            self._I = I
-        self._name = name
-        self.segments = DrawCurrentSource()
-        a, b = (1.2, 0.3), (1.8, 0.3)
-        self.segments.append(schemdraw.Segment((a, b), arrow='->', arrowwidth=.3, arrowlength=.4, color=red))
-        self.anchors['I_label'] = a
-        self.label(f'{self._name}={print_current(self._I)}', loc='I_label', ofst=(0, 0.4), rotate=True, color=red)
+        self._I = I if not reverse else -I
+        self._w = w
+        self._phi = phi
+        self._deg = deg
+        self._sin = sin
+        label = dsp.print_sinosoidal(I*np.exp((1j*phi)), unit='A', precision=precision, w=w, deg=deg)
+        self.label(f'{name}={label}', loc='i_label', ofst=(0, 0.4), rotate=True, color=dsp.red)
+        self.segments.append(extension.current_arrow())
 
     @property
-    def name(self) -> str:
-        return self._name
+    def w(self) -> float:
+        return self._w
 
     @property
-    def I(self) -> complex:
+    def phi(self) -> float:
+        return self._phi
+
+    @property
+    def sin(self) -> bool:
+        return self._sin
+
+    @property
+    def deg(self) -> bool:
+        return self._deg
+
+    @property
+    def I(self) -> float:
         return self._I
 
     def values(self) -> dict[str, complex]:
         return {'I' : self.I}
 
-def DrawSource() -> list[schemdraw.segments.SegmentType]:
-    return [
-        schemdraw.segments.Segment([(0, 0), (0, 0), schemdraw.elements.elements.gap, (1, 0), (1, 0)]),
-        schemdraw.segments.SegmentCircle((0.5, 0), 0.5,)
-    ]
-
-def DrawCurrentSource() -> list[schemdraw.segments.SegmentType]:
-    return DrawSource() + [
-        schemdraw.segments.Segment([(0.5, -0.5), (0.5, 0.5)])
-    ]
-
-def DrawRealCurrentSource() -> list[schemdraw.segments.SegmentType]:
-    return DrawCurrentSource() + [
-        schemdraw.segments.SegmentCircle((-0.5, 0), 0.07, fill='black'),
-        schemdraw.segments.SegmentCircle((1.5, 0), 0.07, fill='black'),
-        schemdraw.segments.Segment([(-0.5, 0), (-0.5, 1)]),
-        schemdraw.segments.Segment([(1.5, 0), (1.5, 1)]),
-        schemdraw.segments.Segment([(-0.5, 1), (0, 1)]),
-        schemdraw.segments.Segment([(1, 1), (1.5, 1)]),
-        schemdraw.segments.Segment([(0, 0.8), (1, 0.8), (1, 1.2), (0, 1.2), (0, 0.8)])
-    ]
-
-def DrawVoltageSource() -> list[schemdraw.segments.SegmentType]:
-    return DrawSource() + [
-        schemdraw.segments.Segment([(0, 0), (1, 0)])
-    ]
-
-class Impedance(schemdraw.elements.twoterm.ResistorIEC):
-    def __init__(self, Z: complex, name: str, *args, show_name: bool = True, show_value: bool = True, precision: int = 3, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._Z = Z
-        self._name = name
-        label = ''
-        label += f'{self._name}' if show_name else ''
-        label += '=' if  show_name and show_value else ''
-        label += str(ScientificComplex(value=self.Z, unit='$\\Omega$', use_exp_prefix=True, precision=precision)) if show_value else ''
-        self.anchors['Z_label'] = (0.5, 0.3)
-        self.label(label, rotate=True, loc='Z_label', halign='center')
+@extension.source
+@simple_analysis_element
+class RectVoltageSource(schemdraw.elements.SourceSquare):
+    def __init__(self, V: float, w: float, phi: float, name: str, *args, sin=False, deg=False, reverse=False, **kwargs):
+        super().__init__(*args, reverse=not reverse, **kwargs)
+        self._V = V if not reverse else -V
+        self._w = w
+        self._phi = phi
+        self._deg = deg
+        self._sin = sin
+        self.segments.append(extension.voltage_arrow())
+        self.label(f'{name}', loc='value_label', halign='center', rotate=True, color=dsp.blue)
 
-    def down(self) -> schemdraw.elements.Element:
-        self.anchors['Z_label'] = (0.5, -0.9)
-        return super().down()
+    @property
+    def w(self) -> float:
+        return self._w
 
-    def left(self) -> schemdraw.elements.Element:
-        self.anchors['Z_label'] = (0.5, -1)
-        return super().left()
+    @property
+    def phi(self) -> float:
+        return self._phi
 
     @property
-    def name(self) -> str:
-        return self._name
+    def sin(self) -> bool:
+        return self._sin
 
     @property
-    def Z(self) -> complex:
-        return self._Z
+    def deg(self) -> bool:
+        return self._deg
 
     @property
-    def Y(self) -> complex:
-        return 1/self._Z
+    def V(self) -> float:
+        return self._V
 
     def values(self) -> dict[str, complex]:
-        return {'Z' : self._Z}
-
-    def _place_label(self, *args, **kwargs):
-        delta = self.end-self.start
-        if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
-            if delta[1] < 0:
-                kwargs.update({'rotation': 90})
-
-        super()._place_label(*args, **kwargs)
-
-class Resistor(schemdraw.elements.twoterm.ResistorIEC):
-    def __init__(self, R: float, name: str, *args, show_name: bool = True, show_value: bool = True, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._R = R
-        self._name = name
-        label = ''
-        label += f'{self._name}' if show_name else ''
-        label += '=' if  show_name and show_value else ''
-        label += str(ScientificFloat(value=self.R, unit='$\\Omega$', use_exp_prefix=True)) if show_value else ''
-        self.anchors['R_label'] = (0.5, 0.3)
-        self.label(label, rotate=True, loc='R_label', halign='center')
-
-    def down(self) -> schemdraw.elements.Element:
-        self.anchors['R_label'] = (0.5, -0.9)
-        return super().down()
+        return {'U' : self.V}
 
-    def left(self) -> schemdraw.elements.Element:
-        self.anchors['R_label'] = (0.5, -1)
-        return super().left()
+@simple_analysis_element
+class RectCurrentSource(schemdraw.elements.SourceSquare):
+    def __init__(self, I: float, w: float, phi: float, name: str, *args, sin=False, deg=False, reverse=False, **kwargs):
+        super().__init__(self, *args, reverse=reverse, **kwargs)
+        self._I = I if not reverse else -I
+        self._w = w
+        self._phi = phi
+        self._deg = deg
+        self._sin = sin
+        self.segments.append(extension.current_arrow())
+        self.label(f'{name}', loc='i_label', halign='center', rotate=True, color=dsp.red)
 
     @property
-    def name(self) -> str:
-        return self._name
+    def w(self) -> float:
+        return self._w
 
     @property
-    def R(self) -> float:
-        return self._R
+    def phi(self) -> float:
+        return self._phi
 
     @property
-    def G(self) -> float:
-        return 1/self._R
+    def sin(self) -> bool:
+        return self._sin
 
-    def values(self) -> dict[str, float]:
-        return {'R' : self._R}
+    @property
+    def deg(self) -> bool:
+        return self._deg
 
-    def _place_label(self, *args, **kwargs):
-        delta = self.end-self.start
-        if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
-            if delta[1] < 0:
-                kwargs.update({'rotation': 90})
+    @property
+    def I(self) -> float:
+        return self._I
 
-        super()._place_label(*args, **kwargs)
+    def values(self) -> dict[str, complex]:
+        return {'I' : self.I}
 
-class Capacitor(schemdraw.elements.twoterm.Capacitor):
-    def __init__(self, C: float, name: str, *args, show_name: bool = True, show_value: bool = True, label_offset: float = 0.2, **kwargs):
-        super().__init__(*args, **kwargs)
+@extension.capacitor
+@simple_analysis_element
+class Capacitor(schemdraw.elements.Capacitor):
+    def __init__(self, C: float, name: str, *args, show_name: bool = True, show_value: bool = True, reverse: bool = False, **kwargs):
         self._C = C
-        self._name = name
+        super().__init__(*args, reverse=reverse, **kwargs)
         label = ''
-        label += f'{self._name}' if show_name else ''
+        label += f'{name}' if show_name else ''
         label += '=' if  show_name and show_value else ''
-        label += str(ScientificFloat(value=self.C, unit='$\\mathrm{F}$', use_exp_prefix=True)) if show_value else ''
-        self.label(label, rotate=True, ofst=label_offset)
-
-    @property
-    def name(self) -> str:
-        return self._name
+        label += dsp.print_capacitance(C) if show_value else ''
+        self.label(label, rotate=True, loc='value_label', halign='center')
 
     @property
     def C(self) -> float:
         return self._C
 
     def values(self) -> dict[str, float]:
         return {'C' : self._C}
 
-    def _place_label(self, *args, **kwargs):
-        delta = self.end-self.start
-        if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
-            if delta[1] < 0:
-                kwargs.update({'rotation': 90})
-
-        super()._place_label(*args, **kwargs)
-
-class Inductance(schemdraw.elements.twoterm.Inductor):
-    def __init__(self, L: float, name: str, *args, show_name: bool = True, show_value: bool = True, label_offset: float = 0.2, **kwargs):
-        super().__init__(*args, **kwargs)
+@extension.inductor
+@simple_analysis_element
+class Inductance(schemdraw.elements.Inductor):
+    def __init__(self, L: float, name: str, *args, show_name: bool = True, show_value: bool = True, label_offset: float = 0.2, reverse: bool = False, **kwargs):
         self._L = L
-        self._name = name
+        super().__init__(*args, reverse=reverse, **kwargs)
         label = ''
-        label += f'{self._name}' if show_name else ''
+        label += f'{name}' if show_name else ''
         label += '=' if  show_name and show_value else ''
-        label += str(ScientificFloat(value=self.L, unit='$\\mathrm{H}$', use_exp_prefix=True)) if show_value else ''
-        self.label(label, rotate=True, ofst=label_offset)
-
-    @property
-    def name(self) -> str:
-        return self._name
+        label += dsp.print_inductance(L) if show_value else ''
+        self.label(label, rotate=True, loc='value_label', halign='center')
 
     @property
     def L(self) -> float:
         return self._L
 
     def values(self) -> dict[str, float]:
         return {'L$' : self._L}
 
-    def _place_label(self, *args, **kwargs):
-        delta = self.end-self.start
-        if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
-            if delta[1] < 0:
-                kwargs.update({'rotation': 90})
-
-        super()._place_label(*args, **kwargs)
-
-class RealCurrentSource(schemdraw.elements.Element2Term):
-    def __init__(self, current_source: CurrentSource, resistor: Resistor, *args, zoom_resistor=0.7, **kwargs):
-        super().__init__(*args, **kwargs)
+class RealCurrentSource(schemdraw.elements.Element2Term, SimpleAnalysisElement):
+    def __init__(self, current_source: CurrentSource, resistor: Resistor, *args, zoom_resistor: float = 0.7, name: str = '', reverse: bool = False, **kwargs):
+        if current_source.is_reverse:
+            reverse = not reverse
+        super().__init__(*args, reverse=reverse, **kwargs)
+        SimpleAnalysisElement.__init__(self, name=current_source.name, reverse=reverse)
         self.segments += segments_of(current_source)
-        transform = schemdraw.transform.Transform(theta = 0, globalshift=((1-zoom_resistor)/2,-1), localshift=(0, 0), zoom=zoom_resistor)
+        transform = schemdraw.transform.Transform(theta = 0, globalshift=((1-zoom_resistor)/2,-1.5), localshift=(0, 0), zoom=zoom_resistor)
         self.segments += [s.xform(transform) for s in segments_of(resistor)]
-        left_line = schemdraw.Segment([(-1, 0), (-1, -1), ((1-zoom_resistor)/2, -1)])
-        right_line = schemdraw.Segment([(2, 0), (2, -1), ((1+zoom_resistor)/2, -1)])
+        left_line = schemdraw.Segment([(-1, 0), (-1, -1.5), ((1-zoom_resistor)/2, -1.5)])
+        right_line = schemdraw.Segment([(2, 0), (2, -1.5), ((1+zoom_resistor)/2, -1.5)])
         self.segments += [left_line, right_line]
-        self.anchors.update(current_source.anchors)
-        self.anchors.update({k:(v[0]+0, v[1]-2.2) for k, v in resistor.anchors.items()})
+        self.anchors['value_label'] = (0.5, -1.2)
+        self.anchors['i_label'] = current_source.anchors['i_label']
+        self.anchors['v_label'] = (0.5, -2.4)
         self._userlabels += current_source._userlabels
         self._userlabels += resistor._userlabels
-        self._name = current_source.name
         self._I = current_source.I
         self._R = resistor.R
 
     @property
-    def name(self) -> str:
-        return self._name
-
-    @property
     def I(self) -> complex:
         return self._I
 
     @property
     def R(self) -> float:
         return self._R
 
     @property
     def G(self) -> float:
         return 1/self._R
 
     def values(self) -> dict[str, complex]:
         return {'I' : self.I, 'R' : self.R}
 
-class RealVoltageSource(schemdraw.elements.Element2Term):
-    def __init__(self, voltage_source: VoltageSource, resistor: Resistor, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.segments.append(schemdraw.segments.Segment([(0, 0), (0, 0), schemdraw.elements.elements.gap, (4, 0), (4, 0)]))
-        self.segments.extend(segments_of(voltage_source))
-        self.segments.append(schemdraw.segments.Segment([(1, 0), (3, 0)]))
-        transform = schemdraw.transform.Transform(theta = 0, globalshift=(3, 0))
-        self.segments.extend([s.xform(transform) for s in segments_of(resistor)])
-        self.anchors.update(voltage_source.anchors)
-        self.anchors.update({k:(v[0]+3, v[1]) for k, v in resistor.anchors.items()})
+class RealVoltageSource(schemdraw.elements.Element2Term, SimpleAnalysisElement):
+    def __init__(self, voltage_source: VoltageSource, resistor: Resistor, *args, reverse: bool = False, **kwargs):
+        reverse_voltage_source = not voltage_source.is_reverse
+        if reverse_voltage_source:
+            reverse = not reverse
+        schemdraw.elements.Element2Term.__init__(self, *args, reverse=reverse_voltage_source, **kwargs)
+        SimpleAnalysisElement.__init__(self, name=voltage_source.name, reverse=reverse_voltage_source)
+        transform_resistor = schemdraw.transform.Transform(theta = 0, globalshift=(0, 0))
+        transform_voltage_source = schemdraw.transform.Transform(theta = 0, globalshift=(3, 0))
+        if reverse:
+            transform_resistor, transform_voltage_source = transform_voltage_source, transform_resistor
+        self.segments.append(schemdraw.segments.Segment([(0, 0), (0, 0), schemdraw.elements.elements.gap, (1, 0), (3, 0), schemdraw.elements.elements.gap, (4, 0), (4, 0)]))
+        self.segments.extend([s.xform(transform_resistor) for s in segments_of(resistor)])
+        self.segments.extend([s.xform(transform_voltage_source) for s in segments_of(voltage_source)])
+        for a, p in voltage_source.anchors.items():
+            self.anchors[a+'_vs'] = transform_voltage_source.transform(p)
+        for a, p in resistor.anchors.items():
+            self.anchors[a+'_res'] = transform_resistor.transform(p)
+        voltage_source_labels = [l for l in voltage_source._userlabels]
+        resistor_labels = [l for l in resistor._userlabels]
+        for l in voltage_source_labels:
+            if type(l.loc) == str:
+                l.loc += '_vs'
+        for l in resistor_labels:
+            if type(l.loc) == str:
+                l.loc += '_res'
         self._userlabels += voltage_source._userlabels
         self._userlabels += resistor._userlabels
-        self._name = voltage_source.name
-        self._V = voltage_source.V
+        self._V = -voltage_source.V
         self._R = resistor.R
-
-    @property
-    def name(self) -> str:
-        return self._name
+        self.anchors['v_label'] = (2, -1.5)
 
     @property
     def V(self) -> complex:
         return self._V
 
     @property
     def R(self) -> float:
@@ -359,16 +477,50 @@
         self.anchors['SE'] = (0.5, -0.3)
         self.anchors['SW'] = (-0.5, -0.3)
 
     @property
     def name(self) -> str:
         return f'Node {self.node_id}'
 
+class Switch(schemdraw.elements.elements.Element2Term):
+    def __init__(self, name: str, *args, state: SwitchState = SwitchState.OPEN, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.state = state
+        self._name = name
+        self.segments.append(schemdraw.Segment([(0, 0), schemdraw.elements.elements.gap, (1, 0)]))
+        self.segments.append(schemdraw.SegmentCircle((schemdraw.elements.switches.sw_dot_r, 0), schemdraw.elements.switches.sw_dot_r, fill='bg', zorder=3))
+        self.segments.append(schemdraw.SegmentCircle((1-schemdraw.elements.switches.sw_dot_r, 0), schemdraw.elements.switches.sw_dot_r, fill='bg', zorder=3))
+        self.segments.append(schemdraw.Segment([(0,0)]))
+        if self.state == SwitchState.OPEN:
+            self.open()
+        if self.state == SwitchState.CLOSED:
+            self.close()
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    def open(self) -> None:
+        self.state = SwitchState.OPEN
+        self.segments.pop()
+        self.segments.append(schemdraw.Segment([(schemdraw.elements.switches.sw_dot_r, 0), (1, 0.6)]))
+
+    def close(self) -> None:
+        self.state = SwitchState.CLOSED
+        self.segments.pop()
+        self.segments.append(schemdraw.Segment([(schemdraw.elements.switches.sw_dot_r, 0), (1, schemdraw.elements.switches.sw_dot_r*1.2)]))
+
+    def toggle(self) -> None:
+        if self.state == self.state.OPEN:
+            self.close()
+        if self.state == self.state.CLOSED:
+            self.open()
+
 class LabelNode(Node):
-    def __init__(self, id : str = '', id_loc : str | dict[str, Any] = '', *args, show=True, **kwargs):
+    def __init__(self, id : str = '', id_loc : str | dict[str, str] = '', *args, show=True, **kwargs):
         super().__init__(id, *args, **kwargs)
         locations = {
             'W': {'loc': 'left', 'halign': 'right', 'valign': 'center'},
             'N': {'loc': 'top', 'halign': 'center', 'valign': 'bottom'},
             'NE': {'loc': 'NE', 'halign': 'left', 'valign': 'bottom'},
             'NW': {'loc': 'NW', 'halign': 'right', 'valign': 'bottom'},
             'E': {'loc': 'right', 'halign': 'left', 'valign': 'center'},
@@ -408,50 +560,79 @@
              (-resheight*.2, -gndgap*2-gnd_lead),
              (resheight*.2, -gndgap*2-gnd_lead)]))
 
     @property
     def name(self) -> str:
         return 'Ground'
 
+    def up(self) -> schemdraw.elements.Element:
+        return super().left()
+
+    def down(self) -> schemdraw.elements.Element:
+        return super().right()
+
+    def left(self) -> schemdraw.elements.Element:
+        return super().down()
+
+    def right(self) -> schemdraw.elements.Element:
+        return super().up()
+
 class VoltageLabel(schemdraw.elements.CurrentLabel):
-    def __init__(self, at: schemdraw.elements.Element, label: str = '', label_loc: str = 'bottom', **kwargs):
-        kwargs['color'] = kwargs.get('color', blue)
-        super().__init__(**kwargs)
+    def __init__(self, at: schemdraw.elements.Element, label: str = '', label_loc: str = 'bottom', reverse: bool = False, **kwargs):
+        kwargs.update({'color': kwargs.get('color', dsp.blue)})
+        kwargs.update({'headlength': kwargs.get('headlength', 0.4)})
+        kwargs.update({'headwidth': kwargs.get('headwidth', 0.3)})
         if isinstance(at, RealVoltageSource):
-            self.at(at.center)
-        else:
-            try:
-                self.at(at.v_label)
-                self.theta(at.transform.theta)
-            except AttributeError:
-                self.at(at)
-        self.label(label, rotate=kwargs.get('rotate', True), loc=label_loc, ofst=(0, -0.1))
+            kwargs.update({'length': kwargs.get('length', 4)})
+        super().__init__(reverse=reverse, **kwargs)
+        try:
+            self.at(at.v_label)
+            self.theta(at.transform.theta)
+        except AttributeError:
+            self.at(at)
+        rotate = kwargs.get('rotate', True)
+        if rotate == True and at.transform.theta == 270:
+            rotate = 90
+        self.label(label, rotate=rotate, loc=label_loc, ofst=(0, -0.1))
 
 class CurrentLabel(schemdraw.elements.CurrentLabelInline):
     def __init__(self, at: schemdraw.elements.Element, label: str = '', **kwargs):
-        kwargs['color'] = kwargs.get('color', red)
+        kwargs.update(i_label_args.get(type(at), {}))
+        kwargs.update({'color': kwargs.get('color', dsp.red)})
+        kwargs.update({'headlength': kwargs.get('headlength', 0.4)})
+        kwargs.update({'headwidth': kwargs.get('headwidth', 0.3)})
         totlen = at._userparams.get('l', at._userparams.get('unit', 3))
-        kwargs['ofst'] = totlen/4-0.15+kwargs.get('ofst', 0)
+        kwargs.update({'ofst': totlen/4-0.15+kwargs.get('ofst', 0)})
         start = kwargs.get('start', True)
         reverse = kwargs.get('reverse', False)
+        if isinstance(at, RealVoltageSource) or isinstance(at, RealCurrentSource): # when replacing CurrentLabelInline this dependency may be removed
+            reverse = not reverse
         kwargs.update({'start' : start, 'reverse' : reverse})
         super().__init__(**kwargs)
         self.at(at)
         self.label(label)
 
-    @property
-    def name(self) -> str:
-        return ''
-
-v_label_args : dict[Any, dict[str, Any]]= {
-    Resistor : {'ofst' : -0.6},
-    Impedance : {'ofst' : -0.6},
-    CurrentSource : {'ofst' : 1.5, 'label_loc': 'top'},
-    RealCurrentSource : {'ofst' : 1.5, 'label_loc': 'top'}
-}
+class PowerLabel(schemdraw.elements.Label):
+    def __init__(self, at: schemdraw.elements.Element, label: str = '', **kwargs):
+        kwargs.update({'color': kwargs.get('color', dsp.green)})
+        super().__init__(**kwargs)
+        try:
+            self.at(at.s_label)
+            self.theta(at.transform.theta)
+        except AttributeError:
+            self.at(at.center)
+        rotate = kwargs.get('rotate', True)
+        if rotate == True and at.transform.theta == 270:
+            rotate = 90
+        self.label(label, rotate=rotate, halign='center')
 
-i_label_args : dict[Any, dict[str, Any]]= {
+i_label_args : dict[Any, dict[str, float]] = {
     Resistor : {'ofst' : 1.4},
     Impedance : {'ofst' : 1.4},
+    Capacitor : {'ofst' : 1.4},
+    Inductance : {'ofst' : 1.4},
     VoltageSource : {'ofst' : -2.8},
-    RealVoltageSource: {'ofst' : -0.8}
+    CurrentSource : {'ofst' : -2.8},
+    ACVoltageSource : {'ofst' : -3.8},
+    RealVoltageSource: {'ofst' : -0.8},
+    RealCurrentSource: {'ofst' : 1.4}
 }
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator/Utils.py` & `CircuitCalculator-0.1.0/src/CircuitCalculator/Utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import numpy as np
 from dataclasses import dataclass, field
 
 @dataclass(frozen=True)
 class FloatPrecision:
     value: float
     precision: int = 3
+    min_exp: int = -16
+    max_exp: int = 16
+
+    @property
+    def is_zero(self) -> bool:
+        if self.value == 0:
+            return True
+        return self.exponent < self.min_exp
+
+    @property
+    def is_inf(self) -> bool:
+        return self.exponent > self.max_exp
 
     @property
     def mantissa(self) -> int:
         return int(np.round(self.value/(10**self.exponent)))
 
     @property
     def exponent(self) -> int:
@@ -28,29 +40,22 @@
     def _float_to_string(self, value: float) -> str:
         str_abs_value = str(value)
         if str_abs_value.count('e') == 1:
             post_decimal_digits = abs(int(str_abs_value.split('e')[-1]))+1+self.precision
             return f'{value:.{post_decimal_digits}f}'
         return str(value)
 
-@dataclass(frozen=True)
-class Float3:
-    value: FloatPrecision
-
-    @property
-    def precision(self) -> int:
-        return self.value.precision
-
+class Float3(FloatPrecision):
     @property
-    def mantissa(self) -> float:
-        return self.value.mantissa * 10**(self.value.exponent-self.exponent)
+    def mantissa3(self) -> float:
+        return self.mantissa * 10**(self.exponent-self.exponent3)
 
     @property
-    def exponent(self) -> int:
-        return int(3*np.floor((self.precision + self.value.exponent - 1)/3))
+    def exponent3(self) -> int:
+        return int(3*np.floor((self.precision + self.exponent - 1)/3))
 
 @dataclass
 class ScientificFloat:
     value: float
     unit: str = ''
     precision: int = 3
     use_exp_prefix: bool = False
@@ -64,15 +69,17 @@
         6 : 'M',
         9 : 'G',
         12 : 'T'
     })
 
     @property
     def value3(self) -> Float3:
-        return Float3(FloatPrecision(self.value, self.precision))
+        if self.use_exp_prefix:
+            return Float3(value=self.value, precision=self.precision, min_exp=min(self.exp_prefixes.keys()), max_exp=max(self.exp_prefixes.keys()))
+        return Float3(value=self.value, precision=self.precision)
 
     def exp_prefix(self, exp) -> str:
         if not self.use_exp_prefix:
             return ''
         if exp > max(self.exp_prefixes.keys()):
             return self.exp_prefixes[max(self.exp_prefixes.keys())]
         if exp < min(self.exp_prefixes.keys()):
@@ -92,29 +99,30 @@
                     return exp - min(self.exp_prefixes.keys())
             return 0
         if rebase_exp(exp) == 0:
             return ''
         return f'e{rebase_exp(exp)}'
 
     def __str__(self) -> str:
-        pre_decimal_positions = 0 if np.abs(self.value3.mantissa) < 1 else len(str(abs(self.value3.mantissa)).split('.')[0])
+        if self.value3.is_inf:
+            return '∞' if self.value3.mantissa >= 0 else '-∞'
+        pre_decimal_positions = 0 if np.abs(self.value3.mantissa3) < 1 else len(str(abs(self.value3.mantissa3)).split('.')[0])
         post_decimal_positions = max(self.precision - pre_decimal_positions, 0)
-        pre_decimal = int(self.value3.mantissa)
+        pre_decimal = int(self.value3.mantissa3)
         pre_decimal_str = f'{pre_decimal:d}'
-        post_decimal = int(np.round(self.value3.mantissa % 1 * 10**(post_decimal_positions)))
+        post_decimal = int(np.round(np.abs(self.value3.mantissa3) % 1 * 10**(post_decimal_positions)))
         post_decimal_str = '' if post_decimal_positions == 0 else f'.{post_decimal:0{post_decimal_positions}d}'
-        return f'{pre_decimal_str}{post_decimal_str}{self.exp_extension(self.value3.exponent)}{self.exp_prefix(self.value3.exponent)}{self.unit}'
+        return f'{pre_decimal_str}{post_decimal_str}{self.exp_extension(self.value3.exponent3)}{self.exp_prefix(self.value3.exponent3)}{self.unit}'
 
 @dataclass(frozen=True)
 class ScientificComplex:
     value: complex
     unit: str = ''
     precision: int = 3
     use_exp_prefix: bool = False
-    hide_minor_part: bool = True
     compact: bool = False
     polar: bool = False
     deg: bool = False
     exp_prefixes: dict[int, str] = field(default_factory=lambda: {
         -12 : 'p',
         -9 : 'n',
         -6 : 'u',
@@ -162,20 +170,12 @@
                 if self.deg:
                     if np.log10(np.abs(self.angle)) <= -2:
                         return f'{str(self.abs)}'
                     return f'{str(self.abs)}∠{self.angle:.2f}'
                 if np.log10(np.abs(self.angle)) <= -5:
                     return f'{str(self.abs)}'
                 return f'{str(self.abs)}∠{self.angle:.4f}'
-            if self.hide_minor_part:
-                if self.imag.value3.exponent > self.real.value3.exponent:
-                    target_exp_prefix = {self.imag.value3.exponent : self.exp_prefixes.get(self.imag.value3.exponent, '')}
-                target_exp_prefix = {self.real.value3.exponent : self.exp_prefixes.get(self.real.value3.exponent, '')}
-                real = ScientificFloat(self.real.value, self.unit, self.precision, self.use_exp_prefix, target_exp_prefix)
-                imag = ScientificFloat(self.imag.value, self.unit, self.precision, self.use_exp_prefix, target_exp_prefix)
-                if real.value3.exponent > imag.value3.exponent or imag.value3.mantissa == 0:
-                    return f'{self.real_sign}{real.__str__()}'
-                if imag.value3.exponent > real.value3.exponent or real.value3.mantissa == 0:
-                    sign = '' if self.imag_sign.strip() == '+' else self.imag_sign
-                    return f'{sign}j{imag.__str__()}'
-                return f'{self.real_sign}{real.__str__()}{self.imag_sign}j{imag.__str__()}'
+            if self.imag.value3.is_zero:
+                return f'{self.real_sign}{self.real.__str__()}'
+            if self.real.value3.is_zero:
+                return f'{self.imag_sign}j{self.imag.__str__()}' if self.value.imag < 0 else f'j{self.imag.__str__()}'
             return f'{self.real_sign}{self.real.__str__()}{self.imag_sign}j{self.imag.__str__()}'
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/PKG-INFO` & `CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.0.9
+Version: 0.1.0
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CircuitCalculator
```

### Comparing `CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/SOURCES.txt` & `CircuitCalculator-0.1.0/src/CircuitCalculator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 LICENSE
 README.md
 pyproject.toml
-src/CircuitCalculator/EquivalentSources.py
-src/CircuitCalculator/NodalAnalysis.py
 src/CircuitCalculator/PlottingTemplates.py
 src/CircuitCalculator/Utils.py
 src/CircuitCalculator/__init__.py
 src/CircuitCalculator.egg-info/PKG-INFO
 src/CircuitCalculator.egg-info/SOURCES.txt
 src/CircuitCalculator.egg-info/dependency_links.txt
 src/CircuitCalculator.egg-info/requires.txt
 src/CircuitCalculator.egg-info/top_level.txt
+src/CircuitCalculator/Circuit/__init__.py
 src/CircuitCalculator/Circuit/circuit.py
 src/CircuitCalculator/Circuit/components.py
+src/CircuitCalculator/Circuit/impedance.py
+src/CircuitCalculator/Circuit/solution.py
 src/CircuitCalculator/Circuit/transformers.py
+src/CircuitCalculator/Network/NodalAnalysis.py
 src/CircuitCalculator/Network/elements.py
+src/CircuitCalculator/Network/equivalent_sources.py
 src/CircuitCalculator/Network/labelmapper.py
 src/CircuitCalculator/Network/loaders.py
 src/CircuitCalculator/Network/network.py
 src/CircuitCalculator/Network/solution.py
 src/CircuitCalculator/Network/supernodes.py
 src/CircuitCalculator/Network/transformers.py
-src/CircuitCalculator/SimpleAnalysis/Elements.py
-src/CircuitCalculator/SimpleAnalysis/Layout.py
+src/CircuitCalculator/SignalProcessing/__init__.py
+src/CircuitCalculator/SignalProcessing/periodic_functions.py
+src/CircuitCalculator/SignalProcessing/types.py
+src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py
+src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py
 src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
+src/CircuitCalculator/SimpleAnalysis/TimeSeries.py
+src/CircuitCalculator/SimpleAnalysis/__init__.py
+src/CircuitCalculator/SimpleAnalysis/layout.py
+src/CircuitCalculator/SimpleAnalysis/plot_elements.py
 src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
 src/CircuitCalculator/SimpleCircuit/DiagramParser.py
+src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
+src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
 src/CircuitCalculator/SimpleCircuit/Display.py
 src/CircuitCalculator/SimpleCircuit/Elements.py
 src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
 src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
+src/CircuitCalculator/SimpleCircuit/__init__.py
+src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
+src/CircuitCalculator/SimpleCircuit/styles/__init__.py
+src/CircuitCalculator/SimpleCircuit/styles/styling.py
+src/CircuitCalculator/SimpleCircuit/styles/DIN/__init__.py
+src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py
+src/CircuitCalculator/SimpleCircuit/styles/DIN/style.py
 tests/test_integration.py
```

### Comparing `CircuitCalculator-0.0.9/tests/test_integration.py` & `CircuitCalculator-0.1.0/tests/test_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,170 @@
 from CircuitCalculator.Network.loaders import load_network_from_json
-from CircuitCalculator.NodalAnalysis import nodal_analysis_solver
+from CircuitCalculator.Network.NodalAnalysis import nodal_analysis_solver, open_circuit_impedance
 import numpy as np
 
 def test_network_1_with_advanced_nodal_analysis() -> None:
     network = load_network_from_json('./examples/networks/json/example_network_1.json')
     solution = nodal_analysis_solver(network)
+    np.testing.assert_almost_equal(solution.get_current('Uq'), -1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('R'), 1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('Uq'), 1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('R'), 1.00, decimal=2)
+
+def test_network_2_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_2.json')
+    solution = nodal_analysis_solver(network)
+    np.testing.assert_almost_equal(solution.get_current('Iq'), 1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('R'), 1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('Iq'), -1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('R'), 1.00, decimal=2)
+
+def test_network_3_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_3.json')
+    solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 7.69, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 15.38, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('I1'), -23.08, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0.77, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.77, decimal=2)
-    np.testing.assert_almost_equal(solution.get_current('I1'), -0.23, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('I1'), -0.77, decimal=2)
 
-def test_network_2_with_advanced_nodal_analysis() -> None:
-    network = load_network_from_json('./examples/networks/json/example_network_2.json')
+def test_network_4_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_4.json')
     solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 0.40, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R3'), 0.60, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0.10, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.02, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R3'), 0.02, decimal=2)
-    np.testing.assert_almost_equal(solution.get_current('U1'), 0.12, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('U1'), -0.12, decimal=2)
 
-def test_network_3_with_advanced_nodal_analysis() -> None:
-    network = load_network_from_json('./examples/networks/json/example_network_3.json')
+def test_network_5_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_5.json')
     solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 0.56, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 0.44, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R3'), 1.04, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R4'), 1.39, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R5'), -2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U2'), 2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0.056, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.022, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R3'), 0.035, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R4'), 0.035, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R5'), -0.04, decimal=2)
-    np.testing.assert_almost_equal(solution.get_current('U1'), 0.056, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U2'), 0.075, decimal=3)
-
-def test_network_4_with_advanced_nodal_analysis() -> None:
-    network = load_network_from_json('./examples/networks/json/example_network_4.json')
+    np.testing.assert_almost_equal(solution.get_current('U1'), -0.056, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U2'), -0.075, decimal=3)
+    
+def test_network_6_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_6.json')
     solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 0.52, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 0.48, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R3'), -2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R4'), 1.10, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R5'), 1.38, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U2'), 2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0.052, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.024, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R3'), -0.067, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R4'), 0.028, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R5'), 0.028, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U1'), 0.052, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U2'), 0.094, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U1'), -0.052, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U2'), -0.094, decimal=3)
 
-def test_network_5_with_advanced_nodal_analysis() -> None:
-    network = load_network_from_json('./examples/networks/json/example_network_5.json')
+def test_network_7_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_7.json')
     solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), -1.56, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 2.14, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R3'), 1.44, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R4'), 0.30, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U2'), 2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U3'), 3.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('I4'), -2.7, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), -0.156, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.107, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R3'), 0.048, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R4'), 0.0075, decimal=4)
-    np.testing.assert_almost_equal(solution.get_current('U1'), 0.156, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U2'), 0.048, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U3'), 0.0075, decimal=4)
+    np.testing.assert_almost_equal(solution.get_current('U1'), -0.156, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U2'), -0.048, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U3'), -0.0075, decimal=4)
     np.testing.assert_almost_equal(solution.get_current('I4'), 0.1, decimal=3)
 
 def test_network_8_with_advanced_nodal_analysis() -> None:
     network = load_network_from_json('./examples/networks/json/example_network_8.json')
+    Rges = open_circuit_impedance(network, '1', '2').real
+    np.testing.assert_almost_equal(Rges, 4.66, decimal=2)
+
+def test_network_9_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_9.json')
+    solution = nodal_analysis_solver(network)
+    np.testing.assert_almost_equal(solution.get_voltage('Vs1'), 1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('Vs2'), 2.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('R1'), 3.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('Vs1'), -0.30, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('Vs2'), -0.30, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('R1'), 0.30, decimal=3)
+
+def test_network_10_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_10.json')
     solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R3'), -0.75, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R4'), -4.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R5'), 3.75, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U1'), 1.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('U2'), 2.00, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('I3'), -7.75, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0.10, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.10, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R3'), -0.025, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R4'), -0.10, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R5'), 0.075, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U1'), 0.075, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('U2'), 0.075, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U1'), -0.075, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('U2'), -0.075, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('I3'), 0.10, decimal=3)
 
-def test_network_9_with_advanced_nodal_analysis() -> None:
-    network = load_network_from_json('./examples/networks/json/example_network_9.json')
+def test_network_11_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_11.json')
     solution = nodal_analysis_solver(network)
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 0, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 20, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R3'), -20, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('R4'), 100, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('Iq'), 0, decimal=2)
     np.testing.assert_almost_equal(solution.get_voltage('Uq'), 120, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R2'), 4, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R3'), -1, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R4'), 5, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('Iq'), 4, decimal=3)
-    np.testing.assert_almost_equal(solution.get_current('Uq'), 5, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('Uq'), -5, decimal=3)
+
+def test_network_13_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_13.json')
+    solution = nodal_analysis_solver(network)
+    np.testing.assert_almost_equal(solution.get_voltage('R1'), 0.182, decimal=3)
+    np.testing.assert_almost_equal(solution.get_voltage('R2'), 0.182, decimal=3)
+    np.testing.assert_almost_equal(solution.get_voltage('R3'), 0.818, decimal=3)
+    np.testing.assert_almost_equal(solution.get_voltage('Vs'), 1, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('R1'), 0.0182, decimal=4)
+    np.testing.assert_almost_equal(solution.get_current('R2'), 0.0091, decimal=4)
+    np.testing.assert_almost_equal(solution.get_current('R3'), 0.0273, decimal=4)
+    np.testing.assert_almost_equal(solution.get_current('Vs'), -0.0273, decimal=3)
+
+def test_network_14_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json('./examples/networks/json/example_network_14.json')
+    solution = nodal_analysis_solver(network)
+    np.testing.assert_almost_equal(solution.get_voltage('R1'), 0.4, decimal=3)
+    np.testing.assert_almost_equal(solution.get_voltage('R2'), 0.4, decimal=3)
+    np.testing.assert_almost_equal(solution.get_voltage('Vs'), -0.4, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('R1'), 0.04, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('R2'), 0.02, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('Vs'), -0.06, decimal=3)
```

