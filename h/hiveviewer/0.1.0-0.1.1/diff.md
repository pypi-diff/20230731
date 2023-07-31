# Comparing `tmp/hiveviewer-0.1.0.tar.gz` & `tmp/hiveviewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.1.0.tar", last modified: Fri Jul 21 04:24:06 2023, max compression
+gzip compressed data, was "hiveviewer-0.1.1.tar", last modified: Mon Jul 31 12:17:30 2023, max compression
```

## Comparing `hiveviewer-0.1.0.tar` & `hiveviewer-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.436545 hiveviewer-0.1.0/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.1.0/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-21 04:24:06.436431 hiveviewer-0.1.0/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.1.0/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.1.0/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-07-21 04:24:06.436595 hiveviewer-0.1.0/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)      988 2023-07-21 04:23:33.000000 hiveviewer-0.1.0/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.431531 hiveviewer-0.1.0/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.432670 hiveviewer-0.1.0/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.1.0/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.434121 hiveviewer-0.1.0/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.1.0/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.434468 hiveviewer-0.1.0/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       64 2023-07-19 09:14:34.000000 hiveviewer-0.1.0/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     4567 2023-07-21 03:20:46.000000 hiveviewer-0.1.0/src/hiveviewer/evaluation/calculate_auc.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.434907 hiveviewer-0.1.0/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-07-19 08:12:07.000000 hiveviewer-0.1.0/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-07-20 10:58:22.000000 hiveviewer-0.1.0/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     5220 2023-07-21 04:19:25.000000 hiveviewer-0.1.0/src/hiveviewer/optimization/profolio_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.435339 hiveviewer-0.1.0/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      106 2023-05-25 06:14:02.000000 hiveviewer-0.1.0/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      667 2023-07-18 12:12:04.000000 hiveviewer-0.1.0/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     2346 2023-07-19 08:03:56.000000 hiveviewer-0.1.0/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.436244 hiveviewer-0.1.0/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.1.0/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-21 04:24:06.433491 hiveviewer-0.1.0/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      971 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       75 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-07-21 04:24:06.000000 hiveviewer-0.1.0/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.241145 hiveviewer-0.1.1/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.1.1/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-31 12:17:30.241032 hiveviewer-0.1.1/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.1.1/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.1.1/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-07-31 12:17:30.241183 hiveviewer-0.1.1/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)      988 2023-07-31 12:17:01.000000 hiveviewer-0.1.1/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.233574 hiveviewer-0.1.1/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.234855 hiveviewer-0.1.1/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.1.1/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.236953 hiveviewer-0.1.1/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.1.1/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.237526 hiveviewer-0.1.1/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.1.1/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     6440 2023-07-31 12:13:52.000000 hiveviewer-0.1.1/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.238275 hiveviewer-0.1.1/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-07-19 08:12:07.000000 hiveviewer-0.1.1/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-07-20 10:58:22.000000 hiveviewer-0.1.1/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     5217 2023-07-28 09:00:29.000000 hiveviewer-0.1.1/src/hiveviewer/optimization/profolio_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.239205 hiveviewer-0.1.1/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.1.1/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.240747 hiveviewer-0.1.1/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.1.1/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:17:30.235699 hiveviewer-0.1.1/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1013 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       75 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-07-31 12:17:30.000000 hiveviewer-0.1.1/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.1.0/LICENSE` & `hiveviewer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/PKG-INFO` & `hiveviewer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.1.0/README.md` & `hiveviewer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/setup.py` & `hiveviewer-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "matplotlib_venn",
         "openpyxl",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.1.0",
+    version="0.1.1",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.1.0/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.1.1/src/hiveviewer/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.1.1/src/hiveviewer/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/dataloader/load_excel.py` & `hiveviewer-0.1.1/src/hiveviewer/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/evaluation/calculate_auc.py` & `hiveviewer-0.1.1/src/hiveviewer/evaluation/calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import roc_auc_score
 from tqdm import tqdm
 
+from ..sampling.frequency_sampler import FrequencySampler
+
 
 class Calculator:
-    """Calculator class for calculating AUC."""
+    """Calculator class for calculating various metrics."""
 
     def __init__(
         self,
         df: pd.DataFrame,
         selected_columns: List[str],
         weights_for_groups: Optional[pd.Series] = None,
     ) -> None:
@@ -80,17 +82,71 @@
             if weights_for_groups is not None:
                 counts_sorted = weights_for_groups.loc[grouped.index]
                 result = float(np.average(grouped, weights=counts_sorted.values))
             else:
                 result = float(np.mean(grouped))
         return result
 
+    def create_score_columns(
+        self, boundary_dict: dict, score_column: str = "score"
+    ) -> None:
+        """Create score columns.
+
+        :param boundary_dict: boundary dict
+        :param score_column: score column to be converted
+        """
+        for k, _ in boundary_dict.items():
+            self.df[f"{score_column}_lt_{k}"] = (self.df[score_column] >= k).astype(int)
+
+    def initialize_fq_sampler(
+        self,
+        sample_size: int,
+        score_column: str,
+        slice_from: Optional[float] = None,
+        slice_to: Optional[float] = None,
+        log_scale: Optional[bool] = True,
+        laplace_smoothing: Optional[bool] = True,
+    ) -> None:
+        """Initialize frequency sampler."""
+        self.sampler = FrequencySampler(
+            sample_size=sample_size,
+            data=self.df[score_column],
+            slice_from=slice_from,
+            slice_to=slice_to,
+            log_scale=log_scale,
+            laplace_smoothing=laplace_smoothing,
+        )
+        self.score_column = score_column
+        self.create_score_columns(
+            boundary_dict=self.sampler.sample(), score_column=score_column
+        )
+
+    def calculate_wouauc(
+        self,
+        weights_for_equation: List,
+    ) -> List[float]:
+        """Calculate weighted ordinal user AUC.
+
+        :param weights_for_equation: weights for equation
+        :param score_column: score column
+        """
+        self.get_overall_score(weights_for_equation)
+        wouauc = []
+        for k, _ in self.sampler.boundary_dict.items():
+            paritial_auc = float(
+                roc_auc_score(
+                    self.df[f"{self.score_column}_lt_{k}"], self.df["overall_score"]
+                )
+            )
+            wouauc.append(paritial_auc)
+        return wouauc
+
     def calculate_portfolio_concentration(
         self, target_column: str, expected_return: Optional[float] = None
-    ) -> tuple[float, float]:
+    ) -> Tuple[float, float]:
         """Calculate portfolio concentration.
 
         :param target_column: target column
         :param expected_return: expected return
         """
         if expected_return is None:
             expected_return = 0.95
@@ -98,15 +154,15 @@
         sum_all = df[target_column].sum()
         df["cumulative_sum"] = df[target_column].cumsum()
         df["cumulative_ratio"] = df["cumulative_sum"] / sum_all
         threshold = df[df["cumulative_ratio"] > expected_return]["overall_score"].max()
         concentration = df[df["overall_score"] > threshold].shape[0] / self.df_len
         return threshold, concentration
 
-    def calculate_auc_triple_parameters(self, grid_interval: int) -> tuple:
+    def calculate_auc_triple_parameters(self, grid_interval: int) -> Tuple:
         """Calculate AUC triple parameters.
 
         :param grid_interval: grid interval
         :return: tuple of W1, W2, WUAUC
         """
         w1_values = np.linspace(0, 1, grid_interval)
         w2_values = np.linspace(0, 1, grid_interval)
```

### Comparing `hiveviewer-0.1.0/src/hiveviewer/optimization/base.py` & `hiveviewer-0.1.1/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/optimization/profolio_objective.py` & `hiveviewer-0.1.1/src/hiveviewer/optimization/profolio_objective.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import List, Literal, Optional
 
 import numpy as np
 import optuna
 from optuna.trial import Trial
 
-from ..evaluation.calculate_auc import Calculator
+from ..evaluation.calculator import Calculator
 from .base import BaseObjective
 
 
 class ProfolioObjective(BaseObjective):
     """
     This class provides methods to optimize the profolio objective.
     """
```

### Comparing `hiveviewer-0.1.0/src/hiveviewer/sampling/base.py` & `hiveviewer-0.1.1/src/hiveviewer/sampling/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 from abc import ABCMeta, abstractmethod
 from typing import List, Optional, Union
 
