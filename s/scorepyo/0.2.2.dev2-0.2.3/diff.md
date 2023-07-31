# Comparing `tmp/scorepyo-0.2.2.dev2.tar.gz` & `tmp/scorepyo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorepyo-0.2.2.dev2.tar", last modified: Tue Mar 21 14:08:29 2023, max compression
+gzip compressed data, was "scorepyo-0.2.3.tar", last modified: Mon Jul 31 12:39:59 2023, max compression
```

## Comparing `scorepyo-0.2.2.dev2.tar` & `scorepyo-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 14:08:29.871120 scorepyo-0.2.2.dev2/
--rw-rw-rw-   0        0        0     1083 2022-11-21 10:46:32.000000 scorepyo-0.2.2.dev2/LICENSE
--rw-rw-rw-   0        0        0       82 2022-12-06 23:13:52.000000 scorepyo-0.2.2.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0      668 2023-03-21 14:08:29.872118 scorepyo-0.2.2.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     7941 2023-03-16 21:20:46.000000 scorepyo-0.2.2.dev2/README.md
--rw-rw-rw-   0        0        0    14531 2023-03-11 19:24:09.000000 scorepyo-0.2.2.dev2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-21 14:08:29.822367 scorepyo-0.2.2.dev2/scorepyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 15:22:58.000000 scorepyo-0.2.2.dev2/scorepyo/__init__.py
--rw-rw-rw-   0        0        0     2759 2023-03-16 21:20:46.000000 scorepyo-0.2.2.dev2/scorepyo/_utils.py
--rw-rw-rw-   0        0        0    23361 2023-03-16 21:20:46.000000 scorepyo-0.2.2.dev2/scorepyo/binarizers.py
--rw-rw-rw-   0        0        0    12011 2023-03-20 22:17:09.000000 scorepyo-0.2.2.dev2/scorepyo/calibration.py
--rw-rw-rw-   0        0        0     2015 2023-03-20 22:17:09.000000 scorepyo-0.2.2.dev2/scorepyo/exceptions.py
--rw-rw-rw-   0        0        0    29092 2023-03-21 13:25:08.000000 scorepyo-0.2.2.dev2/scorepyo/models.py
--rw-rw-rw-   0        0        0    25775 2023-03-20 22:17:09.000000 scorepyo-0.2.2.dev2/scorepyo/ranking.py
-drwxrwxrwx   0        0        0        0 2023-03-21 14:08:29.842198 scorepyo-0.2.2.dev2/scorepyo.egg-info/
--rw-rw-rw-   0        0        0      668 2023-03-21 14:08:29.000000 scorepyo-0.2.2.dev2/scorepyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-03-21 14:08:29.000000 scorepyo-0.2.2.dev2/scorepyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 14:08:29.000000 scorepyo-0.2.2.dev2/scorepyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-21 11:11:44.000000 scorepyo-0.2.2.dev2/scorepyo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      530 2023-03-21 14:08:29.000000 scorepyo-0.2.2.dev2/scorepyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-21 14:08:29.000000 scorepyo-0.2.2.dev2/scorepyo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1419 2023-03-21 14:08:29.876108 scorepyo-0.2.2.dev2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-21 14:08:29.865139 scorepyo-0.2.2.dev2/tests/
--rw-rw-rw-   0        0        0     1655 2022-11-29 16:03:50.000000 scorepyo-0.2.2.dev2/tests/conftest.py
--rw-rw-rw-   0        0        0     4902 2023-03-11 19:24:09.000000 scorepyo-0.2.2.dev2/tests/test_binarizer.py
--rw-rw-rw-   0        0        0     2362 2023-03-16 21:20:46.000000 scorepyo-0.2.2.dev2/tests/test_models.py
--rw-rw-rw-   0        0        0     1994 2023-03-16 21:20:46.000000 scorepyo-0.2.2.dev2/tests/test_scorepyo.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:39:59.284539 scorepyo-0.2.3/
+-rw-rw-rw-   0        0        0     1083 2022-11-21 10:46:32.000000 scorepyo-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       82 2023-04-08 18:41:22.000000 scorepyo-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      663 2023-07-31 12:39:59.284539 scorepyo-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    14531 2023-03-11 19:24:09.000000 scorepyo-0.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-31 12:39:59.232679 scorepyo-0.2.3/scorepyo/
+-rw-rw-rw-   0        0        0        0 2023-04-08 18:41:22.000000 scorepyo-0.2.3/scorepyo/__init__.py
+-rw-rw-rw-   0        0        0     2759 2023-04-08 18:41:22.000000 scorepyo-0.2.3/scorepyo/_utils.py
+-rw-rw-rw-   0        0        0    23482 2023-07-31 12:24:52.000000 scorepyo-0.2.3/scorepyo/binarizers.py
+-rw-rw-rw-   0        0        0    12011 2023-04-08 18:41:22.000000 scorepyo-0.2.3/scorepyo/calibration.py
+-rw-rw-rw-   0        0        0     2015 2023-04-08 18:41:22.000000 scorepyo-0.2.3/scorepyo/exceptions.py
+-rw-rw-rw-   0        0        0    29092 2023-04-08 18:41:22.000000 scorepyo-0.2.3/scorepyo/models.py
+-rw-rw-rw-   0        0        0    28277 2023-07-31 12:24:52.000000 scorepyo-0.2.3/scorepyo/ranking.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:39:59.260632 scorepyo-0.2.3/scorepyo.egg-info/
+-rw-rw-rw-   0        0        0      663 2023-07-31 12:39:58.000000 scorepyo-0.2.3/scorepyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-31 12:39:59.000000 scorepyo-0.2.3/scorepyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:39:58.000000 scorepyo-0.2.3/scorepyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 08:38:57.000000 scorepyo-0.2.3/scorepyo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      552 2023-07-31 12:39:58.000000 scorepyo-0.2.3/scorepyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 12:39:58.000000 scorepyo-0.2.3/scorepyo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1443 2023-07-31 12:39:59.287536 scorepyo-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 12:39:59.279554 scorepyo-0.2.3/tests/
+-rw-rw-rw-   0        0        0     1655 2023-04-08 18:41:22.000000 scorepyo-0.2.3/tests/conftest.py
+-rw-rw-rw-   0        0        0     4902 2023-04-08 18:41:22.000000 scorepyo-0.2.3/tests/test_binarizer.py
+-rw-rw-rw-   0        0        0     2362 2023-04-08 18:41:22.000000 scorepyo-0.2.3/tests/test_models.py
+-rw-rw-rw-   0        0        0     2053 2023-07-31 12:24:52.000000 scorepyo-0.2.3/tests/test_scorepyo.py
```

### Comparing `scorepyo-0.2.2.dev2/LICENSE` & `scorepyo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/PKG-INFO` & `scorepyo-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorepyo
-Version: 0.2.2.dev2
+Version: 0.2.3
 Summary: This is the scorepyo repository.
 Home-page: https://github.com/drskd/scorepyo
 Author: S. Kaddani
 License: MIT
 Keywords: scorepyo risk score
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scorepyo-0.2.2.dev2/pyproject.toml` & `scorepyo-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/scorepyo/_utils.py` & `scorepyo-0.2.3/scorepyo/_utils.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/scorepyo/binarizers.py` & `scorepyo-0.2.3/scorepyo/binarizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -550,11 +550,14 @@
                     "To retain the old behavior, use either.*"
                 ),
             )
             X_binarized.loc[:, list_binary_feature_names] = X_binarized.loc[
                 :, list_binary_feature_names
             ].astype(int)
 
