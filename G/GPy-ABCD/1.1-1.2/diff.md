# Comparing `tmp/GPy-ABCD-1.1.tar.gz` & `tmp/GPy-ABCD-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPy-ABCD-1.1.tar", last modified: Wed Jul 14 19:19:59 2021, max compression
+gzip compressed data, was "GPy-ABCD-1.2.tar", last modified: Sun Jul 30 22:36:25 2023, max compression
```

## Comparing `GPy-ABCD-1.1.tar` & `GPy-ABCD-1.2.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.457033 GPy-ABCD-1.1/GPy_ABCD/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.457033 GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5713 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/grammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     7572 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/kernelExpressionOperations.py
--rw-r--r--   0 runner    (1001) docker     (121)    12021 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/kernelInterpretation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/kernelOperations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     5469 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8255 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/change.py
--rw-r--r--   0 runner    (1001) docker     (121)     6850 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/commutative_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8655 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/commutatives.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/GPy_ABCD/Kernels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/baseKernels.py
--rw-r--r--   0 runner    (1001) docker     (121)    11191 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/changeOperators.py
--rw-r--r--   0 runner    (1001) docker     (121)     9144 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/changeWindowShiftedSides.py
--rw-r--r--   0 runner    (1001) docker     (121)     7930 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/changeWindowThreePart.py
--rw-r--r--   0 runner    (1001) docker     (121)     7390 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/linearKernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/linearOffsetKernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    11396 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/periodicKernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    10596 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Kernels/sigmoidalKernels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/GPy_ABCD/Models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8609 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Models/modelSearch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/GPy_ABCD/Util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Util/dataAndPlottingUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)     6597 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Util/genericUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Util/kernelUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Util/modelUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/Util/showcaseAllKernels.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/GPy_ABCD/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 19:19:59.457033 GPy-ABCD-1.1/GPy_ABCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11742 2021-07-14 19:19:59.000000 GPy-ABCD-1.1/GPy_ABCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2021-07-14 19:19:59.000000 GPy-ABCD-1.1/GPy_ABCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 19:19:59.000000 GPy-ABCD-1.1/GPy_ABCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-07-14 19:19:59.000000 GPy-ABCD-1.1/GPy_ABCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-14 19:19:59.000000 GPy-ABCD-1.1/GPy_ABCD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11742 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10076 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 19:19:59.461033 GPy-ABCD-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-07-14 19:19:50.000000 GPy-ABCD-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.795763 GPy-ABCD-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.791763 GPy-ABCD-1.2/GPy_ABCD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.791763 GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/kernelExpressionOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/kernelInterpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/kernelOperations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.791763 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/commutative_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/commutatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.791763 GPy-ABCD-1.2/GPy_ABCD/Kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/baseKernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/changeOperators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/changeWindowShiftedSides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/changeWindowThreePart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/linearKernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/linearOffsetKernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/periodicKernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Kernels/sigmoidalKernels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.791763 GPy-ABCD-1.2/GPy_ABCD/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Models/modelSearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.795763 GPy-ABCD-1.2/GPy_ABCD/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/dataAndPlottingUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/genericUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/kernelUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/modelUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/numba_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/Util/showcaseAllKernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/GPy_ABCD/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:36:25.791763 GPy-ABCD-1.2/GPy_ABCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-30 22:36:25.000000 GPy-ABCD-1.2/GPy_ABCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-30 22:36:25.000000 GPy-ABCD-1.2/GPy_ABCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:36:25.000000 GPy-ABCD-1.2/GPy_ABCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-30 22:36:25.000000 GPy-ABCD-1.2/GPy_ABCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 22:36:25.000000 GPy-ABCD-1.2/GPy_ABCD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-30 22:36:25.795763 GPy-ABCD-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:36:25.795763 GPy-ABCD-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-30 22:36:11.000000 GPy-ABCD-1.2/setup.py
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/grammar.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/grammar.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/kernelExpressionOperations.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/kernelExpressionOperations.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/kernelInterpretation.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/kernelInterpretation.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpansion/kernelOperations.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpansion/kernelOperations.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/base.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/base.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/change.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/change.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/commutative_base.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/commutative_base.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/KernelExpressions/commutatives.py` & `GPy-ABCD-1.2/GPy_ABCD/KernelExpressions/commutatives.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/baseKernels.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/baseKernels.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/changeOperators.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/changeOperators.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/changeWindowShiftedSides.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/changeWindowShiftedSides.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/changeWindowThreePart.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/changeWindowThreePart.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/linearKernel.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/linearKernel.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/periodicKernel.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/periodicKernel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 import numpy as np
 from scipy.special import i0, i1
 from GPy.kern.src.kern import Kern
 from GPy.core.parameterization import Param
 from paramz.transformations import Logexp
 from paramz.caching import Cache_this
 
+from GPy_ABCD.Util.numba_types import *
+from GPy_ABCD.Util.benchmarking import compare_implementations, numba_comparisons
+
+
+@njit(f8A(f8A))
+def _embi0(x): # == exp(-x) * besseli(0, x) => 9.8.2 Abramowitz & Stegun (http://people.math.sfu.ca/~cbm/aands/page_378.htm)
+    y = 3.75 / x # The below is an efficient polynomial computation
+    f = 0.39894228 + (0.01328592 + (0.00225319 + (-0.00157565 + (0.00916281 + (-0.02057706 + (0.02635537 + (-0.01647633 + (0.00392377)*y)*y)*y)*y)*y)*y)*y)*y
+    return f / np.sqrt(x)
+@njit(f8A(f8A))
+def _embi1(x): # == exp(-x) * besseli(1, x) => 9.8.4 Abramowitz & Stegun (http://people.math.sfu.ca/~cbm/aands/page_378.htm)
+    y = 3.75 / x # The below is an efficient polynomial computation
+    f = 0.39894228 + (-0.03988024 + (-0.00362018 + (0.00163801 + (-0.01031555 + (0.02282967 + (-0.02895312 + (0.01787654 + (-0.00420059)*y)*y)*y)*y)*y)*y)*y)*y
+    return f / np.sqrt(x)
+@njit(f8A(f8A))
+def _embi0min1(x): # == embi0(x) - embi1(x)
+    y = 3.75 / x # The below is an efficient polynomial computation (with the 0-th power term equal to 0)
+    f = (0.05316616 + (0.00587337 + (-0.00321366 + (0.01947836 + (-0.04340673 + (0.05530849 + (-0.03435287 + (0.00812436)*y)*y)*y)*y)*y)*y)*y)*y
+    return f / np.sqrt(x)
+
 
 # Based on GPy's StdPeriodic kernel and gaussianprocess.org/gpml/code/matlab/cov/covPeriodicNoDC.m
 class PureStdPeriodicKernel(Kern):
