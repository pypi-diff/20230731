# Comparing `tmp/onbrdng-0.0.1.tar.gz` & `tmp/onbrdng-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onbrdng-0.0.1.tar", last modified: Mon Jul 31 12:41:47 2023, max compression
+gzip compressed data, was "dist/onbrdng-0.0.2.tar", last modified: Mon Jul 31 13:06:27 2023, max compression
```

## Comparing `onbrdng-0.0.1.tar` & `onbrdng-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-07-31 12:41:47.602062 onbrdng-0.0.1/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    16867 2023-07-31 12:41:47.601906 onbrdng-0.0.1/PKG-INFO
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    13882 2023-07-31 12:21:43.000000 onbrdng-0.0.1/README.md
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-07-31 12:41:47.601023 onbrdng-0.0.1/onbrdng/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        0 2023-02-26 09:19:56.000000 onbrdng-0.0.1/onbrdng/__init__.py
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    21775 2023-04-07 12:26:23.000000 onbrdng-0.0.1/onbrdng/analyse_mmm_models.py
--rwxr-xr-x   0 simonteggelaar   (501) staff       (20)     4864 2023-02-23 10:18:58.000000 onbrdng-0.0.1/onbrdng/creating_dataset.py
--rwxr-xr-x   0 simonteggelaar   (501) staff       (20)     4119 2023-02-24 09:05:32.000000 onbrdng-0.0.1/onbrdng/exploring_dataset.py
--rwxr-xr-x   0 simonteggelaar   (501) staff       (20)    25995 2023-03-02 11:21:00.000000 onbrdng-0.0.1/onbrdng/forecasting_models.py
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     9326 2023-07-31 11:46:40.000000 onbrdng-0.0.1/onbrdng/generate_example_data.py
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     3249 2023-01-25 12:28:06.000000 onbrdng-0.0.1/onbrdng/logistic_regression_decomp.py
--rwxr-xr-x   0 simonteggelaar   (501) staff       (20)    10483 2023-07-08 09:44:13.000000 onbrdng-0.0.1/onbrdng/make_html.py
--rwxr-xr-x   0 simonteggelaar   (501) staff       (20)    15020 2023-07-31 12:30:38.000000 onbrdng-0.0.1/onbrdng/ml_models.py
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    22950 2022-05-12 12:18:32.000000 onbrdng-0.0.1/onbrdng/model_visual_functions.py
--rwxr-xr-x   0 simonteggelaar   (501) staff       (20)     1493 2023-02-24 10:02:09.000000 onbrdng-0.0.1/onbrdng/visualizing_dataset.py
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-07-31 12:41:47.601673 onbrdng-0.0.1/onbrdng.egg-info/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    16867 2023-07-31 12:41:47.000000 onbrdng-0.0.1/onbrdng.egg-info/PKG-INFO
--rw-r--r--   0 simonteggelaar   (501) staff       (20)      487 2023-07-31 12:41:47.000000 onbrdng-0.0.1/onbrdng.egg-info/SOURCES.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        1 2023-07-31 12:41:47.000000 onbrdng-0.0.1/onbrdng.egg-info/dependency_links.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)       74 2023-07-31 12:41:47.000000 onbrdng-0.0.1/onbrdng.egg-info/requires.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        8 2023-07-31 12:41:47.000000 onbrdng-0.0.1/onbrdng.egg-info/top_level.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)       38 2023-07-31 12:41:47.602105 onbrdng-0.0.1/setup.cfg
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     1543 2023-07-31 12:27:57.000000 onbrdng-0.0.1/setup.py
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-07-31 13:06:27.897014 onbrdng-0.0.2/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    16862 2023-07-31 13:06:27.896871 onbrdng-0.0.2/PKG-INFO
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    13869 2023-07-31 13:04:25.000000 onbrdng-0.0.2/README.md
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-07-31 13:06:27.895985 onbrdng-0.0.2/onbrdng/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        0 2023-02-26 09:19:56.000000 onbrdng-0.0.2/onbrdng/__init__.py
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    21775 2023-04-07 12:26:23.000000 onbrdng-0.0.2/onbrdng/analyse_mmm_models.py
+-rwxr-xr-x   0 simonteggelaar   (501) staff       (20)     4864 2023-02-23 10:18:58.000000 onbrdng-0.0.2/onbrdng/creating_dataset.py
+-rwxr-xr-x   0 simonteggelaar   (501) staff       (20)     4119 2023-02-24 09:05:32.000000 onbrdng-0.0.2/onbrdng/exploring_dataset.py
+-rwxr-xr-x   0 simonteggelaar   (501) staff       (20)    25995 2023-03-02 11:21:00.000000 onbrdng-0.0.2/onbrdng/forecasting_models.py
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     9326 2023-07-31 11:46:40.000000 onbrdng-0.0.2/onbrdng/generate_example_data.py
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     3249 2023-01-25 12:28:06.000000 onbrdng-0.0.2/onbrdng/logistic_regression_decomp.py
+-rwxr-xr-x   0 simonteggelaar   (501) staff       (20)    10483 2023-07-08 09:44:13.000000 onbrdng-0.0.2/onbrdng/make_html.py
+-rwxr-xr-x   0 simonteggelaar   (501) staff       (20)    15020 2023-07-31 12:30:38.000000 onbrdng-0.0.2/onbrdng/ml_models.py
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    22950 2022-05-12 12:18:32.000000 onbrdng-0.0.2/onbrdng/model_visual_functions.py
+-rwxr-xr-x   0 simonteggelaar   (501) staff       (20)     1493 2023-02-24 10:02:09.000000 onbrdng-0.0.2/onbrdng/visualizing_dataset.py
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-07-31 13:06:27.896657 onbrdng-0.0.2/onbrdng.egg-info/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    16862 2023-07-31 13:06:27.000000 onbrdng-0.0.2/onbrdng.egg-info/PKG-INFO
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)      487 2023-07-31 13:06:27.000000 onbrdng-0.0.2/onbrdng.egg-info/SOURCES.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        1 2023-07-31 13:06:27.000000 onbrdng-0.0.2/onbrdng.egg-info/dependency_links.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)       79 2023-07-31 13:06:27.000000 onbrdng-0.0.2/onbrdng.egg-info/requires.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        8 2023-07-31 13:06:27.000000 onbrdng-0.0.2/onbrdng.egg-info/top_level.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)       38 2023-07-31 13:06:27.897054 onbrdng-0.0.2/setup.cfg
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     1551 2023-07-31 13:06:27.000000 onbrdng-0.0.2/setup.py
```

### Comparing `onbrdng-0.0.1/PKG-INFO` & `onbrdng-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: onbrdng
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package that makes it a bit easier to understand some complex models and helps you visualize them
 Home-page: UNKNOWN
 Author: Data modelling team Onbrdng
 Author-email: can.yildiz@onbrdng.com
 License: MIT
 Description: # `onbrdng`
         
         The `onbrdng` is a package made by Onbrdng for the data team and it's clients to use
         
         It contains multiple modules to analyse different problems:
-        0. Marketing Mix Modeling
-        1. Decomposition for logistic regressions over time
-        2. Multinomial logistic regression with impact of variables 
-        3. Decision tree / beslisboom
-        4. Time-series forecasting with regressions and random forest
-        5. Saving and loading models
+        
+        1. Marketing Mix Modeling
+        2. Decomposition for logistic regressions over time
+        3. Multinomial logistic regression with impact of variables 
+        4. Decision tree / beslisboom
+        5. Time-series forecasting with regressions and random forest
+        6. Saving and loading models
         
         ## Installation
         
         Use the package manager [pip](https://pip.pypa.io/en/stable/) to install onbrdng.
         
         ```bash
         pip install onbrdng
         ```
         
-        ## 0. MMM
+        ## 1. MMM
         
         ```python
         
         # import modules
         import pandas as pd
         import numpy as np
         from onbrdng.analyse_mmm_models import mmm, s_curve, decay
@@ -75,15 +76,15 @@
         
         # Analyse for adding variables
         analyse_model.select_n_largest_outliers(5)
         analyse_model.check_variables_to_add()
         
         ``` 
         
-        ## 1. Usage Decomposition for logistic regressions over time
+        ## 2. Usage Decomposition for logistic regressions over time
         
         ```python
         
         # import modules
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.creating_dataset import CreatingDataSet
         from onbrdng.logistic_regression_decomp import LogisticDecomposition
@@ -122,15 +123,15 @@
         decomposition_results = model_decomp.decomposition_logistic(X_train, split_var=split_var, plot=True, y=[],
                                                                      X_vars_to_show=vars_to_show,
                                                                      scaling_to_mean_odds_model=True,
                                                                      scaling_to_actual_odds=False)
         
         ```
         
-        ## 2. Usage Multinomial Logistic Regression
+        ## 3. Usage Multinomial Logistic Regression
         ```python
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.creating_dataset import CreatingDataSet
         from onbrdng.ml_models import Models, EvaluateModels
         import plotly.io as pio
         pio.renderers.default = 'browser'
         
@@ -173,15 +174,15 @@
                                                         bin_size=0.01).show()
         
         # Visualize the impact of each variable on a brand, merken_x_as=True gives the brands on the x_as, False the y_as
         evalueren_model.determine_drivers_mvlogit(model_mvl, merken_x_as=False).show()
         ```
         
         
-        ## 3. Usage Decision tree / beslisboom
+        ## 4. Usage Decision tree / beslisboom
         ```python
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.make_html import CreateHTML
         import time
         
         # Generate some sample data
         example_data = GenerateData(10000)
@@ -195,33 +196,33 @@
         min_records = 500  # min N waarna nog een split gemaakt wordt
         max_integer = 5  # maximaal aantal splits bij een integer variabelen
         max_nr_splits = 2  # behalve voor categorische variabelen
         min_split_values = 1000  # minimale N voor een split
         nr_splits = {'leeftijd': 4}  # aantal splits per variabelen (kan overschreven worden door splits)
         splits = {'leeftijd': [20,25,40,60]}  # op welke waarde een split
         color_reverse = True  # omkering kleuren. bij True, rood laag, blauw hoog
-        name_all = 'Alle spelers'  # De naam die bij het eerste bolletje staat
+        name_all = 'All clients'  # De naam die bij het eerste bolletje staat
         
         # Create the actual HTML file
         create_html = CreateHTML(df_example, variables_, y, split_method=split_method, min_records=min_records,
                                  max_integer=max_integer, max_nr_splits=max_nr_splits, min_split_values=min_split_values,
                                  nr_splits=nr_splits, splits=splits, color_reverse=color_reverse, name_all=name_all,
                                  reorder=reorder)
         start = time.process_time()
         
         # Input for the created HTML filel
         output_file = 'beslisboom_voorbeeld.html'  # name you wanna give it (has to end with .html)
         title = 'Super Insights'  # The title on top of the html
         explanation= 'One Planet, Plant it:</br> <span class="emoji">&#128514;</span>' # Text for in the explanation box
-        made_by = 'Een toppertje van BI'  # Made by in the left corner of the file
+        made_by = 'Onbrdng'  # Made by in the left corner of the file
         create_html.build_HTML(output_file=output_file, title=title, explanation=explanation, made_by=made_by)
         print(time.process_time() - start)
         ```
         
-        ## 4. Usage Time-series forecasting with regressions and random forest
+        ## 5. Usage Time-series forecasting with regressions and random forest
         
         ```python
         import pandas as pd
         import numpy as np
         import statsmodels.formula.api as smf
         from onbrdng.forecasting_models import ForecastingModels, check_variables_to_add
         import ssl
@@ -268,15 +269,15 @@
         
         # Only get the data from the above graph:
         forecast_df = forecasting_sales.forecast(formule=formule, date='maand_jaar', te_voorspellen='sales', show_graph=False
                                                  , get_data=True, random_forest_forecast=True, max_features=6, n_estimators=500)
         ```
         
         
-        ## 5. Saving and loading your models
+        ## 6. Saving and loading your models
         ```python
         import joblib
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.creating_dataset import CreatingDataSet
         from onbrdng.ml_models import Models, save_model
         
         # Generate data
```

### Comparing `onbrdng-0.0.1/README.md` & `onbrdng-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # `onbrdng`
 
 The `onbrdng` is a package made by Onbrdng for the data team and it's clients to use
 
 It contains multiple modules to analyse different problems:
-0. Marketing Mix Modeling
-1. Decomposition for logistic regressions over time
-2. Multinomial logistic regression with impact of variables 
-3. Decision tree / beslisboom
-4. Time-series forecasting with regressions and random forest
-5. Saving and loading models
+
+1. Marketing Mix Modeling
+2. Decomposition for logistic regressions over time
+3. Multinomial logistic regression with impact of variables 
+4. Decision tree / beslisboom
+5. Time-series forecasting with regressions and random forest
+6. Saving and loading models
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install onbrdng.
 
 ```bash
 pip install onbrdng
 ```
 
-## 0. MMM
+## 1. MMM
 
 ```python
 
 # import modules
 import pandas as pd
 import numpy as np
 from onbrdng.analyse_mmm_models import mmm, s_curve, decay
@@ -67,15 +68,15 @@
 
 # Analyse for adding variables
 analyse_model.select_n_largest_outliers(5)
 analyse_model.check_variables_to_add()
 
 ``` 
 
-## 1. Usage Decomposition for logistic regressions over time
+## 2. Usage Decomposition for logistic regressions over time
 
 ```python
 
 # import modules
 from onbrdng.generate_example_data import GenerateData
 from onbrdng.creating_dataset import CreatingDataSet
 from onbrdng.logistic_regression_decomp import LogisticDecomposition
@@ -114,15 +115,15 @@
 decomposition_results = model_decomp.decomposition_logistic(X_train, split_var=split_var, plot=True, y=[],
                                                              X_vars_to_show=vars_to_show,
                                                              scaling_to_mean_odds_model=True,
                                                              scaling_to_actual_odds=False)
 
 ```
 
-## 2. Usage Multinomial Logistic Regression
+## 3. Usage Multinomial Logistic Regression
 ```python
 from onbrdng.generate_example_data import GenerateData
 from onbrdng.creating_dataset import CreatingDataSet
 from onbrdng.ml_models import Models, EvaluateModels
 import plotly.io as pio
 pio.renderers.default = 'browser'
 
@@ -165,15 +166,15 @@
                                                 bin_size=0.01).show()
 
 # Visualize the impact of each variable on a brand, merken_x_as=True gives the brands on the x_as, False the y_as
 evalueren_model.determine_drivers_mvlogit(model_mvl, merken_x_as=False).show()
 ```
 
 
-## 3. Usage Decision tree / beslisboom
+## 4. Usage Decision tree / beslisboom
 ```python
 from onbrdng.generate_example_data import GenerateData
 from onbrdng.make_html import CreateHTML
 import time
 
 # Generate some sample data
 example_data = GenerateData(10000)
@@ -187,33 +188,33 @@
 min_records = 500  # min N waarna nog een split gemaakt wordt
 max_integer = 5  # maximaal aantal splits bij een integer variabelen
 max_nr_splits = 2  # behalve voor categorische variabelen
 min_split_values = 1000  # minimale N voor een split
 nr_splits = {'leeftijd': 4}  # aantal splits per variabelen (kan overschreven worden door splits)
 splits = {'leeftijd': [20,25,40,60]}  # op welke waarde een split
 color_reverse = True  # omkering kleuren. bij True, rood laag, blauw hoog
-name_all = 'Alle spelers'  # De naam die bij het eerste bolletje staat
+name_all = 'All clients'  # De naam die bij het eerste bolletje staat
 
 # Create the actual HTML file
 create_html = CreateHTML(df_example, variables_, y, split_method=split_method, min_records=min_records,
                          max_integer=max_integer, max_nr_splits=max_nr_splits, min_split_values=min_split_values,
                          nr_splits=nr_splits, splits=splits, color_reverse=color_reverse, name_all=name_all,
                          reorder=reorder)
 start = time.process_time()
 
 # Input for the created HTML filel
 output_file = 'beslisboom_voorbeeld.html'  # name you wanna give it (has to end with .html)
 title = 'Super Insights'  # The title on top of the html
 explanation= 'One Planet, Plant it:</br> <span class="emoji">&#128514;</span>' # Text for in the explanation box
-made_by = 'Een toppertje van BI'  # Made by in the left corner of the file
+made_by = 'Onbrdng'  # Made by in the left corner of the file
 create_html.build_HTML(output_file=output_file, title=title, explanation=explanation, made_by=made_by)
 print(time.process_time() - start)
 ```
 
-## 4. Usage Time-series forecasting with regressions and random forest
+## 5. Usage Time-series forecasting with regressions and random forest
 
 ```python
 import pandas as pd
 import numpy as np
 import statsmodels.formula.api as smf
 from onbrdng.forecasting_models import ForecastingModels, check_variables_to_add
 import ssl
@@ -260,15 +261,15 @@
 
 # Only get the data from the above graph:
 forecast_df = forecasting_sales.forecast(formule=formule, date='maand_jaar', te_voorspellen='sales', show_graph=False
                                          , get_data=True, random_forest_forecast=True, max_features=6, n_estimators=500)
 ```
 
 
-## 5. Saving and loading your models
+## 6. Saving and loading your models
 ```python
 import joblib
 from onbrdng.generate_example_data import GenerateData
 from onbrdng.creating_dataset import CreatingDataSet
 from onbrdng.ml_models import Models, save_model
 
 # Generate data
```

### Comparing `onbrdng-0.0.1/onbrdng/analyse_mmm_models.py` & `onbrdng-0.0.2/onbrdng/analyse_mmm_models.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/creating_dataset.py` & `onbrdng-0.0.2/onbrdng/creating_dataset.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/exploring_dataset.py` & `onbrdng-0.0.2/onbrdng/exploring_dataset.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/forecasting_models.py` & `onbrdng-0.0.2/onbrdng/forecasting_models.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/generate_example_data.py` & `onbrdng-0.0.2/onbrdng/generate_example_data.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/logistic_regression_decomp.py` & `onbrdng-0.0.2/onbrdng/logistic_regression_decomp.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/make_html.py` & `onbrdng-0.0.2/onbrdng/make_html.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/ml_models.py` & `onbrdng-0.0.2/onbrdng/ml_models.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/model_visual_functions.py` & `onbrdng-0.0.2/onbrdng/model_visual_functions.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng/visualizing_dataset.py` & `onbrdng-0.0.2/onbrdng/visualizing_dataset.py`

 * *Files identical despite different names*

### Comparing `onbrdng-0.0.1/onbrdng.egg-info/PKG-INFO` & `onbrdng-0.0.2/onbrdng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: onbrdng
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package that makes it a bit easier to understand some complex models and helps you visualize them
 Home-page: UNKNOWN
 Author: Data modelling team Onbrdng
 Author-email: can.yildiz@onbrdng.com
 License: MIT
 Description: # `onbrdng`
         
         The `onbrdng` is a package made by Onbrdng for the data team and it's clients to use
         
         It contains multiple modules to analyse different problems:
-        0. Marketing Mix Modeling
-        1. Decomposition for logistic regressions over time
-        2. Multinomial logistic regression with impact of variables 
-        3. Decision tree / beslisboom
-        4. Time-series forecasting with regressions and random forest
-        5. Saving and loading models
+        
+        1. Marketing Mix Modeling
+        2. Decomposition for logistic regressions over time
+        3. Multinomial logistic regression with impact of variables 
+        4. Decision tree / beslisboom
+        5. Time-series forecasting with regressions and random forest
+        6. Saving and loading models
         
         ## Installation
         
         Use the package manager [pip](https://pip.pypa.io/en/stable/) to install onbrdng.
         
         ```bash
         pip install onbrdng
         ```
         
-        ## 0. MMM
+        ## 1. MMM
         
         ```python
         
         # import modules
         import pandas as pd
         import numpy as np
         from onbrdng.analyse_mmm_models import mmm, s_curve, decay
@@ -75,15 +76,15 @@
         
         # Analyse for adding variables
         analyse_model.select_n_largest_outliers(5)
         analyse_model.check_variables_to_add()
         
         ``` 
         
-        ## 1. Usage Decomposition for logistic regressions over time
+        ## 2. Usage Decomposition for logistic regressions over time
         
         ```python
         
         # import modules
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.creating_dataset import CreatingDataSet
         from onbrdng.logistic_regression_decomp import LogisticDecomposition
@@ -122,15 +123,15 @@
         decomposition_results = model_decomp.decomposition_logistic(X_train, split_var=split_var, plot=True, y=[],
                                                                      X_vars_to_show=vars_to_show,
                                                                      scaling_to_mean_odds_model=True,
                                                                      scaling_to_actual_odds=False)
         
         ```
         
-        ## 2. Usage Multinomial Logistic Regression
+        ## 3. Usage Multinomial Logistic Regression
         ```python
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.creating_dataset import CreatingDataSet
         from onbrdng.ml_models import Models, EvaluateModels
         import plotly.io as pio
         pio.renderers.default = 'browser'
         
@@ -173,15 +174,15 @@
                                                         bin_size=0.01).show()
         
         # Visualize the impact of each variable on a brand, merken_x_as=True gives the brands on the x_as, False the y_as
         evalueren_model.determine_drivers_mvlogit(model_mvl, merken_x_as=False).show()
         ```
         
         
-        ## 3. Usage Decision tree / beslisboom
+        ## 4. Usage Decision tree / beslisboom
         ```python
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.make_html import CreateHTML
         import time
         
         # Generate some sample data
         example_data = GenerateData(10000)
@@ -195,33 +196,33 @@
         min_records = 500  # min N waarna nog een split gemaakt wordt
         max_integer = 5  # maximaal aantal splits bij een integer variabelen
         max_nr_splits = 2  # behalve voor categorische variabelen
         min_split_values = 1000  # minimale N voor een split
         nr_splits = {'leeftijd': 4}  # aantal splits per variabelen (kan overschreven worden door splits)
         splits = {'leeftijd': [20,25,40,60]}  # op welke waarde een split
         color_reverse = True  # omkering kleuren. bij True, rood laag, blauw hoog
-        name_all = 'Alle spelers'  # De naam die bij het eerste bolletje staat
+        name_all = 'All clients'  # De naam die bij het eerste bolletje staat
         
         # Create the actual HTML file
         create_html = CreateHTML(df_example, variables_, y, split_method=split_method, min_records=min_records,
                                  max_integer=max_integer, max_nr_splits=max_nr_splits, min_split_values=min_split_values,
                                  nr_splits=nr_splits, splits=splits, color_reverse=color_reverse, name_all=name_all,
                                  reorder=reorder)
         start = time.process_time()
         
         # Input for the created HTML filel
         output_file = 'beslisboom_voorbeeld.html'  # name you wanna give it (has to end with .html)
         title = 'Super Insights'  # The title on top of the html
         explanation= 'One Planet, Plant it:</br> <span class="emoji">&#128514;</span>' # Text for in the explanation box
-        made_by = 'Een toppertje van BI'  # Made by in the left corner of the file
+        made_by = 'Onbrdng'  # Made by in the left corner of the file
         create_html.build_HTML(output_file=output_file, title=title, explanation=explanation, made_by=made_by)
         print(time.process_time() - start)
         ```
         
-        ## 4. Usage Time-series forecasting with regressions and random forest
+        ## 5. Usage Time-series forecasting with regressions and random forest
         
         ```python
         import pandas as pd
         import numpy as np
         import statsmodels.formula.api as smf
         from onbrdng.forecasting_models import ForecastingModels, check_variables_to_add
         import ssl
@@ -268,15 +269,15 @@
         
         # Only get the data from the above graph:
         forecast_df = forecasting_sales.forecast(formule=formule, date='maand_jaar', te_voorspellen='sales', show_graph=False
                                                  , get_data=True, random_forest_forecast=True, max_features=6, n_estimators=500)
         ```
         
         
-        ## 5. Saving and loading your models
+        ## 6. Saving and loading your models
         ```python
         import joblib
         from onbrdng.generate_example_data import GenerateData
         from onbrdng.creating_dataset import CreatingDataSet
         from onbrdng.ml_models import Models, save_model
         
         # Generate data
```

### Comparing `onbrdng-0.0.1/setup.py` & `onbrdng-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="onbrdng",
 
     # version of the module
-    version="0.0.1",
+    version="0.0.2",
 
     # Name of Author
     author="Data modelling team Onbrdng",
 
     # your Email address
     author_email="can.yildiz@onbrdng.com",
 
@@ -31,15 +31,15 @@
     # url="https://github.com/username/",
     packages=setuptools.find_packages(),
 
     # if module has dependencies i.e. if your package rely on other package at pypi.org
     # then you must add there, in order to download every requirement of package
 
     install_requires=[
-         "pandas", "scipy", "plotly", "statsmodels", "tqdm", "xgboost", "scikit-learn", "requests", "joblib"
+         "pandas", "scipy", "plotly", "statsmodels", "tqdm", "xgboost", "scikit-learn", "requests", "joblib", "lxml"
        ],
 
     license="MIT",
 
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
         "Programming Language :: Python :: 3",
```

