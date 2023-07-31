# Comparing `tmp/stable-trunc-gaussian-1.1.0.tar.gz` & `tmp/stable-trunc-gaussian-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-trunc-gaussian-1.1.0.tar", last modified: Sun Jul 30 04:24:30 2023, max compression
+gzip compressed data, was "stable-trunc-gaussian-1.1.1.tar", last modified: Mon Jul 31 20:15:45 2023, max compression
```

## Comparing `stable-trunc-gaussian-1.1.0.tar` & `stable-trunc-gaussian-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.1.0/LICENSE
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.1.0/MANIFEST.in
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4580 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     2730 2023-07-30 04:20:01.000000 stable-trunc-gaussian-1.1.0/README.md
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-30 04:22:54.000000 stable-trunc-gaussian-1.1.0/pyproject.toml
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/setup.cfg
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.741945 stable-trunc-gaussian-1.1.0/src/
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.741945 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      213 2023-07-30 04:23:15.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/__init__.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)    11308 2023-07-30 03:54:38.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/parallel_trunc_gaussian.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7429 2023-07-30 03:59:16.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/sequential_trunc_gaussian.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4095 2023-07-30 04:02:06.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/tests.py
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-30 04:24:30.745945 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4580 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      469 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/SOURCES.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/dependency_links.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/requires.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-30 04:24:30.000000 stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/top_level.txt
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.1.1/LICENSE
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.1.1/MANIFEST.in
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4842 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     2992 2023-07-31 20:08:29.000000 stable-trunc-gaussian-1.1.1/README.md
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-31 19:53:28.000000 stable-trunc-gaussian-1.1.1/pyproject.toml
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/setup.cfg
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.089144 stable-trunc-gaussian-1.1.1/src/
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.089144 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      213 2023-07-31 19:52:48.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/__init__.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)    10080 2023-07-31 20:08:29.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/parallel_trunc_gaussian.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7429 2023-07-30 03:59:16.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/sequential_trunc_gaussian.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4095 2023-07-30 04:02:06.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/tests.py
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-31 20:15:45.093144 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4842 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      469 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/SOURCES.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/dependency_links.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/requires.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-31 20:15:45.000000 stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/top_level.txt
```

### Comparing `stable-trunc-gaussian-1.1.0/LICENSE` & `stable-trunc-gaussian-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.1.0/PKG-INFO` & `stable-trunc-gaussian-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.1.0
+Version: 1.1.1
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-`[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
 [![Downloads](https://static.pepy.tech/badge/stable-trunc-gaussian)](https://pepy.tech/project/stable-trunc-gaussian)
 
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
@@ -76,7 +76,11 @@
     # Parallel computation
     means = TruncatedGaussian(t([0,0.5]),t(1,1),t(-1,2),t(1,5)).mean
 
     # Sequential computation
     # Note: the 'TruncatedGaussian' class can also be used for this sequential case
     mean_0 = SeqTruncatedGaussian(t([0]),t(1),t(-1),t(1)).mean
     mean_1 = SeqTruncatedGaussian(t([0.5]),t(1),t(2),t(5)).mean
+
+# Acknowledgements
+
+We want to thank users [KFrank](https://discuss.pytorch.org/u/KFrank) and [ptrblck](https://discuss.pytorch.org/u/ptrblck) for their help in solving the bug when computing the gradients for the parallel version (bug solved in version 1.1.1).
```