-    """
+    '''
     The standard periodic kernel due to MacKay (1998) can be decomposed into a sum of a periodic and a constant component;
     this kernel is the purely periodic component, as mentioned in:
     Lloyd, James Robert; Duvenaud, David Kristjanson; Grosse, Roger Baker; Tenenbaum, Joshua B.; Ghahramani, Zoubin (2014):
         Automatic construction and natural-language description of nonparametric regression models.
         In. National Conference on Artificial Intelligence, 7/27/2014, pp. 1242–1250.
 
     Note: because of its strict nature, this kernel will fit accurately only purely periodic data;
@@ -33,93 +53,67 @@
     :param lengthscale: the lengthscale :math:`\l`.
     :type lengthscale: array or list of the appropriate size (or float if there is only one lengthscale parameter)
     :param active_dims: indices of dimensions which are used in the computation of the kernel
     :type active_dims: array or list of the appropriate size
     :param name: Name of the kernel for output
     :type String
     :rtype: Kernel object
-    """
+    '''
 
     def __init__(self, input_dim: int, variance: float = 1., period: float = 2.*np.pi, lengthscale: float = 2.*np.pi,
                  active_dims: int = None, name: str = 'pure_std_periodic') -> None:
         super(PureStdPeriodicKernel, self).__init__(input_dim, active_dims, name)
 
         self.name = name
 
         if period is not None:
             period = np.asarray(period)
-            assert period.size == input_dim, "bad number of periods"
+            assert period.size == input_dim, 'bad number of periods'
         else:
             period = 2.*np.pi * np.ones(input_dim)
         if lengthscale is not None:
             lengthscale = np.asarray(lengthscale)
-            assert lengthscale.size == input_dim, "bad number of lengthscales"
+            assert lengthscale.size == input_dim, 'bad number of lengthscales'
         else:
             lengthscale = 2.*np.pi * np.ones(input_dim)
 
         self.variance = Param('variance', variance, Logexp())
-        assert self.variance.size == 1, "Variance size must be one"
+        assert self.variance.size == 1, 'Variance size must be one'
         self.period = Param('period', period, Logexp())
         self.lengthscale = Param('lengthscale', lengthscale, Logexp())
 
         self.link_parameters(self.variance, self.period, self.lengthscale)
 
     def to_dict(self):
         input_dict = super(PureStdPeriodicKernel, self)._save_to_input_dict()
-        input_dict["class"] = "BesselShiftedPeriodic"
-        input_dict["variance"] = self.variance.values.tolist()
-        input_dict["period"] = self.period.values.tolist()
-        input_dict["lengthscale"] = self.lengthscale.values.tolist()
+        input_dict['class'] = 'BesselShiftedPeriodic'
+        input_dict['variance'] = self.variance.values.tolist()
+        input_dict['period'] = self.period.values.tolist()
+        input_dict['lengthscale'] = self.lengthscale.values.tolist()
         return input_dict
 
-    @staticmethod
-    def embi0(x): # == exp(-x) * besseli(0, x) => 9.8.2 Abramowitz & Stegun (http://people.math.sfu.ca/~cbm/aands/page_378.htm)
-        y = 3.75 / x # The below is an efficient polynomial computation
-        f = 0.39894228 + (0.01328592 + (0.00225319 + (-0.00157565 + (0.00916281 + (-0.02057706 + (0.02635537 + (-0.01647633 + (0.00392377)*y)*y)*y)*y)*y)*y)*y)*y
-        return f / np.sqrt(x)
-    @staticmethod
-    def embi1(x): # == exp(-x) * besseli(1, x) => 9.8.4 Abramowitz & Stegun (http://people.math.sfu.ca/~cbm/aands/page_378.htm)
-        y = 3.75 / x # The below is an efficient polynomial computation
-        f = 0.39894228 + (-0.03988024 + (-0.00362018 + (0.00163801 + (-0.01031555 + (0.02282967 + (-0.02895312 + (0.01787654 + (-0.00420059)*y)*y)*y)*y)*y)*y)*y)*y
-        return f / np.sqrt(x)
-    @staticmethod
-    def embi0min1(x): # == embi0(x) - embi1(x)
-        y = 3.75 / x # The below is an efficient polynomial computation (with the 0-th power term equal to 0)
-        f = (0.05316616 + (0.00587337 + (-0.00321366 + (0.01947836 + (-0.04340673 + (0.05530849 + (-0.03435287 + (0.00812436)*y)*y)*y)*y)*y)*y)*y)*y
-        return f / np.sqrt(x)
-
     @Cache_this(limit = 3)
-    def K(self, X, X2=None):
+    def K(self, X, X2 = None):
         if X2 is None: X2 = X
         cos_term = np.cos((2 * np.pi / self.period) * (X - X2.T))
         invL2 = 1 / self.lengthscale ** 2
 
         if np.any(self.lengthscale > 1e4): # Limit for l -> infinity
             return self.variance * cos_term
         elif np.any(invL2 < 3.75):
             exp_term = np.exp(cos_term * invL2)
             bessel0 = i0(invL2)
             return self.variance * ((exp_term - bessel0) / (np.exp(invL2) - bessel0)) # The brackets prevent an overflow; want division first
         else:
             exp_term = np.exp((cos_term - 1) * invL2)
-            embi0 = self.embi0(invL2)
-            return self.variance * ((exp_term - embi0) / (1 - embi0))  # The brackets prevent an overflow; want division first
-    # @Cache_this(limit = 3)
-    # def K(self, X, X2 = None):
-    #     if X2 is None: X2 = X
-    #     cos_term = np.cos(2 * np.pi * (X - X2.T) / self.period)
-    #
-    #     if np.any(self.lengthscale > 1e4): # Limit for l -> infinity
-    #         return self.variance * cos_term
-    #     else:
-    #         # Overflow on exp and i0 by going backwards from sys.float_info.max (1.7976931348623157e+308): 1/l^2 < 709.782712893384
-    #         invL2 = np.clip(1 / np.where(self.lengthscale < 1e-100, 1e-200, self.lengthscale ** 2), 0, 705)
-    #         exp_term = np.exp(cos_term * invL2)
-    #         bessel0 = i0(invL2)
-    #         return self.variance * ((exp_term - bessel0) / (np.exp(invL2) - bessel0)) # The brackets prevent an overflow; want division first
+            embi0 = _embi0(invL2)
+            return self.variance * ((exp_term - embi0) / (1 - embi0)) # The brackets prevent an overflow; want division first
+        # invL2 = 1 / self.lengthscale ** 2
+        # bessel0 = i0(invL2)
+        # return _K(self.variance, self.period, self.lengthscale, invL2, bessel0, X, X if X2 is None else X2)
 
     def Kdiag(self, X): # Correct; nice and fast
         ret = np.empty(X.shape[0])
         ret[:] = self.variance
         return ret
 
     def update_gradients_full(self, dL_dK, X, X2 = None):
@@ -131,15 +125,16 @@
 
         if np.any(self.lengthscale > 1e4):  # Limit for l -> infinity
             dK_dV = cos_term # K / V
 
             dK_dp = (self.variance / self.period) * trig_arg * sin_term
 
             # This is 0 in the limit, but best to set it to a small non-0 value
-            dK_dl = 1e-4 / self.lengthscale
+            dK_dl = np.empty_like(dL_dK)
+            dK_dl[:, :] = 1e-4 / self.lengthscale[0]
         elif np.any(invL2 < 3.75):
             bessel0 = i0(invL2)
             bessel1 = i1(invL2)
             eInvL2 = np.exp(invL2)
             dInvL2_dl = -2 * invL2 / self.lengthscale # == -2 / l^3
 
             denom = eInvL2 - bessel0
@@ -149,18 +144,18 @@
 
             dK_dV = K_no_Var
 
             dK_dp = (self.variance / self.period) * invL2 * trig_arg * sin_term * exp_term / denom
 
             dK_dl = dInvL2_dl * self.variance * ( (cos_term * exp_term - bessel1) - K_no_Var * (eInvL2 - bessel1) ) / denom
         else:
-            embi0 = self.embi0(invL2)
-            # embi1 = self.embi1(invL2)
+            embi0 = _embi0(invL2)
+            # embi1 = _embi1(invL2)
             # embi0min1 = embi0 - embi1
-            embi0min1 = self.embi0min1(invL2)
+            embi0min1 = _embi0min1(invL2)
             dInvL2_dl = -2 * invL2 / self.lengthscale # == -2 / l^3
 
             denom = 1 - embi0
             exp_term = np.exp((cos_term - 1) * invL2)
             K_no_Var = (exp_term - embi0) / denom # == K / V; here just for clarity of further expressions
 
 
@@ -169,48 +164,18 @@
             dK_dp = (self.variance / self.period) * invL2 * trig_arg * sin_term * exp_term / denom # I.e. SAME as the above case at this abstraction level
 
             dK_dl = dInvL2_dl * self.variance * ( (cos_term - 1) * exp_term + embi0min1 - K_no_Var * embi0min1 ) / denom
 
         self.variance.gradient = np.sum(dL_dK * dK_dV)
         self.period.gradient = np.sum(dL_dK * dK_dp)
         self.lengthscale.gradient = np.sum(dL_dK * dK_dl)
-    # def update_gradients_full(self, dL_dK, X, X2 = None):
-    #     if X2 is None: X2 = X
-    #     trig_arg = 2 * np.pi * (X - X2.T) / self.period
-    #     cos_term = np.cos(trig_arg)
-    #     sin_term = np.sin(trig_arg)
-    #
-    #     if np.any(self.lengthscale > 1e4):  # Limit for l -> infinity
-    #         dK_dV = cos_term # K / V
-    #
-    #         dK_dp = self.variance * trig_arg * sin_term / self.period
-    #
-    #         # This is 0 in the limit, but best to set it to a small non-0 value
-    #         dK_dl = 1e-4 / self.lengthscale
-    #     else:
-    #         # Overflow on exp and i0 by going backwards from sys.float_info.max (1.7976931348623157e+308): 1/l^2 < 709.782712893384
-    #         invL2 = np.clip(1 / np.where(self.lengthscale < 1e-100, 1e-200, self.lengthscale ** 2), 0, 705)
-    #         bessel0 = i0(invL2)
-    #         bessel1 = i1(invL2)
-    #         eInvL2 = np.exp(invL2)
-    #         denom = eInvL2 - bessel0
-    #         exp_term = np.exp(cos_term * invL2)
-    #
-    #         dK_dV = (exp_term - bessel0) / denom # = K / V
-    #
-    #         dK_dp = (self.variance * invL2 * trig_arg * sin_term / self.period) * (exp_term / denom) # exp terms division separate because of overflow risk
-    #
-    #         K = self.variance * dK_dV
-    #         dInvL2_dl = -2 / np.where(self.lengthscale < 1e-100, 1e-300, self.lengthscale ** 3)
-    #         dK_dl = dInvL2_dl * ( self.variance * ((cos_term * exp_term - bessel1) / denom) - K * ((eInvL2 - bessel1) / denom) ) # The brackets prevent some overflows; want those divisions first
-    #
-    #     self.variance.gradient = np.sum(dL_dK * dK_dV)
-    #     self.period.gradient = np.sum(dL_dK * dK_dp)
-    #     self.lengthscale.gradient = np.sum(dL_dK * dK_dl)
-
+        # invL2 = 1 / self.lengthscale ** 2
+        # bessel0 = i0(invL2)
+        # bessel1 = i1(invL2)
+        # self.variance.gradient, self.period.gradient, self.lengthscale.gradient = _update_gradients_full(self.variance, self.period, self.lengthscale, invL2, bessel0, bessel1, dL_dK, X, X if X2 is None else X2)
 
 
     # Unused functions for a possible version of this class as a subclass of Stationary
 
     # def K_of_r(self, r):
     #     cos_term = np.cos(2 * np.pi * r / self.period)
     #
@@ -232,7 +197,85 @@
     #         return - self.variance * (trig_arg / r) * sin_term
     #     else:
     #         invL2 = np.sum(1 / self.lengthscale ** 2)
     #         exp_term = np.exp(cos_term * invL2)
     #         return - self.variance * invL2 * (trig_arg / r) * sin_term * exp_term / (np.exp(invL2) - i0(invL2))
 
 
+
+## numba versions of some methods
+
+# from GPy_ABCD.Util.benchmarking import numba_comparisons
+# numba_comparisons(_embi0, f8A(f8A), n = 200, args = [x])
+
+
+# # if X2 is None: X2 = X
+# # invL2 = 1 / lengthscale ** 2
+# # bessel0 = i0(invL2)
+# # @njit(f8A2(f8A, f8A, f8A, f8A, f8A, f8A2, f8A2)) # The numpy version is faster
+# def _K(variance, period, lengthscale, invL2, bessel0, X, X2):
+#     cos_term = np.cos((2 * np.pi / period) * (X - X2.T))
+#
+#     if np.any(lengthscale > 1e4): # Limit for l -> infinity
+#         return variance * cos_term
+#     elif np.any(invL2 < 3.75):
+#         exp_term = np.exp(cos_term * invL2)
+#         return variance * ((exp_term - bessel0) / (np.exp(invL2) - bessel0)) # The brackets prevent an overflow; want division first
+#     else:
+#         exp_term = np.exp((cos_term - 1) * invL2)
+#         embi0 = _embi0(invL2)
+#         return variance * ((exp_term - embi0) / (1 - embi0)) # The brackets prevent an overflow; want division first
+
+
+
+# # invL2 = 1 / lengthscale ** 2
+# # bessel0 = i0(invL2)
+# # bessel1 = i1(invL2)
+# # @njit(nTup(f8, f8, f8)(f8A, f8A, f8A, f8A, f8A, f8A, f8A2, f8A2, f8A2)) # The numpy version is faster
+# def _update_gradients_full(variance, period, lengthscale, invL2, bessel0, bessel1, dL_dK, X, X2):
+#     trig_arg = (2 * np.pi / period) * (X - X2.T)
+#     cos_term = np.cos(trig_arg)
+#     sin_term = np.sin(trig_arg)
+#
+#     if np.any(lengthscale > 1e4):  # Limit for l -> infinity
+#         dK_dV = cos_term # K / V
+#
+#         dK_dp = (variance / period) * trig_arg * sin_term
+#
+#         # This is 0 in the limit, but best to set it to a small non-0 value
+#         dK_dl = np.empty_like(dL_dK)
+#         dK_dl[:,:] = 1e-4 / lengthscale[0]
+#     elif np.any(invL2 < 3.75):
+#         eInvL2 = np.exp(invL2)
+#         dInvL2_dl = -2 * invL2 / lengthscale # == -2 / l^3
+#
+#         denom = eInvL2 - bessel0
+#         exp_term = np.exp(cos_term * invL2)
+#         K_no_Var = (exp_term - bessel0) / denom # == K / V; here just for clarity of further expressions
+#
+#
+#         dK_dV = K_no_Var
+#
+#         dK_dp = (variance / period) * invL2 * trig_arg * sin_term * exp_term / denom
+#
+#         dK_dl = dInvL2_dl * variance * ( (cos_term * exp_term - bessel1) - K_no_Var * (eInvL2 - bessel1) ) / denom
+#     else:
+#         embi0 = _embi0(invL2)
+#         # embi1 = _embi1(invL2)
+#         # embi0min1 = embi0 - embi1
+#         embi0min1 = _embi0min1(invL2)
+#         dInvL2_dl = -2 * invL2 / lengthscale # == -2 / l^3
+#
+#         denom = 1 - embi0
+#         exp_term = np.exp((cos_term - 1) * invL2)
+#         K_no_Var = (exp_term - embi0) / denom # == K / V; here just for clarity of further expressions
+#
+#
+#         dK_dV = K_no_Var
+#
+#         dK_dp = (variance / period) * invL2 * trig_arg * sin_term * exp_term / denom # I.e. SAME as the above case at this abstraction level
+#
+#         dK_dl = dInvL2_dl * variance * ( (cos_term - 1) * exp_term + embi0min1 - K_no_Var * embi0min1 ) / denom
+#
+#     return np.sum(dL_dK * dK_dV), np.sum(dL_dK * dK_dp), np.sum(dL_dK * dK_dl) # variance.gradient, period.gradient, lengthscale.gradient
+
+
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Kernels/sigmoidalKernels.py` & `GPy-ABCD-1.2/GPy_ABCD/Kernels/sigmoidalKernels.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,49 @@
 import numpy as np
 from abc import abstractmethod
 from GPy.kern.src.basis_funcs import BasisFuncKernel
 from GPy.core.parameterization import Param
 from paramz.transformations import Logexp
 from paramz.caching import Cache_this
 
+from GPy_ABCD.Util.numba_types import *
+# from GPy_ABCD.Util.benchmarking import numba_comparisons
+
+
+@njit(f8A2(f8A2))
+def _sigmoid_function(arg): return (1 + arg / (1 + np.abs(arg))) / 2
+@njit(f8A2(f8A2))
+def _sigmoid_function_d(arg): return 0.5 / (1 + np.abs(arg)) ** 2
+# Since arg is usually (x - l) / s, derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
+#       x: * 1/s
+#       l: * -1/s
+#       s: * -(x-l)/s^2, i.e. * -arg/s
+# When arg is (x - l - w) / (-s) [NOTE THE -s], derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
+#       x: * -1/s
+#       l: * 1/s
+#       w: * 1/s
+#       s: * (x-l-w)/(-s)^2, i.e. * -argW/s
+
+@njit(f8(f8))
+def _core_sigmoid_function(arg): return arg / (1 + np.abs(arg))
+# NOTE: This function can be used to compute the maximum height of the sum of opposite sigmoidals - 1 by feeding it arg = w / (2 * s)
+# Let arg = (x - l) / s and argW (x - l - w) / (-s) [NOTE THE -s]
+# This is the height of sig(arg) + sig(argW) - 1 for midpoint x: l + w/2 in both args (which become w/2s)
+# so 2*sig(w/2s) - 1 = the core sigmoid ([-1,1]) on +ve values because of +ve w and s: core_sig(w/2s)
+@njit(f8(f8))
+def _inv_core_sigmoid_d(arg): return - 1 / arg ** 2
+# NOTE: This function comes up in computing the derivatives of the scaled (to 1) version of the above sum of sigmoidals
+# Since arg  is always  w / (2 * s), derivatives are just _inv_core_sigmoid_d(arg) * ...
+#       w: * 1/2s
+#       s: * -w/(2s^2), i.e. * -arg/s
+
 
 
 class SigmoidalKernelBase(BasisFuncKernel):
-    """
-    Abstract superclass for sigmoidal kernels
-    """
+    '''Abstract superclass for sigmoidal kernels'''
 
     def __init__(self, input_dim: int, reverse: bool = False, variance: float = 1., location: float = 0., slope: float = 0.2,
                  active_dims: int = None, name: str = 'sigmoidal_kernel_base', fixed_slope = False) -> None:
         self.reverse = reverse
         super(SigmoidalKernelBase, self).__init__(input_dim, variance, active_dims, False, name)
         # TO REMOVE VARIANCE: comment line above; uncomment below; remove self.variance factors from subclass methods
         # super(BasisFuncKernel, self).__init__(input_dim, active_dims, name)
@@ -26,176 +55,178 @@
 
         self._fixed_slope = fixed_slope # Note: here to be used by subclasses, and changing it from the outside does not link the parameter
         if self._fixed_slope: self.slope = slope
         else:
             self.slope = Param('slope', slope, Logexp()) # This +ve constraint makes non-reverse sigmoids only fit (+ve or -ve) curves going away from 0; similarly for other kernels
             self.link_parameter(self.slope)
 
-    @staticmethod
-    def _sigmoid_function(arg): return (1 + arg / (1 + abs(arg))) / 2
-    @staticmethod
-    def _sigmoid_function_d(arg): return 0.5 / (1 + abs(arg)) ** 2
-    # Since arg is usually (x - l) / s, derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
-    #       x: * 1/s
-    #       l: * -1/s
-    #       s: * -(x-l)/s^2, i.e. * -arg/s
-    # When arg is (x - l - w) / (-s) [NOTE THE -s], derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
-    #       x: * -1/s
-    #       l: * 1/s
-    #       w: * 1/s
-    #       s: * (x-l-w)/(-s)^2, i.e. * -argW/s
-
-    @staticmethod
-    def _core_sigmoid_function(arg): return arg / (1 + abs(arg))
-    # NOTE: This function can be used to compute the maximum height of the sum of opposite sigmoidals - 1 by feeding it arg = w / (2 * s)
-    # Let arg = (x - l) / s and argW (x - l - w) / (-s) [NOTE THE -s]
-    # This is the height of sig(arg) + sig(argW) - 1 for midpoint x: l + w/2 in both args (which become w/2s)
-    # so 2*sig(w/2s) - 1 = the core sigmoid ([-1,1]) on +ve values because of +ve w and s: core_sig(w/2s)
-    @staticmethod
-    def _inv_core_sigmoid_d(arg): return - 1 / arg ** 2
-    # NOTE: This function comes up in computing the derivatives of the scaled (to 1) version of the above sum of sigmoidals
-    # Since arg  is always  w / (2 * s), derivatives are just _inv_core_sigmoid_d(arg) * ...
-    #       w: * 1/2s
-    #       s: * -w/(2s^2), i.e. * -arg/s
-
     def update_gradients_diag(self, dL_dKdiag, X):
         raise NotImplementedError
 
 
 
 # Based on LogisticBasisFuncKernel
 class SigmoidalKernel(SigmoidalKernelBase):
-    """
-    Sigmoidal kernel
-    (ascending by default; descending by reverse=True)
-    """
+    '''Sigmoidal kernel
+    (ascending by default; descending by reverse = True)'''
 
     def __init__(self, input_dim: int, reverse: bool = False, variance: float = 1., location: float = 0., slope: float = 0.2,
                  active_dims: int = None, name: str = 'sigmoidal', fixed_slope = False) -> None:
         super(SigmoidalKernel, self).__init__(input_dim, reverse, variance, location, slope, active_dims, name, fixed_slope)
 
-    @Cache_this(limit=3, ignore_args=())
+    @Cache_this(limit = 3)
     def _phi(self, X):
-        asc = self._sigmoid_function((X - self.location) / self.slope)
-        return 1 - asc if self.reverse else asc
+        return _phi_S(self.location[0], self.slope if self._fixed_slope else self.slope[0], self.reverse, X)
 
-    def update_gradients_full(self, dL_dK, X, X2=None):
+    def update_gradients_full(self, dL_dK, X, X2 = None):
         super(SigmoidalKernel, self).update_gradients_full(dL_dK, X, X2)
+        phi1 = self.phi(X)
+        if phi1.ndim != 2: phi1 = phi1[:, None]
+
         if X2 is None or X is X2:
-            phi1 = self.phi(X)
-            if phi1.ndim != 2:
-                phi1 = phi1[:, None]
-
-            arg = (X - self.location) / self.slope
-            sig_d = self._sigmoid_function_d(arg)
-
-            dphi1_dl = sig_d / (-self.slope)
-            self.location.gradient = np.sum(self.variance * 2 * (dL_dK * phi1.dot(dphi1_dl.T)).sum())
-
-            if not self._fixed_slope:
-                dphi1_ds = sig_d * (-arg / self.slope)
-                self.slope.gradient = np.sum(self.variance * 2 * (dL_dK * phi1.dot(dphi1_ds.T)).sum())
+            self.location.gradient, slope_gradient = _update_gradients_full_S_1(self.variance[0], self.location[0],
+                self.slope if self._fixed_slope else self.slope[0], self._fixed_slope, phi1, dL_dK, X)
+            if not self._fixed_slope: self.slope.gradient = slope_gradient
         else:
-            phi1 = self.phi(X)
             phi2 = self.phi(X2)
-            if phi1.ndim != 2:
-                phi1 = phi1[:, None]
-                phi2 = phi2[:, None]
-
-            arg, arg2 = (X - self.location) / self.slope, (X2 - self.location) / self.slope
-            sig_d, sig_d2 = self._sigmoid_function_d(arg), self._sigmoid_function_d(arg2)
-
-            dphi1_dl, dphi2_dl = sig_d / (-self.slope), sig_d2 / (-self.slope)
-            self.location.gradient = np.sum(self.variance * (dL_dK * (phi1.dot(dphi2_dl.T) + phi2.dot(dphi1_dl.T))).sum())
-            self.location.gradient = np.where(np.isnan(self.location.gradient), 0, self.location.gradient)
-
-            if not self._fixed_slope:
-                dphi1_ds = sig_d * (-arg / self.slope)
-                dphi2_ds = sig_d2 * (-arg2 / self.slope)
-                self.slope.gradient = np.sum(self.variance * (dL_dK * (phi1.dot(dphi2_ds.T) + phi2.dot(dphi1_ds.T))).sum())
-                self.slope.gradient = np.where(np.isnan(self.slope.gradient), 0, self.slope.gradient)
+            if phi1.ndim != 2: phi2 = phi2[:, None]
+
+            self.location.gradient, slope_gradient = _update_gradients_full_S_2(self.variance[0], self.location[0],
+                self.slope if self._fixed_slope else self.slope[0], self._fixed_slope, phi1, phi2, dL_dK, X, X2)
+            if not self._fixed_slope: self.slope.gradient = slope_gradient
 
         if self.reverse: # Works this simply (a single sign flip per product above)
             self.location.gradient = - self.location.gradient
             if not self._fixed_slope: self.slope.gradient = - self.slope.gradient
 
+@njit(f8A2(f8, f8, b1, f8A2)) # Almost 2x faster than numpy version
+def _phi_S(location, slope, reverse, X):
+    asc = _sigmoid_function((X - location) / slope)
+    return 1 - asc if reverse else asc
+
+@njit(nTup(f8, f8)(f8, f8, f8, b1, f8A2, f8A2, f8A2)) # 1.5x faster than numpy version
+def _update_gradients_full_S_1(variance, location, slope, _fixed_slope, phi1, dL_dK, X):
+    arg = (X - location) / slope
+    sig_d = _sigmoid_function_d(arg)
+
+    dphi1_dl = sig_d / (-slope)
+    location_gradient = variance * 2 * (dL_dK * phi1.dot(dphi1_dl.T)).sum()
+    if np.isnan(location_gradient): location_gradient = 0.0
+
+    if not _fixed_slope:
+        dphi1_ds = sig_d * (-arg / slope)
+        slope_gradient = variance * 2 * (dL_dK * phi1.dot(dphi1_ds.T)).sum()
+        if np.isnan(slope_gradient): slope_gradient = 0.0
+    else: slope_gradient = 1.0 # Going to discard it anyway
+
+    return location_gradient, slope_gradient
+
+@njit(nTup(f8, f8)(f8, f8, f8, b1, f8A2, f8A2, f8A2, f8A2, f8A2))
+def _update_gradients_full_S_2(variance, location, slope, _fixed_slope, phi1, phi2, dL_dK, X, X2):
+    arg, arg2 = (X - location) / slope, (X2 - location) / slope
+    sig_d, sig_d2 = _sigmoid_function_d(arg), _sigmoid_function_d(arg2)
+
+    dphi1_dl, dphi2_dl = sig_d / (-slope), sig_d2 / (-slope)
+    location_gradient = variance * (dL_dK * (phi1.dot(dphi2_dl.T) + phi2.dot(dphi1_dl.T))).sum()
+    if np.isnan(location_gradient): location_gradient = 0.0
+
+    if not _fixed_slope:
+        dphi1_ds = sig_d * (-arg / slope)
+        dphi2_ds = sig_d2 * (-arg2 / slope)
+        slope_gradient = variance * (dL_dK * (phi1.dot(dphi2_ds.T) + phi2.dot(dphi1_ds.T))).sum()
+        if np.isnan(slope_gradient): slope_gradient = 0.0
+    else: slope_gradient = 1.0 # Going to discard it anyway
+
+    return location_gradient, slope_gradient
+
 
 
 class SigmoidalIndicatorKernel(SigmoidalKernelBase):
-    """
-    Sigmoidal indicator function kernel with parametrised start location and width:
+    '''Sigmoidal indicator function kernel with parametrised start location and width:
     ascendingSigmoid(location) + (1 - ascendingSigmoid(stop_location + width)) - 1, i.e. ascendingSigmoid(location) - ascendingSigmoid(location + width)
