# Comparing `tmp/synthedata-0.0.3.tar.gz` & `tmp/synthedata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/synthedata-0.0.3.tar", last modified: Thu Jul 20 09:02:49 2023, max compression
+gzip compressed data, was "dist/synthedata-0.0.4.tar", last modified: Mon Jul 31 15:49:56 2023, max compression
```

## Comparing `synthedata-0.0.3.tar` & `synthedata-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-20 09:02:49.594545 synthedata-0.0.3/
--rw-r--r--   0 annli      (501) staff       (20)     8768 2023-07-20 09:02:49.593763 synthedata-0.0.3/PKG-INFO
--rw-r--r--   0 annli      (501) staff       (20)     7176 2023-05-25 20:34:45.000000 synthedata-0.0.3/README.md
--rw-r--r--   0 annli      (501) staff       (20)       38 2023-07-20 09:02:49.594764 synthedata-0.0.3/setup.cfg
--rw-r--r--   0 annli      (501) staff       (20)      662 2023-07-20 09:02:35.000000 synthedata-0.0.3/setup.py
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-20 09:02:49.589125 synthedata-0.0.3/synthedata/
--rw-r--r--   0 annli      (501) staff       (20)       18 2023-05-25 20:33:58.000000 synthedata-0.0.3/synthedata/__init__.py
--rw-r--r--   0 annli      (501) staff       (20)    26603 2023-07-20 08:02:14.000000 synthedata-0.0.3/synthedata/datacreator.py
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-20 09:02:49.592034 synthedata-0.0.3/synthedata.egg-info/
--rw-r--r--   0 annli      (501) staff       (20)     8768 2023-07-20 09:02:49.000000 synthedata-0.0.3/synthedata.egg-info/PKG-INFO
--rw-r--r--   0 annli      (501) staff       (20)      203 2023-07-20 09:02:49.000000 synthedata-0.0.3/synthedata.egg-info/SOURCES.txt
--rw-r--r--   0 annli      (501) staff       (20)        1 2023-07-20 09:02:49.000000 synthedata-0.0.3/synthedata.egg-info/dependency_links.txt
--rw-r--r--   0 annli      (501) staff       (20)       11 2023-07-20 09:02:49.000000 synthedata-0.0.3/synthedata.egg-info/top_level.txt
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-31 15:49:56.036948 synthedata-0.0.4/
+-rw-r--r--   0 annli      (501) staff       (20)     8768 2023-07-31 15:49:56.036666 synthedata-0.0.4/PKG-INFO
+-rw-r--r--   0 annli      (501) staff       (20)     7176 2023-05-25 20:34:45.000000 synthedata-0.0.4/README.md
+-rw-r--r--   0 annli      (501) staff       (20)       38 2023-07-31 15:49:56.037053 synthedata-0.0.4/setup.cfg
+-rw-r--r--   0 annli      (501) staff       (20)      662 2023-07-31 15:49:47.000000 synthedata-0.0.4/setup.py
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-31 15:49:56.033922 synthedata-0.0.4/synthedata/
+-rw-r--r--   0 annli      (501) staff       (20)       18 2023-05-25 20:33:58.000000 synthedata-0.0.4/synthedata/__init__.py
+-rw-r--r--   0 annli      (501) staff       (20)    32184 2023-07-31 15:43:32.000000 synthedata-0.0.4/synthedata/data_creator.py
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-31 15:49:56.035673 synthedata-0.0.4/synthedata.egg-info/
+-rw-r--r--   0 annli      (501) staff       (20)     8768 2023-07-31 15:49:55.000000 synthedata-0.0.4/synthedata.egg-info/PKG-INFO
+-rw-r--r--   0 annli      (501) staff       (20)      204 2023-07-31 15:49:56.000000 synthedata-0.0.4/synthedata.egg-info/SOURCES.txt
+-rw-r--r--   0 annli      (501) staff       (20)        1 2023-07-31 15:49:55.000000 synthedata-0.0.4/synthedata.egg-info/dependency_links.txt
+-rw-r--r--   0 annli      (501) staff       (20)       11 2023-07-31 15:49:55.000000 synthedata-0.0.4/synthedata.egg-info/top_level.txt
```

### Comparing `synthedata-0.0.3/PKG-INFO` & `synthedata-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthedata
-Version: 0.0.3
+Version: 0.0.4
 Summary: A synthetic data creator package
 Home-page: https://github.com/fau-syn-data/synthetic-data.git
 Author: BACS_group1
 Author-email: fausyndata@gmail.com
 License: UNKNOWN
 Description: ﻿# Welcome to StackEdit!
```

### Comparing `synthedata-0.0.3/README.md` & `synthedata-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `synthedata-0.0.3/setup.py` & `synthedata-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="synthedata",
-    version="0.0.3",
+    version="0.0.4",
     author="BACS_group1",
     author_email="fausyndata@gmail.com",
     description="A synthetic data creator package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fau-syn-data/synthetic-data.git",
     #packages=setuptools.find_packages(),
```

### Comparing `synthedata-0.0.3/synthedata/datacreator.py` & `synthedata-0.0.4/synthedata/data_creator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import random
 import math
-from typing import Callable, Union, Optional
+from typing import Callable, Union, Optional, Literal
 
 # for graph plots
 import re
 import graphviz as gv
 # for trackin gthe ground truth functions of the variables
 import inspect
 
