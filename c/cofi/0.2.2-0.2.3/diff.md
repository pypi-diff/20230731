# Comparing `tmp/cofi-0.2.2.tar.gz` & `tmp/cofi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofi-0.2.2.tar", last modified: Mon Jul 17 23:17:39 2023, max compression
+gzip compressed data, was "cofi-0.2.3.tar", last modified: Mon Jul 31 05:15:24 2023, max compression
```

## Comparing `cofi-0.2.2.tar` & `cofi-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.906929 cofi-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-17 23:17:25.000000 cofi-0.2.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-17 23:17:39.906929 cofi-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-17 23:17:25.000000 cofi-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-17 23:17:26.000000 cofi-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:17:39.906929 cofi-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.898929 cofi-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67334 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_base_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_base_inference_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_cofi_simple_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_pytorch_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_scipy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_scipy_opt_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_scipy_opt_min.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_multiple_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_reg_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_reg_lp_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_reg_model_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.906929 cofi-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_for_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_for_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_inversion_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.199464 cofi-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-31 05:15:10.000000 cofi-0.2.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-31 05:15:24.199464 cofi-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-31 05:15:10.000000 cofi-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-31 05:15:10.000000 cofi-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 05:15:24.199464 cofi-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.195464 cofi-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.195464 cofi-0.2.3/src/cofi/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67334 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/_base_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 05:15:24.000000 cofi-0.2.3/src/cofi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.195464 cofi-0.2.3/src/cofi/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_base_inference_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_cofi_simple_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_pytorch_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_scipy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_scipy_opt_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/tools/_scipy_opt_min.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.199464 cofi-0.2.3/src/cofi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/utils/_multiple_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/utils/_reg_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/utils/_reg_lp_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/utils/_reg_model_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 05:15:10.000000 cofi-0.2.3/src/cofi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.195464 cofi-0.2.3/src/cofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-31 05:15:24.000000 cofi-0.2.3/src/cofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-31 05:15:24.000000 cofi-0.2.3/src/cofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:15:24.000000 cofi-0.2.3/src/cofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 05:15:24.000000 cofi-0.2.3/src/cofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 05:15:24.000000 cofi-0.2.3/src/cofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:15:24.199464 cofi-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_base_problem_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_base_problem_for_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_base_problem_for_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_base_problem_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-31 05:15:10.000000 cofi-0.2.3/tests/test_inversion_result.py
```

### Comparing `cofi-0.2.2/LICENCE` & `cofi-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/PKG-INFO` & `cofi-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `cofi-0.2.2/README.md` & `cofi-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/pyproject.toml` & `cofi-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/__init__.py` & `cofi-0.2.3/src/cofi/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/_base_problem.py` & `cofi-0.2.3/src/cofi/_base_problem.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/_exceptions.py` & `cofi-0.2.3/src/cofi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/_inversion.py` & `cofi-0.2.3/src/cofi/_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/_inversion_options.py` & `cofi-0.2.3/src/cofi/_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/tools/__init__.py` & `cofi-0.2.3/src/cofi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/tools/_base_inference_tool.py` & `cofi-0.2.3/src/cofi/tools/_base_inference_tool.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/tools/_cofi_simple_newton.py` & `cofi-0.2.3/src/cofi/tools/_cofi_simple_newton.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,7 +98,12 @@
 
     def _verbose_objective_value(self, i, m):
         obj_val = self.inv_problem.objective(m)
         self._n_obj_evaluations += 1
         if self._params["verbose"]:
             print(f"Iteration #{i}, updated objective function value: {obj_val}")
         return obj_val
+
+
+# CoFI -> Parameter estimation -> Optimization -> Non linear -> cofi.simple_newton -> Newton's method in optimization
+# description: CoFI's own implementation of the Newton's method in optimization with stopping criteria.
+# documentation: https://en.wikipedia.org/wiki/Newton%27s_method_in_optimization
```

### Comparing `cofi-0.2.2/src/cofi/tools/_emcee.py` & `cofi-0.2.3/src/cofi/tools/_emcee.py`

 * *Files 26% similar despite different names*