-    (hat if width > 0, and positive-well otherwise; can flip from one to the other by reverse=True)
-    """
+    (hat if width > 0, and positive-well otherwise; can flip from one to the other by reverse=True)'''
 
     def __init__(self, input_dim: int, reverse: bool = False, variance: float = 1., location: float = 0., slope: float = 0.2, width: float = 1.,
                  active_dims: int = None, name: str = 'sigmoidal_indicator', fixed_slope = False) -> None:
         super(SigmoidalIndicatorKernel, self).__init__(input_dim, reverse, variance, location, slope, active_dims, name, fixed_slope)
         self.width = Param('width', width, Logexp())
         self.link_parameters(self.width)
 
     @Cache_this(limit = 3)
     def _phi(self, X):
-        asc = self._sigmoid_function((X - self.location) / self.slope)
-        desc = self._sigmoid_function((X - self.location - self.width) / (-self.slope))
-        height = self._core_sigmoid_function(self.width / (2 * self.slope))
-        hat = (asc + desc - 1) / height
-        return 1 - hat if self.reverse else hat
+        return _phi_SI(self.location[0], self.slope if self._fixed_slope else self.slope[0], self.width[0], self.reverse, X)
 
-    def update_gradients_full(self, dL_dK, X, X2=None):
+    def update_gradients_full(self, dL_dK, X, X2 = None):
         super(SigmoidalIndicatorKernel, self).update_gradients_full(dL_dK, X, X2)
         if X2 is None: X2 = X
 
         phi1 = self.phi(X)
         phi2 = self.phi(X2) if X2 is not X else phi1
         if phi1.ndim != 2:
             phi1 = phi1[:, None]
             phi2 = phi2[:, None] if X2 is not X else phi1
 
-        arg, arg2 = (X - self.location) / self.slope, (X2 - self.location) / self.slope
-        argW, argW2 = (X - self.location - self.width) / (-self.slope), (X2 - self.location - self.width) / (-self.slope)
-        sig_d, sig_d2 = self._sigmoid_function_d(arg), self._sigmoid_function_d(arg2)
-        sig_dW, sig_dW2 = self._sigmoid_function_d(argW), self._sigmoid_function_d(argW2)
-
-        numerator1 = self._sigmoid_function(arg) + self._sigmoid_function(argW) - 1 # asc1 + desc1 - 1
-        numerator2 = self._sigmoid_function(arg2) + self._sigmoid_function(argW2) - 1 # asc2 + desc2 - 1
-
-        height_arg = self.width / (2 * self.slope)
-        inv_height = 1 / self._core_sigmoid_function(height_arg)
-        inv_height_d = self._inv_core_sigmoid_d(height_arg)
-        dinvheight_dw = inv_height_d / (2 * self.slope)
-        dinvheight_ds = inv_height_d * (-height_arg / self.slope)
-
-        # Repeated _sigmoid_function_d reference:
-        # Since arg is usually (x - l) / s, derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
-        #       x: * 1/s
-        #       l: * -1/s
-        #       s: * -(x-l)/s^2, i.e. * -arg/s
-        # When arg is (x - l - w) / (-s) [NOTE THE -s], derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
-        #       x: * -1/s
-        #       l: * 1/s
-        #       w: * 1/s
-        #       s: * (x-l-w)/(-s)^2, i.e. * -argW/s
-
-        dphi1_dl = ((- sig_d + sig_dW) / self.slope) * inv_height #+ (asc + desc) * dinvheight_dl, which is 0
-        dphi2_dl = ((- sig_d2 + sig_dW2) / self.slope) * inv_height #+ (asc + desc) * dinvheight_dl, which is 0
-        self.location.gradient = np.sum(self.variance * (dL_dK * (phi1.dot(dphi2_dl.T) + phi2.dot(dphi1_dl.T))).sum())
-        self.location.gradient = np.where(np.isnan(self.location.gradient), 0, self.location.gradient)
-
-        if not self._fixed_slope:
-            dphi1_ds = ((sig_d * arg + sig_dW * argW) / (-self.slope)) * inv_height + numerator1 * dinvheight_ds
-            dphi2_ds = ((sig_d2 * arg2 + sig_dW2 * argW2) / (-self.slope)) * inv_height + numerator2 * dinvheight_ds
-            self.slope.gradient = np.sum(self.variance * (dL_dK * (phi1.dot(dphi2_ds.T) + phi2.dot(dphi1_ds.T))).sum())
-            self.slope.gradient = np.where(np.isnan(self.slope.gradient), 0, self.slope.gradient)
-
-        dphi1_dw = (sig_dW / self.slope) * inv_height + numerator1 * dinvheight_dw # d(asc)_dw = 0
-        dphi2_dw = (sig_dW2 / self.slope) * inv_height + numerator2 * dinvheight_dw # d(asc)_dw = 0
-        self.width.gradient = np.sum(self.variance * (dL_dK * (phi1.dot(dphi2_dw.T) + phi2.dot(dphi1_dw.T))).sum())
-        self.width.gradient = np.where(np.isnan(self.width.gradient), 0, self.width.gradient)
+        self.location.gradient, slope_gradient, self.width.gradient = _update_gradients_full_SI(
+            self.variance[0], self.location[0], self.slope if self._fixed_slope else self.slope[0], self.width[0],
+            self.reverse, self._fixed_slope, phi1, phi2, dL_dK, X, X2)
+        if not self._fixed_slope: self.slope.gradient = slope_gradient
+
+@njit(f8A2(f8, f8, f8, b1, f8A2)) # 4.6x faster than numpy version
+def _phi_SI(location, slope, width, reverse, X):
+    asc = _sigmoid_function((X - location) / slope)
+    desc = _sigmoid_function((X - location - width) / (-slope))
+    height = _core_sigmoid_function(width / (2 * slope))
+    hat = (asc + desc - 1) / height
+    return 1 - hat if reverse else hat
+
+@njit(nTup(f8, f8, f8)(f8, f8, f8, f8, b1, b1, f8A2, f8A2, f8A2, f8A2, f8A2)) # 1.45x faster than numpy version
+def _update_gradients_full_SI(variance, location, slope, width, reverse, _fixed_slope, phi1, phi2, dL_dK, X, X2):
+    arg, arg2 = (X - location) / slope, (X2 - location) / slope
+    argW, argW2 = (X - location - width) / (-slope), (X2 - location - width) / (-slope)
+    sig_d, sig_d2 = _sigmoid_function_d(arg), _sigmoid_function_d(arg2)
+    sig_dW, sig_dW2 = _sigmoid_function_d(argW), _sigmoid_function_d(argW2)
+
+    numerator1 = _sigmoid_function(arg) + _sigmoid_function(argW) - 1 # asc1 + desc1 - 1
+    numerator2 = _sigmoid_function(arg2) + _sigmoid_function(argW2) - 1 # asc2 + desc2 - 1
+
+    height_arg = width / (2 * slope)
+    inv_height = 1 / _core_sigmoid_function(height_arg)
+    inv_height_d = _inv_core_sigmoid_d(height_arg)
+    dinvheight_dw = inv_height_d / (2 * slope)
+    dinvheight_ds = inv_height_d * (-height_arg / slope)
+
+    # Repeated _sigmoid_function_d reference:
+    # Since arg is usually (x - l) / s, derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
+    #       x: * 1/s
+    #       l: * -1/s
+    #       s: * -(x-l)/s^2, i.e. * -arg/s
+    # When arg is (x - l - w) / (-s) [NOTE THE -s], derivatives by the constituent terms are just _sigmoid_function_d(arg) * ...
+    #       x: * -1/s
+    #       l: * 1/s
+    #       w: * 1/s
+    #       s: * (x-l-w)/(-s)^2, i.e. * -argW/s
 
+    dphi1_dl = ((- sig_d + sig_dW) / slope) * inv_height #+ (asc + desc) * dinvheight_dl, which is 0
+    dphi2_dl = ((- sig_d2 + sig_dW2) / slope) * inv_height #+ (asc + desc) * dinvheight_dl, which is 0
+    location_gradient = variance * (dL_dK * (phi1.dot(dphi2_dl.T) + phi2.dot(dphi1_dl.T))).sum()
+    if np.isnan(location_gradient): location_gradient = 0.0
+
+    if not _fixed_slope:
+        dphi1_ds = ((sig_d * arg + sig_dW * argW) / (-slope)) * inv_height + numerator1 * dinvheight_ds
+        dphi2_ds = ((sig_d2 * arg2 + sig_dW2 * argW2) / (-slope)) * inv_height + numerator2 * dinvheight_ds
+        slope_gradient = variance * (dL_dK * (phi1.dot(dphi2_ds.T) + phi2.dot(dphi1_ds.T))).sum()
+        if np.isnan(slope_gradient): slope_gradient = 0.0
+    else: slope_gradient = 1.0 # Going to discard it anyway
+
+    dphi1_dw = (sig_dW / slope) * inv_height + numerator1 * dinvheight_dw # d(asc)_dw = 0
+    dphi2_dw = (sig_dW2 / slope) * inv_height + numerator2 * dinvheight_dw # d(asc)_dw = 0
+    width_gradient = variance * (dL_dK * (phi1.dot(dphi2_dw.T) + phi2.dot(dphi1_dw.T))).sum()
+    if np.isnan(width_gradient): width_gradient = 0.0
+
+    if reverse: # Works this simply (a single sign flip per product above)
+        location_gradient = - location_gradient
+        if not _fixed_slope: slope_gradient = - slope_gradient
+        width_gradient = - width_gradient
 
-        if self.reverse: # Works this simply (a single sign flip per product above)
-            self.location.gradient = - self.location.gradient
-            if not self._fixed_slope: self.slope.gradient = - self.slope.gradient
-            self.width.gradient = - self.width.gradient
+    return location_gradient, slope_gradient, width_gradient
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Models/model.py` & `GPy-ABCD-1.2/GPy_ABCD/Models/model.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Models/modelSearch.py` & `GPy-ABCD-1.2/GPy_ABCD/Models/modelSearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
     NOTE: Any code calling this function (however many nested levels in) should be within a "if __name__ == '__main__':" preamble for full OS-agnostic use.
     '''
     with Pool() as pool: return pool.starmap_async(fit_one_model, [(X, Y, kex, restarts, optimiser) for kex in k_exprs], int(len(k_exprs) / cpu_count()) + 1).get()
 
 
 def explore_model_space(X, Y,
-                        start_kernels: List[Union[str, KernelExpression]] = start_kernels['Default'], p_rules: List[Callable] = production_rules['Default'], utility_function: Callable = BIC,
-                        rounds: int = 2, beam: Union[int, List[int]] = [3, 2, 1], restarts: int = 5,
+                        start_kernels: List[Union[str, KernelExpression]] = start_kernels['Default'], p_rules: List[Callable] = production_rules['Default'],
+                        utility_function: Callable = BIC, rounds: int = 2, beam: Union[int, List[int]] = [3, 2, 1], restarts: int = 5,
                         model_list_fitter: Callable = fit_mods_parallel_processes, optimiser: str = GPy_optimisers[0],
                         verbose: bool = True) -> Tuple[List[GPModel], List[List[GPModel]], List[KernelExpression], List[GPModel], List[GPModel]]:
     '''Perform `rounds` rounds of kernel expansion followed by model fit starting from the given `start_kernels` with and expanding the best `buffer` of them with `p_rules` production rules
 
     NOTE: if the default `model_list_fitter` argument `fit_mods_parallel_processes` is used the function should be called from within a :code:`if __name__ == '__main__':` for full OS-agnostic use.
 
     :param start_kernels: the 0th-round starting kernels
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Util/dataAndPlottingUtil.py` & `GPy-ABCD-1.2/GPy_ABCD/Util/dataAndPlottingUtil.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Util/genericUtil.py` & `GPy-ABCD-1.2/GPy_ABCD/Util/genericUtil.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Util/kernelUtil.py` & `GPy-ABCD-1.2/GPy_ABCD/Util/kernelUtil.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Util/modelUtil.py` & `GPy-ABCD-1.2/GPy_ABCD/Util/modelUtil.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,14 @@
 
     m = GPRegression(X, Y, kernel)
     m.optimize_restarts(num_restarts = restarts, **kwargs)
 
     m.plot()
     print(m.kern)
     print(f'Log-Likelihood: {m.log_likelihood()}')
-    print(f'{score.__name__}: {score(m.log_likelihood(), len(X), m._size_transformed())}')
+    print(f'{score.__name__}: {score(m, m.log_likelihood(), len(X), m._size_transformed())}')
 
     plt.show()
 
     return m
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD/Util/showcaseAllKernels.py` & `GPy-ABCD-1.2/GPy_ABCD/Util/showcaseAllKernels.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD/__init__.py` & `GPy-ABCD-1.2/GPy_ABCD/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """GPy-ABCD - Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system"""
 
-__version__ = '1.1' # Change it in setup.py too
+__version__ = '1.2' # Change it in setup.py too
 __author__ = 'Thomas Fletcher <T-Fletcher@outlook.com>'
 # __all__ = []
 
 
 from GPy_ABCD.Models.modelSearch import explore_model_space, model_search_rounds,\
     fit_one_model, fit_mods_not_parallel, fit_mods_parallel_processes
 from GPy_ABCD.Util.modelUtil import BIC, AIC, AICc, fit_kex, fit_GPy_kern, model_printout, GPy_optimisers
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD/config.py` & `GPy-ABCD-1.2/GPy_ABCD/config.py`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/GPy_ABCD.egg-info/PKG-INFO` & `GPy-ABCD-1.2/GPy_ABCD.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,193 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: GPy-ABCD
-Version: 1.1
+Version: 1.2
 Summary: Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system
 Home-page: https://github.com/T-Flet/GPy-ABCD
 Author: Thomas Fletcher
 Author-email: T-Fletcher@outlook.com
 License: BSD 3-Clause
-Description: GPy-ABCD
-        ========
-        
-        .. image:: https://img.shields.io/pypi/v/GPy-ABCD.svg
-            :target: https://pypi.python.org/pypi/GPy-ABCD/
-            :alt: Latest PyPI version
-        
-        .. image:: https://pepy.tech/badge/gpy-abcd
-            :target: https://pepy.tech/project/gpy-abcd
-            :alt: Package Downloads
-        
-        .. image:: https://img.shields.io/pypi/pyversions/GPy-ABCD.svg
-            :target: https://pypi.python.org/pypi/GPy-ABCD/
-            :alt: Python Versions
-        
-        .. image:: https://github.com/T-Flet/GPy-ABCD/workflows/Python%20package/badge.svg
-            :target: https://github.com/T-Flet/GPy-ABCD/actions?query=workflow%3A%22Python+package%22
-            :alt: Build
-        
-        .. image:: https://img.shields.io/pypi/l/GPy-ABCD.svg
-            :target: https://github.com/T-Flet/GPy-ABCD/blob/master/LICENSE
-            :alt: License
-        
-        Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system
-        
-        Briefly: ABCD is a modelling system which consists in exploring a space of compositional kernels
-        (i.e. covariances of Gaussian Processes) constructed by iteratively combining a small set of base ones,
-        returning the best fitting models using them, and capable of generating simple text descriptions of the
-        fits based on the identified functional shapes.
-        
-        See the picture in `Usage` below for an example input/output and read the paper for further details:
-        
-        `Fletcher, T., Bundy, A., & Nuamah, K. . GPy-ABCD: A Configurable Automatic Bayesian Covariance Discovery Implementation.
-        8th ICML Workshop on Automated Machine Learning (2021) <http://icml2021.automl.org/>`_
-        
-        
-        
-        Installation
-        ------------
-        ::
-        
-            pip install GPy_ABCD
-        
-        
-        
-        Usage
-        -----
-        The main function exported by this package is ``explore_model_space``;
-        see its description for parameter information and type hints.
-        Note that with the default ``model_list_fitter = fit_mods_parallel_processes`` argument
-        the function should be called from within a ``if __name__ == '__main__':`` for full OS-agnostic use.
-        
-        A minimal example to showcase the various parameters follows:
-        
-        .. code-block:: Python
-        
-            import numpy as np
-            from GPy_ABCD import *
-        
-        
-            if __name__ == '__main__':
-                # Example data
-                X = np.linspace(-10, 10, 101)[:, None]
-                Y = np.cos((X - 5) / 2) ** 2 * X * 2 + np.random.randn(101, 1)
-        
-                # Main function call with default arguments
-                best_mods, all_mods, all_exprs, expanded, not_expanded = explore_model_space(X, Y,
-                    start_kernels = start_kernels['Default'], p_rules = production_rules['Default'],
-                    utility_function = BIC, rounds = 2, beam = [3, 2, 1], restarts = 5,
-                    model_list_fitter = fit_mods_parallel_processes, optimiser = GPy_optimisers[0],
-                    verbose = True)
-        
-                print('\nFull lists of models by round:')
-                for mod_depth in all_mods: print(', '.join([str(mod.kernel_expression) for mod in mod_depth]) + f'\n{len(mod_depth)}')
-        
-                print('\n\nTop-3 models\' details:')
-                for bm in best_mods[:3]:
-                    model_printout(bm) # See the definition of this convenience function for examples of model details' extraction
-                    print('Prediction at X = 11:', bm.predict(np.array([11])[:, None]), '\n')
-        
-                from matplotlib import pyplot as plt
-                plt.show()
-        
-        
-        
-        .. figure:: selected_output_example.png
-            :align: center
-            :figclass: align-center
-        
-            Selection of output from the above example
-        
-        The directly importable elements from this package are essentially those required to customise any of the arguments of the
-        main model search function plus a few convenient tools (refer to the section below for context):
-        
-        - The main function ``explore_model_space``
-        - The ``model_search_rounds`` function to continue a search from where another left-off
-        - Functions to be used as  ``model_list_fitter`` argument: ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes`` (using ``multiprocessing``'s ``Pool``)
-        - The single-fit function ``fit_one_model``, on which the list-fitting functions above are built (so that a user may implement their preferred parallelisation)
-        - Non-searching single-fit functions: ``fit_kex`` (which takes ``KernelExpression`` inputs and simplifies them if required) and ``fit_GPy_kern`` (which takes GPy kernel inputs and returns GPy GPRegression objects, not full GPy-ABCD GPModel ones)
-        - A few standard model-scoring functions: ``BIC``, ``AIC``, ``AICc``
-        - The aforementioned convenience function ``model_printout``
-        - The list of GPy 1.9.9 model fit optimisers ``GPy_optimisers``
-        - A few (named) choices of start kernels and production rules in the dictionaries ``start_kernels`` and ``production_rules``
-        - The dictionary of available production rules grouped by type ``production_rules_by_type``
-        - The concrete ``KernelExpression`` subclasses ``SumKE``, ``ProductKE`` and ``ChangeKE``
-        - The frozensets of ``base_kerns`` and ``base_sigmoids``
-        
-        (The purpose of exporting elements in the last 3 lines is for users to create alternative sets of production
-        rules and starting kernels lists by mixing kernel expressions and raw strings of base kernels;
-        see the definitions of entries of the ``start_kernels`` and ``production_rules`` dictionaries for examples)
-        
-        
-        
-        Project Structure
-        -----------------
-        
-        A paper on GPy-ABCD and its differences from the original ABCD is planned, but for the time being read the paper mentioned above for a full picture of what an ABCD system is.
-        
-        However, briefly, it consists in exploring a space of compositional kernels built from a few carefully selected base ones,
-        returning the best fitting models using them and generating simple text interpretations of the fits based
-        on the functional shapes of the final composed covariance kernels and parameter values.
-        
-        The core components of this project's ABCD implementation are the following:
-        
-        - ``Kernels.baseKernels`` contains the "mathematical" base kernels (i.e. GPy kernel objects) for the whole machinery
-        
-          - Some of the base kernels are simply wrapped GPy-provided kernels (White-Noise, Constant and Squared-Exponential)
-          - The others are either not present in GPy's default arsenal or are improved versions of ones which are (Linear which can identify polynomial roots and purely-Periodic standard-periodic kernel)
-          - It contains sigmoidal kernels (both base sigmoids and indicator-like ones, i.e. sigmoidal hat/well) which are not used directly in the symbolic expressions but are substituted in by change-type kernels
-          - It contains change-point and change-window kernels which use the aforementioned sigmoidals
-        - ``KernelExpression`` contains the "symbolic" kernel classes constituting the nodes with which to build complex kernel expressions in the form of trees
-        
-          - The non-abstract kernel expression classes are ``SumKE``, ``ProductKE`` and ``ChangeKE``
-          - ``SumKE`` and ``ProductKE`` are direct subclasses of the abstract class `SumOrProductKE` and only really differ in how they self-simplify and distribute over the other
-          - ``ChangeKE`` could be split into separate change-point and change-window classes, but a single argument difference allows full method overlap
-          - ``SumOrProductKE`` and ``ChangeKE`` are direct subclasses of the abstract base class ``KernelExpression``
-        - The above kernel expression classes have a wide variety of methods providing the following general functionality in order to make the rest of the project light of ad-hoc functions:
-        
-          - They self-simplify when modified through the appropriate methods (they are symbolic expressions after all)
-          - They can produce GPy kernel objects
-          - They can line-up with and absorb fit model parameters from a matching GPy object
-          - They can rearrange to a sum-of-products form
-          - They can generate text interpretations of their sum-of-products form
-        - ``KernelExpansion.grammar`` contains the various production rules and default starting kernel lists used in model space exploration
-        - ``Models.modelSearch`` contains the system front-end elements:
-        
-          - The ``GPModel`` class, which is where the GPy kernels/models interact with the symbolic kernel expressions
-          - The aforementioned functions to fit lists of models ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes``
-          - The ``explore_model_space`` function, which is the point of it all
-          - The ``model_search_rounds`` function, which is used by the above but also meant to continue searching by building on past exploration results
-        
-        Note: a ``config.py`` file is present, and it contains a few global-behaviour-altering flags (e.g. enabling/disabling the Squared-Exponential kernel)
-        
-        
-        
-        Further Notes
-        -------------
-        
-        Generic:
-        
-        - Please let know me if you have successfully used this project in your own research
-        - Please feel free to fork and expand this project (pull requests are welcome) since it is not the focus of my research; it was written just because I needed to use it in a broader adaptive statistical modelling context and therefore I have no need to expand its functionality in the near future
-        
-        Code-related:
-        
-        - The important tests are in pytest scripts, but many other scripts are present and intended as functionality showcases or "tests by inspection"
-        - Additionally, pytest.ini has a two opposite configuration lines intended to be toggled to perform "real" tests vs other "by inspection" tests
-        
-        Possible expansion directions:
-        
-        - Many "TODO" comments are present throughout the codebase
-        - Optimising ChangeWindow window-location fitting is an open issue (multiple implementations of change-window and the sigmoidal kernels they rely on have already been tried; see the commented-out declarations in baseKernels.py inv ersions before v1.0)
-        - The periodic kernel could be more stable in non-periodic-data fits (GPy's own as well)
-        - Making each project layer accept multidimensional data, starting from the GPy kernels (some already do)
-        - Expanding on the GPy side of things: add more methods to the kernels in order to make use of the full spectrum of GPy features (MCMC etc)
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+GPy-ABCD
+========
+
+.. image:: https://img.shields.io/pypi/v/GPy-ABCD.svg
+    :target: https://pypi.python.org/pypi/GPy-ABCD/
+    :alt: Latest PyPI version
+
+.. image:: https://pepy.tech/badge/gpy-abcd
+    :target: https://pepy.tech/project/gpy-abcd
+    :alt: Package Downloads
+
+.. image:: https://img.shields.io/pypi/pyversions/GPy-ABCD.svg
+    :target: https://pypi.python.org/pypi/GPy-ABCD/
+    :alt: Python Versions
+
+.. image:: https://github.com/T-Flet/GPy-ABCD/workflows/Python%20package/badge.svg
+    :target: https://github.com/T-Flet/GPy-ABCD/actions?query=workflow%3A%22Python+package%22
+    :alt: Build
+
+.. image:: https://img.shields.io/pypi/l/GPy-ABCD.svg
+    :target: https://github.com/T-Flet/GPy-ABCD/blob/master/LICENSE
+    :alt: License
+
+Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system
+
+Briefly: ABCD is a modelling system which consists in exploring a space of compositional kernels
+(i.e. covariances of Gaussian Processes) constructed by iteratively combining a small set of base ones,
+returning the best fitting models using them, and capable of generating simple text descriptions of the
+fits based on the identified functional shapes.
+
+See the picture in `Usage` below for an example input/output and read the paper for further details:
+
+`Fletcher, T., Bundy, A., & Nuamah, K. . GPy-ABCD: A Configurable Automatic Bayesian Covariance Discovery Implementation.
+8th ICML Workshop on Automated Machine Learning (2021) <https://sites.google.com/view/automl2021/accepted-papers>`_
+
+
+
+Installation
+------------
+::
+
+    pip install GPy_ABCD
+
+
+
+Usage
+-----
+The main function exported by this package is ``explore_model_space``;
+see its description for parameter information and type hints.
+Note that with the default ``model_list_fitter = fit_mods_parallel_processes`` argument
+the function should be called from within a ``if __name__ == '__main__':`` for full OS-agnostic use.
+
+A minimal example to showcase the various parameters follows:
+
+.. code-block:: Python
+
+    import numpy as np
+    from GPy_ABCD import *
+
+
+    if __name__ == '__main__':
+        # Example data
+        X = np.linspace(-10, 10, 101)[:, None]
+        Y = np.cos((X - 5) / 2) ** 2 * X * 2 + np.random.randn(101, 1)
+
+        # Main function call with default arguments
+        best_mods, all_mods, all_exprs, expanded, not_expanded = explore_model_space(X, Y,
+            start_kernels = start_kernels['Default'], p_rules = production_rules['Default'],
+            utility_function = BIC, rounds = 2, beam = [3, 2, 1], restarts = 5,
+            model_list_fitter = fit_mods_parallel_processes, optimiser = GPy_optimisers[0],
+            verbose = True)
+
+        print('\nFull lists of models by round:')
+        for mod_depth in all_mods: print(', '.join([str(mod.kernel_expression) for mod in mod_depth]) + f'\n{len(mod_depth)}')
+
+        print('\n\nTop-3 models\' details:')
+        for bm in best_mods[:3]:
+            model_printout(bm) # See the definition of this convenience function for examples of model details' extraction
+            print('Prediction at X = 11:', bm.predict(np.array([11])[:, None]), '\n')
+
+        from matplotlib import pyplot as plt
+        plt.show()
+
+
+
+.. figure:: selected_output_example.png
+    :align: center
+    :figclass: align-center
+
+    Selection of output from the above example
+
+The directly importable elements from this package are essentially those required to customise any of the arguments of the
+main model search function plus a few convenient tools (refer to the section below for context):
+
+- The main function ``explore_model_space``
+- The ``model_search_rounds`` function to continue a search from where another left-off
+- Functions to be used as  ``model_list_fitter`` argument: ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes`` (using ``multiprocessing``'s ``Pool``)
+- The single-fit function ``fit_one_model``, on which the list-fitting functions above are built (so that a user may implement their preferred parallelisation)
+- Non-searching single-fit functions: ``fit_kex`` (which takes ``KernelExpression`` inputs and simplifies them if required) and ``fit_GPy_kern`` (which takes GPy kernel inputs and returns GPy GPRegression objects, not full GPy-ABCD GPModel ones)
+- A few standard model-scoring functions: ``BIC``, ``AIC``, ``AICc``
+- The aforementioned convenience function ``model_printout``
+- The list of GPy 1.9.9 model fit optimisers ``GPy_optimisers``
+- A few (named) choices of start kernels and production rules in the dictionaries ``start_kernels`` and ``production_rules``
+- The dictionary of available production rules grouped by type ``production_rules_by_type``
+- The concrete ``KernelExpression`` subclasses ``SumKE``, ``ProductKE`` and ``ChangeKE``
+- The frozensets of ``base_kerns`` and ``base_sigmoids``
+
+(The purpose of exporting elements in the last 3 lines is for users to create alternative sets of production
+rules and starting kernels lists by mixing kernel expressions and raw strings of base kernels;
+see the definitions of entries of the ``start_kernels`` and ``production_rules`` dictionaries for examples)
+
+
+
+Project Structure
+-----------------
+
+A paper on GPy-ABCD and its differences from the original ABCD is planned, but for the time being read the paper mentioned above for a full picture of what an ABCD system is.
+
+However, briefly, it consists in exploring a space of compositional kernels built from a few carefully selected base ones,
+returning the best fitting models using them and generating simple text interpretations of the fits based
+on the functional shapes of the final composed covariance kernels and parameter values.
+
+The core components of this project's ABCD implementation are the following:
+
+- ``Kernels.baseKernels`` contains the "mathematical" base kernels (i.e. GPy kernel objects) for the whole machinery
+
+  - Some of the base kernels are simply wrapped GPy-provided kernels (White-Noise, Constant and Squared-Exponential)
+  - The others are either not present in GPy's default arsenal or are improved versions of ones which are (Linear which can identify polynomial roots and purely-Periodic standard-periodic kernel)
+  - It contains sigmoidal kernels (both base sigmoids and indicator-like ones, i.e. sigmoidal hat/well) which are not used directly in the symbolic expressions but are substituted in by change-type kernels
+  - It contains change-point and change-window kernels which use the aforementioned sigmoidals
+- ``KernelExpression`` contains the "symbolic" kernel classes constituting the nodes with which to build complex kernel expressions in the form of trees
+
+  - The non-abstract kernel expression classes are ``SumKE``, ``ProductKE`` and ``ChangeKE``
+  - ``SumKE`` and ``ProductKE`` are direct subclasses of the abstract class `SumOrProductKE` and only really differ in how they self-simplify and distribute over the other
+  - ``ChangeKE`` could be split into separate change-point and change-window classes, but a single argument difference allows full method overlap
+  - ``SumOrProductKE`` and ``ChangeKE`` are direct subclasses of the abstract base class ``KernelExpression``
+- The above kernel expression classes have a wide variety of methods providing the following general functionality in order to make the rest of the project light of ad-hoc functions:
+
+  - They self-simplify when modified through the appropriate methods (they are symbolic expressions after all)
+  - They can produce GPy kernel objects
+  - They can line-up with and absorb fit model parameters from a matching GPy object
+  - They can rearrange to a sum-of-products form
+  - They can generate text interpretations of their sum-of-products form
+- ``KernelExpansion.grammar`` contains the various production rules and default starting kernel lists used in model space exploration
+- ``Models.modelSearch`` contains the system front-end elements:
+
+  - The ``GPModel`` class, which is where the GPy kernels/models interact with the symbolic kernel expressions
+  - The aforementioned functions to fit lists of models ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes``
+  - The ``explore_model_space`` function, which is the point of it all
+  - The ``model_search_rounds`` function, which is used by the above but also meant to continue searching by building on past exploration results
+
+Note: a ``config.py`` file is present, and it contains a few global-behaviour-altering flags (e.g. enabling/disabling the Squared-Exponential kernel)
+
+
+
+Further Notes
+-------------
+
+Generic:
+
+- Please let know me if you have successfully used this project in your own research
+- Please feel free to fork and expand this project (pull requests are welcome) since it is not the focus of my research; it was written just because I needed to use it in a broader adaptive statistical modelling context and therefore I have no need to expand its functionality in the near future
+
+Code-related:
+
+- The important tests are in pytest scripts, but many other scripts are present and intended as functionality showcases or "tests by inspection"
+- Additionally, pytest.ini has a two opposite configuration lines intended to be toggled to perform "real" tests vs other "by inspection" tests
+
+Possible expansion directions:
+
+- Many "TODO" comments are present throughout the codebase
+- Optimising ChangeWindow window-location fitting is an open issue (multiple implementations of change-window and the sigmoidal kernels they rely on have already been tried; see the commented-out declarations in baseKernels.py inv ersions before v1.0)
+- The periodic kernel could be more stable in non-periodic-data fits (GPy's own as well)
+- Making each project layer accept multidimensional data, starting from the GPy kernels (some already do)
+- Expanding on the GPy side of things: add more methods to the kernels in order to make use of the full spectrum of GPy features (MCMC etc)
+
+
```

### Comparing `GPy-ABCD-1.1/GPy_ABCD.egg-info/SOURCES.txt` & `GPy-ABCD-1.2/GPy_ABCD.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -28,12 +28,14 @@
 GPy_ABCD/Kernels/linearOffsetKernel.py
 GPy_ABCD/Kernels/periodicKernel.py
 GPy_ABCD/Kernels/sigmoidalKernels.py
 GPy_ABCD/Models/__init__.py
 GPy_ABCD/Models/model.py
 GPy_ABCD/Models/modelSearch.py
 GPy_ABCD/Util/__init__.py
+GPy_ABCD/Util/benchmarking.py
 GPy_ABCD/Util/dataAndPlottingUtil.py
 GPy_ABCD/Util/genericUtil.py
 GPy_ABCD/Util/kernelUtil.py
 GPy_ABCD/Util/modelUtil.py
+GPy_ABCD/Util/numba_types.py
 GPy_ABCD/Util/showcaseAllKernels.py
```

### Comparing `GPy-ABCD-1.1/LICENSE` & `GPy-ABCD-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GPy-ABCD-1.1/PKG-INFO` & `GPy-ABCD-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,193 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: GPy-ABCD
-Version: 1.1
+Version: 1.2
 Summary: Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system
 Home-page: https://github.com/T-Flet/GPy-ABCD
 Author: Thomas Fletcher
 Author-email: T-Fletcher@outlook.com
 License: BSD 3-Clause
-Description: GPy-ABCD
-        ========
-        
-        .. image:: https://img.shields.io/pypi/v/GPy-ABCD.svg
-            :target: https://pypi.python.org/pypi/GPy-ABCD/
-            :alt: Latest PyPI version
-        
-        .. image:: https://pepy.tech/badge/gpy-abcd
-            :target: https://pepy.tech/project/gpy-abcd
-            :alt: Package Downloads
-        
-        .. image:: https://img.shields.io/pypi/pyversions/GPy-ABCD.svg
-            :target: https://pypi.python.org/pypi/GPy-ABCD/
-            :alt: Python Versions
-        
-        .. image:: https://github.com/T-Flet/GPy-ABCD/workflows/Python%20package/badge.svg
-            :target: https://github.com/T-Flet/GPy-ABCD/actions?query=workflow%3A%22Python+package%22
-            :alt: Build
-        
-        .. image:: https://img.shields.io/pypi/l/GPy-ABCD.svg
-            :target: https://github.com/T-Flet/GPy-ABCD/blob/master/LICENSE
-            :alt: License
-        
-        Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system
-        
-        Briefly: ABCD is a modelling system which consists in exploring a space of compositional kernels
-        (i.e. covariances of Gaussian Processes) constructed by iteratively combining a small set of base ones,
-        returning the best fitting models using them, and capable of generating simple text descriptions of the
-        fits based on the identified functional shapes.
-        
-        See the picture in `Usage` below for an example input/output and read the paper for further details:
-        
-        `Fletcher, T., Bundy, A., & Nuamah, K. . GPy-ABCD: A Configurable Automatic Bayesian Covariance Discovery Implementation.
-        8th ICML Workshop on Automated Machine Learning (2021) <http://icml2021.automl.org/>`_
-        
-        
-        
-        Installation
-        ------------
-        ::
-        
-            pip install GPy_ABCD
-        
-        
-        
-        Usage
-        -----
-        The main function exported by this package is ``explore_model_space``;
-        see its description for parameter information and type hints.
-        Note that with the default ``model_list_fitter = fit_mods_parallel_processes`` argument
-        the function should be called from within a ``if __name__ == '__main__':`` for full OS-agnostic use.
-        
-        A minimal example to showcase the various parameters follows:
-        
-        .. code-block:: Python
-        
-            import numpy as np
-            from GPy_ABCD import *
-        
-        
-            if __name__ == '__main__':
-                # Example data
-                X = np.linspace(-10, 10, 101)[:, None]
-                Y = np.cos((X - 5) / 2) ** 2 * X * 2 + np.random.randn(101, 1)
-        
-                # Main function call with default arguments
-                best_mods, all_mods, all_exprs, expanded, not_expanded = explore_model_space(X, Y,
-                    start_kernels = start_kernels['Default'], p_rules = production_rules['Default'],
-                    utility_function = BIC, rounds = 2, beam = [3, 2, 1], restarts = 5,
-                    model_list_fitter = fit_mods_parallel_processes, optimiser = GPy_optimisers[0],
-                    verbose = True)
-        
-                print('\nFull lists of models by round:')
-                for mod_depth in all_mods: print(', '.join([str(mod.kernel_expression) for mod in mod_depth]) + f'\n{len(mod_depth)}')
-        
-                print('\n\nTop-3 models\' details:')
-                for bm in best_mods[:3]:
-                    model_printout(bm) # See the definition of this convenience function for examples of model details' extraction
-                    print('Prediction at X = 11:', bm.predict(np.array([11])[:, None]), '\n')
-        
-                from matplotlib import pyplot as plt
-                plt.show()
-        
-        
-        
-        .. figure:: selected_output_example.png
-            :align: center
-            :figclass: align-center
-        
-            Selection of output from the above example
-        
-        The directly importable elements from this package are essentially those required to customise any of the arguments of the
-        main model search function plus a few convenient tools (refer to the section below for context):
-        
-        - The main function ``explore_model_space``
-        - The ``model_search_rounds`` function to continue a search from where another left-off
-        - Functions to be used as  ``model_list_fitter`` argument: ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes`` (using ``multiprocessing``'s ``Pool``)
-        - The single-fit function ``fit_one_model``, on which the list-fitting functions above are built (so that a user may implement their preferred parallelisation)
-        - Non-searching single-fit functions: ``fit_kex`` (which takes ``KernelExpression`` inputs and simplifies them if required) and ``fit_GPy_kern`` (which takes GPy kernel inputs and returns GPy GPRegression objects, not full GPy-ABCD GPModel ones)
-        - A few standard model-scoring functions: ``BIC``, ``AIC``, ``AICc``
-        - The aforementioned convenience function ``model_printout``
-        - The list of GPy 1.9.9 model fit optimisers ``GPy_optimisers``
-        - A few (named) choices of start kernels and production rules in the dictionaries ``start_kernels`` and ``production_rules``
-        - The dictionary of available production rules grouped by type ``production_rules_by_type``
-        - The concrete ``KernelExpression`` subclasses ``SumKE``, ``ProductKE`` and ``ChangeKE``
-        - The frozensets of ``base_kerns`` and ``base_sigmoids``
-        
-        (The purpose of exporting elements in the last 3 lines is for users to create alternative sets of production
-        rules and starting kernels lists by mixing kernel expressions and raw strings of base kernels;
-        see the definitions of entries of the ``start_kernels`` and ``production_rules`` dictionaries for examples)
-        
-        
-        
-        Project Structure
-        -----------------
-        
-        A paper on GPy-ABCD and its differences from the original ABCD is planned, but for the time being read the paper mentioned above for a full picture of what an ABCD system is.
-        
-        However, briefly, it consists in exploring a space of compositional kernels built from a few carefully selected base ones,
-        returning the best fitting models using them and generating simple text interpretations of the fits based
-        on the functional shapes of the final composed covariance kernels and parameter values.
-        
-        The core components of this project's ABCD implementation are the following:
-        
-        - ``Kernels.baseKernels`` contains the "mathematical" base kernels (i.e. GPy kernel objects) for the whole machinery
-        
-          - Some of the base kernels are simply wrapped GPy-provided kernels (White-Noise, Constant and Squared-Exponential)
-          - The others are either not present in GPy's default arsenal or are improved versions of ones which are (Linear which can identify polynomial roots and purely-Periodic standard-periodic kernel)
-          - It contains sigmoidal kernels (both base sigmoids and indicator-like ones, i.e. sigmoidal hat/well) which are not used directly in the symbolic expressions but are substituted in by change-type kernels
-          - It contains change-point and change-window kernels which use the aforementioned sigmoidals
-        - ``KernelExpression`` contains the "symbolic" kernel classes constituting the nodes with which to build complex kernel expressions in the form of trees
-        
-          - The non-abstract kernel expression classes are ``SumKE``, ``ProductKE`` and ``ChangeKE``
-          - ``SumKE`` and ``ProductKE`` are direct subclasses of the abstract class `SumOrProductKE` and only really differ in how they self-simplify and distribute over the other
-          - ``ChangeKE`` could be split into separate change-point and change-window classes, but a single argument difference allows full method overlap
-          - ``SumOrProductKE`` and ``ChangeKE`` are direct subclasses of the abstract base class ``KernelExpression``
-        - The above kernel expression classes have a wide variety of methods providing the following general functionality in order to make the rest of the project light of ad-hoc functions:
-        
-          - They self-simplify when modified through the appropriate methods (they are symbolic expressions after all)
-          - They can produce GPy kernel objects
-          - They can line-up with and absorb fit model parameters from a matching GPy object
-          - They can rearrange to a sum-of-products form
-          - They can generate text interpretations of their sum-of-products form
-        - ``KernelExpansion.grammar`` contains the various production rules and default starting kernel lists used in model space exploration
-        - ``Models.modelSearch`` contains the system front-end elements:
-        
-          - The ``GPModel`` class, which is where the GPy kernels/models interact with the symbolic kernel expressions
-          - The aforementioned functions to fit lists of models ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes``
-          - The ``explore_model_space`` function, which is the point of it all
-          - The ``model_search_rounds`` function, which is used by the above but also meant to continue searching by building on past exploration results
-        
-        Note: a ``config.py`` file is present, and it contains a few global-behaviour-altering flags (e.g. enabling/disabling the Squared-Exponential kernel)
-        
-        
-        
-        Further Notes
-        -------------
-        
-        Generic:
-        
-        - Please let know me if you have successfully used this project in your own research
-        - Please feel free to fork and expand this project (pull requests are welcome) since it is not the focus of my research; it was written just because I needed to use it in a broader adaptive statistical modelling context and therefore I have no need to expand its functionality in the near future
-        
-        Code-related:
-        
-        - The important tests are in pytest scripts, but many other scripts are present and intended as functionality showcases or "tests by inspection"
-        - Additionally, pytest.ini has a two opposite configuration lines intended to be toggled to perform "real" tests vs other "by inspection" tests
-        
-        Possible expansion directions:
-        
-        - Many "TODO" comments are present throughout the codebase
-        - Optimising ChangeWindow window-location fitting is an open issue (multiple implementations of change-window and the sigmoidal kernels they rely on have already been tried; see the commented-out declarations in baseKernels.py inv ersions before v1.0)
-        - The periodic kernel could be more stable in non-periodic-data fits (GPy's own as well)
-        - Making each project layer accept multidimensional data, starting from the GPy kernels (some already do)
-        - Expanding on the GPy side of things: add more methods to the kernels in order to make use of the full spectrum of GPy features (MCMC etc)
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+GPy-ABCD
+========
+
+.. image:: https://img.shields.io/pypi/v/GPy-ABCD.svg
+    :target: https://pypi.python.org/pypi/GPy-ABCD/
+    :alt: Latest PyPI version
+
+.. image:: https://pepy.tech/badge/gpy-abcd
+    :target: https://pepy.tech/project/gpy-abcd
+    :alt: Package Downloads
+
+.. image:: https://img.shields.io/pypi/pyversions/GPy-ABCD.svg
+    :target: https://pypi.python.org/pypi/GPy-ABCD/
+    :alt: Python Versions
+
+.. image:: https://github.com/T-Flet/GPy-ABCD/workflows/Python%20package/badge.svg
+    :target: https://github.com/T-Flet/GPy-ABCD/actions?query=workflow%3A%22Python+package%22
+    :alt: Build
+
+.. image:: https://img.shields.io/pypi/l/GPy-ABCD.svg
+    :target: https://github.com/T-Flet/GPy-ABCD/blob/master/LICENSE
+    :alt: License
+
+Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system
+
+Briefly: ABCD is a modelling system which consists in exploring a space of compositional kernels
+(i.e. covariances of Gaussian Processes) constructed by iteratively combining a small set of base ones,
+returning the best fitting models using them, and capable of generating simple text descriptions of the
+fits based on the identified functional shapes.
+
+See the picture in `Usage` below for an example input/output and read the paper for further details:
+
+`Fletcher, T., Bundy, A., & Nuamah, K. . GPy-ABCD: A Configurable Automatic Bayesian Covariance Discovery Implementation.
+8th ICML Workshop on Automated Machine Learning (2021) <https://sites.google.com/view/automl2021/accepted-papers>`_
+
+
+
+Installation
+------------
+::
+
+    pip install GPy_ABCD
+
+
+
+Usage
+-----
+The main function exported by this package is ``explore_model_space``;
+see its description for parameter information and type hints.
+Note that with the default ``model_list_fitter = fit_mods_parallel_processes`` argument
+the function should be called from within a ``if __name__ == '__main__':`` for full OS-agnostic use.
+
+A minimal example to showcase the various parameters follows:
+
+.. code-block:: Python
+
+    import numpy as np
+    from GPy_ABCD import *
+
+
+    if __name__ == '__main__':
+        # Example data
+        X = np.linspace(-10, 10, 101)[:, None]
+        Y = np.cos((X - 5) / 2) ** 2 * X * 2 + np.random.randn(101, 1)
+
+        # Main function call with default arguments
+        best_mods, all_mods, all_exprs, expanded, not_expanded = explore_model_space(X, Y,
+            start_kernels = start_kernels['Default'], p_rules = production_rules['Default'],
+            utility_function = BIC, rounds = 2, beam = [3, 2, 1], restarts = 5,
+            model_list_fitter = fit_mods_parallel_processes, optimiser = GPy_optimisers[0],
+            verbose = True)
+
+        print('\nFull lists of models by round:')
+        for mod_depth in all_mods: print(', '.join([str(mod.kernel_expression) for mod in mod_depth]) + f'\n{len(mod_depth)}')
+
+        print('\n\nTop-3 models\' details:')
+        for bm in best_mods[:3]:
+            model_printout(bm) # See the definition of this convenience function for examples of model details' extraction
+            print('Prediction at X = 11:', bm.predict(np.array([11])[:, None]), '\n')
+
+        from matplotlib import pyplot as plt
+        plt.show()
+
+
+
+.. figure:: selected_output_example.png
+    :align: center
+    :figclass: align-center
+
+    Selection of output from the above example
+
+The directly importable elements from this package are essentially those required to customise any of the arguments of the
+main model search function plus a few convenient tools (refer to the section below for context):
+
+- The main function ``explore_model_space``
+- The ``model_search_rounds`` function to continue a search from where another left-off
+- Functions to be used as  ``model_list_fitter`` argument: ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes`` (using ``multiprocessing``'s ``Pool``)
+- The single-fit function ``fit_one_model``, on which the list-fitting functions above are built (so that a user may implement their preferred parallelisation)
+- Non-searching single-fit functions: ``fit_kex`` (which takes ``KernelExpression`` inputs and simplifies them if required) and ``fit_GPy_kern`` (which takes GPy kernel inputs and returns GPy GPRegression objects, not full GPy-ABCD GPModel ones)
+- A few standard model-scoring functions: ``BIC``, ``AIC``, ``AICc``
+- The aforementioned convenience function ``model_printout``
+- The list of GPy 1.9.9 model fit optimisers ``GPy_optimisers``
+- A few (named) choices of start kernels and production rules in the dictionaries ``start_kernels`` and ``production_rules``
+- The dictionary of available production rules grouped by type ``production_rules_by_type``
+- The concrete ``KernelExpression`` subclasses ``SumKE``, ``ProductKE`` and ``ChangeKE``
+- The frozensets of ``base_kerns`` and ``base_sigmoids``
+
+(The purpose of exporting elements in the last 3 lines is for users to create alternative sets of production
+rules and starting kernels lists by mixing kernel expressions and raw strings of base kernels;
+see the definitions of entries of the ``start_kernels`` and ``production_rules`` dictionaries for examples)
+
+
+
+Project Structure
+-----------------
+
+A paper on GPy-ABCD and its differences from the original ABCD is planned, but for the time being read the paper mentioned above for a full picture of what an ABCD system is.
+
+However, briefly, it consists in exploring a space of compositional kernels built from a few carefully selected base ones,
+returning the best fitting models using them and generating simple text interpretations of the fits based
+on the functional shapes of the final composed covariance kernels and parameter values.
+
+The core components of this project's ABCD implementation are the following:
+
+- ``Kernels.baseKernels`` contains the "mathematical" base kernels (i.e. GPy kernel objects) for the whole machinery
+
+  - Some of the base kernels are simply wrapped GPy-provided kernels (White-Noise, Constant and Squared-Exponential)
+  - The others are either not present in GPy's default arsenal or are improved versions of ones which are (Linear which can identify polynomial roots and purely-Periodic standard-periodic kernel)
+  - It contains sigmoidal kernels (both base sigmoids and indicator-like ones, i.e. sigmoidal hat/well) which are not used directly in the symbolic expressions but are substituted in by change-type kernels
+  - It contains change-point and change-window kernels which use the aforementioned sigmoidals
+- ``KernelExpression`` contains the "symbolic" kernel classes constituting the nodes with which to build complex kernel expressions in the form of trees
+
+  - The non-abstract kernel expression classes are ``SumKE``, ``ProductKE`` and ``ChangeKE``
+  - ``SumKE`` and ``ProductKE`` are direct subclasses of the abstract class `SumOrProductKE` and only really differ in how they self-simplify and distribute over the other
+  - ``ChangeKE`` could be split into separate change-point and change-window classes, but a single argument difference allows full method overlap
+  - ``SumOrProductKE`` and ``ChangeKE`` are direct subclasses of the abstract base class ``KernelExpression``
+- The above kernel expression classes have a wide variety of methods providing the following general functionality in order to make the rest of the project light of ad-hoc functions:
+
+  - They self-simplify when modified through the appropriate methods (they are symbolic expressions after all)
+  - They can produce GPy kernel objects
+  - They can line-up with and absorb fit model parameters from a matching GPy object
+  - They can rearrange to a sum-of-products form
+  - They can generate text interpretations of their sum-of-products form
+- ``KernelExpansion.grammar`` contains the various production rules and default starting kernel lists used in model space exploration
+- ``Models.modelSearch`` contains the system front-end elements:
+
+  - The ``GPModel`` class, which is where the GPy kernels/models interact with the symbolic kernel expressions
+  - The aforementioned functions to fit lists of models ``fit_mods_not_parallel`` and ``fit_mods_parallel_processes``
+  - The ``explore_model_space`` function, which is the point of it all
+  - The ``model_search_rounds`` function, which is used by the above but also meant to continue searching by building on past exploration results
+
+Note: a ``config.py`` file is present, and it contains a few global-behaviour-altering flags (e.g. enabling/disabling the Squared-Exponential kernel)
+
+
+
+Further Notes
+-------------
+
+Generic:
+
+- Please let know me if you have successfully used this project in your own research
+- Please feel free to fork and expand this project (pull requests are welcome) since it is not the focus of my research; it was written just because I needed to use it in a broader adaptive statistical modelling context and therefore I have no need to expand its functionality in the near future
+
+Code-related:
+
+- The important tests are in pytest scripts, but many other scripts are present and intended as functionality showcases or "tests by inspection"
+- Additionally, pytest.ini has a two opposite configuration lines intended to be toggled to perform "real" tests vs other "by inspection" tests
+
+Possible expansion directions:
+
+- Many "TODO" comments are present throughout the codebase
+- Optimising ChangeWindow window-location fitting is an open issue (multiple implementations of change-window and the sigmoidal kernels they rely on have already been tried; see the commented-out declarations in baseKernels.py inv ersions before v1.0)
+- The periodic kernel could be more stable in non-periodic-data fits (GPy's own as well)
+- Making each project layer accept multidimensional data, starting from the GPy kernels (some already do)
+- Expanding on the GPy side of things: add more methods to the kernels in order to make use of the full spectrum of GPy features (MCMC etc)
+
+
```

### Comparing `GPy-ABCD-1.1/README.rst` & `GPy-ABCD-1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 (i.e. covariances of Gaussian Processes) constructed by iteratively combining a small set of base ones,
 returning the best fitting models using them, and capable of generating simple text descriptions of the
 fits based on the identified functional shapes.
 
 See the picture in `Usage` below for an example input/output and read the paper for further details:
 
 `Fletcher, T., Bundy, A., & Nuamah, K. . GPy-ABCD: A Configurable Automatic Bayesian Covariance Discovery Implementation.
-8th ICML Workshop on Automated Machine Learning (2021) <http://icml2021.automl.org/>`_
+8th ICML Workshop on Automated Machine Learning (2021) <https://sites.google.com/view/automl2021/accepted-papers>`_
 
 
 
 Installation
 ------------
 ::
```

### Comparing `GPy-ABCD-1.1/setup.py` & `GPy-ABCD-1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     filename = os.path.join(os.path.dirname(__file__), 'requirements.txt')
     with io.open(filename) as f:
         return [ine for line in f.read().splitlines() if (ine := str.lstrip(line)) if len(ine) > 0 if not ine.startswith('#')]
 
 
 setup(
     name = 'GPy-ABCD',
-    version = '1.1', # Change it in __init__.py too
+    version = '1.2', # Change it in __init__.py too
     url = 'https://github.com/T-Flet/GPy-ABCD',
     license = 'BSD 3-Clause',
 
     author = 'Thomas Fletcher',
     author_email = 'T-Fletcher@outlook.com',
 
     description = 'Basic implementation with GPy of an Automatic Bayesian Covariance Discovery (ABCD) system',
@@ -33,10 +33,13 @@
 
     install_requires = read_requirements(),
 
     classifiers = [
         'Development Status :: 4 - Beta',
         # 'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.8'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
 )
```