@@ -14,152 +14,188 @@
 import warnings
 
 # for adding outliers
 from scipy.stats import pareto
 
 # for imputing NA values
 from pandas.api.types import is_numeric_dtype
-from sklearn.impute import SimpleImputer
 
 
-def add_noise(n, mean = 0,sd =1):
-    return np.random.normal(loc = mean, scale = sd, size= n)
+# possible extension: other noise functions e.g. uniformly distributed, some sort of noise for categorical values
+def add_noise(n, mean=0, sd=1):
+    '''This function simply gives back random numbers. It can be used in the DataCreator class to add noise.
+    The strength is controlled by the sd where mean only determines the location of the normal distribution.'''
+    return np.random.normal(loc = mean, scale = sd, size = n)
 
 # possible extensions: keep exactly the same data type e.g. int as input
 def add_na(vec, n=None, share=0.05):
+    '''This function adds None values to a series of values. The number of None entries can be controlled by n or alternatively the relative share.'''
+    # the input series gets copied
     result = vec.copy()
+    # if no fixed number of None values was input then the share is taken to calculate an absolute number
     if n is None:
         n = math.ceil(share * len(vec))
+    # a list of n indexes is chosen randomly without replacement
     rep = list(np.random.choice(a=range(0,len(vec)), size=n, replace=False))
+    # the values at the chosen indexes get replaced with None
     for i in rep:
         result[i] = None
+    # the transformed series gets returned
     return result
 
 # possible extensions:
 # keep exactly the same data type as input e.g. int
 # pass boundries e.g. only positive value
 def add_outlier(vec, n=None, share=0.01):
+    '''This funciton adds outlier values to a secries of values. The number of None entries can be controlled by n or alternatively the relative share.'''
+    # the input series gets copied
     result = vec.copy()
+    # the interquartile range of the vector gets calculated
     iqr = np.subtract(*np.nanpercentile(vec, [75, 25]))
+    # if no fixed number of None values was input then the share is taken to calculate an absolute number
     if n is None:
         n = math.ceil(share * len(vec))
+    # a list of n indexes is chosen randomly without replacement
     rep = list(np.random.choice(a=range(0,len(vec)), size=n, replace=False))
+    # For each of the chosen index there is a 50-50 chance to have a random outlier below the the 1. quartile - 1.5*iqr or above the 3. quartile + 1-5*iqr.
+    # This corresponds to values outside the whiskers of a boxplot.
+    # The exact value is a random number following a shifted Pareto distribution because this distribution is commonly used to model extreme values.
     for i in rep:
         result[i] = np.random.choice([
-            np.nanpercentile(vec, 25) - pareto.rvs(1, loc=iqr),
-            np.nanpercentile(vec, 75) + pareto.rvs(1, loc=iqr)
+            np.nanpercentile(vec, 25) - pareto.rvs(1, loc=1.5*iqr),
+            np.nanpercentile(vec, 75) + pareto.rvs(1, loc=1.5*iqr)
         ])
+    # the transformed series gets returned
     return result
 
 def target_helper(features_for_target, fun_chain, fun_args, mapping=None):
+    '''This funciton executes the iterable fun_chain for each item of features_for_target.'''
     val = None
-    # print(features_for_target)
-    # print(list(fun_chain.keys()))
-    # print(fun_args)
     for i in range(len(features_for_target)):
         col_name = features_for_target[i].name
-        # print(col_name)
-
+        # categorical columns need a mapping to numerical values that gets passed to this function and applied in the if statement below
         if col_name in mapping:
             feature = features_for_target[i].map(mapping[col_name]).astype("float")
         else:
             feature = features_for_target[i]
+        # the feature is being scale to be between 0 and 1
         if min(feature) == max(feature):
             scaled_feature = pd.Series([1.0] * len(feature))
         else:
-            # feature = (feature - np.mean(feature)) / np.std(feature)
             scaled_feature = (feature - min(feature)) / (max(feature) - min(feature))
+        # if it is not the first step of the iteration the previous result gets added to the function arguments as well as the scaled feature and the other arguments
         if val is not None:
             vars = [val, scaled_feature, fun_args[col_name]]
         else:
             vars = [scaled_feature, fun_args[col_name]]
+        # the i-th iteration step is executed with the current set of arguments
         val = fun_chain[list(fun_chain.keys())[i]](*vars).replace(np.Inf, np.nan)
-    # print(list(val))
     return list(val)
 
 
 
 class DataCreator:
+    '''The DataCreator class is wrapper for a pandas dataframe. Its main advantage is that it saves the interdependencies of columns when they get generated.
+    With it also come various functions to generate synthetic data and visualize the dependencies.
+    '''
     def __init__(self, my_df=None):
+        '''The DataCreator class also allows pandas dataframes as input to add new columns to them.
+        Alternatively, a new dataframe gets created on initialization as well as the dependency dictionary and the ground truth dictionary.'''
         if my_df is None:
             self.df = pd.DataFrame()
         else:
             self.df = my_df
         self.dep_dict = {}
         self.ground_truth = {}
 
     def generate_name(self):
