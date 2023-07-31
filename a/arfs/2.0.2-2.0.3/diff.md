# Comparing `tmp/arfs-2.0.2.tar.gz` & `tmp/arfs-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-2.0.2.tar", last modified: Mon Jul 31 10:42:15 2023, max compression
+gzip compressed data, was "arfs-2.0.3.tar", last modified: Mon Jul 31 14:01:48 2023, max compression
```

## Comparing `arfs-2.0.2.tar` & `arfs-2.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.193393 arfs-2.0.2/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.2/LICENSE.md
--rw-rw-rw-   0        0        0    11967 2023-07-31 10:42:15.194393 arfs-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11277 2023-07-29 14:45:54.000000 arfs-2.0.2/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1611 2023-07-31 10:42:15.203395 arfs-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.709393 arfs-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.894397 arfs-2.0.2/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-07-31 10:33:14.000000 arfs-2.0.2/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    87074 2023-07-29 17:00:56.000000 arfs-2.0.2/src/arfs/association.py
--rw-rw-rw-   0        0        0     6689 2023-07-24 20:31:43.000000 arfs-2.0.2/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.712393 arfs-2.0.2/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.001395 arfs-2.0.2/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.2/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.2/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.148393 arfs-2.0.2/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.2/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    96187 2023-07-29 17:00:56.000000 arfs-2.0.2/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-2.0.2/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    21314 2023-07-31 10:40:40.000000 arfs-2.0.2/src/arfs/feature_selection/lasso.py
--rw-rw-rw-   0        0        0    13385 2023-07-29 17:00:51.000000 arfs-2.0.2/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2457 2023-05-21 19:11:19.000000 arfs-2.0.2/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15864 2023-07-29 17:00:51.000000 arfs-2.0.2/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    15806 2023-07-29 17:00:51.000000 arfs-2.0.2/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21927 2023-06-16 08:19:41.000000 arfs-2.0.2/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-2.0.2/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    40517 2023-07-29 17:00:53.000000 arfs-2.0.2/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-2.0.2/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    25367 2023-07-29 17:00:53.000000 arfs-2.0.2/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:14.978395 arfs-2.0.2/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11967 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.2/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      573 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-31 10:42:14.000000 arfs-2.0.2/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 10:42:15.179392 arfs-2.0.2/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.2/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.2/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.184867 arfs-2.0.3/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0    11944 2023-07-31 14:01:48.185867 arfs-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11254 2023-07-31 13:58:34.000000 arfs-2.0.3/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1611 2023-07-31 14:01:48.195866 arfs-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.613867 arfs-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.872867 arfs-2.0.3/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-07-31 13:56:58.000000 arfs-2.0.3/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    87125 2023-07-31 13:46:30.000000 arfs-2.0.3/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6829 2023-07-31 13:45:23.000000 arfs-2.0.3/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.624868 arfs-2.0.3/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.011866 arfs-2.0.3/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.3/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.3/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.146866 arfs-2.0.3/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.3/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    96187 2023-07-29 17:00:56.000000 arfs-2.0.3/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5398 2023-07-31 13:36:41.000000 arfs-2.0.3/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    22592 2023-07-31 13:36:55.000000 arfs-2.0.3/src/arfs/feature_selection/lasso.py
+-rw-rw-rw-   0        0        0    13812 2023-07-31 13:37:06.000000 arfs-2.0.3/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2473 2023-07-31 13:38:21.000000 arfs-2.0.3/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    16052 2023-07-31 13:40:30.000000 arfs-2.0.3/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    15889 2023-07-31 13:42:08.000000 arfs-2.0.3/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21997 2023-07-31 13:49:08.000000 arfs-2.0.3/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5788 2023-07-31 13:49:56.000000 arfs-2.0.3/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    38641 2023-07-31 13:53:12.000000 arfs-2.0.3/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15511 2023-07-31 13:53:23.000000 arfs-2.0.3/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    25361 2023-07-31 13:53:40.000000 arfs-2.0.3/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.987883 arfs-2.0.3/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11944 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.3/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      573 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.173865 arfs-2.0.3/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.3/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.3/tests/test_featselect.py
```

### Comparing `arfs-2.0.2/LICENSE.md` & `arfs-2.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/PKG-INFO` & `arfs-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.2
+Version: 2.0.3
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
@@ -34,15 +34,15 @@
 
 Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
 
 Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