+import numpy as np
 import pandas as pd
 
 
 class BaseSampler(metaclass=ABCMeta):
     """
     This class provides methods to sample data.
     """
 
     def __init__(
         self,
         sample_size: int,
         data: Union[pd.Series, List[float]],
         slice_from: Optional[float] = None,
         slice_to: Optional[float] = None,
+        log_scale: Optional[bool] = True,
+        laplace_smoothing: Optional[bool] = True,
     ) -> None:
         self.sample_size = sample_size
         self.data = data
         self.slice_from = slice_from
         self.slice_to = slice_to
+        self.log_scale = log_scale
+        self.laplace_smoothing = laplace_smoothing
+        if self.laplace_smoothing:
+            self.data = [x + 1 for x in self.data]
+        if self.log_scale:
+            self.data = [np.log(x) for x in self.data]
+        self.boundary_dict = self.sample()
 
     @abstractmethod
-    def sample(self) -> List[float]:
+    def sample(self) -> dict:
         raise NotImplementedError("Should implement sample()!")
```

### Comparing `hiveviewer-0.1.0/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.1.1/src/hiveviewer/sampling/gini_sampler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from ..visualization.lorenz_curve import LorenzCurveGini
 from .base import BaseSampler
@@ -14,27 +15,31 @@
 
     def __init__(
         self,
         sample_size: int,
         data: Union[pd.Series, List[float]],
         slice_from: Optional[float] = None,
         slice_to: Optional[float] = None,
+        log_scale: Optional[bool] = True,
+        laplace_smoothing: Optional[bool] = True,
         bounds_num: Optional[int] = None,
     ) -> None:
         """
         Initialize with a list of data.
 
         :param sample_size: number of samples
         :param data: a list of floats
         :param slice_from: lower bound of the data
         :param slice_to: upper bound of the data
         :param bounds_num: number of bounds
         :return: a list of floats
         """
-        super().__init__(sample_size, data, slice_from, slice_to)
+        super().__init__(
+            sample_size, data, slice_from, slice_to, log_scale, laplace_smoothing
+        )
         self.lorenz_gini = LorenzCurveGini(self.data)
         if bounds_num is None:
             self.bounds_num = self.sample_size * 10
         else:
             self.bounds_num = bounds_num
         self.bounds = self.lorenz_gini.get_bounds(
             num_quantiles=self.bounds_num,
@@ -61,16 +66,15 @@
             segment_indices.append(segment_idx)
             start_idx = segment_idx
 
         segment_bounds = [self.bounds[i] for i in segment_indices]
 
         return segment_bounds
 
-    def sample(self) -> List[float]:
+    def sample(self) -> dict:
         """
         Sample data according to Gini coefficient.
         """
 
         gini_list = self.lorenz_gini.get_gini_list_from_bounds(self.bounds)
         segment_bounds = self.equidistant_indices(gini_list)
-
-        return sorted(list(set(segment_bounds)))
+        return dict(Counter(segment_bounds))
```

### Comparing `hiveviewer-0.1.0/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.1.1/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.1.1/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.1.1/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.1.1/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.1.1/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.0/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.1.1/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.1.0/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.1.1/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 src/hiveviewer.egg-info/requires.txt
 src/hiveviewer.egg-info/top_level.txt
 src/hiveviewer/dataloader/__init__.py
 src/hiveviewer/dataloader/base.py
 src/hiveviewer/dataloader/load_csv.py
 src/hiveviewer/dataloader/load_excel.py
 src/hiveviewer/evaluation/__init__.py
-src/hiveviewer/evaluation/calculate_auc.py
+src/hiveviewer/evaluation/calculator.py
 src/hiveviewer/optimization/__init__.py
 src/hiveviewer/optimization/base.py
 src/hiveviewer/optimization/profolio_objective.py
 src/hiveviewer/sampling/__init__.py
 src/hiveviewer/sampling/base.py
+src/hiveviewer/sampling/frequency_sampler.py
 src/hiveviewer/sampling/gini_sampler.py
 src/hiveviewer/visualization/__init__.py
 src/hiveviewer/visualization/lorenz_curve.py
 src/hiveviewer/visualization/plot_trisurf.py
 src/hiveviewer/visualization/venn2.py
 src/hiveviewer/visualization/venn3.py
 src/hiveviewer/visualization/venn_base.py
```