-        temp = "col" + str(len(self.df.columns) + 1)
+        '''This function creates generic column names that are not yet used in the dataframe.'''
+        temp = 'col' + str(len(self.df.columns) + 1)
         i = 2
         while temp in self.df.columns.values.tolist():
-            temp = "col" + str(len(self.df.columns) + i)
+            temp = 'col' + str(len(self.df.columns) + i)
+            i += 1
         return temp
 
+    def binarize_column(self, column_name, limit):
+        '''This function binarizes the column of the dataframe based on the input limit.'''
+        self.df[column_name]=(self.df[column_name] < limit).astype(int)
+
+    def categorize_column(self, column_name, limits):
+        '''This function replaces numerical values in a column with generic categories.
+        The limits set the lower and upper boudaries for the categories. The upper limit of the first category is the lower limit of the second and so on.
+        '''
+        self.df[column_name] = pd.cut(self.df[column_name], bins= limits, labels= ["class_" + str(i + 1) for i in range(len(limits) - 1)] )
+        
     def add_var(self, var_name:str, data_generation_function:Callable, features:list or dict=None,
                 noise=True, outliers=True, nas=True):
-        """Adds a variable on basis of a funcion"""
+        '''This function adds a new variable as column to the dataframe of the class instance. It requires a name for the new column and a callable function as input.
+        The features are the column names that are to be interpreted locally relative to the dataframe. They can be passed as a list or as a dictionary.
+        By default None values will be added for any function, noise and outliers will only be added to the new variable if it is a numerical column.'''
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=pd.errors.PerformanceWarning)
             if features is not None and len(features) < data_generation_function.__code__.co_argcount:
                 print("Error - Could not add the variable because too little arguments were given in your dict or list.")
+            # If there is only one column in the dataframe and that gets overwritten then a blank dataframe is created before.
+            # This allows the user to change the number of rows.
             if (len(self.df.columns) == 1) and (features is None or len(features) == 0) and (self.df.columns[0] == var_name):
-                #print(self.df.columns[0])
                 self.df = pd.DataFrame()
-
+            # The input list of dictionary of column names is replaced with its actual values.
             if isinstance(features, dict):
+                # Missing values are imputed to calculate the new column.
+                # For numeric columns the mean is taken. For other columns the first of the most common values is taken.
                 features = {key: (
                     self.df[value].fillna(self.df[value].mean()) if is_numeric_dtype(self.df[value])
-                    # else self.df[value].fillna(np.random.choice(self.df[value].mode()))
                     else self.df[value].fillna(self.df[value].mode()[0])
                 ) for key, value in features.items()}
+                # The input function is executed on the basis of the passed columns.
                 self.df[var_name] = data_generation_function(**features)
+                # The names of the columns the newly created column is based on are saved to the dependency dictionary.
                 self.dep_dict[var_name] = [value.name for value in features.values()]
             if isinstance(features, list):
-                # Replace var names with var values
                 features = [(
                     self.df[var].fillna(self.df[var].mean()) if is_numeric_dtype(self.df[var])
-                    # else self.df[var].fillna(np.random.choice(self.df[var].mode()))
                     else self.df[var].fillna(self.df[var].mode()[0])
                 ) for var in features]
                 self.df[var_name] = data_generation_function(*features)
                 self.dep_dict[var_name] = [value.name for value in features]
             if features is None:
                 self.df[var_name] = data_generation_function()
                 self.dep_dict[var_name] = []
-
+            # For numerical columns and if not opted out noise and outliers get added to the new column.
             if all(isinstance(e, (int, float)) for e in self.df[var_name]):
                 if noise==True:
                     self.df[var_name] += add_noise(len(self.df.index),
                                                    sd=np.subtract(*np.nanpercentile(self.df[var_name], [60, 40])))
                 if outliers==True:
                     self.df[var_name] = add_outlier(list(self.df[var_name]))
+            # If not opted out None values get added to the new column.
             if nas==True:
                 self.df[var_name] = add_na(list(self.df[var_name]))
 
             return self
 
-    def return_call(self):
-        return self.call_str + ".create_df()\n"
 
     def extract_dependencies(self):
-
+        '''Extracts the dependencies of the various columns and assigns the respective levels to them. Exports the levels for the graph visualization.'''
         features = [{"name": name, "level": 0, "depends_on": depends_on} for name, depends_on in self.dep_dict.items()]
         # Assign levels to the features based on dependencies
         for feature in features:
             level = 0
             for dependency in feature["depends_on"]:
                 dependency_level = next((f["level"] for f in features if f["name"] == dependency), 0)
                 level = max(level, dependency_level + 1)
             feature["level"] = level
 
         # Sort the features based on their levels
         features = sorted(features, key=lambda f: f["level"])
         return features
 
     def draw_graph(self):
+        '''Exports a graph file and a .png visualization of the dependencies between different columns in the dataframe of the class instance.'''
         features = self.extract_dependencies()
         # Creates a new Digraph object
         graph = gv.Digraph(format='png', graph_attr={'rankdir': 'LR'}) # LR: left-to-right (direction of graph)
         levels = {}
 
         # Adds the feature to the dictionary of keys
         # Adds a node to the graph for the feature
@@ -175,346 +211,332 @@
             for feature in features:
                 for dependency in feature.get("depends_on", []):
                     graph.edge(dependency, feature["name"])
 
         graph.view()
 
     def check_inputs(self, n:int=None, var_name:str=None):
