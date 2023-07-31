# Comparing `tmp/estyp-0.3.0.tar.gz` & `tmp/estyp-0.4.0.tar.gz`

## Comparing `estyp-0.3.0.tar` & `estyp-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/__init__.py
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/linear_model/stepwise/__init__.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/linear_model/stepwise/__base/__init__.py
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/testing/__init__.py
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.3.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.3.0/LICENSE
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 estyp-0.3.0/README.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 estyp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 estyp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/__init__.py
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/linear_model/stepwise/__init__.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/linear_model/stepwise/__base/__init__.py
+-rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/testing/__init__.py
+-rw-r--r--   0        0        0    23090 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 estyp-0.4.0/README.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 estyp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 estyp-0.4.0/PKG-INFO
```

### Comparing `estyp-0.3.0/estyp/linear_model/__init__.py` & `estyp-0.4.0/estyp/linear_model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from pandas import Series, DataFrame, concat
 from patsy import dmatrices, build_design_matrices
 from typing import Literal
 from scipy.stats import norm
-from sklearn.linear_model import LogisticRegression
+from sklearn._typing import Int
+from sklearn.linear_model import LinearRegression, LogisticRegression
 
 
 class LogisticRegression(LogisticRegression):
     """
 # Logistic Regression
 
 This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
@@ -143,8 +144,8 @@
     @property
     def bic(self):
         bic = -2 * self.__log_likelihood() + np.log(self.X.shape[0]) * (self.coef_.shape[0] - 1)
         return bic.item()
     
     
     def __repr__(self) -> str:
-        return "LogisticRegression()"
+        return "LogisticRegression()"
```

### Comparing `estyp-0.3.0/estyp/linear_model/stepwise/__init__.py` & `estyp-0.4.0/estyp/linear_model/stepwise/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.3.0/estyp/linear_model/stepwise/__base/__init__.py` & `estyp-0.4.0/estyp/linear_model/stepwise/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.3.0/.gitignore` & `estyp-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `estyp-0.3.0/LICENSE` & `estyp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.3.0/README.md` & `estyp-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
+[![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
+
 ## Description
 
 This library is a collection of statistical functions for Python.
 
-Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
+Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
 ## Changelog 
 
+### V0.4.0
+
+* Added `testing.prop_test()` function to perform a test of proportions.
+* Added `testing.CheckModel()` class to perform linear regression assumptions checking.
+* Added badges to README.
+* Minor changes in README.
+
 ### V0.3.0
 
 * Changed `scipy>=1.11.1` to `scipy>=1.10.1` as a depedency of the library.
 * New modularization of the functions in the `linear_model` module.
 * Added `linear_model.stepwise.forward_selection()` function to perform forward variable selection based in p-values.
 * Added `testing.nested_models_test()` function to perform nested models testing.
 * Added option to specity aditional parameters of the model like `kwargs` in `linear_model.stepwise.forward_selection()` and `linear_model.stepwise.both_selection()` functions.  
-* Minor changes in the README.
+* Minor changes in README.
+
+### V0.2.5
+
+* Added `scipy>=1.11.1` as a depedency of the library.
+* New modularization of the functions in the `testing` module.
+* R like documentation in the `testing.var_test()` function.
+* Added `testing.t_test()` function to perform t-test like in software R.
 
-## Functions
+## Features
 
 * `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
 * `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
-* `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
-* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
+* `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
+* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the R software.
+* `testing.prop.test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
 * `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
-# Installation
+## Installation
 
-To install this library, you can use pip:
+To install this library, you can use PyPI:
 
 ```bash
 pip install estyp
 ```
 
 ## License
```

### Comparing `estyp-0.3.0/pyproject.toml` & `estyp-0.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Extended Statistical Toolkit Yet Practical"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Development Status :: 1 - Planning"
+    "Operating System :: OS Independent"
 ]
 dependencies = [
     "numpy >= 1.22.3",
     "scikit-learn >= 1.2.1",
+    "matplotlib >= 3.4.3",
     "patsy >= 0.5.3",
     "statsmodels >= 0.13.5",
     "scipy >= 1.10.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/estebanrucan/estyp"
```

### Comparing `estyp-0.3.0/PKG-INFO` & `estyp-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.3.0
+Version: 0.4.0
 Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -23,57 +23,75 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9.12
+Requires-Dist: matplotlib>=3.4.3
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: patsy>=0.5.3
 Requires-Dist: scikit-learn>=1.2.1
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.5
 Description-Content-Type: text/markdown
 
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
+[![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
+
 ## Description
 
 This library is a collection of statistical functions for Python.
 
-Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
+Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
 ## Changelog 
 
+### V0.4.0
+
+* Added `testing.prop_test()` function to perform a test of proportions.
+* Added `testing.CheckModel()` class to perform linear regression assumptions checking.
+* Added badges to README.
+* Minor changes in README.
+
 ### V0.3.0
 
 * Changed `scipy>=1.11.1` to `scipy>=1.10.1` as a depedency of the library.
 * New modularization of the functions in the `linear_model` module.
 * Added `linear_model.stepwise.forward_selection()` function to perform forward variable selection based in p-values.
 * Added `testing.nested_models_test()` function to perform nested models testing.
 * Added option to specity aditional parameters of the model like `kwargs` in `linear_model.stepwise.forward_selection()` and `linear_model.stepwise.both_selection()` functions.  
-* Minor changes in the README.
+* Minor changes in README.
+
+### V0.2.5
+
+* Added `scipy>=1.11.1` as a depedency of the library.
+* New modularization of the functions in the `testing` module.
+* R like documentation in the `testing.var_test()` function.
+* Added `testing.t_test()` function to perform t-test like in software R.
 
-## Functions
+## Features
 
 * `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
 * `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
-* `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
-* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
+* `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
+* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the R software.
+* `testing.prop.test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
 * `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
-# Installation
+## Installation
 
-To install this library, you can use pip:
+To install this library, you can use PyPI:
 
 ```bash
 pip install estyp
 ```
 
 ## License
```

