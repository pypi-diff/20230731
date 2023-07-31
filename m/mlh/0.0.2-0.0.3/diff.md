# Comparing `tmp/mlh-0.0.2.tar.gz` & `tmp/mlh-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlh-0.0.2.tar", last modified: Thu Mar  7 11:54:19 2019, max compression
+gzip compressed data, was "mlh-0.0.3.tar", last modified: Mon Jul 31 17:08:31 2023, max compression
```

## Comparing `mlh-0.0.2.tar` & `mlh-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxrwxrwx   0        0        0        0 2019-03-07 11:54:19.000000 mlh-0.0.2/
-drwxrwxrwx   0        0        0        0 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh/
--rw-rw-rw-   0        0        0    17290 2019-03-07 11:49:59.000000 mlh-0.0.2/mlh/support.py
--rw-rw-rw-   0        0        0    21460 2019-03-05 10:51:55.000000 mlh-0.0.2/mlh/woe.py
--rw-rw-rw-   0        0        0       52 2019-03-06 10:00:43.000000 mlh-0.0.2/mlh/__init__.py
-drwxrwxrwx   0        0        0        0 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh.egg-info/
--rw-rw-rw-   0        0        0        1 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3933 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       61 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      194 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2019-03-07 11:54:19.000000 mlh-0.0.2/mlh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3933 2019-03-07 11:54:19.000000 mlh-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2019-03-05 10:40:51.000000 mlh-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2019-03-07 11:54:19.000000 mlh-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      821 2019-03-07 11:52:36.000000 mlh-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:08:31.836799 mlh-0.0.3/
+-rw-rw-rw-   0        0        0     3157 2023-07-31 17:08:31.836799 mlh-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-07-31 16:46:11.000000 mlh-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 17:08:31.836799 mlh-0.0.3/mlh.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-07-31 17:08:31.000000 mlh-0.0.3/mlh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-07-31 17:08:31.000000 mlh-0.0.3/mlh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:08:31.000000 mlh-0.0.3/mlh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-07-31 17:08:31.000000 mlh-0.0.3/mlh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 17:08:31.000000 mlh-0.0.3/mlh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 17:08:31.836799 mlh-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-07-31 17:02:31.000000 mlh-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mlh-0.0.2/README.md` & `mlh-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# Machine Learning Helper
-
-This package usage multiple algorithms and parameters to accomodate different set of use cases to help in creating multiple machine learning algorithms.
-
-## 1.0 woe (Weight of Evidence):
-This function will help to calculate Weight of Evidence and Information Value, the charts can be displayed and coarse classing can also be done.
-
-### 1.1 Parameters:
-------------------------------------------------------------
-* **max_bin**: int
-    Maximum number of bins for numeric variables. The default is 10
-* **iv_threshold**: float
-    Threshold value for Information Value. Variables with higher than threshold will be considered for transformation
-* **ignore_threshold**: Boolean
-    This parameter controls whether the defined threshold should be considered or ignored. The default is 'True'
-
-------------------------------------------------------------
-### 1.2 Returns:
-DataFrame having weight of evidence of each column along with the target variable
-
-
-------------------------------------------------------------
-### 1.3 Approach:
-
-1. Create an instance of woe
-     my_woe = woe()
-
-2. Call fit method on the defined object by passing on dataframe and the target variable name
-     my_woe.fit(df,target)
-
-3. Call the transform method
-    transformed_df = my_woe.transform()
-
-------------------------------------------------------------
-## Example
-
-### Create Sample DataFrame
-```python
-from mlh import woe
-import pandas as pd
-import numpy as np
-import random
-
-seed=1456
-np.random.seed(seed)
-random.seed(seed)
-```
-```python
-rows = 1000
-```
-```python
-y = random.choices([0,1],k=rows,weights=[.7,.3])
-```
-```python
-x1 = random.choices(np.arange(20,40),k=rows)
-x2 = np.random.randint(1000,2000,size=rows)
-x3 = random.choices(np.arange(1,100),k=rows)
-x4 = random.choices(['m','f','u'],k=rows)
-x5 = random.choices(['a','b','c','d','e','f','g','h'],k=rows)
-```
-```python
-df = pd.DataFrame({'y':y,'x1':x1,'x2':x2,'x3':x3,'x4':x4,'x5':x5})
-```
-```python
-df.head()
-```
-### Fitting and prediction
-
-**Create Instance of Weight of Evidence Package**
-```python
-my_woe = woe()
-```
-**Fit the data with created instance**
-```python
-my_woe.fit(df,'y')
-```
-**Display the relevant charts**
-```python
-my_woe.getWoeCharts()
-```
-**Merge values of X3 Variable at 1 and 2 indices using the Weight of Evidence chart from the first Iteration**
-```python
-my_woe.reset_woe(2,(1,2),1)
-```
-**Get latest Iteration Information Value**
-```python
-my_woe.get_IV()
-```
-**Replace the original values in the Dataframe with Weight of Evidence**
-```python
-transformed_df = my_woe.transform()
-```
+# Machine Learning Helper
+
+This package usage multiple algorithms and parameters to accomodate different set of use cases to help in creating multiple machine learning algorithms.
+
+## 1.0 woe (Weight of Evidence):
+This function will help to calculate Weight of Evidence and Information Value, the charts can be displayed and coarse classing can also be done.
+
+### 1.1 Parameters:
+------------------------------------------------------------
+* **max_bin**: int
+    Maximum number of bins for numeric variables. The default is 10
+* **iv_threshold**: float
+    Threshold value for Information Value. Variables with higher than threshold will be considered for transformation
+* **ignore_threshold**: Boolean
+    This parameter controls whether the defined threshold should be considered or ignored. The default is 'True'
+
+------------------------------------------------------------
+### 1.2 Returns:
+DataFrame having weight of evidence of each column along with the target variable
+
+
+------------------------------------------------------------
+### 1.3 Approach:
+
+1. Create an instance of woe
+     my_woe = woe()
+
+2. Call fit method on the defined object by passing on dataframe and the target variable name
+     my_woe.fit(df,target)
+
+3. Call the transform method
+    transformed_df = my_woe.transform()
+
+------------------------------------------------------------
+## Example
+
+### Create Sample DataFrame
+```python
+from mlh import woe
+import pandas as pd
+import numpy as np
+import random
+
+seed=1456
+np.random.seed(seed)
+random.seed(seed)
+```
+```python
+rows = 1000
+```
+```python
+y = random.choices([0,1],k=rows,weights=[.7,.3])
+```
+```python
+x1 = random.choices(np.arange(20,40),k=rows)
+x2 = np.random.randint(1000,2000,size=rows)
+x3 = random.choices(np.arange(1,100),k=rows)
+x4 = random.choices(['m','f','u'],k=rows)
+x5 = random.choices(['a','b','c','d','e','f','g','h'],k=rows)
+```
+```python
+df = pd.DataFrame({'y':y,'x1':x1,'x2':x2,'x3':x3,'x4':x4,'x5':x5})
+```
+```python
+df.head()
+```
+### Fitting and prediction
+
+**Create Instance of Weight of Evidence Package**
+```python
+my_woe = woe()
+```
+**Fit the data with created instance**
+```python
+my_woe.fit(df,'y')
+```
+**Display the relevant charts**
+```python
+my_woe.getWoeCharts()
+```
+**Merge values of X3 Variable at 1 and 2 indices using the Weight of Evidence chart from the first Iteration**
+```python
+my_woe.reset_woe(2,(1,2),1)
+```
+**Get latest Iteration Information Value**
+```python
+my_woe.get_IV()
+```
+**Replace the original values in the Dataframe with Weight of Evidence**
+```python
+transformed_df = my_woe.transform()
+```
```