+        '''Replaces the None values of n and var_name with default values. For the row number n the current length of the dataframe is used or 10000 on initialization.
+        Missing variable names are replaced with generic column names.'''
         if n is None:
             n = size=len(self.df.index)
             if n == 0:
                 n = 10000
         if var_name is None:
             var_name = self.generate_name()
         return n, var_name
 
-    def add_nominal(self, n:int=None, var_name:str=None, topic:str = "gender"):
+    def add_nominal(self, n:int=None, var_name:str=None, topic: Literal["gender"] = "gender"):
+        '''Adds a nominal column to the dataframe. So far only a distribution for gender is implemented.
+        Possible extensions include e.g., generic nominal values, race distribution.'''
         n, var_name = self.check_inputs(n, var_name)
         if topic=="gender":
-            # print("WIP")
-            # self.df[var_name] = np.random.choice(['male','female', 'diverse'], len(self.df.index), p=[0.45, 0.45, 0.1])
             return self.add_var(var_name, lambda: np.random.choice(['male','female', 'diverse'], n, p=[0.45, 0.45, 0.1]), [])
         else: return self
 
-    def add_ordinal(self, n:int=None, var_name:str=None, topic:str = "grades"):
+    def add_ordinal(self, n:int=None, var_name:str=None, topic: Literal["grades"] = "grades"):
+        '''Adds an ordinal column to the dataframe. So far only a distribution for grades is implemented.'''        
         n, var_name = self.check_inputs(n, var_name)
         if topic=="grades":
-            # print("WIP")
             return self.add_var(var_name, lambda:
                                 np.clip(
                                     np.around(
                                         np.random.normal(loc=2.5, scale=1, size=n)
                                         ), 1, 6).astype(int),
                                 [])
         else: return self
 
 
-    def add_interval(self, n:int=None, var_name:str=None, topic:str = "IQ"):
+    def add_interval(self, n:int=None, var_name:str=None, topic: Literal["IQ"] = "IQ"):
+        '''Adds an interval column to the dataframe. So far only a distribution for IQ is implemented.'''        
         n, var_name = self.check_inputs(n, var_name)
         if topic=="IQ":
-            # print("WIP")
             return self.add_var(var_name, lambda:
                                 np.clip(
                                     np.around(
                                         np.random.normal(loc=100, scale=15, size=n)
                                         ), 10, 250).astype(int),
                                 [])
         else: return self
 
-    def add_ratio(self, n:int=None, var_name:str=None, topic:str = "revenue"):
+    def add_ratio(self, n:int=None, var_name:str=None, topic: Literal["revenue"] = "revenue"):
+        '''Adds a ratio column to the dataframe. So far only a distribution for revenue is implemented.'''        
         n, var_name = self.check_inputs(n, var_name)
         if topic=="revenue":
-            # print("WIP")
             return self.add_var(var_name, lambda:
                                 np.clip(
                                   np.around(
                                         np.random.lognormal(np.log(1000000.00), 0.75, size=n), 2
                                         ), 0.00, 572754000000.00),
                                 [])
         else: return self
 
     def gen_target(self, var_name="target", dependency_rate = 0.1, mandatory_features = [], bias = []):
+        '''Generates the target and biased target column for the datafame.
+        The mandatory features and the features for the bias get passed as list of strings of their respective names.'''
         categorical_mapping = {}
         features_for_target = []
         biased_columns = []
-        # print(features_for_target)
-        # print(mandatory_features)
-        # print(biased_columns)
         features_for_target.clear()
         biased_columns.clear()
         biased_columns.extend(bias)
-
         target_name = var_name
+
+        # get lists of the numerical and categorical columns in the dataframe
         numeric_columns = [col_name for col_name in self.df.select_dtypes(include=np.number).columns if col_name not in [target_name, "biased_" + target_name]]
         categorical_columns = [col_name for col_name in self.df.select_dtypes(include=['object']).columns if col_name not in [target_name, "biased_" + target_name]]
 
-
-        number_of_dependencies = math.ceil(len(numeric_columns + categorical_columns)*dependency_rate)
+        # calculate the number of columns the target will be based on 
+        number_of_dependencies = math.ceil(len(numeric_columns + categorical_columns) * dependency_rate)
         if number_of_dependencies <= 0: number_of_dependencies = 1
-        min = self.df.min(axis=None, numeric_only=True).min()/2
-        max = self.df.max(axis=None, numeric_only=True).max()/2
-        #create numeric values for categorical columns
+
+        # calculate an arbitrary floor and ceiling for imputing categorical values based on the min ad max numerical values present in the whole dataframe
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=FutureWarning)
+            min = self.df.min(axis=None, numeric_only=True).min() + (self.df.max(axis=None, numeric_only=True).max() - self.df.min(axis=None, numeric_only=True).min())/4
+            max = self.df.max(axis=None, numeric_only=True).max() - (self.df.max(axis=None, numeric_only=True).max() - self.df.min(axis=None, numeric_only=True).min())/4
+        # map numeric values to categorical columns
         for col_name in categorical_columns:
             categorical_values = self.df[col_name].unique()
             categorical_mapping[col_name] = {v: random.uniform(min, max) for v in categorical_values}
 