-`$ pip install arfs`, requires python <3.10
+`$ pip install arfs`
 
 ## Example
 
 Working examples for:
 
  - [Preprocessing](./docs/notebooks/preprocessingipynb)
  - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
```

### Comparing `arfs-2.0.2/README.md` & `arfs-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
 
 Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
-`$ pip install arfs`, requires python <3.10
+`$ pip install arfs`
 
 ## Example
 
 Working examples for:
 
  - [Preprocessing](./docs/notebooks/preprocessingipynb)
  - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
```

### Comparing `arfs-2.0.2/setup.cfg` & `arfs-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/src/arfs/association.py` & `arfs-2.0.3/src/arfs/association.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+""" Parallelized Association and Correlation matrix
+ 
 This module provides parallelized methods for computing associations.
 Namely, correlation, correlation ratio, Theil's U, Cramer's V
 
 They are the basis of the MRmr feature selection
 """
 
 import math
```

### Comparing `arfs-2.0.2/src/arfs/benchmark.py` & `arfs-2.0.3/src/arfs/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-"""
-This module provides utilities for comparing and benchmarking feature selection methods
+"""Benchmark Feature Selection
 
-**The module structure is the following:**
+This module provides utilities for comparing and benchmarking feature selection methods
 
-- The ``sklearn_pimp_bench`` function for comparing using the sklearn permutation importance
-- The ``compare_varimp`` function for comparing using 3 kinds of var.imp.
+Module Structure:
+-----------------
+- ``sklearn_pimp_bench``: function for comparing using the sklearn permutation importance
+- ``compare_varimp``: function for comparing using 3 kinds of var.imp.
+- ``highlight_tick``: function for highlighting specific (genuine or noise for instance) predictors in the importance chart
 """
 
 from __future__ import print_function, division
 
 import itertools
 from matplotlib import pyplot as plt
 from sklearn.model_selection import train_test_split
```

### Comparing `arfs-2.0.2/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.0.3/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/src/arfs/dataset/data/housing.zip` & `arfs-2.0.3/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/src/arfs/feature_selection/__init__.py` & `arfs-2.0.3/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/src/arfs/feature_selection/allrelevant.py` & `arfs-2.0.3/src/arfs/feature_selection/allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/src/arfs/feature_selection/base.py` & `arfs-2.0.3/src/arfs/feature_selection/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""
-This module provides a base class for selector using a statistic and a threshold
+"""Base Submodule
 
-**The module structure is the following:**
+This module provides a base class for selector using a statistic and a threshold
 