### Comparing `stable-trunc-gaussian-1.1.0/README.md` & `stable-trunc-gaussian-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-`[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
 [![Downloads](https://static.pepy.tech/badge/stable-trunc-gaussian)](https://pepy.tech/project/stable-trunc-gaussian)
 
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
@@ -40,7 +40,11 @@
     # Parallel computation
     means = TruncatedGaussian(t([0,0.5]),t(1,1),t(-1,2),t(1,5)).mean
 
     # Sequential computation
     # Note: the 'TruncatedGaussian' class can also be used for this sequential case
     mean_0 = SeqTruncatedGaussian(t([0]),t(1),t(-1),t(1)).mean
     mean_1 = SeqTruncatedGaussian(t([0.5]),t(1),t(2),t(5)).mean
+
+# Acknowledgements
+
+We want to thank users [KFrank](https://discuss.pytorch.org/u/KFrank) and [ptrblck](https://discuss.pytorch.org/u/ptrblck) for their help in solving the bug when computing the gradients for the parallel version (bug solved in version 1.1.1).
```

### Comparing `stable-trunc-gaussian-1.1.0/pyproject.toml` & `stable-trunc-gaussian-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="stable-trunc-gaussian"
-version="1.1.0"
+version="1.1.1"
 description="A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch."
 readme="README.md"
 authors = [{ name = "Carlos Núñez Molina", email = "ccaarlos@ugr.es" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/parallel_trunc_gaussian.py` & `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/parallel_trunc_gaussian.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 
 Right now, we only implement the following methods: mean, variance and log_prob.
 """
 
 import torch
 from torch.special import erf, erfc, erfcx
 from torch.distributions import Distribution, constraints
+from torch import where
 import math
 
 # Constants
 SQRT_PI = math.sqrt(math.pi)
 SQRT_2 = math.sqrt(2)
 SQRT_2_PI = math.sqrt(2*math.pi)
 INV_SQRT_2 = 1/SQRT_2
 INV_SQRT_PI = 1/SQRT_PI
 INV_PI = 1/math.pi
+SQRT_2_DIV_SQRT_PI = SQRT_2 / SQRT_PI
 LOG_SQRT_2_PI = math.log(SQRT_2_PI)
 LOG_2 = math.log(2)
 
+
+EPS = torch.finfo(torch.float32).eps
+
 class ParallelTruncatedGaussian(Distribution):
 
 	has_rsample = False
 
 	arg_constraints = {
 		'mu': constraints.real,
 		'sigma': constraints.positive,
@@ -129,157 +134,127 @@
 	
 	@staticmethod
 	def _F_1(x_, y_):
 		# All values in tensor @x must be smaller than values in tensor @y
 		x = torch.where(torch.abs(x_)<=torch.abs(y_),x_,y_)
 		y = torch.where(torch.abs(y_)>=torch.abs(x_),y_,x_)
 
-		# Values
+		# Obtain masks
+		with torch.no_grad():
+			out1_cond = torch.abs(x - y) < 1e-7 # tensor([False, False, False, False])
+			out2_cond = torch.logical_and( torch.logical_and(x<=0, y<=0), torch.logical_not(out1_cond) ) # tensor([False,  True, False, False])
+			out3_cond = torch.logical_and( torch.logical_and(x>=0, y>=0), torch.logical_not(out1_cond) ) # tensor([False, False, False,  True]) 
+			out4_cond = torch.logical_and( torch.logical_and( torch.logical_not(out1_cond), torch.logical_not(out2_cond) ),
+										   torch.logical_not(out3_cond) ) # All the other conditions must be false
+
+
+		# Mask input values for each operation
+		x1, y1 = where(out1_cond, x, 0), where(out1_cond, y, 0)
+		x2, y2 = where(out2_cond, x, -1), where(out2_cond, y, 0)
+		x3, y3 = where(out3_cond, x, 0), where(out3_cond, y, 1)
+		x4, y4 = where(out4_cond, x, 0), where(out4_cond, y, 1)
+
+		# Apply operations
 		delt = ParallelTruncatedGaussian._delta(x, y)
 		one_minus_delt = 1 - delt
-		out1 = ParallelTruncatedGaussian._P_1(x, y-x)
-		out2 = one_minus_delt / (delt*erfcx(-y) - erfcx(-x))
-		out3 = one_minus_delt / (erfcx(x) - delt*erfcx(y))
-		out4 = (one_minus_delt*torch.exp(-x**2)) / (erf(y)-erf(x))
-
-		# Conditions
-		out1_cond = torch.abs(x - y) < 1e-7
-		out2_cond = torch.logical_and( torch.logical_and(x<=0, y<=0), torch.logical_not(out1_cond) )
-		out3_cond = torch.logical_and( torch.logical_and(x>=0, y>=0), torch.logical_not(out1_cond) )
-		out4_cond = torch.logical_and( torch.logical_and( torch.logical_not(out1_cond), torch.logical_not(out2_cond) ),
-									   torch.logical_not(out3_cond) ) # All the other conditions must be false
-
-		# Final expression
-		# We need to set nan, -inf, inf values to 0.0 since, otherwise, 0*inf may result in NaNs
-		# in the final formula
-		final_out = torch.nan_to_num(out1,nan=0.0,posinf=0.0,neginf=0.0)*out1_cond + \
-			  		torch.nan_to_num(out2,nan=0.0,posinf=0.0,neginf=0.0)*out2_cond + \
-					torch.nan_to_num(out3,nan=0.0,posinf=0.0,neginf=0.0)*out3_cond + \
-					torch.nan_to_num(out4,nan=0.0,posinf=0.0,neginf=0.0)*out4_cond
 
-		return final_out
+		out1_m = ParallelTruncatedGaussian._P_1(x1, y1-x1)
+		out2_m = one_minus_delt / (delt*erfcx(-y2) - erfcx(-x2))
+		out3_m = one_minus_delt / (erfcx(x3) - delt*erfcx(y3))
+		out4_m = (one_minus_delt*torch.exp(-x4**2)) / (erf(y4)-erf(x4))
+
+		# Unmask tensors, by setting masked values to 0
+		out1 = where(out1_cond, out1_m, 0)
+		out2 = where(out2_cond, out2_m, 0)
+		out3 = where(out3_cond, out3_m, 0)
+		out4 = where(out4_cond, out4_m, 0)
 
-		"""
-		Sequential code
-	
-		if torch.abs(x) > torch.abs(y):
-			out = ParallelTruncatedGaussian._F_1(y, x)
+		# Add them up into a single tensor
+		final_out = out1 + out2 + out3 + out4
+		
+		return final_out
 
-		elif torch.abs(x - y) < 1e-7: #out1_cond
-			out = ParallelTruncatedGaussian._P_1(x, y-x)
-		elif x <= 0 and y <= 0: #out2_cond
-			delt = ParallelTruncatedGaussian._delta(x, y)
-			out = (1 - delt) / (delt*erfcx(-y) - erfcx(-x))  
-		elif x >= 0 and y >= 0: #out3_cond
-			delt = ParallelTruncatedGaussian._delta(x, y)
-			out = (1 - delt) / (erfcx(x) - delt*erfcx(y))
-		else: #out4_cond
-			delt = ParallelTruncatedGaussian._delta(x, y)
-			out = ((1-delt)*torch.exp(-x**2)) / (erf(y)-erf(x))
-		"""
-	
 	@staticmethod
 	def _F_2(x_, y_):
 		# All values in tensor @x must be smaller than values in tensor @y
 		x = torch.where(torch.abs(x_)<=torch.abs(y_),x_,y_)
 		y = torch.where(torch.abs(y_)>=torch.abs(x_),y_,x_)
 
-		# Values
+		# Obtain masks
+		with torch.no_grad():
+			out1_cond = torch.abs(x - y) < 1e-7 # tensor([False, False, False, False])
+			out2_cond = torch.logical_and( torch.logical_and(x<=0, y<=0), torch.logical_not(out1_cond) ) # tensor([False,  True, False, False])
+			out3_cond = torch.logical_and( torch.logical_and(x>=0, y>=0), torch.logical_not(out1_cond) ) # tensor([False, False, False,  True]) 
+			out4_cond = torch.logical_and( torch.logical_and( torch.logical_not(out1_cond), torch.logical_not(out2_cond) ),
+										   torch.logical_not(out3_cond) ) # All the other conditions must be false
+
+		# Mask input values for each operation
+		x1, y1 = where(out1_cond, x, 0), where(out1_cond, y, 0)
+		x2, y2 = where(out2_cond, x, -1), where(out2_cond, y, 0)
+		x3, y3 = where(out3_cond, x, 0), where(out3_cond, y, 1)
+		x4, y4 = where(out4_cond, x, 0), where(out4_cond, y, 1)
+
+		# Apply operations
 		delt = ParallelTruncatedGaussian._delta(x, y)
 		x_minus_y_by_delt = x - y*delt
-		out1 = ParallelTruncatedGaussian._P_2(x, y-x)
-		out2 = x_minus_y_by_delt / (delt*erfcx(-y) - erfcx(-x)) 
-		out3 = x_minus_y_by_delt / (erfcx(x) - delt*erfcx(y))
-		out4 = (x_minus_y_by_delt*torch.exp(-x**2)) / (erf(y)-erf(x))
-
-		# Conditions
-		out1_cond = torch.abs(x - y) < 1e-7
-		out2_cond = torch.logical_and( torch.logical_and(x<=0, y<=0), torch.logical_not(out1_cond) )
-		out3_cond = torch.logical_and( torch.logical_and(x>=0, y>=0), torch.logical_not(out1_cond) )
-		out4_cond = torch.logical_and( torch.logical_and( torch.logical_not(out1_cond), torch.logical_not(out2_cond) ),
-									   torch.logical_not(out3_cond) ) # All the other conditions must be false
-
-		# We need to set nan, -inf, inf values to 0.0 since, otherwise, 0*inf may result in NaNs
-		# in the final formula
-		final_out = torch.nan_to_num(out1,nan=0.0,posinf=0.0,neginf=0.0)*out1_cond + \
-			  		torch.nan_to_num(out2,nan=0.0,posinf=0.0,neginf=0.0)*out2_cond + \
-					torch.nan_to_num(out3,nan=0.0,posinf=0.0,neginf=0.0)*out3_cond + \
-					torch.nan_to_num(out4,nan=0.0,posinf=0.0,neginf=0.0)*out4_cond
 
-		return final_out
+		out1_m = ParallelTruncatedGaussian._P_2(x1, y1-x1)
+		out2_m = x_minus_y_by_delt / (delt*erfcx(-y2) - erfcx(-x2)) 
+		out3_m = x_minus_y_by_delt / (erfcx(x3) - delt*erfcx(y3))
+		out4_m = (x_minus_y_by_delt*torch.exp(-x4**2)) / (erf(y4)-erf(x4))
+
+		# Unmask tensors, by setting masked values to 0
+		out1 = where(out1_cond, out1_m, 0)
+		out2 = where(out2_cond, out2_m, 0)
+		out3 = where(out3_cond, out3_m, 0)
+		out4 = where(out4_cond, out4_m, 0)
 
-		"""
-		Sequential code
-		
-		if torch.abs(x) > torch.abs(y):
-			out = ParallelTruncatedGaussian._F_2(y, x)
+		# Add them up into a single tensor
+		final_out = out1 + out2 + out3 + out4
+
+		return final_out
 
-		elif torch.abs(x - y) < 1e-7: #out1_cond
-			out = ParallelTruncatedGaussian._P_2(x, y-x)
-		elif x <= 0 and y <= 0: #out2_cond
-			delt = ParallelTruncatedGaussian._delta(x, y)
-			out = (x - y*delt) / (delt*erfcx(-y) - erfcx(-x))  
-		elif x >= 0 and y >= 0: #out3_cond 
-			delt = ParallelTruncatedGaussian._delta(x, y)
-			out = (x - y*delt) / (erfcx(x) - delt*erfcx(y))
-		else: #out4_cond
-			delt = ParallelTruncatedGaussian._delta(x, y)
-			out = ((x-y*delt)*torch.exp(-x**2)) / (erf(y)-erf(x))
-		"""
-		
-	
 	# Numerically stable implementation of Z=log(big_phi(beta)-big_phi(alpha))
 	def _calculate_log_Z(self):
-		# Values
-		alpha_beta_sqr_diff = (self._alpha+self._beta)*(self._alpha-self._beta)
-		beta_alpha_sqr_diff = -alpha_beta_sqr_diff
-		out1 = -torch.log( (self._mean-self._mu) / self._sigma ) - LOG_SQRT_2_PI - (self._alpha**2)/2 + \
-				torch.log(1 - torch.exp(alpha_beta_sqr_diff / 2))
-		out2 = -torch.log( (self._mu-self._mean) / self._sigma ) - LOG_SQRT_2_PI - (self._beta**2)/2 + \
-				torch.log(1 - torch.exp(beta_alpha_sqr_diff / 2))
-		out3 = -LOG_2 + torch.log(erf(self._beta*INV_SQRT_2) - erf(self._alpha*INV_SQRT_2))
-
-		# Conditions
-		out1_cond = torch.logical_and(self._alpha>=0, self._beta>=0)
-		out2_cond = torch.logical_and(self._alpha<=0, self._beta<=0)
-		out3_cond = torch.logical_and(torch.logical_not(out1_cond), torch.logical_not(out2_cond))
-		
-		# Final expression
-		# We need to set nan, -inf, inf values to 0.0 since, otherwise, 0*inf may result in NaNs
-		# in the final formula
-		final_out = torch.nan_to_num(out1,nan=0.0,posinf=0.0,neginf=0.0)*out1_cond + \
-			  		torch.nan_to_num(out2,nan=0.0,posinf=0.0,neginf=0.0)*out2_cond + \
-					torch.nan_to_num(out3,nan=0.0,posinf=0.0,neginf=0.0)*out3_cond
+		alpha, beta, mu, mean_d = self._alpha, self._beta, self._mu, self._mean.detach()
 
-		return final_out
+		# Obtain masks
+		with torch.no_grad():
+			out1_cond = torch.logical_and(alpha>=0, beta>=0)
+			out2_cond = torch.logical_and(alpha<=0, beta<=0)
+			out3_cond = torch.logical_and(torch.logical_not(out1_cond), torch.logical_not(out2_cond))
+
+		# Mask input values for each operation
+		alpha1, beta1, mu1 = where(out1_cond, alpha, 0), where(out1_cond, beta, 1), where(out1_cond, mu, mean_d-1)
+		alpha2, beta2, mu2 = where(out2_cond, alpha, 1), where(out2_cond, beta, 0), where(out2_cond, mu, mean_d+1)
+		alpha3, beta3 = where(out3_cond, alpha, 0), where(out3_cond, beta, 1)
+
+		# Apply operations
+		out1_m = -torch.log( (self._mean-mu1) / self._sigma ) - LOG_SQRT_2_PI - (alpha1**2)/2 + \
+				torch.log(1 - torch.exp( (alpha1+beta1)*(alpha1-beta1) / 2 ))
+		out2_m = -torch.log( (mu2-self._mean) / self._sigma ) - LOG_SQRT_2_PI - (beta2**2)/2 + \
+			    torch.log(1 - torch.exp( (alpha2+beta2)*(beta2-alpha2) / 2))
+		out3_m = -LOG_2 + torch.log(erf(beta3*INV_SQRT_2) - erf(alpha3*INV_SQRT_2))
+
+		# Unmask tensors, by setting masked values to 0
+		out1 = where(out1_cond, out1_m, 0)
+		out2 = where(out2_cond, out2_m, 0)
+		out3 = where(out3_cond, out3_m, 0)
 
-		"""
-		Sequential code
-		
-		if self._alpha>=0 and self._beta>=0: # mu is smaller or equal than a and b #out1_cond
-			alpha_beta_sqr_diff = (self._alpha+self._beta)*(self._alpha-self._beta) # alpha**2 - beta**2
-			result = -torch.log( (self._mean-self._mu) / self._sigma ) - LOG_SQRT_2_PI - (self._alpha**2)/2 + \
-					torch.log(1 - torch.exp(alpha_beta_sqr_diff / 2))
-		
-		elif self._alpha<=0 and self._beta<=0: # mu is larger or equal than a and b #out2_cond
-			beta_alpha_sqr_diff = (self._beta+self._alpha)*(self._beta-self._alpha) # beta**2 - alpha**2
-			result = -torch.log( (self._mu-self._mean) / self._sigma ) - LOG_SQRT_2_PI - (self._beta**2)/2 + \
-					torch.log(1 - torch.exp(beta_alpha_sqr_diff / 2))
-		
-		else: # alpha and beta have different sign (which means mu lies in the interval [a,b]) #out3_cond
-			result = -LOG_2 + torch.log(erf(self._beta*INV_SQRT_2) - erf(self._alpha*INV_SQRT_2))
-		"""
-		
+		# Add them up into a single tensor
+		final_out = out1 + out2 + out3
+
+		return final_out	
 	
 	# --- Main methods ---
 
 	# Mean of the distribution (after truncation)
 	def _calculate_mean(self):
 		cls = self.__class__
-		fraction = (SQRT_2 / SQRT_PI) * cls._F_1(self._alpha*INV_SQRT_2, self._beta*INV_SQRT_2)
+		fraction = SQRT_2_DIV_SQRT_PI * cls._F_1(self._alpha*INV_SQRT_2, self._beta*INV_SQRT_2)
 		result = self._mu + fraction*self._sigma
 
 		return result
 
 	@property
 	def mean(self):
 		return self._mean
@@ -311,8 +286,8 @@
 
 		xi = (x-self._mu)/self._sigma
 		term_1 = -torch.log(self._sigma)
 		term_2 = -LOG_SQRT_2_PI - (xi**2)/2    
 		term_3 = -self._log_Z
 		result = term_1 + term_2 + term_3
 
-		return result
+		return result
```

### Comparing `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/sequential_trunc_gaussian.py` & `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/sequential_trunc_gaussian.py`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian/tests.py` & `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian/tests.py`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.1.0/src/stable_trunc_gaussian.egg-info/PKG-INFO` & `stable-trunc-gaussian-1.1.1/src/stable_trunc_gaussian.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.1.0
+Version: 1.1.1
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-`[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
 [![Downloads](https://static.pepy.tech/badge/stable-trunc-gaussian)](https://pepy.tech/project/stable-trunc-gaussian)
 
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
@@ -76,7 +76,11 @@
     # Parallel computation
     means = TruncatedGaussian(t([0,0.5]),t(1,1),t(-1,2),t(1,5)).mean
 
     # Sequential computation
     # Note: the 'TruncatedGaussian' class can also be used for this sequential case
     mean_0 = SeqTruncatedGaussian(t([0]),t(1),t(-1),t(1)).mean
     mean_1 = SeqTruncatedGaussian(t([0.5]),t(1),t(2),t(5)).mean
+
+# Acknowledgements
+
+We want to thank users [KFrank](https://discuss.pytorch.org/u/KFrank) and [ptrblck](https://discuss.pytorch.org/u/ptrblck) for their help in solving the bug when computing the gradients for the parallel version (bug solved in version 1.1.1).
```