-        #add mandatory features and bias to features_for_target
+        # add mandatory features and bias to features_for_target
         features_for_target.extend(mandatory_features)
         features_for_target.extend(biased_columns)
 
+        # if the dependency rate allowed the taret to be dependent on more columns than are mandatory or bias then random columns get drawn from the dataframe
         if len(features_for_target) < number_of_dependencies:
             features_for_target.extend(
                 np.random.choice([col_name for col_name in numeric_columns + categorical_columns if col_name not in features_for_target],
-                                 size=number_of_dependencies-len(features_for_target), replace=False))
-        random.shuffle(features_for_target)
-        #check if biased_columns is given and add one if there was none given
+                                 size= number_of_dependencies - len(features_for_target), replace=False))
+
+        # check if biased_columns is given and add one if there was none given
         if len(biased_columns) == 0:
             biased_columns.append(np.random.choice(features_for_target))
 
+        # if all features for the target are also bias features then add one other random column to the features for target
+        if len(biased_columns) == len(features_for_target):
+            features_for_target.extend(np.random.choice([col_name for col_name in numeric_columns + categorical_columns if col_name not in features_for_target], size= 1, replace=False))
+            
+        random.shuffle(features_for_target)
+        # initialize the relevant variables for the target function, arguments, and ground truth
         b_fun_chain = {}
         u_fun_chain = {}
         b_fun_args = {}
         u_fun_args = {}
-        # print("this is the BIASed func_chain at start: ")
-        # print(b_fun_chain)
-        # print("unbiased: ")
-        # print(u_fun_chain)
         b_ground_truth = ""
         u_ground_truth = ""
+
+        # the weight for the first variable is random between 0 and 2
         random_weight = np.random.uniform(0, 2.0)
         random_column = features_for_target[0]
-        b_fun_chain["fun_0"] = lambda x0, rw0: x0 * rw0
-        u_fun_chain["fun_0"] = lambda x0, rw0: x0 * rw0
-
 
+        # while the first column contributes to the bias, choose a different column to start with
         i = 0
-        while random_column in biased_columns and i < len(features_for_target)-1:
+        while random_column in biased_columns and i < len(features_for_target) - 1:
             i += 1
             random_column = features_for_target[i]
         if i > 0:
             features_for_target[i] = features_for_target[0]
             features_for_target[0] = random_column
+
+        # set the arguments and update the ground truth function string based on the chosen column and weight
         b_fun_args[random_column] = random_weight
         u_fun_args[random_column] = random_weight
-
         b_ground_truth = "(" + b_ground_truth + str(random_weight) + " * " + random_column + ")"
         u_ground_truth = "(" + u_ground_truth + str(random_weight) + " * " + random_column + ")"
 
+        # save the function for the first component of the target
+        # the function start out independent and only uses the chosen columns and weights when those get passed to the execution
+        b_fun_chain["fun_0"] = lambda x0, rw0: x0 * rw0
+        u_fun_chain["fun_0"] = lambda x0, rw0: x0 * rw0
+
+        # for all the remaining features for the target execute the following
         for l in range(1, len(features_for_target)):
-            var_str = ""
-            random_operation = np.random.choice(["+", "-", "*", "/"])
+            # previously simple operations other than addition were used but that yielded too chaotic values
+            # random_operation = np.random.choice(["+", "-", "*", "/"])
             random_operation = "+"
+            
+            # the weight for any variable is randomly chosen
             random_weight = np.random.uniform(-2.0, 2.0)
             random_column = features_for_target[l]
-            # for m in range(0, l - 1):
-            #   var_str += "x" + str(m) + ", " + "rw" + str(m) + ", "
-            # var_str += "x" + str(l - 1) + ", " + "rw" + str(l - 1)
-            # # print(var_str)
+            
+            # categorical columns are marked as such in the ground truth function string so the user knows that the levels were imputed with random numerical values
             if random_column in categorical_columns:
                 b_ground_truth = "(" + b_ground_truth + " " + random_operation + " " + str(random_weight) + " * c_" + random_column + ")"
             else:
                 b_ground_truth = "(" + b_ground_truth + " " + random_operation + " " + str(random_weight) + " * " + random_column + ")"
-            # b_fun_chain["fun_" + str(l)] = eval("lambda " + var_str + ", x" + str(l) +  ", rw" + str(l) +
-            #                                     ": x" + str(l-1) + " " +
-            #                                     random_operation + " x" + str(l) + " * rw" + str(l))
+            
+            # the function is stored based on dynamic function strings
             b_fun_chain["fun_" + str(l)] = eval("lambda intercept, x, rw: intercept " + random_operation + " [el * rw for el in x]")
             b_fun_args[random_column] = random_weight
 
+            # if the column is not part of the biased columns then it also gets added to the unbiased target usind the same steps
             if features_for_target[l] not in biased_columns:
                 n = len(u_fun_chain.keys())
-                # print(n)
-                var_str = ', '.join(u_fun_chain[list(u_fun_chain.keys())[-1]].__code__.co_varnames)
-                # print("unbiased" + u_fun_chain[list(u_fun_chain.keys())[-1]].__code__.co_varnames[-2])
                 if random_column in categorical_columns:
                     u_ground_truth = "(" + u_ground_truth + " " + random_operation + " " + str(random_weight) + " * c_" + random_column + ")"
                 else:
                     u_ground_truth = "(" + u_ground_truth + " " + random_operation + " " + str(random_weight) + " * " + random_column + ")"