```diff
@@ -144,7 +144,40 @@
     )
     return (
         required_in_problem,
         optional_in_problem,
         required_in_options,
         optional_in_options,
     )
+
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> MHMove
+# description: A general Metropolis-Hastings proposal.
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.MHMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> GaussianMove
+# description: A Metropolis step with a Gaussian proposal function.
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.GaussianMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> RedBlueMove
+# description: An abstract red-blue ensemble move with parallelization as described in Foreman-Mackey et al. (2013).
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.RedBlueMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> StretchMove
+# description: A Goodman & Weare (2010) “stretch move” with parallelization as described in Foreman-Mackey et al. (2013).
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.StretchMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> WalkMove
+# description: A Goodman & Weare (2010) “walk move” with parallelization as described in Foreman-Mackey et al. (2013).
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.WalkMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> KDEMove
+# description: A proposal using a KDE of the complementary ensemble.
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.KDEMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> DEMove
+# description: A proposal using differential evolution.
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.DEMove
+
+# CoFI -> Ensemble methods -> Bayesian sampling -> McMC samplers -> emcee -> DESnookerMove
+# description: A snooker proposal using differential evolution.
+# documentation: https://emcee.readthedocs.io/en/stable/user/moves/#emcee.moves.DESnookerMove
```

### Comparing `cofi-0.2.2/src/cofi/tools/_pytorch_optim.py` & `cofi-0.2.3/src/cofi/tools/_scipy_opt_lstsq.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,183 +1,150 @@
 import functools
 
 from . import BaseInferenceTool, error_handler
 
 
-class PyTorchOptim(BaseInferenceTool):
+class ScipyOptLstSq(BaseInferenceTool):
     documentation_links = [
-        "https://pytorch.org/docs/stable/optim.html#algorithms",
+        "https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.least_squares.html"
     ]
-    short_description = "PyTorch Optimizers under module `pytorch.optim`"
+    short_description = (
+        "SciPy's non-linear least squares solver with bounds on variables, "
+        "algorithms include 'trf' (default), 'dogbox', and 'lm'"
+    )
 
     @classmethod
     def required_in_problem(cls) -> set:
-        return {"objective", "gradient", "initial_model"}
+        return _init_class_methods()[0]
 
     @classmethod
     def optional_in_problem(cls) -> dict:
-        return dict()
+        return _init_class_methods()[1]
 
     @classmethod
     def required_in_options(cls) -> set:
-        return {"algorithm", "num_iterations"}
+        return _init_class_methods()[2]
 
     @classmethod
     def optional_in_options(cls) -> dict:
-        return {
-            "verbose": True,
-            "callback": None,
-            "algorithm_params": dict(),
-        }
+        return _init_class_methods()[3]
 
     @classmethod
-    @functools.lru_cache(maxsize=None)
     def available_algorithms(cls) -> set:
-        import torch
-
-        optim_dir = dir(torch.optim)
-        algs = {name for name in optim_dir if name[0].isupper() and name != "Optimizer"}
-        return algs
+        return {"trf", "dogbox", "lm"}
 
     def __init__(self, inv_problem, inv_options):
-        # save extra options into inv_options.hyper_params["algorithm_params"]
-        if "algorithm_params" not in inv_options.hyper_params:
-            inv_options.hyper_params["algorithm_params"] = dict()
-        for param in list(inv_options.hyper_params):
-            if (
-                param not in self.optional_in_options()
-                and param not in self.required_in_options()
-            ):
-                inv_options.hyper_params["algorithm_params"][
-                    param
-                ] = inv_options.hyper_params.pop(param)
-
-        # initialisation, validation
         super().__init__(inv_problem, inv_options)
         self._components_used = list(self.required_in_problem())
-        self._validate_algorithm()
-
-        # save problem info for later use
-        self._obj = self.inv_problem.objective
-        self._grad = self.inv_problem.gradient
-
-        # initialize torch stuff
-        self._initialize_torch_tensor()
-        self._initialize_torch_optimizer()
-        self._initialize_torch_objective()
+        self._assign_args()
 
-        # initialize function evaluation counter
-        self._nb_evaluations = 0
+    def _assign_args(self):
+        inv_problem = self.inv_problem
+        # required_in_problem
+        self._fun = inv_problem.residual
+        self._x0 = inv_problem.initial_model
+        # optional_in_problem
+        defined_in_problem = self.inv_problem.defined_components()
+        for component in self.optional_in_problem():
+            if component in defined_in_problem:
+                setattr(
+                    self,
+                    f"_{component}" if component != "jacobian" else "_jac",
+                    getattr(self.inv_problem, component),
+                )
+                self._components_used.append(component)
+            else:  # default
+                setattr(
+                    self,
+                    f"_{component}" if component != "jacobian" else "_jac",
+                    self.optional_in_problem()[component],
+                )
 
     def __call__(self) -> dict:
-        import torch
-
-        losses = []
-        for i in range(self._params["num_iterations"]):
-            self._one_iteration(i, losses)
-        losses_out = torch.stack(losses)
-        return {
-            "model": self._m.detach().numpy(),
-            "objective_value": self._last_loss.detach().numpy(),
-            "losses": losses_out,
-            "n_obj_evaluations": self._nb_evaluations,
-            "n_grad_evaluations": self._nb_evaluations,
-            "success": True,
-        }
-
-    def _validate_algorithm(self):
-        if self._params["algorithm"] not in self.available_algorithms():
-            raise ValueError(
-                f"the algorithm you've chosen ({self._params['algorithm']}) "
-                "is invalid. Please choose from the following: "
-                f"{self.available_algorithms()}"
-            )
+        opt_result = self._call_np_least_squares()
+        result = dict(opt_result.items())
+        result["model"] = result.pop("x")
+        return result
 
     @error_handler(
-        when="in converting initial_model into PyTorch Tensor with requires_grad=True",
-        context="before solving the optimization problem",
+        when="when solving the least_squares optimization problem",
+        context="calling `scipy.optimize.least_squares`",
     )
-    def _initialize_torch_tensor(self):
-        import torch
+    def _call_np_least_squares(self):
+        from scipy.optimize import least_squares
 
