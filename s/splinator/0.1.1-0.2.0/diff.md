# Comparing `tmp/splinator-0.1.1.tar.gz` & `tmp/splinator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splinator-0.1.1.tar", max compression
+gzip compressed data, was "splinator-0.2.0.tar", last modified: Mon Jul 31 07:46:38 2023, max compression
```

## Comparing `splinator-0.1.1.tar` & `splinator-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,20 @@
--rw-r--r--   0        0        0     1520 2022-09-07 07:02:54.532566 splinator-0.1.1/LICENSE
--rw-r--r--   0        0        0      788 2022-09-26 07:39:15.662316 splinator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2022-09-07 07:02:54.538687 splinator-0.1.1/splinator/__init__.py
--rw-r--r--   0        0        0       21 2022-09-07 07:02:54.539219 splinator-0.1.1/splinator/_version.py
--rw-r--r--   0        0        0    12528 2022-09-07 07:02:54.539710 splinator-0.1.1/splinator/estimators.py
--rw-r--r--   0        0        0        0 2022-09-07 07:02:54.539742 splinator-0.1.1/splinator/metrics.py
--rw-r--r--   0        0        0     4895 2022-09-07 07:02:54.540362 splinator-0.1.1/splinator/monotonic_spline.py
--rw-r--r--   0        0        0        0 2022-08-21 20:25:54.389404 splinator-0.1.1/splinator/tests/__init__.py
--rw-r--r--   0        0        0     7114 2022-09-07 07:02:54.540727 splinator-0.1.1/splinator/tests/common.py
--rw-r--r--   0        0        0     1466 2022-09-07 07:02:54.540959 splinator-0.1.1/splinator/tests/test_helpers.py
--rw-r--r--   0        0        0     3421 2022-09-07 07:02:54.541130 splinator-0.1.1/splinator/tests/test_linear_spline_logistic_regression.py
--rw-r--r--   0        0        0      297 2022-09-07 07:02:54.541458 splinator-0.1.1/splinator/tests/test_scikit_learn_estimator.py
--rw-r--r--   0        0        0      795 2022-09-26 07:39:36.682499 splinator-0.1.1/setup.py
--rw-r--r--   0        0        0      798 2022-09-26 07:39:36.682705 splinator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-09-07 07:02:54.532566 splinator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2665 2023-07-31 07:37:36.301233 splinator-0.2.0/README.md
+-rw-r--r--   0        0        0      939 2023-07-31 07:46:38.091542 splinator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2022-09-07 07:02:54.538687 splinator-0.2.0/src/splinator/__init__.py
+-rw-r--r--   0        0        0       21 2022-09-07 07:02:54.539219 splinator-0.2.0/src/splinator/_version.py
+-rw-r--r--   0        0        0    12528 2022-09-07 07:02:54.539710 splinator-0.2.0/src/splinator/estimators.py
+-rw-r--r--   0        0        0      656 2023-07-31 07:26:59.687299 splinator-0.2.0/src/splinator/metrics.py
+-rw-r--r--   0        0        0     4895 2022-09-07 07:02:54.540362 splinator-0.2.0/src/splinator/monotonic_spline.py
+-rw-r--r--   0        0        0       37 2023-07-31 07:29:10.870029 splinator-0.2.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-07-31 07:29:10.870124 splinator-0.2.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-07-31 07:29:10.869928 splinator-0.2.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-07-31 07:29:10.870239 splinator-0.2.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-07-31 07:29:10.870387 splinator-0.2.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-08-21 20:25:54.389404 splinator-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     7114 2022-09-07 07:02:54.540727 splinator-0.2.0/tests/common.py
+-rw-r--r--   0        0        0     1466 2022-09-07 07:02:54.540959 splinator-0.2.0/tests/test_helpers.py
+-rw-r--r--   0        0        0     3401 2023-07-30 04:28:37.122658 splinator-0.2.0/tests/test_linear_spline_logistic_regression.py
+-rw-r--r--   0        0        0     1371 2023-07-31 07:28:43.633374 splinator-0.2.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      297 2022-09-07 07:02:54.541458 splinator-0.2.0/tests/test_scikit_learn_estimator.py
+-rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 splinator-0.2.0/PKG-INFO
```

### Comparing `splinator-0.1.1/LICENSE` & `splinator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splinator-0.1.1/splinator/estimators.py` & `splinator-0.2.0/src/splinator/estimators.py`

 * *Files identical despite different names*

### Comparing `splinator-0.1.1/splinator/monotonic_spline.py` & `splinator-0.2.0/src/splinator/monotonic_spline.py`

 * *Files identical despite different names*

### Comparing `splinator-0.1.1/splinator/tests/common.py` & `splinator-0.2.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `splinator-0.1.1/splinator/tests/test_helpers.py` & `splinator-0.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `splinator-0.1.1/splinator/tests/test_linear_spline_logistic_regression.py` & `splinator-0.2.0/tests/test_linear_spline_logistic_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import absolute_import, division, print_function
 
 import itertools
 import unittest
 import numpy as np
 from splinator.monotonic_spline import Monotonicity
 from splinator.estimators import LinearSplineLogisticRegression
-from splinator.tests.common import (
+from tests.common import (
     generate_piecewise_function,
     generate_training_data,
 )
-from splinator.tests.test_helpers import assert_allclose_absolute
+from tests.test_helpers import assert_allclose_absolute
 
 
 class TestFitOnSyntheticData(unittest.TestCase):
     def setUp(self):
         np.random.seed(123)
         options = dict(
             num_additional_inputs=[0, 1],
```