-                # u_fun_chain["fun_" + str(n)] = eval("lambda " + var_str + ", x" + str(n) +  ", rw" + str(n) +
-                #                                 ": x" + str(n-1) + " " +
-                #                                 random_operation + " x" + str(n) + " * rw" + str(n))
-
                 u_fun_chain["fun_" + str(n)] = eval("lambda intercept, x, rw: intercept " + random_operation + " [el * rw for el in x]")
                 u_fun_args[random_column] = random_weight
-                # print(u_fun_chain)
-                # print(u_fun_args)
+
+        # store the ground truth functions in the respective dictionary of the instance
         self.ground_truth["biased_target"] = b_ground_truth
         self.ground_truth["unbiased_target"] = u_ground_truth
 
+        # execute the calculation of the target with add_target so that the dependencies get saved properly and the None value imputation gets used
         (self.add_var(target_name, lambda *args: target_helper(args, u_fun_chain, u_fun_args, categorical_mapping), list(u_fun_args.keys()),
                       noise=False, outliers=False, nas=False)
         .add_var("biased_" + target_name, lambda *args: target_helper(args, b_fun_chain, b_fun_args, categorical_mapping), list(b_fun_args.keys()),
                       noise=False, outliers=False, nas=False))
-        
-        structure = "numerical"
-
-        if structure == "categorical":
-            structure_limits = []
-            n_classes = 4
-            bin_min = self.df[target_name].min()
-            bin_max = self.df[target_name].max()
-            structure_limits = [bin_min + (i+1) * (bin_max - bin_min) / n_classes for i in range(n_classes - 1)]
-            # print([bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)])
-            # print(pd.cut(self.df[target_name], bins= [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)], labels= ["class_" + str(i + 1) for i in range(n_classes)] ))
-            self.df[target_name] = pd.cut(self.df[target_name], bins= [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)], labels= ["class_" + str(i + 1) for i in range(n_classes)] )
-            bin_min = self.df["biased_" + target_name].min()
-            bin_max = self.df["biased_" + target_name].max()
-            # print(pd.cut(self.df["biased_" + target_name], bins= [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)], labels= ["class_" + str(i + 1) for i in range(n_classes)] ))
-            self.df["biased_" + target_name] = pd.cut(self.df["biased_" + target_name], bins= [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)], labels= ["class_" + str(i + 1) for i in range(n_classes)] )
-        if structure == "binary":
-            bin_min = self.df[target_name].min()
-            bin_max = self.df[target_name].max()
-            # print(bin_min)
-            # print(bin_max)
-            self.df[target_name] = self.df[target_name].apply(lambda x: 0 if x <= (bin_min + (bin_max - bin_min)/2) else 1) 
-            self.df["biased_" + target_name] = self.df["biased_" + target_name].apply(lambda x: 0 if x <= (bin_min + (bin_max - bin_min)/2) else 1) 
-            # print((                
-                # self.df[target_name].apply(lambda x: 0 if x <= (bin_min + (bin_max - bin_min)/2) else 1) 
-                # self.df[target_name].where(
-                #     self.df[target_name] > (bin_min + (bin_max - bin_min)/2), 1, inplace=True)
-                # .where(
-                #     self.df[target_name] <= (bin_min + (bin_max - bin_min)/2), 0, inplace=True)
-                #.astype('int')
-            # ))
-                  
 
         return(self)
 
 
-    def add_target(self, var_name:str=None, topic:str = "random"):
-        """Ads a target variable based on the specified topic.
-          In the future the relationships of previous variables should be specified to lead to the target."""
+    def add_target(self, var_name:str=None, dependency_rate = 0.2, target_type: Literal["numerical", "binary", "categorical"] = "numerical",
+                   topic:Literal["random", "loan"] = "random", n_classes=2):
+        '''Adds a target variable based on the specified topic. So far there are no real world topics implemented.
+         The loan target was implemented independently for debugging and would need a rework.'''
         n = self.df.shape[0]
         if var_name is None:
             var_name = "target"
 
-        number_of_columns = self.df.shape[1]
-        if topic=="loan":
-            # print("WIP")
-            return self.add_var(var_name, lambda: np.random.choice([0, 1], n, p=[0.76, 0.24]), [])
-        elif topic=="random":
-            # return self.add_var(var_name, lambda: self.generate_target(0.3), [])
-            return self.gen_target(var_name)
-        else: return self
+        # number_of_columns = self.df.shape[1]
+        if topic=="random":
+            self.gen_target(var_name, dependency_rate)
+        elif topic=="loan":
+            self.add_var(var_name, lambda: np.random.choice([0, 1], n, p=[0.76, 0.24]), [])
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=FutureWarning)
+            # if the target should be binary then the middle of the numerical results is used as a limit to 0-1 encode the target columns
+            # the unbiased dataset resuses the same limit
+            if target_type == "binary":
+                self.binarize_column(var_name, (self.df[var_name].min() + self.df[var_name].max())/2)
+                self.binarize_column("biased_" + var_name, (self.df[var_name].min() + self.df[var_name].max())/2)
+            # if the target should be categorical then equal distance bins get created for the biased dataset
+            # the unbiased dataset resuses the same limits for the classes
+            elif target_type == "categorical":
+                structure_limits = []
+                bin_min = self.df[var_name].min()
+                bin_max = self.df[var_name].max()
+                structure_limits = [bin_min + (i+1) * (bin_max - bin_min) / n_classes for i in range(n_classes - 1)]
+                self.categorize_column(var_name, [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)])
+                bin_min = self.df["biased_" + var_name].min()
+                bin_max = self.df["biased_" + var_name].max()
+                self.categorize_column("biased_" + var_name, [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)])
+
+        return self
+
 
 
 