-        if torch.is_tensor(self.inv_problem.initial_model):
-            self._m = (
-                self.inv_problem.initial_model.double()
-                .clone()
-                .detach()
-                .requires_grad_(True)
-            )
-        else:
-            self._m = torch.tensor(
-                self.inv_problem.initial_model, dtype=float, requires_grad=True
-            )
-
-    @error_handler(
-        when=f"in creating PyTorch Optimizer",
-        context="before solving the optimization problem",
-    )
-    def _initialize_torch_optimizer(self):
-        import torch
-
-        self.torch_optimizer = getattr(torch.optim, self._params["algorithm"])(
-            [self._m],
-            **self._params["algorithm_params"],
+        return least_squares(
+            fun=self._fun,
+            x0=self._x0,
+            jac=self._jac,
+            bounds=self._bounds,
+            method=self._params["method"],
+            ftol=self._params["ftol"],
+            xtol=self._params["xtol"],
+            gtol=self._params["gtol"],
+            x_scale=self._params["x_scale"],
+            loss=self._params["loss"],
+            f_scale=self._params["f_scale"],
+            diff_step=self._params["diff_step"],
+            tr_solver=self._params["tr_solver"],
+            tr_options=self._params["tr_options"],
+            jac_sparsity=self._params["jac_sparsity"],
+            max_nfev=self._params["max_nfev"],
+            verbose=self._params["verbose"],
+            args=(),  # handled by cofi.BaseProblem
+            kwargs={},  # handled by cofi.BaseProblem
         )
 
-    @error_handler(
-        when="in creating PyTorch custom Loss Function",
-        context="before solving the optimization problem",
-    )
-    def _initialize_torch_objective(self):
-        self.torch_objective = _CoFIObjective().apply
 
-    @error_handler(
-        when="when performing optimization stepping",
-        context="in the process of solving",
-    )
-    def _one_iteration(self, i, losses):
-        def closure():
-            self.torch_optimizer.zero_grad()
-            self._last_loss = self.torch_objective(self._m, self._obj, self._grad)
-            self._last_loss.backward()
-            self._nb_evaluations += 1
-            return self._last_loss
-
-        self.torch_optimizer.step(closure)
-        losses.append(self._last_loss)
-        if self._params["callback"] is not None:
-            self._run_callback()
-        if self._params["verbose"]:
-            print(f"Iteration #{i}, objective value: {self._last_loss}")
-
-    @error_handler(
-        when="when running your callback function",
-        context="in the process of solving",
+@functools.lru_cache(maxsize=None)
+def _init_class_methods():
+    """get a list of arguments and defaults for scipy.minimize.least_squares
+
+    TODO arguments not supported by BaseProblem due to myself not sure how this can be
+    handled for other backend tools: `args`, `kwargs`, `x_scale`, `loss`, `f_scale`
+    """
+    import inspect
+    from scipy.optimize import least_squares
+
+    _scipy_ls_args = dict(inspect.signature(least_squares).parameters)
+    _scipy_ls_args["jacobian"] = _scipy_ls_args.pop("jac")
+    required_in_problem = {"residual", "initial_model"}
+    optional_in_problem = {
+        k: v.default for k, v in _scipy_ls_args.items() if k in {"jacobian", "bounds"}
+    }
+    required_in_options = set()
+    optional_in_options = {
+        k: v.default
+        for k, v in _scipy_ls_args.items()
+        if k
+        in {
+            "method",
+            "ftol",
+            "xtol",
+            "gtol",
+            "x_scale",
+            "f_scale",
+            "loss",
+            "diff_step",
+            "tr_solver",
+            "tr_options",
+            "jac_sparsity",
+            "max_nfev",
+            "verbose",
+        }
+    }
+    return (
+        required_in_problem,
+        optional_in_problem,
+        required_in_options,
+        optional_in_options,
     )
-    def _run_callback(self):
-        self._params["callback"](self._m)
 
 
-def _CoFIObjective():
-    import torch
+# CoFI -> Parameter estimation -> Optimization -> Non linear -> scipy.optimize.least_squares -> trf
+# description: Trust Region Reflective algorithm, particularly suitable for large sparse problems with bounds.
 
-    class CoFIObjective(torch.autograd.Function):
-        # https://pytorch.org/docs/stable/generated/torch.autograd.Function.backward.html
-        @staticmethod
-        def forward(ctx, m, my_objective, my_gradient):
-            # calculate and save gradient value
-            grad = my_gradient(m)
-            if not torch.is_tensor(grad):  # converting type only when not tensor
-                grad = torch.tensor(grad)
-            ctx.save_for_backward(grad)
-            # calculate and return objective value
-            obj_val = my_objective(m)
-            if not torch.is_tensor(obj_val):  # converting type only when not tensor
-                obj_val = torch.tensor(obj_val, requires_grad=True)
-            return obj_val
-
-        @staticmethod
-        def backward(ctx, _):
-            grad = ctx.saved_tensors[0]
-            return grad, None, None
+# CoFI -> Parameter estimation -> Optimization -> Non linear -> scipy.optimize.least_squares -> dogbox
+# description: Dogleg algorithm with rectangular trust regions, typical use case is small problems with bounds.
 
-    return CoFIObjective
+# CoFI -> Parameter estimation -> Optimization -> Non linear -> scipy.optimize.least_squares -> lm
+# description: Levenberg-Marquardt algorithm as implemented in MINPACK. Doesn’t handle bounds and sparse Jacobians.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cofi-0.2.2/src/cofi/tools/_scipy_lstsq.py` & `cofi-0.2.3/src/cofi/tools/_scipy_lstsq.py`

 * *Files 10% similar despite different names*

```diff
@@ -192,7 +192,17 @@
     optional_in_options["with_tikhonov_if_possible"] = True
     return (
         required_in_problem,
         optional_in_problem,
         required_in_options,
         optional_in_options,
     )
+
+
+# CoFI -> Parameter estimation -> Matrix based solvers -> Linear system solvers -> scipy.linalg.lstsq -> gelsd
+# description: Solve linear least squares using divide-and-conquer SVD.
+
+# CoFI -> Parameter estimation -> Matrix based solvers -> Linear system solvers -> scipy.linalg.lstsq -> gelsy
+# description: Solve linear least squares using complete orthogonal factorization.
+
+# CoFI -> Parameter estimation -> Matrix based solvers -> Linear system solvers -> scipy.linalg.lstsq -> gelss
+# description: Solve linear least squares using SVD.
```

### Comparing `cofi-0.2.2/src/cofi/utils/__init__.py` & `cofi-0.2.3/src/cofi/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 """
 
 from ._reg_base import BaseRegularization
 from ._reg_lp_norm import LpNormRegularization, QuadraticReg
 from ._reg_model_cov import ModelCovariance, GaussianPrior
 
-from ._multiple_runs import run_multiple_inversions
+from ._multiple_runs import InversionPool
 
 
 __all__ = [
     "BaseRegularization",
     "LpNormRegularization",
     "QuadraticReg",
     "ModelCovariance",
     "GaussianPrior",
-    "run_multiple_inversions",
+    "InversionPool",
 ]
```

### Comparing `cofi-0.2.2/src/cofi/utils/_reg_base.py` & `cofi-0.2.3/src/cofi/utils/_reg_base.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/utils/_reg_lp_norm.py` & `cofi-0.2.3/src/cofi/utils/_reg_lp_norm.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi/utils/_reg_model_cov.py` & `cofi-0.2.3/src/cofi/utils/_reg_model_cov.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/src/cofi.egg-info/PKG-INFO` & `cofi-0.2.3/src/cofi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `cofi-0.2.2/src/cofi.egg-info/SOURCES.txt` & `cofi-0.2.3/src/cofi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_base_problem_basics.py` & `cofi-0.2.3/tests/test_base_problem_basics.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_base_problem_for_optimization.py` & `cofi-0.2.3/tests/test_base_problem_for_optimization.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_base_problem_for_sampling.py` & `cofi-0.2.3/tests/test_base_problem_for_sampling.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_base_problem_misc.py` & `cofi-0.2.3/tests/test_base_problem_misc.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_inversion.py` & `cofi-0.2.3/tests/test_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_inversion_options.py` & `cofi-0.2.3/tests/test_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.2/tests/test_inversion_result.py` & `cofi-0.2.3/tests/test_inversion_result.py`

 * *Files identical despite different names*