-- The ``BaseThresholdSelector`` parent class for the "treshold-based" selectors
+Module Structure:
+-----------------
+- ``BaseThresholdSelector``: parent class for the "treshold-based" selectors
 
 """
 
 # Settings and libraries
 from __future__ import print_function
 
 # pandas
```

### Comparing `arfs-2.0.2/src/arfs/feature_selection/lasso.py` & `arfs-2.0.3/src/arfs/feature_selection/lasso.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,36 @@
+"""LassoFeatureSelection Submodule
+
+This module provides LASSO-based feature selection, specifically designed for use with Generalized Linear Models (GLM). 
+The Lasso Regularized GLM introduces an L1 regularization penalty (Lasso regularization), 
+encouraging some coefficients to become exactly zero during the model fitting process. 
+This regularization effectively removes irrelevant features from the model, making it a 
+powerful tool for feature selection, particularly in datasets with numerous variables.
+
+Module Structure:
+-----------------
+- `EnetGLM`: class serves as a scikit-learn wrapper for the regularized statsmodels GLM, providing seamless integration with scikit-learn's ecosystem.
+- `weighted_cross_val_score`: function allows users to pass weights to the model and define a custom scoring metric.
+- `grid_search_cv`: function performs a weighted LASSO grid search to find the best Lasso parameter for the model.
+- `LassoFeatureSelection`: class is the core feature selection class, estimating the Lasso parameter through 
+    the grid search process, enabling efficient and effective feature selection.
+
+With this submodule, users can easily leverage Lasso Regularized GLMs and conduct feature selection, 
+improving model performance and interpretability in various datasets.
+"""
+
 import pandas as pd
 import numpy as np
 import statsmodels.api as sm
 from sklearn.base import BaseEstimator, TransformerMixin, RegressorMixin
 from sklearn.base import clone
 from sklearn.utils import check_array
 from sklearn.model_selection import StratifiedKFold, KFold
 from joblib import Parallel, delayed
-from typing import Any, Callable, Union, List, Tuple, Optional, Dict, Literal
+from typing import Union, Optional
 
 
 def _map_family_link(family: str = "gaussian", link: Optional[str] = None):
     family_mapping = {
         "gaussian": sm.families.Gaussian,
         "binomial": sm.families.Binomial,
         "poisson": sm.families.Poisson,
```

### Comparing `arfs-2.0.2/src/arfs/feature_selection/mrmr.py` & `arfs-2.0.3/src/arfs/feature_selection/mrmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-"""
-This module provides a class for the Maximal Relevance, minimal redundancy feature selection
-
-**The module structure is the following:**
+"""MRMR Feature Selection Module
 
-- The ``MinRedundancyMaxRelevance`` parent class for the "treshold-based" selectors
+This module provides MinRedundancyMaxRelevance (MRMR) feature selection for classification or regression tasks. 
+In a classification task, the target should be of object or pandas category dtype, while in a regression task, 
+the target should be of numpy categorical dtype. The predictors can be categorical or numerical without requiring encoding, 
+as the appropriate method (correlation, correlation ratio, or Theil's U) will be automatically selected based on the data type.
 
+Module Structure:
+-----------------
+- ``MinRedundancyMaxRelevance``: MRMR feature selection class for classification or regression tasks.
 """
 
 import functools
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_is_fitted
```

### Comparing `arfs-2.0.2/src/arfs/feature_selection/summary.py` & `arfs-2.0.3/src/arfs/feature_selection/summary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""
-This module provides a function for creating the summary report of a FS pipeline
+"""Feature Selection Summary Module
 
-**The module structure is the following:**
-
-- The ``make_fs_summary`` main function for creating the summary
-- The ``highlight_discarded`` function for creating style for the pd.DataFrame
+This module provides a function for creating the summary report of a FS pipeline
 
+Module Structure:
+-----------------
+- ``make_fs_summary`` main function for creating the summary
+- ``highlight_discarded`` function for creating style for the pd.DataFrame
 """
 
 import pandas as pd
 import numpy as np
 
 
 def highlight_discarded(s):
```

### Comparing `arfs-2.0.2/src/arfs/feature_selection/unsupervised.py` & `arfs-2.0.3/src/arfs/feature_selection/unsupervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""
-This module provides selectors using unsupervised statistics and a threshold
+"""Unsupervised Feature Selection
 
-**The module structure is the following:**
+This module provides selectors using unsupervised statistics and a threshold
 
-- The ``MissingValueThreshold`` child of the ``BaseThresholdSelector``
-- The ``UniqueValuesThreshold`` child of the ``BaseThresholdSelector``
-- The ``CardinalityThreshold`` child of the ``BaseThresholdSelector``
-- The ``CollinearityThreshold`` child of the ``BaseThresholdSelector``
+Module Structure:
+-----------------
+- ``MissingValueThreshold``: child class of the ``BaseThresholdSelector``, filter out columns with too many missing values
+- ``UniqueValuesThreshold`` child of the ``BaseThresholdSelector``, filter out columns with zero variance
+- ``CardinalityThreshold`` child of the ``BaseThresholdSelector``, filter out categorical columns with too many levels  
+- ``CollinearityThreshold`` child of the ``BaseThresholdSelector``, filter out collinear columns
 """
 
 from __future__ import print_function
 from tqdm.auto import trange
 
 # pandas
 import pandas as pd
```

### Comparing `arfs-2.0.2/src/arfs/feature_selection/variable_importance.py` & `arfs-2.0.3/src/arfs/feature_selection/variable_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""
-This module provides selectors using supervised statistics and a threshold
-
-**The module structure is the following:**
+"""Supervised Feature Selection
 
-- The ``VariableImportance`` main class for identifying non-important features
+This module provides selectors using supervised statistics and a threshold, using SHAP, permutation importance or impurity (Gini) importance.
 
+Module Structure:
+-----------------
+- ``VariableImportance`` main class for identifying non-important features
 """
 
 from __future__ import print_function
 from tqdm.auto import trange
 
 # pandas
 import pandas as pd