-    def gen_multi(self, n:int=None, num_cols:int=0, cat_cols:int=0, n_layers:int=None, topic="loan", biased=True, interaction="auto"):
-        """Ads columns based on the number of how many categorical or numerical columns were asked for."""
-        # df_trian, df_unbiased, df_real = datasetCreator(samples=10000, num_cols=6, cat_cols=3, topic="loan", biased=True, interaction="auto")
-        # print("WIP")
+    def gen_multi(self, n:int=None, num_cols:int=0, cat_cols:int=0, n_layers:int=None):
+        '''Adds columns based on the number of how many categorical or numerical columns were asked for.'''
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=FutureWarning)
             n = self.check_inputs(n)[0]
+            # if no number of numerical and categorical columns was specified they are both set to 10
             if num_cols + cat_cols == 0:
                 num_cols = 10
                 cat_cols = 10
+            # if no number of layers is speciefied then it is calculated from the number of iterations in the geometrical series the fit in the number of columns to be created
             if n_layers is None:
                 n_layers = int(math.floor(math.log(num_cols + cat_cols) / math.log(2)))
-            # print(n_layers)
-            # generate the total pool of variables to be generated
-            pool = ["num"]*num_cols + ["cat"]*cat_cols
-
-            # level 1 has half of the remaining columns
+            divisor = 4 - (num_cols + cat_cols) ** (1 / n_layers)
+            # generate the total pool of variable categories to be generated
+            pool = ["num"] * num_cols + ["cat"] * cat_cols
             # save the information about what types of columns should be created in a dictionary
             multi_dict = {}
             # get the names of the previous dataframe to compare to later
             prev_cols = self.df.columns.values.tolist()
+            # for every level/layer of columns the following steps are performed
             for i in range(0, n_layers):
                 # draw randomly from the ramaining types of variables
-                # if the last level would only consist of one variable then it gets added to the previous level
                 if i == n_layers - 1:
                     multi_dict["level_" + str(i)] = list(np.random.choice(a=pool, size=len(pool), replace=False))
                 else:
-                    multi_dict["level_" + str(i)] = list(np.random.choice(a=pool, size=math.ceil(len(pool)/2), replace=False))
+                    multi_dict["level_" + str(i)] = list(np.random.choice(a=pool, size=math.ceil(len(pool)/divisor), replace=False))
+                # for each variable category in the level the following steps get performed
                 for item in multi_dict["level_" + str(i)]:
+                    # one 'cat' or 'num' item gets removed from the overall list of columns to be created
                     pool.remove(item)
-                    # print("Start of createing the variable")
+                    # if it is not level 0 variables then the following steps get performed
                     if i != 0:
+                        # the number of additional dependencies above 1 gets drawn
                         n_rest = np.random.choice(a=[0,1,2,3,4],p=[0.25,0.30,0.25,0.15,0.05])
-                        # print(n_rest)
-                        # print(prev_cols)
-                        # print(np.random.choice(a=prev_cols, size=2))
-                        # print(np.random.choice(a=multi_dict["level_" + str(i-1)]))
+                        # the new column must depend at least on a column from the previous level
                         if n_rest == 0:
                             dep = [np.random.choice(a=multi_dict["level_" + str(i-1)])]
+                        # if there are more dependencies they get drawn from any previous level
                         else:
-                            # print([np.random.choice(a=multi_dict["level_" + str(i-1)])] + [1,2,3,4])
-                            # print(np.random.choice(a=prev_cols, size=n_rest))
                             dep = list(set([np.random.choice(a=multi_dict["level_" + str(i-1)])] + np.random.choice(a=prev_cols, size=n_rest).tolist()))
                         random.shuffle(dep)
+
                         fun_chain = {}
                         fun_args = {}
                         categorical_mapping = {}
 
-                        min = self.df.min(axis=None, numeric_only=True).min()/2
-                        max = self.df.max(axis=None, numeric_only=True).max()/2
-                        # print(self.df[dep[0]].dtype)
+                        # limits for mapping the categorical values to random numerical values get calculated from existing values in the dataframe
+                        min = self.df.min(axis=None, numeric_only=True).min() + (self.df.max(axis=None, numeric_only=True).max() - self.df.min(axis=None, numeric_only=True).min())/4
+                        max = self.df.max(axis=None, numeric_only=True).max() - (self.df.max(axis=None, numeric_only=True).max() - self.df.min(axis=None, numeric_only=True).min())/4
+                        # categorical values get mapped to numerical values
                         if self.df[dep[0]].dtype not in (np.float64, np.int64):
                             categorical_values = self.df[dep[0]].unique().tolist()
                             categorical_mapping[dep[0]] = {v: random.uniform(min, max) for v in categorical_values}