+            # Set the index of the transformed dataframe with original index
+            X_binarized.index = X.index
+
             return X_binarized
 
     def get_info(self) -> pd.DataFrame:
         return self.df_score_feature
```

### Comparing `scorepyo-0.2.2.dev2/scorepyo/calibration.py` & `scorepyo-0.2.3/scorepyo/calibration.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/scorepyo/exceptions.py` & `scorepyo-0.2.3/scorepyo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/scorepyo/models.py` & `scorepyo-0.2.3/scorepyo/models.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/scorepyo/ranking.py` & `scorepyo-0.2.3/scorepyo/ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import ABC, abstractmethod
 from typing import Any, List
 
 import numpy as np
 import pandas as pd
 import pandera as pa
 from fasterrisk.fasterrisk import RiskScoreOptimizer
+from mrmr import mrmr_classif
 from sklearn.linear_model import OrthogonalMatchingPursuit, lars_path, lasso_path
 
 
 class Ranker(ABC):
     """Base class for binary features ranker
 
     Child classes must implement the _compute_ranking_features method.
@@ -56,15 +57,14 @@
 
     def __init__(self, **kwargs):  # pylint: disable=W0613
         ...
 
     def _compute_ranking_features(
         self, df: pd.DataFrame, *args: Any, **kwargs: Any
     ) -> pd.Series:  # pylint disable=W0613
-
         """
         This method ranks the binary features based on the product of :
          - logodds contribution of the binary feature
          - reduced importance of density
 
         This prevents having a too large emphasis on a binary feature with a large density and low log odd contribution
         Args:
@@ -678,7 +678,74 @@
             by=["fasterrisk_chosen_features", "log_odds_sum"], ascending=[False, False]
         )
         df_["rank"] = list(range(len(df_)))
         df_["rank"] = df_["rank"] + 1
 
         index_without_intercept = [c for c in df_.index if c != "intercept"]
         return df_.loc[index_without_intercept, "rank"].astype(int)
+
+
+class MRMRRank(Ranker):
+    """Binary feature ranker based on mRMR.
+
+    From https://github.com/smazzanti/mrmr:
+    " mRMR, which stands for "minimum Redundancy - Maximum Relevance", is a feature selection algorithm.
+    The peculiarity of mRMR is that it is a minimal-optimal feature selection algorithm.
+    This means it is designed to find the smallest relevant subset of features for a given Machine Learning task."
+
+    Based on this, the ranker selects the binary features selected by the mRMR algorithm where the number of non zero coefficients is equal to the specified target.
+
+    Child class of Ranker.
+    """
+
+    def __init__(self, **kwargs):  # pylint: disable=W0613
+        ...
+
+    def _compute_ranking_features(
+        self,
+        df: pd.DataFrame,
+        X_binarized: pd.DataFrame,
+        y: pd.Series,
+        nb_steps: int,
+        **kwargs,
+    ) -> pd.Series:
+        """This function returns binary features rank based on OMP
+
+        Args:
+            df (pd.DataFrame): Information dataframe on logodds, density and binary feature name
+            X_binarized (pd.DataFrame): Binary features
+            y (pd.Series): Binary target
+            nb_steps (int): Number of features to select
+
+        Returns:
+            pd.Series: Rank for each binary feature in a decreasing order of importance
+        """
+        dataframe_schema = pa.DataFrameSchema(
+            {
+                "log_odds": pa.Column(nullable=True),
+                "density": pa.Column(nullable=True),
+            },
+            index=pa.Index(str, name="binary_feature"),
+            strict=False,  # disable check of other columns in the dataframe
+        )
+
+        dataframe_schema.validate(df)
+
+        df_ = df.copy()
+        df_["log_odds_sum"] = df_["log_odds"].abs() * df_["density"].fillna(0)
+
+        mrmr_selected_features = mrmr_classif(
+            X=X_binarized, y=y, K=nb_steps, show_progress=False
+        )
+
+        df_["mrmr_selected_features"] = np.where(
+            df_.index.isin(mrmr_selected_features), 1, 0
+        )
+
+        df_ = df_.sort_values(
+            by=["mrmr_selected_features", "log_odds_sum"], ascending=[False, False]
+        )
+        df_["rank"] = list(range(len(df_)))
+        df_["rank"] = df_["rank"] + 1
+
+        index_without_intercept = [c for c in df_.index if c != "intercept"]
+        return df_.loc[index_without_intercept, "rank"].astype(int)
```

### Comparing `scorepyo-0.2.2.dev2/scorepyo.egg-info/PKG-INFO` & `scorepyo-0.2.3/scorepyo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorepyo
-Version: 0.2.2.dev2
+Version: 0.2.3
 Summary: This is the scorepyo repository.
 Home-page: https://github.com/drskd/scorepyo
 Author: S. Kaddani
 License: MIT
 Keywords: scorepyo risk score
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scorepyo-0.2.2.dev2/scorepyo.egg-info/requires.txt` & `scorepyo-0.2.3/scorepyo.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 optuna==3.0.3
 botorch==0.7.3
 tabulate==0.9.0
 cvxpy==1.3.0
 dask[distributed]==2023.1.1
 bokeh<3,>=2.4.2
 fasterrisk==0.1.2