```

### Comparing `arfs-2.0.2/src/arfs/gbm.py` & `arfs-2.0.3/src/arfs/gbm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-"""
-This module provides a class to train a base lightgbm and catboost models using early stopping as default.
-The target can be finite discrete (classification) or continuous (regression).
-It can boost from an initial score (aka baseline for catboost), take sample weight as input.
+"""GBM Wrapper
 
-**The module structure is the following:**
+This module offers a class to train base LightGBM and CatBoost models, with early stopping as the default behavior. 
+The target variable can be finite discrete (classification) or continuous (regression). 
+Additionally, the model allows boosting from an initial score (also known as a baseline for CatBoost) and accepts sample weights as input.
 
-- The ``GradientBoosting`` main class to train a lightGBM  or catboost with early stopping
+Module Structure:
+-----------------
+- ``GradientBoosting``: main class to train a lightGBM  or catboost with early stopping
 
 """
+
 from sklearn.model_selection import (
     ShuffleSplit,
     StratifiedShuffleSplit,
     GroupShuffleSplit,
 )
 import lightgbm as lgb
 from lightgbm import early_stopping, log_evaluation, record_evaluation
```

### Comparing `arfs-2.0.2/src/arfs/parallel.py` & `arfs-2.0.3/src/arfs/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""
-This module provides utilities for parallelizing operations on pd.DataFrame
+"""Parallelize Pandas
 
-**The module structure is the following:**
+This module provides utilities for parallelizing operations on pd.DataFrame
 
-- The ``parallel_matrix_entries`` for parallelizing operations returning a matrix (2D) (apply on pairs of columns)
-- The ``parallel_df`` for parallelizing operations returning a series (1D) (apply on a single column at a time)
+Module Structure:
+-----------------
+- ``parallel_matrix_entries`` for parallelizing operations returning a matrix (2D) (apply on pairs of columns)
+- ``parallel_df`` for parallelizing operations returning a series (1D) (apply on a single column at a time)
 """
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 from multiprocessing import cpu_count
 from itertools import chain
```

### Comparing `arfs-2.0.2/src/arfs/preprocessing.py` & `arfs-2.0.3/src/arfs/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 This module provides preprocessing classes
 
-**The module structure is the following:**
-
-- The ``OrdinalEncoderPandas`` main class for ordinal encoding, takes in a DF and returns a DF of the same shape
-- The ``dtype_column_selector`` for standardizing selection of columns based on their dtypes
-- The ``TreeDiscretizer`` for discretizing continuous columns and auto-group levels of categorical columns
-
+Module Structure:
+-----------------
+- ``OrdinalEncoderPandas``: main class for ordinal encoding, takes in a DF and returns a DF of the same shape
+- ``dtype_column_selector``: for standardizing selection of columns based on their dtypes
+- ``TreeDiscretizer``: class for discretizing continuous columns and auto-group levels of categorical columns
+- ``IntervalToMidpoint``: class for converting pandas numerical intervals into their float midpoint
+- ``PatsyTransformer``: class for encoding data for (generalized) linear models, leveraging Patsy
 """
 
 # Settings and libraries
 from __future__ import print_function
 from tqdm.auto import tqdm
 
 # pandas
@@ -37,21 +38,14 @@
 from .gbm import GradientBoosting
 from .utils import create_dtype_dict
 
 
 # fix random seed for reproducibility
 np.random.seed(7)
 
-__all__ = [
-    "OrdinalEncoderPandas",
-    "dtype_column_selector",
-    "TreeDiscretizer",
-]
-
-
 class OrdinalEncoderPandas(OrdinalEncoder):
     # class OrdinalEncoderPandas(BaseEstimator, TransformerMixin):
     """Encode categorical features as an integer array and returns a pandas DF.
     The features are converted to ordinal integers. This results in
     a single column of integers (0 to n_categories - 1) per feature.
     Read more in the scikit-learn OrdinalEncoder documentation
 
@@ -709,61 +703,14 @@
     """
     is_X = s == 0
     return [
         "background-color: #d65f5f" if v else "background-color: #33a654" for v in is_X
     ]
 
 
