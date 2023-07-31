# Comparing `tmp/hiveviewer-0.1.1.tar.gz` & `tmp/hiveviewer-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.1.1.tar", last modified: Mon Jul 31 12:17:30 2023, max compression
+gzip compressed data, was "hiveviewer-0.1.12.tar", last modified: Mon Jul 31 12:28:12 2023, max compression
```

## Comparing `hiveviewer-0.1.1.tar` & `hiveviewer-0.1.12.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.241145 hiveviewer-0.1.1/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.1.1/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-31 12:17:30.241032 hiveviewer-0.1.1/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.1.1/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.1.1/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-07-31 12:17:30.241183 hiveviewer-0.1.1/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)      988 2023-07-31 12:17:01.000000 hiveviewer-0.1.1/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.233574 hiveviewer-0.1.1/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.234855 hiveviewer-0.1.1/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.1.1/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.236953 hiveviewer-0.1.1/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.237526 hiveviewer-0.1.1/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.1.1/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     6440 2023-07-31 12:13:52.000000 hiveviewer-0.1.1/src/hiveviewer/evaluation/calculator.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.238275 hiveviewer-0.1.1/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-07-19 08:12:07.000000 hiveviewer-0.1.1/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-07-20 10:58:22.000000 hiveviewer-0.1.1/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     5217 2023-07-28 09:00:29.000000 hiveviewer-0.1.1/src/hiveviewer/optimization/profolio_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.239205 hiveviewer-0.1.1/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/frequency_sampler.py
--rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.240747 hiveviewer-0.1.1/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.235699 hiveviewer-0.1.1/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)     1013 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       75 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.794550 hiveviewer-0.1.12/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.1.12/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1127 2023-07-31 12:28:12.794426 hiveviewer-0.1.12/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.1.12/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.1.12/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-07-31 12:28:12.794589 hiveviewer-0.1.12/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)     1007 2023-07-31 12:27:36.000000 hiveviewer-0.1.12/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.789270 hiveviewer-0.1.12/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.790513 hiveviewer-0.1.12/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.1.12/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.791833 hiveviewer-0.1.12/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.792094 hiveviewer-0.1.12/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.1.12/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     6440 2023-07-31 12:13:52.000000 hiveviewer-0.1.12/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.792574 hiveviewer-0.1.12/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-07-19 08:12:07.000000 hiveviewer-0.1.12/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-07-20 10:58:22.000000 hiveviewer-0.1.12/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     5105 2023-07-31 12:24:57.000000 hiveviewer-0.1.12/src/hiveviewer/optimization/profolio_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.793400 hiveviewer-0.1.12/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.794234 hiveviewer-0.1.12/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.791248 hiveviewer-0.1.12/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1127 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1013 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       82 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.1.1/LICENSE` & `hiveviewer-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/PKG-INFO` & `hiveviewer-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.1.1
+Version: 0.1.12
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.1.1/README.md` & `hiveviewer-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/setup.py` & `hiveviewer-0.1.12/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,21 @@
         "numpy",
         "matplotlib",
         "imageio",
         "tqdm",
         "scikit-learn",
         "matplotlib_venn",
         "openpyxl",
+        "optuna",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.1.1",
+    version="0.1.12",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.1.1/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.1.12/src/hiveviewer/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.1.12/src/hiveviewer/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/dataloader/load_excel.py` & `hiveviewer-0.1.12/src/hiveviewer/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/evaluation/calculator.py` & `hiveviewer-0.1.12/src/hiveviewer/evaluation/calculator.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/optimization/base.py` & `hiveviewer-0.1.12/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/optimization/profolio_objective.py` & `hiveviewer-0.1.12/src/hiveviewer/optimization/profolio_objective.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import logging
-from typing import List, Literal, Optional
+from typing import List, Optional
 
-import numpy as np
 import optuna
 from optuna.trial import Trial
 
 from ..evaluation.calculator import Calculator
 from .base import BaseObjective
 
 
 class ProfolioObjective(BaseObjective):
     """
     This class provides methods to optimize the profolio objective.
     """
 
     def __init__(
         self,
-        direction: Literal["minimize", "maximize"],
+        direction: str,
         weights_num: int,
         formula: str,
         first_order: bool = False,
         first_order_lower_bound: float = 1e-3,
         first_order_upper_bound: float = 1e6,
         dirichlet: bool = True,
         log_file: Optional[str] = None,
     ) -> None:
         """
         Initialize with direction, weights_num, formula and dirichlet.
 
         Args:
-            direction (Literal["minimize", "maximize"]): direction to optimize.
+            direction (str ["minimize", "maximize"]): direction to optimize.
             weights_num (int): numbers of weights to search.
             formula (str): formula of targets to calculate the objective.
             dirichlet (bool, optional): Use dirichlet distribution or not. Defaults to True.
         """
         super().__init__(direction, formula, first_order, dirichlet)
         self.calculators: List[Calculator] = []
-        self.calculator_flags: List[Literal["wuauc", "profolio"]] = []
+        self.calculator_flags: List[str] = []
         self.hyperparameters: List[Optional[float]] = []
         self.target_columns: List[str] = []
         self.weights_num = weights_num
         self.formula = formula
         self.first_order = first_order
         self.first_order_lower_bound = first_order_lower_bound
         self.first_order_upper_bound = first_order_upper_bound
@@ -54,23 +53,23 @@
         file_handler.setLevel(logging.INFO)
         self.logger = optuna.logging.get_logger("optuna")
         self.logger.addHandler(file_handler)
 
     def add_calculator(
         self,
         calculator: Calculator,
-        flag: Literal["wuauc", "profolio"],
+        flag: str,
         hyperparameter: Optional[float],
         target_column: str,
     ) -> None:
         """Add calculators to the objective.
 
         Args:
             calculator (Calculator): calculator building blocks.
-            flag (Literal["wuauc", "profolio"]): type of calculation.
+            flag (str ["wuauc", "profolio"]): type of calculation.
             target_column (str): target column to calculate.
         """
         self.calculators.append(calculator)
         self.calculator_flags.append(flag)
         self.target_columns.append(target_column)
         if hyperparameter:
             self.hyperparameters.append(hyperparameter)
```

### Comparing `hiveviewer-0.1.1/src/hiveviewer/sampling/base.py` & `hiveviewer-0.1.12/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/sampling/frequency_sampler.py` & `hiveviewer-0.1.12/src/hiveviewer/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.1.12/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.1.12/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.1.12/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.1.12/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.1.12/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.1.12/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.1/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.1.12/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.1.1
+Version: 0.1.12
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.1.1/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.1.12/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