+mrmr-selection==0.2.8
 
 [dev]
 black[jupyter]==22.3.0
 isort==5.10.1
 pytest==7.1.2
 pytest-cov==3.0.0
 pylint==2.13.8
```

### Comparing `scorepyo-0.2.2.dev2/setup.cfg` & `scorepyo-0.2.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 636f 7265 7079 6f0d 0a61 7574   = scorepyo..aut
 00000020: 686f 7220 3d20 532e 204b 6164 6461 6e69  hor = S. Kaddani
 00000030: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000040: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000040: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000050: 2054 6869 7320 6973 2074 6865 2073 636f   This is the sco
 00000060: 7265 7079 6f20 7265 706f 7369 746f 7279  repyo repository
 00000070: 2e0d 0a6c 6f6e 675f 6465 7363 7269 7074  ...long_descript
 00000080: 696f 6e20 3d20 5363 6f72 6570 796f 2069  ion = Scorepyo i
 00000090: 7320 6120 7079 7468 6f6e 2070 6163 6b61  s a python packa
 000000a0: 6765 2066 6f72 2063 7265 6174 696e 6720  ge for creating 
 000000b0: 7269 736b 2d73 636f 7265 2074 7970 6520  risk-score type 
@@ -50,40 +50,42 @@
 00000310: 0962 6f74 6f72 6368 3d3d 302e 372e 330d  .botorch==0.7.3.
 00000320: 0a09 7461 6275 6c61 7465 3d3d 302e 392e  ..tabulate==0.9.
 00000330: 300d 0a09 6376 7870 793d 3d31 2e33 2e30  0...cvxpy==1.3.0
 00000340: 0d0a 0964 6173 6b5b 6469 7374 7269 6275  ...dask[distribu
 00000350: 7465 645d 3d3d 3230 3233 2e31 2e31 0d0a  ted]==2023.1.1..
 00000360: 0962 6f6b 6568 3e3d 322e 342e 322c 3c33  .bokeh>=2.4.2,<3
 00000370: 0d0a 0966 6173 7465 7272 6973 6b3d 3d30  ...fasterrisk==0