-                            # categorical_mapping[dep[0]] = {v: categorical_values.index(v) + 1 for v in categorical_values}
 
-                        fun_args[dep[0]] = np.random.uniform(-1.0, 1.0) # np.random.normal()
+                        # random weights get drawn and the function is stored for the first dependency
+                        fun_args[dep[0]] = np.random.uniform(-1.0, 1.0)
                         fun_chain[dep[0]] = lambda x, rw: x * rw
-                        # print(dep[0])
-                        # print(fun_args[dep[0]])
 
+                        # if there is more dependencies then the remaining functions and weights get set analogously
                         for dep_var in dep[1:len(dep)]:
-                            # print(dep_var)
-                            fun_args[dep_var] = np.random.uniform(-1.0, 1.0) # np.random.normal()
-                            # print(fun_args[dep_var])
+                            fun_args[dep_var] = np.random.uniform(-1.0, 1.0)
                             if self.df[dep_var].dtype not in (np.float64, np.int64):
                                 categorical_values = self.df[dep_var].unique().tolist()
-                                # {k:i for i,k in enumerate(dictionary.keys())}
                                 categorical_mapping[dep_var] = {v: random.uniform(min, max) for v in categorical_values}
-                                # categorical_mapping[dep_var] = {v: categorical_values.index(v) + 1 for v in categorical_values}
+                            # previously simple operations other than addition were used but that yielded too chaotic values
                             fun_chain[dep_var] = np.random.choice([
                                 lambda intercept, x, rw: intercept + x * rw,
                                 #lambda intercept, x, rw: intercept - x * rw,
                                 #lambda intercept, x, rw: intercept * x * rw,
                                 #lambda intercept, x, rw: np.divide(intercept, x * rw, out=np.zeros_like(intercept), where=intercept!=0)
                                 #np.divide(a, b, out=np.zeros_like(a), where=b!=0)
                             ])
-                        
-                        # print(fun_chain)
+
                         temp_name = self.generate_name()
-                        # print("creating new variable: " + temp_name)
-                        # print(categorical_mapping)
+                        # the column gets created based on the function chain and weights
                         self.add_var(temp_name, lambda *args: target_helper(args, fun_chain, fun_args, categorical_mapping), dep,
                           noise=False, outliers=False, nas=False)
-                        
-                        # for categorical values transform to 0-1 encoding
+
+                        # for categorical columns the numerical values get binned into classes
                         if item =="cat":
                               structure_limits = []
-                              n_classes = 4
+                              # the number of classes gets drawn randomly between 2 and 6
+                              n_classes = np.random.choice(a=[2,3,4,5,6])
                               bin_min = self.df[temp_name].min()
                               bin_max = self.df[temp_name].max()
                               structure_limits = [bin_min + (i+1) * (bin_max - bin_min) / n_classes for i in range(n_classes - 1)]
-                              # print([bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)])
-                              # print(pd.cut(self.df[temp_name], bins= [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)], labels= ["class_" + str(i + 1) for i in range(n_classes)] ))
-                              self.df[temp_name] = pd.cut(self.df[temp_name], bins= [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)], labels= ["class_" + str(i + 1) for i in range(n_classes)] )
-
+                              self.categorize_column(temp_name, [bin_min - abs(bin_max)] + structure_limits + [bin_max + abs(bin_min)])
 
+                    # if it is the first level of variables they get created from independent random distributions
                     else:
                         if item == "num":
                             self.add_ratio(n)
                         if item == "cat":
                             self.add_nominal(n)
-                # print("level_"+ str(i) + " num: " + str(multi_dict["level_" + str(i)].count("num")) + "\nlevel_"+ str(i) + " cat: " + str(multi_dict["level_" + str(i)].count("cat"))
-                #     + "\npool num: " + str(pool.count("num")) + "\npool cat: " + str(pool.count("cat")))
+                # the new column names get added to the dictionary and the previous colums get extended by the new column names
                 multi_dict["level_" + str(i)] = list(set(self.df.columns.values.tolist()).difference(prev_cols))
                 prev_cols += multi_dict["level_" + str(i)]
-                # print(multi_dict["level_" + str(i)])
-                # print(pool)
 
-            self.add_target(topic="random")
             return self
 
     def get_ground_truth(self):
+        '''Prints the ground truth funtions for the target variables of the class instance.'''
         print(
             "The biased ground truth function is given by: " + self.ground_truth["biased_target"] + "\n" +
             "The unbiased ground truth function is given by: " + self.ground_truth["unbiased_target"] + "\n"
         )
 
-
     def create_df(self):
+        '''Returns a copy of the generated dataframe.'''
         return self.df.copy()
```

### Comparing `synthedata-0.0.3/synthedata.egg-info/PKG-INFO` & `synthedata-0.0.4/synthedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthedata
-Version: 0.0.3
+Version: 0.0.4
 Summary: A synthetic data creator package
 Home-page: https://github.com/fau-syn-data/synthetic-data.git
 Author: BACS_group1
 Author-email: fausyndata@gmail.com
 License: UNKNOWN
 Description: ﻿# Welcome to StackEdit!
```