-def make_fs_summary(selector_pipe):
-    """make_fs_summary makes a summary dataframe highlighting at which step a
-    given predictor has been rejected (if any).
-
-    Parameters
-    ----------
-    selector_pipe : sklearn.pipeline.Pipeline
-        the feature selector pipeline.
-
-    Examples
-    --------
-    >>> groot_pipeline = Pipeline([
-    ... ('missing', MissingValueThreshold()),
-    ... ('unique', UniqueValuesThreshold()),
-    ... ('cardinality', CardinalityThreshold()),
-    ... ('collinearity', CollinearityThreshold(threshold=0.5)),
-    ... ('lowimp', VariableImportance(eval_metric='poisson', objective='poisson', verbose=2)),
-    ... ('grootcv', GrootCV(objective='poisson', cutoff=1, n_folds=3, n_iter=5))])
-    >>> groot_pipeline.fit_transform(
-        X=df[predictors],
-        y=df[target],
-        lowimp__sample_weight=df[weight],
-        grootcv__sample_weight=df[weight])
-    >>> fs_summary_df = make_fs_summary(groot_pipeline)
-    """
-
-    tag_df = pd.DataFrame({"predictor": selector_pipe[0].feature_names_in_})
-    for selector_name in selector_pipe.named_steps.keys():
-        if hasattr(selector_pipe.named_steps[selector_name], "feature_names_in_"):
-            feature_in = selector_pipe.named_steps[selector_name].feature_names_in_
-            to_drop = list(
-                set(selector_pipe.named_steps[selector_name].feature_names_in_)
-                - set(selector_pipe.named_steps[selector_name].get_feature_names_out())
-            )
-            tag_df[selector_name] = np.where(
-                tag_df["predictor"].isin(to_drop), 0, 1
-            ) * np.where(tag_df["predictor"].isin(feature_in), 1, np.nan)
-
-    col_to_apply_style = tag_df.columns[1:]
-    tag_df = (
-        tag_df.style.apply(highlight_discarded, subset=col_to_apply_style)
-        .applymap(lambda x: "" if x == x else "background-color: #ffa500")
-        .format(precision=0)
-    )
-    return tag_df
-
-
 class IntervalToMidpoint(BaseEstimator, TransformerMixin):
     """
     IntervalToMidpoint is a transformer that converts numerical intervals in a pandas DataFrame to their midpoints.
 
     Parameters
     ----------
     cols : list of str or str, default "all"
```

### Comparing `arfs-2.0.2/src/arfs/sampling.py` & `arfs-2.0.3/src/arfs/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """This module provide methods for sampling large datasets for reducing the running time
-    
 """
 import numpy as np
 import pandas as pd
 from scipy.sparse import issparse
 from collections import Counter
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.ensemble import IsolationForest
```

### Comparing `arfs-2.0.2/src/arfs/utils.py` & `arfs-2.0.3/src/arfs/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Utility and validation functions
-  
+"""Utility and validation functions
 """
 
 from __future__ import print_function, division
 
 import lightgbm as lgb
 import matplotlib as mpl
 import numpy as np
```

### Comparing `arfs-2.0.2/src/arfs.egg-info/PKG-INFO` & `arfs-2.0.3/src/arfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.2
+Version: 2.0.3
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
@@ -34,15 +34,15 @@
 
 Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
 
 Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
 
 ## Installation
 
-`$ pip install arfs`, requires python <3.10
+`$ pip install arfs`
 
 ## Example
 
 Working examples for:
 
  - [Preprocessing](./docs/notebooks/preprocessingipynb)
  - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
```

### Comparing `arfs-2.0.2/src/arfs.egg-info/SOURCES.txt` & `arfs-2.0.3/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/src/arfs.egg-info/requires.txt` & `arfs-2.0.3/src/arfs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/tests/test_allrelevant.py` & `arfs-2.0.3/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.2/tests/test_featselect.py` & `arfs-2.0.3/tests/test_featselect.py`

 * *Files identical despite different names*