-00000380: 2e31 2e32 0d0a 0d0a 5b6f 7074 696f 6e73  .1.2....[options
-00000390: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-000003a0: 0d0a 6465 7620 3d20 0d0a 0962 6c61 636b  ..dev = ...black
-000003b0: 5b6a 7570 7974 6572 5d3d 3d32 322e 332e  [jupyter]==22.3.
-000003c0: 300d 0a09 6973 6f72 743d 3d35 2e31 302e  0...isort==5.10.
-000003d0: 310d 0a09 7079 7465 7374 3d3d 372e 312e  1...pytest==7.1.
-000003e0: 320d 0a09 7079 7465 7374 2d63 6f76 3d3d  2...pytest-cov==
-000003f0: 332e 302e 300d 0a09 7079 6c69 6e74 3d3d  3.0.0...pylint==
-00000400: 322e 3133 2e38 0d0a 096d 7970 793d 3d31  2.13.8...mypy==1
-00000410: 2e30 2e30 0d0a 0962 616e 6469 745b 746f  .0.0...bandit[to
-00000420: 6d6c 5d3d 3d31 2e37 2e34 0d0a 0970 6970  ml]==1.7.4...pip
-00000430: 2d74 6f6f 6c73 2023 2066 6f72 2064 6570  -tools # for dep
-00000440: 7320 7069 6e6e 696e 670d 0a09 7479 7065  s pinning...type
-00000450: 732d 7079 7468 6f6e 2d73 6c75 6769 6679  s-python-slugify
-00000460: 3d3d 362e 312e 300d 0a09 6461 7368 3d3d  ==6.1.0...dash==
-00000470: 322e 372e 300d 0a09 6275 696c 640d 0a09  2.7.0...build...
-00000480: 7477 696e 650d 0a69 7079 203d 200d 0a09  twine..ipy = ...
-00000490: 6970 7974 686f 6e0d 0a09 6970 796b 6572  ipython...ipyker
-000004a0: 6e65 6c0d 0a09 6970 7974 686f 6e5f 6765  nel...ipython_ge
-000004b0: 6e75 7469 6c73 0d0a 096e 6f74 6562 6f6f  nutils...noteboo
-000004c0: 6b0d 0a09 6a75 7079 7465 726c 6162 0d0a  k...jupyterlab..
-000004d0: 646f 6320 3d20 0d0a 0969 7079 7468 6f6e  doc = ...ipython
-000004e0: 0d0a 096a 7570 7974 6572 2d62 6f6f 6b3d  ...jupyter-book=
-000004f0: 3d30 2e31 332e 310d 0a09 7370 6869 6e78  =0.13.1...sphinx
-00000500: 2d61 7574 6f61 7069 2023 2061 7574 6f20  -autoapi # auto 
-00000510: 6765 6e65 7261 7465 2041 5049 2064 6f63  generate API doc
-00000520: 0d0a 0967 6870 2d69 6d70 6f72 7420 2370  ...ghp-import #p
-00000530: 7562 6c69 7368 206f 6e20 6769 7468 7562  ublish on github
-00000540: 2070 6167 650d 0a09 6d79 7374 2d6e 620d   page...myst-nb.
-00000550: 0a09 6d79 7374 2d70 6172 7365 720d 0a0d  ..myst-parser...
-00000560: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000570: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000580: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000380: 2e31 2e32 0d0a 096d 726d 722d 7365 6c65  .1.2...mrmr-sele
+00000390: 6374 696f 6e3d 3d30 2e32 2e38 0d0a 0d0a  ction==0.2.8....
+000003a0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+000003b0: 7265 7175 6972 655d 0d0a 6465 7620 3d20  require]..dev = 
+000003c0: 0d0a 0962 6c61 636b 5b6a 7570 7974 6572  ...black[jupyter
+000003d0: 5d3d 3d32 322e 332e 300d 0a09 6973 6f72  ]==22.3.0...isor
+000003e0: 743d 3d35 2e31 302e 310d 0a09 7079 7465  t==5.10.1...pyte
+000003f0: 7374 3d3d 372e 312e 320d 0a09 7079 7465  st==7.1.2...pyte
+00000400: 7374 2d63 6f76 3d3d 332e 302e 300d 0a09  st-cov==3.0.0...
+00000410: 7079 6c69 6e74 3d3d 322e 3133 2e38 0d0a  pylint==2.13.8..
+00000420: 096d 7970 793d 3d31 2e30 2e30 0d0a 0962  .mypy==1.0.0...b
+00000430: 616e 6469 745b 746f 6d6c 5d3d 3d31 2e37  andit[toml]==1.7
+00000440: 2e34 0d0a 0970 6970 2d74 6f6f 6c73 2023  .4...pip-tools #
+00000450: 2066 6f72 2064 6570 7320 7069 6e6e 696e   for deps pinnin
+00000460: 670d 0a09 7479 7065 732d 7079 7468 6f6e  g...types-python
+00000470: 2d73 6c75 6769 6679 3d3d 362e 312e 300d  -slugify==6.1.0.
+00000480: 0a09 6461 7368 3d3d 322e 372e 300d 0a09  ..dash==2.7.0...
+00000490: 6275 696c 640d 0a09 7477 696e 650d 0a69  build...twine..i
+000004a0: 7079 203d 200d 0a09 6970 7974 686f 6e0d  py = ...ipython.
+000004b0: 0a09 6970 796b 6572 6e65 6c0d 0a09 6970  ..ipykernel...ip
+000004c0: 7974 686f 6e5f 6765 6e75 7469 6c73 0d0a  ython_genutils..
+000004d0: 096e 6f74 6562 6f6f 6b0d 0a09 6a75 7079  .notebook...jupy
+000004e0: 7465 726c 6162 0d0a 646f 6320 3d20 0d0a  terlab..doc = ..
+000004f0: 0969 7079 7468 6f6e 0d0a 096a 7570 7974  .ipython...jupyt
+00000500: 6572 2d62 6f6f 6b3d 3d30 2e31 332e 310d  er-book==0.13.1.
+00000510: 0a09 7370 6869 6e78 2d61 7574 6f61 7069  ..sphinx-autoapi
+00000520: 2023 2061 7574 6f20 6765 6e65 7261 7465   # auto generate
+00000530: 2041 5049 2064 6f63 0d0a 0967 6870 2d69   API doc...ghp-i
+00000540: 6d70 6f72 7420 2370 7562 6c69 7368 206f  mport #publish o
+00000550: 6e20 6769 7468 7562 2070 6167 650d 0a09  n github page...
+00000560: 6d79 7374 2d6e 620d 0a09 6d79 7374 2d70  myst-nb...myst-p
+00000570: 6172 7365 720d 0a0d 0a5b 6567 675f 696e  arser....[egg_in
+00000580: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000590: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000005a0: 0a0d 0a                                  ...
```

### Comparing `scorepyo-0.2.2.dev2/tests/conftest.py` & `scorepyo-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/tests/test_binarizer.py` & `scorepyo-0.2.3/tests/test_binarizer.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/tests/test_models.py` & `scorepyo-0.2.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `scorepyo-0.2.2.dev2/tests/test_scorepyo.py` & `scorepyo-0.2.3/tests/test_scorepyo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import numpy as np
 import pandas as pd
+import pytest
 from sklearn.datasets import load_breast_cancer
 from sklearn.metrics import (
     average_precision_score,
     precision_recall_curve,
     precision_score,
 )
 from sklearn.model_selection import train_test_split
 
 from scorepyo._utils import fast_numba_auc
 from scorepyo.calibration import VanillaCalibrator
 from scorepyo.models import EBMRiskScore
-from scorepyo.ranking import LogOddsDensity
+from scorepyo.ranking import LogOddsDensity, MRMRRank
 
 
-def test_end_2_end():
-    # assert True
-
+@pytest.mark.parametrize(
+    "ranker",
+    [LogOddsDensity(), MRMRRank()],
+)
+def test_end_2_end(ranker):
     data = load_breast_cancer()
     data_X, data_y = data.data, data.target
 
     X = pd.DataFrame(data=data_X, columns=data.feature_names)
     X["category"] = np.where(X["mean smoothness"] <= 0.1, "A", "B")
     y = pd.Series(data_y)
 
@@ -30,16 +33,14 @@
 
     X_test["category"] = "C"
 
     min_point_value = -2
     max_point_value = 3
     nb_max_features = 4
 
-    ranker = LogOddsDensity()
-
     optim_method = fast_numba_auc
 
     scorepyo_model = EBMRiskScore(
         min_point_value=min_point_value,
         max_point_value=max_point_value,
         nb_max_features=nb_max_features,
         nb_additional_features=6,
```

